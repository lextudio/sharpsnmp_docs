Agent Development
=================

This page shows you how the agent sample works.

Dependencies
------------

.. note:: The sample projects have been moved to
   `a new location <https://github.com/lextudio/sharpsnmplib-samples>`_.

When you open snmpd.csproj in Visual Studio (or another IDE), you should first
check what are its references.

.. note:: This package targets multiple platforms.

Facade and Pipeline
-------------------
We no longer need to construct an ``Agent`` object, because that class is too
old to be used. We try to construct an ``SnmpEngine`` object instead.

``SnmpEngine`` is the facade that you should put on top. It is a very complex
class that replaces our old Agent class. To construct it, we need: an
``EngineGroup`` object, which contains all engine global objects; A
``Listener`` object, which monitors incoming SNMP message; An
``SnmpApplicationFactory``, who manages the pipelines.

``SnmpApplicationFactory`` creates new pipelines when its pipeline pool is full
of busy pipelines. The objects we pass to its constructor finally goes into
each pipeline as they are shared among them (at this moment).

A pipeline is in fact an ``SnmpApplication`` object. It has several processing
phases and each phase utilizes a few helper classes, which you can extend.

An SNMP message captured by ``Listener`` will be packaged as an ``SnmpContext``
object. This context object is passed to the pipeline and processed in each
phase to generate a correct response message.

About how to construct instances of each classes, you can refer to snmpd sample
source code.

Pipeline in Details
-------------------
Currently we only have four phases in the pipeline,

* Authentication
* Request handler mapping
* Request handler executing
* Logging request

Authentication
^^^^^^^^^^^^^^
By checking the sample code you can see how the primary membership provider
(``ComposedMembershipProvider``) is created and added into the pipeline. The
request is checked by the provider and dropped if it does not contain a proper
community name.

``ComposedMembershipProvider`` is a special membership provider, who allows you
to support different SNMP versions. If you only target a specific version, you
can use the version specific provider as primary one.

To customize authentication, make use of the existing providers or write your
own.

Request handler mapping
^^^^^^^^^^^^^^^^^^^^^^^
For authenticated message, in this phase it is verified again and mapped to a
message handler.

Message handlers are injected to the pipeline, too. So you can analyze the
sample code to know how many handlers are there already, and how each registers
its interested message (SNMP version and verb).

For example, ``GetV1MessageHandler`` is only interested in v1 GET messages,
while ``GetMessageHandler`` in v2 and v3 GET messages.

Carefully configure the existing handlers, you can achieve different SNMP
engine configurations, so as to meet different requirements. You can write your
own handlers to further customize the pipeline.

Request handler executing
^^^^^^^^^^^^^^^^^^^^^^^^^
Once a message handler is found for the message, in this phase the handler
performs the requested operation and generate a response message.

You should notice that ``*V1MessageHandler`` classes follow RFC 1157
specification to handle v1 messages, while other handler classes follow RFC
3416 to handle v2 and v3 messages.

Logging request
^^^^^^^^^^^^^^^
In this phase the response message is sent back, while the logger logs the
processing into log files.

After phase 4, the pipeline is reused by ``SnmpApplicationFactory`` for future
messages.

We may add an authorization phase to achieve user based authorization, but it
is not yet designed and implemented.

ObjectStore and ISnmpObject
^^^^^^^^^^^^^^^^^^^^^^^^^^^
When a handler tries to do a typical SNMP operation, it looks into the
``ObjectStore`` object to locate the specified object.

Currently we only have a few sample objects created, to test out the pipeline.
You can find them under ``Lextm.SharpSnmpLib.Objects`` namespace.

If you want to write more objects, you can follow our sample ones.

``ObjectStore`` is not yet thread safe, which will be improved in the future.

Performance Tuning
------------------
The SNMP engine is multi-threading by nature. Both the ``ListenerBinding`` and
``SnmpApplication`` instances utilize the default thread pool to handle
requests asynchronously. Thus, it is a must to make sure the thread pool is
optimized before requests come in.

Before calling ``SnmpEngine.Start``, it is recommended that the below code to
be executed, which sets the minimal worker thread count to a suitable value.

.. code-block:: csharp

  int minWorker, minIOC;
  // Get the current settings.
  ThreadPool.GetMinThreads(out minWorker, out minIOC);
  var threads = engine.Listener.Bindings.Count;
  ThreadPool.SetMinThreads(threads + 1, minIOC);

If not tuned, the very first request to this agent will cost extra time
(noticeably several seconds if there are too many bindings), as the operating
system needs to create new threads before putting them into the thread pool.

Limitation Explained
--------------------
You should take a look at ``MainForm.cs`` and read what extra lines are
required to configure the ``SnmpEngine`` object, how to start and stop it. SNMP
tables can be quite complex, while this sample only shows simple tables such as
``IfTable`` for simplicity.

As the sample is released under MIT/X11 license. The snmptrapd sample also uses
the pipeline to handle trap messages, and once you are familiar with snmpd, you
can switch to it to learn how to construct a browser side pipeline accordingly.

This sample is provided to demonstrate how the library might be used. If you
want to build a full feature SNMP agent based on this sample, then many changes
(multi-threading and security related) are mandate.

Related Resources
-----------------

- :doc:`/tutorials/introduction`
- :doc:`/samples/command-line-tools`
- :doc:`/getting-started/license-notice`
