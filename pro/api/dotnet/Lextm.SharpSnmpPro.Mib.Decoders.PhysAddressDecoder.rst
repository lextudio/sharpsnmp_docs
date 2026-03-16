PhysAddressDecoder Class
========================

.. dn:class:: Lextm.SharpSnmpPro.Mib.Decoders.PhysAddressDecoder

   Decoder for PhysAddress convention.

   .. code-block:: csharp

      public sealed class PhysAddressDecoder : IDecoder

**Namespace:** ``Lextm.SharpSnmpPro.Mib.Decoders``

**Inheritance:** Object → ``PhysAddressDecoder``

Properties
----------

Key
~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Decoders.PhysAddressDecoder.Key

   Gets the key of decoder.

   .. code-block:: csharp

      public string Key { get; }

   :returns: The key.
   :rtype: ``String``

Methods
-------

Decode(IAsnSerializable)
~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Decoders.PhysAddressDecoder.Decode(DotNetSnmp.Asn1.Serialization.IAsnSerializable)

   Decodes the specified data.

   .. code-block:: csharp

      public string Decode(IAsnSerializable data)

   :param data: The data.
   :type data: :any:`IAsnSerializable <DotNetSnmp.Asn1.Serialization.IAsnSerializable>`

   :rtype: ``String``

