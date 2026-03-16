IPrivacyProvider Interface
==========================

.. dn:interface:: DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider

   Privacy provider interface.

   .. code-block:: csharp

      public interface IPrivacyProvider

**Namespace:** ``DotNetSnmp.Protocol.V3.Security.Privacy``

**Source:** `SharpSnmpLib/V3/Security/Privacy/IPrivacyProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/IPrivacyProvider.cs#L8>`__

Properties
----------

AuthenticationProvider
~~~~~~~~~~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider.AuthenticationProvider

   Corresponding :dn:iface:``~DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider``.

   .. code-block:: csharp

      IAuthenticationProvider AuthenticationProvider { get; }

   :rtype: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider`

**Source:** `SharpSnmpLib/V3/Security/Privacy/IPrivacyProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/IPrivacyProvider.cs#L25>`__

EngineBoots
~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider.EngineBoots

   Gets engine Boots.

   .. code-block:: csharp

      int EngineBoots { get; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/V3/Security/Privacy/IPrivacyProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/IPrivacyProvider.cs#L21>`__

EngineIds
~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider.EngineIds

   Gets known engine ids (legacy compatibility member).

   .. code-block:: csharp

      ICollection<OctetString>? EngineIds { get; }

   :rtype: ``ICollection<OctetString>``

**Source:** `SharpSnmpLib/V3/Security/Privacy/IPrivacyProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/IPrivacyProvider.cs#L35>`__

EngineTime
~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider.EngineTime

   Gets engine Time.

   .. code-block:: csharp

      int EngineTime { get; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/V3/Security/Privacy/IPrivacyProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/IPrivacyProvider.cs#L17>`__

PrivacyParametersLength
~~~~~~~~~~~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider.PrivacyParametersLength

   Gets privacy Parameters Length.

   .. code-block:: csharp

      int PrivacyParametersLength { get; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/V3/Security/Privacy/IPrivacyProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/IPrivacyProvider.cs#L13>`__

Salt
~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider.Salt

   Gets privacy salt (legacy compatibility member).

   .. code-block:: csharp

      OctetString Salt { get; }

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`

**Source:** `SharpSnmpLib/V3/Security/Privacy/IPrivacyProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/IPrivacyProvider.cs#L30>`__

Methods
-------

DecryptMessage(SnmpV3Message)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider.DecryptMessage(DotNetSnmp.Protocol.V3.SnmpV3Message)

   Decrypts a v3 message scope according to the configured privacy protocol.

   .. code-block:: csharp

      void DecryptMessage(SnmpV3Message message)

   :type message: :dn:cls:`~DotNetSnmp.Protocol.V3.SnmpV3Message`

**Source:** `SharpSnmpLib/V3/Security/Privacy/IPrivacyProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/IPrivacyProvider.cs#L45>`__

EncryptMessage(SnmpV3Message)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider.EncryptMessage(DotNetSnmp.Protocol.V3.SnmpV3Message)

   Encrypts a v3 message scope according to the configured privacy protocol.

   .. code-block:: csharp

      void EncryptMessage(SnmpV3Message message)

   :type message: :dn:cls:`~DotNetSnmp.Protocol.V3.SnmpV3Message`

**Source:** `SharpSnmpLib/V3/Security/Privacy/IPrivacyProvider.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/Privacy/IPrivacyProvider.cs#L40>`__

Extension Methods
-----------------

- :dn:meth:`Decrypt <Lextm.SharpSnmpLib.Security.PrivacyProviderCompatibilityExtensions.Decrypt>`
- :dn:meth:`Encrypt <Lextm.SharpSnmpLib.Security.PrivacyProviderCompatibilityExtensions.Encrypt>`
- :dn:meth:`ToSecurityLevel <Lextm.SharpSnmpLib.Security.PrivacyProviderCompatibilityExtensions.ToSecurityLevel>`

