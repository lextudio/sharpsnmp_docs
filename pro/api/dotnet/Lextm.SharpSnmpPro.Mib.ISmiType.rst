ISmiType Interface
==================

.. dn:interface:: Lextm.SharpSnmpPro.Mib.ISmiType

   Represents an SMI (Structure of Management Information) type.

   .. code-block:: csharp

      public interface ISmiType : IConstruct

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

Methods
-------

Append(StringBuilder)
~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.ISmiType.Append(System.Text.StringBuilder)

   Appends the type name to the provided ``StringBuilder``.

   .. code-block:: csharp

      void Append(StringBuilder typeName)

   :param typeName: The ``StringBuilder`` to append the type name to.
   :type typeName: ``StringBuilder``

