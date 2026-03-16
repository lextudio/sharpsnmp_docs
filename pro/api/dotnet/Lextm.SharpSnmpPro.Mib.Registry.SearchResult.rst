SearchResult Class
==================

.. dn:class:: Lextm.SharpSnmpPro.Mib.Registry.SearchResult

   Search result.

   .. code-block:: csharp

      public sealed class SearchResult

**Namespace:** ``Lextm.SharpSnmpPro.Mib.Registry``

**Inheritance:** Object → ``SearchResult``

Constructors
------------

SearchResult(Definition, UInt32[])
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.Registry.SearchResult..ctor(Lextm.SharpSnmpPro.Mib.Registry.Definition,System.UInt32[])

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.Registry.SearchResult`` class.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public SearchResult(Definition definition, uint[] remaining)

   :param definition: The definition.
   :type definition: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Registry.Definition`
   :param remaining: The remaining.
   :type remaining: ``UInt32[]``

SearchResult(Definition)
~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.Registry.SearchResult..ctor(Lextm.SharpSnmpPro.Mib.Registry.Definition)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.Registry.SearchResult`` class.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public SearchResult(Definition definition)

   :param definition: The definition.
   :type definition: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Registry.Definition`

Properties
----------

AlternativeText
~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Registry.SearchResult.AlternativeText

   Gets the alternative textual form.

   .. code-block:: csharp

      [Obsolete("Please use Path property instead.")]
      public string AlternativeText { get; }

   :rtype: ``String``

Definition
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Registry.SearchResult.Definition

   Gets the definition.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public Definition Definition { get; }

   :returns: The definition.
   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Registry.Definition`

Path
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Registry.SearchResult.Path

   Gets the path.

   .. code-block:: csharp

      public string Path { get; }

   :returns: The path.
   :rtype: ``String``

Text
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Registry.SearchResult.Text

   Gets the textual form.

   .. code-block:: csharp

      public string Text { get; }

   :returns: The textual form.
   :rtype: ``String``

Methods
-------

GetRemaining()
~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Registry.SearchResult.GetRemaining

   Gets the remaining.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public ICollection<uint> GetRemaining()

   :returns: The remaining.
   :rtype: ``ICollection<UInt32>``

