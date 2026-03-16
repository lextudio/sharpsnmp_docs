TripleDESPrivacyProvider Class
==============================

.. dn:class:: DotNetSnmp.Protocol.V3.Security.Privacy.TripleDESPrivacyProvider

   Implementation of Triple DES (3DES) privacy protocol for SNMPv3.

   .. code-block:: csharp

      public class TripleDESPrivacyProvider : PrivacyProviderBase, IPrivacyProvider

**Namespace:** ``DotNetSnmp.Protocol.V3.Security.Privacy``

**Inheritance:** Object → PrivacyProviderBase → ``TripleDESPrivacyProvider``

**Source:** `SharpSnmpLib/V3/Security/Privacy/TripleDESPrivacyProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/TripleDESPrivacyProvider.cs#L10>`__

Constructors
------------

TripleDESPrivacyProvider(in IAuthenticationProvider, in ReadOnlyMemory<Byte>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Protocol.V3.Security.Privacy.TripleDESPrivacyProvider..ctor(DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider@,System.ReadOnlyMemory{System.Byte}@)

   Initializes a new instance of TripleDESPrivacyProvider.

   .. code-block:: csharp

      public TripleDESPrivacyProvider(in IAuthenticationProvider authenticationService, in ReadOnlyMemory<byte> passcode)

   :type authenticationService: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider`
   :type passcode: ``ReadOnlyMemory<Byte>``

**Source:** `SharpSnmpLib/V3/Security/Privacy/TripleDESPrivacyProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/TripleDESPrivacyProvider.cs#L59>`__

Methods
-------

DecryptScopedPdu(in ReadOnlyMemory<Byte>, in UsmSecurityParameters, Span<Byte>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Security.Privacy.TripleDESPrivacyProvider.DecryptScopedPdu(System.ReadOnlyMemory{System.Byte}@,DotNetSnmp.Protocol.V3.Security.UsmSecurityParameters@,System.Span{System.Byte})

   Decrypts an encrypted scoped PDU payload into plaintext bytes.

   .. code-block:: csharp

      public override void DecryptScopedPdu(in ReadOnlyMemory<byte> encryptedPdu, in UsmSecurityParameters parameters, Span<byte> decryptedPdu)

   :type encryptedPdu: ``ReadOnlyMemory<Byte>``
   :type parameters: :dn:cls:`~DotNetSnmp.Protocol.V3.Security.UsmSecurityParameters`
   :type decryptedPdu: ``Span<Byte>``

**Source:** `SharpSnmpLib/V3/Security/Privacy/TripleDESPrivacyProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/TripleDESPrivacyProvider.cs#L154>`__

EncryptScopedPdu(in ReadOnlyMemory<Byte>, in UsmSecurityParameters, Span<Byte>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Security.Privacy.TripleDESPrivacyProvider.EncryptScopedPdu(System.ReadOnlyMemory{System.Byte}@,DotNetSnmp.Protocol.V3.Security.UsmSecurityParameters@,System.Span{System.Byte})

   Encrypts a scoped PDU payload and returns the number of bytes written.

   .. code-block:: csharp

      public override int EncryptScopedPdu(in ReadOnlyMemory<byte> scopedPdu, in UsmSecurityParameters parameters, Span<byte> encryptedScopedPdu)

   :type scopedPdu: ``ReadOnlyMemory<Byte>``
   :type parameters: :dn:cls:`~DotNetSnmp.Protocol.V3.Security.UsmSecurityParameters`
   :type encryptedScopedPdu: ``Span<Byte>``

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/V3/Security/Privacy/TripleDESPrivacyProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/TripleDESPrivacyProvider.cs#L67>`__

ExtendShortKey(ReadOnlySpan<Byte>, Int32, IAuthenticationProvider, ReadOnlyMemory<Byte>, Span<Byte>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Security.Privacy.TripleDESPrivacyProvider.ExtendShortKey(System.ReadOnlySpan{System.Byte},System.Int32,DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider,System.ReadOnlyMemory{System.Byte},System.Span{System.Byte})

   Extends a key that is shorter than the required length using a key localization procedure.

   .. code-block:: csharp

      public static void ExtendShortKey(ReadOnlySpan<byte> privKey, int keyLength, IAuthenticationProvider authenticationService, ReadOnlyMemory<byte> engineId, Span<byte> destination)

   :param privKey: The source key to extend
   :type privKey: ``ReadOnlySpan<Byte>``
   :param keyLength: The required key length in bytes
   :type keyLength: ``Int32``
   :param authenticationService: The authentication service to use for key derivation
   :type authenticationService: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider`
   :param engineId: The engine ID to use for localization
   :type engineId: ``ReadOnlyMemory<Byte>``
   :param destination: The destination buffer where the extended key will be stored
   :type destination: ``Span<Byte>``

**Source:** `SharpSnmpLib/V3/Security/Privacy/TripleDESPrivacyProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/TripleDESPrivacyProvider.cs#L22>`__

