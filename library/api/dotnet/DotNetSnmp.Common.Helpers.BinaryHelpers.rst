BinaryHelpers Class
===================

.. dn:class:: DotNetSnmp.Common.Helpers.BinaryHelpers

   Provides helpers for writing integer values in network byte order (big-endian). Use these helpers when building SNMP BER payloads and headers.

   .. code-block:: csharp

      public static class BinaryHelpers

**Namespace:** ``DotNetSnmp.Common.Helpers``

**Inheritance:** Object → ``BinaryHelpers``

**Source:** `SharpSnmpLib/Common/BinaryHelpers.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/BinaryHelpers.cs#L8>`__

Methods
-------

CopyBytesMostSignificantFirst(Int16, Span<Byte>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Common.Helpers.BinaryHelpers.CopyBytesMostSignificantFirst(System.Int16,System.Span{System.Byte})

   Copies i to destination as a big-endian 2-byte value.

   .. code-block:: csharp

      public static void CopyBytesMostSignificantFirst(short i, Span<byte> destination)

   :type i: ``Int16``
   :type destination: ``Span<Byte>``

**Source:** `SharpSnmpLib/Common/BinaryHelpers.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/BinaryHelpers.cs#L40>`__

CopyBytesMostSignificantFirst(Int32, Span<Byte>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Common.Helpers.BinaryHelpers.CopyBytesMostSignificantFirst(System.Int32,System.Span{System.Byte})

   Copies i to destination as a big-endian 4-byte value.

   .. code-block:: csharp

      public static void CopyBytesMostSignificantFirst(int i, Span<byte> destination)

   :type i: ``Int32``
   :type destination: ``Span<Byte>``

**Source:** `SharpSnmpLib/Common/BinaryHelpers.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/BinaryHelpers.cs#L60>`__

CopyBytesMostSignificantFirst(Int64, Span<Byte>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Common.Helpers.BinaryHelpers.CopyBytesMostSignificantFirst(System.Int64,System.Span{System.Byte})

   Copies i to destination as a big-endian 8-byte value.

   .. code-block:: csharp

      public static void CopyBytesMostSignificantFirst(long i, Span<byte> destination)

   :type i: ``Int64``
   :type destination: ``Span<Byte>``

**Source:** `SharpSnmpLib/Common/BinaryHelpers.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/BinaryHelpers.cs#L84>`__

GetBytesMostSignificantFirst(Int32)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Common.Helpers.BinaryHelpers.GetBytesMostSignificantFirst(System.Int32)

   Returns a 4-byte big-endian representation of i.

   .. code-block:: csharp

      public static byte[] GetBytesMostSignificantFirst(int i)

   :type i: ``Int32``

   :rtype: ``Byte[]``

**Source:** `SharpSnmpLib/Common/BinaryHelpers.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/BinaryHelpers.cs#L13>`__

GetBytesMostSignificantFirst(Int64)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Common.Helpers.BinaryHelpers.GetBytesMostSignificantFirst(System.Int64)

   Returns an 8-byte big-endian representation of i.

   .. code-block:: csharp

      public static byte[] GetBytesMostSignificantFirst(long i)

   :type i: ``Int64``

   :rtype: ``Byte[]``

**Source:** `SharpSnmpLib/Common/BinaryHelpers.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/BinaryHelpers.cs#L25>`__

