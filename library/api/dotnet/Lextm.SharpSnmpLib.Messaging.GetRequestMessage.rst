GetRequestMessage Class
=======================

.. dn:class:: Lextm.SharpSnmpLib.Messaging.GetRequestMessage

   Legacy compatibility wrapper for SNMP v3 GET request message.

   .. code-block:: csharp

      public sealed class GetRequestMessage : ISnmpMessage, IAsnSerializable, ILegacyV3Request

**Namespace:** ``Lextm.SharpSnmpLib.Messaging``

**Inheritance:** Object → ``GetRequestMessage``

**Source:** `SharpSnmpLib/Messaging/GetRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/GetRequestMessage.cs#L13>`__

Constructors
------------

GetRequestMessage(Int32, VersionCode, OctetString, IList<Variable>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Messaging.GetRequestMessage..ctor(System.Int32,DotNetSnmp.Common.Definitions.VersionCode,DotNetSnmp.Asn1.SyntaxObjects.OctetString,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable})

   Initializes a new instance of GetRequestMessage.

   .. code-block:: csharp

      public GetRequestMessage(int requestId, VersionCode version, OctetString community, IList<Variable> variables)

   :type requestId: ``Int32``
   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type variables: ``IList<Variable>``

**Source:** `SharpSnmpLib/Messaging/GetRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/GetRequestMessage.cs#L20>`__

GetRequestMessage(VersionCode, Int32, Int32, OctetString, IList<Variable>, IPrivacyProvider, Int32, ISnmpMessage)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Messaging.GetRequestMessage..ctor(DotNetSnmp.Common.Definitions.VersionCode,System.Int32,System.Int32,DotNetSnmp.Asn1.SyntaxObjects.OctetString,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider,System.Int32,DotNetSnmp.Common.Definitions.ISnmpMessage)

   Initializes a new instance of GetRequestMessage.

   .. code-block:: csharp

      [Obsolete("Please use overloads with contextName.")]
      public GetRequestMessage(VersionCode version, int messageId, int requestId, OctetString user, IList<Variable> variables, IPrivacyProvider privacy, int maxMessageSize, ISnmpMessage report)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type messageId: ``Int32``
   :type requestId: ``Int32``
   :type user: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type variables: ``IList<Variable>``
   :type privacy: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`
   :type maxMessageSize: ``Int32``
   :type report: :dn:iface:`~DotNetSnmp.Common.Definitions.ISnmpMessage`

**Source:** `SharpSnmpLib/Messaging/GetRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/GetRequestMessage.cs#L92>`__

GetRequestMessage(VersionCode, Int32, Int32, OctetString, IList<Variable>, IPrivacyProvider, ISnmpMessage)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Messaging.GetRequestMessage..ctor(DotNetSnmp.Common.Definitions.VersionCode,System.Int32,System.Int32,DotNetSnmp.Asn1.SyntaxObjects.OctetString,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider,DotNetSnmp.Common.Definitions.ISnmpMessage)

   Initializes a new instance of GetRequestMessage.

   .. code-block:: csharp

      [Obsolete("Please use overloads with contextName.")]
      public GetRequestMessage(VersionCode version, int messageId, int requestId, OctetString user, IList<Variable> variables, IPrivacyProvider privacy, ISnmpMessage report)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type messageId: ``Int32``
   :type requestId: ``Int32``
   :type user: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type variables: ``IList<Variable>``
   :type privacy: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`
   :type report: :dn:iface:`~DotNetSnmp.Common.Definitions.ISnmpMessage`

**Source:** `SharpSnmpLib/Messaging/GetRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/GetRequestMessage.cs#L67>`__

GetRequestMessage(VersionCode, Int32, Int32, OctetString, OctetString, IList<Variable>, IPrivacyProvider, Int32, ISnmpMessage)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Messaging.GetRequestMessage..ctor(DotNetSnmp.Common.Definitions.VersionCode,System.Int32,System.Int32,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.OctetString,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider,System.Int32,DotNetSnmp.Common.Definitions.ISnmpMessage)

   Initializes a new instance of GetRequestMessage.

   .. code-block:: csharp

      public GetRequestMessage(VersionCode version, int messageId, int requestId, OctetString user, OctetString contextName, IList<Variable> variables, IPrivacyProvider privacy, int maxMessageSize, ISnmpMessage report)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type messageId: ``Int32``
   :type requestId: ``Int32``
   :type user: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type contextName: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type variables: ``IList<Variable>``
   :type privacy: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`
   :type maxMessageSize: ``Int32``
   :type report: :dn:iface:`~DotNetSnmp.Common.Definitions.ISnmpMessage`

**Source:** `SharpSnmpLib/Messaging/GetRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/GetRequestMessage.cs#L35>`__

Properties
----------

Privacy
~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.GetRequestMessage.Privacy

   Gets privacy.

   .. code-block:: csharp

      public IPrivacyProvider Privacy { get; }

   :rtype: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`

**Source:** `SharpSnmpLib/Messaging/GetRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/GetRequestMessage.cs#L118>`__

ProtocolVersion
~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.GetRequestMessage.ProtocolVersion

   Represents protocol Version.

   .. code-block:: csharp

      public VersionCode ProtocolVersion { get; }

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`

**Source:** `SharpSnmpLib/Messaging/GetRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/GetRequestMessage.cs#L123>`__

Scope
~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.GetRequestMessage.Scope

   Represents scope.

   .. code-block:: csharp

      public IScope? Scope { get; }

   :rtype: :dn:iface:`~DotNetSnmp.Common.Definitions.IScope`

**Source:** `SharpSnmpLib/Messaging/GetRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/GetRequestMessage.cs#L128>`__

Methods
-------

ToBytes()
~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.GetRequestMessage.ToBytes

   Serializes the message to a byte array.

   .. code-block:: csharp

      public byte[] ToBytes()

   :rtype: ``Byte[]``

**Source:** `SharpSnmpLib/Messaging/GetRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/GetRequestMessage.cs#L133>`__

ToString()
~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.GetRequestMessage.ToString

   Returns a ``String`` that represents this :dn:cls:``~Lextm.SharpSnmpLib.Messaging.GetRequestMessage``.

   .. code-block:: csharp

      public override string ToString()

   :rtype: ``String``

**Source:** `SharpSnmpLib/Messaging/GetRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/GetRequestMessage.cs#L147>`__

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.GetRequestMessage.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/Messaging/GetRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/GetRequestMessage.cs#L139>`__

