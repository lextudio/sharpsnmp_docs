DecoderRegistry Class
=====================

.. dn:class:: Lextm.SharpSnmpPro.Mib.DecoderRegistry

   Registry for decoders.

   .. code-block:: csharp

      public static class DecoderRegistry

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``DecoderRegistry``

Methods
-------

GetDecoder(String)
~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.DecoderRegistry.GetDecoder(System.String)

   Gets a decoder by key.

   .. code-block:: csharp

      public static IDecoder GetDecoder(string key)

   :param key: The key.
   :type key: ``String``

   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.IDecoder`

Register(IDecoder)
~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.DecoderRegistry.Register(Lextm.SharpSnmpPro.Mib.IDecoder)

   Registers a new decoder.

   .. code-block:: csharp

      public static void Register(IDecoder decoder)

   :param decoder: The decoder to register.
   :type decoder: :dn:iface:`~Lextm.SharpSnmpPro.Mib.IDecoder`

