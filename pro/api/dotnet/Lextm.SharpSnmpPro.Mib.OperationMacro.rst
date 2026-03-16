OperationMacro Class
====================

.. dn:class:: Lextm.SharpSnmpPro.Mib.OperationMacro

   Represents an OPERATION macro in SMI, describing an operation with argument and result types, error list, and linked operations.

   .. code-block:: csharp

      public class OperationMacro : ISmiType, IConstruct

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``OperationMacro``

Properties
----------

ArgumentIdentifier
~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.OperationMacro.ArgumentIdentifier

   Gets or sets the identifier for the argument.

   .. code-block:: csharp

      public string ArgumentIdentifier { get; set; }

   :rtype: ``String``

ArgumentType
~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.OperationMacro.ArgumentType

   Gets or sets the argument type of the operation.

   .. code-block:: csharp

      public ISmiType ArgumentType { get; set; }

   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiType`

CharPositionInLine
~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.OperationMacro.CharPositionInLine

   Gets the char position in line.

   .. code-block:: csharp

      public int CharPositionInLine { get; set; }

   :returns: The char position in line.
   :rtype: ``Int32``

ErrorList
~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.OperationMacro.ErrorList

   Gets or sets the list of possible errors for the operation.

   .. code-block:: csharp

      public IList<TypeOrValue> ErrorList { get; set; }

   :rtype: ``IList<TypeOrValue>``

Line
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.OperationMacro.Line

   Gets the line number.

   .. code-block:: csharp

      public int Line { get; set; }

   :returns: The line.
   :rtype: ``Int32``

LinkedOperationList
~~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.OperationMacro.LinkedOperationList

   Gets or sets the list of linked operations.

   .. code-block:: csharp

      public IList<TypeOrValue> LinkedOperationList { get; set; }

   :rtype: ``IList<TypeOrValue>``

Module
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.OperationMacro.Module

   Gets or sets the module.

   .. code-block:: csharp

      public Module Module { get; set; }

   :returns: The module.
   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Module`

Name
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.OperationMacro.Name

   Name.

   .. code-block:: csharp

      public string Name { get; set; }

   :rtype: ``String``

ResultIdentifier
~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.OperationMacro.ResultIdentifier

   Gets or sets the identifier for the result.

   .. code-block:: csharp

      public string ResultIdentifier { get; set; }

   :rtype: ``String``

ResultType
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.OperationMacro.ResultType

   Gets or sets the result type of the operation.

   .. code-block:: csharp

      public ISmiType ResultType { get; set; }

   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiType`

Methods
-------

Append(StringBuilder)
~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.OperationMacro.Append(System.Text.StringBuilder)

   Appends the type name to the provided ``StringBuilder``.

   .. code-block:: csharp

      public void Append(StringBuilder typeName)

   :param typeName: The ``StringBuilder`` to append the type name to.
   :type typeName: ``StringBuilder``

