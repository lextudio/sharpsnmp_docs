Constraint Class
================

.. dn:class:: Lextm.SharpSnmpPro.Mib.Constraint

   Represents a constraint that can be applied to SNMP data, consisting of element set specifications and exception specifications.

   .. code-block:: csharp

      public class Constraint

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``Constraint``

Properties
----------

ElementSetSpecs
~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Constraint.ElementSetSpecs

   Gets or sets the element set specifications that define the main constraint.

   .. code-block:: csharp

      public ElementSetRange ElementSetSpecs { get; set; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.ElementSetRange`

ExceptionSpec
~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Constraint.ExceptionSpec

   Gets or sets the exception specification that defines exceptions to the main constraint.

   .. code-block:: csharp

      public ExceptionSpec ExceptionSpec { get; set; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.ExceptionSpec`

Methods
-------

Verify(IAsnSerializable)
~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Constraint.Verify(DotNetSnmp.Asn1.Serialization.IAsnSerializable)

   Verifies whether the specified SNMP data satisfies the constraint, including element set and exception specifications.

   .. code-block:: csharp

      public bool Verify(IAsnSerializable data)

   :param data: The SNMP data to verify.
   :type data: :any:`IAsnSerializable <DotNetSnmp.Asn1.Serialization.IAsnSerializable>`

   :returns: true if the data satisfies the constraint; otherwise, false.
   :rtype: ``Boolean``

