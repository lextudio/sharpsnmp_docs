ITransportListener Interface
============================

.. dn:interface:: Lextm.SharpSnmpLib.Transport.ITransportListener

   Defines the contract for an SNMP transport listener that produces received messages from any transport (UDP, TCP, etc.).

   .. code-block:: csharp

      public interface ITransportListener : IAsyncDisposable

**Namespace:** ``Lextm.SharpSnmpLib.Transport``

**Source:** `SharpSnmpLib/Transport/ITransportListener.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/ITransportListener.cs#L42>`__

Properties
----------

DatagramReader
~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Transport.ITransportListener.DatagramReader

   Gets the channel reader that produces received datagrams.

   .. code-block:: csharp

      ChannelReader<SnmpDatagram> DatagramReader { get; }

   :rtype: ``ChannelReader<SnmpDatagram>``

**Source:** `SharpSnmpLib/Transport/ITransportListener.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/ITransportListener.cs#L53>`__

LocalEndPoint
~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Transport.ITransportListener.LocalEndPoint

   Gets the local endpoint this listener is bound to.

   .. code-block:: csharp

      EndPoint LocalEndPoint { get; }

   :rtype: ``EndPoint``

**Source:** `SharpSnmpLib/Transport/ITransportListener.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/ITransportListener.cs#L70>`__

Methods
-------

SendResponseAsync(ReadOnlyMemory<Byte>, SocketAddress, CancellationToken)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Transport.ITransportListener.SendResponseAsync(System.ReadOnlyMemory{System.Byte},System.Net.SocketAddress,System.Threading.CancellationToken)

   Sends a response message back to the specified address.

   .. code-block:: csharp

      ValueTask SendResponseAsync(ReadOnlyMemory<byte> response, SocketAddress receiver, CancellationToken cancellationToken = default(CancellationToken))

   :param response: The encoded SNMP response bytes.
   :type response: ``ReadOnlyMemory<Byte>``
   :param receiver: The destination socket address.
   :type receiver: ``SocketAddress``
   :param cancellationToken: Cancellation token.
   :type cancellationToken: ``CancellationToken``

   :returns: A ``ValueTask`` that completes when the send finishes.
   :rtype: ``ValueTask``

**Source:** `SharpSnmpLib/Transport/ITransportListener.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/ITransportListener.cs#L62>`__

StartAsync(CancellationToken)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Transport.ITransportListener.StartAsync(System.Threading.CancellationToken)

   Starts the listener. After this call returns, the listener is actively receiving messages and writing them to :dn:prop:``~Lextm.SharpSnmpLib.Transport.ITransportListener.DatagramReader``.

   .. code-block:: csharp

      Task StartAsync(CancellationToken cancellationToken = default(CancellationToken))

   :param cancellationToken: Cancellation token.
   :type cancellationToken: ``CancellationToken``

   :rtype: ``Task``

**Source:** `SharpSnmpLib/Transport/ITransportListener.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/ITransportListener.cs#L77>`__

StopAsync(CancellationToken)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Transport.ITransportListener.StopAsync(System.Threading.CancellationToken)

   Stops the listener gracefully, completing the datagram channel and draining in-flight operations.

   .. code-block:: csharp

      Task StopAsync(CancellationToken cancellationToken = default(CancellationToken))

   :param cancellationToken: Cancellation token.
   :type cancellationToken: ``CancellationToken``

   :rtype: ``Task``

**Source:** `SharpSnmpLib/Transport/ITransportListener.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/ITransportListener.cs#L84>`__

