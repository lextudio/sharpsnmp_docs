IDecoder Interface
==================

.. dn:interface:: Lextm.SharpSnmpPro.Mib.IDecoder

   Decoder interface. Decoders are used to convert received SNMP data to proper strings based on object syntax.

   .. code-block:: csharp

      public interface IDecoder

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

Properties
----------

Key
~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.IDecoder.Key

   Gets the key of decoder.

   .. code-block:: csharp

      string Key { get; }

   :returns: The key.
   :rtype: ``String``

Methods
-------

Decode(IAsnSerializable)
~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.IDecoder.Decode(DotNetSnmp.Asn1.Serialization.IAsnSerializable)

   Decodes the specified data.

   .. code-block:: csharp

      string Decode(IAsnSerializable data)

   :param data: The data.
   :type data: :any:`IAsnSerializable <DotNetSnmp.Asn1.Serialization.IAsnSerializable>`

   :rtype: ``String``

