SHA512AuthenticationProvider Class
==================================

.. dn:class:: DotNetSnmp.Protocol.V3.Security.Authentication.SHA512AuthenticationProvider

   Provides authentication for SNMP v3 messages using HMAC-SHA512.

   .. code-block:: csharp

      public class SHA512AuthenticationProvider : AuthenticationProviderBase, IAuthenticationProvider

**Namespace:** ``DotNetSnmp.Protocol.V3.Security.Authentication``

**Inheritance:** Object → AuthenticationProviderBase → ``SHA512AuthenticationProvider``

**Source:** `SharpSnmpLib/V3/Security/Authentication/SHA512AuthenticationProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Authentication/SHA512AuthenticationProvider.cs#L11>`__

Constructors
------------

SHA512AuthenticationProvider(ReadOnlyMemory<Byte>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Protocol.V3.Security.Authentication.SHA512AuthenticationProvider..ctor(System.ReadOnlyMemory{System.Byte})

   Initializes a new instance of SHA512AuthenticationProvider.

   .. code-block:: csharp

      public SHA512AuthenticationProvider(ReadOnlyMemory<byte> passcode)

   :param passcode: The password or passphrase to be used for authentication.
   :type passcode: ``ReadOnlyMemory<Byte>``

**Source:** `SharpSnmpLib/V3/Security/Authentication/SHA512AuthenticationProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Authentication/SHA512AuthenticationProvider.cs#L17>`__

