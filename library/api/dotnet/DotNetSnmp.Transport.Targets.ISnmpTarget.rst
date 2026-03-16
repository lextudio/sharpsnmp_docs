ISnmpTarget Interface
=====================

.. dn:interface:: DotNetSnmp.Transport.Targets.ISnmpTarget

   Defines the contract for ISnmpTarget.

   .. code-block:: csharp

      public interface ISnmpTarget

**Namespace:** ``DotNetSnmp.Transport.Targets``

**Source:** `SharpSnmpLib/Transport/ISnmpTarget.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/ISnmpTarget.cs#L8>`__

Properties
----------

MaxMessageSize
~~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Transport.Targets.ISnmpTarget.MaxMessageSize

   Gets max Message Size.

   .. code-block:: csharp

      int MaxMessageSize { get; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Transport/ISnmpTarget.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/ISnmpTarget.cs#L18>`__

ProtocolVersion
~~~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Transport.Targets.ISnmpTarget.ProtocolVersion

   Gets the SNMP protocol version.

   .. code-block:: csharp

      VersionCode ProtocolVersion { get; }

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`

**Source:** `SharpSnmpLib/Transport/ISnmpTarget.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/ISnmpTarget.cs#L33>`__

Retries
~~~~~~~

.. dn:property:: DotNetSnmp.Transport.Targets.ISnmpTarget.Retries

   Gets retries.

   .. code-block:: csharp

      int Retries { get; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Transport/ISnmpTarget.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/ISnmpTarget.cs#L13>`__

SecurityName
~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Transport.Targets.ISnmpTarget.SecurityName

   Gets security Name.

   .. code-block:: csharp

      OctetString SecurityName { get; }

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`

**Source:** `SharpSnmpLib/Transport/ISnmpTarget.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/ISnmpTarget.cs#L28>`__

Timeout
~~~~~~~

.. dn:property:: DotNetSnmp.Transport.Targets.ISnmpTarget.Timeout

   Gets timeout.

   .. code-block:: csharp

      int Timeout { get; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Transport/ISnmpTarget.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/ISnmpTarget.cs#L23>`__

