AgentCapabilitiesMacro Class
============================

.. dn:class:: Lextm.SharpSnmpPro.Mib.AgentCapabilitiesMacro

   Represents an AGENT-CAPABILITIES macro in a MIB module.

   .. code-block:: csharp

      public class AgentCapabilitiesMacro : ISmiType, IEntity, IConstruct, IValidatable

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``AgentCapabilitiesMacro``

Constructors
------------

AgentCapabilitiesMacro(String)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.AgentCapabilitiesMacro..ctor(System.String)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.AgentCapabilitiesMacro`` class.

   .. code-block:: csharp

      public AgentCapabilitiesMacro(string productRelease)

   :param productRelease: The product release string.
   :type productRelease: ``String``

Properties
----------

CharPositionInLine
~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.AgentCapabilitiesMacro.CharPositionInLine

   Gets the char position in line.

   .. code-block:: csharp

      public int CharPositionInLine { get; set; }

   :returns: The char position in line.
   :rtype: ``Int32``

Description
~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.AgentCapabilitiesMacro.Description

   Gets or sets the description of the agent capabilities.

   .. code-block:: csharp

      public string Description { get; }

   :rtype: ``String``

Line
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.AgentCapabilitiesMacro.Line

   Gets the line number.

   .. code-block:: csharp

      public int Line { get; set; }

   :returns: The line.
   :rtype: ``Int32``

Module
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.AgentCapabilitiesMacro.Module

   Gets or sets the module.

   .. code-block:: csharp

      public Module Module { get; set; }

   :returns: The module.
   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Module`

ModuleName
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.AgentCapabilitiesMacro.ModuleName

   Gets or sets the name of the module this macro belongs to.

   .. code-block:: csharp

      public string ModuleName { get; set; }

   :rtype: ``String``

Modules
~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.AgentCapabilitiesMacro.Modules

   Gets or sets the list of modules associated with this agent capabilities macro.

   .. code-block:: csharp

      public IList<AgentCapabilitiesModule> Modules { get; set; }

   :rtype: ``IList<AgentCapabilitiesModule>``

Name
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.AgentCapabilitiesMacro.Name

   Gets or sets the name of this agent capabilities macro.

   .. code-block:: csharp

      public string Name { get; set; }

   :rtype: ``String``

ObjectIdentifier
~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.AgentCapabilitiesMacro.ObjectIdentifier

   Gets or sets the object identifier.

   .. code-block:: csharp

      [CLSCompliant(false)]
      [Obsolete("Please use GetObjectIdentifier method.")]
      public uint[] ObjectIdentifier { get; set; }

   :returns: The object identifier.
   :rtype: ``UInt32[]``

Parent
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.AgentCapabilitiesMacro.Parent

   Gets or sets the parent.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public IEntity Parent { get; set; }

   :returns: The parent.
   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.IEntity`

Reference
~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.AgentCapabilitiesMacro.Reference

   Gets or sets the reference information for the agent capabilities.

   .. code-block:: csharp

      public string Reference { get; }

   :rtype: ``String``

Status
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.AgentCapabilitiesMacro.Status

   Status.

   .. code-block:: csharp

      public EntityStatus Status { get; set; }

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.EntityStatus`

Value
~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.AgentCapabilitiesMacro.Value

   Gets or sets the value.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public uint Value { get; set; }

   :returns: The value.
   :rtype: ``UInt32``

Values
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.AgentCapabilitiesMacro.Values

   Gets or sets the list of ID components.

   .. code-block:: csharp

      public IdComponentList Values { get; set; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.IdComponentList`

Verified
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.AgentCapabilitiesMacro.Verified

   Gets or sets the verification status of an entity.

   .. code-block:: csharp

      public VerificationStatus Verified { get; set; }

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.VerificationStatus`

Methods
-------

Append(StringBuilder)
~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.AgentCapabilitiesMacro.Append(System.Text.StringBuilder)

   Appends the type name to the provided ``StringBuilder``.

   .. code-block:: csharp

      public void Append(StringBuilder typeName)

   :param typeName: The ``StringBuilder`` to append the type name to.
   :type typeName: ``StringBuilder``

Validate(ICollection<IConstruct>, ErrorRegistry)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.AgentCapabilitiesMacro.Validate(System.Collections.Generic.ICollection{Lextm.SharpSnmpPro.Mib.IConstruct},Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry)

   Validates this entity.

   .. code-block:: csharp

      public void Validate(ICollection<IConstruct> knownConstructs, ErrorRegistry registry)

   :param knownConstructs: Known constructs.
   :type knownConstructs: ``ICollection<IConstruct>``
   :param registry: The registry.
   :type registry: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry`

