GetNextRequestMessage Class
===========================

.. dn:class:: Lextm.SharpSnmpLib.Messaging.GetNextRequestMessage

   Legacy compatibility wrapper for SNMP GET-NEXT request messages.

   .. code-block:: csharp

      public sealed class GetNextRequestMessage : ISnmpMessage, IAsnSerializable, ILegacyV3Request

**Namespace:** ``Lextm.SharpSnmpLib.Messaging``

**Inheritance:** Object → ``GetNextRequestMessage``

**Source:** `SharpSnmpLib/Messaging/GetNextRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/GetNextRequestMessage.cs#L13>`__

Constructors
------------

GetNextRequestMessage(Int32, VersionCode, OctetString, IList<Variable>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Messaging.GetNextRequestMessage..ctor(System.Int32,DotNetSnmp.Common.Definitions.VersionCode,DotNetSnmp.Asn1.SyntaxObjects.OctetString,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable})

   Initializes a new instance of GetNextRequestMessage.

   .. code-block:: csharp

      public GetNextRequestMessage(int requestId, VersionCode version, OctetString community, IList<Variable> variables)

   :type requestId: ``Int32``
   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type variables: ``IList<Variable>``

**Source:** `SharpSnmpLib/Messaging/GetNextRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/GetNextRequestMessage.cs#L20>`__

GetNextRequestMessage(VersionCode, Int32, Int32, OctetString, OctetString, IList<Variable>, IPrivacyProvider, Int32, ISnmpMessage)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Messaging.GetNextRequestMessage..ctor(DotNetSnmp.Common.Definitions.VersionCode,System.Int32,System.Int32,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.OctetString,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider,System.Int32,DotNetSnmp.Common.Definitions.ISnmpMessage)

   Initializes a new instance of GetNextRequestMessage.

   .. code-block:: csharp

      public GetNextRequestMessage(VersionCode version, int messageId, int requestId, OctetString user, OctetString contextName, IList<Variable> variables, IPrivacyProvider privacy, int maxMessageSize, ISnmpMessage report)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type messageId: ``Int32``
   :type requestId: ``Int32``
   :type user: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type contextName: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type variables: ``IList<Variable>``
   :type privacy: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`
   :type maxMessageSize: ``Int32``
   :type report: :dn:iface:`~DotNetSnmp.Common.Definitions.ISnmpMessage`

**Source:** `SharpSnmpLib/Messaging/GetNextRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/GetNextRequestMessage.cs#L35>`__

Properties
----------

Privacy
~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.GetNextRequestMessage.Privacy

   Gets privacy.

   .. code-block:: csharp

      public IPrivacyProvider Privacy { get; }

   :rtype: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`

**Source:** `SharpSnmpLib/Messaging/GetNextRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/GetNextRequestMessage.cs#L67>`__

ProtocolVersion
~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.GetNextRequestMessage.ProtocolVersion

   Represents protocol Version.

   .. code-block:: csharp

      public VersionCode ProtocolVersion { get; }

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`

**Source:** `SharpSnmpLib/Messaging/GetNextRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/GetNextRequestMessage.cs#L72>`__

Scope
~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.GetNextRequestMessage.Scope

   Represents scope.

   .. code-block:: csharp

      public IScope? Scope { get; }

   :rtype: :dn:iface:`~DotNetSnmp.Common.Definitions.IScope`

**Source:** `SharpSnmpLib/Messaging/GetNextRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/GetNextRequestMessage.cs#L77>`__

Methods
-------

ToBytes()
~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.GetNextRequestMessage.ToBytes

   Serializes the message to a byte array.

   .. code-block:: csharp

      public byte[] ToBytes()

   :rtype: ``Byte[]``

**Source:** `SharpSnmpLib/Messaging/GetNextRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/GetNextRequestMessage.cs#L82>`__

ToString()
~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.GetNextRequestMessage.ToString

   Returns a ``String`` that represents this :dn:cls:``~Lextm.SharpSnmpLib.Messaging.GetNextRequestMessage``.

   .. code-block:: csharp

      public override string ToString()

   :rtype: ``String``

**Source:** `SharpSnmpLib/Messaging/GetNextRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/GetNextRequestMessage.cs#L96>`__

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.GetNextRequestMessage.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/Messaging/GetNextRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/GetNextRequestMessage.cs#L88>`__

