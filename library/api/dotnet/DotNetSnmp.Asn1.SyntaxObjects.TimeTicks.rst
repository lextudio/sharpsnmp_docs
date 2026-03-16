TimeTicks Struct
================

.. dn:struct:: DotNetSnmp.Asn1.SyntaxObjects.TimeTicks

   The TimeTicks type represents a non-negative integer which represents the time, modulo 2^32 (4294967296 decimal), in hundredths of a second between two epochs.When objects are defined which use this ASN.1 type, the description of the object identifies both of the reference epochs.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public readonly record struct TimeTicks(uint Value) : IAsnSerializable, IEquatable<TimeTicks>

**Namespace:** ``DotNetSnmp.Asn1.SyntaxObjects``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/TimeTicks.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/TimeTicks.cs#L13>`__

Constructors
------------

TimeTicks(UInt32)
~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Asn1.SyntaxObjects.TimeTicks..ctor(System.UInt32)

   The TimeTicks type represents a non-negative integer which represents the time, modulo 2^32 (4294967296 decimal), in hundredths of a second between two epochs.When objects are defined which use this ASN.1 type, the description of the object identifies both of the reference epochs.

   .. code-block:: csharp

      public TimeTicks(uint Value)

   :type Value: ``UInt32``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/TimeTicks.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/TimeTicks.cs#L13>`__

Properties
----------

Value
~~~~~

.. dn:property:: DotNetSnmp.Asn1.SyntaxObjects.TimeTicks.Value

   .. code-block:: csharp

      public uint Value { get; init; }

   :rtype: ``UInt32``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/TimeTicks.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/TimeTicks.cs#L14>`__

Methods
-------

ReadFrom(AsnReader)
~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.TimeTicks.ReadFrom(System.Formats.Asn1.AsnReader)

   Reads a value from an ASN.1 reader.

   .. code-block:: csharp

      public static TimeTicks ReadFrom(AsnReader reader)

   :type reader: ``AsnReader``

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.TimeTicks`

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/TimeTicks.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/TimeTicks.cs#L26>`__

ToString()
~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.TimeTicks.ToString

   Returns a ``String`` that represents this :dn:struct:``~DotNetSnmp.Asn1.SyntaxObjects.TimeTicks``.

   .. code-block:: csharp

      public readonly override string ToString()

   :rtype: ``String``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/TimeTicks.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/TimeTicks.cs#L37>`__

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.TimeTicks.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public readonly void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/TimeTicks.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/TimeTicks.cs#L17>`__

Operators
---------

Implicit(TimeTicks to UInt32)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:operator:: DotNetSnmp.Asn1.SyntaxObjects.TimeTicks.op_Implicit(DotNetSnmp.Asn1.SyntaxObjects.TimeTicks)

   Performs a conversion to uint.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public static implicit operator uint (TimeTicks t)

   :type t: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.TimeTicks`

   :rtype: ``UInt32``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/TimeTicks.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/TimeTicks.cs#L45>`__

