AuthenticationProviderBase Class
================================

.. dn:class:: DotNetSnmp.Protocol.V3.Security.Authentication.AuthenticationProviderBase

   Base abstract class for SNMP v3 authentication providers that implements common functionality.

   .. code-block:: csharp

      public abstract class AuthenticationProviderBase : IAuthenticationProvider

**Namespace:** ``DotNetSnmp.Protocol.V3.Security.Authentication``

**Inheritance:** Object → ``AuthenticationProviderBase``

**Source:** `SharpSnmpLib/V3/Security/Authentication/AuthenticationProviderBase.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Authentication/AuthenticationProviderBase.cs#L13>`__

Constructors
------------

AuthenticationProviderBase(Int32, Int32, HashAlgorithmName, ReadOnlyMemory<Byte>, Func<Byte[], HMAC>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Protocol.V3.Security.Authentication.AuthenticationProviderBase..ctor(System.Int32,System.Int32,System.Security.Cryptography.HashAlgorithmName,System.ReadOnlyMemory{System.Byte},System.Func{System.Byte[],System.Security.Cryptography.HMAC})

   Initializes a new instance of AuthenticationProviderBase.

   .. code-block:: csharp

      protected AuthenticationProviderBase(int digestSize, int truncatedDigestSize, HashAlgorithmName name, ReadOnlyMemory<byte> passcode, Func<byte[], HMAC> create)

   :param digestSize: The full size of the digest in bytes produced by the hash algorithm.
   :type digestSize: ``Int32``
   :param truncatedDigestSize: The size of the truncated digest in bytes used for authentication parameters.
   :type truncatedDigestSize: ``Int32``
   :param name: The hash algorithm name.
   :type name: ``HashAlgorithmName``
   :param passcode: The password or passphrase to be used for authentication.
   :type passcode: ``ReadOnlyMemory<Byte>``
   :param create: A function that creates an HMAC algorithm instance given a key.
   :type create: ``Func<HMAC>``

**Source:** `SharpSnmpLib/V3/Security/Authentication/AuthenticationProviderBase.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Authentication/AuthenticationProviderBase.cs#L45>`__

Properties
----------

DigestSize
~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Security.Authentication.AuthenticationProviderBase.DigestSize

   Gets digest Size.

   .. code-block:: csharp

      public int DigestSize { get; init; }

   :returns: The full size of the digest in bytes.
   :rtype: ``Int32``

**Source:** `SharpSnmpLib/V3/Security/Authentication/AuthenticationProviderBase.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Authentication/AuthenticationProviderBase.cs#L19>`__

TruncatedDigestSize
~~~~~~~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Security.Authentication.AuthenticationProviderBase.TruncatedDigestSize

   Gets truncated Digest Size.

   .. code-block:: csharp

      public int TruncatedDigestSize { get; init; }

   :returns: The size of the truncated digest in bytes.
   :rtype: ``Int32``

**Source:** `SharpSnmpLib/V3/Security/Authentication/AuthenticationProviderBase.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Authentication/AuthenticationProviderBase.cs#L16>`__

Methods
-------

AuthenticateIncomingMsg(SnmpV3Message)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Security.Authentication.AuthenticationProviderBase.AuthenticateIncomingMsg(DotNetSnmp.Protocol.V3.SnmpV3Message)

   Authenticates an incoming SNMP v3 message by verifying its authentication parameters.

   .. code-block:: csharp

      public bool AuthenticateIncomingMsg(SnmpV3Message message)

   :param message: The SNMP v3 message to authenticate.
   :type message: :dn:cls:`~DotNetSnmp.Protocol.V3.SnmpV3Message`

   :returns: true if the message is authenticated successfully; otherwise, false.
   :rtype: ``Boolean``

**Source:** `SharpSnmpLib/V3/Security/Authentication/AuthenticationProviderBase.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Authentication/AuthenticationProviderBase.cs#L140>`__

AuthenticateOutgoingMsg(SnmpV3Message, Memory<Byte>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Security.Authentication.AuthenticationProviderBase.AuthenticateOutgoingMsg(DotNetSnmp.Protocol.V3.SnmpV3Message,System.Memory{System.Byte})

   Authenticates an outgoing SNMP v3 message by computing and setting its authentication parameters.

   .. code-block:: csharp

      public void AuthenticateOutgoingMsg(SnmpV3Message message, Memory<byte> newAuthParams)

   :param message: The SNMP v3 message to authenticate.
   :type message: :dn:cls:`~DotNetSnmp.Protocol.V3.SnmpV3Message`
   :param newAuthParams: A buffer for storing the authentication parameters.
   :type newAuthParams: ``Memory<Byte>``

**Source:** `SharpSnmpLib/V3/Security/Authentication/AuthenticationProviderBase.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Authentication/AuthenticationProviderBase.cs#L117>`__

PasswordToKey(in ReadOnlyMemory<Byte>, in ReadOnlyMemory<Byte>, Span<Byte>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Security.Authentication.AuthenticationProviderBase.PasswordToKey(System.ReadOnlyMemory{System.Byte}@,System.ReadOnlyMemory{System.Byte}@,System.Span{System.Byte})

   Localizes a user secret into an engine-specific authentication key.

   .. code-block:: csharp

      public void PasswordToKey(in ReadOnlyMemory<byte> secret, in ReadOnlyMemory<byte> engineId, Span<byte> destination)

   :param secret: The password or secret to convert.
   :type secret: ``ReadOnlyMemory<Byte>``
   :param engineId: The engine ID to use in the key generation process.
   :type engineId: ``ReadOnlyMemory<Byte>``
   :param destination: The destination span to write the key into.
   :type destination: ``Span<Byte>``

**Source:** `SharpSnmpLib/V3/Security/Authentication/AuthenticationProviderBase.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Authentication/AuthenticationProviderBase.cs#L167>`__

