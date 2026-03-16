Document Class
==============

.. dn:class:: Lextm.SharpSnmpPro.Mib.Document

   MIB document.

   .. code-block:: csharp

      public class Document

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``Document``

Properties
----------

FileName
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Document.FileName

   Gets or sets the name of the file.

   .. code-block:: csharp

      public string FileName { get; set; }

   :returns: The name of the file.
   :rtype: ``String``

Modules
~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Document.Modules

   Gets the modules.

   .. code-block:: csharp

      public IList<Module> Modules { get; }

   :returns: The modules.
   :rtype: ``IList<Module>``

