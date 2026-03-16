SHA384AuthenticationProvider Class
==================================

.. dn:class:: DotNetSnmp.Protocol.V3.Security.Authentication.SHA384AuthenticationProvider

   Provides authentication for SNMP v3 messages using HMAC-SHA384.

   .. code-block:: csharp

      public class SHA384AuthenticationProvider : AuthenticationProviderBase, IAuthenticationProvider

**Namespace:** ``DotNetSnmp.Protocol.V3.Security.Authentication``

**Inheritance:** Object → AuthenticationProviderBase → ``SHA384AuthenticationProvider``

**Source:** `SharpSnmpLib/V3/Security/Authentication/SHA384AuthenticationProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Authentication/SHA384AuthenticationProvider.cs#L11>`__

Constructors
------------

SHA384AuthenticationProvider(ReadOnlyMemory<Byte>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Protocol.V3.Security.Authentication.SHA384AuthenticationProvider..ctor(System.ReadOnlyMemory{System.Byte})

   Initializes a new instance of SHA384AuthenticationProvider.

   .. code-block:: csharp

      public SHA384AuthenticationProvider(ReadOnlyMemory<byte> passcode)

   :param passcode: The password or passphrase to be used for authentication.
   :type passcode: ``ReadOnlyMemory<Byte>``

**Source:** `SharpSnmpLib/V3/Security/Authentication/SHA384AuthenticationProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Authentication/SHA384AuthenticationProvider.cs#L17>`__

