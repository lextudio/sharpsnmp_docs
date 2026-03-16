DefaultPrivacyProvider Class
============================

.. dn:class:: Lextm.SharpSnmpLib.Security.DefaultPrivacyProvider

   Represents the DefaultPrivacyProvider type.

   .. code-block:: csharp

      public class DefaultPrivacyProvider : DefaultPrivacyProvider, IPrivacyProvider

**Namespace:** ``Lextm.SharpSnmpLib.Security``

**Inheritance:** Object → DefaultPrivacyProvider → ``DefaultPrivacyProvider``

**Source:** `SharpSnmpLib/Security/ProviderCompatibility.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/ProviderCompatibility.cs#L91>`__

Constructors
------------

DefaultPrivacyProvider()
~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Security.DefaultPrivacyProvider..ctor

   Initializes a new instance of DefaultPrivacyProvider.

   .. code-block:: csharp

      public DefaultPrivacyProvider()

**Source:** `SharpSnmpLib/Security/ProviderCompatibility.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/ProviderCompatibility.cs#L104>`__

DefaultPrivacyProvider(IAuthenticationProvider)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Security.DefaultPrivacyProvider..ctor(DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider)

   Initializes a new instance of DefaultPrivacyProvider.

   .. code-block:: csharp

      public DefaultPrivacyProvider(IAuthenticationProvider authenticationProvider)

   :type authenticationProvider: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider`

**Source:** `SharpSnmpLib/Security/ProviderCompatibility.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/ProviderCompatibility.cs#L112>`__

Properties
----------

DefaultPair
~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Security.DefaultPrivacyProvider.DefaultPair

   Stores default Pair.

   .. code-block:: csharp

      public static IPrivacyProvider DefaultPair { get; }

   :rtype: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`

**Source:** `SharpSnmpLib/Security/ProviderCompatibility.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/ProviderCompatibility.cs#L99>`__

EngineIds
~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Security.DefaultPrivacyProvider.EngineIds

   Gets or sets known engine IDs (legacy compatibility member).

   .. code-block:: csharp

      public ICollection<OctetString>? EngineIds { get; set; }

   :rtype: ``ICollection<OctetString>``

**Source:** `SharpSnmpLib/Security/ProviderCompatibility.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/ProviderCompatibility.cs#L120>`__

