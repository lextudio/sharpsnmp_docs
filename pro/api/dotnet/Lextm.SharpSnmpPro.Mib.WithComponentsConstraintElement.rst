WithComponentsConstraintElement Class
=====================================

.. dn:class:: Lextm.SharpSnmpPro.Mib.WithComponentsConstraintElement

   Represents a WITH COMPONENTS constraint element in SNMP MIB definitions.

   .. code-block:: csharp

      public class WithComponentsConstraintElement : ConstraintElement

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ConstraintElement → ``WithComponentsConstraintElement``

Properties
----------

Ellipsis
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.WithComponentsConstraintElement.Ellipsis

   Gets or sets a value indicating whether the ellipsis (...) is present in the WITH COMPONENTS constraint.

   .. code-block:: csharp

      public bool Ellipsis { get; set; }

   :rtype: ``Boolean``

TypeConstraintList
~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.WithComponentsConstraintElement.TypeConstraintList

   Gets or sets the list of type constraint elements for the WITH COMPONENTS constraint.

   .. code-block:: csharp

      public IList<ConstraintElement> TypeConstraintList { get; set; }

   :rtype: ``IList<ConstraintElement>``

