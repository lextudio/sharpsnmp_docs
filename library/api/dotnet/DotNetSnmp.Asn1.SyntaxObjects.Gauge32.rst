Gauge32 Struct
==============

.. dn:struct:: DotNetSnmp.Asn1.SyntaxObjects.Gauge32

   The Gauge32 type represents a non-negative integer, which may increase or decrease, but shall never exceed a maximum value, nor fall below a minimum value. (doesn&apos;t wrap)

   .. code-block:: csharp

      [CLSCompliant(false)]
      public readonly record struct Gauge32(uint Value) : IAsnSerializable, IEquatable<Gauge32>

**Namespace:** ``DotNetSnmp.Asn1.SyntaxObjects``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Gauge32.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Gauge32.cs#L11>`__

Constructors
------------

Gauge32(Int64)
~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Asn1.SyntaxObjects.Gauge32..ctor(System.Int64)

   Initializes a new instance from a legacy long value.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public Gauge32(long value)

   :type value: ``Int64``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Gauge32.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Gauge32.cs#L17>`__

Gauge32(UInt32)
~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Asn1.SyntaxObjects.Gauge32..ctor(System.UInt32)

   The Gauge32 type represents a non-negative integer, which may increase or decrease, but shall never exceed a maximum value, nor fall below a minimum value. (doesn&apos;t wrap)

   .. code-block:: csharp

      public Gauge32(uint Value)

   :type Value: ``UInt32``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Gauge32.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Gauge32.cs#L11>`__

Properties
----------

Value
~~~~~

.. dn:property:: DotNetSnmp.Asn1.SyntaxObjects.Gauge32.Value

   .. code-block:: csharp

      public uint Value { get; init; }

   :rtype: ``UInt32``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Gauge32.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Gauge32.cs#L12>`__

Methods
-------

Deconstruct(out UInt32)
~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.Gauge32.Deconstruct(System.UInt32@)

   Deconstructs the value into its components.

   .. code-block:: csharp

      public readonly void Deconstruct(scoped out uint value)

   :type value: ``UInt32``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Gauge32.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Gauge32.cs#L33>`__

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.Gauge32.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public readonly void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Gauge32.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Gauge32.cs#L24>`__

Operators
---------

Implicit(Gauge32 to UInt32)
~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:operator:: DotNetSnmp.Asn1.SyntaxObjects.Gauge32.op_Implicit(DotNetSnmp.Asn1.SyntaxObjects.Gauge32)

   Performs a conversion to uint.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public static implicit operator uint (Gauge32 x)

   :type x: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.Gauge32`

   :rtype: ``UInt32``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Gauge32.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Gauge32.cs#L41>`__

Implicit(Int64 to Gauge32)
~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:operator:: DotNetSnmp.Asn1.SyntaxObjects.Gauge32.op_Implicit(System.Int64)

   Performs a compatibility conversion from long.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public static implicit operator Gauge32(long value)

   :type value: ``Int64``

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.Gauge32`

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Gauge32.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Gauge32.cs#L47>`__

