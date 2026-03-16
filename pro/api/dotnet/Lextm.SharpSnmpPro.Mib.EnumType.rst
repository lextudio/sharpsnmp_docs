EnumType Class
==============

.. dn:class:: Lextm.SharpSnmpPro.Mib.EnumType

   Represents an enumeration type in a MIB module.

   .. code-block:: csharp

      public class EnumType : ISmiType, IConstruct

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``EnumType``

Constructors
------------

EnumType(IList<ISmiValue>)
~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.EnumType..ctor(System.Collections.Generic.IList{Lextm.SharpSnmpPro.Mib.ISmiValue})

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.EnumType`` class.

   .. code-block:: csharp

      public EnumType(IList<ISmiValue> values)

   :param values: The enumeration values.
   :type values: ``IList<ISmiValue>``

Properties
----------

CharPositionInLine
~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.EnumType.CharPositionInLine

   Gets the char position in line.

   .. code-block:: csharp

      public int CharPositionInLine { get; set; }

   :returns: The char position in line.
   :rtype: ``Int32``

Line
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.EnumType.Line

   Gets the line number.

   .. code-block:: csharp

      public int Line { get; set; }

   :returns: The line.
   :rtype: ``Int32``

Module
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.EnumType.Module

   Gets or sets the module.

   .. code-block:: csharp

      public Module Module { get; set; }

   :returns: The module.
   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Module`

Name
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.EnumType.Name

   Name.

   .. code-block:: csharp

      public string Name { get; set; }

   :rtype: ``String``

Values
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.EnumType.Values

   Gets or sets the list of enumeration values.

   .. code-block:: csharp

      public IList<ISmiValue> Values { get; set; }

   :rtype: ``IList<ISmiValue>``

Methods
-------

Append(StringBuilder)
~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.EnumType.Append(System.Text.StringBuilder)

   Appends the type name to the provided ``StringBuilder``.

   .. code-block:: csharp

      public void Append(StringBuilder typeName)

   :param typeName: The ``StringBuilder`` to append the type name to.
   :type typeName: ``StringBuilder``

