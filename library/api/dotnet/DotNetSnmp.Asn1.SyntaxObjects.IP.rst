IP Struct
=========

.. dn:struct:: DotNetSnmp.Asn1.SyntaxObjects.IP

   The IpAddress type represents a 32-bit internet address. It is represented as an OCTET STRING of length 4, in network byte-order

   .. code-block:: csharp

      public readonly record struct IP : IAsnSerializable, IEquatable<IP>

**Namespace:** ``DotNetSnmp.Asn1.SyntaxObjects``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/IP.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/IP.cs#L10>`__

Constructors
------------

IP(Byte[])
~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Asn1.SyntaxObjects.IP..ctor(System.Byte[])

   Initializes a new instance of IP.

   .. code-block:: csharp

      public IP(byte[] address)

   :type address: ``Byte[]``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/IP.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/IP.cs#L28>`__

IP(IPAddress)
~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Asn1.SyntaxObjects.IP..ctor(System.Net.IPAddress)

   Initializes a new instance of IP.

   .. code-block:: csharp

      public IP(IPAddress address)

   :type address: ``IPAddress``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/IP.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/IP.cs#L41>`__

IP(String)
~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Asn1.SyntaxObjects.IP..ctor(System.String)

   Initializes a new instance of IP.

   .. code-block:: csharp

      public IP(string address)

   :type address: ``String``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/IP.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/IP.cs#L20>`__

Properties
----------

AddressBytes
~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Asn1.SyntaxObjects.IP.AddressBytes

   Gets address Bytes.

   .. code-block:: csharp

      public byte[] AddressBytes { get; }

   :rtype: ``Byte[]``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/IP.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/IP.cs#L15>`__

Methods
-------

Deconstruct(out IPAddress)
~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.IP.Deconstruct(System.Net.IPAddress@)

   Deconstructs the value into its components.

   .. code-block:: csharp

      public readonly void Deconstruct(scoped out IPAddress address)

   :type address: ``IPAddress``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/IP.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/IP.cs#L67>`__

ReadFrom(AsnReader)
~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.IP.ReadFrom(System.Formats.Asn1.AsnReader)

   Reads a value from an ASN.1 reader.

   .. code-block:: csharp

      public static IP ReadFrom(AsnReader reader)

   :type reader: ``AsnReader``

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.IP`

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/IP.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/IP.cs#L57>`__

ToString()
~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.IP.ToString

   Returns a ``String`` that represents this :dn:struct:``~DotNetSnmp.Asn1.SyntaxObjects.IP``.

   .. code-block:: csharp

      public readonly override string ToString()

   :rtype: ``String``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/IP.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/IP.cs#L75>`__

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.IP.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public readonly void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/IP.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/IP.cs#L47>`__

