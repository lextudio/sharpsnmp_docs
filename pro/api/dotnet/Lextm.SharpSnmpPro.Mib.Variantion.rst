Variantion Class
================

.. dn:class:: Lextm.SharpSnmpPro.Mib.Variantion

   Represents a variation of an SMI (Structure of Management Information) object.

   .. code-block:: csharp

      public class Variantion

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``Variantion``

Constructors
------------

Variantion(ISmiValue)
~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.Variantion..ctor(Lextm.SharpSnmpPro.Mib.ISmiValue)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.Variantion`` class.

   .. code-block:: csharp

      public Variantion(ISmiValue variationValue)

   :param variationValue: The default value for the variation.
   :type variationValue: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiValue`

Properties
----------

Access
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Variantion.Access

   Gets or sets the access level of the variation.

   .. code-block:: csharp

      public Access Access { get; set; }

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Access`

CreationRequires
~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Variantion.CreationRequires

   Gets or sets the list of required values for creation.

   .. code-block:: csharp

      public IList<ISmiValue> CreationRequires { get; set; }

   :rtype: ``IList<ISmiValue>``

DefaultValue
~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Variantion.DefaultValue

   Gets or sets the default value of the variation.

   .. code-block:: csharp

      public ISmiValue DefaultValue { get; set; }

   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiValue`

DefaultValueIdentifiers
~~~~~~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Variantion.DefaultValueIdentifiers

   Gets or sets the list of default value identifiers.

   .. code-block:: csharp

      public IList<string> DefaultValueIdentifiers { get; set; }

   :rtype: ``IList<String>``

Description
~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Variantion.Description

   Gets or sets the description of the variation.

   .. code-block:: csharp

      public string Description { get; }

   :rtype: ``String``

Syntax
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Variantion.Syntax

   Gets or sets the syntax type of the variation.

   .. code-block:: csharp

      public ISmiType Syntax { get; set; }

   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiType`

WriteSyntax
~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Variantion.WriteSyntax

   Gets or sets the write syntax type of the variation.

   .. code-block:: csharp

      public ISmiType WriteSyntax { get; set; }

   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiType`

