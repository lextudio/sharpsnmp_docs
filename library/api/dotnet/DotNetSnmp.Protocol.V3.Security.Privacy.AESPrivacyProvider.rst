AESPrivacyProvider Class
========================

.. dn:class:: DotNetSnmp.Protocol.V3.Security.Privacy.AESPrivacyProvider

   Implementation of AES-128 privacy protocol for SNMPv3.

   .. code-block:: csharp

      public class AESPrivacyProvider : AESPrivacyProviderBase, IPrivacyProvider

**Namespace:** ``DotNetSnmp.Protocol.V3.Security.Privacy``

**Inheritance:** Object → PrivacyProviderBase → AESPrivacyProviderBase → ``AESPrivacyProvider``

**Source:** `SharpSnmpLib/V3/Security/Privacy/AESPrivacyProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/AESPrivacyProvider.cs#L7>`__

Constructors
------------

AESPrivacyProvider(IAuthenticationProvider, ReadOnlyMemory<Byte>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Protocol.V3.Security.Privacy.AESPrivacyProvider..ctor(DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider,System.ReadOnlyMemory{System.Byte})

   Initializes a new instance of AESPrivacyProvider.

   .. code-block:: csharp

      public AESPrivacyProvider(IAuthenticationProvider authenticationService, ReadOnlyMemory<byte> passcode)

   :type authenticationService: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider`
   :type passcode: ``ReadOnlyMemory<Byte>``

**Source:** `SharpSnmpLib/V3/Security/Privacy/AESPrivacyProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/AESPrivacyProvider.cs#L14>`__

