Null Struct
===========

.. dn:struct:: DotNetSnmp.Asn1.SyntaxObjects.Null

   Represents the Null type.

   .. code-block:: csharp

      public readonly record struct Null : IAsnSerializable, IEquatable<Null>

**Namespace:** ``DotNetSnmp.Asn1.SyntaxObjects``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Null.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Null.cs#L8>`__

Fields
------

Instance
~~~~~~~~

.. dn:field:: DotNetSnmp.Asn1.SyntaxObjects.Null.Instance

   A reusable SNMP NULL value instance.

   .. code-block:: csharp

      public static readonly Null Instance

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.Null`

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Null.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Null.cs#L13>`__

Methods
-------

ToString()
~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.Null.ToString

   Returns a ``String`` that represents this :dn:struct:``~DotNetSnmp.Asn1.SyntaxObjects.Null``.

   .. code-block:: csharp

      public readonly override string ToString()

   :rtype: ``String``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Null.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Null.cs#L24>`__

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.Null.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public readonly void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/Null.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/Null.cs#L16>`__

