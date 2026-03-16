BitStringType Class
===================

.. dn:class:: Lextm.SharpSnmpPro.Mib.BitStringType

   Represents a BIT STRING type in SMI (Structure of Management Information).

   .. code-block:: csharp

      public class BitStringType : ISmiType, IConstruct, IConstraintable

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``BitStringType``

Properties
----------

CharPositionInLine
~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.BitStringType.CharPositionInLine

   Gets the char position in line.

   .. code-block:: csharp

      public int CharPositionInLine { get; set; }

   :returns: The char position in line.
   :rtype: ``Int32``

Line
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.BitStringType.Line

   Gets the line number.

   .. code-block:: csharp

      public int Line { get; set; }

   :returns: The line.
   :rtype: ``Int32``

Module
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.BitStringType.Module

   Gets or sets the module.

   .. code-block:: csharp

      public Module Module { get; set; }

   :returns: The module.
   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Module`

Name
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.BitStringType.Name

   Name.

   .. code-block:: csharp

      public string Name { get; set; }

   :rtype: ``String``

NamedNumberList
~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.BitStringType.NamedNumberList

   Gets or sets the list of named numbers for this BIT STRING type.

   .. code-block:: csharp

      public IList<ISmiValue> NamedNumberList { get; set; }

   :rtype: ``IList<ISmiValue>``

Methods
-------

Append(StringBuilder)
~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.BitStringType.Append(System.Text.StringBuilder)

   Appends the type name to the provided ``StringBuilder``.

   .. code-block:: csharp

      public void Append(StringBuilder typeName)

   :param typeName: The ``StringBuilder`` to append the type name to.
   :type typeName: ``StringBuilder``

