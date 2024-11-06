Introduction to C# SNMP Library
===============================

This page shows you the basics about #SNMP, an open source SNMP implementation
for C# and .NET.

Basic SNMP operations (GET, SET and so on) you learn from elsewhere can be
easily translated to C# SNMP function calls.

.. note::

   The equivalent Net-SNMP command line is provided for each operation, so you
   can compare the two.

GET Operation
-------------
The following code shows how to send an SNMP v1 GET message to an SNMP agent
located at ``192.168.1.2`` and query on OID ``1.3.6.1.2.1.1.1.0``,

.. code-block:: csharp

  var result = Messenger.Get(VersionCode.V1,
                             new IPEndPoint(IPAddress.Parse("192.168.1.2"), 161),
                             new OctetString("public"),
                             new List<Variable>{new Variable(new ObjectIdentifier("1.3.6.1.2.1.1.1.0"))},
                             60000);

This operation will time out if no reply is received after 60 seconds (1
minute), and throw an exception (``TimeoutException``). If any error occurs, an
``ErrorException`` can be caught. All C# SNMP exceptions are derived from
``SnmpException``.

The result returned is a list that matches the list of ``Variable`` objects
sent. The ``Variable`` in this list contains the value of the OID.

.. note::

   The equivalent Net-SNMP command line is

   .. code-block:: bash
  
      snmpget -v 1 -c public -t 60 192.168.1.2:161 1.3.6.1.2.1.1.1.0

SET Operation
-------------
The following code shows how to send an SNMP v1 SET message to an SNMP agent
located at ``192.168.1.2`` and set the value of OID ``1.3.6.1.2.1.1.6.0`` to
``"Shanghai"``,

.. code-block:: csharp

  var result = Messenger.Set(VersionCode.V1,
                             new IPEndPoint(IPAddress.Parse("192.168.1.2"), 161),
                             new OctetString("public"),
                             new List<Variable>{new Variable(new ObjectIdentifier("1.3.6.1.2.1.1.6.0"), new OctetString("Shanghai"))},
                             60000);

.. note::

   The equivalent Net-SNMP command line is

   .. code-block:: bash

      snmpset -v 1 -c public -t 60 192.168.1.2:161 1.3.6.1.2.1.1.6.0 s "Shanghai"

GET-NEXT Operation
------------------
The following code shows how to send an SNMP v1 GET-NEXT message to an SNMP
agent located at ``192.168.1.2`` and query on OID ``1.3.6.1.2.1.1.1.0``,

.. code-block:: csharp

  GetNextRequestMessage message = new GetNextRequestMessage(0,
                                                            VersionCode.V1,
                                                            new OctetString("public"),
                                                            new List<Variable>{new Variable(new ObjectIdentifier("1.3.6.1.2.1.1.1.0"))});
  ISnmpMessage response = message.GetResponse(60000, new IPEndPoint(IPAddress.Parse("192.168.1.2"), 161));
  if (response.Pdu().ErrorStatus.ToInt32() != 0)
  {
      throw ErrorException.Create(
          "error in response",
          IPAddress.Parse("192.168.1.2"),
          response);
  }

  var result = response.Pdu().Variables;

.. note::

   The equivalent Net-SNMP command line is

   .. code-block:: bash

      snmpgetnext -v 1 -c public -t 60 192.168.1.2:161 1.3.6.1.2.1.1.1.0

GET-BULK Operation
------------------
The following code shows how to send an SNMP v2 GET-BULK message to an SNMP
agent located at ``192.168.1.2`` and query on OID ``1.3.6.1.2.1.1.1.0``,

.. code-block:: csharp

  GetBulkRequestMessage message = new GetBulkRequestMessage(0,
                                                            VersionCode.V2,
                                                            new OctetString("public"),
                                                            0,
                                                            10,
                                                            new List<Variable>{new Variable(new ObjectIdentifier("1.3.6.1.2.1.1.1.0"))});
  ISnmpMessage response = message.GetResponse(60000, new IPEndPoint(IPAddress.Parse("192.168.1.2"), 161));
  if (response.Pdu().ErrorStatus.ToInt32() != 0)
  {
      throw ErrorException.Create(
          "error in response",
          IPAddress.Parse("192.168.1.2"),
          response);
  }

  var result = response.Pdu().Variables;

.. note::

   The equivalent Net-SNMP command line is

   .. code-block:: bash

      snmpbulkget -v 2c -c public -t 60 -Cn0 -Cr10 192.168.1.2:161 1.3.6.1.2.1.1.1.0

Walk Operation
--------------
Walk is not an atomic operation. That means, it utilizes several GET-NEXT (SNMP
v1 walk) or GET-BULK (v2 and above). The following code shows how to perform
walk on an SNMP agent located at ``192.168.1.2`` starting at ``1.3.6.1.2.1.1``,

.. code-block:: csharp

  var result = new List<Variable>();
  Messenger.Walk(VersionCode.V1,
                 new IPEndPoint(IPAddress.Parse("192.168.1.2"), 161),
                 new OctetString("public"),
                 new ObjectIdentifier("1.3.6.1.2.1.1"),
                 result,
                 60000,
                 WalkMode.WithinSubtree);

.. note::

   The equivalent Net-SNMP command line is

   .. code-block:: bash

      snmpwalk -v 1 -c public -t 60 192.168.1.2:161 1.3.6.1.2.1.1

The result returned contains a list of all available OIDs (as ``Variable``) in
this SNMP agent that under tree node of ``1.3.6.1.2.1.1``.

C# SNMP supports two walk modes, ``Default`` and ``WithinSubtree``. The former
ends the WALK operation at the end of MIB view, while the latter ends at the
end of the subtree of initial OID.

``Messenger.Walk`` is built upon GET-NEXT operations. Note that
``Messenger.BulkWalk`` should be used if the device supports SNMP v2, as it is
built upon GET-BULK operations and provide better performance.

.. code-block:: csharp

  var result = new List<Variable>();
  Messenger.BulkWalk(VersionCode.V2,
                    new IPEndPoint(IPAddress.Parse("192.168.1.2"), 161),
                    new OctetString("public"),
                    null,
                    new ObjectIdentifier("1.3.6.1.2.1.1"),
                    result,
                    60000,
                    10,
                    WalkMode.WithinSubtree,
                    null,
                    null);

.. note::

   The equivalent Net-SNMP command line is

   .. code-block:: bash

      snmpbulkwalk -v 2c -c public -t 60 -Cn0 -Cr10 192.168.1.2:161 1.3.6.1.2.1.1

TRAP Operation
--------------
It is usually an SNMP agent that sends out TRAP messages. The following code
shows how to send an empty SNMP v1 TRAP message from ``192.168.1.2`` to an SNMP
manager located at ``192.168.1.3``,

.. code-block:: csharp

  Messenger.SendTrapV1(new IPEndPoint(IPAddress.Parse("192.168.1.3"), 162),
                      IPAddress.Parse("192.168.1.2"),
                      new OctetString("public"),
                      new ObjectIdentifier("1.3.6.1.2.1.1"),
                      GenericCode.ColdStart,
                      0,
                      0,
                      new List<Variable>());

.. note::

   The equivalent Net-SNMP command line is

   .. code-block:: bash

      snmptrap -v 1 -c public 192.168.1.3:162 1.3.6.1.2.1.1 192.168.1.2 6 0 0

SNMP v2 and above introduces a simplified TRAP v2 message,

.. code-block:: csharp

  Messenger.SendTrapV2(0,
                      VersionCode.V2,
                      new IPEndPoint(IPAddress.Parse("192.168.1.3"), 162),
                      new OctetString("public"),
                      new ObjectIdentifier("1.3.6.1.2.1.1"),
                      0,
                      new List<Variable>());

.. note::

   The equivalent Net-SNMP command line is

   .. code-block:: bash

      snmptrap -v 2c -c public 192.168.1.3:162 "" 1.3.6.1.2.1.1

INFORM Operation
----------------
It is usually an SNMP agent that sends out INFORM messages. The following code
shows how to send an empty INFORM message to an SNMP manager located at
``192.168.1.3``,

.. code-block:: csharp

  Messenger.SendInform(0,
                      VersionCode.V2,
                      new IPEndPoint(IPAddress.Parse("192.168.1.3"), 162),
                      new OctetString("public"),
                      new ObjectIdentifier("1.3.6.1.2.1.1"),
                      0,
                      new List<Variable>(),
                      2000,
                      null,
                      null);

.. note::

   The equivalent Net-SNMP command line is

   .. code-block:: bash

      snmpinform -v 2c -c -t 2 public 192.168.1.3:162 "" 1.3.6.1.2.1.1

The manager should send back a reply to this INFORM message. Otherwise, a
``TimeoutException`` occurs.

.. note:: To help you understand how to use the API provided by C# SNMP Library,
   there are more sample projects you can find in this 
   `samples repo <https://github.com/lextudio/sharpsnmplib-samples>`_.

   Both C# and VB.NET samples are available.

Next Steps
----------

C# SNMP Library supports many advanced features, such as SNMP v3 operations and
manager/agent development. And if you need enterprise MIB support, you can use
#SNMP Pro.

Related Resources
-----------------

- :doc:`/tutorials/v3-operations`
- :doc:`/samples/agent-development`
- :doc:`/samples/command-line-tools`
- `#SNMP Pro <https://pro.sharpsnmp.com>`_
- `The API Reference <https://help.sharpsnmp.com>`_
- :doc:`/tutorials/troubleshooting`
- :doc:`/tutorials/security-notice`
