AbstractTarget Class
====================

.. dn:class:: DotNetSnmp.Transport.Targets.AbstractTarget

   Represents the AbstractTarget type.

   .. code-block:: csharp

      public abstract record AbstractTarget : ISnmpTarget, IEquatable<AbstractTarget>

**Namespace:** ``DotNetSnmp.Transport.Targets``

**Inheritance:** Object → ``AbstractTarget``

**Source:** `SharpSnmpLib/Transport/AbstractTarget.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/AbstractTarget.cs#L8>`__

Constructors
------------

AbstractTarget(VersionCode, OctetString)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Transport.Targets.AbstractTarget..ctor(DotNetSnmp.Common.Definitions.VersionCode,DotNetSnmp.Asn1.SyntaxObjects.OctetString)

   Initializes a new instance of AbstractTarget.

   .. code-block:: csharp

      protected AbstractTarget(VersionCode version, OctetString securityName)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type securityName: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`

**Source:** `SharpSnmpLib/Transport/AbstractTarget.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/AbstractTarget.cs#L13>`__

Properties
----------

MaxMessageSize
~~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Transport.Targets.AbstractTarget.MaxMessageSize

   Gets max Message Size.

   .. code-block:: csharp

      public int MaxMessageSize { get; init; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Transport/AbstractTarget.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/AbstractTarget.cs#L37>`__

ProtocolVersion
~~~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Transport.Targets.AbstractTarget.ProtocolVersion

   Represents this member.

   .. code-block:: csharp

      public VersionCode ProtocolVersion { get; }

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`

**Source:** `SharpSnmpLib/Transport/AbstractTarget.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/AbstractTarget.cs#L42>`__

Retries
~~~~~~~

.. dn:property:: DotNetSnmp.Transport.Targets.AbstractTarget.Retries

   Gets retries.

   .. code-block:: csharp

      public int Retries { get; init; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Transport/AbstractTarget.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/AbstractTarget.cs#L27>`__

SecurityName
~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Transport.Targets.AbstractTarget.SecurityName

   Gets security Name.

   .. code-block:: csharp

      public OctetString SecurityName { get; }

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`

**Source:** `SharpSnmpLib/Transport/AbstractTarget.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/AbstractTarget.cs#L22>`__

Timeout
~~~~~~~

.. dn:property:: DotNetSnmp.Transport.Targets.AbstractTarget.Timeout

   Gets timeout.

   .. code-block:: csharp

      public int Timeout { get; init; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Transport/AbstractTarget.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/AbstractTarget.cs#L32>`__

