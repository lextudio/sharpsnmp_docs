Counter32 Struct
================

.. dn:struct:: DotNetSnmp.Asn1.SyntaxObjects.Counter32

   The Counter32 type represents a non-negative integer which monotonically increases until it reaches a maximum value of 2^32-1 (4294967295 decimal), when it wraps around and starts increasing again from zero. (wraps)

   .. code-block:: csharp

      [CLSCompliant(false)]
      public readonly record struct Counter32(uint Value) : IAsnSerializable, IEquatable<Counter32>

**Namespace:** ``DotNetSnmp.Asn1.SyntaxObjects``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Counter32.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Counter32.cs#L12>`__

Constructors
------------

Counter32(Int64)
~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Asn1.SyntaxObjects.Counter32..ctor(System.Int64)

   Initializes a new instance from a legacy long value.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public Counter32(long value)

   :type value: ``Int64``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Counter32.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Counter32.cs#L18>`__

Counter32(UInt32)
~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Asn1.SyntaxObjects.Counter32..ctor(System.UInt32)

   The Counter32 type represents a non-negative integer which monotonically increases until it reaches a maximum value of 2^32-1 (4294967295 decimal), when it wraps around and starts increasing again from zero. (wraps)

   .. code-block:: csharp

      public Counter32(uint Value)

   :type Value: ``UInt32``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Counter32.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Counter32.cs#L12>`__

Properties
----------

Value
~~~~~

.. dn:property:: DotNetSnmp.Asn1.SyntaxObjects.Counter32.Value

   .. code-block:: csharp

      public uint Value { get; init; }

   :rtype: ``UInt32``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Counter32.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Counter32.cs#L13>`__

Methods
-------

Deconstruct(out UInt32)
~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.Counter32.Deconstruct(System.UInt32@)

   Deconstructs the value into its components.

   .. code-block:: csharp

      public readonly void Deconstruct(scoped out uint value)

   :type value: ``UInt32``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Counter32.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Counter32.cs#L35>`__

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.Counter32.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public readonly void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Counter32.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Counter32.cs#L25>`__

Operators
---------

Implicit(Counter32 to UInt32)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:operator:: DotNetSnmp.Asn1.SyntaxObjects.Counter32.op_Implicit(DotNetSnmp.Asn1.SyntaxObjects.Counter32)

   Performs a conversion to uint.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public static implicit operator uint (Counter32 x)

   :type x: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.Counter32`

   :rtype: ``UInt32``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Counter32.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Counter32.cs#L43>`__

Implicit(Int64 to Counter32)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:operator:: DotNetSnmp.Asn1.SyntaxObjects.Counter32.op_Implicit(System.Int64)

   Performs a compatibility conversion from long.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public static implicit operator Counter32(long value)

   :type value: ``Int64``

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.Counter32`

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Counter32.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Counter32.cs#L49>`__

