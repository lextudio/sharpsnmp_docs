IncludeTypeConstraintElement Class
==================================

.. dn:class:: Lextm.SharpSnmpPro.Mib.IncludeTypeConstraintElement

   Represents a constraint element that includes or excludes a specific SMI type.

   .. code-block:: csharp

      public class IncludeTypeConstraintElement : ConstraintElement

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ConstraintElement → ``IncludeTypeConstraintElement``

Properties
----------

ConstraintType
~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.IncludeTypeConstraintElement.ConstraintType

   Gets or sets the SMI type used as the constraint.

   .. code-block:: csharp

      public ISmiType ConstraintType { get; set; }

   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiType`

Includes
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.IncludeTypeConstraintElement.Includes

   Gets or sets a value indicating whether the constraint includes (true) or excludes (false) the specified type.

   .. code-block:: csharp

      public bool Includes { get; set; }

   :rtype: ``Boolean``

