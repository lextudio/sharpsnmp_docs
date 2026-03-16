EntityExtensions Class
======================

.. dn:class:: Lextm.SharpSnmpPro.Mib.EntityExtensions

   Extension methods of :dn:iface:``~Lextm.SharpSnmpPro.Mib.IEntity``.

   .. code-block:: csharp

      public static class EntityExtensions

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``EntityExtensions``

Methods
-------

DescriptionFormatted(IEntity)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.EntityExtensions.DescriptionFormatted(Lextm.SharpSnmpPro.Mib.IEntity)

   Formatted description.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public static string DescriptionFormatted(this IEntity entity)

   :param entity: The entity.
   :type entity: :dn:iface:`~Lextm.SharpSnmpPro.Mib.IEntity`

   :rtype: ``String``

GetObjectIdentifier(IEntity)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.EntityExtensions.GetObjectIdentifier(Lextm.SharpSnmpPro.Mib.IEntity)

   Gets object identifier.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public static uint[] GetObjectIdentifier(this IEntity entity)

   :param entity: Entity.
   :type entity: :dn:iface:`~Lextm.SharpSnmpPro.Mib.IEntity`

   :rtype: ``UInt32[]``

