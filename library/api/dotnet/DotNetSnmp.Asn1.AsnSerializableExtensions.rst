AsnSerializableExtensions Class
===============================

.. dn:class:: DotNetSnmp.Asn1.AsnSerializableExtensions

   Provides helper methods for AsnSerializableExtensions.

   .. code-block:: csharp

      public static class AsnSerializableExtensions

**Namespace:** ``DotNetSnmp.Asn1``

**Inheritance:** Object → ``AsnSerializableExtensions``

**Source:** `SharpSnmpLib/Asn1/AsnSerializableExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/AsnSerializableExtensions.cs#L8>`__

Methods
-------

Encode(IAsnSerializable, Span<Byte>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.AsnSerializableExtensions.Encode(DotNetSnmp.Asn1.Serialization.IAsnSerializable,System.Span{System.Byte})

   Encodes the value to BER bytes.

   .. code-block:: csharp

      public static int Encode(this IAsnSerializable obj, Span<byte> destination)

   :type obj: :dn:iface:`~DotNetSnmp.Asn1.Serialization.IAsnSerializable`
   :type destination: ``Span<Byte>``

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Asn1/AsnSerializableExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/AsnSerializableExtensions.cs#L23>`__

Encode(IAsnSerializable)
~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.AsnSerializableExtensions.Encode(DotNetSnmp.Asn1.Serialization.IAsnSerializable)

   Encodes the value to BER bytes.

   .. code-block:: csharp

      public static byte[] Encode(this IAsnSerializable obj)

   :type obj: :dn:iface:`~DotNetSnmp.Asn1.Serialization.IAsnSerializable`

   :rtype: ``Byte[]``

**Source:** `SharpSnmpLib/Asn1/AsnSerializableExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/AsnSerializableExtensions.cs#L13>`__

