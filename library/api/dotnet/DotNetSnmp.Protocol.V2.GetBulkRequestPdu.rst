GetBulkRequestPdu Class
=======================

.. dn:class:: DotNetSnmp.Protocol.V2.GetBulkRequestPdu

   Represents the GetBulkRequestPdu type.

   .. code-block:: csharp

      public class GetBulkRequestPdu : Pdu, IScope, IAsnSerializable

**Namespace:** ``DotNetSnmp.Protocol.V2``

**Inheritance:** Object → Pdu → ``GetBulkRequestPdu``

**Source:** `SharpSnmpLib/V2c/BulkRequestPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V2c/BulkRequestPdu.cs#L10>`__

Properties
----------

MaxRepetitions
~~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V2.GetBulkRequestPdu.MaxRepetitions

   how many GET_NEXT operations to perform on each variable

   .. code-block:: csharp

      public int MaxRepetitions { get; set; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/V2c/BulkRequestPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V2c/BulkRequestPdu.cs#L20>`__

NonRepeaters
~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V2.GetBulkRequestPdu.NonRepeaters

   how many OIDs in the request should be treated as GET request variables

   .. code-block:: csharp

      public int NonRepeaters { get; set; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/V2c/BulkRequestPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V2c/BulkRequestPdu.cs#L15>`__

PduType
~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V2.GetBulkRequestPdu.PduType

   Represents bulk Msg.

   .. code-block:: csharp

      public override Asn1Tag PduType { get; }

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/V2c/BulkRequestPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V2c/BulkRequestPdu.cs#L25>`__

Methods
-------

ReadFrom(AsnReader)
~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V2.GetBulkRequestPdu.ReadFrom(System.Formats.Asn1.AsnReader)

   Reads a value from an ASN.1 reader.

   .. code-block:: csharp

      public static GetBulkRequestPdu ReadFrom(AsnReader reader)

   :type reader: ``AsnReader``

   :rtype: :dn:cls:`~DotNetSnmp.Protocol.V2.GetBulkRequestPdu`

**Source:** `SharpSnmpLib/V2c/BulkRequestPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V2c/BulkRequestPdu.cs#L30>`__

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V2.GetBulkRequestPdu.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public override void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/V2c/BulkRequestPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V2c/BulkRequestPdu.cs#L51>`__

