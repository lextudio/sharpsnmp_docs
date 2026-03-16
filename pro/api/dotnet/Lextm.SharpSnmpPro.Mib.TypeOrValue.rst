TypeOrValue Class
=================

.. dn:class:: Lextm.SharpSnmpPro.Mib.TypeOrValue

   Represents either an SMI type or an SMI value.

   .. code-block:: csharp

      public class TypeOrValue

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``TypeOrValue``

Constructors
------------

TypeOrValue(ISmiType)
~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.TypeOrValue..ctor(Lextm.SharpSnmpPro.Mib.ISmiType)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.TypeOrValue`` class with the specified SMI type.

   .. code-block:: csharp

      public TypeOrValue(ISmiType type)

   :param type: The SMI type.
   :type type: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiType`

TypeOrValue(ISmiValue)
~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.TypeOrValue..ctor(Lextm.SharpSnmpPro.Mib.ISmiValue)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.TypeOrValue`` class with the specified SMI value.

   .. code-block:: csharp

      public TypeOrValue(ISmiValue value)

   :param value: The SMI value.
   :type value: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiValue`

Properties
----------

Type
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.TypeOrValue.Type

   Gets the SMI type, if this instance represents a type; otherwise, null.

   .. code-block:: csharp

      public ISmiType Type { get; }

   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiType`

Value
~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.TypeOrValue.Value

   Gets the SMI value, if this instance represents a value; otherwise, null.

   .. code-block:: csharp

      public ISmiValue Value { get; }

   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiValue`

