Pdu Class
=========

.. dn:class:: DotNetSnmp.Common.Definitions.Pdu

   The base class for all SNMP PDU types.

   .. code-block:: csharp

      public abstract class Pdu : IScope, IAsnSerializable

**Namespace:** ``DotNetSnmp.Common.Definitions``

**Inheritance:** Object → ``Pdu``

**Source:** `SharpSnmpLib/Common/Pdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/Pdu.cs#L20>`__

Properties
----------

ErrorIndex
~~~~~~~~~~

.. dn:property:: DotNetSnmp.Common.Definitions.Pdu.ErrorIndex

   Gets error Index.

   .. code-block:: csharp

      public int ErrorIndex { get; set; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Common/Pdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/Pdu.cs#L40>`__

ErrorStatus
~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Common.Definitions.Pdu.ErrorStatus

   Gets error Status.

   .. code-block:: csharp

      public ErrorCode ErrorStatus { get; set; }

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.ErrorCode`

**Source:** `SharpSnmpLib/Common/Pdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/Pdu.cs#L35>`__

HasData
~~~~~~~

.. dn:property:: DotNetSnmp.Common.Definitions.Pdu.HasData

   Gets a value indicating whether variable bindings are present.

   .. code-block:: csharp

      public bool HasData { get; }

   :rtype: ``Boolean``

**Source:** `SharpSnmpLib/Common/Pdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/Pdu.cs#L70>`__

IScope.Pdu
~~~~~~~~~~

.. dn:property:: DotNetSnmp.Common.Definitions.Pdu.DotNetSnmp.Common.Definitions.IScope.Pdu

   Gets the protocol data unit (PDU).

   .. code-block:: csharp

      Pdu IScope.Pdu { get; }

   :returns: An enumeration value indicating the type of PDU (e.g., Get, GetNext, Set, Response).
   :rtype: :dn:cls:`~DotNetSnmp.Common.Definitions.Pdu`

**Source:** `SharpSnmpLib/Common/Pdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/Pdu.cs#L73>`__

PduType
~~~~~~~

.. dn:property:: DotNetSnmp.Common.Definitions.Pdu.PduType

   Gets pdu Type.

   .. code-block:: csharp

      public abstract Asn1Tag PduType { get; }

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/Common/Pdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/Pdu.cs#L25>`__

RequestId
~~~~~~~~~

.. dn:property:: DotNetSnmp.Common.Definitions.Pdu.RequestId

   Gets request Id.

   .. code-block:: csharp

      public int RequestId { get; set; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Common/Pdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/Pdu.cs#L30>`__

TypeCode
~~~~~~~~

.. dn:property:: DotNetSnmp.Common.Definitions.Pdu.TypeCode

   Legacy alias for PDU type code.

   .. code-block:: csharp

      public SnmpType TypeCode { get; }

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`

**Source:** `SharpSnmpLib/Common/Pdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/Pdu.cs#L50>`__

VariableBindings
~~~~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Common.Definitions.Pdu.VariableBindings

   Gets variable Bindings.

   .. code-block:: csharp

      public VarBindList? VariableBindings { get; set; }

   :rtype: :dn:cls:`~DotNetSnmp.Asn1.SyntaxObjects.VarBindList`

**Source:** `SharpSnmpLib/Common/Pdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/Pdu.cs#L45>`__

Variables
~~~~~~~~~

.. dn:property:: DotNetSnmp.Common.Definitions.Pdu.Variables

   Legacy alias for variable bindings.

   .. code-block:: csharp

      public IList<Variable> Variables { get; }

   :rtype: ``IList<Variable>``

**Source:** `SharpSnmpLib/Common/Pdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/Pdu.cs#L65>`__

Methods
-------

CopyTo(Pdu)
~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Common.Definitions.Pdu.CopyTo(DotNetSnmp.Common.Definitions.Pdu)

   Copies the PDU data to another PDU.

   .. code-block:: csharp

      protected void CopyTo(Pdu pdu)

   :param pdu: The PDU to copy to.
   :type pdu: :dn:cls:`~DotNetSnmp.Common.Definitions.Pdu`

**Source:** `SharpSnmpLib/Common/Pdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/Pdu.cs#L116>`__

EnsureNoError()
~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Common.Definitions.Pdu.EnsureNoError

   Throws an exception if the ErrorStatus property for the SNMP response PDU is != 0.

   .. code-block:: csharp

      public void EnsureNoError()

**Source:** `SharpSnmpLib/Common/Pdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/Pdu.cs#L101>`__

IsConfirmed()
~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Common.Definitions.Pdu.IsConfirmed

   Returns true if this PDU might trigger a REPORT message.

   .. code-block:: csharp

      public bool IsConfirmed()

   :rtype: ``Boolean``

**Source:** `SharpSnmpLib/Common/Pdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/Pdu.cs#L79>`__

IsResponse()
~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Common.Definitions.Pdu.IsResponse

   Returns true if this PDU is a response PDU.

   .. code-block:: csharp

      public bool IsResponse()

   :rtype: ``Boolean``

**Source:** `SharpSnmpLib/Common/Pdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/Pdu.cs#L90>`__

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Common.Definitions.Pdu.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public abstract void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/Common/Pdu.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/Pdu.cs#L94>`__

