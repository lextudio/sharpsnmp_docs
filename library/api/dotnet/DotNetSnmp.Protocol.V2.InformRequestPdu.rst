InformRequestPdu Class
======================

.. dn:class:: DotNetSnmp.Protocol.V2.InformRequestPdu

   INFORM request PDU.

   .. code-block:: csharp

      public class InformRequestPdu : Pdu, IScope, IAsnSerializable

**Namespace:** ``DotNetSnmp.Protocol.V2``

**Inheritance:** Object → Pdu → ``InformRequestPdu``

**Source:** `SharpSnmpLib/V2c/InformRequestPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V2c/InformRequestPdu.cs#L10>`__

Constructors
------------

InformRequestPdu()
~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Protocol.V2.InformRequestPdu..ctor

   Initializes a new instance of :dn:cls:``~DotNetSnmp.Protocol.V2.InformRequestPdu``.

   .. code-block:: csharp

      public InformRequestPdu()

**Source:** `SharpSnmpLib/V2c/InformRequestPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V2c/InformRequestPdu.cs#L18>`__

InformRequestPdu(Int32, ObjectIdentifier, UInt32, IList<Variable>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Protocol.V2.InformRequestPdu..ctor(System.Int32,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,System.UInt32,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable})

   Initializes a legacy-compatible instance of :dn:cls:``~DotNetSnmp.Protocol.V2.InformRequestPdu``.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public InformRequestPdu(int requestId, ObjectIdentifier enterprise, uint timeStamp, IList<Variable> variables)

   :type requestId: ``Int32``
   :type enterprise: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type timeStamp: ``UInt32``
   :type variables: ``IList<Variable>``

**Source:** `SharpSnmpLib/V2c/InformRequestPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V2c/InformRequestPdu.cs#L26>`__

Properties
----------

Enterprise
~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V2.InformRequestPdu.Enterprise

   Gets enterprise.

   .. code-block:: csharp

      public ObjectIdentifier Enterprise { get; set; }

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`

**Source:** `SharpSnmpLib/V2c/InformRequestPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V2c/InformRequestPdu.cs#L44>`__

PduType
~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V2.InformRequestPdu.PduType

   Represents inform Msg.

   .. code-block:: csharp

      public override Asn1Tag PduType { get; }

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/V2c/InformRequestPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V2c/InformRequestPdu.cs#L49>`__

TimeStamp
~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V2.InformRequestPdu.TimeStamp

   Gets time Stamp.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public uint TimeStamp { get; set; }

   :rtype: ``UInt32``

**Source:** `SharpSnmpLib/V2c/InformRequestPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V2c/InformRequestPdu.cs#L38>`__

Methods
-------

Decorate(IList<Variable>)
~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V2.InformRequestPdu.Decorate(System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable})

   Decorates variable bindings with timestamp and enterprise metadata.

   .. code-block:: csharp

      public IList<Variable> Decorate(IList<Variable> variables)

   :type variables: ``IList<Variable>``

   :rtype: ``IList<Variable>``

**Source:** `SharpSnmpLib/V2c/InformRequestPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V2c/InformRequestPdu.cs#L103>`__

ReadFrom(AsnReader)
~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V2.InformRequestPdu.ReadFrom(System.Formats.Asn1.AsnReader)

   Reads a value from an ASN.1 reader.

   .. code-block:: csharp

      public static InformRequestPdu ReadFrom(AsnReader reader)

   :type reader: ``AsnReader``

   :rtype: :dn:cls:`~DotNetSnmp.Protocol.V2.InformRequestPdu`

**Source:** `SharpSnmpLib/V2c/InformRequestPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V2c/InformRequestPdu.cs#L54>`__

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V2.InformRequestPdu.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public override void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/V2c/InformRequestPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V2c/InformRequestPdu.cs#L77>`__

