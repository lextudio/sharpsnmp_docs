MessageFactoryException Class
=============================

.. dn:class:: Lextm.SharpSnmpLib.Messaging.MessageFactoryException

   Exception raised when message parsing fails.

   .. code-block:: csharp

      [Obsolete("This type is for internal use only and may be removed in a future release.")]
      public sealed class MessageFactoryException : SnmpException, ISerializable

**Namespace:** ``Lextm.SharpSnmpLib.Messaging``

**Inheritance:** Object → Exception → SnmpException → ``MessageFactoryException``

**Source:** `SharpSnmpLib/Messaging/MessageFactoryException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/MessageFactoryException.cs#L5>`__

Constructors
------------

MessageFactoryException()
~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Messaging.MessageFactoryException..ctor

   Initializes a new instance of :dn:cls:``~Lextm.SharpSnmpLib.Messaging.MessageFactoryException``.

   .. code-block:: csharp

      public MessageFactoryException()

**Source:** `SharpSnmpLib/Messaging/MessageFactoryException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/MessageFactoryException.cs#L13>`__

MessageFactoryException(String, Exception)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Messaging.MessageFactoryException..ctor(System.String,System.Exception)

   Initializes a new instance of :dn:cls:``~Lextm.SharpSnmpLib.Messaging.MessageFactoryException``.

   .. code-block:: csharp

      public MessageFactoryException(string message, Exception inner)

   :type message: ``String``
   :type inner: ``Exception``

**Source:** `SharpSnmpLib/Messaging/MessageFactoryException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/MessageFactoryException.cs#L28>`__

MessageFactoryException(String)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Messaging.MessageFactoryException..ctor(System.String)

   Initializes a new instance of :dn:cls:``~Lextm.SharpSnmpLib.Messaging.MessageFactoryException``.

   .. code-block:: csharp

      public MessageFactoryException(string message)

   :type message: ``String``

**Source:** `SharpSnmpLib/Messaging/MessageFactoryException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/MessageFactoryException.cs#L20>`__

Methods
-------

GetBytes()
~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.MessageFactoryException.GetBytes

   Gets parsed bytes.

   .. code-block:: csharp

      public byte[]? GetBytes()

   :rtype: ``Byte[]``

**Source:** `SharpSnmpLib/Messaging/MessageFactoryException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/MessageFactoryException.cs#L36>`__

SetBytes(Byte[])
~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.MessageFactoryException.SetBytes(System.Byte[])

   Sets parsed bytes.

   .. code-block:: csharp

      public void SetBytes(byte[] value)

   :type value: ``Byte[]``

**Source:** `SharpSnmpLib/Messaging/MessageFactoryException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/MessageFactoryException.cs#L44>`__

