DefinedValue Class
==================

.. dn:class:: Lextm.SharpSnmpPro.Mib.DefinedValue

   Represents a value defined in a specific module.

   .. code-block:: csharp

      public class DefinedValue : ISmiValue

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``DefinedValue``

Properties
----------

Module
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.DefinedValue.Module

   Gets or sets the module name where the value is defined.

   .. code-block:: csharp

      public string Module { get; set; }

   :rtype: ``String``

Value
~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.DefinedValue.Value

   Gets or sets the value name.

   .. code-block:: csharp

      public string Value { get; set; }

   :rtype: ``String``

Methods
-------

ToString()
~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.DefinedValue.ToString

   .. code-block:: csharp

      public override string ToString()

   :rtype: ``String``

