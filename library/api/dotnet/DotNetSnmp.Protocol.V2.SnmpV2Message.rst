SnmpV2Message Class
===================

.. dn:class:: DotNetSnmp.Protocol.V2.SnmpV2Message

   Represents the SnmpV2Message type.

   .. code-block:: csharp

      public class SnmpV2Message : ISnmpMessage, IAsnSerializable

**Namespace:** ``DotNetSnmp.Protocol.V2``

**Inheritance:** Object → ``SnmpV2Message``

**Source:** `SharpSnmpLib/V2c/SnmpV2Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V2c/SnmpV2Message.cs#L11>`__

Properties
----------

Community
~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V2.SnmpV2Message.Community

   Gets community.

   .. code-block:: csharp

      public OctetString Community { get; set; }

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`

**Source:** `SharpSnmpLib/V2c/SnmpV2Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V2c/SnmpV2Message.cs#L21>`__

Pdu
~~~

.. dn:property:: DotNetSnmp.Protocol.V2.SnmpV2Message.Pdu

   Represents pdu.

   .. code-block:: csharp

      public Pdu Pdu { get; }

   :rtype: :dn:cls:`~DotNetSnmp.Common.Definitions.Pdu`

**Source:** `SharpSnmpLib/V2c/SnmpV2Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V2c/SnmpV2Message.cs#L31>`__

ProtocolVersion
~~~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V2.SnmpV2Message.ProtocolVersion

   Represents v2.

   .. code-block:: csharp

      public VersionCode ProtocolVersion { get; }

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`

**Source:** `SharpSnmpLib/V2c/SnmpV2Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V2c/SnmpV2Message.cs#L16>`__

Scope
~~~~~

.. dn:property:: DotNetSnmp.Protocol.V2.SnmpV2Message.Scope

   Gets the message scope.

   .. code-block:: csharp

      public IScope? Scope { get; init; }

   :rtype: :dn:iface:`~DotNetSnmp.Common.Definitions.IScope`

**Source:** `SharpSnmpLib/V2c/SnmpV2Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V2c/SnmpV2Message.cs#L26>`__

Methods
-------

ReadFrom(AsnReader)
~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V2.SnmpV2Message.ReadFrom(System.Formats.Asn1.AsnReader)

   Reads a value from an ASN.1 reader.

   .. code-block:: csharp

      public static SnmpV2Message ReadFrom(AsnReader reader)

   :type reader: ``AsnReader``

   :rtype: :dn:cls:`~DotNetSnmp.Protocol.V2.SnmpV2Message`

**Source:** `SharpSnmpLib/V2c/SnmpV2Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V2c/SnmpV2Message.cs#L52>`__

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V2.SnmpV2Message.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/V2c/SnmpV2Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V2c/SnmpV2Message.cs#L34>`__

