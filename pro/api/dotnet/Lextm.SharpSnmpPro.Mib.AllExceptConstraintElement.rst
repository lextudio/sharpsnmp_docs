AllExceptConstraintElement Class
================================

.. dn:class:: Lextm.SharpSnmpPro.Mib.AllExceptConstraintElement

   Represents a constraint element that matches all values except those specified by the given constraint.

   .. code-block:: csharp

      public class AllExceptConstraintElement : ConstraintElement

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ConstraintElement → ``AllExceptConstraintElement``

Constructors
------------

AllExceptConstraintElement(ConstraintElement)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.AllExceptConstraintElement..ctor(Lextm.SharpSnmpPro.Mib.ConstraintElement)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.AllExceptConstraintElement`` class with the specified constraint to exclude.

   .. code-block:: csharp

      public AllExceptConstraintElement(ConstraintElement constraintElement)

   :param constraintElement: The constraint element to be excluded.
   :type constraintElement: :dn:cls:`~Lextm.SharpSnmpPro.Mib.ConstraintElement`

