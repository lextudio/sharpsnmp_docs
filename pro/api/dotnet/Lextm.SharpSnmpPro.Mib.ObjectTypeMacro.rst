ObjectTypeMacro Class
=====================

.. dn:class:: Lextm.SharpSnmpPro.Mib.ObjectTypeMacro

   Object type macro.

   .. code-block:: csharp

      public class ObjectTypeMacro : ISmiType, IEntity, IConstruct, IValidatable, IObjectTypeMacro

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``ObjectTypeMacro``

Properties
----------

Augments
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectTypeMacro.Augments

   Gets or sets the augments.

   .. code-block:: csharp

      public Augments Augments { get; set; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Augments`

CharPositionInLine
~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectTypeMacro.CharPositionInLine

   Gets the char position in line.

   .. code-block:: csharp

      public int CharPositionInLine { get; set; }

   :returns: The char position in line.
   :rtype: ``Int32``

DefaultValue
~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectTypeMacro.DefaultValue

   Gets or sets the default value.

   .. code-block:: csharp

      public ISmiValue DefaultValue { get; set; }

   :returns: The default value.
   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiValue`

DefaultValueBits
~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectTypeMacro.DefaultValueBits

   Gets or sets the default value bits.

   .. code-block:: csharp

      public IList<string> DefaultValueBits { get; }

   :returns: The default value bits.
   :rtype: ``IList<String>``

Description
~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectTypeMacro.Description

   Provides a textual description of the item being defined.

   .. code-block:: csharp

      public string Description { get; }

   :rtype: ``String``

Entry
~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectTypeMacro.Entry

   Gets or sets the entry.

   .. code-block:: csharp

      public ObjectTypeMacro Entry { get; }

   :returns: The entry.
   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.ObjectTypeMacro`

IndexList
~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectTypeMacro.IndexList

   Gets or sets the index list.

   .. code-block:: csharp

      public IList<Index> IndexList { get; }

   :returns: The index list.
   :rtype: ``IList<Index>``

InstallErrors
~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectTypeMacro.InstallErrors

   Gets or sets the install errors.

   .. code-block:: csharp

      public IList<NamedBit> InstallErrors { get; }

   :returns: The install errors.
   :rtype: ``IList<NamedBit>``

Line
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectTypeMacro.Line

   Gets the line number.

   .. code-block:: csharp

      public int Line { get; set; }

   :returns: The line.
   :rtype: ``Int32``

MibAccess
~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectTypeMacro.MibAccess

   Gets or sets the mib access.

   .. code-block:: csharp

      public Access MibAccess { get; set; }

   :returns: The mib access.
   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Access`

MibAugments
~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectTypeMacro.MibAugments

   Gets or sets the mib augments.

   .. code-block:: csharp

      [Obsolete("Please use Augments property instead.")]
      public ISmiValue MibAugments { get; set; }

   :returns: The mib augments.
   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiValue`

MibIndex
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectTypeMacro.MibIndex

   Gets or sets the index of the mib.

   .. code-block:: csharp

      [Obsolete("Please use IndexList property instead.")]
      public IList<ISmiValue> MibIndex { get; }

   :returns: The index of the mib.
   :rtype: ``IList<ISmiValue>``

Module
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectTypeMacro.Module

   Gets or sets the module.

   .. code-block:: csharp

      public Module Module { get; set; }

   :returns: The module.
   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Module`

ModuleName
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectTypeMacro.ModuleName

   Gets or sets the name of the module.

   .. code-block:: csharp

      public string ModuleName { get; set; }

   :returns: The name of the module.
   :rtype: ``String``

Name
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectTypeMacro.Name

   Name.

   .. code-block:: csharp

      public string Name { get; set; }

   :rtype: ``String``

ObjectIdentifier
~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectTypeMacro.ObjectIdentifier

   Gets or sets the object identifier.

   .. code-block:: csharp

      [CLSCompliant(false)]
      [Obsolete("Please use GetObjectIdentifier method.")]
      public uint[] ObjectIdentifier { get; set; }

   :returns: The object identifier.
   :rtype: ``UInt32[]``

Parent
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectTypeMacro.Parent

   Gets or sets the parent.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public IEntity Parent { get; set; }

   :returns: The parent.
   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.IEntity`

PibAccess
~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectTypeMacro.PibAccess

   Gets or sets the pib access.

   .. code-block:: csharp

      public PibAccess PibAccess { get; set; }

   :returns: The pib access.
   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.PibAccess`

PibExtends
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectTypeMacro.PibExtends

   Gets or sets the pib extends.

   .. code-block:: csharp

      public ISmiValue PibExtends { get; set; }

   :returns: The pib extends.
   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiValue`

PibIndex
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectTypeMacro.PibIndex

   Gets or sets the index of the pib.

   .. code-block:: csharp

      public ISmiValue PibIndex { get; set; }

   :returns: The index of the pib.
   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiValue`

PibReference
~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectTypeMacro.PibReference

   Gets or sets the pib reference.

   .. code-block:: csharp

      public ISmiValue PibReference { get; set; }

   :returns: The pib reference.
   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiValue`

PibTag
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectTypeMacro.PibTag

   Gets or sets the pib tag.

   .. code-block:: csharp

      public ISmiValue PibTag { get; set; }

   :returns: The pib tag.
   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiValue`

Reference
~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectTypeMacro.Reference

   Specifies the source of the definition (such as a document from another standards organization, or an architectural document for a proprietary system).

   .. code-block:: csharp

      public string Reference { get; }

   :rtype: ``String``

ResolvedSyntax
~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectTypeMacro.ResolvedSyntax

   Gets the resolved syntax.

   .. code-block:: csharp

      public ISmiType ResolvedSyntax { get; }

   :returns: The resolved syntax.
   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiType`

SmiVersion
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectTypeMacro.SmiVersion

   Gets or sets the type of the access.

   .. code-block:: csharp

      public SmiVersion SmiVersion { get; set; }

   :returns: The type of the access.
   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.SmiVersion`

Status
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectTypeMacro.Status

   Gets or sets the status.

   .. code-block:: csharp

      public EntityStatus Status { get; set; }

   :returns: The status.
   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.EntityStatus`

Syntax
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectTypeMacro.Syntax

   Gets or sets the syntax.

   .. code-block:: csharp

      public ISmiType Syntax { get; }

   :returns: The syntax.
   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiType`

Type
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectTypeMacro.Type

   Gets or sets the type.

   .. code-block:: csharp

      public DefinitionType Type { get; }

   :returns: The type.
   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.DefinitionType`

UniquenessValues
~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectTypeMacro.UniquenessValues

   Gets or sets the uniqueness values.

   .. code-block:: csharp

      public IList<ISmiValue> UniquenessValues { get; }

   :returns: The uniqueness values.
   :rtype: ``IList<ISmiValue>``

Units
~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectTypeMacro.Units

   Gets or sets the units.

   .. code-block:: csharp

      public string Units { get; set; }

   :returns: The units.
   :rtype: ``String``

Value
~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectTypeMacro.Value

   Gets or sets the value.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public uint Value { get; set; }

   :returns: The value.
   :rtype: ``UInt32``

Values
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectTypeMacro.Values

   Gets or sets the list of ID components.

   .. code-block:: csharp

      public IdComponentList Values { get; set; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.IdComponentList`

Verified
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectTypeMacro.Verified

   Gets or sets the verification status of an entity.

   .. code-block:: csharp

      public VerificationStatus Verified { get; set; }

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.VerificationStatus`

Methods
-------

Append(StringBuilder)
~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.ObjectTypeMacro.Append(System.Text.StringBuilder)

   Appends the type name to the provided ``StringBuilder``.

   .. code-block:: csharp

      public void Append(StringBuilder typeName)

   :param typeName: The ``StringBuilder`` to append the type name to.
   :type typeName: ``StringBuilder``

Validate(ICollection<IConstruct>, ErrorRegistry)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.ObjectTypeMacro.Validate(System.Collections.Generic.ICollection{Lextm.SharpSnmpPro.Mib.IConstruct},Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry)

   Validates this entity.

   .. code-block:: csharp

      public void Validate(ICollection<IConstruct> knownConstructs, ErrorRegistry registry)

   :param knownConstructs: Known constructs.
   :type knownConstructs: ``ICollection<IConstruct>``
   :param registry: The registry.
   :type registry: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry`

