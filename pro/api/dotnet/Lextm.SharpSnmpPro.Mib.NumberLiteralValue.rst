NumberLiteralValue Class
========================

.. dn:class:: Lextm.SharpSnmpPro.Mib.NumberLiteralValue

   Represents a numeric literal value for SMI (Structure of Management Information). Supports both signed and unsigned values.

   .. code-block:: csharp

      public class NumberLiteralValue : ISmiValue

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``NumberLiteralValue``

Constructors
------------

NumberLiteralValue(Int64)
~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.NumberLiteralValue..ctor(System.Int64)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.NumberLiteralValue`` class with a signed value.

   .. code-block:: csharp

      public NumberLiteralValue(long value)

   :param value: The signed value.
   :type value: ``Int64``

NumberLiteralValue(UInt64)
~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.NumberLiteralValue..ctor(System.UInt64)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.NumberLiteralValue`` class with an unsigned value.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public NumberLiteralValue(ulong value)

   :param value: The unsigned value.
   :type value: ``UInt64``

Properties
----------

UnsignedValue
~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.NumberLiteralValue.UnsignedValue

   Gets or sets the unsigned value, if applicable.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public ulong? UnsignedValue { get; set; }

   :rtype: ``Nullable<UInt64>``

Value
~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.NumberLiteralValue.Value

   Gets or sets the signed value, if applicable.

   .. code-block:: csharp

      public long? Value { get; set; }

   :rtype: ``Nullable<Int64>``

Methods
-------

ToString()
~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.NumberLiteralValue.ToString

   .. code-block:: csharp

      public override string ToString()

   :rtype: ``String``

