TrapV2Message Class
===================

.. dn:class:: Lextm.SharpSnmpLib.Messaging.TrapV2Message

   Legacy compatibility wrapper for TrapV2 message sending.

   .. code-block:: csharp

      public sealed class TrapV2Message : ISnmpMessage, IAsnSerializable

**Namespace:** ``Lextm.SharpSnmpLib.Messaging``

**Inheritance:** Object → ``TrapV2Message``

**Source:** `SharpSnmpLib/Messaging/TrapV2Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TrapV2Message.cs#L13>`__

Constructors
------------

TrapV2Message(Int32, VersionCode, OctetString, ObjectIdentifier, UInt32, IList<Variable>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Messaging.TrapV2Message..ctor(System.Int32,DotNetSnmp.Common.Definitions.VersionCode,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,System.UInt32,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable})

   Initializes a new instance of TrapV2Message.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public TrapV2Message(int requestId, VersionCode version, OctetString community, ObjectIdentifier enterprise, uint timestamp, IList<Variable> variables)

   :type requestId: ``Int32``
   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type enterprise: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type timestamp: ``UInt32``
   :type variables: ``IList<Variable>``

**Source:** `SharpSnmpLib/Messaging/TrapV2Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TrapV2Message.cs#L23>`__

TrapV2Message(VersionCode, Int32, Int32, OctetString, ObjectIdentifier, UInt32, IList<Variable>, IPrivacyProvider, Int32, OctetString, Int32, Int32)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Messaging.TrapV2Message..ctor(DotNetSnmp.Common.Definitions.VersionCode,System.Int32,System.Int32,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,System.UInt32,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider,System.Int32,DotNetSnmp.Asn1.SyntaxObjects.OctetString,System.Int32,System.Int32)

   Initializes a new instance of TrapV2Message.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public TrapV2Message(VersionCode version, int messageId, int requestId, OctetString user, ObjectIdentifier enterprise, uint timestamp, IList<Variable> variables, IPrivacyProvider privacy, int maxMessageSize, OctetString engineId, int engineBoots, int engineTime)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type messageId: ``Int32``
   :type requestId: ``Int32``
   :type user: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type enterprise: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type timestamp: ``UInt32``
   :type variables: ``IList<Variable>``
   :type privacy: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`
   :type maxMessageSize: ``Int32``
   :type engineId: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type engineBoots: ``Int32``
   :type engineTime: ``Int32``

**Source:** `SharpSnmpLib/Messaging/TrapV2Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TrapV2Message.cs#L43>`__

Properties
----------

EngineBoots
~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.TrapV2Message.EngineBoots

   Gets engine Boots.

   .. code-block:: csharp

      public int EngineBoots { get; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Messaging/TrapV2Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TrapV2Message.cs#L122>`__

EngineId
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.TrapV2Message.EngineId

   Gets engine Id.

   .. code-block:: csharp

      public OctetString EngineId { get; }

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`

**Source:** `SharpSnmpLib/Messaging/TrapV2Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TrapV2Message.cs#L117>`__

EngineTime
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.TrapV2Message.EngineTime

   Gets engine Time.

   .. code-block:: csharp

      public int EngineTime { get; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Messaging/TrapV2Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TrapV2Message.cs#L127>`__

Enterprise
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.TrapV2Message.Enterprise

   Enterprise.

   .. code-block:: csharp

      public ObjectIdentifier Enterprise { get; }

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`

**Source:** `SharpSnmpLib/Messaging/TrapV2Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TrapV2Message.cs#L132>`__

MaxMessageSize
~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.TrapV2Message.MaxMessageSize

   Gets max Message Size.

   .. code-block:: csharp

      public int MaxMessageSize { get; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Messaging/TrapV2Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TrapV2Message.cs#L112>`__

MessageId
~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.TrapV2Message.MessageId

   Gets message Id.

   .. code-block:: csharp

      public int MessageId { get; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Messaging/TrapV2Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TrapV2Message.cs#L107>`__

ProtocolVersion
~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.TrapV2Message.ProtocolVersion

   Gets the SNMP protocol version.

   .. code-block:: csharp

      public VersionCode ProtocolVersion { get; }

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`

**Source:** `SharpSnmpLib/Messaging/TrapV2Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TrapV2Message.cs#L205>`__

Scope
~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.TrapV2Message.Scope

   Gets the message scope.

   .. code-block:: csharp

      public IScope? Scope { get; }

   :rtype: :dn:iface:`~DotNetSnmp.Common.Definitions.IScope`

**Source:** `SharpSnmpLib/Messaging/TrapV2Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TrapV2Message.cs#L208>`__

TimeStamp
~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.TrapV2Message.TimeStamp

   Time stamp.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public uint TimeStamp { get; }

   :rtype: ``UInt32``

**Source:** `SharpSnmpLib/Messaging/TrapV2Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TrapV2Message.cs#L137>`__

Version
~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.TrapV2Message.Version

   Gets version.

   .. code-block:: csharp

      public VersionCode Version { get; }

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`

**Source:** `SharpSnmpLib/Messaging/TrapV2Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TrapV2Message.cs#L102>`__

Methods
-------

Send(IPEndPoint)
~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.TrapV2Message.Send(System.Net.IPEndPoint)

   Sends the trap to the specified endpoint.

   .. code-block:: csharp

      public void Send(IPEndPoint endpoint)

   :type endpoint: ``IPEndPoint``

**Source:** `SharpSnmpLib/Messaging/TrapV2Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TrapV2Message.cs#L153>`__

SendAsync(IPEndPoint, CancellationToken)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.TrapV2Message.SendAsync(System.Net.IPEndPoint,System.Threading.CancellationToken)

   Sends the trap to the specified endpoint asynchronously.

   .. code-block:: csharp

      public Task SendAsync(IPEndPoint endpoint, CancellationToken cancellationToken)

   :type endpoint: ``IPEndPoint``
   :type cancellationToken: ``CancellationToken``

   :rtype: ``Task``

**Source:** `SharpSnmpLib/Messaging/TrapV2Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TrapV2Message.cs#L190>`__

SendAsync(IPEndPoint)
~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.TrapV2Message.SendAsync(System.Net.IPEndPoint)

   Sends the trap to the specified endpoint asynchronously.

   .. code-block:: csharp

      public Task SendAsync(IPEndPoint endpoint)

   :type endpoint: ``IPEndPoint``

   :rtype: ``Task``

**Source:** `SharpSnmpLib/Messaging/TrapV2Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TrapV2Message.cs#L166>`__

ToBytes()
~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.TrapV2Message.ToBytes

   Serializes the message to bytes when this instance wraps a parsed SNMP message.

   .. code-block:: csharp

      public byte[] ToBytes()

   :rtype: ``Byte[]``

**Source:** `SharpSnmpLib/Messaging/TrapV2Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TrapV2Message.cs#L213>`__

ToString()
~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.TrapV2Message.ToString

   Returns a ``String`` that represents the current :dn:cls:``~Lextm.SharpSnmpLib.Messaging.TrapV2Message``.

   .. code-block:: csharp

      public override string ToString()

   :rtype: ``String``

**Source:** `SharpSnmpLib/Messaging/TrapV2Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TrapV2Message.cs#L199>`__

Variables()
~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.TrapV2Message.Variables

   Gets the variable bindings carried by this trap message.

   .. code-block:: csharp

      public IList<Variable> Variables()

   :rtype: ``IList<Variable>``

**Source:** `SharpSnmpLib/Messaging/TrapV2Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TrapV2Message.cs#L145>`__

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.TrapV2Message.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/Messaging/TrapV2Message.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TrapV2Message.cs#L241>`__

