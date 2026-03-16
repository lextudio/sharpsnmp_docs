SequenceValue Class
===================

.. dn:class:: Lextm.SharpSnmpPro.Mib.SequenceValue

   Represents a sequence value consisting of a collection of named values.

   .. code-block:: csharp

      public class SequenceValue : ISmiValue

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``SequenceValue``

Properties
----------

Values
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.SequenceValue.Values

   Gets the list of :dn:cls:``~Lextm.SharpSnmpPro.Mib.NamedValue`` items in the sequence.

   .. code-block:: csharp

      public IList<NamedValue> Values { get; }

   :rtype: ``IList<NamedValue>``

Methods
-------

Add(NamedValue)
~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.SequenceValue.Add(Lextm.SharpSnmpPro.Mib.NamedValue)

   Adds a :dn:cls:``~Lextm.SharpSnmpPro.Mib.NamedValue`` to the sequence.

   .. code-block:: csharp

      public void Add(NamedValue namedValue)

   :param namedValue: The named value to add.
   :type namedValue: :dn:cls:`~Lextm.SharpSnmpPro.Mib.NamedValue`

