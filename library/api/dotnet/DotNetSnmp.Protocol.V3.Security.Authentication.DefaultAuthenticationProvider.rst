DefaultAuthenticationProvider Class
===================================

.. dn:class:: DotNetSnmp.Protocol.V3.Security.Authentication.DefaultAuthenticationProvider

   Provides a default implementation of the :dn:iface:``~DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider`` interface. This class implements a pass-through authentication method that does not perform any actual authentication.

   .. code-block:: csharp

      public class DefaultAuthenticationProvider : IAuthenticationProvider

**Namespace:** ``DotNetSnmp.Protocol.V3.Security.Authentication``

**Inheritance:** Object → ``DefaultAuthenticationProvider``

**Source:** `SharpSnmpLib/V3/Security/Authentication/DefaultAuthenticationProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Authentication/DefaultAuthenticationProvider.cs#L12>`__

Properties
----------

DigestSize
~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Security.Authentication.DefaultAuthenticationProvider.DigestSize

   Gets digest Size.

   .. code-block:: csharp

      public int DigestSize { get; }

   :returns: The full size of the digest in bytes.
   :rtype: ``Int32``

**Source:** `SharpSnmpLib/V3/Security/Authentication/DefaultAuthenticationProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Authentication/DefaultAuthenticationProvider.cs#L50>`__

Instance
~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Security.Authentication.DefaultAuthenticationProvider.Instance

   Represents this member.

   .. code-block:: csharp

      public static DefaultAuthenticationProvider Instance { get; }

   :returns: The singleton instance.
   :rtype: :dn:cls:`~DotNetSnmp.Protocol.V3.Security.Authentication.DefaultAuthenticationProvider`

**Source:** `SharpSnmpLib/V3/Security/Authentication/DefaultAuthenticationProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Authentication/DefaultAuthenticationProvider.cs#L33>`__

TruncatedDigestSize
~~~~~~~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Security.Authentication.DefaultAuthenticationProvider.TruncatedDigestSize

   Gets truncated Digest Size.

   .. code-block:: csharp

      public int TruncatedDigestSize { get; }

   :returns: The size of the truncated digest in bytes.
   :rtype: ``Int32``

**Source:** `SharpSnmpLib/V3/Security/Authentication/DefaultAuthenticationProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Authentication/DefaultAuthenticationProvider.cs#L53>`__

Methods
-------

AuthenticateIncomingMsg(SnmpV3Message)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Security.Authentication.DefaultAuthenticationProvider.AuthenticateIncomingMsg(DotNetSnmp.Protocol.V3.SnmpV3Message)

   Authenticates an incoming SNMP v3 message by verifying its authentication parameters.

   .. code-block:: csharp

      public bool AuthenticateIncomingMsg(SnmpV3Message message)

   :param message: The SNMP v3 message to authenticate.
   :type message: :dn:cls:`~DotNetSnmp.Protocol.V3.SnmpV3Message`

   :returns: true if the message is authenticated successfully; otherwise, false.
   :rtype: ``Boolean``

**Source:** `SharpSnmpLib/V3/Security/Authentication/DefaultAuthenticationProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Authentication/DefaultAuthenticationProvider.cs#L62>`__

AuthenticateOutgoingMsg(SnmpV3Message, Memory<Byte>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Security.Authentication.DefaultAuthenticationProvider.AuthenticateOutgoingMsg(DotNetSnmp.Protocol.V3.SnmpV3Message,System.Memory{System.Byte})

   Authenticates an outgoing SNMP v3 message by computing and setting its authentication parameters.

   .. code-block:: csharp

      public void AuthenticateOutgoingMsg(SnmpV3Message message, Memory<byte> newAuthParams)

   :param message: The SNMP v3 message to authenticate.
   :type message: :dn:cls:`~DotNetSnmp.Protocol.V3.SnmpV3Message`
   :param newAuthParams: A buffer for storing the authentication parameters.
   :type newAuthParams: ``Memory<Byte>``

**Source:** `SharpSnmpLib/V3/Security/Authentication/DefaultAuthenticationProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Authentication/DefaultAuthenticationProvider.cs#L56>`__

PasswordToKey(in ReadOnlyMemory<Byte>, in ReadOnlyMemory<Byte>, Span<Byte>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Security.Authentication.DefaultAuthenticationProvider.PasswordToKey(System.ReadOnlyMemory{System.Byte}@,System.ReadOnlyMemory{System.Byte}@,System.Span{System.Byte})

   Localizes a user secret into an engine-specific authentication key.

   .. code-block:: csharp

      public void PasswordToKey(in ReadOnlyMemory<byte> secret, in ReadOnlyMemory<byte> engineId, Span<byte> destination)

   :param secret: The password or secret to convert.
   :type secret: ``ReadOnlyMemory<Byte>``
   :param engineId: The engine ID to use in the key generation process.
   :type engineId: ``ReadOnlyMemory<Byte>``
   :param destination: The destination span to write the key into.
   :type destination: ``Span<Byte>``

**Source:** `SharpSnmpLib/V3/Security/Authentication/DefaultAuthenticationProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Authentication/DefaultAuthenticationProvider.cs#L69>`__

