SnmpV3Message Class
===================

.. dn:class:: DotNetSnmp.Protocol.V3.SnmpV3Message

   Represents the SnmpV3Message type.

   .. code-block:: csharp

      public class SnmpV3Message : ISnmpMessage, IAsnSerializable

**Namespace:** ``DotNetSnmp.Protocol.V3``

**Inheritance:** Object → ``SnmpV3Message``

**Source:** `SharpSnmpLib/V3/SnmpV3Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/SnmpV3Message.cs#L10>`__

Properties
----------

EncryptedScopedPdu
~~~~~~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.SnmpV3Message.EncryptedScopedPdu

   Gets encrypted Scoped Pdu.

   .. code-block:: csharp

      public ReadOnlyMemory<byte> EncryptedScopedPdu { get; set; }

   :rtype: ``ReadOnlyMemory<Byte>``

**Source:** `SharpSnmpLib/V3/SnmpV3Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/SnmpV3Message.cs#L30>`__

Header
~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.SnmpV3Message.Header

   Gets header.

   .. code-block:: csharp

      public required HeaderData Header { get; set; }

   :rtype: :dn:cls:`~DotNetSnmp.Protocol.V3.HeaderData`

**Source:** `SharpSnmpLib/V3/SnmpV3Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/SnmpV3Message.cs#L20>`__

ProtocolVersion
~~~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.SnmpV3Message.ProtocolVersion

   Represents v3.

   .. code-block:: csharp

      public VersionCode ProtocolVersion { get; }

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`

**Source:** `SharpSnmpLib/V3/SnmpV3Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/SnmpV3Message.cs#L15>`__

Scope
~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.SnmpV3Message.Scope

   Gets the message scope.

   .. code-block:: csharp

      public IScope? Scope { get; set; }

   :rtype: :dn:iface:`~DotNetSnmp.Common.Definitions.IScope`

**Source:** `SharpSnmpLib/V3/SnmpV3Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/SnmpV3Message.cs#L35>`__

SecurityParameters
~~~~~~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.SnmpV3Message.SecurityParameters

   Gets security Parameters.

   .. code-block:: csharp

      public required UsmSecurityParameters SecurityParameters { get; set; }

   :rtype: :dn:cls:`~DotNetSnmp.Protocol.V3.Security.UsmSecurityParameters`

**Source:** `SharpSnmpLib/V3/SnmpV3Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/SnmpV3Message.cs#L25>`__

Methods
-------

ReadFrom(AsnReader)
~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.SnmpV3Message.ReadFrom(System.Formats.Asn1.AsnReader)

   Reads a value from an ASN.1 reader.

   .. code-block:: csharp

      public static SnmpV3Message ReadFrom(AsnReader reader)

   :type reader: ``AsnReader``

   :rtype: :dn:cls:`~DotNetSnmp.Protocol.V3.SnmpV3Message`

**Source:** `SharpSnmpLib/V3/SnmpV3Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/SnmpV3Message.cs#L74>`__

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.SnmpV3Message.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/V3/SnmpV3Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/SnmpV3Message.cs#L38>`__

