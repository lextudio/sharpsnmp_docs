MD5AuthenticationProvider Class
===============================

.. dn:class:: Lextm.SharpSnmpLib.Security.MD5AuthenticationProvider

   Represents the MD5AuthenticationProvider type.

   .. code-block:: csharp

      public sealed class MD5AuthenticationProvider : MD5AuthenticationProvider, IAuthenticationProvider

**Namespace:** ``Lextm.SharpSnmpLib.Security``

**Inheritance:** Object → AuthenticationProviderBase → MD5AuthenticationProvider → ``MD5AuthenticationProvider``

**Source:** `SharpSnmpLib/Security/ProviderCompatibility.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/ProviderCompatibility.cs#L21>`__

Constructors
------------

MD5AuthenticationProvider(OctetString)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Security.MD5AuthenticationProvider..ctor(DotNetSnmp.Asn1.SyntaxObjects.OctetString)

   Initializes a new instance of MD5AuthenticationProvider.

   .. code-block:: csharp

      public MD5AuthenticationProvider(OctetString passphrase)

   :type passphrase: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`

**Source:** `SharpSnmpLib/Security/ProviderCompatibility.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/ProviderCompatibility.cs#L26>`__

