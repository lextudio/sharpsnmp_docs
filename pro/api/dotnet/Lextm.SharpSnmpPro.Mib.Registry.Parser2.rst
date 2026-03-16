Parser2 Class
=============

.. dn:class:: Lextm.SharpSnmpPro.Mib.Registry.Parser2

   Parser, a high level class that embeds compiler functionality.

   .. code-block:: csharp

      public static class Parser2

**Namespace:** ``Lextm.SharpSnmpPro.Mib.Registry``

**Inheritance:** Object → ``Parser2``

Methods
-------

Compile(Stream, ErrorRegistry, String)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Registry.Parser2.Compile(System.IO.Stream,Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry,System.String)

   Loads a MIB file.

   .. code-block:: csharp

      public static IEnumerable<Module> Compile(Stream stream, ErrorRegistry registry, string fileName = "")

   :param stream: The stream.
   :type stream: ``Stream``
   :param registry: The registry.
   :type registry: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry`
   :param fileName: The file name (default value is empty).
   :type fileName: ``String``

   :rtype: ``IEnumerable<Module>``

Compile(String, ErrorRegistry)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Registry.Parser2.Compile(System.String,Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry)

   Loads a MIB file.

   .. code-block:: csharp

      public static IEnumerable<Module> Compile(string fileName, ErrorRegistry registry)

   :param fileName: File name.
   :type fileName: ``String``
   :param registry: The registry.
   :type registry: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry`

   :rtype: ``IEnumerable<Module>``

