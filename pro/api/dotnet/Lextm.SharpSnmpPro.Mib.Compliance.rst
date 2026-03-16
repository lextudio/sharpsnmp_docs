Compliance Class
================

.. dn:class:: Lextm.SharpSnmpPro.Mib.Compliance

   Represents a compliance statement for an SNMP MIB module.

   .. code-block:: csharp

      public class Compliance

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``Compliance``

Properties
----------

Description
~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Compliance.Description

   Gets or sets the description of the compliance statement.

   .. code-block:: csharp

      public string Description { get; protected set; }

   :rtype: ``String``

MinAccess
~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Compliance.MinAccess

   Access modifier.

   .. code-block:: csharp

      public Access MinAccess { get; set; }

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Access`

PibMinAccess
~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Compliance.PibMinAccess

   Specifies the access level for a Protocol Information Base (PIB) object.

   .. code-block:: csharp

      public PibAccess PibMinAccess { get; set; }

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.PibAccess`

Syntax
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Compliance.Syntax

   Represents an SMI (Structure of Management Information) type.

   .. code-block:: csharp

      public ISmiType Syntax { get; set; }

   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiType`

WriteSyntax
~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Compliance.WriteSyntax

   Represents an SMI (Structure of Management Information) type.

   .. code-block:: csharp

      public ISmiType WriteSyntax { get; set; }

   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiType`

