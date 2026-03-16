ISnmpDispatcher Interface
=========================

.. dn:interface:: DotNetSnmp.Client.ISnmpDispatcher

   Defines the contract for ISnmpDispatcher.

   .. code-block:: csharp

      public interface ISnmpDispatcher

**Namespace:** ``DotNetSnmp.Client``

**Source:** `SharpSnmpLib/Dispatch/ISnmpDispatcher.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Dispatch/ISnmpDispatcher.cs#L10>`__

Methods
-------

SendPdu(ISnmpTransport, ISnmpTarget, IPEndPoint, IScope, Boolean, CancellationToken)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Client.ISnmpDispatcher.SendPdu(DotNetSnmp.Transport.ISnmpTransport,DotNetSnmp.Transport.Targets.ISnmpTarget,System.Net.IPEndPoint,DotNetSnmp.Common.Definitions.IScope,System.Boolean,System.Threading.CancellationToken)

   Sends pdu.

   .. code-block:: csharp

      ValueTask<IScope> SendPdu(ISnmpTransport transport, ISnmpTarget target, IPEndPoint targetAddress, IScope scope, bool expectResponse, CancellationToken cancellationToken)

   :type transport: :dn:iface:`~DotNetSnmp.Transport.ISnmpTransport`
   :type target: :dn:iface:`~DotNetSnmp.Transport.Targets.ISnmpTarget`
   :type targetAddress: ``IPEndPoint``
   :type scope: :dn:iface:`~DotNetSnmp.Common.Definitions.IScope`
   :type expectResponse: ``Boolean``
   :type cancellationToken: ``CancellationToken``

   :rtype: ``ValueTask<IScope>``

**Source:** `SharpSnmpLib/Dispatch/ISnmpDispatcher.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Dispatch/ISnmpDispatcher.cs#L15>`__

