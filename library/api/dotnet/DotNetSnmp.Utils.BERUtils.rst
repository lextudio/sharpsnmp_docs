BERUtils Class
==============

.. dn:class:: DotNetSnmp.Utils.BERUtils

   Provides helper methods for BERUtils.

   .. code-block:: csharp

      public static class BERUtils

**Namespace:** ``DotNetSnmp.Utils``

**Inheritance:** Object → ``BERUtils``

**Source:** `SharpSnmpLib/Utils/BERUtils.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Utils/BERUtils.cs#L95>`__

Methods
-------

Dump(ReadOnlyMemory<Byte>, Boolean)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Utils.BERUtils.Dump(System.ReadOnlyMemory{System.Byte},System.Boolean)

   Decodes BER bytes into a list of tagged members for inspection and diagnostics.

   .. code-block:: csharp

      public static IList<AsnMember> Dump(ReadOnlyMemory<byte> berEncodedBytes, bool colorize = true)

   :type berEncodedBytes: ``ReadOnlyMemory<Byte>``
   :type colorize: ``Boolean``

   :rtype: ``IList<AsnMember>``

**Source:** `SharpSnmpLib/Utils/BERUtils.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Utils/BERUtils.cs#L108>`__

