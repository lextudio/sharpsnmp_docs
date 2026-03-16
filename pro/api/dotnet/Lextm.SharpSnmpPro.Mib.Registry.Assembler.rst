Assembler Class
===============

.. dn:class:: Lextm.SharpSnmpPro.Mib.Registry.Assembler

   MIB assembler which assembles MIB documents to an object tree.

   .. code-block:: csharp

      public class Assembler

**Namespace:** ``Lextm.SharpSnmpPro.Mib.Registry``

**Inheritance:** Object → ``Assembler``

Constructors
------------

Assembler(String)
~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.Registry.Assembler..ctor(System.String)

   Creates an instance of :dn:cls:``~Lextm.SharpSnmpPro.Mib.Registry.Assembler``.

   .. code-block:: csharp

      public Assembler(string folder)

   :param folder: Folder.
   :type folder: ``String``

Properties
----------

Folder
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Registry.Assembler.Folder

   Folder.

   .. code-block:: csharp

      public string Folder { get; }

   :rtype: ``String``

Tree
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Registry.Assembler.Tree

   Tree.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public ObjectTree Tree { get; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Registry.ObjectTree`

Methods
-------

Assemble(IEnumerable<Module>, ErrorRegistry)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Registry.Assembler.Assemble(System.Collections.Generic.IEnumerable{Lextm.SharpSnmpPro.Mib.Module},Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry)

   Assemblers modules.

   .. code-block:: csharp

      public void Assemble(IEnumerable<Module> modules, ErrorRegistry registry)

   :param modules: Modules.
   :type modules: ``IEnumerable<Module>``
   :param registry: Error registry.
   :type registry: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry`

Reload()
~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Registry.Assembler.Reload

   Drops all modules.

   .. code-block:: csharp

      public void Reload()

