GetBulkRequestMessage Class
===========================

.. dn:class:: Lextm.SharpSnmpLib.Messaging.GetBulkRequestMessage

   Legacy compatibility wrapper for SNMP GET-BULK request messages.

   .. code-block:: csharp

      public sealed class GetBulkRequestMessage : ISnmpMessage, IAsnSerializable, ILegacyV3Request

**Namespace:** ``Lextm.SharpSnmpLib.Messaging``

**Inheritance:** Object → ``GetBulkRequestMessage``

**Source:** `SharpSnmpLib/Messaging/GetBulkRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/GetBulkRequestMessage.cs#L13>`__

Constructors
------------

GetBulkRequestMessage(Int32, VersionCode, OctetString, Int32, Int32, IList<Variable>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Messaging.GetBulkRequestMessage..ctor(System.Int32,DotNetSnmp.Common.Definitions.VersionCode,DotNetSnmp.Asn1.SyntaxObjects.OctetString,System.Int32,System.Int32,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable})

   Initializes a new instance of GetBulkRequestMessage.

   .. code-block:: csharp

      public GetBulkRequestMessage(int requestId, VersionCode version, OctetString community, int nonRepeaters, int maxRepetitions, IList<Variable> variables)

   :type requestId: ``Int32``
   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type nonRepeaters: ``Int32``
   :type maxRepetitions: ``Int32``
   :type variables: ``IList<Variable>``

**Source:** `SharpSnmpLib/Messaging/GetBulkRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/GetBulkRequestMessage.cs#L20>`__

GetBulkRequestMessage(VersionCode, Int32, Int32, OctetString, OctetString, Int32, Int32, IList<Variable>, IPrivacyProvider, Int32, ISnmpMessage)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Messaging.GetBulkRequestMessage..ctor(DotNetSnmp.Common.Definitions.VersionCode,System.Int32,System.Int32,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.OctetString,System.Int32,System.Int32,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider,System.Int32,DotNetSnmp.Common.Definitions.ISnmpMessage)

   Initializes a new instance of GetBulkRequestMessage.

   .. code-block:: csharp

      public GetBulkRequestMessage(VersionCode version, int messageId, int requestId, OctetString user, OctetString contextName, int nonRepeaters, int maxRepetitions, IList<Variable> variables, IPrivacyProvider privacy, int maxMessageSize, ISnmpMessage report)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type messageId: ``Int32``
   :type requestId: ``Int32``
   :type user: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type contextName: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type nonRepeaters: ``Int32``
   :type maxRepetitions: ``Int32``
   :type variables: ``IList<Variable>``
   :type privacy: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`
   :type maxMessageSize: ``Int32``
   :type report: :dn:iface:`~DotNetSnmp.Common.Definitions.ISnmpMessage`

**Source:** `SharpSnmpLib/Messaging/GetBulkRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/GetBulkRequestMessage.cs#L50>`__

Properties
----------

Privacy
~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.GetBulkRequestMessage.Privacy

   Gets privacy.

   .. code-block:: csharp

      public IPrivacyProvider Privacy { get; }

   :rtype: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`

**Source:** `SharpSnmpLib/Messaging/GetBulkRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/GetBulkRequestMessage.cs#L88>`__

ProtocolVersion
~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.GetBulkRequestMessage.ProtocolVersion

   Represents protocol Version.

   .. code-block:: csharp

      public VersionCode ProtocolVersion { get; }

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`

**Source:** `SharpSnmpLib/Messaging/GetBulkRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/GetBulkRequestMessage.cs#L93>`__

Scope
~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.GetBulkRequestMessage.Scope

   Represents scope.

   .. code-block:: csharp

      public IScope? Scope { get; }

   :rtype: :dn:iface:`~DotNetSnmp.Common.Definitions.IScope`

**Source:** `SharpSnmpLib/Messaging/GetBulkRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/GetBulkRequestMessage.cs#L98>`__

Methods
-------

ToBytes()
~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.GetBulkRequestMessage.ToBytes

   Serializes the message to a byte array.

   .. code-block:: csharp

      public byte[] ToBytes()

   :rtype: ``Byte[]``

**Source:** `SharpSnmpLib/Messaging/GetBulkRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/GetBulkRequestMessage.cs#L103>`__

ToString()
~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.GetBulkRequestMessage.ToString

   Returns a ``String`` that represents this :dn:cls:``~Lextm.SharpSnmpLib.Messaging.GetBulkRequestMessage``.

   .. code-block:: csharp

      public override string ToString()

   :rtype: ``String``

**Source:** `SharpSnmpLib/Messaging/GetBulkRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/GetBulkRequestMessage.cs#L117>`__

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.GetBulkRequestMessage.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/Messaging/GetBulkRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/GetBulkRequestMessage.cs#L109>`__

