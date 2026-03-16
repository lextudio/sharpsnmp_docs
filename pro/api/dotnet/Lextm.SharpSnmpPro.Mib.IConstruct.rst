IConstruct Interface
====================

.. dn:interface:: Lextm.SharpSnmpPro.Mib.IConstruct

   Construct interface.

   .. code-block:: csharp

      [SuppressMessage("Microsoft.Design", "CA1040:AvoidEmptyInterfaces")]
      public interface IConstruct

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

Properties
----------

CharPositionInLine
~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.IConstruct.CharPositionInLine

   Gets the char position in line.

   .. code-block:: csharp

      int CharPositionInLine { get; set; }

   :returns: The char position in line.
   :rtype: ``Int32``

Line
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.IConstruct.Line

   Gets the line number.

   .. code-block:: csharp

      int Line { get; set; }

   :returns: The line.
   :rtype: ``Int32``

Module
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.IConstruct.Module

   Gets or sets the module.

   .. code-block:: csharp

      Module Module { get; set; }

   :returns: The module.
   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Module`

Name
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.IConstruct.Name

   Name.

   .. code-block:: csharp

      string Name { get; set; }

   :rtype: ``String``

