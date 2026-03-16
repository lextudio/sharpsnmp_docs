Module Class
============

.. dn:class:: Lextm.SharpSnmpPro.Mib.Module

   MIB module.

   .. code-block:: csharp

      public class Module

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``Module``

Constructors
------------

Module()
~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.Module..ctor

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.Module`` class.

   .. code-block:: csharp

      public Module()

Properties
----------

AllExported
~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Module.AllExported

   Gets or sets a value indicating whether all types in this module are exported.

   .. code-block:: csharp

      public bool AllExported { get; set; }

   :returns: true if all are exported; otherwise, false.
   :rtype: ``Boolean``

Constructs
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Module.Constructs

   Gets the constructs.

   .. code-block:: csharp

      public IList<IConstruct> Constructs { get; }

   :returns: The constructs.
   :rtype: ``IList<IConstruct>``

Entities
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Module.Entities

   Gets the entities.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public IList<IEntity> Entities { get; }

   :returns: The entities.
   :rtype: ``IList<IEntity>``

Exports
~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Module.Exports

   Gets or sets the export types.

   .. code-block:: csharp

      public Exports Exports { get; set; }

   :returns: The exports.
   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Exports`

FileName
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Module.FileName

   Gets or sets the name of the file.

   .. code-block:: csharp

      public string FileName { get; set; }

   :returns: The name of the file.
   :rtype: ``String``

Imports
~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Module.Imports

   Gets or sets the import types.

   .. code-block:: csharp

      public IList<Import> Imports { get; set; }

   :returns: The imports.
   :rtype: ``IList<Import>``

Name
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Module.Name

   Gets or sets the name.

   .. code-block:: csharp

      public string Name { get; set; }

   :returns: The name.
   :rtype: ``String``

Objects
~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Module.Objects

   Gets the objects.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public IList<IEntity> Objects { get; }

   :returns: The objects.
   :rtype: ``IList<IEntity>``

Traps
~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Module.Traps

   Gets the traps.

   .. code-block:: csharp

      [Obsolete("Please use Entities property to find TRAP-TYPE items.")]
      public IList<TrapTypeMacro> Traps { get; }

   :returns: The traps.
   :rtype: ``IList<TrapTypeMacro>``

