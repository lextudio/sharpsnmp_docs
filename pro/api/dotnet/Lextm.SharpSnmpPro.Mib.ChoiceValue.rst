ChoiceValue Class
=================

.. dn:class:: Lextm.SharpSnmpPro.Mib.ChoiceValue

   Represents a choice value in an SMI (Structure of Management Information) context.

   .. code-block:: csharp

      public class ChoiceValue : ISmiValue

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``ChoiceValue``

Properties
----------

ContainsColon
~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ChoiceValue.ContainsColon

   Gets or sets a value indicating whether the name contains a colon.

   .. code-block:: csharp

      public bool ContainsColon { get; set; }

   :rtype: ``Boolean``

Name
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ChoiceValue.Name

   Gets or sets the name of the choice value.

   .. code-block:: csharp

      public string Name { get; set; }

   :rtype: ``String``

Value
~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ChoiceValue.Value

   Gets or sets the value of the choice. This should implement the :dn:iface:``~Lextm.SharpSnmpPro.Mib.ISmiValue`` interface.

   .. code-block:: csharp

      public ISmiValue Value { get; set; }

   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiValue`

