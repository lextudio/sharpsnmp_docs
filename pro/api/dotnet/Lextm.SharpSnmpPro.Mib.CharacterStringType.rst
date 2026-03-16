CharacterStringType Class
=========================

.. dn:class:: Lextm.SharpSnmpPro.Mib.CharacterStringType

   Represents a character string SMI type.

   .. code-block:: csharp

      public class CharacterStringType : ISmiType, IConstruct, IConstraintable

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``CharacterStringType``

Properties
----------

CharacterSet
~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.CharacterStringType.CharacterSet

   Gets or sets the character set.

   .. code-block:: csharp

      public CharacterSet CharacterSet { get; set; }

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.CharacterSet`

CharPositionInLine
~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.CharacterStringType.CharPositionInLine

   Gets the char position in line.

   .. code-block:: csharp

      public int CharPositionInLine { get; set; }

   :returns: The char position in line.
   :rtype: ``Int32``

Line
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.CharacterStringType.Line

   Gets the line number.

   .. code-block:: csharp

      public int Line { get; set; }

   :returns: The line.
   :rtype: ``Int32``

Module
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.CharacterStringType.Module

   Gets or sets the module.

   .. code-block:: csharp

      public Module Module { get; set; }

   :returns: The module.
   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Module`

Name
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.CharacterStringType.Name

   Name.

   .. code-block:: csharp

      public string Name { get; set; }

   :rtype: ``String``

Methods
-------

Append(StringBuilder)
~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.CharacterStringType.Append(System.Text.StringBuilder)

   Appends the type name to the provided ``StringBuilder``.

   .. code-block:: csharp

      public void Append(StringBuilder typeName)

   :param typeName: The ``StringBuilder`` to append the type name to.
   :type typeName: ``StringBuilder``

