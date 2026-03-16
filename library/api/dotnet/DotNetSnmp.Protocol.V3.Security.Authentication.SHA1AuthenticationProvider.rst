SHA1AuthenticationProvider Class
================================

.. dn:class:: DotNetSnmp.Protocol.V3.Security.Authentication.SHA1AuthenticationProvider

   Provides authentication for SNMP v3 messages using HMAC-SHA1.

   .. code-block:: csharp

      public class SHA1AuthenticationProvider : AuthenticationProviderBase, IAuthenticationProvider

**Namespace:** ``DotNetSnmp.Protocol.V3.Security.Authentication``

**Inheritance:** Object → AuthenticationProviderBase → ``SHA1AuthenticationProvider``

**Source:** `SharpSnmpLib/V3/Security/Authentication/SHA1AuthenticationProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Authentication/SHA1AuthenticationProvider.cs#L11>`__

Constructors
------------

SHA1AuthenticationProvider(ReadOnlyMemory<Byte>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Protocol.V3.Security.Authentication.SHA1AuthenticationProvider..ctor(System.ReadOnlyMemory{System.Byte})

   Initializes a new instance of SHA1AuthenticationProvider.

   .. code-block:: csharp

      public SHA1AuthenticationProvider(ReadOnlyMemory<byte> passcode)

   :param passcode: The password or passphrase to be used for authentication.
   :type passcode: ``ReadOnlyMemory<Byte>``

**Source:** `SharpSnmpLib/V3/Security/Authentication/SHA1AuthenticationProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Authentication/SHA1AuthenticationProvider.cs#L17>`__

