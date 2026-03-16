GenericCode Enum
================

.. dn:enum:: Lextm.SharpSnmpLib.GenericCode

   Generic trap code.

   .. code-block:: csharp

      [DataContract]
      public enum GenericCode

**Namespace:** ``Lextm.SharpSnmpLib``

**Source:** `SharpSnmpLib/GenericCode.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/GenericCode.cs#L7>`__

Fields
------

AuthenticationFailure
~~~~~~~~~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpLib.GenericCode.AuthenticationFailure

   Indicates that someone has tried to query your agent with an incorrect community string; useful in determining if someone is trying to gain unauthorized access to one of your devices.

   .. code-block:: csharp

      AuthenticationFailure = 4

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.GenericCode`

**Source:** `SharpSnmpLib/GenericCode.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/GenericCode.cs#L29>`__

ColdStart
~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpLib.GenericCode.ColdStart

   Indicates that the agent has rebooted. All management variables will be reset; specifically, Counters and Gauges will be reset to zero (0). One nice thing about the coldStart trap is that it can be used to determine when new hardware is added to the network. When a device is powered on, it sends this trap to its trap destination. If the trap destination is set correctly (i.e., to the IP address of your NMS) the NMS can receive the trap and determine whether it needs to manage the device.

   .. code-block:: csharp

      ColdStart = 0

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.GenericCode`

**Source:** `SharpSnmpLib/GenericCode.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/GenericCode.cs#L13>`__

EgpNeighborLoss
~~~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpLib.GenericCode.EgpNeighborLoss

   Indicates that an Exterior Gateway Protocol (EGP) neighbor has gone down.

   .. code-block:: csharp

      EgpNeighborLoss = 5

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.GenericCode`

**Source:** `SharpSnmpLib/GenericCode.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/GenericCode.cs#L33>`__

EnterpriseSpecific
~~~~~~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpLib.GenericCode.EnterpriseSpecific

   Indicates that the trap is enterprise-specific. SNMP vendors and users define their own traps under the private-enterprise branch of the SMI object tree. To process this trap properly, the NMS has to decode the specific trap number that is part of the SNMP message.

   .. code-block:: csharp

      EnterpriseSpecific = 6

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.GenericCode`

**Source:** `SharpSnmpLib/GenericCode.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/GenericCode.cs#L37>`__

LinkDown
~~~~~~~~

.. dn:field:: Lextm.SharpSnmpLib.GenericCode.LinkDown

   Sent when an interface on a device goes down. The first variable binding identifies which interface went down.

   .. code-block:: csharp

      LinkDown = 2

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.GenericCode`

**Source:** `SharpSnmpLib/GenericCode.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/GenericCode.cs#L21>`__

LinkUp
~~~~~~

.. dn:field:: Lextm.SharpSnmpLib.GenericCode.LinkUp

   Sent when an interface on a device comes back up. The first variable binding identifies which interface came back up.

   .. code-block:: csharp

      LinkUp = 3

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.GenericCode`

**Source:** `SharpSnmpLib/GenericCode.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/GenericCode.cs#L25>`__

WarmStart
~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpLib.GenericCode.WarmStart

   Indicates that the agent has reinitialized itself. None of the management variables will be reset.

   .. code-block:: csharp

      WarmStart = 1

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.GenericCode`

**Source:** `SharpSnmpLib/GenericCode.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/GenericCode.cs#L17>`__

