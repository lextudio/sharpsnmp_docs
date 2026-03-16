Definition Class
================

.. dn:class:: Lextm.SharpSnmpPro.Mib.Registry.Definition

   Object definition. A definition might map to multiple entities defined in different MIB documents.

   .. code-block:: csharp

      public sealed class Definition

**Namespace:** ``Lextm.SharpSnmpPro.Mib.Registry``

**Inheritance:** Object → ``Definition``

Properties
----------

Children
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Registry.Definition.Children

   Children definitions.

   .. code-block:: csharp

      public IEnumerable<Definition> Children { get; }

   :rtype: ``IEnumerable<Definition>``

DisplayEntity
~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Registry.Definition.DisplayEntity

   Returns one of the :dn:iface:``~Lextm.SharpSnmpPro.Mib.IEntity`` in this :dn:cls:``~Lextm.SharpSnmpPro.Mib.Registry.Definition``.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public IEntity DisplayEntity { get; }

   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.IEntity`

Parent
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Registry.Definition.Parent

   Gets the parent definition.

   .. code-block:: csharp

      public Definition Parent { get; }

   :returns: The parent definition.
   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Registry.Definition`

TextualForms
~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Registry.Definition.TextualForms

   Returns the textual forms.

   .. code-block:: csharp

      public ICollection<string> TextualForms { get; }

   :rtype: ``ICollection<String>``

Type
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Registry.Definition.Type

   Gets the type.

   .. code-block:: csharp

      public DefinitionType Type { get; }

   :returns: The type.
   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.DefinitionType`

Value
~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Registry.Definition.Value

   Value.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public uint Value { get; }

   :rtype: ``UInt32``

Methods
-------

GetNumericalForm()
~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Registry.Definition.GetNumericalForm

   Gets the numerical form.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public uint[] GetNumericalForm()

   :rtype: ``UInt32[]``

