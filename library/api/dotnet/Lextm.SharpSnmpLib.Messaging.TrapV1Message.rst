TrapV1Message Class
===================

.. dn:class:: Lextm.SharpSnmpLib.Messaging.TrapV1Message

   Legacy compatibility wrapper for SNMP TRAP v1 messages.

   .. code-block:: csharp

      public sealed class TrapV1Message : ISnmpMessage, IAsnSerializable

**Namespace:** ``Lextm.SharpSnmpLib.Messaging``

**Inheritance:** Object → ``TrapV1Message``

**Source:** `SharpSnmpLib/Messaging/TrapV1Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TrapV1Message.cs#L11>`__

Constructors
------------

TrapV1Message(VersionCode, IPAddress, OctetString, ObjectIdentifier, GenericCode, Int32, UInt32, IList<Variable>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Messaging.TrapV1Message..ctor(DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPAddress,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,Lextm.SharpSnmpLib.GenericCode,System.Int32,System.UInt32,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable})

   Creates a :dn:cls:``~Lextm.SharpSnmpLib.Messaging.TrapV1Message`` with all content.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public TrapV1Message(VersionCode version, IPAddress agent, OctetString community, ObjectIdentifier enterprise, GenericCode generic, int specific, uint time, IList<Variable> variables)

   :param version: Protocol version.
   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :param agent: Agent address.
   :type agent: ``IPAddress``
   :param community: Community name.
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :param enterprise: Enterprise.
   :type enterprise: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :param generic: Generic code.
   :type generic: :dn:enum:`~Lextm.SharpSnmpLib.GenericCode`
   :param specific: Specific code.
   :type specific: ``Int32``
   :param time: Time stamp.
   :type time: ``UInt32``
   :param variables: Variables.
   :type variables: ``IList<Variable>``

**Source:** `SharpSnmpLib/Messaging/TrapV1Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TrapV1Message.cs#L28>`__

Properties
----------

AgentAddress
~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.TrapV1Message.AgentAddress

   Agent address.

   .. code-block:: csharp

      public IPAddress AgentAddress { get; }

   :rtype: ``IPAddress``

**Source:** `SharpSnmpLib/Messaging/TrapV1Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TrapV1Message.cs#L102>`__

Enterprise
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.TrapV1Message.Enterprise

   Enterprise.

   .. code-block:: csharp

      public ObjectIdentifier Enterprise { get; }

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`

**Source:** `SharpSnmpLib/Messaging/TrapV1Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TrapV1Message.cs#L97>`__

Generic
~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.TrapV1Message.Generic

   Generic code.

   .. code-block:: csharp

      public GenericCode Generic { get; }

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.GenericCode`

**Source:** `SharpSnmpLib/Messaging/TrapV1Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TrapV1Message.cs#L107>`__

ProtocolVersion
~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.TrapV1Message.ProtocolVersion

   Gets the SNMP protocol version.

   .. code-block:: csharp

      public VersionCode ProtocolVersion { get; }

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`

**Source:** `SharpSnmpLib/Messaging/TrapV1Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TrapV1Message.cs#L129>`__

Scope
~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.TrapV1Message.Scope

   Gets the message scope.

   .. code-block:: csharp

      public IScope? Scope { get; }

   :rtype: :dn:iface:`~DotNetSnmp.Common.Definitions.IScope`

**Source:** `SharpSnmpLib/Messaging/TrapV1Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TrapV1Message.cs#L132>`__

Specific
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.TrapV1Message.Specific

   Specific code.

   .. code-block:: csharp

      public int Specific { get; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Messaging/TrapV1Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TrapV1Message.cs#L112>`__

TimeStamp
~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.TrapV1Message.TimeStamp

   Time stamp.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public uint TimeStamp { get; }

   :rtype: ``UInt32``

**Source:** `SharpSnmpLib/Messaging/TrapV1Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TrapV1Message.cs#L117>`__

Version
~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.TrapV1Message.Version

   Protocol version.

   .. code-block:: csharp

      public VersionCode Version { get; }

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`

**Source:** `SharpSnmpLib/Messaging/TrapV1Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TrapV1Message.cs#L92>`__

Methods
-------

ToBytes()
~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.TrapV1Message.ToBytes

   Serializes the message to a byte array.

   .. code-block:: csharp

      public byte[] ToBytes()

   :rtype: ``Byte[]``

**Source:** `SharpSnmpLib/Messaging/TrapV1Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TrapV1Message.cs#L143>`__

ToString()
~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.TrapV1Message.ToString

   Returns a string representation.

   .. code-block:: csharp

      public override string ToString()

   :rtype: ``String``

**Source:** `SharpSnmpLib/Messaging/TrapV1Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TrapV1Message.cs#L151>`__

Variables()
~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.TrapV1Message.Variables

   Gets the variable bindings.

   .. code-block:: csharp

      public IList<Variable> Variables()

   :rtype: ``IList<Variable>``

**Source:** `SharpSnmpLib/Messaging/TrapV1Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TrapV1Message.cs#L123>`__

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.TrapV1Message.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/Messaging/TrapV1Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TrapV1Message.cs#L135>`__

