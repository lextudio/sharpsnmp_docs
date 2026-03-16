SecureAgentParameters Class
===========================

.. dn:class:: DotNetSnmp.Protocol.V3.Security.SecureAgentParameters

   Represents the SecureAgentParameters type.

   .. code-block:: csharp

      public class SecureAgentParameters

**Namespace:** ``DotNetSnmp.Protocol.V3.Security``

**Inheritance:** Object → ``SecureAgentParameters``

**Source:** `SharpSnmpLib/V3/Security/SecureAgentParameters.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/SecureAgentParameters.cs#L8>`__

Properties
----------

HashAlgorithm
~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Security.SecureAgentParameters.HashAlgorithm

   Gets hash Algorithm.

   .. code-block:: csharp

      public HashAlgorithmName? HashAlgorithm { get; set; }

   :rtype: ``Nullable<HashAlgorithmName>``

**Source:** `SharpSnmpLib/V3/Security/SecureAgentParameters.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/SecureAgentParameters.cs#L15>`__

SecurityName
~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Security.SecureAgentParameters.SecurityName

   Represents this member.

   .. code-block:: csharp

      public string? SecurityName { get; set; }

   :rtype: ``String``

**Source:** `SharpSnmpLib/V3/Security/SecureAgentParameters.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/SecureAgentParameters.cs#L20>`__

UserPassphrase
~~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Security.SecureAgentParameters.UserPassphrase

   Represents this member.

   .. code-block:: csharp

      public string UserPassphrase { get; set; }

   :rtype: ``String``

**Source:** `SharpSnmpLib/V3/Security/SecureAgentParameters.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/SecureAgentParameters.cs#L25>`__

UserPassphraseBytes
~~~~~~~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.Security.SecureAgentParameters.UserPassphraseBytes

   Stores user Passphrase Bytes.

   .. code-block:: csharp

      public ReadOnlyMemory<byte> UserPassphraseBytes { get; }

   :rtype: ``ReadOnlyMemory<Byte>``

**Source:** `SharpSnmpLib/V3/Security/SecureAgentParameters.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/SecureAgentParameters.cs#L37>`__

