SnmpDispatcher Class
====================

.. dn:class:: DotNetSnmp.Client.SnmpDispatcher

   Coordinates SNMP Protocol Data Unit (PDU) transmission and reception across all SNMP versions (v1, v2c, v3).

   .. code-block:: csharp

      public class SnmpDispatcher : ISnmpDispatcher

**Namespace:** ``DotNetSnmp.Client``

**Inheritance:** Object → ``SnmpDispatcher``

**Source:** `SharpSnmpLib/Dispatch/SnmpDispatcher.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Dispatch/SnmpDispatcher.cs#L35>`__

Constructors
------------

SnmpDispatcher(ILogger<SnmpDispatcher>?)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Client.SnmpDispatcher..ctor(Microsoft.Extensions.Logging.ILogger{DotNetSnmp.Client.SnmpDispatcher})

   Initializes a new instance of :dn:cls:``~DotNetSnmp.Client.SnmpDispatcher``.

   .. code-block:: csharp

      public SnmpDispatcher(ILogger<SnmpDispatcher>? logger = null)

   :param logger: Optional logger for diagnostic output. If null, logging is disabled.
   :type logger: ``ILogger<SnmpDispatcher>``

**Source:** `SharpSnmpLib/Dispatch/SnmpDispatcher.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Dispatch/SnmpDispatcher.cs#L49>`__

Methods
-------

SendPdu(ISnmpTransport, ISnmpTarget, IPEndPoint, IScope, Boolean, CancellationToken)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Client.SnmpDispatcher.SendPdu(DotNetSnmp.Transport.ISnmpTransport,DotNetSnmp.Transport.Targets.ISnmpTarget,System.Net.IPEndPoint,DotNetSnmp.Common.Definitions.IScope,System.Boolean,System.Threading.CancellationToken)

   Sends an SNMP PDU to the target and optionally waits for the response.

   .. code-block:: csharp

      public ValueTask<IScope> SendPdu(ISnmpTransport transport, ISnmpTarget target, IPEndPoint targetAddress, IScope scope, bool expectResponse = true, CancellationToken cancellationToken = default(CancellationToken))

   :param transport: The network transport layer (e.g., UDP) used to send/receive data.
   :type transport: :dn:iface:`~DotNetSnmp.Transport.ISnmpTransport`
   :param target: The SNMP target containing protocol version, security, and timeout parameters.
   :type target: :dn:iface:`~DotNetSnmp.Transport.Targets.ISnmpTarget`
   :param targetAddress: The network address (IP:port) of the SNMP agent.
   :type targetAddress: ``IPEndPoint``
   :param scope: The PDU wrapped in a scope object containing version-specific data.
   :type scope: :dn:iface:`~DotNetSnmp.Common.Definitions.IScope`
   :param expectResponse: If true, waits for and validates the response; if false, returns immediately.
   :type expectResponse: ``Boolean``
   :param cancellationToken: A cancellation token to abort the operation. The dispatcher also enforces the target&apos;s timeout.
   :type cancellationToken: ``CancellationToken``

   :returns: The response scope containing the SNMP agent&apos;s reply, or the original scope if no response expected.
   :rtype: ``ValueTask<IScope>``

**Source:** `SharpSnmpLib/Dispatch/SnmpDispatcher.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Dispatch/SnmpDispatcher.cs#L115>`__

