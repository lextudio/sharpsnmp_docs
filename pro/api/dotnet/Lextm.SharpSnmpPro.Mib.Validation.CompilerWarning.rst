CompilerWarning Class
=====================

.. dn:class:: Lextm.SharpSnmpPro.Mib.Validation.CompilerWarning

   Compiler generated warning.

   .. code-block:: csharp

      public class CompilerWarning

**Namespace:** ``Lextm.SharpSnmpPro.Mib.Validation``

**Inheritance:** Object → ``CompilerWarning``

Constructors
------------

CompilerWarning(WarningCategory, String, IConstruct[])
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.Validation.CompilerWarning..ctor(Lextm.SharpSnmpPro.Mib.Validation.WarningCategory,System.String,Lextm.SharpSnmpPro.Mib.IConstruct[])

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.Validation.CompilerWarning`` class, representing a warning generated during compilation.

   .. code-block:: csharp

      public CompilerWarning(WarningCategory category, string message, IConstruct[] constructs)

   :param category: The category of the warning, indicating its type or severity.
   :type category: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.WarningCategory`
   :param message: The message describing the warning in detail.
   :type message: ``String``
   :param constructs: An array of constructs associated with the warning, such as code elements or locations.
   :type constructs: ``IConstruct[]``

CompilerWarning(WarningCategory, String, IToken, String)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.Validation.CompilerWarning..ctor(Lextm.SharpSnmpPro.Mib.Validation.WarningCategory,System.String,Antlr4.Runtime.IToken,System.String)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.Validation.CompilerWarning`` class, representing a compiler warning with detailed information.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public CompilerWarning(WarningCategory category, string message, IToken token, string fileName)

   :param category: The category of the warning, indicating its type or severity.
   :type category: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.WarningCategory`
   :param message: The message describing the warning in detail.
   :type message: ``String``
   :param token: The token associated with the warning, providing context within the source code.
   :type token: ``IToken``
   :param fileName: The name of the file where the warning occurred.
   :type fileName: ``String``

Properties
----------

Category
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Validation.CompilerWarning.Category

   Gets or sets the category of the warning.

   .. code-block:: csharp

      public WarningCategory Category { get; set; }

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.WarningCategory`

Methods
-------

ToString()
~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Validation.CompilerWarning.ToString

   .. code-block:: csharp

      public override string ToString()

   :rtype: ``String``

