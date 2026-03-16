IAuthenticationProvider Interface
=================================

.. dn:interface:: DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider

   Authentication provider interface.

   .. code-block:: csharp

      public interface IAuthenticationProvider

**Namespace:** ``DotNetSnmp.Protocol.V3.Security.Authentication``

**Source:** `SharpSnmpLib/V3/Security/Authentication/IAuthenticationProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Authentication/IAuthenticationProvider.cs#L12>`__

Properties
----------

CleanDigest
~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider.CleanDigest

   Gets a zeroed digest with provider-specific truncated size (legacy compatibility member).

   .. code-block:: csharp

      OctetString CleanDigest { get; }

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`

**Source:** `SharpSnmpLib/V3/Security/Authentication/IAuthenticationProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Authentication/IAuthenticationProvider.cs#L72>`__

DigestSize
~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider.DigestSize

   Gets digest Size.

   .. code-block:: csharp

      int DigestSize { get; }

   :returns: The full size of the digest in bytes.
   :rtype: ``Int32``

**Source:** `SharpSnmpLib/V3/Security/Authentication/IAuthenticationProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Authentication/IAuthenticationProvider.cs#L28>`__

TruncatedDigestSize
~~~~~~~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider.TruncatedDigestSize

   Gets truncated Digest Size.

   .. code-block:: csharp

      int TruncatedDigestSize { get; }

   :returns: The size of the truncated digest in bytes.
   :rtype: ``Int32``

**Source:** `SharpSnmpLib/V3/Security/Authentication/IAuthenticationProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Authentication/IAuthenticationProvider.cs#L20>`__

Methods
-------

AuthenticateIncomingMsg(SnmpV3Message)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider.AuthenticateIncomingMsg(DotNetSnmp.Protocol.V3.SnmpV3Message)

   Authenticates an incoming SNMP v3 message by verifying its authentication parameters.

   .. code-block:: csharp

      bool AuthenticateIncomingMsg(SnmpV3Message message)

   :param message: The SNMP v3 message to authenticate.
   :type message: :dn:cls:`~DotNetSnmp.Protocol.V3.SnmpV3Message`

   :returns: true if the message is authenticated successfully; otherwise, false.
   :rtype: ``Boolean``

**Source:** `SharpSnmpLib/V3/Security/Authentication/IAuthenticationProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Authentication/IAuthenticationProvider.cs#L66>`__

AuthenticateOutgoingMsg(SnmpV3Message, Memory<Byte>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider.AuthenticateOutgoingMsg(DotNetSnmp.Protocol.V3.SnmpV3Message,System.Memory{System.Byte})

   Authenticates an outgoing SNMP v3 message by computing and setting its authentication parameters.

   .. code-block:: csharp

      void AuthenticateOutgoingMsg(SnmpV3Message message, Memory<byte> newAuthParams)

   :param message: The SNMP v3 message to authenticate.
   :type message: :dn:cls:`~DotNetSnmp.Protocol.V3.SnmpV3Message`
   :param newAuthParams: A buffer for storing the authentication parameters.
   :type newAuthParams: ``Memory<Byte>``

**Source:** `SharpSnmpLib/V3/Security/Authentication/IAuthenticationProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Authentication/IAuthenticationProvider.cs#L51>`__

PasswordToKey(in ReadOnlyMemory<Byte>, in ReadOnlyMemory<Byte>, Span<Byte>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider.PasswordToKey(System.ReadOnlyMemory{System.Byte}@,System.ReadOnlyMemory{System.Byte}@,System.Span{System.Byte})

   Localizes a user secret into an engine-specific authentication key.

   .. code-block:: csharp

      void PasswordToKey(in ReadOnlyMemory<byte> secret, in ReadOnlyMemory<byte> engineId, Span<byte> destination)

   :param secret: The password or secret to convert.
   :type secret: ``ReadOnlyMemory<Byte>``
   :param engineId: The engine ID to use in the key generation process.
   :type engineId: ``ReadOnlyMemory<Byte>``
   :param destination: The destination span to write the key into.
   :type destination: ``Span<Byte>``

**Source:** `SharpSnmpLib/V3/Security/Authentication/IAuthenticationProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Authentication/IAuthenticationProvider.cs#L40>`__

