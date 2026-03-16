NamedConstraintElement Class
============================

.. dn:class:: Lextm.SharpSnmpPro.Mib.NamedConstraintElement

   Represents a named constraint element for SNMP, which can be present, absent, or optional, and may have an associated constraint.

   .. code-block:: csharp

      public class NamedConstraintElement : ConstraintElement

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ConstraintElement → ``NamedConstraintElement``

Constructors
------------

NamedConstraintElement(String)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.NamedConstraintElement..ctor(System.String)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.NamedConstraintElement`` class with the specified name.

   .. code-block:: csharp

      public NamedConstraintElement(string name)

   :param name: The name of the constraint element.
   :type name: ``String``

Properties
----------

Absent
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.NamedConstraintElement.Absent

   Gets or sets a value indicating whether the element is absent.

   .. code-block:: csharp

      public bool Absent { get; set; }

   :rtype: ``Boolean``

Constraint
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.NamedConstraintElement.Constraint

   Gets or sets the associated constraint.

   .. code-block:: csharp

      public Constraint Constraint { get; set; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Constraint`

Name
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.NamedConstraintElement.Name

   Gets or sets the name of the constraint element.

   .. code-block:: csharp

      public string Name { get; set; }

   :rtype: ``String``

Optinal
~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.NamedConstraintElement.Optinal

   Gets or sets a value indicating whether the element is optional. Kept for backward compatibility due to legacy typo.

   .. code-block:: csharp

      [Obsolete("Use Optional instead.")]
      public bool Optinal { get; set; }

   :rtype: ``Boolean``

Optional
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.NamedConstraintElement.Optional

   Gets or sets a value indicating whether the element is optional.

   .. code-block:: csharp

      public bool Optional { get; set; }

   :rtype: ``Boolean``

Present
~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.NamedConstraintElement.Present

   Gets or sets a value indicating whether the element is present.

   .. code-block:: csharp

      public bool Present { get; set; }

   :rtype: ``Boolean``

