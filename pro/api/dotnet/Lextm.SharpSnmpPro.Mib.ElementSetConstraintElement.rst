ElementSetConstraintElement Class
=================================

.. dn:class:: Lextm.SharpSnmpPro.Mib.ElementSetConstraintElement

   Represents a constraint element that wraps another :dn:cls:``~Lextm.SharpSnmpPro.Mib.ConstraintElement`` as part of an element set.

   .. code-block:: csharp

      public class ElementSetConstraintElement : ConstraintElement

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ConstraintElement → ``ElementSetConstraintElement``

Constructors
------------

ElementSetConstraintElement(ConstraintElement)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.ElementSetConstraintElement..ctor(Lextm.SharpSnmpPro.Mib.ConstraintElement)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.ElementSetConstraintElement`` class.

   .. code-block:: csharp

      public ElementSetConstraintElement(ConstraintElement constraintElement)

   :param constraintElement: The constraint element to wrap.
   :type constraintElement: :dn:cls:`~Lextm.SharpSnmpPro.Mib.ConstraintElement`

