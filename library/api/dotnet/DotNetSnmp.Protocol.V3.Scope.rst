Scope Class
===========

.. dn:class:: DotNetSnmp.Protocol.V3.Scope

   Represents an SNMP v3 scoped PDU, which is a block of data containing a ContextEngineId, a ContextName, and a PDU.

   .. code-block:: csharp

      public class Scope : IScope, IAsnSerializable

**Namespace:** ``DotNetSnmp.Protocol.V3``

**Inheritance:** Object → ``Scope``

**Source:** `SharpSnmpLib/V3/Scope.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Scope.cs#L21>`__

Constructors
------------

Scope()
~~~~~~~

.. dn:constructor:: DotNetSnmp.Protocol.V3.Scope..ctor

   Initializes a new instance of :dn:cls:``~DotNetSnmp.Protocol.V3.Scope``.

   .. code-block:: csharp

      public Scope()

**Source:** `SharpSnmpLib/V3/Scope.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Scope.cs#L26>`__

Scope(OctetString, OctetString, Pdu)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Protocol.V3.Scope..ctor(DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Common.Definitions.Pdu)

   Initializes a legacy-compatible instance of :dn:cls:``~DotNetSnmp.Protocol.V3.Scope``.

   .. code-block:: csharp

      public Scope(OctetString contextEngineId, OctetString contextName, Pdu pdu)

   :type contextEngineId: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type contextName: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type pdu: :dn:cls:`~DotNetSnmp.Common.Definitions.Pdu`

**Source:** `SharpSnmpLib/V3/Scope.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Scope.cs#L35>`__

Properties
----------

ContextEngineId
~~~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Scope.ContextEngineId

   Gets context Engine Id.

   .. code-block:: csharp

      public ReadOnlyMemory<byte> ContextEngineId { get; set; }

   :returns: A byte array containing the context engine ID.
   :rtype: ``ReadOnlyMemory<Byte>``

**Source:** `SharpSnmpLib/V3/Scope.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Scope.cs#L52>`__

ContextName
~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Scope.ContextName

   Gets context Name.

   .. code-block:: csharp

      public string ContextName { get; set; }

   :returns: A string containing the context name.
   :rtype: ``String``

**Source:** `SharpSnmpLib/V3/Scope.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Scope.cs#L64>`__

Pdu
~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Scope.Pdu

   Gets the protocol data unit (PDU).

   .. code-block:: csharp

      public Pdu Pdu { get; set; }

   :returns: The PDU object representing an SNMP operation.
   :rtype: :dn:cls:`~DotNetSnmp.Common.Definitions.Pdu`

**Source:** `SharpSnmpLib/V3/Scope.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Scope.cs#L76>`__

RequestId
~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Scope.RequestId

   Gets request Id.

   .. code-block:: csharp

      public int RequestId { get; }

   :returns: An integer value that uniquely identifies this SNMP request or response.
   :rtype: ``Int32``

**Source:** `SharpSnmpLib/V3/Scope.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Scope.cs#L84>`__

TypeCode
~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Scope.TypeCode

   Legacy type code compatibility for scoped PDUs.

   .. code-block:: csharp

      public SnmpType TypeCode { get; }

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`

**Source:** `SharpSnmpLib/V3/Scope.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Scope.cs#L81>`__

VariableBindings
~~~~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Scope.VariableBindings

   Gets variable Bindings.

   .. code-block:: csharp

      public VarBindList? VariableBindings { get; set; }

   :returns: A collection of OID-value pairs representing the variables being requested, set, or returned in a response.
   :rtype: :dn:cls:`~DotNetSnmp.Asn1.SyntaxObjects.VarBindList`

**Source:** `SharpSnmpLib/V3/Scope.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Scope.cs#L87>`__

Methods
-------

GetData(VersionCode)
~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Scope.GetData(DotNetSnmp.Common.Definitions.VersionCode)

   Gets serialized scope data for the specified protocol version (legacy compatibility member).

   .. code-block:: csharp

      public IAsnSerializable GetData(VersionCode version)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`

   :rtype: :dn:iface:`~DotNetSnmp.Asn1.Serialization.IAsnSerializable`

**Source:** `SharpSnmpLib/V3/Scope.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Scope.cs#L188>`__

IsResponse()
~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Scope.IsResponse

   Determines whether response.

   .. code-block:: csharp

      public bool IsResponse()

   :returns: true if this scope is a response; otherwise, false.
   :rtype: ``Boolean``

**Source:** `SharpSnmpLib/V3/Scope.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Scope.cs#L180>`__

ReadFrom(AsnReader)
~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Scope.ReadFrom(System.Formats.Asn1.AsnReader)

   Deserializes a Scope object from an ASN.1 encoded representation.

   .. code-block:: csharp

      public static Scope ReadFrom(AsnReader reader)

   :param reader: The ASN.1 reader containing the encoded scope data.
   :type reader: ``AsnReader``

   :returns: A new instance of the Scope class populated with the deserialized data.
   :rtype: :dn:cls:`~DotNetSnmp.Protocol.V3.Scope`

**Source:** `SharpSnmpLib/V3/Scope.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Scope.cs#L120>`__

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Scope.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/V3/Scope.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Scope.cs#L94>`__

