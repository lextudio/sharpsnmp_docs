SHA512AuthenticationProvider Class
==================================

.. dn:class:: Lextm.SharpSnmpLib.Security.SHA512AuthenticationProvider

   Represents the SHA512AuthenticationProvider type.

   .. code-block:: csharp

      public sealed class SHA512AuthenticationProvider : SHA512AuthenticationProvider, IAuthenticationProvider

**Namespace:** ``Lextm.SharpSnmpLib.Security``

**Inheritance:** Object → AuthenticationProviderBase → SHA512AuthenticationProvider → ``SHA512AuthenticationProvider``

**Source:** `SharpSnmpLib/Security/ProviderCompatibility.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/ProviderCompatibility.cs#L77>`__

Constructors
------------

SHA512AuthenticationProvider(OctetString)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Security.SHA512AuthenticationProvider..ctor(DotNetSnmp.Asn1.SyntaxObjects.OctetString)

   Initializes a new instance of SHA512AuthenticationProvider.

   .. code-block:: csharp

      public SHA512AuthenticationProvider(OctetString passphrase)

   :type passphrase: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`

**Source:** `SharpSnmpLib/Security/ProviderCompatibility.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/ProviderCompatibility.cs#L82>`__

