SharpSnmpPro.Mib Assembly Features
==================================

This page provides an overview of the main features of the
``SharpSnmpPro.Mib`` assembly.

Background
----------
Our legacy product, #SNMP Suite, used to ship with an assembly called
``SharpSnmpLib.Mib``. However, that assembly only provided limited
functionality, and power users requested more advanced features. As a result,
we developed a new assembly called ``SharpSnmpPro.Mib``.

The Brand New SharpSnmpPro.Mib Assembly
---------------------------------------
The ``SharpSnmpPro.Mib`` assembly is a key component that empowers our Compiler
Pro product.

.. image:: _static/sharpsnmppro.mib.png
    :alt: SharpSnmpPro.Mib Assembly
    :align: center

Supported Platforms
-------------------
Unlike the Compiler Pro, which requires .NET 4.7.1 and Windows, the
``SharpSnmpPro.Mib`` assembly can be used on multiple platforms, including:

- .NET 6 and 8
- .NET Framework 4.7.1 and above
- Other platforms compliant with .NET Standard 2.0.

Features
--------
Let's explore some examples that demonstrate the power of this library.

MIB Document Compilation
^^^^^^^^^^^^^^^^^^^^^^^^
The following code demonstrates how to compile multiple MIB documents and load
their metadata into memory:

.. code-block:: csharp

  var registry = new SimpleObjectRegistry();
  var collector = new ErrorRegistry();
  registry.Tree.Collector = collector;
  registry.Import(Parser.Compile(new MemoryStream(Resources.SNMPv2_SMI),
                                collector));
  registry.Import(Parser.Compile(new MemoryStream(Resources.SNMPv2_CONF),
                                collector));
  registry.Import(Parser.Compile(new MemoryStream(Resources.SNMPv2_TC),
                                collector));
  registry.Import(Parser.Compile(new MemoryStream(Resources.SNMPv2_MIB),
                                collector));
  registry.Import(Parser.Compile(new MemoryStream(Resources.SNMPv2_TM),
                                collector));
  registry.Refresh()

The ``SimpleObjectRegistry`` class holds the metadata in memory and can import
metadata generated via the ``Parser.Compile`` method.

The ``ErrorRegistry`` container stores errors and warnings. After calling
``SimpleObjectRegistry.Refresh``, you can find all errors and warnings in the
``ErrorRegistry`` instance, helping you identify why some MIB documents cannot
be compiled or imported.

.. note::

   The Trial version may not report all issues due to certain limitations,
   while the Full version does not have such limitations.

You can query ``SimpleObjectRegistry.Tree.PendingModules`` to see a list of
modules that failed to load, and ``SimpleObjectRegistry.Tree.LoadedModules``
for a list of loaded modules.

Name/OID Translation
^^^^^^^^^^^^^^^^^^^^
Once the metadata is extracted from MIB documents, you can use it to enable OID
translation. The translation is bi-directional, allowing you to convert between
names and OIDs.

.. code-block:: csharp

  const string textual = "SNMPv2-SMI::zeroDotZero";
  var number = new uint[] { 0, 0 };
  Assert.AreEqual(textual, registry.Translate(number));
  Assert.AreEqual(number, registry.Translate(textual));

The ``Translate`` method provides a single textual form of the OID. In some
cases, a single OID can have multiple textual forms, as it might be defined in
multiple documents with different modules and names. To retrieve all the textual
forms of an OID, you can use the following code:

.. code-block:: csharp

  var number = new uint[] { 0, 0 };
  var searchResult = registry.Tree.Search(number);
  var definition = searchResult.Definition;
  var textualForms = definition.TextualForms;

Extract Object Identifier Metadata
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Once all the metadata is loaded in a ``SimpleObjectRegistry`` instance, you can
easily extract information for individual objects:

.. code-block:: csharp

  Definition item = registry.Tree.Find("SNMPv2-MIB", "sysDescr");
  IEntity entity = item.DisplayEntity;
  Assert.AreEqual("A textual description of the entity.  This value should include the full name and version identification of the system's hardware type, software operating-system, and networking software.", entity.DescriptionFormatted());
  Assert.AreEqual(EntityStatus.Current, entity.Status);
  Assert.AreEqual(string.Empty, entity.Reference);

  var obj = entity as IObjectTypeMacro;
  Assert.AreEqual(Access.ReadOnly, obj.MibAccess);
  Assert.AreEqual(SnmpType.OctetString, obj.BaseSyntax);

By using the ``SimpleObjectRegistry.Tree.Find`` method, you can locate a
``Definition`` instance for a specific OID, such as ``SNMPv2-MIB::sysDescr``
(OID: ``1.3.6.1.2.1.1.1``). Each ``Definition`` instance contains one or more
``IEntity`` instances that match their entity definition in MIB documents.

From the ``Definition.DisplayEntity`` property, you can access various
properties of the entity, such as ``IEntity.DescriptionFormatted``,
``IEntity.Status``, and ``IEntity.Reference``.

If the entity is an ``OBJECT-TYPE`` macro, you can cast it to
``IObjectTypeMacro`` to access additional properties, such as
``IObjectTypeMacro.MibAccess`` and ``IObjectTypeMacro.BaseSyntax``. In the case
of ``SNMPv2-MIB::sysDescr``, the data type is ``OCTET STRING``.

There are other properties you can review, which are documented in the `API
reference`_.

.. note::

   The Trial version has limitations on which attributes you can see, while the
   Full version does not have such limitations.

Table Validation
^^^^^^^^^^^^^^^^
With MIB documents, it is easy to determine if an OID represents a table, a
table entry, or a table column.

.. code-block:: csharp

  var table = new ObjectIdentifier(new uint[] { 1, 3, 6, 1, 2, 1, 1, 9 });
  var entry = new ObjectIdentifier(new uint[] { 1, 3, 6, 1, 2, 1, 1, 9, 1 });
  var unknown = new ObjectIdentifier(new uint[] { 1, 3, 6, 8, 18579, 111111 });
  Assert.IsTrue(registry.ValidateTable(table));
  Assert.IsFalse(registry.ValidateTable(entry));
  Assert.IsFalse(registry.ValidateTable(unknown));

By accessing the ``Children`` property of a table object, you can query the
entries of that table. Similarly, by accessing the ``Children`` property of an
entry object, you can query the columns of the table.

Input Data Validation
^^^^^^^^^^^^^^^^^^^^^
In SNMP managers or agents, it is common to validate whether a piece of data is
valid for an OID. MIB documents define various constraints, but extracting them
from the files can be challenging. With a few lines of code, you can now perform
data validation:

.. code-block:: csharp

  Assert.IsTrue(registry.Verify("SNMPv2-MIB", "sysDescr", new OctetString("test")));
  Assert.IsTrue(registry.Verify("SNMPv2-MIB", "sysDescr", new OctetString(string.Empty)));
  Assert.IsFalse(registry.Verify("SNMPv2-MIB", "sysDescr", new Integer32(2)));

You can easily test if the data is valid for ``SNMPv2-MIB::sysDescr``.

.. note::
  
   The Trial version only supports data validation against a limited set of
   default types (defined in core MIB documents), while the Full version
   supports custom types such as ``BITS``, ``CiscoRowOperStatus``, and
   ``CiscoPort``.

.. _API reference: https://help.sharpsnmp.com

Related Resources
-----------------

- :doc:`/support/purchase`
- `API Documentation <https://help.sharpsnmp.com>`_
- `Requesting a Trial <https://www.sharpsnmp.com/#contact-us>`_
- :doc:`/getting-started/compiler-features`
- :doc:`/tutorials/assembly-trial-guide`
- :doc:`/tutorials/assembly-full-guide`
