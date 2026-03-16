IdComponentList Class
=====================

.. dn:class:: Lextm.SharpSnmpPro.Mib.IdComponentList

   Represents a list of identifier components, optionally associated with a defined value.

   .. code-block:: csharp

      public class IdComponentList : ISmiValue

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``IdComponentList``

Constructors
------------

IdComponentList()
~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.IdComponentList..ctor

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.IdComponentList`` class.

   .. code-block:: csharp

      public IdComponentList()

Properties
----------

DefinedValue
~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.IdComponentList.DefinedValue

   Gets or sets the defined value associated with this list.

   .. code-block:: csharp

      public DefinedValue DefinedValue { get; set; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.DefinedValue`

IdComponents
~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.IdComponentList.IdComponents

   Gets the list of identifier components.

   .. code-block:: csharp

      public IList<IdComponent> IdComponents { get; }

   :rtype: ``IList<IdComponent>``

Methods
-------

Add(IdComponent)
~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.IdComponentList.Add(Lextm.SharpSnmpPro.Mib.IdComponent)

   Adds an identifier component to the list.

   .. code-block:: csharp

      public void Add(IdComponent component)

   :param component: The identifier component to add.
   :type component: :dn:cls:`~Lextm.SharpSnmpPro.Mib.IdComponent`

