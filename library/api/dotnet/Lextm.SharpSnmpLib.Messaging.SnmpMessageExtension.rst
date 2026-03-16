SnmpMessageExtension Class
==========================

.. dn:class:: Lextm.SharpSnmpLib.Messaging.SnmpMessageExtension

   Backward-compatible entry point for legacy extension APIs.

   .. code-block:: csharp

      [Obsolete("This type is for internal use only and may be removed in a future release.")]
      public static class SnmpMessageExtension

**Namespace:** ``Lextm.SharpSnmpLib.Messaging``

**Inheritance:** Object → ``SnmpMessageExtension``

**Source:** `SharpSnmpLib/Messaging/SnmpMessageExtension.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/SnmpMessageExtension.cs#L5>`__

Properties
----------

IsRunningOnIOS
~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.SnmpMessageExtension.IsRunningOnIOS

   Gets a value indicating whether current runtime is iOS.

   .. code-block:: csharp

      public static bool IsRunningOnIOS { get; }

   :rtype: ``Boolean``

**Source:** `SharpSnmpLib/Messaging/SnmpMessageExtension.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/SnmpMessageExtension.cs#L21>`__

IsRunningOnMac
~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.SnmpMessageExtension.IsRunningOnMac

   Gets a value indicating whether current runtime is macOS.

   .. code-block:: csharp

      public static bool IsRunningOnMac { get; }

   :rtype: ``Boolean``

**Source:** `SharpSnmpLib/Messaging/SnmpMessageExtension.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/SnmpMessageExtension.cs#L16>`__

IsRunningOnWindows
~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.SnmpMessageExtension.IsRunningOnWindows

   Gets a value indicating whether current runtime is Windows.

   .. code-block:: csharp

      public static bool IsRunningOnWindows { get; }

   :rtype: ``Boolean``

**Source:** `SharpSnmpLib/Messaging/SnmpMessageExtension.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/SnmpMessageExtension.cs#L11>`__

Methods
-------

IsRunningOnMono()
~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.SnmpMessageExtension.IsRunningOnMono

   Tests whether current runtime is Mono.

   .. code-block:: csharp

      public static bool IsRunningOnMono()

   :rtype: ``Boolean``

**Source:** `SharpSnmpLib/Messaging/SnmpMessageExtension.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/SnmpMessageExtension.cs#L26>`__

