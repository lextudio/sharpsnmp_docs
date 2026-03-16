IObjectTypeMacro Interface
==========================

.. dn:interface:: Lextm.SharpSnmpPro.Mib.IObjectTypeMacro

   OBJECT-TYPE macro interface.

   .. code-block:: csharp

      public interface IObjectTypeMacro

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

Properties
----------

MibAccess
~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.IObjectTypeMacro.MibAccess

   MAX-ACCESS.

   .. code-block:: csharp

      Access MibAccess { get; }

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Access`

ResolvedSyntax
~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.IObjectTypeMacro.ResolvedSyntax

   Gets the resolved syntax.

   .. code-block:: csharp

      ISmiType ResolvedSyntax { get; }

   :returns: The resolved syntax.
   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiType`

Status
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.IObjectTypeMacro.Status

   Gets the status.

   .. code-block:: csharp

      EntityStatus Status { get; }

   :returns: The status.
   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.EntityStatus`

Syntax
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.IObjectTypeMacro.Syntax

   Gets the syntax.

   .. code-block:: csharp

      ISmiType Syntax { get; }

   :returns: The syntax.
   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiType`

