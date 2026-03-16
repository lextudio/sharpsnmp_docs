AES192PrivacyProvider Class
===========================

.. dn:class:: Lextm.SharpSnmpLib.Security.AES192PrivacyProvider

   Represents the AES192PrivacyProvider type.

   .. code-block:: csharp

      public sealed class AES192PrivacyProvider : AES192PrivacyProvider, IPrivacyProvider

**Namespace:** ``Lextm.SharpSnmpLib.Security``

**Inheritance:** Object → PrivacyProviderBase → AESPrivacyProviderBase → AES192PrivacyProvider → ``AES192PrivacyProvider``

**Source:** `SharpSnmpLib/Security/ProviderCompatibility.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/ProviderCompatibility.cs#L380>`__

Constructors
------------

AES192PrivacyProvider(Nullable<OctetString>, IAuthenticationProvider)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Security.AES192PrivacyProvider..ctor(System.Nullable{DotNetSnmp.Asn1.SyntaxObjects.OctetString},DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider)

   Initializes a new instance of AES192PrivacyProvider.

   .. code-block:: csharp

      public AES192PrivacyProvider(OctetString? passphrase, IAuthenticationProvider authenticationProvider)

   :type passphrase: ``Nullable<OctetString>``
   :type authenticationProvider: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider`

**Source:** `SharpSnmpLib/Security/ProviderCompatibility.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/ProviderCompatibility.cs#L387>`__

