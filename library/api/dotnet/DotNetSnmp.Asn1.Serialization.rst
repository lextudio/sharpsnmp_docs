DotNetSnmp.Asn1.Serialization Namespace
=======================================

.. dn:namespace:: DotNetSnmp.Asn1.Serialization

Classes
-------

.. list-table::
   :header-rows: 1
   :widths: 30 70

   * - Type
     - Description
   * - :doc:`AsnTypes <DotNetSnmp.Asn1.Serialization.AsnTypes>`
     - Defines ASN.1 tags used by SNMP syntax values, including opaque extension tags.
   * - :doc:`SnmpAsnTags <DotNetSnmp.Asn1.Serialization.SnmpAsnTags>`
     - Defines ASN.1 context-specific tags used by SNMP PDUs and exception syntax values.
   * - :doc:`SnmpDecodeException <DotNetSnmp.Asn1.Serialization.SnmpDecodeException>`
     - The exception that is thrown when ASN.1 payload data cannot be decoded as valid SNMP data.

Interfaces
----------

.. list-table::
   :header-rows: 1
   :widths: 30 70

   * - Type
     - Description
   * - :doc:`IAsnSerializable <DotNetSnmp.Asn1.Serialization.IAsnSerializable>`
     - Defines the contract for values that can serialize themselves as ASN.1.

