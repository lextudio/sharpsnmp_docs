ElementType Class
=================

.. dn:class:: Lextm.SharpSnmpPro.Mib.ElementType

   Represents an element type in a MIB module.

   .. code-block:: csharp

      public class ElementType : ISmiType, IConstruct

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``ElementType``

Properties
----------

CharPositionInLine
~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ElementType.CharPositionInLine

   Gets the char position in line.

   .. code-block:: csharp

      public int CharPositionInLine { get; set; }

   :returns: The char position in line.
   :rtype: ``Int32``

Default
~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ElementType.Default

   Gets or sets a value indicating whether this element has a default value.

   .. code-block:: csharp

      public bool Default { get; set; }

   :rtype: ``Boolean``

Line
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ElementType.Line

   Gets the line number.

   .. code-block:: csharp

      public int Line { get; set; }

   :returns: The line.
   :rtype: ``Int32``

Module
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ElementType.Module

   Gets or sets the module.

   .. code-block:: csharp

      public Module Module { get; set; }

   :returns: The module.
   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Module`

Name
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ElementType.Name

   Name.

   .. code-block:: csharp

      public string Name { get; set; }

   :rtype: ``String``

Optional
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ElementType.Optional

   Gets or sets a value indicating whether this element is optional.

   .. code-block:: csharp

      public bool Optional { get; set; }

   :rtype: ``Boolean``

Subtype
~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ElementType.Subtype

   Gets or sets the subtype of this element type.

   .. code-block:: csharp

      public ISmiType Subtype { get; set; }

   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiType`

Tag
~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ElementType.Tag

   Gets or sets the tag associated with this element type.

   .. code-block:: csharp

      public Tag Tag { get; set; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Tag`

TagDefault
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ElementType.TagDefault

   Gets or sets the default tagging mode for this element type.

   .. code-block:: csharp

      public TagDefault TagDefault { get; set; }

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.TagDefault`

Value
~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ElementType.Value

   Gets or sets the value associated with this element type.

   .. code-block:: csharp

      public ISmiValue Value { get; set; }

   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiValue`

Methods
-------

Append(StringBuilder)
~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.ElementType.Append(System.Text.StringBuilder)

   Appends the type name to the provided ``StringBuilder``.

   .. code-block:: csharp

      public void Append(StringBuilder typeName)

   :param typeName: The ``StringBuilder`` to append the type name to.
   :type typeName: ``StringBuilder``

