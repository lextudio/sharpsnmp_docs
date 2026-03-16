InformRequestMessage Class
==========================

.. dn:class:: Lextm.SharpSnmpLib.Messaging.InformRequestMessage

   Legacy compatibility wrapper for SNMP INFORM request messages.

   .. code-block:: csharp

      public sealed class InformRequestMessage : ISnmpMessage, IAsnSerializable

**Namespace:** ``Lextm.SharpSnmpLib.Messaging``

**Inheritance:** Object → ``InformRequestMessage``

**Source:** `SharpSnmpLib/Messaging/InformRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/InformRequestMessage.cs#L12>`__

Constructors
------------

InformRequestMessage(Int32, VersionCode, OctetString, ObjectIdentifier, UInt32, IList<Variable>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Messaging.InformRequestMessage..ctor(System.Int32,DotNetSnmp.Common.Definitions.VersionCode,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,System.UInt32,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable})

   Creates a :dn:cls:``~Lextm.SharpSnmpLib.Messaging.InformRequestMessage`` with all contents (v1/v2c).

   .. code-block:: csharp

      [CLSCompliant(false)]
      public InformRequestMessage(int requestId, VersionCode version, OctetString community, ObjectIdentifier enterprise, uint time, IList<Variable> variables)

   :param requestId: The request id.
   :type requestId: ``Int32``
   :param version: Protocol version.
   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :param community: Community name.
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :param enterprise: Enterprise.
   :type enterprise: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :param time: Time ticks.
   :type time: ``UInt32``
   :param variables: Variables.
   :type variables: ``IList<Variable>``

**Source:** `SharpSnmpLib/Messaging/InformRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/InformRequestMessage.cs#L26>`__

Properties
----------

Enterprise
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.InformRequestMessage.Enterprise

   Enterprise.

   .. code-block:: csharp

      public ObjectIdentifier Enterprise { get; }

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`

**Source:** `SharpSnmpLib/Messaging/InformRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/InformRequestMessage.cs#L90>`__

ProtocolVersion
~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.InformRequestMessage.ProtocolVersion

   Gets the SNMP protocol version.

   .. code-block:: csharp

      public VersionCode ProtocolVersion { get; }

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`

**Source:** `SharpSnmpLib/Messaging/InformRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/InformRequestMessage.cs#L107>`__

Scope
~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.InformRequestMessage.Scope

   Gets the message scope.

   .. code-block:: csharp

      public IScope? Scope { get; }

   :rtype: :dn:iface:`~DotNetSnmp.Common.Definitions.IScope`

**Source:** `SharpSnmpLib/Messaging/InformRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/InformRequestMessage.cs#L110>`__

TimeStamp
~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.InformRequestMessage.TimeStamp

   Time stamp.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public uint TimeStamp { get; }

   :rtype: ``UInt32``

**Source:** `SharpSnmpLib/Messaging/InformRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/InformRequestMessage.cs#L95>`__

Version
~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.InformRequestMessage.Version

   Protocol version.

   .. code-block:: csharp

      public VersionCode Version { get; }

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`

**Source:** `SharpSnmpLib/Messaging/InformRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/InformRequestMessage.cs#L85>`__

Methods
-------

ToBytes()
~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.InformRequestMessage.ToBytes

   Serializes the message to a byte array.

   .. code-block:: csharp

      public byte[] ToBytes()

   :rtype: ``Byte[]``

**Source:** `SharpSnmpLib/Messaging/InformRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/InformRequestMessage.cs#L121>`__

ToString()
~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.InformRequestMessage.ToString

   Returns a string representation.

   .. code-block:: csharp

      public override string ToString()

   :rtype: ``String``

**Source:** `SharpSnmpLib/Messaging/InformRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/InformRequestMessage.cs#L129>`__

Variables()
~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.InformRequestMessage.Variables

   Gets the variable bindings.

   .. code-block:: csharp

      public IList<Variable> Variables()

   :rtype: ``IList<Variable>``

**Source:** `SharpSnmpLib/Messaging/InformRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/InformRequestMessage.cs#L101>`__

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.InformRequestMessage.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/Messaging/InformRequestMessage.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/InformRequestMessage.cs#L113>`__

