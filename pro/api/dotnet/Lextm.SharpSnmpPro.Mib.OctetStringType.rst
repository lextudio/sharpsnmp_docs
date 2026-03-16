OctetStringType Class
=====================

.. dn:class:: Lextm.SharpSnmpPro.Mib.OctetStringType

   Represents the OCTET STRING type in SMI, with optional BITS support.

   .. code-block:: csharp

      public class OctetStringType : IBasicType, ISmiType, IConstruct, IConstraintable

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``OctetStringType``

Properties
----------

CharPositionInLine
~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.OctetStringType.CharPositionInLine

   Gets the char position in line.

   .. code-block:: csharp

      public int CharPositionInLine { get; set; }

   :returns: The char position in line.
   :rtype: ``Int32``

Line
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.OctetStringType.Line

   Gets the line number.

   .. code-block:: csharp

      public int Line { get; set; }

   :returns: The line.
   :rtype: ``Int32``

Module
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.OctetStringType.Module

   Gets or sets the module.

   .. code-block:: csharp

      public Module Module { get; set; }

   :returns: The module.
   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Module`

Name
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.OctetStringType.Name

   Name.

   .. code-block:: csharp

      public string Name { get; set; }

   :rtype: ``String``

NamedBits
~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.OctetStringType.NamedBits

   Gets or sets the named bits for BITS type.

   .. code-block:: csharp

      public IList<NamedBit> NamedBits { get; set; }

   :rtype: ``IList<NamedBit>``

Methods
-------

Append(StringBuilder)
~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.OctetStringType.Append(System.Text.StringBuilder)

   Appends the type name &quot;OCTET STRING&quot; to the provided ``StringBuilder``.

   .. code-block:: csharp

      public void Append(StringBuilder typeName)

   :param typeName: The ``StringBuilder`` to append to.
   :type typeName: ``StringBuilder``

VerifyData(IAsnSerializable)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.OctetStringType.VerifyData(DotNetSnmp.Asn1.Serialization.IAsnSerializable)

   .. code-block:: csharp

      public bool VerifyData(IAsnSerializable data)

   :type data: :any:`IAsnSerializable <DotNetSnmp.Asn1.Serialization.IAsnSerializable>`

   :rtype: ``Boolean``

