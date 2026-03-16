CharDefinition Class
====================

.. dn:class:: Lextm.SharpSnmpPro.Mib.CharDefinition

   Represents a character definition in the MIB.

   .. code-block:: csharp

      public class CharDefinition

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``CharDefinition``

Constructors
------------

CharDefinition(ISmiValue)
~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.CharDefinition..ctor(Lextm.SharpSnmpPro.Mib.ISmiValue)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.CharDefinition`` class with the specified :dn:iface:``~Lextm.SharpSnmpPro.Mib.ISmiValue`` name.

   .. code-block:: csharp

      public CharDefinition(ISmiValue name)

   :param name: The name as an :dn:iface:``~Lextm.SharpSnmpPro.Mib.ISmiValue``.
   :type name: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiValue`

CharDefinition(String)
~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.CharDefinition..ctor(System.String)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.CharDefinition`` class with the specified string name.

   .. code-block:: csharp

      public CharDefinition(string name)

   :param name: The name as a string.
   :type name: ``String``

Properties
----------

Name
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.CharDefinition.Name

   Gets or sets the name of the character definition.

   .. code-block:: csharp

      public ISmiValue Name { get; set; }

   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiValue`

