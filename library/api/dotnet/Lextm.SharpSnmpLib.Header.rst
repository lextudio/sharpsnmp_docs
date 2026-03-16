Header Class
============

.. dn:class:: Lextm.SharpSnmpLib.Header

   Legacy compatibility wrapper for SNMP v3 header data.

   .. code-block:: csharp

      [Obsolete("This type is for internal use only and may be removed in a future release.")]
      public sealed class Header

**Namespace:** ``Lextm.SharpSnmpLib``

**Inheritance:** Object → ``Header``

**Source:** `SharpSnmpLib/Header.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Header.cs#L12>`__

Constructors
------------

Header(Nullable<Integer32>, Integer32, Levels)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Header..ctor(System.Nullable{DotNetSnmp.Asn1.SyntaxObjects.Integer32},DotNetSnmp.Asn1.SyntaxObjects.Integer32,DotNetSnmp.Common.Definitions.Levels)

   Initializes a new instance of :dn:cls:``~Lextm.SharpSnmpLib.Header``.

   .. code-block:: csharp

      public Header(Integer32? messageId, Integer32 maxMessageSize, Levels securityLevel)

   :type messageId: ``Nullable<Integer32>``
   :type maxMessageSize: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.Integer32`
   :type securityLevel: :dn:enum:`~DotNetSnmp.Common.Definitions.Levels`

**Source:** `SharpSnmpLib/Header.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Header.cs#L44>`__

Fields
------

MaxMessageSize
~~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpLib.Header.MaxMessageSize

   Max message size used by legacy #SNMP APIs.

   .. code-block:: csharp

      public const int MaxMessageSize = 65507

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Header.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Header.cs#L18>`__

Properties
----------

Empty
~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Header.Empty

   Empty header for v1/v2c messages.

   .. code-block:: csharp

      public static Header Empty { get; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpLib.Header`

**Source:** `SharpSnmpLib/Header.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Header.cs#L54>`__

MaxSize
~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Header.MaxSize

   Gets maximum message size.

   .. code-block:: csharp

      public int MaxSize { get; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Header.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Header.cs#L69>`__

MessageId
~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Header.MessageId

   Gets message id.

   .. code-block:: csharp

      public int MessageId { get; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Header.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Header.cs#L64>`__

SecurityLevel
~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Header.SecurityLevel

   Gets security flags.

   .. code-block:: csharp

      public Levels SecurityLevel { get; }

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.Levels`

**Source:** `SharpSnmpLib/Header.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Header.cs#L59>`__

