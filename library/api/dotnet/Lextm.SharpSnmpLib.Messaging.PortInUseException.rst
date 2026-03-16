PortInUseException Class
========================

.. dn:class:: Lextm.SharpSnmpLib.Messaging.PortInUseException

   Exception raised when an endpoint is already in use.

   .. code-block:: csharp

      [Obsolete("This type is for internal use only and may be removed in a future release.")]
      public sealed class PortInUseException : SnmpException, ISerializable

**Namespace:** ``Lextm.SharpSnmpLib.Messaging``

**Inheritance:** Object → Exception → SnmpException → ``PortInUseException``

**Source:** `SharpSnmpLib/Messaging/PortInUseException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/PortInUseException.cs#L7>`__

Constructors
------------

PortInUseException()
~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Messaging.PortInUseException..ctor

   Initializes a new instance of :dn:cls:``~Lextm.SharpSnmpLib.Messaging.PortInUseException``.

   .. code-block:: csharp

      public PortInUseException()

**Source:** `SharpSnmpLib/Messaging/PortInUseException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/PortInUseException.cs#L13>`__

PortInUseException(String, Exception)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Messaging.PortInUseException..ctor(System.String,System.Exception)

   Initializes a new instance of :dn:cls:``~Lextm.SharpSnmpLib.Messaging.PortInUseException``.

   .. code-block:: csharp

      public PortInUseException(string message, Exception inner)

   :type message: ``String``
   :type inner: ``Exception``

**Source:** `SharpSnmpLib/Messaging/PortInUseException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/PortInUseException.cs#L28>`__

PortInUseException(String)
~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Messaging.PortInUseException..ctor(System.String)

   Initializes a new instance of :dn:cls:``~Lextm.SharpSnmpLib.Messaging.PortInUseException``.

   .. code-block:: csharp

      public PortInUseException(string message)

   :type message: ``String``

**Source:** `SharpSnmpLib/Messaging/PortInUseException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/PortInUseException.cs#L20>`__

Properties
----------

Endpoint
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.PortInUseException.Endpoint

   Gets or sets endpoint already in use.

   .. code-block:: csharp

      public IPEndPoint? Endpoint { get; set; }

   :rtype: ``IPEndPoint``

**Source:** `SharpSnmpLib/Messaging/PortInUseException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/PortInUseException.cs#L36>`__

