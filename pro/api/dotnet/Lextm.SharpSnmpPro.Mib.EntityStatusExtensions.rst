EntityStatusExtensions Class
============================

.. dn:class:: Lextm.SharpSnmpPro.Mib.EntityStatusExtensions

   Extension methods for the :dn:enum:``~Lextm.SharpSnmpPro.Mib.EntityStatus`` enumeration.

   .. code-block:: csharp

      public static class EntityStatusExtensions

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``EntityStatusExtensions``

Methods
-------

ToStatusString(EntityStatus)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.EntityStatusExtensions.ToStatusString(Lextm.SharpSnmpPro.Mib.EntityStatus)

   Converts the :dn:enum:``~Lextm.SharpSnmpPro.Mib.EntityStatus`` value to its lowercase string representation.

   .. code-block:: csharp

      public static string ToStatusString(this EntityStatus status)

   :param status: The :dn:enum:``~Lextm.SharpSnmpPro.Mib.EntityStatus`` value.
   :type status: :dn:enum:`~Lextm.SharpSnmpPro.Mib.EntityStatus`

   :returns: The lowercase string representation of the status.
   :rtype: ``String``

