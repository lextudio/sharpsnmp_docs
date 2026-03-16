Unsigned32 Struct
=================

.. dn:struct:: DotNetSnmp.Asn1.SyntaxObjects.Unsigned32

   Represents the Unsigned32 type.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public readonly record struct Unsigned32(uint Value) : IAsnSerializable, IEquatable<Unsigned32>

**Namespace:** ``DotNetSnmp.Asn1.SyntaxObjects``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Unsigned32.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Unsigned32.cs#L8>`__

Constructors
------------

Unsigned32(UInt32)
~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Asn1.SyntaxObjects.Unsigned32..ctor(System.UInt32)

   Represents the Unsigned32 type.

   .. code-block:: csharp

      public Unsigned32(uint Value)

   :type Value: ``UInt32``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Unsigned32.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Unsigned32.cs#L8>`__

Properties
----------

Value
~~~~~

.. dn:property:: DotNetSnmp.Asn1.SyntaxObjects.Unsigned32.Value

   .. code-block:: csharp

      public uint Value { get; init; }

   :rtype: ``UInt32``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Unsigned32.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Unsigned32.cs#L9>`__

Methods
-------

Deconstruct(out UInt32)
~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.Unsigned32.Deconstruct(System.UInt32@)

   Deconstructs the value into its components.

   .. code-block:: csharp

      public readonly void Deconstruct(scoped out uint value)

   :type value: ``UInt32``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Unsigned32.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Unsigned32.cs#L22>`__

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.Unsigned32.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public readonly void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Unsigned32.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Unsigned32.cs#L12>`__

Operators
---------

Implicit(Unsigned32 to UInt32)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:operator:: DotNetSnmp.Asn1.SyntaxObjects.Unsigned32.op_Implicit(DotNetSnmp.Asn1.SyntaxObjects.Unsigned32)

   Performs a conversion to uint.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public static implicit operator uint (Unsigned32 x)

   :type x: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.Unsigned32`

   :rtype: ``UInt32``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Unsigned32.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Unsigned32.cs#L30>`__

