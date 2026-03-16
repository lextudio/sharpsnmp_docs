TimeTicksType Class
===================

.. dn:class:: Lextm.SharpSnmpPro.Mib.TimeTicksType

   Represents the TimeTicks basic type in SNMP MIBs.

   .. code-block:: csharp

      public class TimeTicksType : IBasicType, ISmiType, IConstruct

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``TimeTicksType``

Properties
----------

CharPositionInLine
~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.TimeTicksType.CharPositionInLine

   Gets the char position in line.

   .. code-block:: csharp

      public int CharPositionInLine { get; set; }

   :returns: The char position in line.
   :rtype: ``Int32``

Line
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.TimeTicksType.Line

   Gets the line number.

   .. code-block:: csharp

      public int Line { get; set; }

   :returns: The line.
   :rtype: ``Int32``

Module
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.TimeTicksType.Module

   Gets or sets the module.

   .. code-block:: csharp

      public Module Module { get; set; }

   :returns: The module.
   :rtype: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Module`

Name
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.TimeTicksType.Name

   Name.

   .. code-block:: csharp

      public string Name { get; set; }

   :rtype: ``String``

Methods
-------

Append(StringBuilder)
~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.TimeTicksType.Append(System.Text.StringBuilder)

   Appends the type name to the provided ``StringBuilder``.

   .. code-block:: csharp

      public void Append(StringBuilder typeName)

   :param typeName: The ``StringBuilder`` to append the type name to.
   :type typeName: ``StringBuilder``

VerifyData(IAsnSerializable)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.TimeTicksType.VerifyData(DotNetSnmp.Asn1.Serialization.IAsnSerializable)

   .. code-block:: csharp

      public bool VerifyData(IAsnSerializable data)

   :type data: :any:`IAsnSerializable <DotNetSnmp.Asn1.Serialization.IAsnSerializable>`

   :rtype: ``Boolean``

