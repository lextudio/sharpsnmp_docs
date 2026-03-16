SemanticException Class
=======================

.. dn:class:: Lextm.SharpSnmpPro.Mib.SemanticException

   Semantic exception.

   .. code-block:: csharp

      [CLSCompliant(false)]
      [Serializable]
      public class SemanticException : RecognitionException, ISerializable

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → Exception → RecognitionException → ``SemanticException``

Constructors
------------

SemanticException(SerializationInfo, StreamingContext)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.SemanticException..ctor(System.Runtime.Serialization.SerializationInfo,System.Runtime.Serialization.StreamingContext)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.SemanticException`` class with serialized data.

   .. code-block:: csharp

      protected SemanticException(SerializationInfo serializationInfo, StreamingContext streamingContext)

   :param serializationInfo: The object that holds the serialized data about the exception being thrown.
   :type serializationInfo: ``SerializationInfo``
   :param streamingContext: The contextual information about the source or destination of the serialized data.
   :type streamingContext: ``StreamingContext``

Properties
----------

Allowed
~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.SemanticException.Allowed

   Gets or sets the allowed.

   .. code-block:: csharp

      public string Allowed { get; }

   :returns: The allowed.
   :rtype: ``String``

