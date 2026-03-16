SetRequestPdu Class
===================

.. dn:class:: DotNetSnmp.Protocol.V1.SetRequestPdu

   SET request PDU.

   .. code-block:: csharp

      public class SetRequestPdu : Pdu, IScope, IAsnSerializable

**Namespace:** ``DotNetSnmp.Protocol.V1``

**Inheritance:** Object → Pdu → ``SetRequestPdu``

**Source:** `SharpSnmpLib/V1/SetRequestPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/SetRequestPdu.cs#L10>`__

Constructors
------------

SetRequestPdu()
~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Protocol.V1.SetRequestPdu..ctor

   Initializes a new instance of SetRequestPdu.

   .. code-block:: csharp

      public SetRequestPdu()

**Source:** `SharpSnmpLib/V1/SetRequestPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/SetRequestPdu.cs#L20>`__

Properties
----------

PduType
~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V1.SetRequestPdu.PduType

   Represents set Msg.

   .. code-block:: csharp

      public override Asn1Tag PduType { get; }

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/V1/SetRequestPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/SetRequestPdu.cs#L15>`__

Methods
-------

ReadFrom(AsnReader)
~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V1.SetRequestPdu.ReadFrom(System.Formats.Asn1.AsnReader)

   Reads a value from an ASN.1 reader.

   .. code-block:: csharp

      public static SetRequestPdu ReadFrom(AsnReader reader)

   :type reader: ``AsnReader``

   :rtype: :dn:cls:`~DotNetSnmp.Protocol.V1.SetRequestPdu`

**Source:** `SharpSnmpLib/V1/SetRequestPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/SetRequestPdu.cs#L44>`__

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V1.SetRequestPdu.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public override void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/V1/SetRequestPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/SetRequestPdu.cs#L27>`__

