Integer32 Struct
================

.. dn:struct:: DotNetSnmp.Asn1.SyntaxObjects.Integer32

   Represents the Integer32 type.

   .. code-block:: csharp

      public readonly record struct Integer32(int Value) : IAsnSerializable, IEquatable<Integer32>

**Namespace:** ``DotNetSnmp.Asn1.SyntaxObjects``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Integer32.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Integer32.cs#L8>`__

Constructors
------------

Integer32(Int32)
~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Asn1.SyntaxObjects.Integer32..ctor(System.Int32)

   Represents the Integer32 type.

   .. code-block:: csharp

      public Integer32(int Value)

   :type Value: ``Int32``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Integer32.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Integer32.cs#L8>`__

Properties
----------

Value
~~~~~

.. dn:property:: DotNetSnmp.Asn1.SyntaxObjects.Integer32.Value

   .. code-block:: csharp

      public int Value { get; init; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Integer32.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Integer32.cs#L8>`__

Zero
~~~~

.. dn:property:: DotNetSnmp.Asn1.SyntaxObjects.Integer32.Zero

   Zero value.

   .. code-block:: csharp

      public static Integer32 Zero { get; }

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.Integer32`

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Integer32.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Integer32.cs#L13>`__

Methods
-------

Deconstruct(out Int32)
~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.Integer32.Deconstruct(System.Int32@)

   Deconstructs the value into its components.

   .. code-block:: csharp

      public readonly void Deconstruct(scoped out int value)

   :type value: ``Int32``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Integer32.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Integer32.cs#L26>`__

ReadFrom(AsnReader)
~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.Integer32.ReadFrom(System.Formats.Asn1.AsnReader)

   Reads a value from an ASN.1 reader.

   .. code-block:: csharp

      public static Integer32 ReadFrom(AsnReader reader)

   :type reader: ``AsnReader``

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.Integer32`

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Integer32.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Integer32.cs#L39>`__

ToString()
~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.Integer32.ToString

   Returns a string representation of this value.

   .. code-block:: csharp

      public readonly override string ToString()

   :rtype: ``String``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Integer32.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Integer32.cs#L34>`__

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.Integer32.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public readonly void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Integer32.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Integer32.cs#L16>`__

Operators
---------

Implicit(Integer32 to Int32)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:operator:: DotNetSnmp.Asn1.SyntaxObjects.Integer32.op_Implicit(DotNetSnmp.Asn1.SyntaxObjects.Integer32)

   Performs a conversion to int.

   .. code-block:: csharp

      public static implicit operator int (Integer32 x)

   :type x: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.Integer32`

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Integer32.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Integer32.cs#L48>`__

Extension Methods
-----------------

- :dn:meth:`ToErrorCode <Lextm.SharpSnmpLib.CompatibilityExtensions.ToErrorCode>`
- :dn:meth:`ToInt32 <Lextm.SharpSnmpLib.CompatibilityExtensions.ToInt32>`
- :dn:meth:`TryToErrorCode <Lextm.SharpSnmpLib.CompatibilityExtensions.TryToErrorCode>`

