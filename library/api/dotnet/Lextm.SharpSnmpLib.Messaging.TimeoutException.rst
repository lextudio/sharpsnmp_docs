TimeoutException Class
======================

.. dn:class:: Lextm.SharpSnmpLib.Messaging.TimeoutException

   Exception raised when an SNMP operation times out.

   .. code-block:: csharp

      [Obsolete("This type is for internal use only and may be removed in a future release.")]
      public sealed class TimeoutException : SnmpException, ISerializable

**Namespace:** ``Lextm.SharpSnmpLib.Messaging``

**Inheritance:** Object → Exception → SnmpException → ``TimeoutException``

**Source:** `SharpSnmpLib/Messaging/TimeoutException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TimeoutException.cs#L7>`__

Constructors
------------

TimeoutException()
~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Messaging.TimeoutException..ctor

   Initializes a new instance of :dn:cls:``~Lextm.SharpSnmpLib.Messaging.TimeoutException``.

   .. code-block:: csharp

      public TimeoutException()

**Source:** `SharpSnmpLib/Messaging/TimeoutException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TimeoutException.cs#L13>`__

TimeoutException(String, Exception)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Messaging.TimeoutException..ctor(System.String,System.Exception)

   Initializes a new instance of :dn:cls:``~Lextm.SharpSnmpLib.Messaging.TimeoutException``.

   .. code-block:: csharp

      public TimeoutException(string message, Exception inner)

   :type message: ``String``
   :type inner: ``Exception``

**Source:** `SharpSnmpLib/Messaging/TimeoutException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TimeoutException.cs#L28>`__

TimeoutException(String)
~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Messaging.TimeoutException..ctor(System.String)

   Initializes a new instance of :dn:cls:``~Lextm.SharpSnmpLib.Messaging.TimeoutException``.

   .. code-block:: csharp

      public TimeoutException(string message)

   :type message: ``String``

**Source:** `SharpSnmpLib/Messaging/TimeoutException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TimeoutException.cs#L20>`__

Properties
----------

Agent
~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.TimeoutException.Agent

   Gets or sets timed-out target address.

   .. code-block:: csharp

      public IPAddress? Agent { get; set; }

   :rtype: ``IPAddress``

**Source:** `SharpSnmpLib/Messaging/TimeoutException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TimeoutException.cs#L36>`__

Timeout
~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.TimeoutException.Timeout

   Gets or sets timeout in milliseconds.

   .. code-block:: csharp

      public int Timeout { get; set; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Messaging/TimeoutException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TimeoutException.cs#L41>`__

Methods
-------

Create(IPAddress, Int32)
~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.TimeoutException.Create(System.Net.IPAddress,System.Int32)

   Creates a timeout exception populated with target and timeout values.

   .. code-block:: csharp

      public static TimeoutException Create(IPAddress agent, int timeout)

   :type agent: ``IPAddress``
   :type timeout: ``Int32``

   :rtype: :dn:cls:`~Lextm.SharpSnmpLib.Messaging.TimeoutException`

**Source:** `SharpSnmpLib/Messaging/TimeoutException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/TimeoutException.cs#L46>`__

