ReportPdu Class
===============

.. dn:class:: DotNetSnmp.Protocol.V1.ReportPdu

   Report PDU.

   .. code-block:: csharp

      public class ReportPdu : Pdu, IScope, IAsnSerializable

**Namespace:** ``DotNetSnmp.Protocol.V1``

**Inheritance:** Object → Pdu → ``ReportPdu``

**Source:** `SharpSnmpLib/V2c/ReportPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V2c/ReportPdu.cs#L10>`__

Constructors
------------

ReportPdu()
~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Protocol.V1.ReportPdu..ctor

   Initializes a new instance of :dn:cls:``~DotNetSnmp.Protocol.V1.ReportPdu``.

   .. code-block:: csharp

      public ReportPdu()

**Source:** `SharpSnmpLib/V2c/ReportPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V2c/ReportPdu.cs#L15>`__

ReportPdu(Int32, ErrorCode, Int32, IList<Variable>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Protocol.V1.ReportPdu..ctor(System.Int32,DotNetSnmp.Common.Definitions.ErrorCode,System.Int32,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable})

   Initializes a legacy-compatible instance of :dn:cls:``~DotNetSnmp.Protocol.V1.ReportPdu``.

   .. code-block:: csharp

      public ReportPdu(int requestId, ErrorCode errorStatus, int errorIndex, IList<Variable> variables)

   :type requestId: ``Int32``
   :type errorStatus: :dn:enum:`~DotNetSnmp.Common.Definitions.ErrorCode`
   :type errorIndex: ``Int32``
   :type variables: ``IList<Variable>``

**Source:** `SharpSnmpLib/V2c/ReportPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V2c/ReportPdu.cs#L22>`__

Properties
----------

PduType
~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V1.ReportPdu.PduType

   Represents report Msg.

   .. code-block:: csharp

      public override Asn1Tag PduType { get; }

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/V2c/ReportPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V2c/ReportPdu.cs#L33>`__

Methods
-------

ReadFrom(AsnReader)
~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V1.ReportPdu.ReadFrom(System.Formats.Asn1.AsnReader)

   Reads a value from an ASN.1 reader.

   .. code-block:: csharp

      public static ReportPdu ReadFrom(AsnReader reader)

   :type reader: ``AsnReader``

   :rtype: :dn:cls:`~DotNetSnmp.Protocol.V1.ReportPdu`

**Source:** `SharpSnmpLib/V2c/ReportPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V2c/ReportPdu.cs#L53>`__

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V1.ReportPdu.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public override void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/V2c/ReportPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V2c/ReportPdu.cs#L36>`__

