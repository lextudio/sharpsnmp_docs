Index Class
===========

.. dn:class:: Lextm.SharpSnmpPro.Mib.Index

   Represents an index in a MIB table, including its type and whether it is implied.

   .. code-block:: csharp

      public class Index

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``Index``

Properties
----------

Implied
~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Index.Implied

   Gets or sets a value indicating whether this index is implied.

   .. code-block:: csharp

      public bool Implied { get; }

   :rtype: ``Boolean``

Type
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Index.Type

   Gets or sets the object type macro associated with this index.

   .. code-block:: csharp

      public ObjectTypeMacro Type { get; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.ObjectTypeMacro`

