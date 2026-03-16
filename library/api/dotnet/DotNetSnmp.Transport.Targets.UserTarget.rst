UserTarget Class
================

.. dn:class:: DotNetSnmp.Transport.Targets.UserTarget

   Represents the UserTarget type.

   .. code-block:: csharp

      public record UserTarget : AbstractTarget, ISnmpTarget, IEquatable<AbstractTarget>, IEquatable<UserTarget>

**Namespace:** ``DotNetSnmp.Transport.Targets``

**Inheritance:** Object → AbstractTarget → ``UserTarget``

**Source:** `SharpSnmpLib/Transport/Targets/UserTarget.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/Targets/UserTarget.cs#L10>`__

Constructors
------------

UserTarget(OctetString, IPrivacyProvider, Int32)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Transport.Targets.UserTarget..ctor(DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider,System.Int32)

   Initializes a new instance of UserTarget.

   .. code-block:: csharp

      public UserTarget(OctetString securityName, IPrivacyProvider privacy, int maxMessageSize = 65507)

   :type securityName: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type privacy: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`
   :type maxMessageSize: ``Int32``

**Source:** `SharpSnmpLib/Transport/Targets/UserTarget.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/Targets/UserTarget.cs#L43>`__

Properties
----------

AuthenticationService
~~~~~~~~~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Transport.Targets.UserTarget.AuthenticationService

   Represents this member.

   .. code-block:: csharp

      public IAuthenticationProvider AuthenticationService { get; }

   :rtype: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Authentication.IAuthenticationProvider`

**Source:** `SharpSnmpLib/Transport/Targets/UserTarget.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/Targets/UserTarget.cs#L15>`__

EngineBoots
~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Transport.Targets.UserTarget.EngineBoots

   Gets engine Boots.

   .. code-block:: csharp

      public int EngineBoots { get; set; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Transport/Targets/UserTarget.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/Targets/UserTarget.cs#L33>`__

EngineId
~~~~~~~~

.. dn:property:: DotNetSnmp.Transport.Targets.UserTarget.EngineId

   Gets engine Id.

   .. code-block:: csharp

      public ReadOnlyMemory<byte> EngineId { get; set; }

   :rtype: ``ReadOnlyMemory<Byte>``

**Source:** `SharpSnmpLib/Transport/Targets/UserTarget.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/Targets/UserTarget.cs#L28>`__

EngineTime
~~~~~~~~~~

.. dn:property:: DotNetSnmp.Transport.Targets.UserTarget.EngineTime

   Gets engine Time.

   .. code-block:: csharp

      public int EngineTime { get; set; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Transport/Targets/UserTarget.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/Targets/UserTarget.cs#L38>`__

PrivacyService
~~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Transport.Targets.UserTarget.PrivacyService

   Gets privacy Service.

   .. code-block:: csharp

      public IPrivacyProvider PrivacyService { get; }

   :rtype: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`

**Source:** `SharpSnmpLib/Transport/Targets/UserTarget.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/Targets/UserTarget.cs#L23>`__

SecurityLevel
~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Transport.Targets.UserTarget.SecurityLevel

   Represents this member.

   .. code-block:: csharp

      public Levels SecurityLevel { get; }

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.Levels`

**Source:** `SharpSnmpLib/Transport/Targets/UserTarget.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/Targets/UserTarget.cs#L53>`__

SecurityModel
~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Transport.Targets.UserTarget.SecurityModel

   Represents usm.

   .. code-block:: csharp

      public SecurityModel SecurityModel { get; }

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.SecurityModel`

**Source:** `SharpSnmpLib/Transport/Targets/UserTarget.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/Targets/UserTarget.cs#L78>`__

