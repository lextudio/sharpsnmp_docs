TupleValue Class
================

.. dn:class:: Lextm.SharpSnmpPro.Mib.TupleValue

   Represents a tuple of two :dn:cls:``~Lextm.SharpSnmpPro.Mib.NumberLiteralValue`` values.

   .. code-block:: csharp

      public class TupleValue : ISmiValue

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``TupleValue``

Constructors
------------

TupleValue(NumberLiteralValue, NumberLiteralValue)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.TupleValue..ctor(Lextm.SharpSnmpPro.Mib.NumberLiteralValue,Lextm.SharpSnmpPro.Mib.NumberLiteralValue)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.TupleValue`` class with two :dn:cls:``~Lextm.SharpSnmpPro.Mib.NumberLiteralValue`` values.

   .. code-block:: csharp

      public TupleValue(NumberLiteralValue value1, NumberLiteralValue value2)

   :param value1: The first value.
   :type value1: :dn:cls:`~Lextm.SharpSnmpPro.Mib.NumberLiteralValue`
   :param value2: The second value.
   :type value2: :dn:cls:`~Lextm.SharpSnmpPro.Mib.NumberLiteralValue`

Properties
----------

Value1
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.TupleValue.Value1

   Gets the first value of the tuple.

   .. code-block:: csharp

      public NumberLiteralValue Value1 { get; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.NumberLiteralValue`

Value2
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.TupleValue.Value2

   Gets the second value of the tuple.

   .. code-block:: csharp

      public NumberLiteralValue Value2 { get; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.NumberLiteralValue`

