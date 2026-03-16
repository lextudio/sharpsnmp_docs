CompatibilityExtensions Class
=============================

.. dn:class:: Lextm.SharpSnmpLib.CompatibilityExtensions

   Provides compatibility helpers for legacy SharpSnmpLib APIs.

   .. code-block:: csharp

      public static class CompatibilityExtensions

**Namespace:** ``Lextm.SharpSnmpLib``

**Inheritance:** Object → ``CompatibilityExtensions``

**Source:** `SharpSnmpLib/CompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/CompatibilityExtensions.cs#L12>`__

Methods
-------

GetRaw(OctetString)
~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.CompatibilityExtensions.GetRaw(DotNetSnmp.Asn1.SyntaxObjects.OctetString)

   Returns raw octets from :dn:struct:``~DotNetSnmp.Asn1.SyntaxObjects.OctetString``.

   .. code-block:: csharp

      public static byte[] GetRaw(this OctetString value)

   :rtype: ``Byte[]``

**Source:** `SharpSnmpLib/CompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/CompatibilityExtensions.cs#L80>`__

ToBytes(IAsnSerializable)
~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.CompatibilityExtensions.ToBytes(DotNetSnmp.Asn1.Serialization.IAsnSerializable)

   Serializes ASN.1 data to BER bytes (legacy helper signature).

   .. code-block:: csharp

      public static byte[] ToBytes(this IAsnSerializable value)

   :rtype: ``Byte[]``

**Source:** `SharpSnmpLib/CompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/CompatibilityExtensions.cs#L108>`__

ToErrorCode(ErrorCode)
~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.CompatibilityExtensions.ToErrorCode(DotNetSnmp.Common.Definitions.ErrorCode)

   Converts an :dn:enum:``~DotNetSnmp.Common.Definitions.ErrorCode`` value to itself (legacy helper signature).

   .. code-block:: csharp

      public static ErrorCode ToErrorCode(this ErrorCode value)

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.ErrorCode`

**Source:** `SharpSnmpLib/CompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/CompatibilityExtensions.cs#L33>`__

ToErrorCode(Integer32)
~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.CompatibilityExtensions.ToErrorCode(DotNetSnmp.Asn1.SyntaxObjects.Integer32)

   Converts an :dn:struct:``~DotNetSnmp.Asn1.SyntaxObjects.Integer32`` value to :dn:enum:``~DotNetSnmp.Common.Definitions.ErrorCode`` (legacy helper signature).

   .. code-block:: csharp

      public static ErrorCode ToErrorCode(this Integer32 value)

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.ErrorCode`

**Source:** `SharpSnmpLib/CompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/CompatibilityExtensions.cs#L41>`__

ToHexString(OctetString)
~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.CompatibilityExtensions.ToHexString(DotNetSnmp.Asn1.SyntaxObjects.OctetString)

   Returns the octets as uppercase hexadecimal text.

   .. code-block:: csharp

      public static string ToHexString(this OctetString value)

   :rtype: ``String``

**Source:** `SharpSnmpLib/CompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/CompatibilityExtensions.cs#L88>`__

ToInt32(ErrorCode)
~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.CompatibilityExtensions.ToInt32(DotNetSnmp.Common.Definitions.ErrorCode)

   Converts an :dn:enum:``~DotNetSnmp.Common.Definitions.ErrorCode`` value to ``Int32``.

   .. code-block:: csharp

      public static int ToInt32(this ErrorCode value)

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/CompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/CompatibilityExtensions.cs#L25>`__

ToInt32(Integer32)
~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.CompatibilityExtensions.ToInt32(DotNetSnmp.Asn1.SyntaxObjects.Integer32)

   Converts an :dn:struct:``~DotNetSnmp.Asn1.SyntaxObjects.Integer32`` value to ``Int32``.

   .. code-block:: csharp

      public static int ToInt32(this Integer32 value)

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/CompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/CompatibilityExtensions.cs#L17>`__

TryToErrorCode(Integer32, out ErrorCode)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.CompatibilityExtensions.TryToErrorCode(DotNetSnmp.Asn1.SyntaxObjects.Integer32,DotNetSnmp.Common.Definitions.ErrorCode@)

   Tries to convert an :dn:struct:``~DotNetSnmp.Asn1.SyntaxObjects.Integer32`` value to :dn:enum:``~DotNetSnmp.Common.Definitions.ErrorCode``.

   .. code-block:: csharp

      public static bool TryToErrorCode(this Integer32 value, scoped out ErrorCode code)

   :type code: :dn:enum:`~DotNetSnmp.Common.Definitions.ErrorCode`

   :rtype: ``Boolean``

**Source:** `SharpSnmpLib/CompatibilityExtensions.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/CompatibilityExtensions.cs#L58>`__

