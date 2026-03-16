UnknownType Class
=================

.. dn:class:: Lextm.SharpSnmpPro.Mib.UnknownType

   Represents an unknown derived type in the MIB.

   .. code-block:: csharp

      public class UnknownType : IDerivedType, ISmiType, IConstruct

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``UnknownType``

Properties
----------

BaseType
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.UnknownType.BaseType

   Gets or sets the base type of this derived type.

   .. code-block:: csharp

      public ISmiType BaseType { get; set; }

   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiType`

CharPositionInLine
~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.UnknownType.CharPositionInLine

   Gets the char position in line.

   .. code-block:: csharp

      public int CharPositionInLine { get; set; }

   :returns: The char position in line.
   :rtype: ``Int32``

Line
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.UnknownType.Line

   Gets the line number.

   .. code-block:: csharp

      public int Line { get; set; }

   :returns: The line.
   :rtype: ``Int32``

Module
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.UnknownType.Module

   Gets or sets the module.

   .. code-block:: csharp

      public Module Module { get; set; }

   :returns: The module.
   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Module`

ModuleName
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.UnknownType.ModuleName

   Gets or sets the name of the module where this type is defined.

   .. code-block:: csharp

      public string ModuleName { get; set; }

   :rtype: ``String``

Name
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.UnknownType.Name

   Name.

   .. code-block:: csharp

      public string Name { get; set; }

   :rtype: ``String``

NamedBits
~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.UnknownType.NamedBits

   Gets or sets the named bits for this type.

   .. code-block:: csharp

      public IList<NamedBit> NamedBits { get; set; }

   :rtype: ``IList<NamedBit>``

Methods
-------

Append(StringBuilder)
~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.UnknownType.Append(System.Text.StringBuilder)

   Appends the type name to the provided ``StringBuilder``.

   .. code-block:: csharp

      public void Append(StringBuilder typeName)

   :param typeName: The ``StringBuilder`` to append the type name to.
   :type typeName: ``StringBuilder``

