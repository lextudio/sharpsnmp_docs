ISnmpTransport Interface
========================

.. dn:interface:: DotNetSnmp.Transport.ISnmpTransport

   Defines the contract for ISnmpTransport.

   .. code-block:: csharp

      public interface ISnmpTransport : IDisposable

**Namespace:** ``DotNetSnmp.Transport``

**Source:** `SharpSnmpLib/Transport/ISnmpTransport.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/ISnmpTransport.cs#L7>`__

Methods
-------

ReceiveAsync(IPEndPoint, CancellationToken)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Transport.ISnmpTransport.ReceiveAsync(System.Net.IPEndPoint,System.Threading.CancellationToken)

   Receives async.

   .. code-block:: csharp

      ValueTask<ReadOnlyMemory<byte>> ReceiveAsync(IPEndPoint targetEndPoint, CancellationToken cancellationToken)

   :type targetEndPoint: ``IPEndPoint``
   :type cancellationToken: ``CancellationToken``

   :rtype: ``ValueTask<ReadOnlyMemory<Byte>>``

**Source:** `SharpSnmpLib/Transport/ISnmpTransport.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/ISnmpTransport.cs#L20>`__

SendAsync(ReadOnlyMemory<Byte>, IPEndPoint, CancellationToken)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Transport.ISnmpTransport.SendAsync(System.ReadOnlyMemory{System.Byte},System.Net.IPEndPoint,System.Threading.CancellationToken)

   Sends async.

   .. code-block:: csharp

      ValueTask<int> SendAsync(ReadOnlyMemory<byte> message, IPEndPoint targetEndPoint, CancellationToken cancellationToken = default(CancellationToken))

   :type message: ``ReadOnlyMemory<Byte>``
   :type targetEndPoint: ``IPEndPoint``
   :type cancellationToken: ``CancellationToken``

   :rtype: ``ValueTask<Int32>``

**Source:** `SharpSnmpLib/Transport/ISnmpTransport.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/ISnmpTransport.cs#L12>`__

