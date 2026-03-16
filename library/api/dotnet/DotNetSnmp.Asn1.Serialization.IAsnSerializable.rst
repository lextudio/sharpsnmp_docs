IAsnSerializable Interface
==========================

.. dn:interface:: DotNetSnmp.Asn1.Serialization.IAsnSerializable

   Defines the contract for values that can serialize themselves as ASN.1.

   .. code-block:: csharp

      public interface IAsnSerializable

**Namespace:** ``DotNetSnmp.Asn1.Serialization``

**Source:** `SharpSnmpLib/Asn1/IAsnSerializable.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/IAsnSerializable.cs#L9>`__

Properties
----------

TypeCode
~~~~~~~~

.. dn:property:: DotNetSnmp.Asn1.Serialization.IAsnSerializable.TypeCode

   Gets SNMP type code (legacy compatibility member).

   .. code-block:: csharp

      SnmpType TypeCode { get; }

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`

**Source:** `SharpSnmpLib/Asn1/IAsnSerializable.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/IAsnSerializable.cs#L20>`__

Methods
-------

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.Serialization.IAsnSerializable.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/Asn1/IAsnSerializable.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/IAsnSerializable.cs#L15>`__

