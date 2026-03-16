SnmpV1Message Class
===================

.. dn:class:: DotNetSnmp.Protocol.V1.SnmpV1Message

   Represents the SnmpV1Message type.

   .. code-block:: csharp

      public class SnmpV1Message : ISnmpMessage, IAsnSerializable

**Namespace:** ``DotNetSnmp.Protocol.V1``

**Inheritance:** Object → ``SnmpV1Message``

**Source:** `SharpSnmpLib/V1/SnmpV1Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/SnmpV1Message.cs#L10>`__

Properties
----------

Community
~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V1.SnmpV1Message.Community

   Gets community.

   .. code-block:: csharp

      public OctetString Community { get; set; }

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`

**Source:** `SharpSnmpLib/V1/SnmpV1Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/SnmpV1Message.cs#L20>`__

Pdu
~~~

.. dn:property:: DotNetSnmp.Protocol.V1.SnmpV1Message.Pdu

   Represents pdu.

   .. code-block:: csharp

      public Pdu Pdu { get; }

   :rtype: :dn:cls:`~DotNetSnmp.Common.Definitions.Pdu`

**Source:** `SharpSnmpLib/V1/SnmpV1Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/SnmpV1Message.cs#L30>`__

ProtocolVersion
~~~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V1.SnmpV1Message.ProtocolVersion

   Represents v1.

   .. code-block:: csharp

      public VersionCode ProtocolVersion { get; }

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`

**Source:** `SharpSnmpLib/V1/SnmpV1Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/SnmpV1Message.cs#L15>`__

Scope
~~~~~

.. dn:property:: DotNetSnmp.Protocol.V1.SnmpV1Message.Scope

   Gets the message scope.

   .. code-block:: csharp

      public IScope? Scope { get; init; }

   :rtype: :dn:iface:`~DotNetSnmp.Common.Definitions.IScope`

**Source:** `SharpSnmpLib/V1/SnmpV1Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/SnmpV1Message.cs#L25>`__

Methods
-------

ReadFrom(AsnReader)
~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V1.SnmpV1Message.ReadFrom(System.Formats.Asn1.AsnReader)

   Reads a value from an ASN.1 reader.

   .. code-block:: csharp

      public static SnmpV1Message ReadFrom(AsnReader reader)

   :type reader: ``AsnReader``

   :rtype: :dn:cls:`~DotNetSnmp.Protocol.V1.SnmpV1Message`

**Source:** `SharpSnmpLib/V1/SnmpV1Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/SnmpV1Message.cs#L51>`__

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V1.SnmpV1Message.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/V1/SnmpV1Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/SnmpV1Message.cs#L33>`__

