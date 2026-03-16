TrapPdu Class
=============

.. dn:class:: DotNetSnmp.Protocol.V1.TrapPdu

   Represents the TrapPdu type.

   .. code-block:: csharp

      public class TrapPdu : Pdu, IScope, IAsnSerializable

**Namespace:** ``DotNetSnmp.Protocol.V1``

**Inheritance:** Object → Pdu → ``TrapPdu``

**Source:** `SharpSnmpLib/V1/TrapPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/TrapPdu.cs#L11>`__

Properties
----------

AgentAddress
~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V1.TrapPdu.AgentAddress

   Gets agent Address.

   .. code-block:: csharp

      public IPAddress? AgentAddress { get; set; }

   :rtype: ``IPAddress``

**Source:** `SharpSnmpLib/V1/TrapPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/TrapPdu.cs#L20>`__

Enterprise
~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V1.TrapPdu.Enterprise

   Gets enterprise.

   .. code-block:: csharp

      public ObjectIdentifier Enterprise { get; set; }

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`

**Source:** `SharpSnmpLib/V1/TrapPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/TrapPdu.cs#L16>`__

GenericTrap
~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V1.TrapPdu.GenericTrap

   Gets generic Trap.

   .. code-block:: csharp

      public int GenericTrap { get; set; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/V1/TrapPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/TrapPdu.cs#L24>`__

PduType
~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V1.TrapPdu.PduType

   Represents trap Msg.

   .. code-block:: csharp

      public override Asn1Tag PduType { get; }

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/V1/TrapPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/TrapPdu.cs#L38>`__

SpecificTrap
~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V1.TrapPdu.SpecificTrap

   Gets specific Trap.

   .. code-block:: csharp

      public int SpecificTrap { get; set; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/V1/TrapPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/TrapPdu.cs#L28>`__

TimeStamp
~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V1.TrapPdu.TimeStamp

   Gets time Stamp.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public uint TimeStamp { get; set; }

   :rtype: ``UInt32``

**Source:** `SharpSnmpLib/V1/TrapPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/TrapPdu.cs#L32>`__

Methods
-------

ReadFrom(AsnReader)
~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V1.TrapPdu.ReadFrom(System.Formats.Asn1.AsnReader)

   Reads a value from an ASN.1 reader.

   .. code-block:: csharp

      public static TrapPdu ReadFrom(AsnReader reader)

   :type reader: ``AsnReader``

   :rtype: :dn:cls:`~DotNetSnmp.Protocol.V1.TrapPdu`

**Source:** `SharpSnmpLib/V1/TrapPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/TrapPdu.cs#L60>`__

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V1.TrapPdu.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public override void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/V1/TrapPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/TrapPdu.cs#L41>`__

