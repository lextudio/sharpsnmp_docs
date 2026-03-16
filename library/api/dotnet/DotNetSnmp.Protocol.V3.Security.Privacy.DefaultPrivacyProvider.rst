DefaultPrivacyProvider Class
============================

.. dn:class:: DotNetSnmp.Protocol.V3.Security.Privacy.DefaultPrivacyProvider

   Default privacy provider.

   .. code-block:: csharp

      public class DefaultPrivacyProvider : IPrivacyProvider

**Namespace:** ``DotNetSnmp.Protocol.V3.Security.Privacy``

**Inheritance:** Object → ``DefaultPrivacyProvider``

**Source:** `SharpSnmpLib/V3/Security/Privacy/DefaultPrivacyProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/DefaultPrivacyProvider.cs#L8>`__

Constructors
------------

DefaultPrivacyProvider()
~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Protocol.V3.Security.Privacy.DefaultPrivacyProvider..ctor

   Initializes a new instance of DefaultPrivacyProvider.

   .. code-block:: csharp

      public DefaultPrivacyProvider()

**Source:** `SharpSnmpLib/V3/Security/Privacy/DefaultPrivacyProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/DefaultPrivacyProvider.cs#L25>`__

DefaultPrivacyProvider(IAuthenticationProvider)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Protocol.V3.Security.Privacy.DefaultPrivacyProvider..ctor(DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider)

   Initializes a new instance of DefaultPrivacyProvider.

   .. code-block:: csharp

      public DefaultPrivacyProvider(IAuthenticationProvider authenticationProvider)

   :type authenticationProvider: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider`

**Source:** `SharpSnmpLib/V3/Security/Privacy/DefaultPrivacyProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/DefaultPrivacyProvider.cs#L33>`__

Properties
----------

AuthenticationProvider
~~~~~~~~~~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Security.Privacy.DefaultPrivacyProvider.AuthenticationProvider

   Corresponding :dn:iface:``~DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider``.

   .. code-block:: csharp

      public IAuthenticationProvider AuthenticationProvider { get; }

   :rtype: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider`

**Source:** `SharpSnmpLib/V3/Security/Privacy/DefaultPrivacyProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/DefaultPrivacyProvider.cs#L20>`__

EngineBoots
~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Security.Privacy.DefaultPrivacyProvider.EngineBoots

   Gets engine Boots.

   .. code-block:: csharp

      public int EngineBoots { get; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/V3/Security/Privacy/DefaultPrivacyProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/DefaultPrivacyProvider.cs#L17>`__

EngineTime
~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Security.Privacy.DefaultPrivacyProvider.EngineTime

   Gets engine Time.

   .. code-block:: csharp

      public int EngineTime { get; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/V3/Security/Privacy/DefaultPrivacyProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/DefaultPrivacyProvider.cs#L14>`__

PrivacyParametersLength
~~~~~~~~~~~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Security.Privacy.DefaultPrivacyProvider.PrivacyParametersLength

   Gets privacy Parameters Length.

   .. code-block:: csharp

      public int PrivacyParametersLength { get; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/V3/Security/Privacy/DefaultPrivacyProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/DefaultPrivacyProvider.cs#L11>`__

Methods
-------

DecryptMessage(SnmpV3Message)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Security.Privacy.DefaultPrivacyProvider.DecryptMessage(DotNetSnmp.Protocol.V3.SnmpV3Message)

   Decrypts a v3 message scope according to the configured privacy protocol.

   .. code-block:: csharp

      public void DecryptMessage(SnmpV3Message message)

   :type message: :dn:cls:`~DotNetSnmp.Protocol.V3.SnmpV3Message`

**Source:** `SharpSnmpLib/V3/Security/Privacy/DefaultPrivacyProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/DefaultPrivacyProvider.cs#L55>`__

DecryptScopedPdu(in ReadOnlyMemory<Byte>, in UsmSecurityParameters, Span<Byte>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Security.Privacy.DefaultPrivacyProvider.DecryptScopedPdu(System.ReadOnlyMemory{System.Byte}@,DotNetSnmp.Protocol.V3.Security.UsmSecurityParameters@,System.Span{System.Byte})

   Decrypts a scoped PDU payload. The default provider performs no decryption.

   .. code-block:: csharp

      public void DecryptScopedPdu(in ReadOnlyMemory<byte> encryptedPdu, in UsmSecurityParameters parameters, Span<byte> decryptedPdu)

   :type encryptedPdu: ``ReadOnlyMemory<Byte>``
   :type parameters: :dn:cls:`~DotNetSnmp.Protocol.V3.Security.UsmSecurityParameters`
   :type decryptedPdu: ``Span<Byte>``

**Source:** `SharpSnmpLib/V3/Security/Privacy/DefaultPrivacyProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/DefaultPrivacyProvider.cs#L41>`__

EncryptMessage(SnmpV3Message)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Security.Privacy.DefaultPrivacyProvider.EncryptMessage(DotNetSnmp.Protocol.V3.SnmpV3Message)

   Encrypts a v3 message scope according to the configured privacy protocol.

   .. code-block:: csharp

      public void EncryptMessage(SnmpV3Message message)

   :type message: :dn:cls:`~DotNetSnmp.Protocol.V3.SnmpV3Message`

**Source:** `SharpSnmpLib/V3/Security/Privacy/DefaultPrivacyProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/DefaultPrivacyProvider.cs#L61>`__

EncryptScopedPdu(in ReadOnlyMemory<Byte>, in UsmSecurityParameters, Span<Byte>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Security.Privacy.DefaultPrivacyProvider.EncryptScopedPdu(System.ReadOnlyMemory{System.Byte}@,DotNetSnmp.Protocol.V3.Security.UsmSecurityParameters@,System.Span{System.Byte})

   Encrypts a scoped PDU payload. The default provider performs no encryption.

   .. code-block:: csharp

      public int EncryptScopedPdu(in ReadOnlyMemory<byte> scopedPdu, in UsmSecurityParameters parameters, Span<byte> encryptedScopedPdu)

   :type scopedPdu: ``ReadOnlyMemory<Byte>``
   :type parameters: :dn:cls:`~DotNetSnmp.Protocol.V3.Security.UsmSecurityParameters`
   :type encryptedScopedPdu: ``Span<Byte>``

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/V3/Security/Privacy/DefaultPrivacyProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/DefaultPrivacyProvider.cs#L49>`__

PrepareBuffer(Int32)
~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Security.Privacy.DefaultPrivacyProvider.PrepareBuffer(System.Int32)

   Allocates a temporary buffer for compatibility with legacy call paths.

   .. code-block:: csharp

      public byte[] PrepareBuffer(int encodedLength)

   :type encodedLength: ``Int32``

   :rtype: ``Byte[]``

**Source:** `SharpSnmpLib/V3/Security/Privacy/DefaultPrivacyProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/DefaultPrivacyProvider.cs#L69>`__

