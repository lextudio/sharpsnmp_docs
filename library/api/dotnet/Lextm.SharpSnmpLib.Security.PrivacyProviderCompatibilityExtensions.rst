PrivacyProviderCompatibilityExtensions Class
============================================

.. dn:class:: Lextm.SharpSnmpLib.Security.PrivacyProviderCompatibilityExtensions

   Legacy extension helpers for privacy providers.

   .. code-block:: csharp

      [Obsolete("This type is for internal use only and may be removed in a future release.")]
      public static class PrivacyProviderCompatibilityExtensions

**Namespace:** ``Lextm.SharpSnmpLib.Security``

**Inheritance:** Object → ``PrivacyProviderCompatibilityExtensions``

**Source:** `SharpSnmpLib/Security/PrivacyProviderCompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/PrivacyProviderCompatibilityExtensions.cs#L17>`__

Methods
-------

Decrypt(AES192PrivacyProvider, Byte[], Byte[], Int32, Int32, Byte[])
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Security.PrivacyProviderCompatibilityExtensions.Decrypt(Lextm.SharpSnmpLib.Security.AES192PrivacyProvider,System.Byte[],System.Byte[],System.Int32,System.Int32,System.Byte[])

   Decrypts raw bytes using legacy AES192 helper signature.

   .. code-block:: csharp

      public static byte[] Decrypt(this AES192PrivacyProvider privacy, byte[] encryptedData, byte[] key, int engineBoots, int engineTime, byte[] privacyParameters)

   :type encryptedData: ``Byte[]``
   :type key: ``Byte[]``
   :type engineBoots: ``Int32``
   :type engineTime: ``Int32``
   :type privacyParameters: ``Byte[]``

   :rtype: ``Byte[]``

**Source:** `SharpSnmpLib/Security/PrivacyProviderCompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/PrivacyProviderCompatibilityExtensions.cs#L280>`__

Decrypt(AES256PrivacyProvider, Byte[], Byte[], Int32, Int32, Byte[])
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Security.PrivacyProviderCompatibilityExtensions.Decrypt(Lextm.SharpSnmpLib.Security.AES256PrivacyProvider,System.Byte[],System.Byte[],System.Int32,System.Int32,System.Byte[])

   Decrypts raw bytes using legacy AES256 helper signature.

   .. code-block:: csharp

      public static byte[] Decrypt(this AES256PrivacyProvider privacy, byte[] encryptedData, byte[] key, int engineBoots, int engineTime, byte[] privacyParameters)

   :type encryptedData: ``Byte[]``
   :type key: ``Byte[]``
   :type engineBoots: ``Int32``
   :type engineTime: ``Int32``
   :type privacyParameters: ``Byte[]``

   :rtype: ``Byte[]``

**Source:** `SharpSnmpLib/Security/PrivacyProviderCompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/PrivacyProviderCompatibilityExtensions.cs#L306>`__

Decrypt(AESPrivacyProvider, Byte[], Byte[], Int32, Int32, Byte[])
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Security.PrivacyProviderCompatibilityExtensions.Decrypt(Lextm.SharpSnmpLib.Security.AESPrivacyProvider,System.Byte[],System.Byte[],System.Int32,System.Int32,System.Byte[])

   Decrypts raw bytes using legacy AES helper signature.

   .. code-block:: csharp

      public static byte[] Decrypt(this AESPrivacyProvider privacy, byte[] encryptedData, byte[] key, int engineBoots, int engineTime, byte[] privacyParameters)

   :type encryptedData: ``Byte[]``
   :type key: ``Byte[]``
   :type engineBoots: ``Int32``
   :type engineTime: ``Int32``
   :type privacyParameters: ``Byte[]``

   :rtype: ``Byte[]``

**Source:** `SharpSnmpLib/Security/PrivacyProviderCompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/PrivacyProviderCompatibilityExtensions.cs#L254>`__

Decrypt(IPrivacyProvider, IAsnSerializable, SecurityParameters)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Security.PrivacyProviderCompatibilityExtensions.Decrypt(DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider,DotNetSnmp.Asn1.Serialization.IAsnSerializable,Lextm.SharpSnmpLib.SecurityParameters)

   Decrypts scope data using legacy compatibility signature.

   .. code-block:: csharp

      public static IAsnSerializable Decrypt(this IPrivacyProvider privacy, IAsnSerializable data, SecurityParameters parameters)

   :type data: :dn:iface:`~DotNetSnmp.Asn1.Serialization.IAsnSerializable`
   :type parameters: :dn:cls:`~Lextm.SharpSnmpLib.SecurityParameters`

   :rtype: :dn:iface:`~DotNetSnmp.Asn1.Serialization.IAsnSerializable`

**Source:** `SharpSnmpLib/Security/PrivacyProviderCompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/PrivacyProviderCompatibilityExtensions.cs#L115>`__

Encrypt(AES192PrivacyProvider, Byte[], Byte[], Int32, Int32, Byte[])
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Security.PrivacyProviderCompatibilityExtensions.Encrypt(Lextm.SharpSnmpLib.Security.AES192PrivacyProvider,System.Byte[],System.Byte[],System.Int32,System.Int32,System.Byte[])

   Encrypts raw bytes using legacy AES192 helper signature.

   .. code-block:: csharp

      public static byte[] Encrypt(this AES192PrivacyProvider privacy, byte[] unencryptedData, byte[] key, int engineBoots, int engineTime, byte[] privacyParameters)

   :type unencryptedData: ``Byte[]``
   :type key: ``Byte[]``
   :type engineBoots: ``Int32``
   :type engineTime: ``Int32``
   :type privacyParameters: ``Byte[]``

   :rtype: ``Byte[]``

**Source:** `SharpSnmpLib/Security/PrivacyProviderCompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/PrivacyProviderCompatibilityExtensions.cs#L267>`__

Encrypt(AES256PrivacyProvider, Byte[], Byte[], Int32, Int32, Byte[])
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Security.PrivacyProviderCompatibilityExtensions.Encrypt(Lextm.SharpSnmpLib.Security.AES256PrivacyProvider,System.Byte[],System.Byte[],System.Int32,System.Int32,System.Byte[])

   Encrypts raw bytes using legacy AES256 helper signature.

   .. code-block:: csharp

      public static byte[] Encrypt(this AES256PrivacyProvider privacy, byte[] unencryptedData, byte[] key, int engineBoots, int engineTime, byte[] privacyParameters)

   :type unencryptedData: ``Byte[]``
   :type key: ``Byte[]``
   :type engineBoots: ``Int32``
   :type engineTime: ``Int32``
   :type privacyParameters: ``Byte[]``

   :rtype: ``Byte[]``

**Source:** `SharpSnmpLib/Security/PrivacyProviderCompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/PrivacyProviderCompatibilityExtensions.cs#L293>`__

Encrypt(AESPrivacyProvider, Byte[], Byte[], Int32, Int32, Byte[])
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Security.PrivacyProviderCompatibilityExtensions.Encrypt(Lextm.SharpSnmpLib.Security.AESPrivacyProvider,System.Byte[],System.Byte[],System.Int32,System.Int32,System.Byte[])

   Encrypts raw bytes using legacy AES helper signature.

   .. code-block:: csharp

      public static byte[] Encrypt(this AESPrivacyProvider privacy, byte[] unencryptedData, byte[] key, int engineBoots, int engineTime, byte[] privacyParameters)

   :type unencryptedData: ``Byte[]``
   :type key: ``Byte[]``
   :type engineBoots: ``Int32``
   :type engineTime: ``Int32``
   :type privacyParameters: ``Byte[]``

   :rtype: ``Byte[]``

**Source:** `SharpSnmpLib/Security/PrivacyProviderCompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/PrivacyProviderCompatibilityExtensions.cs#L241>`__

Encrypt(IPrivacyProvider, IAsnSerializable, SecurityParameters)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Security.PrivacyProviderCompatibilityExtensions.Encrypt(DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider,DotNetSnmp.Asn1.Serialization.IAsnSerializable,Lextm.SharpSnmpLib.SecurityParameters)

   Encrypts scope data using legacy compatibility signature.

   .. code-block:: csharp

      public static IAsnSerializable Encrypt(this IPrivacyProvider privacy, IAsnSerializable data, SecurityParameters parameters)

   :type data: :dn:iface:`~DotNetSnmp.Asn1.Serialization.IAsnSerializable`
   :type parameters: :dn:cls:`~Lextm.SharpSnmpLib.SecurityParameters`

   :rtype: :dn:iface:`~DotNetSnmp.Asn1.Serialization.IAsnSerializable`

**Source:** `SharpSnmpLib/Security/PrivacyProviderCompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/PrivacyProviderCompatibilityExtensions.cs#L46>`__

ToSecurityLevel(IPrivacyProvider)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Security.PrivacyProviderCompatibilityExtensions.ToSecurityLevel(DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider)

   Converts provider settings to legacy security levels.

   .. code-block:: csharp

      public static Levels ToSecurityLevel(this IPrivacyProvider privacy)

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.Levels`

**Source:** `SharpSnmpLib/Security/PrivacyProviderCompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/PrivacyProviderCompatibilityExtensions.cs#L23>`__

