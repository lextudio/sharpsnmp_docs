AES192PrivacyProvider Class
===========================

.. dn:class:: DotNetSnmp.Protocol.V3.Security.Privacy.AES192PrivacyProvider

   Implementation of AES-192 privacy protocol for SNMPv3.

   .. code-block:: csharp

      public class AES192PrivacyProvider : AESPrivacyProviderBase, IPrivacyProvider

**Namespace:** ``DotNetSnmp.Protocol.V3.Security.Privacy``

**Inheritance:** Object → PrivacyProviderBase → AESPrivacyProviderBase → ``AES192PrivacyProvider``

**Source:** `SharpSnmpLib/V3/Security/Privacy/AES192PrivacyProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/AES192PrivacyProvider.cs#L7>`__

Constructors
------------

AES192PrivacyProvider(IAuthenticationProvider, ReadOnlyMemory<Byte>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Protocol.V3.Security.Privacy.AES192PrivacyProvider..ctor(DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider,System.ReadOnlyMemory{System.Byte})

   Initializes a new instance of AES192PrivacyProvider.

   .. code-block:: csharp

      public AES192PrivacyProvider(IAuthenticationProvider authenticationService, ReadOnlyMemory<byte> passcode)

   :type authenticationService: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider`
   :type passcode: ``ReadOnlyMemory<Byte>``

**Source:** `SharpSnmpLib/V3/Security/Privacy/AES192PrivacyProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/AES192PrivacyProvider.cs#L14>`__

