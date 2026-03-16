ErrorMacro Class
================

.. dn:class:: Lextm.SharpSnmpPro.Mib.ErrorMacro

   Represents an ERROR MACRO type in a MIB module.

   .. code-block:: csharp

      public class ErrorMacro : ISmiType, IConstruct

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``ErrorMacro``

Properties
----------

CharPositionInLine
~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ErrorMacro.CharPositionInLine

   Gets the char position in line.

   .. code-block:: csharp

      public int CharPositionInLine { get; set; }

   :returns: The char position in line.
   :rtype: ``Int32``

Identifier
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ErrorMacro.Identifier

   Gets or sets the identifier of this error macro.

   .. code-block:: csharp

      public string Identifier { get; set; }

   :rtype: ``String``

Line
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ErrorMacro.Line

   Gets the line number.

   .. code-block:: csharp

      public int Line { get; set; }

   :returns: The line.
   :rtype: ``Int32``

Module
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ErrorMacro.Module

   Gets or sets the module.

   .. code-block:: csharp

      public Module Module { get; set; }

   :returns: The module.
   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Module`

Name
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ErrorMacro.Name

   Name.

   .. code-block:: csharp

      public string Name { get; set; }

   :rtype: ``String``

Subtype
~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ErrorMacro.Subtype

   Gets or sets the subtype of this error macro.

   .. code-block:: csharp

      public ISmiType Subtype { get; set; }

   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiType`

Methods
-------

Append(StringBuilder)
~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.ErrorMacro.Append(System.Text.StringBuilder)

   Appends the type name to the provided ``StringBuilder``.

   .. code-block:: csharp

      public void Append(StringBuilder typeName)

   :param typeName: The ``StringBuilder`` to append the type name to.
   :type typeName: ``StringBuilder``

