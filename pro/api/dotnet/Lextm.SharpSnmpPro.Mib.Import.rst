Import Class
============

.. dn:class:: Lextm.SharpSnmpPro.Mib.Import

   IMPORT statement.

   .. code-block:: csharp

      public class Import : IConstruct

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``Import``

Properties
----------

CharPositionInLine
~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Import.CharPositionInLine

   Gets the char position in line.

   .. code-block:: csharp

      public int CharPositionInLine { get; set; }

   :returns: The char position in line.
   :rtype: ``Int32``

Line
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Import.Line

   Gets the line number.

   .. code-block:: csharp

      public int Line { get; set; }

   :returns: The line.
   :rtype: ``Int32``

Module
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Import.Module

   Gets or sets the module.

   .. code-block:: csharp

      public Module Module { get; set; }

   :returns: The module.
   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Module`

ModuleName
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Import.ModuleName

   Gets or sets the name of the module.

   .. code-block:: csharp

      public string ModuleName { get; set; }

   :returns: The name of the module.
   :rtype: ``String``

Name
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Import.Name

   Name.

   .. code-block:: csharp

      public string Name { get; set; }

   :rtype: ``String``

Symbols
~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Import.Symbols

   Gets or sets the symbols to import.

   .. code-block:: csharp

      public IEnumerable<Symbol> Symbols { get; set; }

   :returns: The symbols.
   :rtype: ``IEnumerable<Symbol>``

