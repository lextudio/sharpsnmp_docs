SequenceOfType Class
====================

.. dn:class:: Lextm.SharpSnmpPro.Mib.SequenceOfType

   Represents an SMI SEQUENCE OF type.

   .. code-block:: csharp

      public class SequenceOfType : ISmiType, IConstruct, IConstrainted

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``SequenceOfType``

Properties
----------

BaseType
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.SequenceOfType.BaseType

   Gets or sets the base type of the sequence.

   .. code-block:: csharp

      public ISmiType BaseType { get; set; }

   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiType`

CharPositionInLine
~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.SequenceOfType.CharPositionInLine

   Gets the char position in line.

   .. code-block:: csharp

      public int CharPositionInLine { get; set; }

   :returns: The char position in line.
   :rtype: ``Int32``

Constraint
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.SequenceOfType.Constraint

   Gets or sets the constraint for the sequence of type.

   .. code-block:: csharp

      public Constraint Constraint { get; set; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Constraint`

Line
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.SequenceOfType.Line

   Gets the line number.

   .. code-block:: csharp

      public int Line { get; set; }

   :returns: The line.
   :rtype: ``Int32``

Module
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.SequenceOfType.Module

   Gets or sets the module.

   .. code-block:: csharp

      public Module Module { get; set; }

   :returns: The module.
   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Module`

Name
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.SequenceOfType.Name

   Name.

   .. code-block:: csharp

      public string Name { get; set; }

   :rtype: ``String``

Methods
-------

Append(StringBuilder)
~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.SequenceOfType.Append(System.Text.StringBuilder)

   Appends the type name to the provided ``StringBuilder``.

   .. code-block:: csharp

      public void Append(StringBuilder typeName)

   :param typeName: The ``StringBuilder`` to append the type name to.
   :type typeName: ``StringBuilder``

