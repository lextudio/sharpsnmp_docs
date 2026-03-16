AES256PrivacyProvider Class
===========================

.. dn:class:: DotNetSnmp.Protocol.V3.Security.Privacy.AES256PrivacyProvider

   Implementation of AES-256 privacy protocol for SNMPv3.

   .. code-block:: csharp

      public class AES256PrivacyProvider : AESPrivacyProviderBase, IPrivacyProvider

**Namespace:** ``DotNetSnmp.Protocol.V3.Security.Privacy``

**Inheritance:** Object → PrivacyProviderBase → AESPrivacyProviderBase → ``AES256PrivacyProvider``

**Source:** `SharpSnmpLib/V3/Security/Privacy/AES256PrivacyProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/AES256PrivacyProvider.cs#L7>`__

Constructors
------------

AES256PrivacyProvider(IAuthenticationProvider, ReadOnlyMemory<Byte>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Protocol.V3.Security.Privacy.AES256PrivacyProvider..ctor(DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider,System.ReadOnlyMemory{System.Byte})

   Initializes a new instance of AES256PrivacyProvider.

   .. code-block:: csharp

      public AES256PrivacyProvider(IAuthenticationProvider authenticationService, ReadOnlyMemory<byte> passcode)

   :type authenticationService: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider`
   :type passcode: ``ReadOnlyMemory<Byte>``

**Source:** `SharpSnmpLib/V3/Security/Privacy/AES256PrivacyProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/AES256PrivacyProvider.cs#L14>`__

