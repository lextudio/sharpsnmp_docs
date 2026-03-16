FullQualifiedValue Class
========================

.. dn:class:: Lextm.SharpSnmpPro.Mib.FullQualifiedValue

   Represents a fully qualified value in the MIB (Management Information Base).

   .. code-block:: csharp

      public class FullQualifiedValue : ISmiValue

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``FullQualifiedValue``

Properties
----------

Values
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.FullQualifiedValue.Values

   Gets the list of parts that make up the fully qualified value.

   .. code-block:: csharp

      public IList<string> Values { get; }

   :rtype: ``IList<String>``

Methods
-------

Add(String)
~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.FullQualifiedValue.Add(System.String)

   Adds a part to the fully qualified value.

   .. code-block:: csharp

      public void Add(string part)

   :param part: The part to add.
   :type part: ``String``

