AgentCapabilitiesModule Class
=============================

.. dn:class:: Lextm.SharpSnmpPro.Mib.AgentCapabilitiesModule

   Represents an agent capabilities module in an SNMP MIB.

   .. code-block:: csharp

      public class AgentCapabilitiesModule

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``AgentCapabilitiesModule``

Constructors
------------

AgentCapabilitiesModule(String)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.AgentCapabilitiesModule..ctor(System.String)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.AgentCapabilitiesModule`` class.

   .. code-block:: csharp

      public AgentCapabilitiesModule(string name)

   :param name: The name of the agent capabilities module.
   :type name: ``String``

Properties
----------

Includes
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.AgentCapabilitiesModule.Includes

   Gets the list of SMI values included in this agent capabilities module.

   .. code-block:: csharp

      public IList<ISmiValue> Includes { get; }

   :rtype: ``IList<ISmiValue>``

Value
~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.AgentCapabilitiesModule.Value

   Gets or sets the SMI value associated with this agent capabilities module.

   .. code-block:: csharp

      public ISmiValue Value { get; set; }

   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiValue`

Variations
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.AgentCapabilitiesModule.Variations

   Gets or sets the list of variations for this agent capabilities module.

   .. code-block:: csharp

      public IList<Variantion> Variations { get; set; }

   :rtype: ``IList<Variantion>``

