SizeConstraintElement Class
===========================

.. dn:class:: Lextm.SharpSnmpPro.Mib.SizeConstraintElement

   Represents a size constraint element for SNMP data.

   .. code-block:: csharp

      public class SizeConstraintElement : ConstraintElement

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ConstraintElement → ``SizeConstraintElement``

Constructors
------------

SizeConstraintElement(Constraint)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.SizeConstraintElement..ctor(Lextm.SharpSnmpPro.Mib.Constraint)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.SizeConstraintElement`` class with the specified constraint.

   .. code-block:: csharp

      public SizeConstraintElement(Constraint constraint)

   :param constraint: The constraint to associate with this element.
   :type constraint: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Constraint`

Properties
----------

Constraint
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.SizeConstraintElement.Constraint

   Gets or sets the constraint associated with this size constraint element.

   .. code-block:: csharp

      public Constraint Constraint { get; set; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Constraint`

Methods
-------

Verify(IAsnSerializable)
~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.SizeConstraintElement.Verify(DotNetSnmp.Asn1.Serialization.IAsnSerializable)

   Verifies whether the specified SNMP data satisfies the constraint.

   .. code-block:: csharp

      public override bool Verify(IAsnSerializable data)

   :param data: The SNMP data to verify.
   :type data: :any:`IAsnSerializable <DotNetSnmp.Asn1.Serialization.IAsnSerializable>`

   :returns: true if the data satisfies the constraint; otherwise, false.
   :rtype: ``Boolean``

