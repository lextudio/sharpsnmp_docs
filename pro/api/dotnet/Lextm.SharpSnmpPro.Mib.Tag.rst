Tag Class
=========

.. dn:class:: Lextm.SharpSnmpPro.Mib.Tag

   Represents a tag with a type and a class number in the SNMP MIB context.

   .. code-block:: csharp

      public class Tag

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``Tag``

Properties
----------

TagNumber
~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Tag.TagNumber

   Gets or sets the class number associated with the tag.

   .. code-block:: csharp

      public ClassNumber TagNumber { get; set; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.ClassNumber`

TagType
~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Tag.TagType

   Gets or sets the tag type.

   .. code-block:: csharp

      public string TagType { get; set; }

   :rtype: ``String``

