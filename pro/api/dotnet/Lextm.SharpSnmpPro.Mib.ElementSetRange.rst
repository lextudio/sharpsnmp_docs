ElementSetRange Class
=====================

.. dn:class:: Lextm.SharpSnmpPro.Mib.ElementSetRange

   Represents a range of constraint elements, optionally containing an ellipsis.

   .. code-block:: csharp

      public class ElementSetRange

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``ElementSetRange``

Properties
----------

ContainsEllipsis
~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ElementSetRange.ContainsEllipsis

   Gets or sets a value indicating whether the range contains an ellipsis (...).

   .. code-block:: csharp

      public bool ContainsEllipsis { get; set; }

   :rtype: ``Boolean``

LeftElement
~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ElementSetRange.LeftElement

   Gets or sets the left constraint element of the range.

   .. code-block:: csharp

      public ConstraintElement LeftElement { get; set; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.ConstraintElement`

RightElement
~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ElementSetRange.RightElement

   Gets or sets the right constraint element of the range.

   .. code-block:: csharp

      public ConstraintElement RightElement { get; set; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.ConstraintElement`

Methods
-------

Verify(IAsnSerializable)
~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.ElementSetRange.Verify(DotNetSnmp.Asn1.Serialization.IAsnSerializable)

   Verifies whether the specified SNMP data satisfies the constraints of the range.

   .. code-block:: csharp

      public bool Verify(IAsnSerializable data)

   :param data: The SNMP data to verify.
   :type data: :any:`IAsnSerializable <DotNetSnmp.Asn1.Serialization.IAsnSerializable>`

   :returns: true if the data satisfies the constraints; otherwise, false.
   :rtype: ``Boolean``

