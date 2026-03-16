VersionCode Enum
================

.. dn:enum:: DotNetSnmp.Common.Definitions.VersionCode

   Protocol version code.

   .. code-block:: csharp

      [DataContract]
      public enum VersionCode

**Namespace:** ``DotNetSnmp.Common.Definitions``

**Source:** `SharpSnmpLib/Common/ProtocolVersion.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/ProtocolVersion.cs#L7>`__

Fields
------

V1
~~

.. dn:field:: DotNetSnmp.Common.Definitions.VersionCode.V1

   SNMP v1.

   .. code-block:: csharp

      V1 = 0

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`

**Source:** `SharpSnmpLib/Common/ProtocolVersion.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/ProtocolVersion.cs#L13>`__

V2
~~

.. dn:field:: DotNetSnmp.Common.Definitions.VersionCode.V2

   SNMP v2 classic.

   .. code-block:: csharp

      V2 = 1

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`

**Source:** `SharpSnmpLib/Common/ProtocolVersion.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/ProtocolVersion.cs#L18>`__

V2U
~~~

.. dn:field:: DotNetSnmp.Common.Definitions.VersionCode.V2U

   SNMP v2u is obsolete.

   .. code-block:: csharp

      [Obsolete("This version of SNMP is obsolete and replaced by v3.")]
      V2U = 2

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`

**Source:** `SharpSnmpLib/Common/ProtocolVersion.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/ProtocolVersion.cs#L23>`__

V3
~~

.. dn:field:: DotNetSnmp.Common.Definitions.VersionCode.V3

   SNMP v3.

   .. code-block:: csharp

      V3 = 3

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`

**Source:** `SharpSnmpLib/Common/ProtocolVersion.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/ProtocolVersion.cs#L29>`__

