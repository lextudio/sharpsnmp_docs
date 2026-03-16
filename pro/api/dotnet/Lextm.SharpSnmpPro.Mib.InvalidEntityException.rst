InvalidEntityException Class
============================

.. dn:class:: Lextm.SharpSnmpPro.Mib.InvalidEntityException

   The exception that is thrown when an invalid entity is encountered in the MIB.

   .. code-block:: csharp

      public class InvalidEntityException : SnmpException, ISerializable

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → Exception → SnmpException → ``InvalidEntityException``

Constructors
------------

InvalidEntityException()
~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.InvalidEntityException..ctor

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.InvalidEntityException`` class.

   .. code-block:: csharp

      public InvalidEntityException()

InvalidEntityException(String, Exception)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.InvalidEntityException..ctor(System.String,System.Exception)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.InvalidEntityException`` class with a specified error message and a reference to the inner exception that is the cause of this exception.

   .. code-block:: csharp

      public InvalidEntityException(string message, Exception innerException)

   :param message: The message that describes the error.
   :type message: ``String``
   :param innerException: The exception that is the cause of the current exception, or a null reference if no inner exception is specified.
   :type innerException: ``Exception``

InvalidEntityException(String)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.InvalidEntityException..ctor(System.String)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.InvalidEntityException`` class with a specified error message.

   .. code-block:: csharp

      public InvalidEntityException(string message)

   :param message: The message that describes the error.
   :type message: ``String``

