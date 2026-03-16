EndOfMibView Struct
===================

.. dn:struct:: DotNetSnmp.Asn1.SyntaxObjects.EndOfMibView

   Represents the EndOfMibView type.

   .. code-block:: csharp

      public readonly record struct EndOfMibView : IAsnSerializable, IEquatable<EndOfMibView>

**Namespace:** ``DotNetSnmp.Asn1.SyntaxObjects``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/EndOfMibView.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/EndOfMibView.cs#L8>`__

Methods
-------

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.EndOfMibView.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public readonly void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/EndOfMibView.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/EndOfMibView.cs#L11>`__

