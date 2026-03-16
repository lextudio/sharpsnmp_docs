WalkMode Enum
=============

.. dn:enum:: Lextm.SharpSnmpLib.Messaging.WalkMode

   Walk mode.

   .. code-block:: csharp

      [DataContract]
      public enum WalkMode

**Namespace:** ``Lextm.SharpSnmpLib.Messaging``

**Source:** `SharpSnmpLib/Messaging/WalkMode.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/WalkMode.cs#L7>`__

Fields
------

Default
~~~~~~~

.. dn:field:: Lextm.SharpSnmpLib.Messaging.WalkMode.Default

   Default mode walk to the end of MIB view.

   .. code-block:: csharp

      Default = 0

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.Messaging.WalkMode`

**Source:** `SharpSnmpLib/Messaging/WalkMode.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/WalkMode.cs#L13>`__

WithinSubtree
~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpLib.Messaging.WalkMode.WithinSubtree

   In this mode, walk within sub-tree.

   .. code-block:: csharp

      WithinSubtree = 1

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.Messaging.WalkMode`

**Source:** `SharpSnmpLib/Messaging/WalkMode.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/WalkMode.cs#L18>`__

