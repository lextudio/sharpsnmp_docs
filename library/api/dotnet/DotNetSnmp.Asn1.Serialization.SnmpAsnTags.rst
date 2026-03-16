SnmpAsnTags Class
=================

.. dn:class:: DotNetSnmp.Asn1.Serialization.SnmpAsnTags

   Defines ASN.1 context-specific tags used by SNMP PDUs and exception syntax values.

   .. code-block:: csharp

      public static class SnmpAsnTags

**Namespace:** ``DotNetSnmp.Asn1.Serialization``

**Inheritance:** Object → ``SnmpAsnTags``

**Source:** `SharpSnmpLib/Asn1/SnmpAsnTags.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SnmpAsnTags.cs#L7>`__

Fields
------

BulkMsg
~~~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.SnmpAsnTags.BulkMsg

   The tag for a GetBulkRequest-PDU.

   .. code-block:: csharp

      public static readonly Asn1Tag BulkMsg

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/Asn1/SnmpAsnTags.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SnmpAsnTags.cs#L50>`__

EndOfMibView
~~~~~~~~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.SnmpAsnTags.EndOfMibView

   The exception tag used when the end of the MIB view is reached during lexicographic traversal.

   .. code-block:: csharp

      public static readonly Asn1Tag EndOfMibView

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/Asn1/SnmpAsnTags.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SnmpAsnTags.cs#L91>`__

GetMsg
~~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.SnmpAsnTags.GetMsg

   The tag for a GetRequest-PDU.

   .. code-block:: csharp

      public static readonly Asn1Tag GetMsg

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/Asn1/SnmpAsnTags.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SnmpAsnTags.cs#L14>`__

GetNextMsg
~~~~~~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.SnmpAsnTags.GetNextMsg

   The tag for a GetNextRequest-PDU.

   .. code-block:: csharp

      public static readonly Asn1Tag GetNextMsg

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/Asn1/SnmpAsnTags.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SnmpAsnTags.cs#L20>`__

GetResponseMsg
~~~~~~~~~~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.SnmpAsnTags.GetResponseMsg

   The tag for a GetResponse-PDU.

   .. code-block:: csharp

      public static readonly Asn1Tag GetResponseMsg

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/Asn1/SnmpAsnTags.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SnmpAsnTags.cs#L26>`__

InformMsg
~~~~~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.SnmpAsnTags.InformMsg

   The tag for an InformRequest-PDU.

   .. code-block:: csharp

      public static readonly Asn1Tag InformMsg

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/Asn1/SnmpAsnTags.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SnmpAsnTags.cs#L56>`__

NoSuchInstance
~~~~~~~~~~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.SnmpAsnTags.NoSuchInstance

   The exception tag used when an object exists but has no instance at the requested index.

   .. code-block:: csharp

      public static readonly Asn1Tag NoSuchInstance

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/Asn1/SnmpAsnTags.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SnmpAsnTags.cs#L85>`__

NoSuchObject
~~~~~~~~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.SnmpAsnTags.NoSuchObject

   The exception tag used when a referenced object identifier does not exist.

   .. code-block:: csharp

      public static readonly Asn1Tag NoSuchObject

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/Asn1/SnmpAsnTags.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SnmpAsnTags.cs#L79>`__

ReportMsg
~~~~~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.SnmpAsnTags.ReportMsg

   The tag for a Report-PDU.

   .. code-block:: csharp

      public static readonly Asn1Tag ReportMsg

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/Asn1/SnmpAsnTags.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SnmpAsnTags.cs#L71>`__

SetMsg
~~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.SnmpAsnTags.SetMsg

   The tag for a SetRequest-PDU.

   .. code-block:: csharp

      public static readonly Asn1Tag SetMsg

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/Asn1/SnmpAsnTags.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SnmpAsnTags.cs#L32>`__

Trap2Msg
~~~~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.SnmpAsnTags.Trap2Msg

   The tag for an SNMPv2 Trap-PDU.

   .. code-block:: csharp

      public static readonly Asn1Tag Trap2Msg

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/Asn1/SnmpAsnTags.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SnmpAsnTags.cs#L62>`__

TrapMsg
~~~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.SnmpAsnTags.TrapMsg

   The tag for an SNMPv1 Trap-PDU.

   .. code-block:: csharp

      public static readonly Asn1Tag TrapMsg

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/Asn1/SnmpAsnTags.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SnmpAsnTags.cs#L41>`__

