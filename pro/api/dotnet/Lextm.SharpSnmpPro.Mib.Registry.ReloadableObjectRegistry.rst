ReloadableObjectRegistry Class
==============================

.. dn:class:: Lextm.SharpSnmpPro.Mib.Registry.ReloadableObjectRegistry

   Object registry.

   .. code-block:: csharp

      public class ReloadableObjectRegistry : ObjectRegistryBase

**Namespace:** ``Lextm.SharpSnmpPro.Mib.Registry``

**Inheritance:** Object → ObjectRegistryBase → ``ReloadableObjectRegistry``

Constructors
------------

ReloadableObjectRegistry(String)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.Registry.ReloadableObjectRegistry..ctor(System.String)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.Registry.ReloadableObjectRegistry`` class.

   .. code-block:: csharp

      public ReloadableObjectRegistry(string path)

   :param path: The path.
   :type path: ``String``

Properties
----------

Path
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Registry.ReloadableObjectRegistry.Path

   Gets the path.

   .. code-block:: csharp

      public string Path { get; }

   :returns: The path.
   :rtype: ``String``

UnloadedModules
~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Registry.ReloadableObjectRegistry.UnloadedModules

   Gets or sets the list of modules that have been unloaded.

   .. code-block:: csharp

      public List<Module> UnloadedModules { get; set; }

   :rtype: ``List<Module>``

Methods
-------

Load(String)
~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Registry.ReloadableObjectRegistry.Load(System.String)

   Loads a module by its name and imports it into the current tree structure.

   .. code-block:: csharp

      public void Load(string name)

   :param name: The name of the module to load. Cannot be null or empty.
   :type name: ``String``

Reload()
~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Registry.ReloadableObjectRegistry.Reload

   Reloads the registry.

   .. code-block:: csharp

      public void Reload()

Unload(String)
~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Registry.ReloadableObjectRegistry.Unload(System.String)

   Unloads the specified module by name and adds it to the list of unloaded modules.

   .. code-block:: csharp

      public void Unload(string name)

   :param name: The name of the module to unload. Cannot be null or empty.
   :type name: ``String``

