ObjectTree Class
================

.. dn:class:: Lextm.SharpSnmpPro.Mib.Registry.ObjectTree

   Object tree class.

   .. code-block:: csharp

      public sealed class ObjectTree

**Namespace:** ``Lextm.SharpSnmpPro.Mib.Registry``

**Inheritance:** Object → ``ObjectTree``

Constructors
------------

ObjectTree()
~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.Registry.ObjectTree..ctor

   Creates an :dn:cls:``~Lextm.SharpSnmpPro.Mib.Registry.ObjectTree`` instance.

   .. code-block:: csharp

      public ObjectTree()

Properties
----------

Collector
~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Registry.ObjectTree.Collector

   Gets or sets the collector.

   .. code-block:: csharp

      public ErrorRegistry Collector { get; set; }

   :returns: The collector.
   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry`

LoadedModules
~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Registry.ObjectTree.LoadedModules

   Loaded MIB modules.

   .. code-block:: csharp

      public IReadOnlyCollection<Module> LoadedModules { get; }

   :returns: The loaded modules.
   :rtype: ``IReadOnlyCollection<Module>``

PendingModules
~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Registry.ObjectTree.PendingModules

   Pending MIB modules.

   .. code-block:: csharp

      public IReadOnlyCollection<Module> PendingModules { get; }

   :returns: The pending modules.
   :rtype: ``IReadOnlyCollection<Module>``

PendingModulesAllowed
~~~~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Registry.ObjectTree.PendingModulesAllowed

   Gets or sets a value indicating whether pending modules are allowed.

   .. code-block:: csharp

      public bool PendingModulesAllowed { get; set; }

   :rtype: ``Boolean``

Roots
~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Registry.ObjectTree.Roots

   Root definitions.

   .. code-block:: csharp

      public IList<Definition> Roots { get; }

   :rtype: ``IList<Definition>``

Methods
-------

Find(String, String)
~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Registry.ObjectTree.Find(System.String,System.String)

   Finds the name in specified module.

   .. code-block:: csharp

      public Definition Find(string moduleName, string name)

   :param moduleName: Name of the module.
   :type moduleName: ``String``
   :param name: The name.
   :type name: ``String``

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Registry.Definition`

Import(IEnumerable<Module>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Registry.ObjectTree.Import(System.Collections.Generic.IEnumerable{Lextm.SharpSnmpPro.Mib.Module})

   Imports the specified modules.

   .. code-block:: csharp

      public void Import(IEnumerable<Module> modules)

   :param modules: The modules.
   :type modules: ``IEnumerable<Module>``

Refresh()
~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Registry.ObjectTree.Refresh

   Refreshes this instance.

   .. code-block:: csharp

      public void Refresh()

Search(UInt32[])
~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Registry.ObjectTree.Search(System.UInt32[])

   Searches the specified object via identifier.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public SearchResult Search(uint[] id)

   :param id: The identifier.
   :type id: ``UInt32[]``

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Registry.SearchResult`

Unload(String)
~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Registry.ObjectTree.Unload(System.String)

   Unloads a module.

   .. code-block:: csharp

      public Module Unload(string name)

   :param name: Module name.
   :type name: ``String``

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Module`

