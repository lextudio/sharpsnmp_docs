TaggedType Class
================

.. dn:class:: Lextm.SharpSnmpPro.Mib.TaggedType

   Represents a tagged type in an SMI module, such as those using [APPLICATION n] or [IMPLICIT].

   .. code-block:: csharp

      public class TaggedType : IDerivedType, ISmiType, IConstruct

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``TaggedType``

Properties
----------

BaseType
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.TaggedType.BaseType

   Gets or sets the base type of this tagged type. This is typically the type that is being tagged, such as an INTEGER or OCTET STRING.

   .. code-block:: csharp

      public ISmiType BaseType { get; set; }

   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiType`

CharPositionInLine
~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.TaggedType.CharPositionInLine

   Gets the char position in line.

   .. code-block:: csharp

      public int CharPositionInLine { get; set; }

   :returns: The char position in line.
   :rtype: ``Int32``

Line
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.TaggedType.Line

   Gets the line number.

   .. code-block:: csharp

      public int Line { get; set; }

   :returns: The line.
   :rtype: ``Int32``

Module
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.TaggedType.Module

   Gets or sets the module.

   .. code-block:: csharp

      public Module Module { get; set; }

   :returns: The module.
   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Module`

Name
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.TaggedType.Name

   Name.

   .. code-block:: csharp

      public string Name { get; set; }

   :rtype: ``String``

Subtype
~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.TaggedType.Subtype

   Gets or sets the subtype of this tagged type.

   .. code-block:: csharp

      public ISmiType Subtype { get; set; }

   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiType`

Tag
~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.TaggedType.Tag

   Gets or sets the tag associated with this type.

   .. code-block:: csharp

      public Tag Tag { get; set; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Tag`

TagDefault
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.TaggedType.TagDefault

   Gets or sets the tag default (Explicit, Implicit, or Automatic).

   .. code-block:: csharp

      public TagDefault TagDefault { get; set; }

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.TagDefault`

Methods
-------

Append(StringBuilder)
~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.TaggedType.Append(System.Text.StringBuilder)

   Appends the type name to the provided ``StringBuilder``.

   .. code-block:: csharp

      public void Append(StringBuilder typeName)

   :param typeName: The ``StringBuilder`` to append the type name to.
   :type typeName: ``StringBuilder``

