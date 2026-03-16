BitsType Class
==============

.. dn:class:: Lextm.SharpSnmpPro.Mib.BitsType

   Represents a BITS type in SMI, which is a derived type with named bits.

   .. code-block:: csharp

      public class BitsType : IDerivedType, ISmiType, IConstruct

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``BitsType``

Properties
----------

BaseType
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.BitsType.BaseType

   Gets or sets the base type of this BITS type. If not set, it defaults to an :dn:cls:``~Lextm.SharpSnmpPro.Mib.UnknownType`` or :dn:cls:``~Lextm.SharpSnmpPro.Mib.OctetStringType`` based on the presence of a name.

   .. code-block:: csharp

      public ISmiType BaseType { get; set; }

   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiType`

CharPositionInLine
~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.BitsType.CharPositionInLine

   Gets the char position in line.

   .. code-block:: csharp

      public int CharPositionInLine { get; set; }

   :returns: The char position in line.
   :rtype: ``Int32``

Line
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.BitsType.Line

   Gets the line number.

   .. code-block:: csharp

      public int Line { get; set; }

   :returns: The line.
   :rtype: ``Int32``

Module
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.BitsType.Module

   Gets or sets the module.

   .. code-block:: csharp

      public Module Module { get; set; }

   :returns: The module.
   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Module`

Name
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.BitsType.Name

   Name.

   .. code-block:: csharp

      public string Name { get; set; }

   :rtype: ``String``

NamedBits
~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.BitsType.NamedBits

   Gets or sets the list of named bits for this BITS type.

   .. code-block:: csharp

      public IList<NamedBit> NamedBits { get; set; }

   :rtype: ``IList<NamedBit>``

Methods
-------

Append(StringBuilder)
~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.BitsType.Append(System.Text.StringBuilder)

   Appends the type name to the provided ``StringBuilder``.

   .. code-block:: csharp

      public void Append(StringBuilder typeName)

   :param typeName: The ``StringBuilder`` to append the type name to.
   :type typeName: ``StringBuilder``

