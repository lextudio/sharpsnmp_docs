SnmpDatagram Struct
===================

.. dn:struct:: Lextm.SharpSnmpLib.Transport.SnmpDatagram

   Represents a received UDP datagram with a pooled buffer and the sender&apos;s address.

   .. code-block:: csharp

      public readonly struct SnmpDatagram

**Namespace:** ``Lextm.SharpSnmpLib.Transport``

**Source:** `SharpSnmpLib/Transport/SnmpDatagram.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/SnmpDatagram.cs#L41>`__

Constructors
------------

SnmpDatagram(Byte[], Int32, SocketAddress)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Transport.SnmpDatagram..ctor(System.Byte[],System.Int32,System.Net.SocketAddress)

   Initializes a new instance of :dn:struct:``~Lextm.SharpSnmpLib.Transport.SnmpDatagram``.

   .. code-block:: csharp

      public SnmpDatagram(byte[] buffer, int length, SocketAddress senderAddress)

   :param buffer: A buffer rented from ``Shared``. The caller transfers ownership to the consumer.
   :type buffer: ``Byte[]``
   :param length: Number of valid bytes in buffer.
   :type length: ``Int32``
   :param senderAddress: A copy of the sender&apos;s ``SocketAddress``.
   :type senderAddress: ``SocketAddress``

**Source:** `SharpSnmpLib/Transport/SnmpDatagram.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/SnmpDatagram.cs#L54>`__

Properties
----------

Buffer
~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Transport.SnmpDatagram.Buffer

   Gets the rented buffer containing the datagram payload. Only the first :dn:prop:``~Lextm.SharpSnmpLib.Transport.SnmpDatagram.Length`` bytes are valid.

   .. code-block:: csharp

      public byte[] Buffer { get; }

   :rtype: ``Byte[]``

**Source:** `SharpSnmpLib/Transport/SnmpDatagram.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/SnmpDatagram.cs#L65>`__

Length
~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Transport.SnmpDatagram.Length

   Gets the number of valid bytes in :dn:prop:``~Lextm.SharpSnmpLib.Transport.SnmpDatagram.Buffer``.

   .. code-block:: csharp

      public int Length { get; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Transport/SnmpDatagram.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/SnmpDatagram.cs#L70>`__

SenderAddress
~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Transport.SnmpDatagram.SenderAddress

   Gets the sender&apos;s socket address (a snapshot, safe to use after the receive loop overwrites its working copy).

   .. code-block:: csharp

      public SocketAddress SenderAddress { get; }

   :rtype: ``SocketAddress``

**Source:** `SharpSnmpLib/Transport/SnmpDatagram.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/SnmpDatagram.cs#L76>`__

Methods
-------

GetSenderEndPoint()
~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Transport.SnmpDatagram.GetSenderEndPoint

   Creates an ``IPEndPoint`` from :dn:prop:``~Lextm.SharpSnmpLib.Transport.SnmpDatagram.SenderAddress``. This allocates; prefer using :dn:prop:``~Lextm.SharpSnmpLib.Transport.SnmpDatagram.SenderAddress`` directly on the hot path.

   .. code-block:: csharp

      public readonly IPEndPoint GetSenderEndPoint()

   :rtype: ``IPEndPoint``

**Source:** `SharpSnmpLib/Transport/SnmpDatagram.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/SnmpDatagram.cs#L82>`__

ReturnBuffer()
~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Transport.SnmpDatagram.ReturnBuffer

   Returns :dn:prop:``~Lextm.SharpSnmpLib.Transport.SnmpDatagram.Buffer`` to ``Shared``. Call this exactly once after the datagram has been fully processed.

   .. code-block:: csharp

      public readonly void ReturnBuffer()

**Source:** `SharpSnmpLib/Transport/SnmpDatagram.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/SnmpDatagram.cs#L94>`__

