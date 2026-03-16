ModuleCompliance Class
======================

.. dn:class:: Lextm.SharpSnmpPro.Mib.ModuleCompliance

   Represents a module compliance statement in an SNMP MIB.

   .. code-block:: csharp

      public class ModuleCompliance

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``ModuleCompliance``

Constructors
------------

ModuleCompliance()
~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.ModuleCompliance..ctor

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.ModuleCompliance`` class.

   .. code-block:: csharp

      public ModuleCompliance()

Properties
----------

Compliances
~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ModuleCompliance.Compliances

   Gets or sets the list of compliance statements for this module.

   .. code-block:: csharp

      public IList<Compliance> Compliances { get; set; }

   :rtype: ``IList<Compliance>``

MandatoryGroups
~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ModuleCompliance.MandatoryGroups

   Gets or sets the list of mandatory group values for this module compliance.

   .. code-block:: csharp

      public IList<ISmiValue> MandatoryGroups { get; set; }

   :rtype: ``IList<ISmiValue>``

Name
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ModuleCompliance.Name

   Gets or sets the name of the module compliance.

   .. code-block:: csharp

      public string Name { get; set; }

   :rtype: ``String``

Value
~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ModuleCompliance.Value

   Gets or sets the SMI value associated with this module compliance.

   .. code-block:: csharp

      public ISmiValue Value { get; set; }

   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiValue`

