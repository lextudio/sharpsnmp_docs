PrivacyProviderBase Class
=========================

.. dn:class:: DotNetSnmp.Protocol.V3.Security.Privacy.PrivacyProviderBase

   Represents the PrivacyProviderBase type.

   .. code-block:: csharp

      public abstract class PrivacyProviderBase : IPrivacyProvider

**Namespace:** ``DotNetSnmp.Protocol.V3.Security.Privacy``

**Inheritance:** Object → ``PrivacyProviderBase``

**Source:** `SharpSnmpLib/V3/Security/Privacy/PrivacyProviderBase.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/PrivacyProviderBase.cs#L10>`__

Constructors
------------

PrivacyProviderBase(Int32, IAuthenticationProvider, ReadOnlyMemory<Byte>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Protocol.V3.Security.Privacy.PrivacyProviderBase..ctor(System.Int32,DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider,System.ReadOnlyMemory{System.Byte})

   Initializes a new instance of PrivacyProviderBase.

   .. code-block:: csharp

      protected PrivacyProviderBase(int privacyParametersLength, IAuthenticationProvider authenticationService, ReadOnlyMemory<byte> passcode)

   :type privacyParametersLength: ``Int32``
   :type authenticationService: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider`
   :type passcode: ``ReadOnlyMemory<Byte>``

**Source:** `SharpSnmpLib/V3/Security/Privacy/PrivacyProviderBase.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/PrivacyProviderBase.cs#L33>`__

Fields
------

EngineBootsMemory
~~~~~~~~~~~~~~~~~

.. dn:field:: DotNetSnmp.Protocol.V3.Security.Privacy.PrivacyProviderBase.EngineBootsMemory

   Represents engine Boots Memory.

   .. code-block:: csharp

      protected Memory<byte> EngineBootsMemory

   :rtype: ``Memory<Byte>``

**Source:** `SharpSnmpLib/V3/Security/Privacy/PrivacyProviderBase.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/PrivacyProviderBase.cs#L16>`__

EngineTimeMemory
~~~~~~~~~~~~~~~~

.. dn:field:: DotNetSnmp.Protocol.V3.Security.Privacy.PrivacyProviderBase.EngineTimeMemory

   Represents engine Time Memory.

   .. code-block:: csharp

      protected Memory<byte> EngineTimeMemory

   :rtype: ``Memory<Byte>``

**Source:** `SharpSnmpLib/V3/Security/Privacy/PrivacyProviderBase.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/PrivacyProviderBase.cs#L20>`__

Passcode
~~~~~~~~

.. dn:field:: DotNetSnmp.Protocol.V3.Security.Privacy.PrivacyProviderBase.Passcode

   Represents passcode.

   .. code-block:: csharp

      protected ReadOnlyMemory<byte> Passcode

   :rtype: ``ReadOnlyMemory<Byte>``

**Source:** `SharpSnmpLib/V3/Security/Privacy/PrivacyProviderBase.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/PrivacyProviderBase.cs#L28>`__

Properties
----------

AuthenticationProvider
~~~~~~~~~~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Security.Privacy.PrivacyProviderBase.AuthenticationProvider

   Gets the authentication provider associated with this privacy provider.

   .. code-block:: csharp

      public IAuthenticationProvider AuthenticationProvider { get; }

   :rtype: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider`

**Source:** `SharpSnmpLib/V3/Security/Privacy/PrivacyProviderBase.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/PrivacyProviderBase.cs#L24>`__

EngineBoots
~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Security.Privacy.PrivacyProviderBase.EngineBoots

   Gets engine Boots.

   .. code-block:: csharp

      public int EngineBoots { get; protected set; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/V3/Security/Privacy/PrivacyProviderBase.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/PrivacyProviderBase.cs#L45>`__

EngineTime
~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Security.Privacy.PrivacyProviderBase.EngineTime

   Gets engine Time.

   .. code-block:: csharp

      public int EngineTime { get; protected set; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/V3/Security/Privacy/PrivacyProviderBase.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/PrivacyProviderBase.cs#L43>`__

PrivacyParametersLength
~~~~~~~~~~~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Security.Privacy.PrivacyProviderBase.PrivacyParametersLength

   Gets privacy Parameters Length.

   .. code-block:: csharp

      public int PrivacyParametersLength { get; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/V3/Security/Privacy/PrivacyProviderBase.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/PrivacyProviderBase.cs#L41>`__

Methods
-------

DecryptMessage(SnmpV3Message)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Security.Privacy.PrivacyProviderBase.DecryptMessage(DotNetSnmp.Protocol.V3.SnmpV3Message)

   Decrypts a v3 message scope according to the configured privacy protocol.

   .. code-block:: csharp

      public void DecryptMessage(SnmpV3Message message)

   :type message: :dn:cls:`~DotNetSnmp.Protocol.V3.SnmpV3Message`

**Source:** `SharpSnmpLib/V3/Security/Privacy/PrivacyProviderBase.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/PrivacyProviderBase.cs#L64>`__

DecryptScopedPdu(in ReadOnlyMemory<Byte>, in UsmSecurityParameters, Span<Byte>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Security.Privacy.PrivacyProviderBase.DecryptScopedPdu(System.ReadOnlyMemory{System.Byte}@,DotNetSnmp.Protocol.V3.Security.UsmSecurityParameters@,System.Span{System.Byte})

   Decrypts an encrypted scoped PDU payload into plaintext bytes.

   .. code-block:: csharp

      public abstract void DecryptScopedPdu(in ReadOnlyMemory<byte> encryptedPdu, in UsmSecurityParameters parameters, Span<byte> decryptedPdu)

   :type encryptedPdu: ``ReadOnlyMemory<Byte>``
   :type parameters: :dn:cls:`~DotNetSnmp.Protocol.V3.Security.UsmSecurityParameters`
   :type decryptedPdu: ``Span<Byte>``

**Source:** `SharpSnmpLib/V3/Security/Privacy/PrivacyProviderBase.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/PrivacyProviderBase.cs#L49>`__

EncryptMessage(SnmpV3Message)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Security.Privacy.PrivacyProviderBase.EncryptMessage(DotNetSnmp.Protocol.V3.SnmpV3Message)

   Encrypts a v3 message scope according to the configured privacy protocol.

   .. code-block:: csharp

      public void EncryptMessage(SnmpV3Message message)

   :type message: :dn:cls:`~DotNetSnmp.Protocol.V3.SnmpV3Message`

**Source:** `SharpSnmpLib/V3/Security/Privacy/PrivacyProviderBase.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/PrivacyProviderBase.cs#L88>`__

EncryptScopedPdu(in ReadOnlyMemory<Byte>, in UsmSecurityParameters, Span<Byte>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Security.Privacy.PrivacyProviderBase.EncryptScopedPdu(System.ReadOnlyMemory{System.Byte}@,DotNetSnmp.Protocol.V3.Security.UsmSecurityParameters@,System.Span{System.Byte})

   Encrypts a scoped PDU payload and returns the number of bytes written.

   .. code-block:: csharp

      public abstract int EncryptScopedPdu(in ReadOnlyMemory<byte> scopedPdu, in UsmSecurityParameters parameters, Span<byte> encryptedScopedPdu)

   :type scopedPdu: ``ReadOnlyMemory<Byte>``
   :type parameters: :dn:cls:`~DotNetSnmp.Protocol.V3.Security.UsmSecurityParameters`
   :type encryptedScopedPdu: ``Span<Byte>``

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/V3/Security/Privacy/PrivacyProviderBase.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/PrivacyProviderBase.cs#L61>`__

GetNextSalt()
~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Security.Privacy.PrivacyProviderBase.GetNextSalt

   Gets next Salt.

   .. code-block:: csharp

      protected int GetNextSalt()

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/V3/Security/Privacy/PrivacyProviderBase.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/PrivacyProviderBase.cs#L115>`__

PrepareBuffer(Int32)
~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Security.Privacy.PrivacyProviderBase.PrepareBuffer(System.Int32)

   Allocates a temporary buffer for scoped-PDU encryption output.

   .. code-block:: csharp

      public virtual byte[] PrepareBuffer(int encodedLength)

   :type encodedLength: ``Int32``

   :rtype: ``Byte[]``

**Source:** `SharpSnmpLib/V3/Security/Privacy/PrivacyProviderBase.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/PrivacyProviderBase.cs#L53>`__

UpdateEngineBoots(Int32)
~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Security.Privacy.PrivacyProviderBase.UpdateEngineBoots(System.Int32)

   Updates engine Boots.

   .. code-block:: csharp

      protected void UpdateEngineBoots(int authoritativeEngineBoots)

   :type authoritativeEngineBoots: ``Int32``

**Source:** `SharpSnmpLib/V3/Security/Privacy/PrivacyProviderBase.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/PrivacyProviderBase.cs#L134>`__

UpdateEngineTime(Int32)
~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Security.Privacy.PrivacyProviderBase.UpdateEngineTime(System.Int32)

   Updates engine Time.

   .. code-block:: csharp

      protected void UpdateEngineTime(int authoritativeEngineTime)

   :type authoritativeEngineTime: ``Int32``

**Source:** `SharpSnmpLib/V3/Security/Privacy/PrivacyProviderBase.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/PrivacyProviderBase.cs#L146>`__

