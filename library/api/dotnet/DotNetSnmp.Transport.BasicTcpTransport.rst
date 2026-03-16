BasicTcpTransport Class
=======================

.. dn:class:: DotNetSnmp.Transport.BasicTcpTransport

   SNMP-over-TCP client transport implementing RFC 3430 length-prefix framing.

   .. code-block:: csharp

      public class BasicTcpTransport : ISnmpTransport, IDisposable

**Namespace:** ``DotNetSnmp.Transport``

**Inheritance:** Object → ``BasicTcpTransport``

**Source:** `SharpSnmpLib/Transport/BasicTcpTransport.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/BasicTcpTransport.cs#L39>`__

Constructors
------------

BasicTcpTransport(IPEndPoint)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Transport.BasicTcpTransport..ctor(System.Net.IPEndPoint)

   Initializes a new instance of :dn:cls:``~DotNetSnmp.Transport.BasicTcpTransport``.

   .. code-block:: csharp

      public BasicTcpTransport(IPEndPoint targetEndPoint)

   :param targetEndPoint: The remote SNMP agent endpoint to connect to.
   :type targetEndPoint: ``IPEndPoint``

**Source:** `SharpSnmpLib/Transport/BasicTcpTransport.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/BasicTcpTransport.cs#L55>`__

Properties
----------

TargetEndPoint
~~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Transport.BasicTcpTransport.TargetEndPoint

   Gets the target endpoint.

   .. code-block:: csharp

      public IPEndPoint TargetEndPoint { get; }

   :rtype: ``IPEndPoint``

**Source:** `SharpSnmpLib/Transport/BasicTcpTransport.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/BasicTcpTransport.cs#L63>`__

Methods
-------

Close()
~~~~~~~

.. dn:method:: DotNetSnmp.Transport.BasicTcpTransport.Close

   Closes the TCP connection.

   .. code-block:: csharp

      public void Close()

**Source:** `SharpSnmpLib/Transport/BasicTcpTransport.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/BasicTcpTransport.cs#L125>`__

Dispose()
~~~~~~~~~

.. dn:method:: DotNetSnmp.Transport.BasicTcpTransport.Dispose

   .. code-block:: csharp

      public void Dispose()

**Source:** `SharpSnmpLib/Transport/BasicTcpTransport.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/BasicTcpTransport.cs#L134>`__

Dispose(Boolean)
~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Transport.BasicTcpTransport.Dispose(System.Boolean)

   Disposes managed resources.

   .. code-block:: csharp

      protected virtual void Dispose(bool disposing)

   :type disposing: ``Boolean``

**Source:** `SharpSnmpLib/Transport/BasicTcpTransport.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/BasicTcpTransport.cs#L143>`__

Finalize()
~~~~~~~~~~

.. dn:method:: DotNetSnmp.Transport.BasicTcpTransport.Finalize

   Finalizer.

   .. code-block:: csharp

      protected void Finalize()

**Source:** `SharpSnmpLib/Transport/BasicTcpTransport.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/BasicTcpTransport.cs#L161>`__

ReceiveAsync(IPEndPoint, CancellationToken)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Transport.BasicTcpTransport.ReceiveAsync(System.Net.IPEndPoint,System.Threading.CancellationToken)

   Receives an SNMP response with RFC 3430 length-prefix framing.

   .. code-block:: csharp

      public ValueTask<ReadOnlyMemory<byte>> ReceiveAsync(IPEndPoint targetEndPoint, CancellationToken cancellationToken)

   :type targetEndPoint: ``IPEndPoint``
   :type cancellationToken: ``CancellationToken``

   :rtype: ``ValueTask<ReadOnlyMemory<Byte>>``

**Source:** `SharpSnmpLib/Transport/BasicTcpTransport.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/BasicTcpTransport.cs#L92>`__

SendAsync(ReadOnlyMemory<Byte>, IPEndPoint, CancellationToken)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Transport.BasicTcpTransport.SendAsync(System.ReadOnlyMemory{System.Byte},System.Net.IPEndPoint,System.Threading.CancellationToken)

   Sends an SNMP message with RFC 3430 length-prefix framing. Establishes the TCP connection on first call.

   .. code-block:: csharp

      public ValueTask<int> SendAsync(ReadOnlyMemory<byte> message, IPEndPoint targetEndPoint, CancellationToken cancellationToken = default(CancellationToken))

   :type message: ``ReadOnlyMemory<Byte>``
   :type targetEndPoint: ``IPEndPoint``
   :type cancellationToken: ``CancellationToken``

   :rtype: ``ValueTask<Int32>``

**Source:** `SharpSnmpLib/Transport/BasicTcpTransport.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/BasicTcpTransport.cs#L69>`__

