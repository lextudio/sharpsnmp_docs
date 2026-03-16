CompilerError Class
===================

.. dn:class:: Lextm.SharpSnmpPro.Mib.Validation.CompilerError

   Compiler generated error.

   .. code-block:: csharp

      [DataContract]
      public class CompilerError

**Namespace:** ``Lextm.SharpSnmpPro.Mib.Validation``

**Inheritance:** Object → ``CompilerError``

Constructors
------------

CompilerError(ErrorCategory, String, IConstruct[])
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.Validation.CompilerError..ctor(Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory,System.String,Lextm.SharpSnmpPro.Mib.IConstruct[])

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.Validation.CompilerError`` class.

   .. code-block:: csharp

      public CompilerError(ErrorCategory category, string message, params IConstruct[] constructs)

   :param category: The category.
   :type category: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory`
   :param message: The message.
   :type message: ``String``
   :param constructs: The constructs.
   :type constructs: ``IConstruct[]``

CompilerError(ErrorCategory, String, IToken, String)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.Validation.CompilerError..ctor(Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory,System.String,Antlr4.Runtime.IToken,System.String)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.Validation.CompilerError`` class.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public CompilerError(ErrorCategory category, string message, IToken token, string fileName)

   :param category: The category.
   :type category: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory`
   :param message: The message.
   :type message: ``String``
   :param token: The token.
   :type token: ``IToken``
   :param fileName: Name of the file.
   :type fileName: ``String``

CompilerError(RecognitionException, String)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.Validation.CompilerError..ctor(Antlr4.Runtime.RecognitionException,System.String)

   Creates a :dn:cls:``~Lextm.SharpSnmpPro.Mib.Validation.CompilerError`` instance with a specific ``Exception``.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public CompilerError(RecognitionException exception, string fileName)

   :param exception: Compiler exception.
   :type exception: ``RecognitionException``
   :param fileName: Name of the file.
   :type fileName: ``String``

Properties
----------

Category
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Validation.CompilerError.Category

   Category of the error.

   .. code-block:: csharp

      public ErrorCategory Category { get; set; }

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory`

Methods
-------

ToString()
~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Validation.CompilerError.ToString

   Returns a ``String`` that represents this :dn:cls:``~Lextm.SharpSnmpPro.Mib.Validation.CompilerError``.

   .. code-block:: csharp

      public override string ToString()

   :rtype: ``String``

