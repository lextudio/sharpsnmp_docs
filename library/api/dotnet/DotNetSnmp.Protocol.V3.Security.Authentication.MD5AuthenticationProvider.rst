MD5AuthenticationProvider Class
===============================

.. dn:class:: DotNetSnmp.Protocol.V3.Security.Authentication.MD5AuthenticationProvider

   Provides authentication for SNMP v3 messages using HMAC-MD5.

   .. code-block:: csharp

      public class MD5AuthenticationProvider : AuthenticationProviderBase, IAuthenticationProvider

**Namespace:** ``DotNetSnmp.Protocol.V3.Security.Authentication``

**Inheritance:** Object → AuthenticationProviderBase → ``MD5AuthenticationProvider``

**Source:** `SharpSnmpLib/V3/Security/Authentication/MD5AuthenticationProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Authentication/MD5AuthenticationProvider.cs#L11>`__

Constructors
------------

MD5AuthenticationProvider(ReadOnlyMemory<Byte>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Protocol.V3.Security.Authentication.MD5AuthenticationProvider..ctor(System.ReadOnlyMemory{System.Byte})

   Initializes a new instance of MD5AuthenticationProvider.

   .. code-block:: csharp

      public MD5AuthenticationProvider(ReadOnlyMemory<byte> passcode)

   :param passcode: The password or passphrase to be used for authentication.
   :type passcode: ``ReadOnlyMemory<Byte>``

**Source:** `SharpSnmpLib/V3/Security/Authentication/MD5AuthenticationProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Authentication/MD5AuthenticationProvider.cs#L17>`__

