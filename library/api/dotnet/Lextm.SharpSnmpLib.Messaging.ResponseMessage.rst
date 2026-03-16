ResponseMessage Class
=====================

.. dn:class:: Lextm.SharpSnmpLib.Messaging.ResponseMessage

   Legacy compatibility wrapper for SNMP response messages.

   .. code-block:: csharp

      [Obsolete("This type is for internal use only and may be removed in a future release.")]
      public sealed class ResponseMessage : ISnmpMessage, IAsnSerializable

**Namespace:** ``Lextm.SharpSnmpLib.Messaging``

**Inheritance:** Object → ``ResponseMessage``

**Source:** `SharpSnmpLib/Messaging/ResponseMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/ResponseMessage.cs#L16>`__

Constructors
------------

ResponseMessage(Int32, VersionCode, OctetString, ErrorCode, Int32, IList<Variable>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Messaging.ResponseMessage..ctor(System.Int32,DotNetSnmp.Common.Definitions.VersionCode,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Common.Definitions.ErrorCode,System.Int32,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable})

   Creates a v1/v2c response message.

   .. code-block:: csharp

      public ResponseMessage(int requestId, VersionCode version, OctetString community, ErrorCode error, int index, IList<Variable> variables)

   :type requestId: ``Int32``
   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type error: :dn:enum:`~DotNetSnmp.Common.Definitions.ErrorCode`
   :type index: ``Int32``
   :type variables: ``IList<Variable>``

**Source:** `SharpSnmpLib/Messaging/ResponseMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/ResponseMessage.cs#L24>`__

ResponseMessage(VersionCode, Header, SecurityParameters, Scope, IPrivacyProvider, Boolean, Byte[]?)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Messaging.ResponseMessage..ctor(DotNetSnmp.Common.Definitions.VersionCode,Lextm.SharpSnmpLib.Header,Lextm.SharpSnmpLib.SecurityParameters,DotNetSnmp.Protocol.V3.Scope,DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider,System.Boolean,System.Byte[])

   Creates a v3 response message.

   .. code-block:: csharp

      public ResponseMessage(VersionCode version, Header header, SecurityParameters parameters, Scope scope, IPrivacyProvider privacy, bool needAuthentication, byte[]? length)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type header: :dn:cls:`~Lextm.SharpSnmpLib.Header`
   :type parameters: :dn:cls:`~Lextm.SharpSnmpLib.SecurityParameters`
   :type scope: :dn:cls:`~DotNetSnmp.Protocol.V3.Scope`
   :type privacy: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`
   :type needAuthentication: ``Boolean``
   :type length: ``Byte[]``

**Source:** `SharpSnmpLib/Messaging/ResponseMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/ResponseMessage.cs#L65>`__

Properties
----------

ErrorIndex
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.ResponseMessage.ErrorIndex

   Gets response error index.

   .. code-block:: csharp

      public int ErrorIndex { get; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Messaging/ResponseMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/ResponseMessage.cs#L142>`__

ErrorStatus
~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.ResponseMessage.ErrorStatus

   Gets response error status.

   .. code-block:: csharp

      public ErrorCode ErrorStatus { get; }

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.ErrorCode`

**Source:** `SharpSnmpLib/Messaging/ResponseMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/ResponseMessage.cs#L137>`__

Header
~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.ResponseMessage.Header

   Gets header.

   .. code-block:: csharp

      public Header Header { get; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpLib.Header`

**Source:** `SharpSnmpLib/Messaging/ResponseMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/ResponseMessage.cs#L122>`__

Parameters
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.ResponseMessage.Parameters

   Gets security parameters.

   .. code-block:: csharp

      public SecurityParameters Parameters { get; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpLib.SecurityParameters`

**Source:** `SharpSnmpLib/Messaging/ResponseMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/ResponseMessage.cs#L127>`__

Privacy
~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.ResponseMessage.Privacy

   Gets privacy provider.

   .. code-block:: csharp

      public IPrivacyProvider Privacy { get; }

   :rtype: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`

**Source:** `SharpSnmpLib/Messaging/ResponseMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/ResponseMessage.cs#L132>`__

ProtocolVersion
~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.ResponseMessage.ProtocolVersion

   Gets protocol version.

   .. code-block:: csharp

      public VersionCode ProtocolVersion { get; }

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`

**Source:** `SharpSnmpLib/Messaging/ResponseMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/ResponseMessage.cs#L112>`__

Scope
~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.ResponseMessage.Scope

   Gets scope.

   .. code-block:: csharp

      public IScope? Scope { get; }

   :rtype: :dn:iface:`~DotNetSnmp.Common.Definitions.IScope`

**Source:** `SharpSnmpLib/Messaging/ResponseMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/ResponseMessage.cs#L117>`__

Version
~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.ResponseMessage.Version

   Gets legacy version alias.

   .. code-block:: csharp

      public VersionCode Version { get; }

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`

**Source:** `SharpSnmpLib/Messaging/ResponseMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/ResponseMessage.cs#L107>`__

Methods
-------

ToBytes()
~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.ResponseMessage.ToBytes

   Serializes message to bytes.

   .. code-block:: csharp

      public byte[] ToBytes()

   :rtype: ``Byte[]``

**Source:** `SharpSnmpLib/Messaging/ResponseMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/ResponseMessage.cs#L147>`__

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.ResponseMessage.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/Messaging/ResponseMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/ResponseMessage.cs#L153>`__

