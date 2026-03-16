HeaderData Class
================

.. dn:class:: DotNetSnmp.Protocol.V3.HeaderData

   Represents the HeaderData type.

   .. code-block:: csharp

      public class HeaderData : IAsnSerializable

**Namespace:** ``DotNetSnmp.Protocol.V3``

**Inheritance:** Object → ``HeaderData``

**Source:** `SharpSnmpLib/V3/HeaderData.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/HeaderData.cs#L11>`__

Properties
----------

MsgFlags
~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.HeaderData.MsgFlags

   Gets msg Flags.

   .. code-block:: csharp

      public MsgFlag MsgFlags { get; set; }

   :rtype: :dn:enum:`~DotNetSnmp.Protocol.V3.Security.MsgFlag`

**Source:** `SharpSnmpLib/V3/HeaderData.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/HeaderData.cs#L27>`__

MsgId
~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.HeaderData.MsgId

   Gets msg Id.

   .. code-block:: csharp

      public int MsgId { get; set; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/V3/HeaderData.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/HeaderData.cs#L16>`__

MsgMaxSize
~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.HeaderData.MsgMaxSize

   Gets msg Max Size.

   .. code-block:: csharp

      [Range(384, 2147483647)]
      public int MsgMaxSize { get; set; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/V3/HeaderData.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/HeaderData.cs#L21>`__

MsgSecurityModel
~~~~~~~~~~~~~~~~

.. dn:property:: DotNetSnmp.Protocol.V3.HeaderData.MsgSecurityModel

   Gets msg Security Model.

   .. code-block:: csharp

      [Range(1, 2147483647)]
      public SecurityModel MsgSecurityModel { get; set; }

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.SecurityModel`

**Source:** `SharpSnmpLib/V3/HeaderData.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/HeaderData.cs#L32>`__

Methods
-------

ReadFrom(AsnReader)
~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.HeaderData.ReadFrom(System.Formats.Asn1.AsnReader)

   Reads a value from an ASN.1 reader.

   .. code-block:: csharp

      public static HeaderData ReadFrom(AsnReader reader)

   :type reader: ``AsnReader``

   :rtype: :dn:cls:`~DotNetSnmp.Protocol.V3.HeaderData`

**Source:** `SharpSnmpLib/V3/HeaderData.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/HeaderData.cs#L55>`__

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Protocol.V3.HeaderData.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/V3/HeaderData.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/V3/HeaderData.cs#L36>`__

