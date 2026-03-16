LegacyPdu Class
===============

.. dn:class:: Lextm.SharpSnmpLib.Messaging.LegacyPdu

   Legacy PDU facade exposed by compatibility APIs.

   .. code-block:: csharp

      public sealed class LegacyPdu : ISnmpPdu

**Namespace:** ``Lextm.SharpSnmpLib.Messaging``

**Inheritance:** Object → ``LegacyPdu``

**Source:** `SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs#L18>`__

Properties
----------

ErrorIndex
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.LegacyPdu.ErrorIndex

   Gets error Index.

   .. code-block:: csharp

      public Integer32 ErrorIndex { get; }

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.Integer32`

**Source:** `SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs#L84>`__

ErrorStatus
~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.LegacyPdu.ErrorStatus

   Gets error Status.

   .. code-block:: csharp

      public Integer32 ErrorStatus { get; }

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.Integer32`

**Source:** `SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs#L79>`__

RequestId
~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.LegacyPdu.RequestId

   Gets request id.

   .. code-block:: csharp

      public Integer32 RequestId { get; }

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.Integer32`

**Source:** `SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs#L89>`__

TypeCode
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.LegacyPdu.TypeCode

   Gets PDU type code.

   .. code-block:: csharp

      public SnmpType TypeCode { get; }

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`

**Source:** `SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs#L94>`__

Variables
~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.LegacyPdu.Variables

   Gets variables.

   .. code-block:: csharp

      public IList<Variable> Variables { get; }

   :rtype: ``IList<Variable>``

**Source:** `SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs#L74>`__

Operators
---------

Explicit(LegacyPdu to InformRequestPdu)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:operator:: Lextm.SharpSnmpLib.Messaging.LegacyPdu.op_Explicit(Lextm.SharpSnmpLib.Messaging.LegacyPdu)

   Casts to :dn:cls:``~DotNetSnmp.Protocol.V2.InformRequestPdu`` when possible.

   .. code-block:: csharp

      public static explicit operator InformRequestPdu(LegacyPdu pdu)

   :type pdu: :dn:cls:`~Lextm.SharpSnmpLib.Messaging.LegacyPdu`

   :rtype: :dn:cls:`~DotNetSnmp.Protocol.V2.InformRequestPdu`

**Source:** `SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs#L129>`__

Explicit(LegacyPdu to TrapV2Pdu)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:operator:: Lextm.SharpSnmpLib.Messaging.LegacyPdu.op_Explicit(Lextm.SharpSnmpLib.Messaging.LegacyPdu)

   Casts to :dn:cls:``~DotNetSnmp.Protocol.V2.TrapV2Pdu`` when possible.

   .. code-block:: csharp

      public static explicit operator TrapV2Pdu(LegacyPdu pdu)

   :type pdu: :dn:cls:`~Lextm.SharpSnmpLib.Messaging.LegacyPdu`

   :rtype: :dn:cls:`~DotNetSnmp.Protocol.V2.TrapV2Pdu`

**Source:** `SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs#L111>`__

