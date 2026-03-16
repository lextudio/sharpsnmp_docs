ConstraintedType Class
======================

.. dn:class:: Lextm.SharpSnmpPro.Mib.ConstraintedType

   Represents a type with constraints in a MIB module.

   .. code-block:: csharp

      public class ConstraintedType : IDerivedType, ISmiType, IConstruct, IConstrainted

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``ConstraintedType``

Constructors
------------

ConstraintedType(ISmiType)
~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.ConstraintedType..ctor(Lextm.SharpSnmpPro.Mib.ISmiType)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.ConstraintedType`` class.

   .. code-block:: csharp

      public ConstraintedType(ISmiType smiType)

   :param smiType: The base SMI type.
   :type smiType: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiType`

Properties
----------

BaseType
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ConstraintedType.BaseType

   Gets or sets the base type of this constrainted type.

   .. code-block:: csharp

      public ISmiType BaseType { get; set; }

   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiType`

CharPositionInLine
~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ConstraintedType.CharPositionInLine

   Gets the char position in line.

   .. code-block:: csharp

      public int CharPositionInLine { get; set; }

   :returns: The char position in line.
   :rtype: ``Int32``

Constraint
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ConstraintedType.Constraint

   Gets or sets the constraint for this type.

   .. code-block:: csharp

      public Constraint Constraint { get; set; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Constraint`

Line
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ConstraintedType.Line

   Gets the line number.

   .. code-block:: csharp

      public int Line { get; set; }

   :returns: The line.
   :rtype: ``Int32``

Module
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ConstraintedType.Module

   Gets or sets the module.

   .. code-block:: csharp

      public Module Module { get; set; }

   :returns: The module.
   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Module`

Name
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ConstraintedType.Name

   Name.

   .. code-block:: csharp

      public string Name { get; set; }

   :rtype: ``String``

Methods
-------

Append(StringBuilder)
~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.ConstraintedType.Append(System.Text.StringBuilder)

   Appends the type name to the provided ``StringBuilder``.

   .. code-block:: csharp

      public void Append(StringBuilder typeName)

   :param typeName: The ``StringBuilder`` to append the type name to.
   :type typeName: ``StringBuilder``

Validate(ICollection<IConstruct>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.ConstraintedType.Validate(System.Collections.Generic.ICollection{Lextm.SharpSnmpPro.Mib.IConstruct})

   Validates this type against known constructs.

   .. code-block:: csharp

      public void Validate(ICollection<IConstruct> knownConstructs)

   :param knownConstructs: The collection of known constructs.
   :type knownConstructs: ``ICollection<IConstruct>``

