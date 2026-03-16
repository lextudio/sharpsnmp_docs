Dump Class
==========

.. dn:class:: DotNetSnmp.Utils.Dump

   Provides helper methods for Dump.

   .. code-block:: csharp

      [ExcludeFromCodeCoverage]
      public static class Dump

**Namespace:** ``DotNetSnmp.Utils``

**Inheritance:** Object → ``Dump``

**Source:** `SharpSnmpLib/Utils/Dump.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Utils/Dump.cs#L9>`__

Methods
-------

BytesFromDumpString(String)
~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Utils.Dump.BytesFromDumpString(System.String)

   Parses a textual packet dump into raw bytes.

   .. code-block:: csharp

      public static byte[] BytesFromDumpString(string textualDump)

   :type textualDump: ``String``

   :rtype: ``Byte[]``

**Source:** `SharpSnmpLib/Utils/Dump.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Utils/Dump.cs#L24>`__

BytesFromHexString(String)
~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Utils.Dump.BytesFromHexString(System.String)

   Parses a hexadecimal string into raw bytes.

   .. code-block:: csharp

      public static byte[] BytesFromHexString(string hexString)

   :type hexString: ``String``

   :rtype: ``Byte[]``

**Source:** `SharpSnmpLib/Utils/Dump.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Utils/Dump.cs#L56>`__

BytesToHexString(Byte[])
~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Utils.Dump.BytesToHexString(System.Byte[])

   Converts raw bytes to an uppercase hexadecimal string without separators.

   .. code-block:: csharp

      public static string BytesToHexString(byte[] bytes)

   :type bytes: ``Byte[]``

   :rtype: ``String``

**Source:** `SharpSnmpLib/Utils/Dump.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Utils/Dump.cs#L70>`__

