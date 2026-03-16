TextualConventionMacro Class
============================

.. dn:class:: Lextm.SharpSnmpPro.Mib.TextualConventionMacro

   Represents a TEXTUAL-CONVENTION macro in an SMI module.

   .. code-block:: csharp

      public class TextualConventionMacro : IDerivedType, ISmiType, IConstruct

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``TextualConventionMacro``

Properties
----------

BaseType
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.TextualConventionMacro.BaseType

   Gets or sets the base type of the textual convention.

   .. code-block:: csharp

      public ISmiType BaseType { get; set; }

   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiType`

CharPositionInLine
~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.TextualConventionMacro.CharPositionInLine

   Gets the char position in line.

   .. code-block:: csharp

      public int CharPositionInLine { get; set; }

   :returns: The char position in line.
   :rtype: ``Int32``

Description
~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.TextualConventionMacro.Description

   Provides a textual description of the textual convention.

   .. code-block:: csharp

      public string Description { get; }

   :rtype: ``String``

DisplayHint
~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.TextualConventionMacro.DisplayHint

   Gets or sets the display hint for the textual convention.

   .. code-block:: csharp

      public string DisplayHint { get; }

   :rtype: ``String``

Line
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.TextualConventionMacro.Line

   Gets the line number.

   .. code-block:: csharp

      public int Line { get; set; }

   :returns: The line.
   :rtype: ``Int32``

Module
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.TextualConventionMacro.Module

   Gets or sets the module.

   .. code-block:: csharp

      public Module Module { get; set; }

   :returns: The module.
   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Module`

Name
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.TextualConventionMacro.Name

   Name.

   .. code-block:: csharp

      public string Name { get; set; }

   :rtype: ``String``

Reference
~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.TextualConventionMacro.Reference

   Specifies the source of the definition (such as a document from another standards organization, or an architectural document for a proprietary system).

   .. code-block:: csharp

      public string Reference { get; }

   :rtype: ``String``

Status
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.TextualConventionMacro.Status

   Gets or sets the status of the textual convention.

   .. code-block:: csharp

      public EntityStatus Status { get; set; }

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.EntityStatus`

Methods
-------

Append(StringBuilder)
~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.TextualConventionMacro.Append(System.Text.StringBuilder)

   Appends the textual convention macro definition to the provided ``StringBuilder``.

   .. code-block:: csharp

      public void Append(StringBuilder typeName)

   :param typeName: The ``StringBuilder`` to append the definition to.
   :type typeName: ``StringBuilder``

