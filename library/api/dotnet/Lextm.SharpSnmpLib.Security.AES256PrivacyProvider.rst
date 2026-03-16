AES256PrivacyProvider Class
===========================

.. dn:class:: Lextm.SharpSnmpLib.Security.AES256PrivacyProvider

   Represents the AES256PrivacyProvider type.

   .. code-block:: csharp

      public sealed class AES256PrivacyProvider : AES256PrivacyProvider, IPrivacyProvider

**Namespace:** ``Lextm.SharpSnmpLib.Security``

**Inheritance:** Object → PrivacyProviderBase → AESPrivacyProviderBase → AES256PrivacyProvider → ``AES256PrivacyProvider``

**Source:** `SharpSnmpLib/Security/ProviderCompatibility.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/ProviderCompatibility.cs#L412>`__

Constructors
------------

AES256PrivacyProvider(Nullable<OctetString>, IAuthenticationProvider)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Security.AES256PrivacyProvider..ctor(System.Nullable{DotNetSnmp.Asn1.SyntaxObjects.OctetString},DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider)

   Initializes a new instance of AES256PrivacyProvider.

   .. code-block:: csharp

      public AES256PrivacyProvider(OctetString? passphrase, IAuthenticationProvider authenticationProvider)

   :type passphrase: ``Nullable<OctetString>``
   :type authenticationProvider: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider`

**Source:** `SharpSnmpLib/Security/ProviderCompatibility.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/ProviderCompatibility.cs#L419>`__

Extension Methods
-----------------

- :dn:meth:`Decrypt <Lextm.SharpSnmpLib.Security.PrivacyProviderCompatibilityExtensions.Decrypt>`
- :dn:meth:`Encrypt <Lextm.SharpSnmpLib.Security.PrivacyProviderCompatibilityExtensions.Encrypt>`

