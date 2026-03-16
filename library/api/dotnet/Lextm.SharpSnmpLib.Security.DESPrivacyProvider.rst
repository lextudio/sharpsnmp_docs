DESPrivacyProvider Class
========================

.. dn:class:: Lextm.SharpSnmpLib.Security.DESPrivacyProvider

   Represents the DESPrivacyProvider type.

   .. code-block:: csharp

      public sealed class DESPrivacyProvider : DESPrivacyProvider, IPrivacyProvider

**Namespace:** ``Lextm.SharpSnmpLib.Security``

**Inheritance:** Object → PrivacyProviderBase → DESPrivacyProvider → ``DESPrivacyProvider``

**Source:** `SharpSnmpLib/Security/ProviderCompatibility.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/ProviderCompatibility.cs#L126>`__

Constructors
------------

DESPrivacyProvider(Nullable<OctetString>, IAuthenticationProvider)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Security.DESPrivacyProvider..ctor(System.Nullable{DotNetSnmp.Asn1.SyntaxObjects.OctetString},DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider)

   Initializes a new instance of DESPrivacyProvider.

   .. code-block:: csharp

      public DESPrivacyProvider(OctetString? passphrase, IAuthenticationProvider authenticationProvider)

   :type passphrase: ``Nullable<OctetString>``
   :type authenticationProvider: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider`

**Source:** `SharpSnmpLib/Security/ProviderCompatibility.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/ProviderCompatibility.cs#L154>`__

Properties
----------

IsSupported
~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Security.DESPrivacyProvider.IsSupported

   Represents this member.

   .. code-block:: csharp

      public static bool IsSupported { get; }

   :rtype: ``Boolean``

**Source:** `SharpSnmpLib/Security/ProviderCompatibility.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/ProviderCompatibility.cs#L135>`__

Methods
-------

Decrypt(Byte[], Byte[], Byte[])
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Security.DESPrivacyProvider.Decrypt(System.Byte[],System.Byte[],System.Byte[])

   Decrypts scoped PDU payload bytes using legacy DES helper signature.

   .. code-block:: csharp

      public static byte[] Decrypt(byte[] encryptedData, byte[] key, byte[] privacyParameters)

   :type encryptedData: ``Byte[]``
   :type key: ``Byte[]``
   :type privacyParameters: ``Byte[]``

   :rtype: ``Byte[]``

**Source:** `SharpSnmpLib/Security/ProviderCompatibility.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/ProviderCompatibility.cs#L218>`__

Encrypt(Byte[], Byte[], Byte[])
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Security.DESPrivacyProvider.Encrypt(System.Byte[],System.Byte[],System.Byte[])

   Encrypts scoped PDU payload bytes using legacy DES helper signature.

   .. code-block:: csharp

      public static byte[] Encrypt(byte[] unencryptedData, byte[] key, byte[] privacyParameters)

   :type unencryptedData: ``Byte[]``
   :type key: ``Byte[]``
   :type privacyParameters: ``Byte[]``

   :rtype: ``Byte[]``

**Source:** `SharpSnmpLib/Security/ProviderCompatibility.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/ProviderCompatibility.cs#L168>`__

