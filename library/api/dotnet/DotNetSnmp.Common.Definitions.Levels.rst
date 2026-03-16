Levels Enum
===========

.. dn:enum:: DotNetSnmp.Common.Definitions.Levels

   Security level.

   .. code-block:: csharp

      [Flags]
      [DataContract]
      public enum Levels : byte

**Namespace:** ``DotNetSnmp.Common.Definitions``

**Source:** `SharpSnmpLib/Common/SecurityLevel.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/SecurityLevel.cs#L7>`__

Fields
------

Authentication
~~~~~~~~~~~~~~

.. dn:field:: DotNetSnmp.Common.Definitions.Levels.Authentication

   Authentication flag.

   .. code-block:: csharp

      Authentication = 1

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.Levels`

**Source:** `SharpSnmpLib/Common/SecurityLevel.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/SecurityLevel.cs#L14>`__

Privacy
~~~~~~~

.. dn:field:: DotNetSnmp.Common.Definitions.Levels.Privacy

   Privacy flag.

   .. code-block:: csharp

      Privacy = 2

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.Levels`

**Source:** `SharpSnmpLib/Common/SecurityLevel.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/SecurityLevel.cs#L19>`__

Reportable
~~~~~~~~~~

.. dn:field:: DotNetSnmp.Common.Definitions.Levels.Reportable

   Reportable flag.

   .. code-block:: csharp

      Reportable = 4

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.Levels`

**Source:** `SharpSnmpLib/Common/SecurityLevel.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/SecurityLevel.cs#L24>`__

