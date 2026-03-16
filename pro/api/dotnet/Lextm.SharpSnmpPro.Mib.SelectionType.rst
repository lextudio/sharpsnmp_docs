SelectionType Class
===================

.. dn:class:: Lextm.SharpSnmpPro.Mib.SelectionType

   Represents a selection type in SMI (Structure of Management Information).

   .. code-block:: csharp

      public class SelectionType : ISmiType, IConstruct

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``SelectionType``

Constructors
------------

SelectionType(String, ISmiType)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.SelectionType..ctor(System.String,Lextm.SharpSnmpPro.Mib.ISmiType)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.SelectionType`` class.

   .. code-block:: csharp

      public SelectionType(string name, ISmiType subtype)

   :param name: The name of the selection type.
   :type name: ``String``
   :param subtype: The subtype of the selection type.
   :type subtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiType`

Properties
----------

CharPositionInLine
~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.SelectionType.CharPositionInLine

   Gets the char position in line.

   .. code-block:: csharp

      public int CharPositionInLine { get; set; }

   :returns: The char position in line.
   :rtype: ``Int32``

Line
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.SelectionType.Line

   Gets the line number.

   .. code-block:: csharp

      public int Line { get; set; }

   :returns: The line.
   :rtype: ``Int32``

Module
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.SelectionType.Module

   Gets or sets the module.

   .. code-block:: csharp

      public Module Module { get; set; }

   :returns: The module.
   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Module`

Name
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.SelectionType.Name

   Name.

   .. code-block:: csharp

      public string Name { get; set; }

   :rtype: ``String``

Subtype
~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.SelectionType.Subtype

   Gets or sets the subtype of this selection type.

   .. code-block:: csharp

      public ISmiType Subtype { get; set; }

   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiType`

Methods
-------

Append(StringBuilder)
~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.SelectionType.Append(System.Text.StringBuilder)

   Appends the type name to the provided ``StringBuilder``.

   .. code-block:: csharp

      public void Append(StringBuilder typeName)

   :param typeName: The ``StringBuilder`` to append the type name to.
   :type typeName: ``StringBuilder``

