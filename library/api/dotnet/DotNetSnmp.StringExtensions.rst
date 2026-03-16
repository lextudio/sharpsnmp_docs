StringExtensions Class
======================

.. dn:class:: DotNetSnmp.StringExtensions

   Provides helper methods for StringExtensions.

   .. code-block:: csharp

      public static class StringExtensions

**Namespace:** ``DotNetSnmp``

**Inheritance:** Object → ``StringExtensions``

**Source:** `SharpSnmpLib/Common/StringExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/StringExtensions.cs#L7>`__

Methods
-------

GetBytesMemoryOrDefault(String, Encoding)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.StringExtensions.GetBytesMemoryOrDefault(System.String,System.Text.Encoding)

   Gets bytes Memory Or Default.

   .. code-block:: csharp

      public static ReadOnlyMemory<byte> GetBytesMemoryOrDefault(this string s, Encoding encoding)

   :type s: ``String``
   :type encoding: ``Encoding``

   :rtype: ``ReadOnlyMemory<Byte>``

**Source:** `SharpSnmpLib/Common/StringExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/StringExtensions.cs#L24>`__

GetBytesSpanOrDefault(String, Encoding)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.StringExtensions.GetBytesSpanOrDefault(System.String,System.Text.Encoding)

   Gets bytes Span Or Default.

   .. code-block:: csharp

      public static ReadOnlySpan<byte> GetBytesSpanOrDefault(this string s, Encoding encoding)

   :type s: ``String``
   :type encoding: ``Encoding``

   :rtype: ``ReadOnlySpan<Byte>``

**Source:** `SharpSnmpLib/Common/StringExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/StringExtensions.cs#L12>`__

