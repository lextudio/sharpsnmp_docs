SecurityParameters Class
========================

.. dn:class:: Lextm.SharpSnmpLib.SecurityParameters

   Legacy compatibility wrapper for SNMP security parameters.

   .. code-block:: csharp

      [Obsolete("This type is for internal use only and may be removed in a future release.")]
      public sealed class SecurityParameters

**Namespace:** ``Lextm.SharpSnmpLib``

**Inheritance:** Object → ``SecurityParameters``

**Source:** `SharpSnmpLib/SecurityParameters.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SecurityParameters.cs#L14>`__

Constructors
------------

SecurityParameters(Nullable<OctetString>, Nullable<Integer32>, Nullable<Integer32>, OctetString, Nullable<OctetString>, Nullable<OctetString>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.SecurityParameters..ctor(System.Nullable{DotNetSnmp.Asn1.SyntaxObjects.OctetString},System.Nullable{DotNetSnmp.Asn1.SyntaxObjects.Integer32},System.Nullable{DotNetSnmp.Asn1.SyntaxObjects.Integer32},DotNetSnmp.Asn1.SyntaxObjects.OctetString,System.Nullable{DotNetSnmp.Asn1.SyntaxObjects.OctetString},System.Nullable{DotNetSnmp.Asn1.SyntaxObjects.OctetString})

   Initializes a new instance of :dn:cls:``~Lextm.SharpSnmpLib.SecurityParameters``.

   .. code-block:: csharp

      public SecurityParameters(OctetString? engineId, Integer32? engineBoots, Integer32? engineTime, OctetString userName, OctetString? authenticationParameters, OctetString? privacyParameters)

   :type engineId: ``Nullable<OctetString>``
   :type engineBoots: ``Nullable<Integer32>``
   :type engineTime: ``Nullable<Integer32>``
   :type userName: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type authenticationParameters: ``Nullable<OctetString>``
   :type privacyParameters: ``Nullable<OctetString>``

**Source:** `SharpSnmpLib/SecurityParameters.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SecurityParameters.cs#L55>`__

Properties
----------

AuthenticationParameters
~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.SecurityParameters.AuthenticationParameters

   Gets authentication parameters.

   .. code-block:: csharp

      public OctetString? AuthenticationParameters { get; }

   :rtype: ``Nullable<OctetString>``

**Source:** `SharpSnmpLib/SecurityParameters.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SecurityParameters.cs#L40>`__

EngineBoots
~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.SecurityParameters.EngineBoots

   Gets engine boots.

   .. code-block:: csharp

      public Integer32 EngineBoots { get; }

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.Integer32`

**Source:** `SharpSnmpLib/SecurityParameters.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SecurityParameters.cs#L25>`__

EngineId
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.SecurityParameters.EngineId

   Gets engine id.

   .. code-block:: csharp

      public OctetString EngineId { get; }

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`

**Source:** `SharpSnmpLib/SecurityParameters.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SecurityParameters.cs#L20>`__

EngineTime
~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.SecurityParameters.EngineTime

   Gets engine time.

   .. code-block:: csharp

      public Integer32 EngineTime { get; }

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.Integer32`

**Source:** `SharpSnmpLib/SecurityParameters.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SecurityParameters.cs#L30>`__

IsInvalid
~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.SecurityParameters.IsInvalid

   Gets or sets a value indicating whether hashes are invalid.

   .. code-block:: csharp

      public bool IsInvalid { get; set; }

   :rtype: ``Boolean``

**Source:** `SharpSnmpLib/SecurityParameters.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SecurityParameters.cs#L50>`__

PrivacyParameters
~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.SecurityParameters.PrivacyParameters

   Gets privacy parameters.

   .. code-block:: csharp

      public OctetString? PrivacyParameters { get; }

   :rtype: ``Nullable<OctetString>``

**Source:** `SharpSnmpLib/SecurityParameters.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SecurityParameters.cs#L45>`__

UserName
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.SecurityParameters.UserName

   Gets user name (or community for v1/v2c).

   .. code-block:: csharp

      public OctetString UserName { get; }

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`

**Source:** `SharpSnmpLib/SecurityParameters.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SecurityParameters.cs#L35>`__

Methods
-------

Create(OctetString)
~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.SecurityParameters.Create(DotNetSnmp.Asn1.SyntaxObjects.OctetString)

   Creates community-based security parameters.

   .. code-block:: csharp

      public static SecurityParameters Create(OctetString userName)

   :type userName: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`

   :rtype: :dn:cls:`~Lextm.SharpSnmpLib.SecurityParameters`

**Source:** `SharpSnmpLib/SecurityParameters.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SecurityParameters.cs#L89>`__

