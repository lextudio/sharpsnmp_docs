FromConstraintElement Class
===========================

.. dn:class:: Lextm.SharpSnmpPro.Mib.FromConstraintElement

   Represents a constraint element that is constructed from a :dn:prop:``~Lextm.SharpSnmpPro.Mib.FromConstraintElement.Constraint`` instance.

   .. code-block:: csharp

      public class FromConstraintElement : ConstraintElement

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ConstraintElement → ``FromConstraintElement``

Constructors
------------

FromConstraintElement(Constraint)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.FromConstraintElement..ctor(Lextm.SharpSnmpPro.Mib.Constraint)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.FromConstraintElement`` class using the specified :dn:prop:``~Lextm.SharpSnmpPro.Mib.FromConstraintElement.Constraint``.

   .. code-block:: csharp

      public FromConstraintElement(Constraint constraint)

   :param constraint: The constraint to use for this element.
   :type constraint: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Constraint`

Properties
----------

Constraint
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.FromConstraintElement.Constraint

   Gets the wrapped FROM constraint.

   .. code-block:: csharp

      public Constraint Constraint { get; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Constraint`

Methods
-------

Verify(IAsnSerializable)
~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.FromConstraintElement.Verify(DotNetSnmp.Asn1.Serialization.IAsnSerializable)

   Verifies whether the specified SNMP data satisfies the constraint.

   .. code-block:: csharp

      public override bool Verify(IAsnSerializable data)

   :param data: The SNMP data to verify.
   :type data: :any:`IAsnSerializable <DotNetSnmp.Asn1.Serialization.IAsnSerializable>`

   :returns: true if the data satisfies the constraint; otherwise, false.
   :rtype: ``Boolean``

