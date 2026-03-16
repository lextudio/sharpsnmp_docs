DotNetSnmp.Protocol.V3.Security.Authentication Namespace
========================================================

.. dn:namespace:: DotNetSnmp.Protocol.V3.Security.Authentication

Classes
-------

.. list-table::
   :header-rows: 1
   :widths: 30 70

   * - Type
     - Description
   * - :doc:`AuthenticationProviderBase <DotNetSnmp.Protocol.V3.Security.Authentication.AuthenticationProviderBase>`
     - Base abstract class for SNMP v3 authentication providers that implements common functionality.
   * - :doc:`DefaultAuthenticationProvider <DotNetSnmp.Protocol.V3.Security.Authentication.DefaultAuthenticationProvider>`
     - Provides a default implementation of the :dn:iface:``~DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider`` interface.
   * - :doc:`MD5AuthenticationProvider <DotNetSnmp.Protocol.V3.Security.Authentication.MD5AuthenticationProvider>`
     - Provides authentication for SNMP v3 messages using HMAC-MD5.
   * - :doc:`SHA1AuthenticationProvider <DotNetSnmp.Protocol.V3.Security.Authentication.SHA1AuthenticationProvider>`
     - Provides authentication for SNMP v3 messages using HMAC-SHA1.
   * - :doc:`SHA256AuthenticationProvider <DotNetSnmp.Protocol.V3.Security.Authentication.SHA256AuthenticationProvider>`
     - Provides authentication for SNMP v3 messages using HMAC-SHA256.
   * - :doc:`SHA384AuthenticationProvider <DotNetSnmp.Protocol.V3.Security.Authentication.SHA384AuthenticationProvider>`
     - Provides authentication for SNMP v3 messages using HMAC-SHA384.
   * - :doc:`SHA512AuthenticationProvider <DotNetSnmp.Protocol.V3.Security.Authentication.SHA512AuthenticationProvider>`
     - Provides authentication for SNMP v3 messages using HMAC-SHA512.

Interfaces
----------

.. list-table::
   :header-rows: 1
   :widths: 30 70

   * - Type
     - Description
   * - :doc:`IAuthenticationProvider <DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider>`
     - Authentication provider interface.

