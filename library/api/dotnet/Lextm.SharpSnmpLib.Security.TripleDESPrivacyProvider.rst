TripleDESPrivacyProvider Class
==============================

.. dn:class:: Lextm.SharpSnmpLib.Security.TripleDESPrivacyProvider

   Represents the TripleDESPrivacyProvider type.

   .. code-block:: csharp

      public sealed class TripleDESPrivacyProvider : TripleDESPrivacyProvider, IPrivacyProvider

**Namespace:** ``Lextm.SharpSnmpLib.Security``

**Inheritance:** Object → PrivacyProviderBase → TripleDESPrivacyProvider → ``TripleDESPrivacyProvider``

**Source:** `SharpSnmpLib/Security/ProviderCompatibility.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/ProviderCompatibility.cs#L303>`__

Constructors
------------

TripleDESPrivacyProvider(Nullable<OctetString>, IAuthenticationProvider)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Security.TripleDESPrivacyProvider..ctor(System.Nullable{DotNetSnmp.Asn1.SyntaxObjects.OctetString},DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider)

   Initializes a new instance of TripleDESPrivacyProvider.

   .. code-block:: csharp

      public TripleDESPrivacyProvider(OctetString? passphrase, IAuthenticationProvider authenticationProvider)

   :type passphrase: ``Nullable<OctetString>``
   :type authenticationProvider: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider`

**Source:** `SharpSnmpLib/Security/ProviderCompatibility.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/ProviderCompatibility.cs#L308>`__

