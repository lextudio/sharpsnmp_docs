WithComponentConstraintElement Class
====================================

.. dn:class:: Lextm.SharpSnmpPro.Mib.WithComponentConstraintElement

   Represents a constraint element with a component constraint in SNMP MIB definitions.

   .. code-block:: csharp

      public class WithComponentConstraintElement : ConstraintElement

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ConstraintElement → ``WithComponentConstraintElement``

Constructors
------------

WithComponentConstraintElement(Constraint)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.WithComponentConstraintElement..ctor(Lextm.SharpSnmpPro.Mib.Constraint)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.WithComponentConstraintElement`` class with the specified :dn:cls:``~Lextm.SharpSnmpPro.Mib.Constraint``.

   .. code-block:: csharp

      public WithComponentConstraintElement(Constraint constraint)

   :param constraint: The component constraint to associate with this element.
   :type constraint: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Constraint`

Properties
----------

ComponentConstraint
~~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.WithComponentConstraintElement.ComponentConstraint

   Gets the component constraint associated with this element.

   .. code-block:: csharp

      public Constraint ComponentConstraint { get; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Constraint`

