NamedBit Class
==============

.. dn:class:: Lextm.SharpSnmpPro.Mib.NamedBit

   Represents a named bit value in an SNMP MIB.

   .. code-block:: csharp

      public class NamedBit : ISmiValue

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``NamedBit``

Constructors
------------

NamedBit(String, UInt64)
~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.NamedBit..ctor(System.String,System.UInt64)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.NamedBit`` class with the specified name and bit number.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public NamedBit(string name, ulong bit)

   :param name: The name of the bit.
   :type name: ``String``
   :param bit: The bit number.
   :type bit: ``UInt64``

NamedBit(String)
~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.NamedBit..ctor(System.String)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.NamedBit`` class with the specified name and a bit number of 0.

   .. code-block:: csharp

      public NamedBit(string name)

   :param name: The name of the bit.
   :type name: ``String``

Properties
----------

Minus
~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.NamedBit.Minus

   Gets or sets a value indicating whether the bit is negative.

   .. code-block:: csharp

      public bool Minus { get; set; }

   :rtype: ``Boolean``

Name
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.NamedBit.Name

   Gets the name of the bit.

   .. code-block:: csharp

      public string Name { get; }

   :rtype: ``String``

Number
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.NamedBit.Number

   Gets or sets the bit number.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public ulong Number { get; set; }

   :rtype: ``UInt64``

