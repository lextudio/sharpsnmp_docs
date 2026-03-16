ValueRange Class
================

.. dn:class:: Lextm.SharpSnmpPro.Mib.ValueRange

   Represents a value range with optional minimum and maximum values and comparison options.

   .. code-block:: csharp

      public class ValueRange

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``ValueRange``

Properties
----------

GreaterThan
~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ValueRange.GreaterThan

   Gets or sets a value indicating whether the comparison should be greater than the maximum value.

   .. code-block:: csharp

      public bool GreaterThan { get; set; }

   :rtype: ``Boolean``

LessThan
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ValueRange.LessThan

   Gets or sets a value indicating whether the comparison should be less than the minimum value.

   .. code-block:: csharp

      public bool LessThan { get; set; }

   :rtype: ``Boolean``

MaxValue
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ValueRange.MaxValue

   Gets or sets the maximum value of the range.

   .. code-block:: csharp

      public ISmiValue MaxValue { get; set; }

   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiValue`

MinValue
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ValueRange.MinValue

   Gets or sets the minimum value of the range.

   .. code-block:: csharp

      public ISmiValue MinValue { get; set; }

   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiValue`

NoMaxValue
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ValueRange.NoMaxValue

   Gets or sets a value indicating whether there is no maximum value.

   .. code-block:: csharp

      public bool NoMaxValue { get; set; }

   :rtype: ``Boolean``

NoMinValue
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ValueRange.NoMinValue

   Gets or sets a value indicating whether there is no minimum value.

   .. code-block:: csharp

      public bool NoMinValue { get; set; }

   :rtype: ``Boolean``

Methods
-------

Verify(IAsnSerializable)
~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.ValueRange.Verify(DotNetSnmp.Asn1.Serialization.IAsnSerializable)

   Verifies whether the specified data falls within the defined value range.

   .. code-block:: csharp

      public bool Verify(IAsnSerializable data)

   :param data: The SNMP data to verify.
   :type data: :any:`IAsnSerializable <DotNetSnmp.Asn1.Serialization.IAsnSerializable>`

   :returns: true if the data is within the range; otherwise, false.
   :rtype: ``Boolean``

