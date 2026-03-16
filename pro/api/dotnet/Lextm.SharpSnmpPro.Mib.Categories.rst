Categories Class
================

.. dn:class:: Lextm.SharpSnmpPro.Mib.Categories

   Represents a set of SNMP MIB categories.

   .. code-block:: csharp

      public class Categories

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``Categories``

Properties
----------

AllCategories
~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Categories.AllCategories

   Gets or sets a value indicating whether all categories are included.

   .. code-block:: csharp

      public bool AllCategories { get; set; }

   :rtype: ``Boolean``

CategoryIds
~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Categories.CategoryIds

   Gets or sets the list of category identifiers.

   .. code-block:: csharp

      public IList<NamedBit> CategoryIds { get; set; }

   :rtype: ``IList<NamedBit>``

