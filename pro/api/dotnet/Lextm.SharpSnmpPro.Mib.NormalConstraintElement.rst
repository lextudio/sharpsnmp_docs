NormalConstraintElement Class
=============================

.. dn:class:: Lextm.SharpSnmpPro.Mib.NormalConstraintElement

   Represents a normal constraint element that can combine multiple constraints using union, bar, or intersect logic.

   .. code-block:: csharp

      public class NormalConstraintElement : ConstraintElement

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ConstraintElement → ``NormalConstraintElement``

Constructors
------------

NormalConstraintElement()
~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.NormalConstraintElement..ctor

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.NormalConstraintElement`` class.

   .. code-block:: csharp

      public NormalConstraintElement()

NormalConstraintElement(ConstraintElement)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.NormalConstraintElement..ctor(Lextm.SharpSnmpPro.Mib.ConstraintElement)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.NormalConstraintElement`` class with a specified constraint element.

   .. code-block:: csharp

      public NormalConstraintElement(ConstraintElement constraintElement)

   :param constraintElement: The initial constraint element.
   :type constraintElement: :dn:cls:`~Lextm.SharpSnmpPro.Mib.ConstraintElement`

Properties
----------

Bar
~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.NormalConstraintElement.Bar

   Gets or sets a value indicating whether this constraint uses bar logic.

   .. code-block:: csharp

      public bool Bar { get; set; }

   :rtype: ``Boolean``

ExtraElements
~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.NormalConstraintElement.ExtraElements

   Gets the list of extra constraint elements associated with this constraint.

   .. code-block:: csharp

      public List<ConstraintElement> ExtraElements { get; }

   :rtype: ``List<ConstraintElement>``

Intersect
~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.NormalConstraintElement.Intersect

   Gets or sets a value indicating whether this constraint uses intersect logic.

   .. code-block:: csharp

      public bool Intersect { get; set; }

   :rtype: ``Boolean``

Union
~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.NormalConstraintElement.Union

   Gets or sets a value indicating whether this constraint uses union logic.

   .. code-block:: csharp

      public bool Union { get; set; }

   :rtype: ``Boolean``

Methods
-------

Add(ConstraintElement)
~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.NormalConstraintElement.Add(Lextm.SharpSnmpPro.Mib.ConstraintElement)

   Adds an extra constraint element to this constraint.

   .. code-block:: csharp

      public void Add(ConstraintElement constraint)

   :param constraint: The constraint element to add.
   :type constraint: :dn:cls:`~Lextm.SharpSnmpPro.Mib.ConstraintElement`

Verify(IAsnSerializable)
~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.NormalConstraintElement.Verify(DotNetSnmp.Asn1.Serialization.IAsnSerializable)

   Verifies whether the specified SNMP data satisfies the constraint.

   .. code-block:: csharp

      public override bool Verify(IAsnSerializable data)

   :param data: The SNMP data to verify.
   :type data: :any:`IAsnSerializable <DotNetSnmp.Asn1.Serialization.IAsnSerializable>`

   :returns: true if the data satisfies the constraint; otherwise, false.
   :rtype: ``Boolean``

