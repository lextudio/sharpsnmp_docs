TaggedElementType Class
=======================

.. dn:class:: Lextm.SharpSnmpPro.Mib.TaggedElementType

   Represents a tagged element type in the MIB, which is derived from another type and can be validated.

   .. code-block:: csharp

      public class TaggedElementType : ElementType, IDerivedType, ISmiType, IConstruct, IValidatable

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ElementType → ``TaggedElementType``

Constructors
------------

TaggedElementType(String)
~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.TaggedElementType..ctor(System.String)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.TaggedElementType`` class with the specified name.

   .. code-block:: csharp

      public TaggedElementType(string name)

   :param name: The name of the tagged element type.
   :type name: ``String``

Properties
----------

BaseType
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.TaggedElementType.BaseType

   Gets or sets the base type of this tagged element type. This property is set during validation and represents the type that this tagged element derives from.

   .. code-block:: csharp

      public ISmiType BaseType { get; set; }

   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.ISmiType`

Methods
-------

Validate(ICollection<IConstruct>, ErrorRegistry)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.TaggedElementType.Validate(System.Collections.Generic.ICollection{Lextm.SharpSnmpPro.Mib.IConstruct},Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry)

   Validates this entity.

   .. code-block:: csharp

      public void Validate(ICollection<IConstruct> knownConstructs, ErrorRegistry registry)

   :param knownConstructs: Known constructs.
   :type knownConstructs: ``ICollection<IConstruct>``
   :param registry: The registry.
   :type registry: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry`

