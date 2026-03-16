CommunityTarget Class
=====================

.. dn:class:: DotNetSnmp.Transport.Targets.CommunityTarget

   Represents the CommunityTarget type.

   .. code-block:: csharp

      public record CommunityTarget : AbstractTarget, ISnmpTarget, IEquatable<AbstractTarget>, IEquatable<CommunityTarget>

**Namespace:** ``DotNetSnmp.Transport.Targets``

**Inheritance:** Object → AbstractTarget → ``CommunityTarget``

**Source:** `SharpSnmpLib/Transport/CommunityTarget.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/CommunityTarget.cs#L7>`__

Constructors
------------

CommunityTarget(VersionCode, OctetString)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Transport.Targets.CommunityTarget..ctor(DotNetSnmp.Common.Definitions.VersionCode,DotNetSnmp.Asn1.SyntaxObjects.OctetString)

   Initializes a new instance of CommunityTarget.

   .. code-block:: csharp

      public CommunityTarget(VersionCode version, OctetString community)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`

**Source:** `SharpSnmpLib/Transport/CommunityTarget.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/CommunityTarget.cs#L12>`__

Properties
----------

Community
~~~~~~~~~

.. dn:property:: DotNetSnmp.Transport.Targets.CommunityTarget.Community

   Represents this member.

   .. code-block:: csharp

      public OctetString Community { get; }

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`

**Source:** `SharpSnmpLib/Transport/CommunityTarget.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/CommunityTarget.cs#L20>`__

