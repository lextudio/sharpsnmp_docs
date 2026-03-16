ConstraintElement Class
=======================

.. dn:class:: Lextm.SharpSnmpPro.Mib.ConstraintElement

   Represents an abstract base class for SNMP constraint elements.

   .. code-block:: csharp

      public abstract class ConstraintElement

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``ConstraintElement``

Properties
----------

Element
~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ConstraintElement.Element

   Gets or sets the next constraint element in the chain.

   .. code-block:: csharp

      public ConstraintElement Element { get; set; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.ConstraintElement`

ExceptConstraint
~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ConstraintElement.ExceptConstraint

   Gets or sets the constraint that, if satisfied, will cause this constraint to be excluded.

   .. code-block:: csharp

      public ConstraintElement ExceptConstraint { get; set; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.ConstraintElement`

Methods
-------

Verify(IAsnSerializable)
~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.ConstraintElement.Verify(DotNetSnmp.Asn1.Serialization.IAsnSerializable)

   Verifies whether the specified SNMP data satisfies the constraint.

   .. code-block:: csharp

      public virtual bool Verify(IAsnSerializable data)

   :param data: The SNMP data to verify.
   :type data: :any:`IAsnSerializable <DotNetSnmp.Asn1.Serialization.IAsnSerializable>`

   :returns: true if the data satisfies the constraint; otherwise, false.
   :rtype: ``Boolean``

