AsnTypes Class
==============

.. dn:class:: DotNetSnmp.Asn1.Serialization.AsnTypes

   Defines ASN.1 tags used by SNMP syntax values, including opaque extension tags.

   .. code-block:: csharp

      public static class AsnTypes

**Namespace:** ``DotNetSnmp.Asn1.Serialization``

**Inheritance:** Object → ``AsnTypes``

**Source:** `SharpSnmpLib/Asn1/AsnTypes.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/AsnTypes.cs#L7>`__

Fields
------

AsnContext
~~~~~~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.AsnTypes.AsnContext

   The ASN.1 context-specific class bit mask used by opaque extension tags.

   .. code-block:: csharp

      public const byte AsnContext = 128

   :rtype: ``Byte``

**Source:** `SharpSnmpLib/Asn1/AsnTypes.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/AsnTypes.cs#L68>`__

AsnExtensionId
~~~~~~~~~~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.AsnTypes.AsnExtensionId

   The low-bit extension marker for multi-octet tag identifiers.

   .. code-block:: csharp

      public const byte AsnExtensionId = 31

   :rtype: ``Byte``

**Source:** `SharpSnmpLib/Asn1/AsnTypes.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/AsnTypes.cs#L73>`__

AsnOpaqueCounter64TagValue
~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.AsnTypes.AsnOpaqueCounter64TagValue

   The second-octet tag value for opaque Counter64 extension values.

   .. code-block:: csharp

      public const int AsnOpaqueCounter64TagValue = 118

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Asn1/AsnTypes.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/AsnTypes.cs#L102>`__

AsnOpaqueDoubleTagValue
~~~~~~~~~~~~~~~~~~~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.AsnTypes.AsnOpaqueDoubleTagValue

   The second-octet tag value for opaque Double extension values.

   .. code-block:: csharp

      public const int AsnOpaqueDoubleTagValue = 121

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Asn1/AsnTypes.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/AsnTypes.cs#L114>`__

AsnOpaqueFloatTagValue
~~~~~~~~~~~~~~~~~~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.AsnTypes.AsnOpaqueFloatTagValue

   The second-octet tag value for opaque Float extension values.

   .. code-block:: csharp

      public const int AsnOpaqueFloatTagValue = 120

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Asn1/AsnTypes.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/AsnTypes.cs#L108>`__

AsnOpaqueInteger64TagValue
~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.AsnTypes.AsnOpaqueInteger64TagValue

   The second-octet tag value for opaque signed 64-bit extension values.

   .. code-block:: csharp

      public const int AsnOpaqueInteger64TagValue = 122

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Asn1/AsnTypes.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/AsnTypes.cs#L120>`__

AsnOpaqueTag1
~~~~~~~~~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.AsnTypes.AsnOpaqueTag1

   First octet of the tag

   .. code-block:: csharp

      public const byte AsnOpaqueTag1 = 159

   :rtype: ``Byte``

**Source:** `SharpSnmpLib/Asn1/AsnTypes.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/AsnTypes.cs#L78>`__

AsnOpaqueTag2
~~~~~~~~~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.AsnTypes.AsnOpaqueTag2

   Base value for the second octet of the tag the second octet is the value for the tag

   .. code-block:: csharp

      public const byte AsnOpaqueTag2 = 48

   :rtype: ``Byte``

**Source:** `SharpSnmpLib/Asn1/AsnTypes.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/AsnTypes.cs#L84>`__

AsnOpaqueTag2U
~~~~~~~~~~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.AsnTypes.AsnOpaqueTag2U

   Second octet of tag for unions

   .. code-block:: csharp

      public const byte AsnOpaqueTag2U = 47

   :rtype: ``Byte``

**Source:** `SharpSnmpLib/Asn1/AsnTypes.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/AsnTypes.cs#L89>`__

AsnOpaqueUnsigned64TagValue
~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.AsnTypes.AsnOpaqueUnsigned64TagValue

   The second-octet tag value for opaque unsigned 64-bit extension values.

   .. code-block:: csharp

      public const int AsnOpaqueUnsigned64TagValue = 123

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Asn1/AsnTypes.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/AsnTypes.cs#L126>`__

Counter32
~~~~~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.AsnTypes.Counter32

   The application tag for the Counter32 syntax.

   .. code-block:: csharp

      public static readonly Asn1Tag Counter32

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/Asn1/AsnTypes.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/AsnTypes.cs#L17>`__

Counter64
~~~~~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.AsnTypes.Counter64

   The application tag for the Counter64 syntax.

   .. code-block:: csharp

      public static readonly Asn1Tag Counter64

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/Asn1/AsnTypes.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/AsnTypes.cs#L42>`__

Double
~~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.AsnTypes.Double

   The application tag for the opaque floating-point extension (Double).

   .. code-block:: csharp

      public static readonly Asn1Tag Double

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/Asn1/AsnTypes.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/AsnTypes.cs#L62>`__

Float
~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.AsnTypes.Float

   The application tag for the opaque floating-point extension (Float).

   .. code-block:: csharp

      public static readonly Asn1Tag Float

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/Asn1/AsnTypes.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/AsnTypes.cs#L57>`__

Gauge32
~~~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.AsnTypes.Gauge32

   The application tag for the Gauge32 syntax.

   .. code-block:: csharp

      public static readonly Asn1Tag Gauge32

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/Asn1/AsnTypes.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/AsnTypes.cs#L22>`__

Integer32
~~~~~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.AsnTypes.Integer32

   The universal ASN.1 INTEGER tag used for Integer32.

   .. code-block:: csharp

      public static readonly Asn1Tag Integer32

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/Asn1/AsnTypes.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/AsnTypes.cs#L47>`__

IpAddress
~~~~~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.AsnTypes.IpAddress

   The application tag for the IpAddress syntax.

   .. code-block:: csharp

      public static readonly Asn1Tag IpAddress

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/Asn1/AsnTypes.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/AsnTypes.cs#L12>`__

Opaque
~~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.AsnTypes.Opaque

   The application tag for the Opaque syntax.

   .. code-block:: csharp

      public static readonly Asn1Tag Opaque

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/Asn1/AsnTypes.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/AsnTypes.cs#L37>`__

OpaqueCounter64
~~~~~~~~~~~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.AsnTypes.OpaqueCounter64

   The ASN.1 tag used to encode opaque Counter64 extension values.

   .. code-block:: csharp

      public static readonly Asn1Tag OpaqueCounter64

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/Asn1/AsnTypes.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/AsnTypes.cs#L132>`__

OpaqueDouble
~~~~~~~~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.AsnTypes.OpaqueDouble

   The ASN.1 tag used to encode opaque Double extension values.

   .. code-block:: csharp

      public static readonly Asn1Tag OpaqueDouble

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/Asn1/AsnTypes.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/AsnTypes.cs#L144>`__

OpaqueFloat
~~~~~~~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.AsnTypes.OpaqueFloat

   The ASN.1 tag used to encode opaque Float extension values.

   .. code-block:: csharp

      public static readonly Asn1Tag OpaqueFloat

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/Asn1/AsnTypes.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/AsnTypes.cs#L138>`__

OpaqueInteger64
~~~~~~~~~~~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.AsnTypes.OpaqueInteger64

   The ASN.1 tag used to encode opaque signed 64-bit extension values.

   .. code-block:: csharp

      public static readonly Asn1Tag OpaqueInteger64

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/Asn1/AsnTypes.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/AsnTypes.cs#L150>`__

OpaqueUnsigned64
~~~~~~~~~~~~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.AsnTypes.OpaqueUnsigned64

   The ASN.1 tag used to encode opaque unsigned 64-bit extension values.

   .. code-block:: csharp

      public static readonly Asn1Tag OpaqueUnsigned64

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/Asn1/AsnTypes.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/AsnTypes.cs#L156>`__

TimeTicks
~~~~~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.AsnTypes.TimeTicks

   The application tag for the TimeTicks syntax.

   .. code-block:: csharp

      public static readonly Asn1Tag TimeTicks

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/Asn1/AsnTypes.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/AsnTypes.cs#L32>`__

Unsigned32
~~~~~~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.AsnTypes.Unsigned32

   An alias for :dn:field:``~DotNetSnmp.Asn1.Serialization.AsnTypes.Gauge32`` used for the Unsigned32 syntax.

   .. code-block:: csharp

      public static readonly Asn1Tag Unsigned32

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/Asn1/AsnTypes.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/AsnTypes.cs#L27>`__

Unsigned64
~~~~~~~~~~

.. dn:field:: DotNetSnmp.Asn1.Serialization.AsnTypes.Unsigned64

   An alias for :dn:field:``~DotNetSnmp.Asn1.Serialization.AsnTypes.Counter64`` used for unsigned 64-bit values.

   .. code-block:: csharp

      public static readonly Asn1Tag Unsigned64

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/Asn1/AsnTypes.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/AsnTypes.cs#L52>`__

