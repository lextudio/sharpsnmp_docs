MacAddressDecoder Class
=======================

.. dn:class:: Lextm.SharpSnmpPro.Mib.Decoders.MacAddressDecoder

   Decoder for MacAddress convention.

   .. code-block:: csharp

      public sealed class MacAddressDecoder : IDecoder

**Namespace:** ``Lextm.SharpSnmpPro.Mib.Decoders``

**Inheritance:** Object → ``MacAddressDecoder``

Properties
----------

Key
~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Decoders.MacAddressDecoder.Key

   Gets the key of decoder.

   .. code-block:: csharp

      public string Key { get; }

   :returns: The key.
   :rtype: ``String``

Methods
-------

Decode(IAsnSerializable)
~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Decoders.MacAddressDecoder.Decode(DotNetSnmp.Asn1.Serialization.IAsnSerializable)

   Decodes the specified data.

   .. code-block:: csharp

      public string Decode(IAsnSerializable data)

   :param data: The data.
   :type data: :any:`IAsnSerializable <DotNetSnmp.Asn1.Serialization.IAsnSerializable>`

   :rtype: ``String``

