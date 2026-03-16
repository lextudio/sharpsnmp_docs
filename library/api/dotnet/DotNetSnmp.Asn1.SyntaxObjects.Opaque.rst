Opaque Struct
=============

.. dn:struct:: DotNetSnmp.Asn1.SyntaxObjects.Opaque

   Represents the Opaque type.

   .. code-block:: csharp

      public readonly record struct Opaque(byte[] OctetString) : IAsnSerializable, IEquatable<Opaque>

**Namespace:** ``DotNetSnmp.Asn1.SyntaxObjects``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Opaque.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Opaque.cs#L8>`__

Constructors
------------

Opaque(Byte[])
~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Asn1.SyntaxObjects.Opaque..ctor(System.Byte[])

   Represents the Opaque type.

   .. code-block:: csharp

      public Opaque(byte[] OctetString)

   :type OctetString: ``Byte[]``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Opaque.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Opaque.cs#L8>`__

Properties
----------

OctetString
~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Asn1.SyntaxObjects.Opaque.OctetString

   .. code-block:: csharp

      public byte[] OctetString { get; init; }

   :rtype: ``Byte[]``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Opaque.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Opaque.cs#L8>`__

Methods
-------

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.Opaque.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public readonly void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Opaque.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Opaque.cs#L11>`__

Operators
---------

Implicit(Opaque to Byte[])
~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:operator:: DotNetSnmp.Asn1.SyntaxObjects.Opaque.op_Implicit(DotNetSnmp.Asn1.SyntaxObjects.Opaque)

   Performs a conversion to byte[].

   .. code-block:: csharp

      public static implicit operator byte[](Opaque o)

   :type o: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.Opaque`

   :rtype: ``Byte[]``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Opaque.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Opaque.cs#L19>`__

