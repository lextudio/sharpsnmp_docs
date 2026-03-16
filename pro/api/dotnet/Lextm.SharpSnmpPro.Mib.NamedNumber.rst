NamedNumber Class
=================

.. dn:class:: Lextm.SharpSnmpPro.Mib.NamedNumber

   Represents a named number, which associates a name with a numeric or defined value.

   .. code-block:: csharp

      public class NamedNumber : ISmiValue

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``NamedNumber``

Constructors
------------

NamedNumber(String, DefinedValue)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.NamedNumber..ctor(System.String,Lextm.SharpSnmpPro.Mib.DefinedValue)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.NamedNumber`` class with a defined value.

   .. code-block:: csharp

      public NamedNumber(string name, DefinedValue value)

   :param name: The name associated with the value.
   :type name: ``String``
   :param value: The defined value.
   :type value: :dn:cls:`~Lextm.SharpSnmpPro.Mib.DefinedValue`

NamedNumber(String, NumberLiteralValue)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.NamedNumber..ctor(System.String,Lextm.SharpSnmpPro.Mib.NumberLiteralValue)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.NamedNumber`` class with a numeric value.

   .. code-block:: csharp

      public NamedNumber(string name, NumberLiteralValue value)

   :param name: The name associated with the value.
   :type name: ``String``
   :param value: The numeric value.
   :type value: :dn:cls:`~Lextm.SharpSnmpPro.Mib.NumberLiteralValue`

Properties
----------

Name
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.NamedNumber.Name

   Gets or sets the name associated with the value.

   .. code-block:: csharp

      public string Name { get; set; }

   :rtype: ``String``

Value
~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.NamedNumber.Value

   Gets or sets the value associated with the name.

   .. code-block:: csharp

      public ISmiValue Value { get; set; }

   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiValue`

