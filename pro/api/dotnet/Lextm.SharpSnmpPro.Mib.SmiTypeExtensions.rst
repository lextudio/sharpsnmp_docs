SmiTypeExtensions Class
=======================

.. dn:class:: Lextm.SharpSnmpPro.Mib.SmiTypeExtensions

   Provides extension methods for working with :dn:iface:``~Lextm.SharpSnmpPro.Mib.ISmiType`` objects, enabling operations such as verification, decoding, and type resolution.

   .. code-block:: csharp

      public static class SmiTypeExtensions

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``SmiTypeExtensions``

Methods
-------

Decode(ISmiType, IAsnSerializable)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.SmiTypeExtensions.Decode(Lextm.SharpSnmpPro.Mib.ISmiType,DotNetSnmp.Asn1.Serialization.IAsnSerializable)

   Decodes the provided SNMP data into a human-readable string representation based on the specified SMI type.

   .. code-block:: csharp

      public static string Decode(this ISmiType type, IAsnSerializable data)

   :param type: The SMI type used to interpret and decode the SNMP data. Must implement :dn:iface:``~Lextm.SharpSnmpPro.Mib.ISmiType``.
   :type type: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiType`
   :param data: The SNMP data to decode. Cannot be ``null``.
   :type data: :any:`IAsnSerializable <DotNetSnmp.Asn1.Serialization.IAsnSerializable>`

   :returns: A string representation of the decoded SNMP data. If the data matches a named number in the SMI type, the result includes the name and value (e.g., &quot;Name(123)&quot;). Otherwise, the raw string representation of the data is returned.
   :rtype: ``String``

GetLastType(ISmiType)
~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.SmiTypeExtensions.GetLastType(Lextm.SharpSnmpPro.Mib.ISmiType)

   The true base type of a syntax.

   .. code-block:: csharp

      public static ISmiType GetLastType(this ISmiType type)

   :param type: A syntax.
   :type type: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiType`

   :returns: The true base type.
   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiType`

Verify(ISmiType, IAsnSerializable)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.SmiTypeExtensions.Verify(Lextm.SharpSnmpPro.Mib.ISmiType,DotNetSnmp.Asn1.Serialization.IAsnSerializable)

   Verifies the input data against the syntax.

   .. code-block:: csharp

      public static bool Verify(this ISmiType type, IAsnSerializable data)

   :param type: Syntax type.
   :type type: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiType`
   :param data: Input data.
   :type data: :any:`IAsnSerializable <DotNetSnmp.Asn1.Serialization.IAsnSerializable>`

   :returns: true if the data matches the syntax. Otherwise, false.
   :rtype: ``Boolean``

