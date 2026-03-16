SnmpDecodeException Class
=========================

.. dn:class:: DotNetSnmp.Asn1.Serialization.SnmpDecodeException

   The exception that is thrown when ASN.1 payload data cannot be decoded as valid SNMP data.

   .. code-block:: csharp

      public class SnmpDecodeException : Exception, ISerializable

**Namespace:** ``DotNetSnmp.Asn1.Serialization``

**Inheritance:** Object → Exception → ``SnmpDecodeException``

**Source:** `SharpSnmpLib/Asn1/SnmpDecodeException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SnmpDecodeException.cs#L5>`__

Constructors
------------

SnmpDecodeException(String?)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Asn1.Serialization.SnmpDecodeException..ctor(System.String)

   Initializes a new instance of the :dn:cls:``~DotNetSnmp.Asn1.Serialization.SnmpDecodeException`` class.

   .. code-block:: csharp

      public SnmpDecodeException(string? message)

   :param message: The message that describes the decode failure.
   :type message: ``String``

**Source:** `SharpSnmpLib/Asn1/SnmpDecodeException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SnmpDecodeException.cs#L11>`__

