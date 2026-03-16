ObjectRegistryBase Class
========================

.. dn:class:: Lextm.SharpSnmpPro.Mib.Registry.ObjectRegistryBase

   Base class of object registry.

   .. code-block:: csharp

      public abstract class ObjectRegistryBase

**Namespace:** ``Lextm.SharpSnmpPro.Mib.Registry``

**Inheritance:** Object → ``ObjectRegistryBase``

Properties
----------

Tree
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Registry.ObjectRegistryBase.Tree

   Object tree.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public ObjectTree Tree { get; protected set; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Registry.ObjectTree`

Methods
-------

CreateVariable(String, IAsnSerializable)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Registry.ObjectRegistryBase.CreateVariable(System.String,DotNetSnmp.Asn1.Serialization.IAsnSerializable)

   Creates a variable.

   .. code-block:: csharp

      public Variable CreateVariable(string textual, IAsnSerializable data)

   :param textual: The textual ID.
   :type textual: ``String``
   :param data: The data.
   :type data: :any:`IAsnSerializable <DotNetSnmp.Asn1.Serialization.IAsnSerializable>`

   :rtype: :any:`Variable <DotNetSnmp.Asn1.SyntaxObjects.Variable>`

CreateVariable(String)
~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Registry.ObjectRegistryBase.CreateVariable(System.String)

   Creates a variable.

   .. code-block:: csharp

      public Variable CreateVariable(string textual)

   :param textual: The textual.
   :type textual: ``String``

   :rtype: :any:`Variable <DotNetSnmp.Asn1.SyntaxObjects.Variable>`

Decode(ObjectIdentifier, IAsnSerializable)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Registry.ObjectRegistryBase.Decode(DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,DotNetSnmp.Asn1.Serialization.IAsnSerializable)

   Decodes the data against the object identifier.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public string Decode(ObjectIdentifier oid, IAsnSerializable data)

   :param oid: The object identifier.
   :type oid: :any:`ObjectIdentifier <DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier>`
   :param data: The data.
   :type data: :any:`IAsnSerializable <DotNetSnmp.Asn1.Serialization.IAsnSerializable>`

   :rtype: ``String``

Decode(String, String, IAsnSerializable)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Registry.ObjectRegistryBase.Decode(System.String,System.String,DotNetSnmp.Asn1.Serialization.IAsnSerializable)

   Decodes the data against the object name in specified module.

   .. code-block:: csharp

      public string Decode(string module, string name, IAsnSerializable data)

   :param module: The module.
   :type module: ``String``
   :param name: The name.
   :type name: ``String``
   :param data: The data.
   :type data: :any:`IAsnSerializable <DotNetSnmp.Asn1.Serialization.IAsnSerializable>`

   :rtype: ``String``

Decode(UInt32[], IAsnSerializable)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Registry.ObjectRegistryBase.Decode(System.UInt32[],DotNetSnmp.Asn1.Serialization.IAsnSerializable)

   Decodes the data against the object identifier.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public string Decode(uint[] oid, IAsnSerializable data)

   :param oid: The object identifier.
   :type oid: ``UInt32[]``
   :param data: The data.
   :type data: :any:`IAsnSerializable <DotNetSnmp.Asn1.Serialization.IAsnSerializable>`

   :rtype: ``String``

Import(IEnumerable<Module>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Registry.ObjectRegistryBase.Import(System.Collections.Generic.IEnumerable{Lextm.SharpSnmpPro.Mib.Module})

   Imports instances of :dn:cls:``~Lextm.SharpSnmpPro.Mib.Module``.

   .. code-block:: csharp

      public ObjectRegistryBase Import(IEnumerable<Module> modules)

   :param modules: Modules.
   :type modules: ``IEnumerable<Module>``

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Registry.ObjectRegistryBase`

Refresh()
~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Registry.ObjectRegistryBase.Refresh

   Refreshes.

   .. code-block:: csharp

      public ObjectRegistryBase Refresh()

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Registry.ObjectRegistryBase`

Translate(String, String)
~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Registry.ObjectRegistryBase.Translate(System.String,System.String)

   Gets numerical form from textual form.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public uint[] Translate(string moduleName, string name)

   :param moduleName: Module name
   :type moduleName: ``String``
   :param name: Object name
   :type name: ``String``

   :rtype: ``UInt32[]``

Translate(String)
~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Registry.ObjectRegistryBase.Translate(System.String)

   Gets numerical form from textual form.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public uint[] Translate(string textual)

   :param textual: Textual
   :type textual: ``String``

   :rtype: ``UInt32[]``

Translate(UInt32[])
~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Registry.ObjectRegistryBase.Translate(System.UInt32[])

   Gets textual form from numerical form.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public string Translate(uint[] numerical)

   :param numerical: Numerical form
   :type numerical: ``UInt32[]``

   :rtype: ``String``

ValidateTable(ObjectIdentifier)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Registry.ObjectRegistryBase.ValidateTable(DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier)

   Validates if an is a table.

   .. code-block:: csharp

      public bool ValidateTable(ObjectIdentifier identifier)

   :param identifier: The object identifier.
   :type identifier: :any:`ObjectIdentifier <DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier>`

   :rtype: ``Boolean``

Verify(ObjectIdentifier, IAsnSerializable)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Registry.ObjectRegistryBase.Verify(DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,DotNetSnmp.Asn1.Serialization.IAsnSerializable)

   Verifies the data against the object identifier.

   .. code-block:: csharp

      public bool Verify(ObjectIdentifier oid, IAsnSerializable data)

   :param oid: The object identifier.
   :type oid: :any:`ObjectIdentifier <DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier>`
   :param data: The data.
   :type data: :any:`IAsnSerializable <DotNetSnmp.Asn1.Serialization.IAsnSerializable>`

   :rtype: ``Boolean``

Verify(String, String, IAsnSerializable)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Registry.ObjectRegistryBase.Verify(System.String,System.String,DotNetSnmp.Asn1.Serialization.IAsnSerializable)

   Verifies the data against the object name defined in specified module.

   .. code-block:: csharp

      public bool Verify(string module, string name, IAsnSerializable data)

   :param module: The module.
   :type module: ``String``
   :param name: The name.
   :type name: ``String``
   :param data: The data.
   :type data: :any:`IAsnSerializable <DotNetSnmp.Asn1.Serialization.IAsnSerializable>`

   :rtype: ``Boolean``

Events
------

OnChanged
~~~~~~~~~

.. dn:event:: Lextm.SharpSnmpPro.Mib.Registry.ObjectRegistryBase.OnChanged

   This event occurs when new documents are loaded.

   .. code-block:: csharp

      public event EventHandler<EventArgs> OnChanged

   :rtype: ``EventHandler<EventArgs>``

