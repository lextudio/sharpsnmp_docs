SetOfType Class
===============

.. dn:class:: Lextm.SharpSnmpPro.Mib.SetOfType

   Represents a SET OF type in SMI, which is a collection of elements of a specified subtype.

   .. code-block:: csharp

      public class SetOfType : ISmiType, IConstruct, IConstrainted

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``SetOfType``

Properties
----------

CharPositionInLine
~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.SetOfType.CharPositionInLine

   Gets the char position in line.

   .. code-block:: csharp

      public int CharPositionInLine { get; set; }

   :returns: The char position in line.
   :rtype: ``Int32``

Constraint
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.SetOfType.Constraint

   Gets or sets the constraint for the set of type. This defines the rules that the elements in the set must adhere to.

   .. code-block:: csharp

      public Constraint Constraint { get; set; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Constraint`

Line
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.SetOfType.Line

   Gets the line number.

   .. code-block:: csharp

      public int Line { get; set; }

   :returns: The line.
   :rtype: ``Int32``

Module
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.SetOfType.Module

   Gets or sets the module.

   .. code-block:: csharp

      public Module Module { get; set; }

   :returns: The module.
   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Module`

Name
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.SetOfType.Name

   Name.

   .. code-block:: csharp

      public string Name { get; set; }

   :rtype: ``String``

Subtype
~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.SetOfType.Subtype

   Gets or sets the subtype of the elements in the set.

   .. code-block:: csharp

      public ISmiType Subtype { get; set; }

   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiType`

Methods
-------

Append(StringBuilder)
~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.SetOfType.Append(System.Text.StringBuilder)

   Appends the type name to the provided ``StringBuilder``.

   .. code-block:: csharp

      public void Append(StringBuilder typeName)

   :param typeName: The ``StringBuilder`` to append the type name to.
   :type typeName: ``StringBuilder``

