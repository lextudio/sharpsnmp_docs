ReportMessage Class
===================

.. dn:class:: Lextm.SharpSnmpLib.Messaging.ReportMessage

   REPORT message wrapper for compatibility APIs.

   .. code-block:: csharp

      public sealed class ReportMessage : ISnmpMessage, IAsnSerializable

**Namespace:** ``Lextm.SharpSnmpLib.Messaging``

**Inheritance:** Object → ``ReportMessage``

**Source:** `SharpSnmpLib/Messaging/ReportMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/ReportMessage.cs#L13>`__

Constructors
------------

ReportMessage(SnmpV3Message)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Messaging.ReportMessage..ctor(DotNetSnmp.Protocol.V3.SnmpV3Message)

   Initializes a new instance of ReportMessage.

   .. code-block:: csharp

      public ReportMessage(SnmpV3Message message)

   :param message: The parsed SNMP v3 message.
   :type message: :dn:cls:`~DotNetSnmp.Protocol.V3.SnmpV3Message`

**Source:** `SharpSnmpLib/Messaging/ReportMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/ReportMessage.cs#L19>`__

ReportMessage(VersionCode, Header, SecurityParameters, Scope, IPrivacyProvider, Byte[]?)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Messaging.ReportMessage..ctor(DotNetSnmp.Common.Definitions.VersionCode,Lextm.SharpSnmpLib.Header,Lextm.SharpSnmpLib.SecurityParameters,DotNetSnmp.Protocol.V3.Scope,DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider,System.Byte[])

   Initializes a new instance of ReportMessage from legacy v3 constructor arguments.

   .. code-block:: csharp

      public ReportMessage(VersionCode version, Header header, SecurityParameters parameters, Scope scope, IPrivacyProvider privacy, byte[]? length)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type header: :dn:cls:`~Lextm.SharpSnmpLib.Header`
   :type parameters: :dn:cls:`~Lextm.SharpSnmpLib.SecurityParameters`
   :type scope: :dn:cls:`~DotNetSnmp.Protocol.V3.Scope`
   :type privacy: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`
   :type length: ``Byte[]``

**Source:** `SharpSnmpLib/Messaging/ReportMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/ReportMessage.cs#L45>`__

Properties
----------

Header
~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.ReportMessage.Header

   Gets header.

   .. code-block:: csharp

      public Header Header { get; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpLib.Header`

**Source:** `SharpSnmpLib/Messaging/ReportMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/ReportMessage.cs#L111>`__

Message
~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.ReportMessage.Message

   Gets message.

   .. code-block:: csharp

      public SnmpV3Message Message { get; }

   :rtype: :dn:cls:`~DotNetSnmp.Protocol.V3.SnmpV3Message`

**Source:** `SharpSnmpLib/Messaging/ReportMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/ReportMessage.cs#L106>`__

Parameters
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.ReportMessage.Parameters

   Gets security parameters.

   .. code-block:: csharp

      public SecurityParameters Parameters { get; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpLib.SecurityParameters`

**Source:** `SharpSnmpLib/Messaging/ReportMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/ReportMessage.cs#L116>`__

Privacy
~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.ReportMessage.Privacy

   Gets privacy provider.

   .. code-block:: csharp

      public IPrivacyProvider Privacy { get; }

   :rtype: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`

**Source:** `SharpSnmpLib/Messaging/ReportMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/ReportMessage.cs#L121>`__

ProtocolVersion
~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.ReportMessage.ProtocolVersion

   Represents protocol Version.

   .. code-block:: csharp

      public VersionCode ProtocolVersion { get; }

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`

**Source:** `SharpSnmpLib/Messaging/ReportMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/ReportMessage.cs#L131>`__

Scope
~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.ReportMessage.Scope

   Represents scope.

   .. code-block:: csharp

      public IScope? Scope { get; }

   :rtype: :dn:iface:`~DotNetSnmp.Common.Definitions.IScope`

**Source:** `SharpSnmpLib/Messaging/ReportMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/ReportMessage.cs#L136>`__

Version
~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.ReportMessage.Version

   Represents protocol Version.

   .. code-block:: csharp

      public VersionCode Version { get; }

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`

**Source:** `SharpSnmpLib/Messaging/ReportMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/ReportMessage.cs#L126>`__

Methods
-------

ToBytes()
~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.ReportMessage.ToBytes

   Serializes the message to a byte array.

   .. code-block:: csharp

      public byte[] ToBytes()

   :returns: Encoded SNMP message bytes.
   :rtype: ``Byte[]``

**Source:** `SharpSnmpLib/Messaging/ReportMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/ReportMessage.cs#L142>`__

ToString()
~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.ReportMessage.ToString

   .. code-block:: csharp

      public override string ToString()

   :rtype: ``String``

**Source:** `SharpSnmpLib/Messaging/ReportMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/ReportMessage.cs#L154>`__

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.ReportMessage.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/Messaging/ReportMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/ReportMessage.cs#L148>`__

