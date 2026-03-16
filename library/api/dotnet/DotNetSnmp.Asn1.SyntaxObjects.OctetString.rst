OctetString Struct
==================

.. dn:struct:: DotNetSnmp.Asn1.SyntaxObjects.OctetString

   Represents the OctetString type.

   .. code-block:: csharp

      public readonly record struct OctetString : IAsnSerializable, IEquatable<OctetString>

**Namespace:** ``DotNetSnmp.Asn1.SyntaxObjects``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/OctetString.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/OctetString.cs#L10>`__

Constructors
------------

OctetString(Byte[])
~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Asn1.SyntaxObjects.OctetString..ctor(System.Byte[])

   Initializes a new instance of OctetString.

   .. code-block:: csharp

      public OctetString(byte[] octets)

   :type octets: ``Byte[]``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/OctetString.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/OctetString.cs#L55>`__

OctetString(String, Encoding)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Asn1.SyntaxObjects.OctetString..ctor(System.String,System.Text.Encoding)

   Initializes a new instance of OctetString.

   .. code-block:: csharp

      public OctetString(string str, Encoding encoding)

   :type str: ``String``
   :type encoding: ``Encoding``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/OctetString.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/OctetString.cs#L43>`__

OctetString(String)
~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Asn1.SyntaxObjects.OctetString..ctor(System.String)

   Initializes a new instance of OctetString.

   .. code-block:: csharp

      public OctetString(string str)

   :type str: ``String``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/OctetString.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/OctetString.cs#L35>`__

Properties
----------

DefaultEncoding
~~~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Asn1.SyntaxObjects.OctetString.DefaultEncoding

   Default text encoding used by string-based OctetString conversions.

   .. code-block:: csharp

      public static Encoding DefaultEncoding { get; set; }

   :rtype: ``Encoding``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/OctetString.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/OctetString.cs#L15>`__

Empty
~~~~~

.. dn:property:: DotNetSnmp.Asn1.SyntaxObjects.OctetString.Empty

   An empty octet string value.

   .. code-block:: csharp

      public static OctetString Empty { get; }

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/OctetString.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/OctetString.cs#L20>`__

Encoding
~~~~~~~~

.. dn:property:: DotNetSnmp.Asn1.SyntaxObjects.OctetString.Encoding

   Gets the text encoding associated with this value.

   .. code-block:: csharp

      public Encoding Encoding { get; }

   :rtype: ``Encoding``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/OctetString.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/OctetString.cs#L30>`__

Octets
~~~~~~

.. dn:property:: DotNetSnmp.Asn1.SyntaxObjects.OctetString.Octets

   Gets octets.

   .. code-block:: csharp

      public byte[] Octets { get; }

   :rtype: ``Byte[]``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/OctetString.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/OctetString.cs#L25>`__

Methods
-------

Equals(OctetString)
~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.OctetString.Equals(DotNetSnmp.Asn1.SyntaxObjects.OctetString)

   Indicates whether the current object is equal to another object of the same type.

   .. code-block:: csharp

      public readonly bool Equals(OctetString other)

   :type other: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`

   :rtype: ``Boolean``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/OctetString.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/OctetString.cs#L103>`__

GetHashCode()
~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.OctetString.GetHashCode

   Serves as a hash function for a particular type.

   .. code-block:: csharp

      public readonly override int GetHashCode()

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/OctetString.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/OctetString.cs#L116>`__

ReadFrom(AsnReader)
~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.OctetString.ReadFrom(System.Formats.Asn1.AsnReader)

   Reads a value from an ASN.1 reader.

   .. code-block:: csharp

      public static OctetString ReadFrom(AsnReader reader)

   :type reader: ``AsnReader``

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/OctetString.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/OctetString.cs#L88>`__

ToString()
~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.OctetString.ToString

   Returns a ``String`` that represents this :dn:struct:``~DotNetSnmp.Asn1.SyntaxObjects.OctetString``.

   .. code-block:: csharp

      public readonly override string ToString()

   :rtype: ``String``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/OctetString.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/OctetString.cs#L74>`__

ToString(Encoding)
~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.OctetString.ToString(System.Text.Encoding)

   Returns a ``String`` using a specified encoding.

   .. code-block:: csharp

      public readonly string ToString(Encoding encoding)

   :type encoding: ``Encoding``

   :rtype: ``String``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/OctetString.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/OctetString.cs#L65>`__

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.OctetString.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public readonly void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/OctetString.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/OctetString.cs#L80>`__

Operators
---------

Implicit(OctetString to String)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:operator:: DotNetSnmp.Asn1.SyntaxObjects.OctetString.op_Implicit(DotNetSnmp.Asn1.SyntaxObjects.OctetString)

   Performs a conversion to string.

   .. code-block:: csharp

      public static implicit operator string (OctetString o)

   :type o: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`

   :rtype: ``String``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/OctetString.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/OctetString.cs#L97>`__

