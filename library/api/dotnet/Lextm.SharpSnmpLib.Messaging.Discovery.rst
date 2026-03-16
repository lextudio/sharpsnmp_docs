Discovery Class
===============

.. dn:class:: Lextm.SharpSnmpLib.Messaging.Discovery

   Discovery class that participates in SNMP v3 discovery process.

   .. code-block:: csharp

      public sealed class Discovery

**Namespace:** ``Lextm.SharpSnmpLib.Messaging``

**Inheritance:** Object → ``Discovery``

**Source:** `SharpSnmpLib/Messaging/Discovery.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Discovery.cs#L18>`__

Constructors
------------

Discovery(Int32, Int32, Int32, SnmpType, OctetString)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Messaging.Discovery..ctor(System.Int32,System.Int32,System.Int32,Lextm.SharpSnmpLib.SnmpType,DotNetSnmp.Asn1.SyntaxObjects.OctetString)

   Initializes a new instance of Discovery.

   .. code-block:: csharp

      public Discovery(int messageId, int requestId, int maxMessageSize, SnmpType type, OctetString contextName)

   :param messageId: The message id.
   :type messageId: ``Int32``
   :param requestId: The request id.
   :type requestId: ``Int32``
   :param maxMessageSize: The max size of message.
   :type maxMessageSize: ``Int32``
   :param type: Message type.
   :type type: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`
   :param contextName: Scoped context name for v3 discovery.
   :type contextName: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`

**Source:** `SharpSnmpLib/Messaging/Discovery.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Discovery.cs#L57>`__

Discovery(Int32, Int32, Int32, SnmpType, String)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Messaging.Discovery..ctor(System.Int32,System.Int32,System.Int32,Lextm.SharpSnmpLib.SnmpType,System.String)

   Initializes a new instance of Discovery.

   .. code-block:: csharp

      public Discovery(int messageId, int requestId, int maxMessageSize, SnmpType type, string contextName)

   :param messageId: The message id.
   :type messageId: ``Int32``
   :param requestId: The request id.
   :type requestId: ``Int32``
   :param maxMessageSize: The max size of message.
   :type maxMessageSize: ``Int32``
   :param type: Message type.
   :type type: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`
   :param contextName: Scoped context name for v3 discovery.
   :type contextName: ``String``

**Source:** `SharpSnmpLib/Messaging/Discovery.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Discovery.cs#L70>`__

Discovery(Int32, Int32, Int32, SnmpType)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Messaging.Discovery..ctor(System.Int32,System.Int32,System.Int32,Lextm.SharpSnmpLib.SnmpType)

   Initializes a new instance of Discovery.

   .. code-block:: csharp

      public Discovery(int messageId, int requestId, int maxMessageSize, SnmpType type)

   :param messageId: The message id.
   :type messageId: ``Int32``
   :param requestId: The request id.
   :type requestId: ``Int32``
   :param maxMessageSize: The max size of message.
   :type maxMessageSize: ``Int32``
   :param type: Message type.
   :type type: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`

**Source:** `SharpSnmpLib/Messaging/Discovery.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Discovery.cs#L44>`__

Discovery(Int32, Int32, Int32)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Messaging.Discovery..ctor(System.Int32,System.Int32,System.Int32)

   Initializes a new instance of Discovery.

   .. code-block:: csharp

      public Discovery(int messageId, int requestId, int maxMessageSize)

   :param messageId: The message id.
   :type messageId: ``Int32``
   :param requestId: The request id.
   :type requestId: ``Int32``
   :param maxMessageSize: The max size of message.
   :type maxMessageSize: ``Int32``

**Source:** `SharpSnmpLib/Messaging/Discovery.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Discovery.cs#L32>`__

Methods
-------

GetResponse(Int32, IPEndPoint, ISnmpTransport)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Discovery.GetResponse(System.Int32,System.Net.IPEndPoint,DotNetSnmp.Transport.ISnmpTransport)

   Gets the response message using the specified transport.

   .. code-block:: csharp

      public ReportMessage GetResponse(int timeout, IPEndPoint receiver, ISnmpTransport transport)

   :param timeout: The timeout value in milliseconds. 0 and -1 indicate infinite timeout.
   :type timeout: ``Int32``
   :param receiver: The receiver endpoint.
   :type receiver: ``IPEndPoint``
   :param transport: The transport to use for send/receive.
   :type transport: :dn:iface:`~DotNetSnmp.Transport.ISnmpTransport`

   :returns: A parsed report message.
   :rtype: :dn:cls:`~Lextm.SharpSnmpLib.Messaging.ReportMessage`

**Source:** `SharpSnmpLib/Messaging/Discovery.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Discovery.cs#L110>`__

GetResponse(Int32, IPEndPoint)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Discovery.GetResponse(System.Int32,System.Net.IPEndPoint)

   Gets the response message.

   .. code-block:: csharp

      public ReportMessage GetResponse(int timeout, IPEndPoint receiver)

   :param timeout: The timeout value in milliseconds. 0 and -1 indicate infinite timeout.
   :type timeout: ``Int32``
   :param receiver: The receiver endpoint.
   :type receiver: ``IPEndPoint``

   :returns: A parsed report message.
   :rtype: :dn:cls:`~Lextm.SharpSnmpLib.Messaging.ReportMessage`

**Source:** `SharpSnmpLib/Messaging/Discovery.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Discovery.cs#L95>`__

GetResponseAsync(IPEndPoint, ISnmpTransport)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Discovery.GetResponseAsync(System.Net.IPEndPoint,DotNetSnmp.Transport.ISnmpTransport)

   Gets response Async using the specified transport.

   .. code-block:: csharp

      public Task<ReportMessage> GetResponseAsync(IPEndPoint receiver, ISnmpTransport transport)

   :param receiver: The receiver endpoint.
   :type receiver: ``IPEndPoint``
   :param transport: The transport to use for send/receive.
   :type transport: :dn:iface:`~DotNetSnmp.Transport.ISnmpTransport`

   :returns: A parsed report message.
   :rtype: ``Task<ReportMessage>``

**Source:** `SharpSnmpLib/Messaging/Discovery.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Discovery.cs#L157>`__

GetResponseAsync(IPEndPoint)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Discovery.GetResponseAsync(System.Net.IPEndPoint)

   Gets response Async.

   .. code-block:: csharp

      public Task<ReportMessage> GetResponseAsync(IPEndPoint receiver)

   :param receiver: The receiver endpoint.
   :type receiver: ``IPEndPoint``

   :returns: A parsed report message.
   :rtype: ``Task<ReportMessage>``

**Source:** `SharpSnmpLib/Messaging/Discovery.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Discovery.cs#L145>`__

ToBytes()
~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Discovery.ToBytes

   Serializes the message to a byte array.

   .. code-block:: csharp

      public byte[] ToBytes()

   :returns: Encoded bytes.
   :rtype: ``Byte[]``

**Source:** `SharpSnmpLib/Messaging/Discovery.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Discovery.cs#L183>`__

ToString()
~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Discovery.ToString

   .. code-block:: csharp

      public override string ToString()

   :rtype: ``String``

**Source:** `SharpSnmpLib/Messaging/Discovery.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Discovery.cs#L189>`__

