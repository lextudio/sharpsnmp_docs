GetNextRequestPdu Class
=======================

.. dn:class:: DotNetSnmp.Protocol.V1.GetNextRequestPdu

   GETNEXT request PDU.

   .. code-block:: csharp

      public class GetNextRequestPdu : Pdu, IScope, IAsnSerializable

**Namespace:** ``DotNetSnmp.Protocol.V1``

**Inheritance:** Object → Pdu → ``GetNextRequestPdu``

**Source:** `SharpSnmpLib/V1/GetNextRequestPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/GetNextRequestPdu.cs#L10>`__

Constructors
------------

GetNextRequestPdu()
~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Protocol.V1.GetNextRequestPdu..ctor

   Initializes a new instance of GetNextRequestPdu.

   .. code-block:: csharp

      public GetNextRequestPdu()

**Source:** `SharpSnmpLib/V1/GetNextRequestPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/GetNextRequestPdu.cs#L20>`__

Properties
----------

PduType
~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V1.GetNextRequestPdu.PduType

   Represents get Next Msg.

   .. code-block:: csharp

      public override Asn1Tag PduType { get; }

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/V1/GetNextRequestPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/GetNextRequestPdu.cs#L15>`__

Methods
-------

ReadFrom(AsnReader)
~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V1.GetNextRequestPdu.ReadFrom(System.Formats.Asn1.AsnReader)

   Reads a value from an ASN.1 reader.

   .. code-block:: csharp

      public static GetNextRequestPdu ReadFrom(AsnReader reader)

   :type reader: ``AsnReader``

   :rtype: :dn:cls:`~DotNetSnmp.Protocol.V1.GetNextRequestPdu`

**Source:** `SharpSnmpLib/V1/GetNextRequestPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/GetNextRequestPdu.cs#L29>`__

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V1.GetNextRequestPdu.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public override void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/V1/GetNextRequestPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/GetNextRequestPdu.cs#L50>`__

