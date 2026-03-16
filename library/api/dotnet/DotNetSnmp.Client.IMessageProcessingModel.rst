IMessageProcessingModel Interface
=================================

.. dn:interface:: DotNetSnmp.Client.IMessageProcessingModel

   Defines the contract for IMessageProcessingModel.

   .. code-block:: csharp

      public interface IMessageProcessingModel

**Namespace:** ``DotNetSnmp.Client``

**Source:** `SharpSnmpLib/Dispatch/IMessageProcessingModel.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Dispatch/IMessageProcessingModel.cs#L9>`__

Methods
-------

IsProtocolVersionSupported(VersionCode)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Client.IMessageProcessingModel.IsProtocolVersionSupported(DotNetSnmp.Common.Definitions.VersionCode)

   Determines whether this processing model supports the specified SNMP protocol version.

   .. code-block:: csharp

      bool IsProtocolVersionSupported(VersionCode version)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`

   :rtype: ``Boolean``

**Source:** `SharpSnmpLib/Dispatch/IMessageProcessingModel.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Dispatch/IMessageProcessingModel.cs#L14>`__

TryPrepareDataElements(in ReadOnlyMemory<Byte>, in ISnmpTarget, out String, out Levels, out SecurityModel, out ISnmpMessage?, out Int32, out MessageProcessingResult)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Client.IMessageProcessingModel.TryPrepareDataElements(System.ReadOnlyMemory{System.Byte}@,DotNetSnmp.Transport.Targets.ISnmpTarget@,System.String@,DotNetSnmp.Common.Definitions.Levels@,DotNetSnmp.Common.Definitions.SecurityModel@,DotNetSnmp.Common.Definitions.ISnmpMessage@,System.Int32@,DotNetSnmp.Client.MessageProcessingResult@)

   Parses an incoming SNMP message into dispatch data elements.

   .. code-block:: csharp

      bool TryPrepareDataElements(in ReadOnlyMemory<byte> incomingMessage, in ISnmpTarget target, scoped out string securityName, scoped out Levels securityLevel, scoped out SecurityModel securityModel, [NotNullWhen(true)] scoped out ISnmpMessage? message, scoped out int sendPduHandle, scoped out MessageProcessingResult result)

   :type incomingMessage: ``ReadOnlyMemory<Byte>``
   :type target: :dn:iface:`~DotNetSnmp.Transport.Targets.ISnmpTarget`
   :type securityName: ``String``
   :type securityLevel: :dn:enum:`~DotNetSnmp.Common.Definitions.Levels`
   :type securityModel: :dn:enum:`~DotNetSnmp.Common.Definitions.SecurityModel`
   :type message: :dn:iface:`~DotNetSnmp.Common.Definitions.ISnmpMessage`
   :type sendPduHandle: ``Int32``
   :type result: :dn:enum:`~DotNetSnmp.Client.MessageProcessingResult`

   :rtype: ``Boolean``

**Source:** `SharpSnmpLib/Dispatch/IMessageProcessingModel.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Dispatch/IMessageProcessingModel.cs#L32>`__

TryPrepareOutgoingMessage(in ISnmpTarget, in IScope, in ReadOnlyMemory<Byte>, out Int32, out ISnmpMessage?, out MessageProcessingResult, Memory<Byte>, Boolean)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Client.IMessageProcessingModel.TryPrepareOutgoingMessage(DotNetSnmp.Transport.Targets.ISnmpTarget@,DotNetSnmp.Common.Definitions.IScope@,System.ReadOnlyMemory{System.Byte}@,System.Int32@,DotNetSnmp.Common.Definitions.ISnmpMessage@,DotNetSnmp.Client.MessageProcessingResult@,System.Memory{System.Byte},System.Boolean)

   Builds an outgoing SNMP message from a target and PDU scope.

   .. code-block:: csharp

      bool TryPrepareOutgoingMessage(in ISnmpTarget target, in IScope scope, in ReadOnlyMemory<byte> secEngineId, scoped out int sendPduHandle, [NotNullWhen(true)] scoped out ISnmpMessage? outgoingMessage, scoped out MessageProcessingResult result, Memory<byte> digestBuffer, bool expectResponse = true)

   :type target: :dn:iface:`~DotNetSnmp.Transport.Targets.ISnmpTarget`
   :type scope: :dn:iface:`~DotNetSnmp.Common.Definitions.IScope`
   :type secEngineId: ``ReadOnlyMemory<Byte>``
   :type sendPduHandle: ``Int32``
   :type outgoingMessage: :dn:iface:`~DotNetSnmp.Common.Definitions.ISnmpMessage`
   :type result: :dn:enum:`~DotNetSnmp.Client.MessageProcessingResult`
   :type digestBuffer: ``Memory<Byte>``
   :type expectResponse: ``Boolean``

   :rtype: ``Boolean``

**Source:** `SharpSnmpLib/Dispatch/IMessageProcessingModel.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Dispatch/IMessageProcessingModel.cs#L19>`__

