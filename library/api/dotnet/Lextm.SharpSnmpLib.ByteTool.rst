ByteTool Class
==============

.. dn:class:: Lextm.SharpSnmpLib.ByteTool

   Helper utility that performs data conversions from/to bytes.

   .. code-block:: csharp

      public static class ByteTool

**Namespace:** ``Lextm.SharpSnmpLib``

**Inheritance:** Object → ``ByteTool``

**Source:** `SharpSnmpLib/ByteTool.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/ByteTool.cs#L9>`__

Methods
-------

Convert(Byte[])
~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.ByteTool.Convert(System.Byte[])

   Converts bytes into an uppercase hexadecimal string without separators.

   .. code-block:: csharp

      public static string Convert(this byte[] bytes)

   :rtype: ``String``

**Source:** `SharpSnmpLib/ByteTool.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/ByteTool.cs#L101>`__

Convert(IEnumerable<Char>)
~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.ByteTool.Convert(System.Collections.Generic.IEnumerable{System.Char})

   Converts a hexadecimal character sequence into bytes.

   .. code-block:: csharp

      [Obsolete("Use Convert(this string str) instead.")]
      public static byte[] Convert(this IEnumerable<char> description)

   :rtype: ``Byte[]``

**Source:** `SharpSnmpLib/ByteTool.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/ByteTool.cs#L45>`__

Convert(String)
~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.ByteTool.Convert(System.String)

   Converts a hexadecimal string into bytes.

   .. code-block:: csharp

      public static byte[] Convert(this string str)

   :rtype: ``Byte[]``

**Source:** `SharpSnmpLib/ByteTool.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/ByteTool.cs#L93>`__

ConvertDecimal(String)
~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.ByteTool.ConvertDecimal(System.String)

   Converts decimal.

   .. code-block:: csharp

      [Obsolete("Use Convert(this string str) instead.")]
      public static byte[] ConvertDecimal(string description)

   :type description: ``String``

   :rtype: ``Byte[]``

**Source:** `SharpSnmpLib/ByteTool.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/ByteTool.cs#L14>`__

