DataFactory Class
=================

.. dn:class:: Lextm.SharpSnmpLib.DataFactory

   Factory that creates ASN.1 data instances from encoded bytes.

   .. code-block:: csharp

      public static class DataFactory

**Namespace:** ``Lextm.SharpSnmpLib``

**Inheritance:** Object → ``DataFactory``

**Source:** `SharpSnmpLib/DataFactory.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/DataFactory.cs#L13>`__

Methods
-------

CreateSnmpData(Byte[], Int32, Int32)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.DataFactory.CreateSnmpData(System.Byte[],System.Int32,System.Int32)

   Creates ASN.1 data from a BER-encoded buffer slice.

   .. code-block:: csharp

      public static IAsnSerializable CreateSnmpData(byte[] buffer, int index, int count)

   :type buffer: ``Byte[]``
   :type index: ``Int32``
   :type count: ``Int32``

   :rtype: :dn:iface:`~DotNetSnmp.Asn1.Serialization.IAsnSerializable`

**Source:** `SharpSnmpLib/DataFactory.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/DataFactory.cs#L31>`__

CreateSnmpData(Byte[])
~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.DataFactory.CreateSnmpData(System.Byte[])

   Creates ASN.1 data from a full BER-encoded buffer.

   .. code-block:: csharp

      public static IAsnSerializable CreateSnmpData(byte[] buffer)

   :type buffer: ``Byte[]``

   :rtype: :dn:iface:`~DotNetSnmp.Asn1.Serialization.IAsnSerializable`

**Source:** `SharpSnmpLib/DataFactory.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/DataFactory.cs#L18>`__

CreateSnmpData(Int32, Stream)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.DataFactory.CreateSnmpData(System.Int32,System.IO.Stream)

   Creates ASN.1 data from type + payload stream (legacy overload).

   .. code-block:: csharp

      public static IAsnSerializable CreateSnmpData(int type, Stream stream)

   :type type: ``Int32``
   :type stream: ``Stream``

   :rtype: :dn:iface:`~DotNetSnmp.Asn1.Serialization.IAsnSerializable`

**Source:** `SharpSnmpLib/DataFactory.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/DataFactory.cs#L80>`__

CreateSnmpData(Stream)
~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.DataFactory.CreateSnmpData(System.IO.Stream)

   Creates ASN.1 data from a stream containing one BER value.

   .. code-block:: csharp

      public static IAsnSerializable CreateSnmpData(Stream stream)

   :type stream: ``Stream``

   :rtype: :dn:iface:`~DotNetSnmp.Asn1.Serialization.IAsnSerializable`

**Source:** `SharpSnmpLib/DataFactory.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/DataFactory.cs#L59>`__

