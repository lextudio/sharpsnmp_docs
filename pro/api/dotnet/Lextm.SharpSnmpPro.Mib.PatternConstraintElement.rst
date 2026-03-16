PatternConstraintElement Class
==============================

.. dn:class:: Lextm.SharpSnmpPro.Mib.PatternConstraintElement

   Represents a constraint element that enforces a pattern on SNMP values.

   .. code-block:: csharp

      public class PatternConstraintElement : ConstraintElement

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ConstraintElement → ``PatternConstraintElement``

Constructors
------------

PatternConstraintElement(ISmiValue)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.PatternConstraintElement..ctor(Lextm.SharpSnmpPro.Mib.ISmiValue)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.PatternConstraintElement`` class.

   .. code-block:: csharp

      public PatternConstraintElement(ISmiValue value)

   :param value: The SNMP value representing the pattern constraint.
   :type value: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiValue`

Properties
----------

Value
~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.PatternConstraintElement.Value

   Gets the value expression used by PATTERN.

   .. code-block:: csharp

      public ISmiValue Value { get; }

   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiValue`

