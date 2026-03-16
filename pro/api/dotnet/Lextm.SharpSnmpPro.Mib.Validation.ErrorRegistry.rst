ErrorRegistry Class
===================

.. dn:class:: Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry

   A registry that stores all errors and warnings.

   .. code-block:: csharp

      public class ErrorRegistry

**Namespace:** ``Lextm.SharpSnmpPro.Mib.Validation``

**Inheritance:** Object → ``ErrorRegistry``

Constructors
------------

ErrorRegistry()
~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry..ctor

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry`` class.

   .. code-block:: csharp

      public ErrorRegistry()

Properties
----------

Errors
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry.Errors

   Errors.

   .. code-block:: csharp

      public IReadOnlyCollection<CompilerError> Errors { get; }

   :rtype: ``IReadOnlyCollection<CompilerError>``

Messages
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry.Messages

   Messages.

   .. code-block:: csharp

      public IReadOnlyCollection<CompilerMessage> Messages { get; }

   :rtype: ``IReadOnlyCollection<CompilerMessage>``

Warnings
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry.Warnings

   Warnings.

   .. code-block:: csharp

      public IReadOnlyCollection<CompilerWarning> Warnings { get; }

   :rtype: ``IReadOnlyCollection<CompilerWarning>``

Methods
-------

AddError(ErrorCategory, String, IConstruct[])
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry.AddError(Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory,System.String,Lextm.SharpSnmpPro.Mib.IConstruct[])

   Adds an error.

   .. code-block:: csharp

      public void AddError(ErrorCategory category, string message, params IConstruct[] constructs)

   :param category: The category.
   :type category: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory`
   :param message: The message.
   :type message: ``String``
   :param constructs: The constructs.
   :type constructs: ``IConstruct[]``

AddError(ErrorCategory, String, IToken, String)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry.AddError(Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory,System.String,Antlr4.Runtime.IToken,System.String)

   Adds an error.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public void AddError(ErrorCategory category, string message, IToken token, string fileName)

   :param category: The category.
   :type category: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory`
   :param message: The message.
   :type message: ``String``
   :param token: The token.
   :type token: ``IToken``
   :param fileName: Name of the file.
   :type fileName: ``String``

AddError(RecognitionException, String)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry.AddError(Antlr4.Runtime.RecognitionException,System.String)

   Adds an error.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public void AddError(RecognitionException exception, string fileName)

   :param exception: The exception.
   :type exception: ``RecognitionException``
   :param fileName: Name of the file.
   :type fileName: ``String``

AddMessage(MessageCategory, String, IConstruct[])
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry.AddMessage(Lextm.SharpSnmpPro.Mib.Validation.MessageCategory,System.String,Lextm.SharpSnmpPro.Mib.IConstruct[])

   Adds a message.

   .. code-block:: csharp

      public void AddMessage(MessageCategory category, string message, params IConstruct[] constructs)

   :param category: The category.
   :type category: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.MessageCategory`
   :param message: The message.
   :type message: ``String``
   :param constructs: The constructs.
   :type constructs: ``IConstruct[]``

AddMessage(MessageCategory, String, IToken, String)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry.AddMessage(Lextm.SharpSnmpPro.Mib.Validation.MessageCategory,System.String,Antlr4.Runtime.IToken,System.String)

   Adds a message.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public void AddMessage(MessageCategory category, string message, IToken token, string fileName)

   :param category: The category.
   :type category: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.MessageCategory`
   :param message: The message.
   :type message: ``String``
   :param token: The token.
   :type token: ``IToken``
   :param fileName: Name of the file.
   :type fileName: ``String``

AddWarning(WarningCategory, String, IConstruct[])
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry.AddWarning(Lextm.SharpSnmpPro.Mib.Validation.WarningCategory,System.String,Lextm.SharpSnmpPro.Mib.IConstruct[])

   Adds a warning.

   .. code-block:: csharp

      public void AddWarning(WarningCategory category, string message, params IConstruct[] constructs)

   :param category: The category.
   :type category: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.WarningCategory`
   :param message: The message.
   :type message: ``String``
   :param constructs: The constructs.
   :type constructs: ``IConstruct[]``

AddWarning(WarningCategory, String, IToken, String)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry.AddWarning(Lextm.SharpSnmpPro.Mib.Validation.WarningCategory,System.String,Antlr4.Runtime.IToken,System.String)

   Adds a warning.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public void AddWarning(WarningCategory category, string message, IToken token, string fileName)

   :param category: The category.
   :type category: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.WarningCategory`
   :param message: The message.
   :type message: ``String``
   :param token: The token.
   :type token: ``IToken``
   :param fileName: Name of the file.
   :type fileName: ``String``

OnErrorAdded(Object, CompilerError)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry.OnErrorAdded(System.Object,Lextm.SharpSnmpPro.Mib.Validation.CompilerError)

   Called when an error is added.

   .. code-block:: csharp

      protected virtual void OnErrorAdded(object sender, CompilerError error)

   :param sender: The sender.
   :type sender: ``Object``
   :param error: The error.
   :type error: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Validation.CompilerError`

OnMessageAdded(Object, CompilerMessage)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry.OnMessageAdded(System.Object,Lextm.SharpSnmpPro.Mib.Validation.CompilerMessage)

   Called when a message is added.

   .. code-block:: csharp

      protected virtual void OnMessageAdded(object sender, CompilerMessage message)

   :param sender: The sender.
   :type sender: ``Object``
   :param message: The message.
   :type message: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Validation.CompilerMessage`

OnWarningAdded(Object, CompilerWarning)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry.OnWarningAdded(System.Object,Lextm.SharpSnmpPro.Mib.Validation.CompilerWarning)

   Called when a warning is added.

   .. code-block:: csharp

      protected virtual void OnWarningAdded(object sender, CompilerWarning warning)

   :param sender: The sender.
   :type sender: ``Object``
   :param warning: The warning.
   :type warning: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Validation.CompilerWarning`

Events
------

ErrorAdded
~~~~~~~~~~

.. dn:event:: Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry.ErrorAdded

   Occurs when an error is added.

   .. code-block:: csharp

      public event EventHandler<CompilerError> ErrorAdded

   :rtype: ``EventHandler<CompilerError>``

MessageAdded
~~~~~~~~~~~~

.. dn:event:: Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry.MessageAdded

   Occurs when a message is added.

   .. code-block:: csharp

      public event EventHandler<CompilerMessage> MessageAdded

   :rtype: ``EventHandler<CompilerMessage>``

WarningAdded
~~~~~~~~~~~~

.. dn:event:: Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry.WarningAdded

   Occurs when a warning is added.

   .. code-block:: csharp

      public event EventHandler<CompilerWarning> WarningAdded

   :rtype: ``EventHandler<CompilerWarning>``

