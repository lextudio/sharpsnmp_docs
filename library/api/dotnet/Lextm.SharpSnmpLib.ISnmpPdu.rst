ISnmpPdu Interface
==================

.. dn:interface:: Lextm.SharpSnmpLib.ISnmpPdu

   Legacy compatibility abstraction for SNMP PDU data.

   .. code-block:: csharp

      public interface ISnmpPdu

**Namespace:** ``Lextm.SharpSnmpLib``

**Source:** `SharpSnmpLib/ISnmpPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/ISnmpPdu.cs#L9>`__

Properties
----------

ErrorIndex
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.ISnmpPdu.ErrorIndex

   Gets error index.

   .. code-block:: csharp

      Integer32 ErrorIndex { get; }

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.Integer32`

**Source:** `SharpSnmpLib/ISnmpPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/ISnmpPdu.cs#L24>`__

ErrorStatus
~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.ISnmpPdu.ErrorStatus

   Gets error status.

   .. code-block:: csharp

      Integer32 ErrorStatus { get; }

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.Integer32`

**Source:** `SharpSnmpLib/ISnmpPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/ISnmpPdu.cs#L19>`__

RequestId
~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.ISnmpPdu.RequestId

   Gets request id.

   .. code-block:: csharp

      Integer32 RequestId { get; }

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.Integer32`

**Source:** `SharpSnmpLib/ISnmpPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/ISnmpPdu.cs#L14>`__

TypeCode
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.ISnmpPdu.TypeCode

   Gets PDU type code.

   .. code-block:: csharp

      SnmpType TypeCode { get; }

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`

**Source:** `SharpSnmpLib/ISnmpPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/ISnmpPdu.cs#L34>`__

Variables
~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.ISnmpPdu.Variables

   Gets variable bindings.

   .. code-block:: csharp

      IList<Variable> Variables { get; }

   :rtype: ``IList<Variable>``

**Source:** `SharpSnmpLib/ISnmpPdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/ISnmpPdu.cs#L29>`__

