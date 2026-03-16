SetType Class
=============

.. dn:class:: Lextm.SharpSnmpPro.Mib.SetType

   Represents an SMI SET type, which is a collection of element types.

   .. code-block:: csharp

      public class SetType : ISmiType, IConstruct

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``SetType``

Properties
----------

CharPositionInLine
~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.SetType.CharPositionInLine

   Gets the char position in line.

   .. code-block:: csharp

      public int CharPositionInLine { get; set; }

   :returns: The char position in line.
   :rtype: ``Int32``

ElementTypeList
~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.SetType.ElementTypeList

   Gets or sets the list of element types contained in this SET type.

   .. code-block:: csharp

      public IList<ISmiType> ElementTypeList { get; set; }

   :rtype: ``IList<ISmiType>``

Line
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.SetType.Line

   Gets the line number.

   .. code-block:: csharp

      public int Line { get; set; }

   :returns: The line.
   :rtype: ``Int32``

Module
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.SetType.Module

   Gets or sets the module.

   .. code-block:: csharp

      public Module Module { get; set; }

   :returns: The module.
   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Module`

Name
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.SetType.Name

   Name.

   .. code-block:: csharp

      public string Name { get; set; }

   :rtype: ``String``

Methods
-------

Append(StringBuilder)
~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.SetType.Append(System.Text.StringBuilder)

   Appends the type name to the provided ``StringBuilder``.

   .. code-block:: csharp

      public void Append(StringBuilder typeName)

   :param typeName: The ``StringBuilder`` to append the type name to.
   :type typeName: ``StringBuilder``

