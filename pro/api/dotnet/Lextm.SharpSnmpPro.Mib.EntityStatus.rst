EntityStatus Enum
=================

.. dn:enum:: Lextm.SharpSnmpPro.Mib.EntityStatus

   Status enumeration for entities.

   .. code-block:: csharp

      public enum EntityStatus

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

Fields
------

Current
~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.EntityStatus.Current

   The entity is current and recommended for use.

   .. code-block:: csharp

      Current = 4

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.EntityStatus`

Deprecated
~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.EntityStatus.Deprecated

   The entity is deprecated and may be removed in the future.

   .. code-block:: csharp

      Deprecated = 5

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.EntityStatus`

Mandatory
~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.EntityStatus.Mandatory

   Entity with mandatory status should be converted to current for compatibility. Mandatory is obsolete in SMIv2.

   .. code-block:: csharp

      Mandatory = 1

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.EntityStatus`

Obsolete
~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.EntityStatus.Obsolete

   The entity is obsolete and should not be used.

   .. code-block:: csharp

      Obsolete = 3

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.EntityStatus`

Optional
~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.EntityStatus.Optional

   The entity is optional.

   .. code-block:: csharp

      Optional = 2

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.EntityStatus`

Unknown
~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.EntityStatus.Unknown

   The status of the entity is unknown.

   .. code-block:: csharp

      Unknown = 0

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.EntityStatus`

