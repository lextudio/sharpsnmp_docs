AESPrivacyProviderBase Class
============================

.. dn:class:: Lextm.SharpSnmpLib.Security.AESPrivacyProviderBase

   Legacy facade for AES privacy provider capability checks.

   .. code-block:: csharp

      [Obsolete("This type is for internal use only and may be removed in a future release.")]
      public abstract class AESPrivacyProviderBase

**Namespace:** ``Lextm.SharpSnmpLib.Security``

**Inheritance:** Object → ``AESPrivacyProviderBase``

**Source:** `SharpSnmpLib/Security/ProviderCompatibility.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/ProviderCompatibility.cs#L368>`__

Properties
----------

IsSupported
~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Security.AESPrivacyProviderBase.IsSupported

   Gets a value indicating whether AES is supported on current runtime.

   .. code-block:: csharp

      public static bool IsSupported { get; }

   :rtype: ``Boolean``

**Source:** `SharpSnmpLib/Security/ProviderCompatibility.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/ProviderCompatibility.cs#L374>`__

