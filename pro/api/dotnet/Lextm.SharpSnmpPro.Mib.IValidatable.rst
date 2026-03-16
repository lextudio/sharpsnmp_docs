IValidatable Interface
======================

.. dn:interface:: Lextm.SharpSnmpPro.Mib.IValidatable

   Validable interface. Types implementing this interface can be validated against rules.

   .. code-block:: csharp

      public interface IValidatable

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

Methods
-------

Validate(ICollection<IConstruct>, ErrorRegistry)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.IValidatable.Validate(System.Collections.Generic.ICollection{Lextm.SharpSnmpPro.Mib.IConstruct},Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry)

   Validates this entity.

   .. code-block:: csharp

      void Validate(ICollection<IConstruct> knownConstructs, ErrorRegistry registry)

   :param knownConstructs: Known constructs.
   :type knownConstructs: ``ICollection<IConstruct>``
   :param registry: The registry.
   :type registry: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry`

