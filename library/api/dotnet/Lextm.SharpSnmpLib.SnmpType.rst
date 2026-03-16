SnmpType Enum
=============

.. dn:enum:: Lextm.SharpSnmpLib.SnmpType

   SNMP type code. The values are tag values for SNMP types.

   .. code-block:: csharp

      [DataContract]
      public enum SnmpType

**Namespace:** ``Lextm.SharpSnmpLib``

**Source:** `SharpSnmpLib/SnmpType.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SnmpType.cs#L7>`__

Fields
------

Counter32
~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpLib.SnmpType.Counter32

   Counter32 type. (SMIv1, SMIv2)

   .. code-block:: csharp

      Counter32 = 65

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`

**Source:** `SharpSnmpLib/SnmpType.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SnmpType.cs#L41>`__

Counter64
~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpLib.SnmpType.Counter64

   Counter64 type. (SMIv2)

   .. code-block:: csharp

      Counter64 = 70

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`

**Source:** `SharpSnmpLib/SnmpType.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SnmpType.cs#L61>`__

EndMarker
~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpLib.SnmpType.EndMarker

   End marker.

   .. code-block:: csharp

      EndMarker = 0

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`

**Source:** `SharpSnmpLib/SnmpType.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SnmpType.cs#L13>`__

EndOfMibView
~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpLib.SnmpType.EndOfMibView

   End of MIB view exception.

   .. code-block:: csharp

      EndOfMibView = 130

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`

**Source:** `SharpSnmpLib/SnmpType.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SnmpType.cs#L77>`__

Gauge32
~~~~~~~

.. dn:field:: Lextm.SharpSnmpLib.SnmpType.Gauge32

   Gauge32 type. (SMIv1, SMIv2)

   .. code-block:: csharp

      Gauge32 = 66

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`

**Source:** `SharpSnmpLib/SnmpType.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SnmpType.cs#L45>`__

GetBulkRequestPdu
~~~~~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpLib.SnmpType.GetBulkRequestPdu

   Get Bulk PDU.

   .. code-block:: csharp

      GetBulkRequestPdu = 165

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`

**Source:** `SharpSnmpLib/SnmpType.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SnmpType.cs#L101>`__

GetNextRequestPdu
~~~~~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpLib.SnmpType.GetNextRequestPdu

   Get Next request PDU.

   .. code-block:: csharp

      GetNextRequestPdu = 161

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`

**Source:** `SharpSnmpLib/SnmpType.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SnmpType.cs#L85>`__

GetRequestPdu
~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpLib.SnmpType.GetRequestPdu

   Get request PDU.

   .. code-block:: csharp

      GetRequestPdu = 160

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`

**Source:** `SharpSnmpLib/SnmpType.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SnmpType.cs#L81>`__

InformRequestPdu
~~~~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpLib.SnmpType.InformRequestPdu

   Inform PDU.

   .. code-block:: csharp

      InformRequestPdu = 166

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`

**Source:** `SharpSnmpLib/SnmpType.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SnmpType.cs#L105>`__

Integer32
~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpLib.SnmpType.Integer32

   INTEGER type. (SMIv1, SMIv2)

   .. code-block:: csharp

      Integer32 = 2

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`

**Source:** `SharpSnmpLib/SnmpType.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SnmpType.cs#L17>`__

IPAddress
~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpLib.SnmpType.IPAddress

   IpAddress type. (SMIv1)

   .. code-block:: csharp

      IPAddress = 64

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`

**Source:** `SharpSnmpLib/SnmpType.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SnmpType.cs#L37>`__

NetAddress
~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpLib.SnmpType.NetAddress

   Network Address. (SMIv1)

   .. code-block:: csharp

      NetAddress = 69

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`

**Source:** `SharpSnmpLib/SnmpType.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SnmpType.cs#L57>`__

NoSuchInstance
~~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpLib.SnmpType.NoSuchInstance

   No such instance exception.

   .. code-block:: csharp

      NoSuchInstance = 129

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`

**Source:** `SharpSnmpLib/SnmpType.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SnmpType.cs#L73>`__

NoSuchObject
~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpLib.SnmpType.NoSuchObject

   No such object exception.

   .. code-block:: csharp

      NoSuchObject = 128

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`

**Source:** `SharpSnmpLib/SnmpType.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SnmpType.cs#L69>`__

Null
~~~~

.. dn:field:: Lextm.SharpSnmpLib.SnmpType.Null

   NULL type. (SMIv1)

   .. code-block:: csharp

      Null = 5

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`

**Source:** `SharpSnmpLib/SnmpType.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SnmpType.cs#L25>`__

ObjectIdentifier
~~~~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpLib.SnmpType.ObjectIdentifier

   OBJECT IDENTIFIER type. (SMIv1)

   .. code-block:: csharp

      ObjectIdentifier = 6

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`

**Source:** `SharpSnmpLib/SnmpType.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SnmpType.cs#L29>`__

OctetString
~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpLib.SnmpType.OctetString

   OCTET STRING type.

   .. code-block:: csharp

      OctetString = 4

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`

**Source:** `SharpSnmpLib/SnmpType.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SnmpType.cs#L21>`__

Opaque
~~~~~~

.. dn:field:: Lextm.SharpSnmpLib.SnmpType.Opaque

   Opaque type. (SMIv1)

   .. code-block:: csharp

      Opaque = 68

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`

**Source:** `SharpSnmpLib/SnmpType.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SnmpType.cs#L53>`__

ReportPdu
~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpLib.SnmpType.ReportPdu

   Report PDU. SNMP v3.

   .. code-block:: csharp

      ReportPdu = 168

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`

**Source:** `SharpSnmpLib/SnmpType.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SnmpType.cs#L113>`__

ResponsePdu
~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpLib.SnmpType.ResponsePdu

   Response PDU.

   .. code-block:: csharp

      ResponsePdu = 162

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`

**Source:** `SharpSnmpLib/SnmpType.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SnmpType.cs#L89>`__

Sequence
~~~~~~~~

.. dn:field:: Lextm.SharpSnmpLib.SnmpType.Sequence

   RFC1213 sequence for whole SNMP packet beginning

   .. code-block:: csharp

      Sequence = 48

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`

**Source:** `SharpSnmpLib/SnmpType.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SnmpType.cs#L33>`__

SetRequestPdu
~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpLib.SnmpType.SetRequestPdu

   Set request PDU.

   .. code-block:: csharp

      SetRequestPdu = 163

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`

**Source:** `SharpSnmpLib/SnmpType.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SnmpType.cs#L93>`__

TimeTicks
~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpLib.SnmpType.TimeTicks

   TimeTicks type. (SMIv1)

   .. code-block:: csharp

      TimeTicks = 67

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`

**Source:** `SharpSnmpLib/SnmpType.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SnmpType.cs#L49>`__

TrapV1Pdu
~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpLib.SnmpType.TrapV1Pdu

   Trap v1 PDU.

   .. code-block:: csharp

      TrapV1Pdu = 164

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`

**Source:** `SharpSnmpLib/SnmpType.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SnmpType.cs#L97>`__

TrapV2Pdu
~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpLib.SnmpType.TrapV2Pdu

   Trap v2 PDU.

   .. code-block:: csharp

      TrapV2Pdu = 167

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`

**Source:** `SharpSnmpLib/SnmpType.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SnmpType.cs#L109>`__

Unknown
~~~~~~~

.. dn:field:: Lextm.SharpSnmpLib.SnmpType.Unknown

   Defined by #SNMP for unknown type.

   .. code-block:: csharp

      Unknown = 65535

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`

**Source:** `SharpSnmpLib/SnmpType.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SnmpType.cs#L117>`__

Unsigned32
~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpLib.SnmpType.Unsigned32

   Unsigned32 type. (Use this code in RFC 1442)

   .. code-block:: csharp

      Unsigned32 = 71

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`

**Source:** `SharpSnmpLib/SnmpType.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SnmpType.cs#L65>`__

