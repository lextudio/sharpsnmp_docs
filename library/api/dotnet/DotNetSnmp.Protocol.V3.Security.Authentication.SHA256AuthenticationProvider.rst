SHA256AuthenticationProvider Class
==================================

.. dn:class:: DotNetSnmp.Protocol.V3.Security.Authentication.SHA256AuthenticationProvider

   Provides authentication for SNMP v3 messages using HMAC-SHA256.

   .. code-block:: csharp

      public class SHA256AuthenticationProvider : AuthenticationProviderBase, IAuthenticationProvider

**Namespace:** ``DotNetSnmp.Protocol.V3.Security.Authentication``

**Inheritance:** Object → AuthenticationProviderBase → ``SHA256AuthenticationProvider``

**Source:** `SharpSnmpLib/V3/Security/Authentication/SHA256AuthenticationProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Authentication/SHA256AuthenticationProvider.cs#L11>`__

Constructors
------------

SHA256AuthenticationProvider(ReadOnlyMemory<Byte>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Protocol.V3.Security.Authentication.SHA256AuthenticationProvider..ctor(System.ReadOnlyMemory{System.Byte})

   Initializes a new instance of SHA256AuthenticationProvider.

   .. code-block:: csharp

      public SHA256AuthenticationProvider(ReadOnlyMemory<byte> passcode)

   :param passcode: The password or passphrase to be used for authentication.
   :type passcode: ``ReadOnlyMemory<Byte>``

**Source:** `SharpSnmpLib/V3/Security/Authentication/SHA256AuthenticationProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Authentication/SHA256AuthenticationProvider.cs#L17>`__

