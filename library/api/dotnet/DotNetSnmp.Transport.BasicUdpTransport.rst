BasicUdpTransport Class
=======================

.. dn:class:: DotNetSnmp.Transport.BasicUdpTransport

   Represents the BasicUdpTransport type.

   .. code-block:: csharp

      public class BasicUdpTransport : ISnmpTransport, IDisposable

**Namespace:** ``DotNetSnmp.Transport``

**Inheritance:** Object → ``BasicUdpTransport``

**Source:** `SharpSnmpLib/Transport/BasicUdpTransport.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/BasicUdpTransport.cs#L8>`__

Constructors
------------

BasicUdpTransport(IPEndPoint, IPEndPoint)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Transport.BasicUdpTransport..ctor(System.Net.IPEndPoint,System.Net.IPEndPoint)

   Initializes a new instance of BasicUdpTransport.

   .. code-block:: csharp

      public BasicUdpTransport(IPEndPoint localEndPoint, IPEndPoint targetEndPoint)

   :type localEndPoint: ``IPEndPoint``
   :type targetEndPoint: ``IPEndPoint``

**Source:** `SharpSnmpLib/Transport/BasicUdpTransport.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/BasicUdpTransport.cs#L32>`__

BasicUdpTransport(IPEndPoint)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Transport.BasicUdpTransport..ctor(System.Net.IPEndPoint)

   Initializes a new instance of BasicUdpTransport.

   .. code-block:: csharp

      public BasicUdpTransport(IPEndPoint targetEndPoint)

   :type targetEndPoint: ``IPEndPoint``

**Source:** `SharpSnmpLib/Transport/BasicUdpTransport.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/BasicUdpTransport.cs#L45>`__

Properties
----------

ListenEndpoint
~~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Transport.BasicUdpTransport.ListenEndpoint

   Gets listen Endpoint.

   .. code-block:: csharp

      public IPEndPoint ListenEndpoint { get; init; }

   :rtype: ``IPEndPoint``

**Source:** `SharpSnmpLib/Transport/BasicUdpTransport.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/BasicUdpTransport.cs#L20>`__

TargetEndPoint
~~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Transport.BasicUdpTransport.TargetEndPoint

   Gets target End Point.

   .. code-block:: csharp

      public IPEndPoint TargetEndPoint { get; }

   :rtype: ``IPEndPoint``

**Source:** `SharpSnmpLib/Transport/BasicUdpTransport.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/BasicUdpTransport.cs#L27>`__

UdpClient
~~~~~~~~~

.. dn:property:: DotNetSnmp.Transport.BasicUdpTransport.UdpClient

   Stores udp Client.

   .. code-block:: csharp

      public UdpClient UdpClient { get; }

   :rtype: ``UdpClient``

**Source:** `SharpSnmpLib/Transport/BasicUdpTransport.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/BasicUdpTransport.cs#L15>`__

Methods
-------

Close()
~~~~~~~

.. dn:method:: DotNetSnmp.Transport.BasicUdpTransport.Close

   Closes the underlying UDP socket.

   .. code-block:: csharp

      public void Close()

**Source:** `SharpSnmpLib/Transport/BasicUdpTransport.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/BasicUdpTransport.cs#L87>`__

Dispose()
~~~~~~~~~

.. dn:method:: DotNetSnmp.Transport.BasicUdpTransport.Dispose

   .. code-block:: csharp

      public void Dispose()

**Source:** `SharpSnmpLib/Transport/BasicUdpTransport.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/BasicUdpTransport.cs#L93>`__

Dispose(Boolean)
~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Transport.BasicUdpTransport.Dispose(System.Boolean)

   Disposes the underlying UDP client.

   .. code-block:: csharp

      protected virtual void Dispose(bool disposing)

   :param disposing: Whether to dispose managed resources.
   :type disposing: ``Boolean``

**Source:** `SharpSnmpLib/Transport/BasicUdpTransport.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/BasicUdpTransport.cs#L103>`__

Finalize()
~~~~~~~~~~

.. dn:method:: DotNetSnmp.Transport.BasicUdpTransport.Finalize

   Finalizer to ensure resources are released if Dispose is not called.

   .. code-block:: csharp

      protected void Finalize()

**Source:** `SharpSnmpLib/Transport/BasicUdpTransport.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/BasicUdpTransport.cs#L114>`__

ReceiveAsync(IPEndPoint, CancellationToken)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Transport.BasicUdpTransport.ReceiveAsync(System.Net.IPEndPoint,System.Threading.CancellationToken)

   Receives async.

   .. code-block:: csharp

      public ValueTask<ReadOnlyMemory<byte>> ReceiveAsync(IPEndPoint targetEndPoint, CancellationToken cancellationToken = default(CancellationToken))

   :type targetEndPoint: ``IPEndPoint``
   :type cancellationToken: ``CancellationToken``

   :rtype: ``ValueTask<ReadOnlyMemory<Byte>>``

**Source:** `SharpSnmpLib/Transport/BasicUdpTransport.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/BasicUdpTransport.cs#L68>`__

SendAsync(ReadOnlyMemory<Byte>, IPEndPoint, CancellationToken)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Transport.BasicUdpTransport.SendAsync(System.ReadOnlyMemory{System.Byte},System.Net.IPEndPoint,System.Threading.CancellationToken)

   Sends async.

   .. code-block:: csharp

      public ValueTask<int> SendAsync(ReadOnlyMemory<byte> message, IPEndPoint targetEndPoint, CancellationToken cancellationToken = default(CancellationToken))

   :type message: ``ReadOnlyMemory<Byte>``
   :type targetEndPoint: ``IPEndPoint``
   :type cancellationToken: ``CancellationToken``

   :rtype: ``ValueTask<Int32>``

**Source:** `SharpSnmpLib/Transport/BasicUdpTransport.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/BasicUdpTransport.cs#L54>`__

