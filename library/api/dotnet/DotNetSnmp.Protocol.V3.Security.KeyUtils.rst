KeyUtils Class
==============

.. dn:class:: DotNetSnmp.Protocol.V3.Security.KeyUtils

   Provides helper methods for KeyUtils.

   .. code-block:: csharp

      public static class KeyUtils

**Namespace:** ``DotNetSnmp.Protocol.V3.Security``

**Inheritance:** Object → ``KeyUtils``

**Source:** `SharpSnmpLib/V3/Security/KeyUtils.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/KeyUtils.cs#L7>`__

Fields
------

UsmExpandedPassphraseLengthInBytes
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:field:: DotNetSnmp.Protocol.V3.Security.KeyUtils.UsmExpandedPassphraseLengthInBytes

   Represents this member.

   .. code-block:: csharp

      public const int UsmExpandedPassphraseLengthInBytes = 1048576

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/V3/Security/KeyUtils.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/KeyUtils.cs#L12>`__

UsmHashBlockSizeInBytes
~~~~~~~~~~~~~~~~~~~~~~~

.. dn:field:: DotNetSnmp.Protocol.V3.Security.KeyUtils.UsmHashBlockSizeInBytes

   Represents this member.

   .. code-block:: csharp

      public const int UsmHashBlockSizeInBytes = 64

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/V3/Security/KeyUtils.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/KeyUtils.cs#L17>`__

UsmMinPassPhraseLen
~~~~~~~~~~~~~~~~~~~

.. dn:field:: DotNetSnmp.Protocol.V3.Security.KeyUtils.UsmMinPassPhraseLen

   Represents this member.

   .. code-block:: csharp

      public const int UsmMinPassPhraseLen = 8

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/V3/Security/KeyUtils.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/KeyUtils.cs#L22>`__

Methods
-------

GenerateLocalizedKey(in ReadOnlySpan<Byte>, in ReadOnlySpan<Byte>, IncrementalHash, Span<Byte>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Security.KeyUtils.GenerateLocalizedKey(System.ReadOnlySpan{System.Byte}@,System.ReadOnlySpan{System.Byte}@,System.Security.Cryptography.IncrementalHash,System.Span{System.Byte})

   Convert passphrase into a localized master user key, Kul, according to the algorithm given in RFC 2274 concerning the SNMPv3 User Security Model(USM) as follows: Expand the passphrase to fill the passphrase buffer space, if necessary, concatenation as many duplicates as possible of P to itself. If P is larger than the buffer space, truncate it to fit. Then hash the result with the given hash provider. Finally localize the produced digest with engineId

   .. code-block:: csharp

      public static void GenerateLocalizedKey(in ReadOnlySpan<byte> passphrase, in ReadOnlySpan<byte> engineId, IncrementalHash hash, Span<byte> destination)

   :type passphrase: ``ReadOnlySpan<Byte>``
   :type engineId: ``ReadOnlySpan<Byte>``
   :type hash: ``IncrementalHash``
   :type destination: ``Span<Byte>``

**Source:** `SharpSnmpLib/V3/Security/KeyUtils.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/KeyUtils.cs#L36>`__

