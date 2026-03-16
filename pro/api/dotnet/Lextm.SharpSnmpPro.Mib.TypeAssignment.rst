TypeAssignment Class
====================

.. dn:class:: Lextm.SharpSnmpPro.Mib.TypeAssignment

   Represents a type assignment in a MIB module.

   .. code-block:: csharp

      public class TypeAssignment : IDerivedType, ISmiType, IConstruct

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``TypeAssignment``

Constructors
------------

TypeAssignment(ISmiType)
~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.TypeAssignment..ctor(Lextm.SharpSnmpPro.Mib.ISmiType)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.TypeAssignment`` class.

   .. code-block:: csharp

      public TypeAssignment(ISmiType smiType)

   :param smiType: The base SMI type.
   :type smiType: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiType`

Properties
----------

BaseType
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.TypeAssignment.BaseType

   Gets or sets the base type of this type assignment.

   .. code-block:: csharp

      public ISmiType BaseType { get; set; }

   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiType`

CharPositionInLine
~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.TypeAssignment.CharPositionInLine

   Gets the char position in line.

   .. code-block:: csharp

      public int CharPositionInLine { get; set; }

   :returns: The char position in line.
   :rtype: ``Int32``

Line
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.TypeAssignment.Line

   Gets the line number.

   .. code-block:: csharp

      public int Line { get; set; }

   :returns: The line.
   :rtype: ``Int32``

Module
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.TypeAssignment.Module

   Gets or sets the module.

   .. code-block:: csharp

      public Module Module { get; set; }

   :returns: The module.
   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Module`

Name
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.TypeAssignment.Name

   Name.

   .. code-block:: csharp

      public string Name { get; set; }

   :rtype: ``String``

Methods
-------

Append(StringBuilder)
~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.TypeAssignment.Append(System.Text.StringBuilder)

   Appends the type assignment to the provided ``StringBuilder``.

   .. code-block:: csharp

      public void Append(StringBuilder typeName)

   :param typeName: The ``StringBuilder`` to append the type assignment to.
   :type typeName: ``StringBuilder``

Validate(ICollection<IConstruct>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.TypeAssignment.Validate(System.Collections.Generic.ICollection{Lextm.SharpSnmpPro.Mib.IConstruct})

   Validates this type assignment against known constructs.

   .. code-block:: csharp

      public void Validate(ICollection<IConstruct> knownConstructs)

   :param knownConstructs: The collection of known constructs.
   :type knownConstructs: ``ICollection<IConstruct>``

