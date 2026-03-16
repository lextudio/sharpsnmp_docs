AESPrivacyProvider Class
========================

.. dn:class:: Lextm.SharpSnmpLib.Security.AESPrivacyProvider

   Represents the AESPrivacyProvider type.

   .. code-block:: csharp

      public class AESPrivacyProvider : AESPrivacyProvider, IPrivacyProvider

**Namespace:** ``Lextm.SharpSnmpLib.Security``

**Inheritance:** Object → PrivacyProviderBase → AESPrivacyProviderBase → AESPrivacyProvider → ``AESPrivacyProvider``

**Source:** `SharpSnmpLib/Security/ProviderCompatibility.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/ProviderCompatibility.cs#L317>`__

Constructors
------------

AESPrivacyProvider(Nullable<OctetString>, IAuthenticationProvider)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Security.AESPrivacyProvider..ctor(System.Nullable{DotNetSnmp.Asn1.SyntaxObjects.OctetString},DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider)

   Initializes a new instance of AESPrivacyProvider.

   .. code-block:: csharp

      public AESPrivacyProvider(OctetString? passphrase, IAuthenticationProvider authenticationProvider)

   :type passphrase: ``Nullable<OctetString>``
   :type authenticationProvider: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider`

**Source:** `SharpSnmpLib/Security/ProviderCompatibility.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/ProviderCompatibility.cs#L343>`__

Properties
----------

IsSupported
~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Security.AESPrivacyProvider.IsSupported

   Represents this member.

   .. code-block:: csharp

      public static bool IsSupported { get; }

   :rtype: ``Boolean``

**Source:** `SharpSnmpLib/Security/ProviderCompatibility.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/ProviderCompatibility.cs#L324>`__

Extension Methods
-----------------

- :dn:meth:`Decrypt <Lextm.SharpSnmpLib.Security.PrivacyProviderCompatibilityExtensions.Decrypt>`
- :dn:meth:`Encrypt <Lextm.SharpSnmpLib.Security.PrivacyProviderCompatibilityExtensions.Encrypt>`

