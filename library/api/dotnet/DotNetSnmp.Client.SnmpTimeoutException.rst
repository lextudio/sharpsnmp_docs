SnmpTimeoutException Class
==========================

.. dn:class:: DotNetSnmp.Client.SnmpTimeoutException

   Exception thrown when an SNMP operation times out.

   .. code-block:: csharp

      public class SnmpTimeoutException : Exception, ISerializable

**Namespace:** ``DotNetSnmp.Client``

**Inheritance:** Object → Exception → ``SnmpTimeoutException``

**Source:** `SharpSnmpLib/Dispatch/SnmpTimeoutException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Dispatch/SnmpTimeoutException.cs#L7>`__

Constructors
------------

SnmpTimeoutException(String, Exception)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Client.SnmpTimeoutException..ctor(System.String,System.Exception)

   Initializes a new instance of SnmpTimeoutException.

   .. code-block:: csharp

      public SnmpTimeoutException(string message, Exception innerException)

   :param message: The error message.
   :type message: ``String``
   :param innerException: The inner exception.
   :type innerException: ``Exception``

**Source:** `SharpSnmpLib/Dispatch/SnmpTimeoutException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Dispatch/SnmpTimeoutException.cs#L57>`__

SnmpTimeoutException(String, IPEndPoint, Exception)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Client.SnmpTimeoutException..ctor(System.String,System.Net.IPEndPoint,System.Exception)

   Initializes a new instance of SnmpTimeoutException.

   .. code-block:: csharp

      public SnmpTimeoutException(string message, IPEndPoint targetEndpoint, Exception innerException)

   :param message: The error message.
   :type message: ``String``
   :param targetEndpoint: The target endpoint that timed out.
   :type targetEndpoint: ``IPEndPoint``
   :param innerException: The inner exception.
   :type innerException: ``Exception``

**Source:** `SharpSnmpLib/Dispatch/SnmpTimeoutException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Dispatch/SnmpTimeoutException.cs#L68>`__

SnmpTimeoutException(String, IPEndPoint, Int32)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Client.SnmpTimeoutException..ctor(System.String,System.Net.IPEndPoint,System.Int32)

   Initializes a new instance of SnmpTimeoutException.

   .. code-block:: csharp

      public SnmpTimeoutException(string message, IPEndPoint targetEndpoint, int timeout)

   :param message: The error message.
   :type message: ``String``
   :param targetEndpoint: The target endpoint that timed out.
   :type targetEndpoint: ``IPEndPoint``
   :param timeout: The timeout duration that was exceeded (in milliseconds).
   :type timeout: ``Int32``

**Source:** `SharpSnmpLib/Dispatch/SnmpTimeoutException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Dispatch/SnmpTimeoutException.cs#L45>`__

SnmpTimeoutException(String, IPEndPoint)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Client.SnmpTimeoutException..ctor(System.String,System.Net.IPEndPoint)

   Initializes a new instance of SnmpTimeoutException.

   .. code-block:: csharp

      public SnmpTimeoutException(string message, IPEndPoint targetEndpoint)

   :param message: The error message.
   :type message: ``String``
   :param targetEndpoint: The target endpoint that timed out.
   :type targetEndpoint: ``IPEndPoint``

**Source:** `SharpSnmpLib/Dispatch/SnmpTimeoutException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Dispatch/SnmpTimeoutException.cs#L33>`__

SnmpTimeoutException(String)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Client.SnmpTimeoutException..ctor(System.String)

   Initializes a new instance of SnmpTimeoutException.

   .. code-block:: csharp

      public SnmpTimeoutException(string message)

   :param message: The error message.
   :type message: ``String``

**Source:** `SharpSnmpLib/Dispatch/SnmpTimeoutException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Dispatch/SnmpTimeoutException.cs#L23>`__

Properties
----------

TargetEndpoint
~~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Client.SnmpTimeoutException.TargetEndpoint

   Gets target Endpoint.

   .. code-block:: csharp

      public IPEndPoint? TargetEndpoint { get; }

   :rtype: ``IPEndPoint``

**Source:** `SharpSnmpLib/Dispatch/SnmpTimeoutException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Dispatch/SnmpTimeoutException.cs#L12>`__

Timeout
~~~~~~~

.. dn:property:: DotNetSnmp.Client.SnmpTimeoutException.Timeout

   Gets timeout.

   .. code-block:: csharp

      public int Timeout { get; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Dispatch/SnmpTimeoutException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Dispatch/SnmpTimeoutException.cs#L17>`__

