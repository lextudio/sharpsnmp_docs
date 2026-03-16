ISnmpMessage Interface
======================

.. dn:interface:: DotNetSnmp.Common.Definitions.ISnmpMessage

   SNMP message.

   .. code-block:: csharp

      public interface ISnmpMessage : IAsnSerializable

**Namespace:** ``DotNetSnmp.Common.Definitions``

**Source:** `SharpSnmpLib/Common/ISnmpMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/ISnmpMessage.cs#L8>`__

Properties
----------

Header
~~~~~~

.. dn:property:: DotNetSnmp.Common.Definitions.ISnmpMessage.Header

   Gets message header information.

   .. code-block:: csharp

      Header Header { get; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpLib.Header`

**Source:** `SharpSnmpLib/Common/ISnmpMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/ISnmpMessage.cs#L28>`__

Parameters
~~~~~~~~~~

.. dn:property:: DotNetSnmp.Common.Definitions.ISnmpMessage.Parameters

   Gets security parameters.

   .. code-block:: csharp

      SecurityParameters Parameters { get; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpLib.SecurityParameters`

**Source:** `SharpSnmpLib/Common/ISnmpMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/ISnmpMessage.cs#L33>`__

ProtocolVersion
~~~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Common.Definitions.ISnmpMessage.ProtocolVersion

   Gets the SNMP protocol version.

   .. code-block:: csharp

      VersionCode ProtocolVersion { get; }

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`

**Source:** `SharpSnmpLib/Common/ISnmpMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/ISnmpMessage.cs#L13>`__

Scope
~~~~~

.. dn:property:: DotNetSnmp.Common.Definitions.ISnmpMessage.Scope

   Gets the message scope.

   .. code-block:: csharp

      IScope? Scope { get; }

   :rtype: :dn:iface:`~DotNetSnmp.Common.Definitions.IScope`

**Source:** `SharpSnmpLib/Common/ISnmpMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/ISnmpMessage.cs#L23>`__

Version
~~~~~~~

.. dn:property:: DotNetSnmp.Common.Definitions.ISnmpMessage.Version

   Gets the SNMP protocol version (legacy compatibility alias).

   .. code-block:: csharp

      VersionCode Version { get; }

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`

**Source:** `SharpSnmpLib/Common/ISnmpMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/ISnmpMessage.cs#L18>`__

