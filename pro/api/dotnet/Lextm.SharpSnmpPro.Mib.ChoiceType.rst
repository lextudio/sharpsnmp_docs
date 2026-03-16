ChoiceType Class
================

.. dn:class:: Lextm.SharpSnmpPro.Mib.ChoiceType

   Represents a CHOICE type in SMI, which allows one of several types.

   .. code-block:: csharp

      public class ChoiceType : ISmiType, IConstruct, IValidatable

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``ChoiceType``

Constructors
------------

ChoiceType(IList<ISmiType>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.ChoiceType..ctor(System.Collections.Generic.IList{Lextm.SharpSnmpPro.Mib.ISmiType})

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.ChoiceType`` class.

   .. code-block:: csharp

      public ChoiceType(IList<ISmiType> elementTypes)

   :param elementTypes: The element types that can be chosen.
   :type elementTypes: ``IList<ISmiType>``

Properties
----------

CharPositionInLine
~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ChoiceType.CharPositionInLine

   Gets the char position in line.

   .. code-block:: csharp

      public int CharPositionInLine { get; set; }

   :returns: The char position in line.
   :rtype: ``Int32``

ElementTypes
~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ChoiceType.ElementTypes

   Gets or sets the element types that can be chosen.

   .. code-block:: csharp

      public IList<ISmiType> ElementTypes { get; set; }

   :rtype: ``IList<ISmiType>``

Line
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ChoiceType.Line

   Gets the line number.

   .. code-block:: csharp

      public int Line { get; set; }

   :returns: The line.
   :rtype: ``Int32``

Module
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ChoiceType.Module

   Gets or sets the module.

   .. code-block:: csharp

      public Module Module { get; set; }

   :returns: The module.
   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Module`

Name
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ChoiceType.Name

   Name.

   .. code-block:: csharp

      public string Name { get; set; }

   :rtype: ``String``

Methods
-------

Append(StringBuilder)
~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.ChoiceType.Append(System.Text.StringBuilder)

   Appends the type name to the provided ``StringBuilder``.

   .. code-block:: csharp

      public void Append(StringBuilder typeName)

   :param typeName: The ``StringBuilder`` to append the type name to.
   :type typeName: ``StringBuilder``

Validate(ICollection<IConstruct>, ErrorRegistry)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.ChoiceType.Validate(System.Collections.Generic.ICollection{Lextm.SharpSnmpPro.Mib.IConstruct},Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry)

   Validates this entity.

   .. code-block:: csharp

      public void Validate(ICollection<IConstruct> knownContructs, ErrorRegistry registry)

   :type knownContructs: ``ICollection<IConstruct>``
   :param registry: The registry.
   :type registry: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry`

