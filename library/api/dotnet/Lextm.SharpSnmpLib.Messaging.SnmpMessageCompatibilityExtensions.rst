SnmpMessageCompatibilityExtensions Class
========================================

.. dn:class:: Lextm.SharpSnmpLib.Messaging.SnmpMessageCompatibilityExtensions

   Provides helper methods for SnmpMessageCompatibilityExtensions.

   .. code-block:: csharp

      public static class SnmpMessageCompatibilityExtensions

**Namespace:** ``Lextm.SharpSnmpLib.Messaging``

**Inheritance:** Object → ``SnmpMessageCompatibilityExtensions``

**Source:** `SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs#L148>`__

Methods
-------

GetResponse(ISnmpMessage, Int32, IPEndPoint, Socket)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.SnmpMessageCompatibilityExtensions.GetResponse(DotNetSnmp.Common.Definitions.ISnmpMessage,System.Int32,System.Net.IPEndPoint,System.Net.Sockets.Socket)

   Sends an SNMP request and handles the response using a provided socket.

   .. code-block:: csharp

      public static ISnmpMessage GetResponse(this ISnmpMessage request, int timeout, IPEndPoint receiver, Socket udpSocket)

   :type timeout: ``Int32``
   :type receiver: ``IPEndPoint``
   :type udpSocket: ``Socket``

   :rtype: :dn:iface:`~DotNetSnmp.Common.Definitions.ISnmpMessage`

**Source:** `SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs#L285>`__

GetResponse(ISnmpMessage, Int32, IPEndPoint, UserRegistry, Socket)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.SnmpMessageCompatibilityExtensions.GetResponse(DotNetSnmp.Common.Definitions.ISnmpMessage,System.Int32,System.Net.IPEndPoint,Lextm.SharpSnmpLib.Security.UserRegistry,System.Net.Sockets.Socket)

   Sends an SNMP request and handles the response using a provided socket and user registry.

   .. code-block:: csharp

      public static ISnmpMessage GetResponse(this ISnmpMessage request, int timeout, IPEndPoint receiver, UserRegistry registry, Socket udpSocket)

   :type timeout: ``Int32``
   :type receiver: ``IPEndPoint``
   :type registry: :dn:cls:`~Lextm.SharpSnmpLib.Security.UserRegistry`
   :type udpSocket: ``Socket``

   :rtype: :dn:iface:`~DotNetSnmp.Common.Definitions.ISnmpMessage`

**Source:** `SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs#L317>`__

GetResponse(ISnmpMessage, Int32, IPEndPoint)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.SnmpMessageCompatibilityExtensions.GetResponse(DotNetSnmp.Common.Definitions.ISnmpMessage,System.Int32,System.Net.IPEndPoint)

   Gets the response message.

   .. code-block:: csharp

      public static ISnmpMessage GetResponse(this ISnmpMessage request, int timeout, IPEndPoint receiver)

   :type timeout: ``Int32``
   :type receiver: ``IPEndPoint``

   :rtype: :dn:iface:`~DotNetSnmp.Common.Definitions.ISnmpMessage`

**Source:** `SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs#L247>`__

GetResponseAsync(ISnmpMessage, IPEndPoint, Socket, CancellationToken)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.SnmpMessageCompatibilityExtensions.GetResponseAsync(DotNetSnmp.Common.Definitions.ISnmpMessage,System.Net.IPEndPoint,System.Net.Sockets.Socket,System.Threading.CancellationToken)

   Sends an SNMP request and handles the response asynchronously using a provided socket.

   .. code-block:: csharp

      public static Task<ISnmpMessage> GetResponseAsync(this ISnmpMessage request, IPEndPoint receiver, Socket udpSocket, CancellationToken cancellationToken)

   :type receiver: ``IPEndPoint``
   :type udpSocket: ``Socket``
   :type cancellationToken: ``CancellationToken``

   :rtype: ``Task<ISnmpMessage>``

**Source:** `SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs#L397>`__

GetResponseAsync(ISnmpMessage, IPEndPoint, Socket)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.SnmpMessageCompatibilityExtensions.GetResponseAsync(DotNetSnmp.Common.Definitions.ISnmpMessage,System.Net.IPEndPoint,System.Net.Sockets.Socket)

   Sends an SNMP request and handles the response asynchronously using a provided socket.

   .. code-block:: csharp

      public static Task<ISnmpMessage> GetResponseAsync(this ISnmpMessage request, IPEndPoint receiver, Socket udpSocket)

   :type receiver: ``IPEndPoint``
   :type udpSocket: ``Socket``

   :rtype: ``Task<ISnmpMessage>``

**Source:** `SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs#L365>`__

GetResponseAsync(ISnmpMessage, IPEndPoint, UserRegistry, Socket, CancellationToken)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.SnmpMessageCompatibilityExtensions.GetResponseAsync(DotNetSnmp.Common.Definitions.ISnmpMessage,System.Net.IPEndPoint,Lextm.SharpSnmpLib.Security.UserRegistry,System.Net.Sockets.Socket,System.Threading.CancellationToken)

   Sends an SNMP request and handles the response asynchronously using a provided socket and user registry.

   .. code-block:: csharp

      public static Task<ISnmpMessage> GetResponseAsync(this ISnmpMessage request, IPEndPoint receiver, UserRegistry registry, Socket udpSocket, CancellationToken cancellationToken)

   :type receiver: ``IPEndPoint``
   :type registry: :dn:cls:`~Lextm.SharpSnmpLib.Security.UserRegistry`
   :type udpSocket: ``Socket``
   :type cancellationToken: ``CancellationToken``

   :rtype: ``Task<ISnmpMessage>``

**Source:** `SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs#L481>`__

GetResponseAsync(ISnmpMessage, IPEndPoint, UserRegistry, Socket)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.SnmpMessageCompatibilityExtensions.GetResponseAsync(DotNetSnmp.Common.Definitions.ISnmpMessage,System.Net.IPEndPoint,Lextm.SharpSnmpLib.Security.UserRegistry,System.Net.Sockets.Socket)

   Sends an SNMP request and handles the response asynchronously using a provided socket and user registry.

   .. code-block:: csharp

      public static Task<ISnmpMessage> GetResponseAsync(this ISnmpMessage request, IPEndPoint receiver, UserRegistry registry, Socket udpSocket)

   :type receiver: ``IPEndPoint``
   :type registry: :dn:cls:`~Lextm.SharpSnmpLib.Security.UserRegistry`
   :type udpSocket: ``Socket``

   :rtype: ``Task<ISnmpMessage>``

**Source:** `SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs#L406>`__

MessageId(ISnmpMessage)
~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.SnmpMessageCompatibilityExtensions.MessageId(DotNetSnmp.Common.Definitions.ISnmpMessage)

   Gets message id.

   .. code-block:: csharp

      public static int MessageId(this ISnmpMessage message)

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs#L195>`__

Pdu(ISnmpMessage)
~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.SnmpMessageCompatibilityExtensions.Pdu(DotNetSnmp.Common.Definitions.ISnmpMessage)

   Returns the message PDU wrapped in the legacy compatibility facade.

   .. code-block:: csharp

      public static LegacyPdu Pdu(this ISnmpMessage message)

   :rtype: :dn:cls:`~Lextm.SharpSnmpLib.Messaging.LegacyPdu`

**Source:** `SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs#L228>`__

RequestId(ISnmpMessage)
~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.SnmpMessageCompatibilityExtensions.RequestId(DotNetSnmp.Common.Definitions.ISnmpMessage)

   Gets request id.

   .. code-block:: csharp

      public static int RequestId(this ISnmpMessage message)

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs#L182>`__

ToBytes(ISnmpMessage)
~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.SnmpMessageCompatibilityExtensions.ToBytes(DotNetSnmp.Common.Definitions.ISnmpMessage)

   Serializes the message to a byte array.

   .. code-block:: csharp

      public static byte[] ToBytes(this ISnmpMessage message)

   :rtype: ``Byte[]``

**Source:** `SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs#L210>`__

TypeCode(ISnmpMessage)
~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.SnmpMessageCompatibilityExtensions.TypeCode(DotNetSnmp.Common.Definitions.ISnmpMessage)

   Gets message PDU type.

   .. code-block:: csharp

      public static SnmpType TypeCode(this ISnmpMessage message)

   :rtype: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`

**Source:** `SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs#L153>`__

Variables(ISnmpMessage)
~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.SnmpMessageCompatibilityExtensions.Variables(DotNetSnmp.Common.Definitions.ISnmpMessage)

   Gets message variable bindings.

   .. code-block:: csharp

      public static IList<Variable> Variables(this ISnmpMessage message)

   :rtype: ``IList<Variable>``

**Source:** `SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/SnmpMessageCompatibilityExtensions.cs#L167>`__

