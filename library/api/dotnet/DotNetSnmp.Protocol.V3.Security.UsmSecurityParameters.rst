UsmSecurityParameters Class
===========================

.. dn:class:: DotNetSnmp.Protocol.V3.Security.UsmSecurityParameters

   Represents the UsmSecurityParameters type.

   .. code-block:: csharp

      public class UsmSecurityParameters : IAsnSerializable

**Namespace:** ``DotNetSnmp.Protocol.V3.Security``

**Inheritance:** Object → ``UsmSecurityParameters``

**Source:** `SharpSnmpLib/V3/Security/UsmSecurityParameters.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/UsmSecurityParameters.cs#L9>`__

Properties
----------

AuthParams
~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Security.UsmSecurityParameters.AuthParams

   Gets auth Params.

   .. code-block:: csharp

      public Memory<byte> AuthParams { get; set; }

   :rtype: ``Memory<Byte>``

**Source:** `SharpSnmpLib/V3/Security/UsmSecurityParameters.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/UsmSecurityParameters.cs#L37>`__

EngineBoots
~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Security.UsmSecurityParameters.EngineBoots

   count of the number of times the SNMP engine has re-booted/re-initialized since snmpEngineID was last configured

   .. code-block:: csharp

      public int EngineBoots { get; set; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/V3/Security/UsmSecurityParameters.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/UsmSecurityParameters.cs#L21>`__

EngineId
~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Security.UsmSecurityParameters.EngineId

   Gets engine Id.

   .. code-block:: csharp

      public Memory<byte> EngineId { get; set; }

   :rtype: ``Memory<Byte>``

**Source:** `SharpSnmpLib/V3/Security/UsmSecurityParameters.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/UsmSecurityParameters.cs#L14>`__

EngineTime
~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Security.UsmSecurityParameters.EngineTime

   the number of seconds since the snmpEngineBoots counter was last incremented

   .. code-block:: csharp

      public int EngineTime { get; set; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/V3/Security/UsmSecurityParameters.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/UsmSecurityParameters.cs#L27>`__

PrivParams
~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Security.UsmSecurityParameters.PrivParams

   Gets priv Params.

   .. code-block:: csharp

      public Memory<byte> PrivParams { get; set; }

   :rtype: ``Memory<Byte>``

**Source:** `SharpSnmpLib/V3/Security/UsmSecurityParameters.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/UsmSecurityParameters.cs#L42>`__

SecurityName
~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Security.UsmSecurityParameters.SecurityName

   Gets security Name.

   .. code-block:: csharp

      public OctetString SecurityName { get; set; }

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`

**Source:** `SharpSnmpLib/V3/Security/UsmSecurityParameters.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/UsmSecurityParameters.cs#L32>`__

Methods
-------

ReadFrom(AsnReader)
~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Security.UsmSecurityParameters.ReadFrom(System.Formats.Asn1.AsnReader)

   Reads a value from an ASN.1 reader.

   .. code-block:: csharp

      public static UsmSecurityParameters ReadFrom(AsnReader reader)

   :type reader: ``AsnReader``

   :rtype: :dn:cls:`~DotNetSnmp.Protocol.V3.Security.UsmSecurityParameters`

**Source:** `SharpSnmpLib/V3/Security/UsmSecurityParameters.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/UsmSecurityParameters.cs#L74>`__

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.Security.UsmSecurityParameters.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/V3/Security/UsmSecurityParameters.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/UsmSecurityParameters.cs#L45>`__

