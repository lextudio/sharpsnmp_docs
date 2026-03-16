SHA256AuthenticationProvider Class
==================================

.. dn:class:: Lextm.SharpSnmpLib.Security.SHA256AuthenticationProvider

   Represents the SHA256AuthenticationProvider type.

   .. code-block:: csharp

      public sealed class SHA256AuthenticationProvider : SHA256AuthenticationProvider, IAuthenticationProvider

**Namespace:** ``Lextm.SharpSnmpLib.Security``

**Inheritance:** Object → AuthenticationProviderBase → SHA256AuthenticationProvider → ``SHA256AuthenticationProvider``

**Source:** `SharpSnmpLib/Security/ProviderCompatibility.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/ProviderCompatibility.cs#L49>`__

Constructors
------------

SHA256AuthenticationProvider(OctetString)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Security.SHA256AuthenticationProvider..ctor(DotNetSnmp.Asn1.SyntaxObjects.OctetString)

   Initializes a new instance of SHA256AuthenticationProvider.

   .. code-block:: csharp

      public SHA256AuthenticationProvider(OctetString passphrase)

   :type passphrase: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`

**Source:** `SharpSnmpLib/Security/ProviderCompatibility.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/ProviderCompatibility.cs#L54>`__

