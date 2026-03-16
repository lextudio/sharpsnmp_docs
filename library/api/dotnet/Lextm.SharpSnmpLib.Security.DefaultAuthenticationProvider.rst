DefaultAuthenticationProvider Class
===================================

.. dn:class:: Lextm.SharpSnmpLib.Security.DefaultAuthenticationProvider

   Legacy facade for default authentication provider singleton.

   .. code-block:: csharp

      public static class DefaultAuthenticationProvider

**Namespace:** ``Lextm.SharpSnmpLib.Security``

**Inheritance:** Object → ``DefaultAuthenticationProvider``

**Source:** `SharpSnmpLib/Security/ProviderCompatibility.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/ProviderCompatibility.cs#L10>`__

Properties
----------

Instance
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Security.DefaultAuthenticationProvider.Instance

   Represents instance.

   .. code-block:: csharp

      public static IAuthenticationProvider Instance { get; }

   :rtype: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider`

**Source:** `SharpSnmpLib/Security/ProviderCompatibility.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/ProviderCompatibility.cs#L15>`__

