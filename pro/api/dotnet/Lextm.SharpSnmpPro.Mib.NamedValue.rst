NamedValue Class
================

.. dn:class:: Lextm.SharpSnmpPro.Mib.NamedValue

   Represents a named value pair for SNMP MIB entities.

   .. code-block:: csharp

      public class NamedValue

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``NamedValue``

Constructors
------------

NamedValue(String, ISmiValue)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.NamedValue..ctor(System.String,Lextm.SharpSnmpPro.Mib.ISmiValue)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.NamedValue`` class.

   .. code-block:: csharp

      public NamedValue(string name, ISmiValue smiValue)

   :param name: The name associated with the value.
   :type name: ``String``
   :param smiValue: The SMI value.
   :type smiValue: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiValue`

Properties
----------

Name
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.NamedValue.Name

   Gets or sets the name associated with the value.

   .. code-block:: csharp

      public string Name { get; set; }

   :rtype: ``String``

Value
~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.NamedValue.Value

   Gets or sets the SMI value.

   .. code-block:: csharp

      public ISmiValue Value { get; set; }

   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiValue`

