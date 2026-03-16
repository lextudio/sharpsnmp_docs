IScope Interface
================

.. dn:interface:: DotNetSnmp.Common.Definitions.IScope

   Defines the contract for IScope.

   .. code-block:: csharp

      public interface IScope : IAsnSerializable

**Namespace:** ``DotNetSnmp.Common.Definitions``

**Source:** `SharpSnmpLib/Common/IScope.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/IScope.cs#L15>`__

Properties
----------

ContextEngineId
~~~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Common.Definitions.IScope.ContextEngineId

   Gets context engine id (legacy compatibility member).

   .. code-block:: csharp

      OctetString ContextEngineId { get; }

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`

**Source:** `SharpSnmpLib/Common/IScope.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/IScope.cs#L68>`__

ContextName
~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Common.Definitions.IScope.ContextName

   Gets context name (legacy compatibility member).

   .. code-block:: csharp

      OctetString ContextName { get; }

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`

**Source:** `SharpSnmpLib/Common/IScope.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/IScope.cs#L74>`__

Pdu
~~~

.. dn:property:: DotNetSnmp.Common.Definitions.IScope.Pdu

   Gets the protocol data unit (PDU).

   .. code-block:: csharp

      Pdu Pdu { get; }

   :returns: An enumeration value indicating the type of PDU (e.g., Get, GetNext, Set, Response).
   :rtype: :dn:cls:`~DotNetSnmp.Common.Definitions.Pdu`

**Source:** `SharpSnmpLib/Common/IScope.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/IScope.cs#L51>`__

RequestId
~~~~~~~~~

.. dn:property:: DotNetSnmp.Common.Definitions.IScope.RequestId

   Gets request Id.

   .. code-block:: csharp

      int RequestId { get; }

   :returns: An integer value that uniquely identifies this SNMP request or response.
   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Common/IScope.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/IScope.cs#L27>`__

VariableBindings
~~~~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Common.Definitions.IScope.VariableBindings

   Gets variable Bindings.

   .. code-block:: csharp

      VarBindList? VariableBindings { get; set; }

   :returns: A collection of OID-value pairs representing the variables being requested, set, or returned in a response.
   :rtype: :dn:cls:`~DotNetSnmp.Asn1.SyntaxObjects.VarBindList`

**Source:** `SharpSnmpLib/Common/IScope.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/IScope.cs#L40>`__

Methods
-------

GetData(VersionCode)
~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Common.Definitions.IScope.GetData(DotNetSnmp.Common.Definitions.VersionCode)

   Gets serialized scope data for a target protocol version (legacy compatibility member).

   .. code-block:: csharp

      IAsnSerializable GetData(VersionCode version)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`

   :rtype: :dn:iface:`~DotNetSnmp.Asn1.Serialization.IAsnSerializable`

**Source:** `SharpSnmpLib/Common/IScope.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/IScope.cs#L80>`__

IsResponse()
~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Common.Definitions.IScope.IsResponse

   Determines whether response.

   .. code-block:: csharp

      bool IsResponse()

   :returns: true if this scope is a response; otherwise, false.
   :rtype: ``Boolean``

**Source:** `SharpSnmpLib/Common/IScope.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/IScope.cs#L63>`__

