SNMP v3 Operations with C#
==========================

This page shows you how to perform SNMP v3 operations. Basic SNMP v3
operations (GET, SET and so on) are translated to C# SNMP function calls.

Background
----------
SNMP v1 and v2c were designed to be simple, but one significant issue of them
is security. It is very hard to hide community strings from sniffers, and also
difficult to set access control on entities.

IETF recognized those security challenges and finalized SNMP v3 RFC documents
in 2004, which uses a new design to address the concerns. The changes were so
huge from message format to agent/manager details, so C# SNMP Library has to
expose a different styles of APIs enabling developers to perform v3 operations.

Discovery Process
-----------------
SNMP v3 defines a unique discovery process in RFC 3414. For example, before an
SNMP agent responds to a manager the two must interchange information such as
time stamp, engine ID and so on.

.. code-block:: csharp

  Discovery discovery = Messenger.GetNextDiscovery(SnmpType.GetRequestPdu);
  ReportMessage report = discovery.GetResponse(60000, new IPEndPoint(IPAddress.Parse("192.168.1.2"), 161));

Above we perform such a discovery process by sending out a ``GetRequestPdu``
type of discovery message, and the agent replies with a ``ReportMessage``
which we can reuse later to construct a valid request.

User Credentials
----------------
SNMP v3 requires user credentials to be passed on in each requests, so we need
to prepare that information ahead of time.

.. code-block:: csharp

  var auth = new SHA1AuthenticationProvider(new OctetString("myauthenticationpassword"));
  var priv = new DESPrivacyProvider(new OctetString("myprivacypassword"), auth);

Assume the agent requires both authentication (SHA-1) and privacy (DES)
protection, then above we create a single provider that embeds both passwords.

GET Operation
-------------
The following code shows how to send an SNMP v3 GET message to an agent
located at ``192.168.1.2`` and query on OID ``1.3.6.1.2.1.1.1.0``,

.. code-block:: csharp

  GetRequestMessage request = new GetRequestMessage(VersionCode.V3, Messenger.NextMessageId, Messenger.NextRequestId, new OctetString("myname"), new List<Variable>{new Variable(new ObjectIdentifier("1.3.6.1.2.1.1.1.0"))}, priv, Messenger.MaxMessageSize, report);
  ISnmpMessage reply = request.GetResponse(60000, new IPEndPoint(IPAddress.Parse("192.168.1.2"), 161));
  if (reply.Pdu().ErrorStatus.ToInt32() != 0) // != ErrorCode.NoError
  {
      throw ErrorException.Create(
          "error in response",
          IPAddress.Parse("192.168.1.2"),
          reply);
  }

The reply object usually contains the response message we expect. By accessing
``reply.Pdu().Variables`` we can see what data are returned.

SET Operation
-------------
The following code shows how to send an SNMP v3 SET message to an SNMP agent
located at ``192.168.1.2`` and set the value of OID ``1.3.6.1.2.1.1.6.0`` to
``"Shanghai"``,

.. code-block:: csharp

  SetRequestMessage request = new SetRequestMessage(VersionCode.V3, Messenger.NextMessageId, Messenger.NextRequestId, new OctetString("myname"), new List<Variable>{new Variable(new ObjectIdentifier("1.3.6.1.2.1.1.1.0"), new OctetString("Shanghai"))}, priv, Messenger.MaxMessageSize, report);
  ISnmpMessage reply = request.GetResponse(60000, new IPEndPoint(IPAddress.Parse("192.168.1.2"), 161));
  if (reply.Pdu().ErrorStatus.ToInt32() != 0) // != ErrorCode.NoError
  {
      throw ErrorException.Create(
          "error in response",
          IPAddress.Parse("192.168.1.2"),
          reply);
  }

GET-BULK Operation
------------------
The following code shows how to send an SNMP v3 GET-BULK message to an SNMP
agent located at ``192.168.1.2`` and query on OID ``1.3.6.1.2.1.1.1.0``,

.. code-block:: csharp

  GetBulkRequestMessage request = new GetBulkRequestMessage(VersionCode.V3, Messenger.NextMessageId, Messenger.NextRequestId, new OctetString("myname"), 0, 10, new List<Variable>{new Variable(new ObjectIdentifier("1.3.6.1.2.1.1.1.0"))}, priv, Messenger.MaxMessageSize, report);
  ISnmpMessage reply = request.GetResponse(60000, new IPEndPoint(IPAddress.Parse("192.168.1.2"), 161));
  if (reply.Pdu().ErrorStatus.ToInt32() != 0) // != ErrorCode.NoError
  {
      throw ErrorException.Create(
          "error in response",
          IPAddress.Parse("192.168.1.2"),
          reply);
  }

  var result = reply.Pdu().Variables;

WALK Operation
--------------
The following code shows how to perform v3 WALK on an SNMP agent located at
``192.168.1.2`` starting at ``1.3.6.1.2.1.1``,

.. code-block:: csharp

  var result = new List<Variable>();
  Messenger.BulkWalk(VersionCode.V3, 
                    new IPEndPoint(IPAddress.Parse("192.168.1.2"), 161), 
                    new OctetString("public"),
                    OctetString.Empty, // context name
                    new ObjectIdentifier("1.3.6.1.2.1.1"),
                    result,
                    60000,
                    10,
                    WalkMode.WithinSubtree,
                    priv,
                    report);

INFORM Operation
----------------
.. note:: Comparing to sending TRAP v2 messages, it is common to send INFORM
   messages.

The following code shows how to send an INFORM message to an SNMP manager/trap
listener located at ``192.168.1.2``,

.. code-block:: csharp

  Messenger.SendInform(
    0,
    VersionCode.V3,
    new IPEndPoint(IPAddress.Parse("192.168.1.2"), 162),
    new OctetString("neither"),
    new ObjectIdentifier(new uint[] { 1, 3, 6 }),
    0,
    new List<Variable>(),
    2000,
    DefaultPrivacyProvider.DefaultPair,
    report);

TRAP v2 Operation
-----------------
.. note:: TRAP v1 message format is obsolete by TRAP v2. Thus, for SNMP v3
   TRAP operations, you can only use TRAP v2 message format.

The following code shows how to send a TRAP v2 message to an SNMP manager/trap
listener located at ``192.168.1.2``,

.. code-block:: csharp

  var trap = new TrapV2Message(
    VersionCode.V3,
    528732060,
    1905687779,
    new OctetString("neither"),
    new ObjectIdentifier("1.3.6"),
    0,
    new List<Variable>(),
    DefaultPrivacyProvider.DefaultPair,
    0x10000,
    new OctetString(ByteTool.Convert("80001F8880E9630000D61FF449")), // engine ID
    0,
    0);
  trap.Send(new IPEndPoint(IPAddress.Parse("192.168.1.2"), 162));

.. note::

  The TRAP sending/processing steps in SNMP v3 are quite different from other
  message types. Because the TRAP message is sent out by the agent, and will
  not be acknowledged by the manager, the normal discovery process is not
  applicable.

  Instead, who sends out the TRAP v2 message has to reveal the engine ID of
  ``0x80001F8880E9630000D61FF449`` in the message, and the manager has to
  trust the engine ID to process the message according to its configuration.

Next Steps
----------

To help you understand how to use the API provided by C# SNMP Library, there
are sample projects with ready-to-use code you can find in this
`samples repo <https://github.com/lextudio/sharpsnmplib-samples>`_ where more
details are demonstrated.

Besides essential SNMP operations, C# SNMP Library supports many advanced
features, such as manager and agent development. And if you need enterprise MIB
support, you can evaluate and purchase #SNMP Pro. All useful links are shared
in the section below.

Related Resources
-----------------

- :doc:`/tutorials/introduction`
- :doc:`/tutorials/aes`
- :doc:`/tutorials/security-notice`
- :doc:`/samples/agent-development`
- :doc:`/samples/command-line-tools`
- `#SNMP Pro <https://pro.sharpsnmp.com>`_
- :doc:`/tutorials/troubleshooting`
- `The API Reference <https://help.sharpsnmp.com>`_
