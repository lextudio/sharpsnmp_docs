Exports Class
=============

.. dn:class:: Lextm.SharpSnmpPro.Mib.Exports

   Represents a collection of exported symbols from a MIB module.

   .. code-block:: csharp

      public class Exports

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``Exports``

Properties
----------

AllExported
~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Exports.AllExported

   Gets or sets a value indicating whether all symbols are exported.

   .. code-block:: csharp

      public bool AllExported { get; set; }

   :rtype: ``Boolean``

Symbols
~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Exports.Symbols

   Gets the list of exported symbol names.

   .. code-block:: csharp

      public IList<string> Symbols { get; }

   :rtype: ``IList<String>``

Methods
-------

Add(String)
~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Exports.Add(System.String)

   Adds a symbol to the list of exported symbols.

   .. code-block:: csharp

      public void Add(string symbol)

   :param symbol: The symbol name to add.
   :type symbol: ``String``

