GetRequestPdu Class
===================

.. dn:class:: DotNetSnmp.Protocol.V1.GetRequestPdu

   GET request PDU.

   .. code-block:: csharp

      public class GetRequestPdu : Pdu, IScope, IAsnSerializable

**Namespace:** ``DotNetSnmp.Protocol.V1``

**Inheritance:** Object → Pdu → ``GetRequestPdu``

**Source:** `SharpSnmpLib/V1/GetRequestPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/GetRequestPdu.cs#L11>`__

Constructors
------------

GetRequestPdu()
~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Protocol.V1.GetRequestPdu..ctor

   Initializes a new instance of GetRequestPdu.

   .. code-block:: csharp

      public GetRequestPdu()

**Source:** `SharpSnmpLib/V1/GetRequestPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/GetRequestPdu.cs#L21>`__

GetRequestPdu(Int32, IList<Variable>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Protocol.V1.GetRequestPdu..ctor(System.Int32,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable})

   Initializes a new instance of GetRequestPdu (legacy compatibility overload).

   .. code-block:: csharp

      public GetRequestPdu(int requestId, IList<Variable> variables)

   :type requestId: ``Int32``
   :type variables: ``IList<Variable>``

**Source:** `SharpSnmpLib/V1/GetRequestPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/GetRequestPdu.cs#L30>`__

Properties
----------

PduType
~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V1.GetRequestPdu.PduType

   Represents get Msg.

   .. code-block:: csharp

      public override Asn1Tag PduType { get; }

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/V1/GetRequestPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/GetRequestPdu.cs#L16>`__

Methods
-------

ReadFrom(AsnReader)
~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V1.GetRequestPdu.ReadFrom(System.Formats.Asn1.AsnReader)

   Reads a value from an ASN.1 reader.

   .. code-block:: csharp

      public static GetRequestPdu ReadFrom(AsnReader reader)

   :type reader: ``AsnReader``

   :rtype: :dn:cls:`~DotNetSnmp.Protocol.V1.GetRequestPdu`

**Source:** `SharpSnmpLib/V1/GetRequestPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/GetRequestPdu.cs#L66>`__

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V1.GetRequestPdu.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public override void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/V1/GetRequestPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V1/GetRequestPdu.cs#L49>`__

