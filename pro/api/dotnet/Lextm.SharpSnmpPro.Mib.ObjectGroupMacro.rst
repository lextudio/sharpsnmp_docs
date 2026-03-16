ObjectGroupMacro Class
======================

.. dn:class:: Lextm.SharpSnmpPro.Mib.ObjectGroupMacro

   Object group macro.

   .. code-block:: csharp

      public class ObjectGroupMacro : ISmiType, IEntity, IConstruct, IValidatable

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``ObjectGroupMacro``

Properties
----------

CharPositionInLine
~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectGroupMacro.CharPositionInLine

   Gets the char position in line.

   .. code-block:: csharp

      public int CharPositionInLine { get; set; }

   :returns: The char position in line.
   :rtype: ``Int32``

Description
~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectGroupMacro.Description

   Provides a textual description of the item being defined.

   .. code-block:: csharp

      public string Description { get; }

   :rtype: ``String``

Line
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectGroupMacro.Line

   Gets the line number.

   .. code-block:: csharp

      public int Line { get; set; }

   :returns: The line.
   :rtype: ``Int32``

Module
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectGroupMacro.Module

   Gets or sets the module.

   .. code-block:: csharp

      public Module Module { get; set; }

   :returns: The module.
   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Module`

ModuleName
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectGroupMacro.ModuleName

   Gets or sets the name of the module.

   .. code-block:: csharp

      public string ModuleName { get; set; }

   :returns: The name of the module.
   :rtype: ``String``

Name
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectGroupMacro.Name

   Name.

   .. code-block:: csharp

      public string Name { get; set; }

   :rtype: ``String``

ObjectIdentifier
~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectGroupMacro.ObjectIdentifier

   Gets or sets the object identifier.

   .. code-block:: csharp

      [CLSCompliant(false)]
      [Obsolete("Please use GetObjectIdentifier method.")]
      public uint[] ObjectIdentifier { get; set; }

   :returns: The object identifier.
   :rtype: ``UInt32[]``

Objects
~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectGroupMacro.Objects

   Gets the objects.

   .. code-block:: csharp

      public IList<ISmiValue> Objects { get; }

   :returns: The objects.
   :rtype: ``IList<ISmiValue>``

Parent
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectGroupMacro.Parent

   Gets or sets the parent.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public IEntity Parent { get; set; }

   :returns: The parent.
   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.IEntity`

Reference
~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectGroupMacro.Reference

   Specifies the source of the definition (such as a document from another standards organization, or an architectural document for a proprietary system).

   .. code-block:: csharp

      public string Reference { get; }

   :rtype: ``String``

Status
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectGroupMacro.Status

   Gets or sets the status.

   .. code-block:: csharp

      public EntityStatus Status { get; set; }

   :returns: The status.
   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.EntityStatus`

Value
~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectGroupMacro.Value

   Gets or sets the value.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public uint Value { get; set; }

   :returns: The value.
   :rtype: ``UInt32``

Values
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectGroupMacro.Values

   Gets or sets the list of ID components.

   .. code-block:: csharp

      public IdComponentList Values { get; set; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.IdComponentList`

Verified
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectGroupMacro.Verified

   Gets or sets the verification status of an entity.

   .. code-block:: csharp

      public VerificationStatus Verified { get; set; }

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.VerificationStatus`

Methods
-------

Append(StringBuilder)
~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.ObjectGroupMacro.Append(System.Text.StringBuilder)

   Appends the type name to the provided ``StringBuilder``.

   .. code-block:: csharp

      public void Append(StringBuilder typeName)

   :param typeName: The ``StringBuilder`` to append the type name to.
   :type typeName: ``StringBuilder``

Validate(ICollection<IConstruct>, ErrorRegistry)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.ObjectGroupMacro.Validate(System.Collections.Generic.ICollection{Lextm.SharpSnmpPro.Mib.IConstruct},Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry)

   Validates this entity.

   .. code-block:: csharp

      public void Validate(ICollection<IConstruct> knownConstructs, ErrorRegistry registry)

   :param knownConstructs: Known constructs.
   :type knownConstructs: ``ICollection<IConstruct>``
   :param registry: The registry.
   :type registry: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry`

