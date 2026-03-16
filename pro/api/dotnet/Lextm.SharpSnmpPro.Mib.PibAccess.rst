PibAccess Enum
==============

.. dn:enum:: Lextm.SharpSnmpPro.Mib.PibAccess

   Specifies the access level for a Protocol Information Base (PIB) object.

   .. code-block:: csharp

      public enum PibAccess

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

Fields
------

Install
~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.PibAccess.Install

   The object can be installed.

   .. code-block:: csharp

      Install = 0

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.PibAccess`

InstallNotify
~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.PibAccess.InstallNotify

   The object can be installed and notified.

   .. code-block:: csharp

      InstallNotify = 2

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.PibAccess`

NotAccessible
~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.PibAccess.NotAccessible

   The object is not accessible.

   .. code-block:: csharp

      NotAccessible = 4

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.PibAccess`

Notify
~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.PibAccess.Notify

   The object can be notified.

   .. code-block:: csharp

      Notify = 1

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.PibAccess`

ReportOnly
~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.PibAccess.ReportOnly

   The object is report-only.

   .. code-block:: csharp

      ReportOnly = 3

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.PibAccess`

