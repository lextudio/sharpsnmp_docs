AsnMember Class
===============

.. dn:class:: DotNetSnmp.Utils.AsnMember

   Represents the AsnMember type.

   .. code-block:: csharp

      public record AsnMember : IEquatable<AsnMember>

**Namespace:** ``DotNetSnmp.Utils``

**Inheritance:** Object → ``AsnMember``

**Source:** `SharpSnmpLib/Utils/BERUtils.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Utils/BERUtils.cs#L10>`__

Properties
----------

BerHeaderLen
~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Utils.AsnMember.BerHeaderLen

   Gets ber Header Len.

   .. code-block:: csharp

      public int BerHeaderLen { get; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Utils/BERUtils.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Utils/BERUtils.cs#L63>`__

ContentLen
~~~~~~~~~~

.. dn:property:: DotNetSnmp.Utils.AsnMember.ContentLen

   Gets content Len.

   .. code-block:: csharp

      public int ContentLen { get; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Utils/BERUtils.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Utils/BERUtils.cs#L68>`__

ContentSize
~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Utils.AsnMember.ContentSize

   Gets content Size.

   .. code-block:: csharp

      public int ContentSize { get; init; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Utils/BERUtils.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Utils/BERUtils.cs#L28>`__

HeaderSize
~~~~~~~~~~

.. dn:property:: DotNetSnmp.Utils.AsnMember.HeaderSize

   Gets header Size.

   .. code-block:: csharp

      public int HeaderSize { get; init; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Utils/BERUtils.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Utils/BERUtils.cs#L23>`__

IndentLevel
~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Utils.AsnMember.IndentLevel

   Gets indent Level.

   .. code-block:: csharp

      public int IndentLevel { get; set; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Utils/BERUtils.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Utils/BERUtils.cs#L58>`__

Offset
~~~~~~

.. dn:property:: DotNetSnmp.Utils.AsnMember.Offset

   Gets offset.

   .. code-block:: csharp

      public int Offset { get; init; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Utils/BERUtils.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Utils/BERUtils.cs#L33>`__

OffsetEnd
~~~~~~~~~

.. dn:property:: DotNetSnmp.Utils.AsnMember.OffsetEnd

   Represents content Size.

   .. code-block:: csharp

      public int OffsetEnd { get; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Utils/BERUtils.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Utils/BERUtils.cs#L73>`__

Tag
~~~

.. dn:property:: DotNetSnmp.Utils.AsnMember.Tag

   Gets tag.

   .. code-block:: csharp

      public Asn1Tag Tag { get; init; }

   :rtype: ``Asn1Tag``

**Source:** `SharpSnmpLib/Utils/BERUtils.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Utils/BERUtils.cs#L18>`__

TagColor
~~~~~~~~

.. dn:property:: DotNetSnmp.Utils.AsnMember.TagColor

   Gets tag Color.

   .. code-block:: csharp

      public string TagColor { get; set; }

   :rtype: ``String``

**Source:** `SharpSnmpLib/Utils/BERUtils.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Utils/BERUtils.cs#L48>`__

TagLabel
~~~~~~~~

.. dn:property:: DotNetSnmp.Utils.AsnMember.TagLabel

   Gets tag Label.

   .. code-block:: csharp

      public string TagLabel { get; set; }

   :rtype: ``String``

**Source:** `SharpSnmpLib/Utils/BERUtils.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Utils/BERUtils.cs#L38>`__

ValueColor
~~~~~~~~~~

.. dn:property:: DotNetSnmp.Utils.AsnMember.ValueColor

   Gets value Color.

   .. code-block:: csharp

      public string ValueColor { get; set; }

   :rtype: ``String``

**Source:** `SharpSnmpLib/Utils/BERUtils.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Utils/BERUtils.cs#L53>`__

ValueLabel
~~~~~~~~~~

.. dn:property:: DotNetSnmp.Utils.AsnMember.ValueLabel

   Gets value Label.

   .. code-block:: csharp

      public string ValueLabel { get; set; }

   :rtype: ``String``

**Source:** `SharpSnmpLib/Utils/BERUtils.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Utils/BERUtils.cs#L43>`__

Methods
-------

ToString()
~~~~~~~~~~

.. dn:method:: DotNetSnmp.Utils.AsnMember.ToString

   Returns a string representation of the current value.

   .. code-block:: csharp

      public override string ToString()

   :rtype: ``String``

**Source:** `SharpSnmpLib/Utils/BERUtils.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Utils/BERUtils.cs#L78>`__

