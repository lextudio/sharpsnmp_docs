NotResolvedException Class
==========================

.. dn:class:: Lextm.SharpSnmpPro.Mib.NotResolvedException

   Exception raised when type resolution fails.

   .. code-block:: csharp

      public class NotResolvedException : SnmpException, ISerializable

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → Exception → SnmpException → ``NotResolvedException``

Constructors
------------

NotResolvedException()
~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.NotResolvedException..ctor

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.NotResolvedException`` class.

   .. code-block:: csharp

      public NotResolvedException()

NotResolvedException(String, Exception)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.NotResolvedException..ctor(System.String,System.Exception)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.NotResolvedException`` class with a specified error message and a reference to the inner exception that is the cause of this exception.

   .. code-block:: csharp

      public NotResolvedException(string message, Exception inner)

   :param message: The error message that explains the reason for the exception.
   :type message: ``String``
   :param inner: The exception that is the cause of the current exception.
   :type inner: ``Exception``

NotResolvedException(String)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.NotResolvedException..ctor(System.String)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.NotResolvedException`` class with a specified error message.

   .. code-block:: csharp

      public NotResolvedException(string message)

   :param message: The message that describes the error.
   :type message: ``String``

Properties
----------

BrokenType
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.NotResolvedException.BrokenType

   Gets the :dn:iface:``~Lextm.SharpSnmpPro.Mib.ISmiType`` that could not be resolved.

   .. code-block:: csharp

      public ISmiType BrokenType { get; }

   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiType`

FullMessage
~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.NotResolvedException.FullMessage

   Gets the full error message including inner exception messages.

   .. code-block:: csharp

      public string FullMessage { get; }

   :rtype: ``String``

Type
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.NotResolvedException.Type

   Gets or sets the :dn:iface:``~Lextm.SharpSnmpPro.Mib.ISmiType`` associated with this exception.

   .. code-block:: csharp

      public ISmiType Type { get; }

   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiType`

