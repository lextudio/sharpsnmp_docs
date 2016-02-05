SharpSnmpPro.Mib Assembly Features
==================================

By `Lex Li`_

This page shows you the main features of SharpSnmpPro.Mib assembly.

.. contents:: In this article:
  :local:
  :depth: 1

Background
----------
#SNMP Suite ships with an assembly SharpSnmpLib.Mib which can compile MIB documents and extract some information from them. It only provides limited functionality and users ask for more advanced editions. Here it comes.

The Brand New SharpSnmpPro.Mib Assembly
---------------------------------------
This assembly is the key component that empowers the Compiler Pro product.

.. image:: _static/sharpsnmppro.mib.png

Supported Platforms
-------------------
Unlike the Compiler Pro which requires .NET 4.5 and Windows, this assembly can be used on multiple platforms,

* .NET Framework 4.5.2 and above
* Mono 4.2.1 and above
* Xamarin.iOS Unified
* Xamarin.Android
* Xamarin.Mac

Features
--------
Now let us see a few common examples that reveal the power of this library.

MIB Document Compilation
^^^^^^^^^^^^^^^^^^^^^^^^
The following code shows how to compile several essential MIB documents and load the metadata into memory,

.. code-block:: csharp

  var registry = new SimpleObjectRegistry();
  var collector = new ErrorRegistry();
  registry.Tree.Collector = collector;
  registry.Import(Parser.Compile(new MemoryStream(Resources.SNMPv2_SMI), collector));
  registry.Import(Parser.Compile(new MemoryStream(Resources.SNMPv2_CONF), collector));
  registry.Import(Parser.Compile(new MemoryStream(Resources.SNMPv2_TC), collector));
  registry.Import(Parser.Compile(new MemoryStream(Resources.SNMPv2_MIB), collector));
  registry.Import(Parser.Compile(new MemoryStream(Resources.SNMPv2_TM), collector));
  registry.Refresh();

``SimpleObjectRegistry`` is a class that holds metadata in memory. It can be used to import metadata generated via ``Parser.Compile``. 

``ErrorRegistry`` is the container of errors and warnings. When ``SimpleObjectRegistry.Refresh`` is called, all errors and warnings can be found 
in the ``ErrorRegistry`` instance, to help you identify why some MIB documents cannot be compiled or imported.

.. note:: The Trial version lacks of certain validation so it might not report all the issues, while the Full version does not have such limitations.

``SimpleObjectRegistry.Tree.PendingModules`` can be queried to see a list of modules that fail to be loaded.

Similarly, ``SimpleObjectRegistry.Tree.LoadedModules`` is a list of loaded modules.

Name/OID Translation
^^^^^^^^^^^^^^^^^^^^
Once the metadata are extracted from MIB documents, an obvious application of them is to enable OID translation. The translation is bi-directional 
(from names to OIDs or vice verse).

.. code-block:: csharp

  const string textual = "SNMPv2-SMI::zeroDotZero";
  var number = new uint[] { 0, 0 };
  Assert.AreEqual(textual, registry.Translate(number));
  Assert.AreEqual(number, registry.Translate(textual));

Here the ``Translate`` method only provides a single textual form of the OID, while in some cases a single OID can have many textual forms (as it 
might be defined in multiple documents with different modules and names). Below is the code to get all the textual forms of the OID,

.. code-block:: csharp

  var number = new uint[] { 0, 0 };
  var searchResult = registry.Tree.Search(number);
  var definition = searchResult.Definition;
  var textualForms = definition.TextualForms;

Extract Object Identifier Metadata
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Once all metadata are loaded in a ``SimpleObjectRegistry`` instance we can easily extract the information for individual objects,

.. code-block:: csharp

  Definition item = registry.Tree.Find("SNMPv2-MIB", "sysDescr");
  IEntity entity = item.DisplayEntity;
  Assert.AreEqual("A textual description of the entity.  This value should include the full name and version identification of the system's hardware type, software operating-system, and networking software.", entity.DescriptionFormatted());
  Assert.AreEqual(EntityStatus.Current, entity.Status);
  Assert.AreEqual(string.Empty, entity.Reference);

  var obj = entity as IObjectTypeMacro;
  Assert.AreEqual(Access.ReadOnly, obj.MibAccess);
  Assert.AreEqual(SnmpType.OctetString, obj.BaseSyntax);

We can see that if we are looking for ``SNMPv2-MIB::sysDescr`` (whose OID is ``1.3.6.1.2.1.1.1``), we can use ``SimpleObjectRegistry.Tree.Find`` method to locate the ``Definition`` instance. Each such instance contains one or 
more ``IEntity`` instances to match their entity definition in MIB documents.

From ``Definition.DisplayEntity`` we can get one of the entities, and check its properties such as ``IEntity.DescriptionFormatted``, ``IEntity.Status``, and ``IEntity.Reference``. 

Since ``SNMPv2-MIB::sysDescr`` is an ``OBJECT-TYPE`` macro entity, we can further cast it to ``IObjectTypeMacro`` to access more properties, such as ``IObjectTypeMacro.MibAccess`` and ``IObjectTypeMacro.BaseSyntax``. It is 
obvious that the data type of ``SNMPv2-MIB::sysDescr`` is ``OCTET STRING``.

There are of course other properties you can review, which are documented online at `the help site`_ . 

.. note:: The Trial version limits which attributes you can see, while the Full version does not have such limitations.

Table Validation
^^^^^^^^^^^^^^^^
With MIB documents, it is very easy to determine if an OID is a table, a table entry, or a table column.

.. code-block:: csharp

  var table = new ObjectIdentifier(new uint[] { 1, 3, 6, 1, 2, 1, 1, 9 });
  var entry = new ObjectIdentifier(new uint[] { 1, 3, 6, 1, 2, 1, 1, 9, 1 });
  var unknown = new ObjectIdentifier(new uint[] { 1, 3, 6, 8, 18579, 111111 });
  Assert.IsTrue(registry.ValidateTable(table));
  Assert.IsFalse(registry.ValidateTable(entry));
  Assert.IsFalse(registry.ValidateTable(unknown));

By accessing ``Children`` property of a table object, the entry of that table can be queries. 

Similarly, by accessing ``Children`` property of an entry object, the columns of the table can be queried easily.

Input Data Validation
^^^^^^^^^^^^^^^^^^^^^
In SNMP managers or agents, it is a common need to determine if a piece of data is valid for an OID. Various constraints can be defined at MIB document level, but it is often difficult to extract that from the files. With a 
few lines of code you can now do that

.. code-block:: csharp

  Assert.IsTrue(registry.Verify("SNMPv2-MIB", "sysDescr", new OctetString("test")));
  Assert.IsTrue(registry.Verify("SNMPv2-MIB", "sysDescr", new OctetString(string.Empty)));
  Assert.IsFalse(registry.Verify("SNMPv2-MIB", "sysDescr", new Integer32(2)));

We can easily test if the data is valid for ``SNMPv2-MIB::sysDescr``. 

.. note:: The Trial version does only support data validation against a limited set of default types (defined in core MIB documents), while the Full version supports even custom types such as ``BITS``, ``CiscoRowOperStatus``, and ``CiscoPort``.

.. _the help site: http://help.sharpsnmp.com

Related Resources
-----------------

- :doc:`/support/purchase`
- `Requesting Trial <http://sharpsnmp.com>`_
- :doc:`/getting-started/compiler-features`
- :doc:`/tutorials/assembly-trial-guide`
- :doc:`/tutorials/assembly-full-guide`
