ResponsePdu Class
=================

.. dn:class:: DotNetSnmp.Protocol.V1.ResponsePdu

   Represents the ResponsePdu type.

   .. code-block:: csharp

      public class ResponsePdu : Pdu, IScope, IAsnSerializable

**Namespace:** ``DotNetSnmp.Protocol.V1``

**Inheritance:** Object → Pdu → ``ResponsePdu``

**Source:** `SharpSnmpLib/V1/GetResponsePdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/GetResponsePdu.cs#L10>`__

Constructors
------------

ResponsePdu()
~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Protocol.V1.ResponsePdu..ctor

   Initializes a new instance of :dn:cls:``~DotNetSnmp.Protocol.V1.ResponsePdu``.

   .. code-block:: csharp

      public ResponsePdu()

**Source:** `SharpSnmpLib/V1/GetResponsePdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/GetResponsePdu.cs#L15>`__

ResponsePdu(Int32, ErrorCode, Int32, IList<Variable>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Protocol.V1.ResponsePdu..ctor(System.Int32,DotNetSnmp.Common.Definitions.ErrorCode,System.Int32,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable})

   Initializes a legacy-compatible instance of :dn:cls:``~DotNetSnmp.Protocol.V1.ResponsePdu``.

   .. code-block:: csharp

      public ResponsePdu(int requestId, ErrorCode errorStatus, int errorIndex, IList<Variable> variables)

   :type requestId: ``Int32``
   :type errorStatus: :dn:enum:`~DotNetSnmp.Common.Definitions.ErrorCode`
   :type errorIndex: ``Int32``
   :type variables: ``IList<Variable>``

**Source:** `SharpSnmpLib/V1/GetResponsePdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/GetResponsePdu.cs#L22>`__

Properties
----------

PduType
~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V1.ResponsePdu.PduType

   Represents get Response Msg.

   .. code-block:: csharp

      public override Asn1Tag PduType { get; }

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/V1/GetResponsePdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/GetResponsePdu.cs#L33>`__

Methods
-------

ReadFrom(AsnReader)
~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V1.ResponsePdu.ReadFrom(System.Formats.Asn1.AsnReader)

   Reads a value from an ASN.1 reader.

   .. code-block:: csharp

      public static ResponsePdu ReadFrom(AsnReader reader)

   :type reader: ``AsnReader``

   :rtype: :dn:cls:`~DotNetSnmp.Protocol.V1.ResponsePdu`

**Source:** `SharpSnmpLib/V1/GetResponsePdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/GetResponsePdu.cs#L53>`__

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V1.ResponsePdu.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public override void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/V1/GetResponsePdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/GetResponsePdu.cs#L36>`__

