IEntity Interface
=================

.. dn:interface:: Lextm.SharpSnmpPro.Mib.IEntity

   Entity interface.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public interface IEntity : IConstruct, IValidatable

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

Properties
----------

Description
~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.IEntity.Description

   Provides a textual description of the item being defined.

   .. code-block:: csharp

      string Description { get; }

   :rtype: ``String``

ObjectIdentifier
~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.IEntity.ObjectIdentifier

   Gets or sets the object identifier.

   .. code-block:: csharp

      [CLSCompliant(false)]
      [Obsolete("Please use GetObjectIdentifier method.")]
      uint[] ObjectIdentifier { get; set; }

   :returns: The object identifier.
   :rtype: ``UInt32[]``

Parent
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.IEntity.Parent

   Gets or sets the parent.

   .. code-block:: csharp

      IEntity Parent { get; set; }

   :returns: The parent.
   :rtype: :dn:iface:`~Lextm.SharpSnmpPro.Mib.IEntity`

Reference
~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.IEntity.Reference

   Specifies the source of the definition (such as a document from another standards organization, or an architectural document for a proprietary system).

   .. code-block:: csharp

      string Reference { get; }

   :rtype: ``String``

Status
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.IEntity.Status

   Status.

   .. code-block:: csharp

      EntityStatus Status { get; }

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.EntityStatus`

Value
~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.IEntity.Value

   Gets or sets the value.

   .. code-block:: csharp

      [CLSCompliant(false)]
      uint Value { get; set; }

   :returns: The value.
   :rtype: ``UInt32``

Values
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.IEntity.Values

   Gets or sets the list of ID components.

   .. code-block:: csharp

      IdComponentList Values { get; set; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.IdComponentList`

Verified
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.IEntity.Verified

   Gets or sets the verification status of an entity.

   .. code-block:: csharp

      VerificationStatus Verified { get; set; }

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.VerificationStatus`

