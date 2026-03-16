ExceptionSpec Class
===================

.. dn:class:: Lextm.SharpSnmpPro.Mib.ExceptionSpec

   Represents an exception specification for SNMP MIB values.

   .. code-block:: csharp

      public class ExceptionSpec

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``ExceptionSpec``

Constructors
------------

ExceptionSpec(DefinedValue)
~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.ExceptionSpec..ctor(Lextm.SharpSnmpPro.Mib.DefinedValue)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.ExceptionSpec`` class with a defined value.

   .. code-block:: csharp

      public ExceptionSpec(DefinedValue value)

   :param value: The defined value.
   :type value: :dn:cls:`~Lextm.SharpSnmpPro.Mib.DefinedValue`

ExceptionSpec(ISmiType, ISmiValue)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.ExceptionSpec..ctor(Lextm.SharpSnmpPro.Mib.ISmiType,Lextm.SharpSnmpPro.Mib.ISmiValue)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.ExceptionSpec`` class with a specific SMI type and value.

   .. code-block:: csharp

      public ExceptionSpec(ISmiType smiType, ISmiValue value)

   :param smiType: The SMI type.
   :type smiType: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiType`
   :param value: The SMI value.
   :type value: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiValue`

ExceptionSpec(NumberLiteralValue)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.ExceptionSpec..ctor(Lextm.SharpSnmpPro.Mib.NumberLiteralValue)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.ExceptionSpec`` class with a numeric literal value.

   .. code-block:: csharp

      public ExceptionSpec(NumberLiteralValue value)

   :param value: The numeric literal value.
   :type value: :dn:cls:`~Lextm.SharpSnmpPro.Mib.NumberLiteralValue`

Methods
-------

Verify(IAsnSerializable)
~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.ExceptionSpec.Verify(DotNetSnmp.Asn1.Serialization.IAsnSerializable)

   Verifies whether the specified SNMP data matches the exception specification.

   .. code-block:: csharp

      public bool Verify(IAsnSerializable data)

   :param data: The SNMP data to verify.
   :type data: :any:`IAsnSerializable <DotNetSnmp.Asn1.Serialization.IAsnSerializable>`

   :returns: true if the data matches the exception specification; otherwise, false.
   :rtype: ``Boolean``

