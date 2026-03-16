SnmpMessageProcessingException Class
====================================

.. dn:class:: DotNetSnmp.Client.SnmpMessageProcessingException

   Exception thrown when SNMP message processing fails.

   .. code-block:: csharp

      public class SnmpMessageProcessingException : Exception, ISerializable

**Namespace:** ``DotNetSnmp.Client``

**Inheritance:** Object → Exception → ``SnmpMessageProcessingException``

**Source:** `SharpSnmpLib/Dispatch/SnmpMessageProcessingException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Dispatch/SnmpMessageProcessingException.cs#L5>`__

Constructors
------------

SnmpMessageProcessingException(String, Exception)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Client.SnmpMessageProcessingException..ctor(System.String,System.Exception)

   Initializes a new instance of SnmpMessageProcessingException.

   .. code-block:: csharp

      public SnmpMessageProcessingException(string message, Exception innerException)

   :param message: The error message.
   :type message: ``String``
   :param innerException: The inner exception.
   :type innerException: ``Exception``

**Source:** `SharpSnmpLib/Dispatch/SnmpMessageProcessingException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Dispatch/SnmpMessageProcessingException.cs#L37>`__

SnmpMessageProcessingException(String, MessageProcessingResult, Exception)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Client.SnmpMessageProcessingException..ctor(System.String,DotNetSnmp.Client.MessageProcessingResult,System.Exception)

   Initializes a new instance of SnmpMessageProcessingException.

   .. code-block:: csharp

      public SnmpMessageProcessingException(string message, MessageProcessingResult processingResult, Exception innerException)

   :param message: The error message.
   :type message: ``String``
   :param processingResult: The message processing result that caused the exception.
   :type processingResult: :dn:enum:`~DotNetSnmp.Client.MessageProcessingResult`
   :param innerException: The inner exception.
   :type innerException: ``Exception``

**Source:** `SharpSnmpLib/Dispatch/SnmpMessageProcessingException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Dispatch/SnmpMessageProcessingException.cs#L48>`__

SnmpMessageProcessingException(String, MessageProcessingResult)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Client.SnmpMessageProcessingException..ctor(System.String,DotNetSnmp.Client.MessageProcessingResult)

   Initializes a new instance of SnmpMessageProcessingException.

   .. code-block:: csharp

      public SnmpMessageProcessingException(string message, MessageProcessingResult processingResult)

   :param message: The error message.
   :type message: ``String``
   :param processingResult: The message processing result that caused the exception.
   :type processingResult: :dn:enum:`~DotNetSnmp.Client.MessageProcessingResult`

**Source:** `SharpSnmpLib/Dispatch/SnmpMessageProcessingException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Dispatch/SnmpMessageProcessingException.cs#L26>`__

SnmpMessageProcessingException(String)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Client.SnmpMessageProcessingException..ctor(System.String)

   Initializes a new instance of SnmpMessageProcessingException.

   .. code-block:: csharp

      public SnmpMessageProcessingException(string message)

   :param message: The error message.
   :type message: ``String``

**Source:** `SharpSnmpLib/Dispatch/SnmpMessageProcessingException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Dispatch/SnmpMessageProcessingException.cs#L16>`__

Properties
----------

ProcessingResult
~~~~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Client.SnmpMessageProcessingException.ProcessingResult

   Gets processing Result.

   .. code-block:: csharp

      public MessageProcessingResult ProcessingResult { get; }

   :rtype: :dn:enum:`~DotNetSnmp.Client.MessageProcessingResult`

**Source:** `SharpSnmpLib/Dispatch/SnmpMessageProcessingException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Dispatch/SnmpMessageProcessingException.cs#L10>`__

