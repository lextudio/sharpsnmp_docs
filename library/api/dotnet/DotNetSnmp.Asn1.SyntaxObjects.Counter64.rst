Counter64 Struct
================

.. dn:struct:: DotNetSnmp.Asn1.SyntaxObjects.Counter64

   Represents the Counter64 type.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public readonly record struct Counter64(ulong Value) : IAsnSerializable, IEquatable<Counter64>

**Namespace:** ``DotNetSnmp.Asn1.SyntaxObjects``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Counter64.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Counter64.cs#L8>`__

Constructors
------------

Counter64(UInt64)
~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Asn1.SyntaxObjects.Counter64..ctor(System.UInt64)

   Represents the Counter64 type.

   .. code-block:: csharp

      public Counter64(ulong Value)

   :type Value: ``UInt64``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Counter64.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Counter64.cs#L8>`__

Properties
----------

Value
~~~~~

.. dn:property:: DotNetSnmp.Asn1.SyntaxObjects.Counter64.Value

   .. code-block:: csharp

      public ulong Value { get; init; }

   :rtype: ``UInt64``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Counter64.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Counter64.cs#L9>`__

Methods
-------

Deconstruct(out UInt64)
~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.Counter64.Deconstruct(System.UInt64@)

   Deconstructs the value into its components.

   .. code-block:: csharp

      public readonly void Deconstruct(scoped out ulong value)

   :type value: ``UInt64``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Counter64.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Counter64.cs#L33>`__

ReadFrom(AsnReader)
~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.Counter64.ReadFrom(System.Formats.Asn1.AsnReader)

   Reads a value from an ASN.1 reader.

   .. code-block:: csharp

      public static Counter64 ReadFrom(AsnReader reader)

   :type reader: ``AsnReader``

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.Counter64`

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Counter64.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Counter64.cs#L22>`__

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.Counter64.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public readonly void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Counter64.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Counter64.cs#L12>`__

Operators
---------

Implicit(Counter64 to UInt64)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:operator:: DotNetSnmp.Asn1.SyntaxObjects.Counter64.op_Implicit(DotNetSnmp.Asn1.SyntaxObjects.Counter64)

   Performs a conversion to ulong.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public static implicit operator ulong (Counter64 x)

   :type x: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.Counter64`

   :rtype: ``UInt64``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Counter64.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Counter64.cs#L41>`__

