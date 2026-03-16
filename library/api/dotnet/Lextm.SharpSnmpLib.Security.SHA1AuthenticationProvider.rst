SHA1AuthenticationProvider Class
================================

.. dn:class:: Lextm.SharpSnmpLib.Security.SHA1AuthenticationProvider

   Represents the SHA1AuthenticationProvider type.

   .. code-block:: csharp

      public sealed class SHA1AuthenticationProvider : SHA1AuthenticationProvider, IAuthenticationProvider

**Namespace:** ``Lextm.SharpSnmpLib.Security``

**Inheritance:** Object → AuthenticationProviderBase → SHA1AuthenticationProvider → ``SHA1AuthenticationProvider``

**Source:** `SharpSnmpLib/Security/ProviderCompatibility.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/ProviderCompatibility.cs#L35>`__

Constructors
------------

SHA1AuthenticationProvider(OctetString)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Security.SHA1AuthenticationProvider..ctor(DotNetSnmp.Asn1.SyntaxObjects.OctetString)

   Initializes a new instance of SHA1AuthenticationProvider.

   .. code-block:: csharp

      public SHA1AuthenticationProvider(OctetString passphrase)

   :type passphrase: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`

**Source:** `SharpSnmpLib/Security/ProviderCompatibility.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/ProviderCompatibility.cs#L40>`__

