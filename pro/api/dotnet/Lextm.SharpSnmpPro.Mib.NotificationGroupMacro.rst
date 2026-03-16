NotificationGroupMacro Class
============================

.. dn:class:: Lextm.SharpSnmpPro.Mib.NotificationGroupMacro

   Represents a NOTIFICATION-GROUP macro in an SNMP MIB.

   .. code-block:: csharp

      public class NotificationGroupMacro : ISmiType, IEntity, IConstruct, IValidatable

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``NotificationGroupMacro``

Constructors
------------

NotificationGroupMacro(ISmiValue)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.NotificationGroupMacro..ctor(Lextm.SharpSnmpPro.Mib.ISmiValue)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.NotificationGroupMacro`` class.

   .. code-block:: csharp

      public NotificationGroupMacro(ISmiValue value)

   :param value: The notification value.
   :type value: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiValue`

Properties
----------

CharPositionInLine
~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.NotificationGroupMacro.CharPositionInLine

   Gets the char position in line.

   .. code-block:: csharp

      public int CharPositionInLine { get; set; }

   :returns: The char position in line.
   :rtype: ``Int32``

Description
~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.NotificationGroupMacro.Description

   Gets the description of the notification group.

   .. code-block:: csharp

      public string Description { get; }

   :rtype: ``String``

Line
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.NotificationGroupMacro.Line

   Gets the line number.

   .. code-block:: csharp

      public int Line { get; set; }

   :returns: The line.
   :rtype: ``Int32``

Module
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.NotificationGroupMacro.Module

   Gets or sets the module.

   .. code-block:: csharp

      public Module Module { get; set; }

   :returns: The module.
   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Module`

ModuleName
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.NotificationGroupMacro.ModuleName

   Gets or sets the name of the module this notification group belongs to.

   .. code-block:: csharp

      public string ModuleName { get; set; }

   :rtype: ``String``

Name
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.NotificationGroupMacro.Name

   Name.

   .. code-block:: csharp

      public string Name { get; set; }

   :rtype: ``String``

Notifications
~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.NotificationGroupMacro.Notifications

   Gets the list of notifications in this group.

   .. code-block:: csharp

      public IList<ISmiValue> Notifications { get; }

   :rtype: ``IList<ISmiValue>``

ObjectIdentifier
~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.NotificationGroupMacro.ObjectIdentifier

   Gets or sets the object identifier.

   .. code-block:: csharp

      [CLSCompliant(false)]
      [Obsolete("Please use GetObjectIdentifier method.")]
      public uint[] ObjectIdentifier { get; set; }

   :returns: The object identifier.
   :rtype: ``UInt32[]``

Parent
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.NotificationGroupMacro.Parent

   Gets or sets the parent.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public IEntity Parent { get; set; }

   :returns: The parent.
   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.IEntity`

Reference
~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.NotificationGroupMacro.Reference

   Gets the reference information for the notification group.

   .. code-block:: csharp

      public string Reference { get; }

   :rtype: ``String``

Status
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.NotificationGroupMacro.Status

   Status.

   .. code-block:: csharp

      public EntityStatus Status { get; set; }

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.EntityStatus`

Value
~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.NotificationGroupMacro.Value

   Gets or sets the value.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public uint Value { get; set; }

   :returns: The value.
   :rtype: ``UInt32``

Values
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.NotificationGroupMacro.Values

   Gets or sets the list of ID components.

   .. code-block:: csharp

      public IdComponentList Values { get; set; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.IdComponentList`

Verified
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.NotificationGroupMacro.Verified

   Gets or sets the verification status of an entity.

   .. code-block:: csharp

      public VerificationStatus Verified { get; set; }

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.VerificationStatus`

Methods
-------

Append(StringBuilder)
~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.NotificationGroupMacro.Append(System.Text.StringBuilder)

   Appends the type name to the provided ``StringBuilder``.

   .. code-block:: csharp

      public void Append(StringBuilder typeName)

   :param typeName: The ``StringBuilder`` to append the type name to.
   :type typeName: ``StringBuilder``

Validate(ICollection<IConstruct>, ErrorRegistry)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.NotificationGroupMacro.Validate(System.Collections.Generic.ICollection{Lextm.SharpSnmpPro.Mib.IConstruct},Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry)

   Validates this entity.

   .. code-block:: csharp

      public void Validate(ICollection<IConstruct> knownConstructs, ErrorRegistry registry)

   :param knownConstructs: Known constructs.
   :type knownConstructs: ``ICollection<IConstruct>``
   :param registry: The registry.
   :type registry: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry`

