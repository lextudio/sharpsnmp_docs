MsgFlag Enum
============

.. dn:enum:: DotNetSnmp.Protocol.V3.Security.MsgFlag

   Defines the message flags for SNMPv3 message processing (RFC 3414).

   .. code-block:: csharp

      [Flags]
      public enum MsgFlag : byte

**Namespace:** ``DotNetSnmp.Protocol.V3.Security``

**Source:** `SharpSnmpLib/V3/Security/MsgFlags.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/MsgFlags.cs#L25>`__

Fields
------

Auth
~~~~

.. dn:field:: DotNetSnmp.Protocol.V3.Security.MsgFlag.Auth

   Authentication enabled (bit 0 of msgFlags, value 0x01).

   .. code-block:: csharp

      Auth = 1

   :rtype: :dn:enum:`~DotNetSnmp.Protocol.V3.Security.MsgFlag`

**Source:** `SharpSnmpLib/V3/Security/MsgFlags.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/MsgFlags.cs#L45>`__

NoAuthNoPriv
~~~~~~~~~~~~

.. dn:field:: DotNetSnmp.Protocol.V3.Security.MsgFlag.NoAuthNoPriv

   No authentication and no privacy encryption (security level: noAuthNoPriv).

   .. code-block:: csharp

      NoAuthNoPriv = 0

   :rtype: :dn:enum:`~DotNetSnmp.Protocol.V3.Security.MsgFlag`

**Source:** `SharpSnmpLib/V3/Security/MsgFlags.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/MsgFlags.cs#L35>`__

Priv
~~~~

.. dn:field:: DotNetSnmp.Protocol.V3.Security.MsgFlag.Priv

   Privacy (encryption) enabled (bit 1 of msgFlags, value 0x02).

   .. code-block:: csharp

      Priv = 2

   :rtype: :dn:enum:`~DotNetSnmp.Protocol.V3.Security.MsgFlag`

**Source:** `SharpSnmpLib/V3/Security/MsgFlags.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/MsgFlags.cs#L55>`__

Reportable
~~~~~~~~~~

.. dn:field:: DotNetSnmp.Protocol.V3.Security.MsgFlag.Reportable

   Reportable message (bit 2 of msgFlags, value 0x04).

   .. code-block:: csharp

      Reportable = 4

   :rtype: :dn:enum:`~DotNetSnmp.Protocol.V3.Security.MsgFlag`

**Source:** `SharpSnmpLib/V3/Security/MsgFlags.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/Security/MsgFlags.cs#L65>`__

