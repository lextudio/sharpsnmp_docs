ObjectIdentityMacro Class
=========================

.. dn:class:: Lextm.SharpSnmpPro.Mib.ObjectIdentityMacro

   Represents the OBJECT-IDENTITY macro in a MIB module.

   .. code-block:: csharp

      public class ObjectIdentityMacro : IEntity, IValidatable, IBasicType, ISmiType, IConstruct

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``ObjectIdentityMacro``

Constructors
------------

ObjectIdentityMacro()
~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.ObjectIdentityMacro..ctor

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.ObjectIdentityMacro`` class.

   .. code-block:: csharp

      public ObjectIdentityMacro()

ObjectIdentityMacro(EntityStatus, String)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.ObjectIdentityMacro..ctor(Lextm.SharpSnmpPro.Mib.EntityStatus,System.String)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.ObjectIdentityMacro`` class with the specified status and description.

   .. code-block:: csharp

      public ObjectIdentityMacro(EntityStatus status, string description)

   :param status: The status of the entity.
   :type status: :dn:enum:`~Lextm.SharpSnmpPro.Mib.EntityStatus`
   :param description: The description of the object identity.
   :type description: ``String``

ObjectIdentityMacro(String, String, IEntity, UInt32, Boolean)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.ObjectIdentityMacro..ctor(System.String,System.String,Lextm.SharpSnmpPro.Mib.IEntity,System.UInt32,System.Boolean)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.ObjectIdentityMacro`` class with the specified module name, name, parent, value, and lock module flag.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public ObjectIdentityMacro(string moduleName, string name, IEntity parent, uint value, bool lockModule = false)

   :param moduleName: The name of the module.
   :type moduleName: ``String``
   :param name: The name of the object identity.
   :type name: ``String``
   :param parent: The parent entity.
   :type parent: :dn:iface:`~Lextm.SharpSnmpPro.Mib.IEntity`
   :param value: The value of the object identity.
   :type value: ``UInt32``
   :param lockModule: Whether to lock the module assignment.
   :type lockModule: ``Boolean``

Properties
----------

CharPositionInLine
~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectIdentityMacro.CharPositionInLine

   Gets the char position in line.

   .. code-block:: csharp

      public int CharPositionInLine { get; set; }

   :returns: The char position in line.
   :rtype: ``Int32``

Description
~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectIdentityMacro.Description

   Gets or sets the description of the object identity.

   .. code-block:: csharp

      public string Description { get; }

   :rtype: ``String``

Line
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectIdentityMacro.Line

   Gets the line number.

   .. code-block:: csharp

      public int Line { get; set; }

   :returns: The line.
   :rtype: ``Int32``

Module
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectIdentityMacro.Module

   Gets or sets the module to which this object identity belongs.

   .. code-block:: csharp

      public Module Module { get; set; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Module`

ModuleName
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectIdentityMacro.ModuleName

   Gets or sets the name of the module.

   .. code-block:: csharp

      public string ModuleName { get; set; }

   :rtype: ``String``

Name
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectIdentityMacro.Name

   Name.

   .. code-block:: csharp

      public string Name { get; set; }

   :rtype: ``String``

ObjectIdentifier
~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectIdentityMacro.ObjectIdentifier

   Gets or sets the object identifier.

   .. code-block:: csharp

      [CLSCompliant(false)]
      [Obsolete("Please use GetObjectIdentifier method.")]
      public uint[] ObjectIdentifier { get; set; }

   :returns: The object identifier.
   :rtype: ``UInt32[]``

Parent
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectIdentityMacro.Parent

   Gets or sets the parent.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public IEntity Parent { get; set; }

   :returns: The parent.
   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.IEntity`

Reference
~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectIdentityMacro.Reference

   Gets or sets the reference for the object identity.

   .. code-block:: csharp

      public string Reference { get; }

   :rtype: ``String``

Status
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectIdentityMacro.Status

   Status.

   .. code-block:: csharp

      public EntityStatus Status { get; set; }

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.EntityStatus`

Value
~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectIdentityMacro.Value

   Gets or sets the value.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public uint Value { get; set; }

   :returns: The value.
   :rtype: ``UInt32``

Values
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectIdentityMacro.Values

   Gets or sets the list of ID components.

   .. code-block:: csharp

      public IdComponentList Values { get; set; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.IdComponentList`

Verified
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ObjectIdentityMacro.Verified

   Gets or sets the verification status of an entity.

   .. code-block:: csharp

      public VerificationStatus Verified { get; set; }

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.VerificationStatus`

Methods
-------

Append(StringBuilder)
~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.ObjectIdentityMacro.Append(System.Text.StringBuilder)

   Appends the type name to the provided ``StringBuilder``.

   .. code-block:: csharp

      public void Append(StringBuilder typeName)

   :param typeName: The ``StringBuilder`` to append the type name to.
   :type typeName: ``StringBuilder``

Validate(ICollection<IConstruct>, ErrorRegistry)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.ObjectIdentityMacro.Validate(System.Collections.Generic.ICollection{Lextm.SharpSnmpPro.Mib.IConstruct},Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry)

   Validates this entity.

   .. code-block:: csharp

      public void Validate(ICollection<IConstruct> knownConstructs, ErrorRegistry registry)

   :param knownConstructs: Known constructs.
   :type knownConstructs: ``ICollection<IConstruct>``
   :param registry: The registry.
   :type registry: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry`

VerifyData(IAsnSerializable)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.ObjectIdentityMacro.VerifyData(DotNetSnmp.Asn1.Serialization.IAsnSerializable)

   .. code-block:: csharp

      public bool VerifyData(IAsnSerializable data)

   :type data: :any:`IAsnSerializable <DotNetSnmp.Asn1.Serialization.IAsnSerializable>`

   :rtype: ``Boolean``

