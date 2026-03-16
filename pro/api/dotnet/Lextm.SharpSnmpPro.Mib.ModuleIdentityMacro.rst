ModuleIdentityMacro Class
=========================

.. dn:class:: Lextm.SharpSnmpPro.Mib.ModuleIdentityMacro

   Represents the MODULE-IDENTITY macro in a MIB module.

   .. code-block:: csharp

      public class ModuleIdentityMacro : ISmiType, IEntity, IConstruct, IValidatable

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``ModuleIdentityMacro``

Constructors
------------

ModuleIdentityMacro()
~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.ModuleIdentityMacro..ctor

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.ModuleIdentityMacro`` class.

   .. code-block:: csharp

      public ModuleIdentityMacro()

Properties
----------

Categories
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ModuleIdentityMacro.Categories

   Gets or sets the categories for this module identity.

   .. code-block:: csharp

      public Categories Categories { get; set; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Categories`

CharPositionInLine
~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ModuleIdentityMacro.CharPositionInLine

   Gets the char position in line.

   .. code-block:: csharp

      public int CharPositionInLine { get; set; }

   :returns: The char position in line.
   :rtype: ``Int32``

ContactInfo
~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ModuleIdentityMacro.ContactInfo

   Gets or sets the contact information string.

   .. code-block:: csharp

      public string ContactInfo { get; set; }

   :rtype: ``String``

Description
~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ModuleIdentityMacro.Description

   Gets the description.

   .. code-block:: csharp

      public string Description { get; }

   :rtype: ``String``

LastUpdate
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ModuleIdentityMacro.LastUpdate

   Gets or sets the last update string.

   .. code-block:: csharp

      public string LastUpdate { get; set; }

   :rtype: ``String``

Line
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ModuleIdentityMacro.Line

   Gets the line number.

   .. code-block:: csharp

      public int Line { get; set; }

   :returns: The line.
   :rtype: ``Int32``

Module
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ModuleIdentityMacro.Module

   Gets or sets the module.

   .. code-block:: csharp

      public Module Module { get; set; }

   :returns: The module.
   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Module`

ModuleName
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ModuleIdentityMacro.ModuleName

   Gets or sets the module name.

   .. code-block:: csharp

      public string ModuleName { get; set; }

   :rtype: ``String``

Name
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ModuleIdentityMacro.Name

   Name.

   .. code-block:: csharp

      public string Name { get; set; }

   :rtype: ``String``

ObjectIdentifier
~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ModuleIdentityMacro.ObjectIdentifier

   Gets or sets the object identifier.

   .. code-block:: csharp

      [CLSCompliant(false)]
      [Obsolete("Please use GetObjectIdentifier method.")]
      public uint[] ObjectIdentifier { get; set; }

   :returns: The object identifier.
   :rtype: ``UInt32[]``

Organization
~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ModuleIdentityMacro.Organization

   Gets or sets the organization string.

   .. code-block:: csharp

      public string Organization { get; set; }

   :rtype: ``String``

Parent
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ModuleIdentityMacro.Parent

   Gets or sets the parent.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public IEntity Parent { get; set; }

   :returns: The parent.
   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.IEntity`

Reference
~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ModuleIdentityMacro.Reference

   Specifies the source of the definition (such as a document from another standards organization, or an architectural document for a proprietary system).

   .. code-block:: csharp

      public string Reference { get; }

   :rtype: ``String``

Revisions
~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ModuleIdentityMacro.Revisions

   Gets or sets the list of revisions.

   .. code-block:: csharp

      public IList<Revision> Revisions { get; set; }

   :rtype: ``IList<Revision>``

Status
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ModuleIdentityMacro.Status

   Status.

   .. code-block:: csharp

      public EntityStatus Status { get; }

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.EntityStatus`

Value
~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ModuleIdentityMacro.Value

   Gets or sets the value.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public uint Value { get; set; }

   :returns: The value.
   :rtype: ``UInt32``

Values
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ModuleIdentityMacro.Values

   Gets or sets the list of ID components.

   .. code-block:: csharp

      public IdComponentList Values { get; set; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.IdComponentList`

Verified
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ModuleIdentityMacro.Verified

   Gets or sets the verification status of an entity.

   .. code-block:: csharp

      public VerificationStatus Verified { get; set; }

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.VerificationStatus`

Methods
-------

Append(StringBuilder)
~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.ModuleIdentityMacro.Append(System.Text.StringBuilder)

   Appends the type name to the provided ``StringBuilder``.

   .. code-block:: csharp

      public void Append(StringBuilder typeName)

   :param typeName: The ``StringBuilder`` to append the type name to.
   :type typeName: ``StringBuilder``

Validate(ICollection<IConstruct>, ErrorRegistry)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.ModuleIdentityMacro.Validate(System.Collections.Generic.ICollection{Lextm.SharpSnmpPro.Mib.IConstruct},Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry)

   Validates this entity.

   .. code-block:: csharp

      public void Validate(ICollection<IConstruct> knownConstructs, ErrorRegistry registry)

   :param knownConstructs: Known constructs.
   :type knownConstructs: ``ICollection<IConstruct>``
   :param registry: The registry.
   :type registry: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry`

