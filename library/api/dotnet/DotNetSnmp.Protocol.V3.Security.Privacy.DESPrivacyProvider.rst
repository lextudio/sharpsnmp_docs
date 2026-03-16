DESPrivacyProvider Class
========================

.. dn:class:: DotNetSnmp.Protocol.V3.Security.Privacy.DESPrivacyProvider

   Privacy provider for DES.

   .. code-block:: csharp

      public class DESPrivacyProvider : PrivacyProviderBase, IPrivacyProvider

**Namespace:** ``DotNetSnmp.Protocol.V3.Security.Privacy``

**Inheritance:** Object → PrivacyProviderBase → ``DESPrivacyProvider``

**Source:** `SharpSnmpLib/V3/Security/Privacy/DESPrivacyProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/DESPrivacyProvider.cs#L10>`__

Constructors
------------

DESPrivacyProvider(in IAuthenticationProvider, in ReadOnlyMemory<Byte>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Protocol.V3.Security.Privacy.DESPrivacyProvider..ctor(DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider@,System.ReadOnlyMemory{System.Byte}@)

   Initializes a new instance of DESPrivacyProvider.

   .. code-block:: csharp

      public DESPrivacyProvider(in IAuthenticationProvider authenticationService, in ReadOnlyMemory<byte> passcode)

   :type authenticationService: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider`
   :type passcode: ``ReadOnlyMemory<Byte>``

**Source:** `SharpSnmpLib/V3/Security/Privacy/DESPrivacyProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/DESPrivacyProvider.cs#L15>`__

Methods
-------

DecryptScopedPdu(in ReadOnlyMemory<Byte>, in UsmSecurityParameters, Span<Byte>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Security.Privacy.DESPrivacyProvider.DecryptScopedPdu(System.ReadOnlyMemory{System.Byte}@,DotNetSnmp.Protocol.V3.Security.UsmSecurityParameters@,System.Span{System.Byte})

   Decrypts an encrypted scoped PDU payload into plaintext bytes.

   .. code-block:: csharp

      public override void DecryptScopedPdu(in ReadOnlyMemory<byte> encryptedPdu, in UsmSecurityParameters parameters, Span<byte> decryptedPdu)

   :type encryptedPdu: ``ReadOnlyMemory<Byte>``
   :type parameters: :dn:cls:`~DotNetSnmp.Protocol.V3.Security.UsmSecurityParameters`
   :type decryptedPdu: ``Span<Byte>``

**Source:** `SharpSnmpLib/V3/Security/Privacy/DESPrivacyProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/DESPrivacyProvider.cs#L102>`__

EncryptScopedPdu(in ReadOnlyMemory<Byte>, in UsmSecurityParameters, Span<Byte>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Security.Privacy.DESPrivacyProvider.EncryptScopedPdu(System.ReadOnlyMemory{System.Byte}@,DotNetSnmp.Protocol.V3.Security.UsmSecurityParameters@,System.Span{System.Byte})

   Encrypts a scoped PDU payload and returns the number of bytes written.

   .. code-block:: csharp

      public override int EncryptScopedPdu(in ReadOnlyMemory<byte> scopedPdu, in UsmSecurityParameters parameters, Span<byte> encryptedScopedPdu)

   :type scopedPdu: ``ReadOnlyMemory<Byte>``
   :type parameters: :dn:cls:`~DotNetSnmp.Protocol.V3.Security.UsmSecurityParameters`
   :type encryptedScopedPdu: ``Span<Byte>``

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/V3/Security/Privacy/DESPrivacyProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/DESPrivacyProvider.cs#L23>`__

