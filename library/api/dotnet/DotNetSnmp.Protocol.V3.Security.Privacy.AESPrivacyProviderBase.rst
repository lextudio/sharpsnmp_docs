AESPrivacyProviderBase Class
============================

.. dn:class:: DotNetSnmp.Protocol.V3.Security.Privacy.AESPrivacyProviderBase

   Base class for AES-based privacy protocols (AES-128, AES-192, AES-256).

   .. code-block:: csharp

      public abstract class AESPrivacyProviderBase : PrivacyProviderBase, IPrivacyProvider

**Namespace:** ``DotNetSnmp.Protocol.V3.Security.Privacy``

**Inheritance:** Object → PrivacyProviderBase → ``AESPrivacyProviderBase``

**Source:** `SharpSnmpLib/V3/Security/Privacy/AESPrivacyProviderBase.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/AESPrivacyProviderBase.cs#L10>`__

Constructors
------------

AESPrivacyProviderBase(IAuthenticationProvider, ReadOnlyMemory<Byte>, Int32)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Protocol.V3.Security.Privacy.AESPrivacyProviderBase..ctor(DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider,System.ReadOnlyMemory{System.Byte},System.Int32)

   Initializes a new instance of AESPrivacyProviderBase.

   .. code-block:: csharp

      protected AESPrivacyProviderBase(IAuthenticationProvider authenticationService, ReadOnlyMemory<byte> passcode, int keyLength)

   :type authenticationService: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider`
   :type passcode: ``ReadOnlyMemory<Byte>``
   :type keyLength: ``Int32``

**Source:** `SharpSnmpLib/V3/Security/Privacy/AESPrivacyProviderBase.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/AESPrivacyProviderBase.cs#L22>`__

Fields
------

MinimalBlockSize
~~~~~~~~~~~~~~~~

.. dn:field:: DotNetSnmp.Protocol.V3.Security.Privacy.AESPrivacyProviderBase.MinimalBlockSize

   Minimum AES block size in bytes.

   .. code-block:: csharp

      protected const int MinimalBlockSize = 16

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/V3/Security/Privacy/AESPrivacyProviderBase.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/AESPrivacyProviderBase.cs#L15>`__

Methods
-------

DecryptScopedPdu(in ReadOnlyMemory<Byte>, in UsmSecurityParameters, Span<Byte>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Security.Privacy.AESPrivacyProviderBase.DecryptScopedPdu(System.ReadOnlyMemory{System.Byte}@,DotNetSnmp.Protocol.V3.Security.UsmSecurityParameters@,System.Span{System.Byte})

   Decrypts an encrypted scoped PDU payload into plaintext bytes.

   .. code-block:: csharp

      public override void DecryptScopedPdu(in ReadOnlyMemory<byte> encryptedPdu, in UsmSecurityParameters parameters, Span<byte> decryptedPdu)

   :type encryptedPdu: ``ReadOnlyMemory<Byte>``
   :type parameters: :dn:cls:`~DotNetSnmp.Protocol.V3.Security.UsmSecurityParameters`
   :type decryptedPdu: ``Span<Byte>``

**Source:** `SharpSnmpLib/V3/Security/Privacy/AESPrivacyProviderBase.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/AESPrivacyProviderBase.cs#L101>`__

EncryptScopedPdu(in ReadOnlyMemory<Byte>, in UsmSecurityParameters, Span<Byte>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Security.Privacy.AESPrivacyProviderBase.EncryptScopedPdu(System.ReadOnlyMemory{System.Byte}@,DotNetSnmp.Protocol.V3.Security.UsmSecurityParameters@,System.Span{System.Byte})

   Encrypts a scoped PDU payload and returns the number of bytes written.

   .. code-block:: csharp

      public override int EncryptScopedPdu(in ReadOnlyMemory<byte> scopedPdu, in UsmSecurityParameters parameters, Span<byte> encryptedScopedPdu)

   :type scopedPdu: ``ReadOnlyMemory<Byte>``
   :type parameters: :dn:cls:`~DotNetSnmp.Protocol.V3.Security.UsmSecurityParameters`
   :type encryptedScopedPdu: ``Span<Byte>``

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/V3/Security/Privacy/AESPrivacyProviderBase.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/AESPrivacyProviderBase.cs#L32>`__

PrepareBuffer(Int32)
~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Security.Privacy.AESPrivacyProviderBase.PrepareBuffer(System.Int32)

   Allocates a temporary buffer for scoped-PDU encryption output.

   .. code-block:: csharp

      public override byte[] PrepareBuffer(int encodedLength)

   :type encodedLength: ``Int32``

   :rtype: ``Byte[]``

**Source:** `SharpSnmpLib/V3/Security/Privacy/AESPrivacyProviderBase.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/AESPrivacyProviderBase.cs#L193>`__

