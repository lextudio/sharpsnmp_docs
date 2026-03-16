MessageFactory Class
====================

.. dn:class:: Lextm.SharpSnmpLib.Messaging.MessageFactory

   Factory that creates :dn:iface:``~DotNetSnmp.Common.Definitions.ISnmpMessage`` instances from byte format.

   .. code-block:: csharp

      public static class MessageFactory

**Namespace:** ``Lextm.SharpSnmpLib.Messaging``

**Inheritance:** Object → ``MessageFactory``

**Source:** `SharpSnmpLib/Messaging/MessageFactory.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/MessageFactory.cs#L12>`__

Methods
-------

ParseMessages(Byte[], Int32, Int32, UserRegistry, Boolean)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.MessageFactory.ParseMessages(System.Byte[],System.Int32,System.Int32,Lextm.SharpSnmpLib.Security.UserRegistry,System.Boolean)

   Parses one or more SNMP messages from a segment of a byte array.

   .. code-block:: csharp

      public static IList<ISnmpMessage> ParseMessages(byte[] buffer, int index, int length, UserRegistry registry, bool throwOnV3SecurityError)

   :type buffer: ``Byte[]``
   :type index: ``Int32``
   :type length: ``Int32``
   :type registry: :dn:cls:`~Lextm.SharpSnmpLib.Security.UserRegistry`
   :type throwOnV3SecurityError: ``Boolean``

   :rtype: ``IList<ISnmpMessage>``

**Source:** `SharpSnmpLib/Messaging/MessageFactory.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/MessageFactory.cs#L77>`__

ParseMessages(Byte[], Int32, Int32, UserRegistry)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.MessageFactory.ParseMessages(System.Byte[],System.Int32,System.Int32,Lextm.SharpSnmpLib.Security.UserRegistry)

   Parses one or more SNMP messages from a segment of a byte array.

   .. code-block:: csharp

      public static IList<ISnmpMessage> ParseMessages(byte[] buffer, int index, int length, UserRegistry registry)

   :type buffer: ``Byte[]``
   :type index: ``Int32``
   :type length: ``Int32``
   :type registry: :dn:cls:`~Lextm.SharpSnmpLib.Security.UserRegistry`

   :rtype: ``IList<ISnmpMessage>``

**Source:** `SharpSnmpLib/Messaging/MessageFactory.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/MessageFactory.cs#L69>`__

ParseMessages(Byte[], UserRegistry)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.MessageFactory.ParseMessages(System.Byte[],Lextm.SharpSnmpLib.Security.UserRegistry)

   Parses one or more SNMP messages from a byte array.

   .. code-block:: csharp

      public static IList<ISnmpMessage> ParseMessages(byte[] buffer, UserRegistry registry)

   :type buffer: ``Byte[]``
   :type registry: :dn:cls:`~Lextm.SharpSnmpLib.Security.UserRegistry`

   :rtype: ``IList<ISnmpMessage>``

**Source:** `SharpSnmpLib/Messaging/MessageFactory.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/MessageFactory.cs#L56>`__

ParseMessages(IEnumerable<Char>, UserRegistry)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.MessageFactory.ParseMessages(System.Collections.Generic.IEnumerable{System.Char},Lextm.SharpSnmpLib.Security.UserRegistry)

   Parses one or more SNMP messages from hexadecimal text.

   .. code-block:: csharp

      public static IList<ISnmpMessage> ParseMessages(IEnumerable<char> bytes, UserRegistry registry)

   :type bytes: ``IEnumerable<Char>``
   :type registry: :dn:cls:`~Lextm.SharpSnmpLib.Security.UserRegistry`

   :rtype: ``IList<ISnmpMessage>``

**Source:** `SharpSnmpLib/Messaging/MessageFactory.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/MessageFactory.cs#L42>`__

ParseMessages(ReadOnlyMemory<Byte>, UserRegistry, Boolean)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.MessageFactory.ParseMessages(System.ReadOnlyMemory{System.Byte},Lextm.SharpSnmpLib.Security.UserRegistry,System.Boolean)

   Parses one or more SNMP messages from BER-encoded bytes.

   .. code-block:: csharp

      public static IList<ISnmpMessage> ParseMessages(ReadOnlyMemory<byte> bytes, UserRegistry registry, bool throwOnV3SecurityError)

   :param bytes: Byte string.
   :type bytes: ``ReadOnlyMemory<Byte>``
   :param registry: The registry.
   :type registry: :dn:cls:`~Lextm.SharpSnmpLib.Security.UserRegistry`
   :param throwOnV3SecurityError: If true, throws on v3 security failures (manager/client behavior). If false, keeps parsing and records failures for agent-side report generation.
   :type throwOnV3SecurityError: ``Boolean``

   :rtype: ``IList<ISnmpMessage>``

**Source:** `SharpSnmpLib/Messaging/MessageFactory.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/MessageFactory.cs#L118>`__

ParseMessages(ReadOnlyMemory<Byte>, UserRegistry)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.MessageFactory.ParseMessages(System.ReadOnlyMemory{System.Byte},Lextm.SharpSnmpLib.Security.UserRegistry)

   Parses one or more SNMP messages from BER-encoded bytes.

   .. code-block:: csharp

      public static IList<ISnmpMessage> ParseMessages(ReadOnlyMemory<byte> bytes, UserRegistry registry)

   :param bytes: Byte string.
   :type bytes: ``ReadOnlyMemory<Byte>``
   :param registry: The registry.
   :type registry: :dn:cls:`~Lextm.SharpSnmpLib.Security.UserRegistry`

   :rtype: ``IList<ISnmpMessage>``

**Source:** `SharpSnmpLib/Messaging/MessageFactory.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/MessageFactory.cs#L103>`__

