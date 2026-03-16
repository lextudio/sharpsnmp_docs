QuadValue Class
===============

.. dn:class:: Lextm.SharpSnmpPro.Mib.QuadValue

   Represents a value composed of four :dn:cls:``~Lextm.SharpSnmpPro.Mib.NumberLiteralValue`` instances.

   .. code-block:: csharp

      public class QuadValue : ISmiValue

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``QuadValue``

Constructors
------------

QuadValue(NumberLiteralValue, NumberLiteralValue, NumberLiteralValue, NumberLiteralValue)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.QuadValue..ctor(Lextm.SharpSnmpPro.Mib.NumberLiteralValue,Lextm.SharpSnmpPro.Mib.NumberLiteralValue,Lextm.SharpSnmpPro.Mib.NumberLiteralValue,Lextm.SharpSnmpPro.Mib.NumberLiteralValue)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.QuadValue`` class.

   .. code-block:: csharp

      public QuadValue(NumberLiteralValue value1, NumberLiteralValue value2, NumberLiteralValue value3, NumberLiteralValue value4)

   :param value1: The first number literal value.
   :type value1: :dn:cls:`~Lextm.SharpSnmpPro.Mib.NumberLiteralValue`
   :param value2: The second number literal value.
   :type value2: :dn:cls:`~Lextm.SharpSnmpPro.Mib.NumberLiteralValue`
   :param value3: The third number literal value.
   :type value3: :dn:cls:`~Lextm.SharpSnmpPro.Mib.NumberLiteralValue`
   :param value4: The fourth number literal value.
   :type value4: :dn:cls:`~Lextm.SharpSnmpPro.Mib.NumberLiteralValue`

