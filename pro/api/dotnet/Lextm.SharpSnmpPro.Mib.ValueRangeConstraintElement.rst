ValueRangeConstraintElement Class
=================================

.. dn:class:: Lextm.SharpSnmpPro.Mib.ValueRangeConstraintElement

   Represents a constraint element that verifies whether SNMP data falls within a specified value range.

   .. code-block:: csharp

      public class ValueRangeConstraintElement : ConstraintElement

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ConstraintElement → ``ValueRangeConstraintElement``

Constructors
------------

ValueRangeConstraintElement(ValueRange)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.ValueRangeConstraintElement..ctor(Lextm.SharpSnmpPro.Mib.ValueRange)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.ValueRangeConstraintElement`` class with the specified value range.

   .. code-block:: csharp

      public ValueRangeConstraintElement(ValueRange valueRange)

   :param valueRange: The value range to use for verification.
   :type valueRange: :dn:cls:`~Lextm.SharpSnmpPro.Mib.ValueRange`

Properties
----------

ValueRange
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ValueRangeConstraintElement.ValueRange

   Gets or sets the value range used for verification.

   .. code-block:: csharp

      public ValueRange ValueRange { get; set; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.ValueRange`

Methods
-------

Verify(IAsnSerializable)
~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.ValueRangeConstraintElement.Verify(DotNetSnmp.Asn1.Serialization.IAsnSerializable)

   Verifies whether the specified SNMP data satisfies the constraint.

   .. code-block:: csharp

      public override bool Verify(IAsnSerializable data)

   :param data: The SNMP data to verify.
   :type data: :any:`IAsnSerializable <DotNetSnmp.Asn1.Serialization.IAsnSerializable>`

   :returns: true if the data satisfies the constraint; otherwise, false.
   :rtype: ``Boolean``

