AsnReaderExtensions Class
=========================

.. dn:class:: DotNetSnmp.Asn1.AsnReaderExtensions

   Try to consume an OctetString, optionally asserting an expected value

   .. code-block:: csharp

      public static class AsnReaderExtensions

**Namespace:** ``DotNetSnmp.Asn1``

**Inheritance:** Object → ``AsnReaderExtensions``

**Source:** `SharpSnmpLib/Asn1/AsnReaderExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/AsnReaderExtensions.cs#L7>`__

Methods
-------

ConsumeInt32(AsnReader, Nullable<Int32>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.AsnReaderExtensions.ConsumeInt32(System.Formats.Asn1.AsnReader,System.Nullable{System.Int32})

   Try to consume an Int32, optionally asserting an expected value

   .. code-block:: csharp

      public static void ConsumeInt32(this AsnReader reader, int? expectedValue = default(int? ))

   :type expectedValue: ``Nullable<Int32>``

**Source:** `SharpSnmpLib/Asn1/AsnReaderExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/AsnReaderExtensions.cs#L31>`__

ConsumeOctetString(AsnReader, Nullable<ReadOnlyMemory<Byte>>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.AsnReaderExtensions.ConsumeOctetString(System.Formats.Asn1.AsnReader,System.Nullable{System.ReadOnlyMemory{System.Byte}})

   Reads an OCTET STRING and optionally validates its value.

   .. code-block:: csharp

      public static void ConsumeOctetString(this AsnReader reader, ReadOnlyMemory<byte>? expectedValue = default(ReadOnlyMemory<byte>? ))

   :type expectedValue: ``Nullable<ReadOnlyMemory<Byte>>``

**Source:** `SharpSnmpLib/Asn1/AsnReaderExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/AsnReaderExtensions.cs#L12>`__

