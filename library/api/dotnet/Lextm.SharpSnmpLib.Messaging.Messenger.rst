Messenger Class
===============

.. dn:class:: Lextm.SharpSnmpLib.Messaging.Messenger

   Messenger class contains all static helper methods you need to send out SNMP messages. Static methods in Manager or Agent class will be removed in the future.

   .. code-block:: csharp

      public static class Messenger

**Namespace:** ``Lextm.SharpSnmpLib.Messaging``

**Inheritance:** Object → ``Messenger``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L19>`__

Properties
----------

AuthenticationFailure
~~~~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.Messenger.AuthenticationFailure

   If the authentication module returns failure, then the message cannot be trusted, so the usmStatsWrongDigests counter is incremented and an error indication (authenticationFailure) together with the OID and value of the incremented counter is returned to the calling module.

   .. code-block:: csharp

      public static ObjectIdentifier AuthenticationFailure { get; }

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L84>`__

DecryptionError
~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.Messenger.DecryptionError

   If the privacy module returns failure, then the message can not be processed, so the usmStatsDecryptionErrors counter is incremented and an error indication (decryptionError) together with the OID and value of the incremented counter is returned to the calling module.

   .. code-block:: csharp

      public static ObjectIdentifier DecryptionError { get; }

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L75>`__

MaxMessageSize
~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.Messenger.MaxMessageSize

   Max message size used in #SNMP.

   .. code-block:: csharp

      public static int MaxMessageSize { get; set; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L66>`__

NextMessageId
~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.Messenger.NextMessageId

   Represents next Id.

   .. code-block:: csharp

      public static int NextMessageId { get; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L61>`__

NextRequestId
~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.Messenger.NextRequestId

   Represents next Id.

   .. code-block:: csharp

      public static int NextRequestId { get; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L56>`__

NotInTimeWindow
~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.Messenger.NotInTimeWindow

   If the message is considered to be outside of the Time Window then the usmStatsNotInTimeWindows counter is incremented and an error indication (notInTimeWindow) together with the OID, the value of the incremented counter, and an indication that the error must be reported with a securityLevel of authNoPriv, is returned to the calling module

   .. code-block:: csharp

      public static ObjectIdentifier NotInTimeWindow { get; }

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L115>`__

RequestCounter
~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.Messenger.RequestCounter

   The universal counter for request IDs and other IDs.

   .. code-block:: csharp

      public static NumberGenerator RequestCounter { get; set; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpLib.Messaging.NumberGenerator`

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L36>`__

UnknownEngineId
~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.Messenger.UnknownEngineId

   If the value of the msgAuthoritativeEngineID field in the securityParameters is unknown then the usmStatsUnknownEngineIDs counter is incremented, and an error indication (unknownEngineID) together with the OID and value of the incremented counter is returned to the calling module.

   .. code-block:: csharp

      public static ObjectIdentifier UnknownEngineId { get; }

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L94>`__

UnknownSecurityName
~~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.Messenger.UnknownSecurityName

   Information about the value of the msgUserName and msgAuthoritativeEngineID fields is extracted from the Local Configuration Datastore (LCD, usmUserTable). If no information is available for the user, then the usmStatsUnknownUserNames counter is incremented and an error indication (unknownSecurityName) together with the OID and value of the incremented counter is returned to the calling module.

   .. code-block:: csharp

      public static ObjectIdentifier UnknownSecurityName { get; }

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L105>`__

UnsupportedSecurityLevel
~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.Messenger.UnsupportedSecurityLevel

   If the information about the user indicates that it does not support the securityLevel requested by the caller, then the usmStatsUnsupportedSecLevels counter is incremented and an error indication (unsupportedSecurityLevel) together with the OID and value of the incremented counter is returned to the calling module.

   .. code-block:: csharp

      public static ObjectIdentifier UnsupportedSecurityLevel { get; }

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L125>`__

UseFullRange
~~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.Messenger.UseFullRange

   A flag to control request ID range.

   .. code-block:: csharp

      public static bool UseFullRange { get; set; }

   :rtype: ``Boolean``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L51>`__

Methods
-------

BulkWalk(VersionCode, IPEndPoint, OctetString, OctetString, ObjectIdentifier, IList<Variable>, Int32, Int32, WalkMode, IPrivacyProvider?, ISnmpMessage?, ISnmpTransport)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.BulkWalk(DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},System.Int32,System.Int32,Lextm.SharpSnmpLib.Messaging.WalkMode,DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider,DotNetSnmp.Common.Definitions.ISnmpMessage,DotNetSnmp.Transport.ISnmpTransport)

   Performs a bulk walk operation using the specified transport.

   .. code-block:: csharp

      public static int BulkWalk(VersionCode version, IPEndPoint endpoint, OctetString community, OctetString contextName, ObjectIdentifier table, IList<Variable> list, int timeout, int maxRepetitions, WalkMode mode, IPrivacyProvider? privacy, ISnmpMessage? report, ISnmpTransport transport)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type endpoint: ``IPEndPoint``
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type contextName: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type table: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type list: ``IList<Variable>``
   :type timeout: ``Int32``
   :type maxRepetitions: ``Int32``
   :type mode: :dn:enum:`~Lextm.SharpSnmpLib.Messaging.WalkMode`
   :type privacy: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`
   :type report: :dn:iface:`~DotNetSnmp.Common.Definitions.ISnmpMessage`
   :type transport: :dn:iface:`~DotNetSnmp.Transport.ISnmpTransport`

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L779>`__

BulkWalk(VersionCode, IPEndPoint, OctetString, OctetString, ObjectIdentifier, IList<Variable>, Int32, Int32, WalkMode, IPrivacyProvider?, ISnmpMessage?)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.BulkWalk(DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},System.Int32,System.Int32,Lextm.SharpSnmpLib.Messaging.WalkMode,DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider,DotNetSnmp.Common.Definitions.ISnmpMessage)

   Performs a bulk walk operation.

   .. code-block:: csharp

      public static int BulkWalk(VersionCode version, IPEndPoint endpoint, OctetString community, OctetString contextName, ObjectIdentifier table, IList<Variable> list, int timeout, int maxRepetitions, WalkMode mode, IPrivacyProvider? privacy, ISnmpMessage? report)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type endpoint: ``IPEndPoint``
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type contextName: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type table: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type list: ``IList<Variable>``
   :type timeout: ``Int32``
   :type maxRepetitions: ``Int32``
   :type mode: :dn:enum:`~Lextm.SharpSnmpLib.Messaging.WalkMode`
   :type privacy: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`
   :type report: :dn:iface:`~DotNetSnmp.Common.Definitions.ISnmpMessage`

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L758>`__

BulkWalkAsync(VersionCode, IPEndPoint, OctetString, OctetString, ObjectIdentifier, IList<Variable>, Int32, WalkMode, IPrivacyProvider, ISnmpMessage, CancellationToken)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.BulkWalkAsync(DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},System.Int32,Lextm.SharpSnmpLib.Messaging.WalkMode,DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider,DotNetSnmp.Common.Definitions.ISnmpMessage,System.Threading.CancellationToken)

   Performs an asynchronous bulk walk operation.

   .. code-block:: csharp

      public static Task<int> BulkWalkAsync(VersionCode version, IPEndPoint endpoint, OctetString community, OctetString contextName, ObjectIdentifier table, IList<Variable> list, int maxRepetitions, WalkMode mode, IPrivacyProvider privacy, ISnmpMessage report, CancellationToken cancellationToken)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type endpoint: ``IPEndPoint``
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type contextName: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type table: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type list: ``IList<Variable>``
   :type maxRepetitions: ``Int32``
   :type mode: :dn:enum:`~Lextm.SharpSnmpLib.Messaging.WalkMode`
   :type privacy: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`
   :type report: :dn:iface:`~DotNetSnmp.Common.Definitions.ISnmpMessage`
   :type cancellationToken: ``CancellationToken``

   :rtype: ``Task<Int32>``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L667>`__

BulkWalkAsync(VersionCode, IPEndPoint, OctetString, OctetString, ObjectIdentifier, IList<Variable>, Int32, WalkMode, IPrivacyProvider, ISnmpMessage)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.BulkWalkAsync(DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},System.Int32,Lextm.SharpSnmpLib.Messaging.WalkMode,DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider,DotNetSnmp.Common.Definitions.ISnmpMessage)

   Performs an asynchronous bulk walk operation.

   .. code-block:: csharp

      public static Task<int> BulkWalkAsync(VersionCode version, IPEndPoint endpoint, OctetString community, OctetString contextName, ObjectIdentifier table, IList<Variable> list, int maxRepetitions, WalkMode mode, IPrivacyProvider privacy, ISnmpMessage report)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type endpoint: ``IPEndPoint``
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type contextName: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type table: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type list: ``IList<Variable>``
   :type maxRepetitions: ``Int32``
   :type mode: :dn:enum:`~Lextm.SharpSnmpLib.Messaging.WalkMode`
   :type privacy: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`
   :type report: :dn:iface:`~DotNetSnmp.Common.Definitions.ISnmpMessage`

   :rtype: ``Task<Int32>``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L649>`__

BulkWalkAsync(VersionCode, IPEndPoint, OctetString, OctetString, ObjectIdentifier, IList<Variable>, Int32, WalkMode, ISnmpTransport)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.BulkWalkAsync(DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},System.Int32,Lextm.SharpSnmpLib.Messaging.WalkMode,DotNetSnmp.Transport.ISnmpTransport)

   Performs an asynchronous bulk walk operation using the specified transport.

   .. code-block:: csharp

      public static Task<int> BulkWalkAsync(VersionCode version, IPEndPoint endpoint, OctetString community, OctetString contextName, ObjectIdentifier table, IList<Variable> list, int maxRepetitions, WalkMode mode, ISnmpTransport transport)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type endpoint: ``IPEndPoint``
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type contextName: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type table: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type list: ``IList<Variable>``
   :type maxRepetitions: ``Int32``
   :type mode: :dn:enum:`~Lextm.SharpSnmpLib.Messaging.WalkMode`
   :type transport: :dn:iface:`~DotNetSnmp.Transport.ISnmpTransport`

   :rtype: ``Task<Int32>``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L547>`__

BulkWalkAsync(VersionCode, IPEndPoint, OctetString, OctetString, ObjectIdentifier, IList<Variable>, Int32, WalkMode)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.BulkWalkAsync(DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},System.Int32,Lextm.SharpSnmpLib.Messaging.WalkMode)

   Performs an asynchronous bulk walk operation.

   .. code-block:: csharp

      public static Task<int> BulkWalkAsync(VersionCode version, IPEndPoint endpoint, OctetString community, OctetString contextName, ObjectIdentifier table, IList<Variable> list, int maxRepetitions, WalkMode mode)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type endpoint: ``IPEndPoint``
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type contextName: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type table: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type list: ``IList<Variable>``
   :type maxRepetitions: ``Int32``
   :type mode: :dn:enum:`~Lextm.SharpSnmpLib.Messaging.WalkMode`

   :rtype: ``Task<Int32>``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L538>`__

BulkWalkV3Async(IPEndPoint, String, IPrivacyProvider, ObjectIdentifier, IList<Variable>, Int32, WalkMode, String, ISnmpTransport)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.BulkWalkV3Async(System.Net.IPEndPoint,System.String,DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},System.Int32,Lextm.SharpSnmpLib.Messaging.WalkMode,System.String,DotNetSnmp.Transport.ISnmpTransport)

   Walks a subtree with GetBulk requests over SNMPv3 and appends results using the specified transport.

   .. code-block:: csharp

      public static Task<int> BulkWalkV3Async(IPEndPoint endpoint, string username, IPrivacyProvider privacyProvider, ObjectIdentifier table, IList<Variable> list, int maxRepetitions, WalkMode mode, string contextName, ISnmpTransport transport)

   :type endpoint: ``IPEndPoint``
   :type username: ``String``
   :type privacyProvider: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`
   :type table: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type list: ``IList<Variable>``
   :type maxRepetitions: ``Int32``
   :type mode: :dn:enum:`~Lextm.SharpSnmpLib.Messaging.WalkMode`
   :type contextName: ``String``
   :type transport: :dn:iface:`~DotNetSnmp.Transport.ISnmpTransport`

   :rtype: ``Task<Int32>``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L1358>`__

BulkWalkV3Async(IPEndPoint, String, IPrivacyProvider, ObjectIdentifier, IList<Variable>, Int32, WalkMode, String)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.BulkWalkV3Async(System.Net.IPEndPoint,System.String,DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},System.Int32,Lextm.SharpSnmpLib.Messaging.WalkMode,System.String)

   Walks a subtree with GetBulk requests over SNMPv3 and appends results to list.

   .. code-block:: csharp

      public static Task<int> BulkWalkV3Async(IPEndPoint endpoint, string username, IPrivacyProvider privacyProvider, ObjectIdentifier table, IList<Variable> list, int maxRepetitions, WalkMode mode, string contextName = "")

   :type endpoint: ``IPEndPoint``
   :type username: ``String``
   :type privacyProvider: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`
   :type table: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type list: ``IList<Variable>``
   :type maxRepetitions: ``Int32``
   :type mode: :dn:enum:`~Lextm.SharpSnmpLib.Messaging.WalkMode`
   :type contextName: ``String``

   :rtype: ``Task<Int32>``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L1341>`__

Get(VersionCode, IPEndPoint, OctetString, IList<Variable>, Int32, ISnmpTransport)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.Get(DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,DotNetSnmp.Asn1.SyntaxObjects.OctetString,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},System.Int32,DotNetSnmp.Transport.ISnmpTransport)

   Retrieves data using the specified transport.

   .. code-block:: csharp

      public static IList<Variable> Get(VersionCode version, IPEndPoint endpoint, OctetString community, IList<Variable> variables, int timeout, ISnmpTransport transport)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type endpoint: ``IPEndPoint``
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type variables: ``IList<Variable>``
   :type timeout: ``Int32``
   :type transport: :dn:iface:`~DotNetSnmp.Transport.ISnmpTransport`

   :rtype: ``IList<Variable>``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L698>`__

Get(VersionCode, IPEndPoint, OctetString, IList<Variable>, Int32)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.Get(DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,DotNetSnmp.Asn1.SyntaxObjects.OctetString,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},System.Int32)

   Retrieves data.

   .. code-block:: csharp

      public static IList<Variable> Get(VersionCode version, IPEndPoint endpoint, OctetString community, IList<Variable> variables, int timeout)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type endpoint: ``IPEndPoint``
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type variables: ``IList<Variable>``
   :type timeout: ``Int32``

   :rtype: ``IList<Variable>``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L690>`__

GetAsync(VersionCode, IPEndPoint, OctetString, IList<Variable>, ISnmpTransport)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.GetAsync(DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,DotNetSnmp.Asn1.SyntaxObjects.OctetString,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},DotNetSnmp.Transport.ISnmpTransport)

   Performs asynchronous retrieval using the specified transport.

   .. code-block:: csharp

      public static Task<IList<Variable>> GetAsync(VersionCode version, IPEndPoint endpoint, OctetString community, IList<Variable> variables, ISnmpTransport transport)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type endpoint: ``IPEndPoint``
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type variables: ``IList<Variable>``
   :type transport: :dn:iface:`~DotNetSnmp.Transport.ISnmpTransport`

   :rtype: ``Task<IList<Variable>>``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L193>`__

GetAsync(VersionCode, IPEndPoint, OctetString, IList<Variable>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.GetAsync(DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,DotNetSnmp.Asn1.SyntaxObjects.OctetString,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable})

   Performs asynchronous retrieval.

   .. code-block:: csharp

      public static Task<IList<Variable>> GetAsync(VersionCode version, IPEndPoint endpoint, OctetString community, IList<Variable> variables)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type endpoint: ``IPEndPoint``
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type variables: ``IList<Variable>``

   :rtype: ``Task<IList<Variable>>``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L184>`__

GetErrorMessage(ObjectIdentifier)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.GetErrorMessage(DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier)

   Returns error message for the specific :dn:struct:``~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier``.

   .. code-block:: csharp

      public static string GetErrorMessage(this ObjectIdentifier id)

   :rtype: ``String``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L146>`__

GetNextDiscovery(SnmpType, OctetString)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.GetNextDiscovery(Lextm.SharpSnmpLib.SnmpType,DotNetSnmp.Asn1.SyntaxObjects.OctetString)

   Returns a new discovery request with scoped context name.

   .. code-block:: csharp

      public static Discovery GetNextDiscovery(SnmpType type, OctetString contextName)

   :type type: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`
   :type contextName: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`

   :rtype: :dn:cls:`~Lextm.SharpSnmpLib.Messaging.Discovery`

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L138>`__

GetNextDiscovery(SnmpType)
~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.GetNextDiscovery(Lextm.SharpSnmpLib.SnmpType)

   Returns a new discovery request.

   .. code-block:: csharp

      public static Discovery GetNextDiscovery(SnmpType type)

   :type type: :dn:enum:`~Lextm.SharpSnmpLib.SnmpType`

   :rtype: :dn:cls:`~Lextm.SharpSnmpLib.Messaging.Discovery`

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L130>`__

GetTable(VersionCode, IPEndPoint, OctetString, ObjectIdentifier, Int32, Int32)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.GetTable(DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,System.Int32,System.Int32)

   Gets table.

   .. code-block:: csharp

      [Obsolete("This method only works for a few scenarios. Might be replaced by new methods in the future. If it does not work for you, parse WALK result on your own.")]
      public static Variable[, ] GetTable(VersionCode version, IPEndPoint endpoint, OctetString community, ObjectIdentifier table, int timeout, int maxRepetitions)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type endpoint: ``IPEndPoint``
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type table: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type timeout: ``Int32``
   :type maxRepetitions: ``Int32``

   :rtype: ``Variable[,]``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L801>`__

GetV3Async(IPEndPoint, String, IList<Variable>, ISnmpTransport)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.GetV3Async(System.Net.IPEndPoint,System.String,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},DotNetSnmp.Transport.ISnmpTransport)

   Gets v3 Async using the specified transport.

   .. code-block:: csharp

      public static Task<IList<Variable>> GetV3Async(IPEndPoint endpoint, string username, IList<Variable> variables, ISnmpTransport transport)

   :type endpoint: ``IPEndPoint``
   :type username: ``String``
   :type variables: ``IList<Variable>``
   :type transport: :dn:iface:`~DotNetSnmp.Transport.ISnmpTransport`

   :rtype: ``Task<IList<Variable>>``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L241>`__

GetV3Async(IPEndPoint, String, IList<Variable>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.GetV3Async(System.Net.IPEndPoint,System.String,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable})

   Gets v3 Async.

   .. code-block:: csharp

      public static Task<IList<Variable>> GetV3Async(IPEndPoint endpoint, string username, IList<Variable> variables)

   :type endpoint: ``IPEndPoint``
   :type username: ``String``
   :type variables: ``IList<Variable>``

   :rtype: ``Task<IList<Variable>>``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L233>`__

GetV3Async(IPEndPoint, String, IPrivacyProvider, IList<Variable>, String, ISnmpTransport)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.GetV3Async(System.Net.IPEndPoint,System.String,DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},System.String,DotNetSnmp.Transport.ISnmpTransport)

   Gets v3 Async using the specified transport.

   .. code-block:: csharp

      public static Task<IList<Variable>> GetV3Async(IPEndPoint endpoint, string username, IPrivacyProvider privacyProvider, IList<Variable> variables, string contextName, ISnmpTransport transport)

   :type endpoint: ``IPEndPoint``
   :type username: ``String``
   :type privacyProvider: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`
   :type variables: ``IList<Variable>``
   :type contextName: ``String``
   :type transport: :dn:iface:`~DotNetSnmp.Transport.ISnmpTransport`

   :rtype: ``Task<IList<Variable>>``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L259>`__

GetV3Async(IPEndPoint, String, IPrivacyProvider, IList<Variable>, String)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.GetV3Async(System.Net.IPEndPoint,System.String,DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},System.String)

   Gets v3 Async.

   .. code-block:: csharp

      public static Task<IList<Variable>> GetV3Async(IPEndPoint endpoint, string username, IPrivacyProvider privacyProvider, IList<Variable> variables, string contextName = "")

   :type endpoint: ``IPEndPoint``
   :type username: ``String``
   :type privacyProvider: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`
   :type variables: ``IList<Variable>``
   :type contextName: ``String``

   :rtype: ``Task<IList<Variable>>``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L250>`__

SendInform(Int32, VersionCode, IPEndPoint, OctetString, OctetString, ObjectIdentifier, UInt32, IList<Variable>, Int32, IPrivacyProvider, ISnmpMessage)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.SendInform(System.Int32,DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,System.UInt32,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},System.Int32,DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider,DotNetSnmp.Common.Definitions.ISnmpMessage)

   Sends inform.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public static void SendInform(int requestId, VersionCode version, IPEndPoint receiver, OctetString community, OctetString contextName, ObjectIdentifier enterprise, uint timestamp, IList<Variable> variables, int timeout, IPrivacyProvider privacy, ISnmpMessage report)

   :type requestId: ``Int32``
   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type receiver: ``IPEndPoint``
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type contextName: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type enterprise: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type timestamp: ``UInt32``
   :type variables: ``IList<Variable>``
   :type timeout: ``Int32``
   :type privacy: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`
   :type report: :dn:iface:`~DotNetSnmp.Common.Definitions.ISnmpMessage`

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L1296>`__

SendInformAsync(Int32, VersionCode, IPEndPoint, OctetString, OctetString, ObjectIdentifier, UInt32, IList<Variable>, IPrivacyProvider, ISnmpMessage, CancellationToken)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.SendInformAsync(System.Int32,DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,System.UInt32,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider,DotNetSnmp.Common.Definitions.ISnmpMessage,System.Threading.CancellationToken)

   Sends inform Async.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public static Task SendInformAsync(int requestId, VersionCode version, IPEndPoint endpoint, OctetString community, OctetString contextName, ObjectIdentifier enterprise, uint timestamp, IList<Variable> variables, IPrivacyProvider privacy, ISnmpMessage report, CancellationToken cancellationToken)

   :type requestId: ``Int32``
   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type endpoint: ``IPEndPoint``
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type contextName: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type enterprise: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type timestamp: ``UInt32``
   :type variables: ``IList<Variable>``
   :type privacy: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`
   :type report: :dn:iface:`~DotNetSnmp.Common.Definitions.ISnmpMessage`
   :type cancellationToken: ``CancellationToken``

   :rtype: ``Task``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L969>`__

SendInformAsync(Int32, VersionCode, IPEndPoint, OctetString, OctetString, ObjectIdentifier, UInt32, IList<Variable>, IPrivacyProvider, ISnmpMessage, ISnmpTransport, CancellationToken)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.SendInformAsync(System.Int32,DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,System.UInt32,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider,DotNetSnmp.Common.Definitions.ISnmpMessage,DotNetSnmp.Transport.ISnmpTransport,System.Threading.CancellationToken)

   Sends inform Async using the specified transport.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public static Task SendInformAsync(int requestId, VersionCode version, IPEndPoint endpoint, OctetString community, OctetString contextName, ObjectIdentifier enterprise, uint timestamp, IList<Variable> variables, IPrivacyProvider privacy, ISnmpMessage report, ISnmpTransport transport, CancellationToken cancellationToken)

   :type requestId: ``Int32``
   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type endpoint: ``IPEndPoint``
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type contextName: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type enterprise: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type timestamp: ``UInt32``
   :type variables: ``IList<Variable>``
   :type privacy: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`
   :type report: :dn:iface:`~DotNetSnmp.Common.Definitions.ISnmpMessage`
   :type transport: :dn:iface:`~DotNetSnmp.Transport.ISnmpTransport`
   :type cancellationToken: ``CancellationToken``

   :rtype: ``Task``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L1003>`__

SendInformAsync(Int32, VersionCode, IPEndPoint, OctetString, OctetString, ObjectIdentifier, UInt32, IList<Variable>, IPrivacyProvider, ISnmpMessage, ISnmpTransport)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.SendInformAsync(System.Int32,DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,System.UInt32,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider,DotNetSnmp.Common.Definitions.ISnmpMessage,DotNetSnmp.Transport.ISnmpTransport)

   Sends inform Async using the specified transport.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public static Task SendInformAsync(int requestId, VersionCode version, IPEndPoint endpoint, OctetString community, OctetString contextName, ObjectIdentifier enterprise, uint timestamp, IList<Variable> variables, IPrivacyProvider privacy, ISnmpMessage report, ISnmpTransport transport)

   :type requestId: ``Int32``
   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type endpoint: ``IPEndPoint``
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type contextName: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type enterprise: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type timestamp: ``UInt32``
   :type variables: ``IList<Variable>``
   :type privacy: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`
   :type report: :dn:iface:`~DotNetSnmp.Common.Definitions.ISnmpMessage`
   :type transport: :dn:iface:`~DotNetSnmp.Transport.ISnmpTransport`

   :rtype: ``Task``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L937>`__

SendInformAsync(Int32, VersionCode, IPEndPoint, OctetString, OctetString, ObjectIdentifier, UInt32, IList<Variable>, IPrivacyProvider, ISnmpMessage)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.SendInformAsync(System.Int32,DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,System.UInt32,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider,DotNetSnmp.Common.Definitions.ISnmpMessage)

   Sends inform Async.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public static Task SendInformAsync(int requestId, VersionCode version, IPEndPoint endpoint, OctetString community, OctetString contextName, ObjectIdentifier enterprise, uint timestamp, IList<Variable> variables, IPrivacyProvider privacy, ISnmpMessage report)

   :type requestId: ``Int32``
   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type endpoint: ``IPEndPoint``
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type contextName: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type enterprise: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type timestamp: ``UInt32``
   :type variables: ``IList<Variable>``
   :type privacy: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`
   :type report: :dn:iface:`~DotNetSnmp.Common.Definitions.ISnmpMessage`

   :rtype: ``Task``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L905>`__

SendInformAsync(Int32, VersionCode, IPEndPoint, OctetString, OctetString, ObjectIdentifier, UInt32, IList<Variable>, ISnmpTransport)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.SendInformAsync(System.Int32,DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,System.UInt32,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},DotNetSnmp.Transport.ISnmpTransport)

   Sends inform Async using the specified transport.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public static Task SendInformAsync(int requestId, VersionCode version, IPEndPoint endpoint, OctetString community, OctetString contextName, ObjectIdentifier enterprise, uint timestamp, IList<Variable> variables, ISnmpTransport transport)

   :type requestId: ``Int32``
   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type endpoint: ``IPEndPoint``
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type contextName: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type enterprise: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type timestamp: ``UInt32``
   :type variables: ``IList<Variable>``
   :type transport: :dn:iface:`~DotNetSnmp.Transport.ISnmpTransport`

   :rtype: ``Task``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L853>`__

SendInformAsync(Int32, VersionCode, IPEndPoint, OctetString, OctetString, ObjectIdentifier, UInt32, IList<Variable>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.SendInformAsync(System.Int32,DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,System.UInt32,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable})

   Sends inform Async.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public static Task SendInformAsync(int requestId, VersionCode version, IPEndPoint endpoint, OctetString community, OctetString contextName, ObjectIdentifier enterprise, uint timestamp, IList<Variable> variables)

   :type requestId: ``Int32``
   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type endpoint: ``IPEndPoint``
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type contextName: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type enterprise: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type timestamp: ``UInt32``
   :type variables: ``IList<Variable>``

   :rtype: ``Task``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L843>`__

SendInformV3Async(IPEndPoint, String, IPrivacyProvider, ObjectIdentifier, UInt32, IList<Variable>, String, ISnmpTransport)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.SendInformV3Async(System.Net.IPEndPoint,System.String,DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,System.UInt32,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},System.String,DotNetSnmp.Transport.ISnmpTransport)

   Sends inform V3 Async using the specified transport.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public static Task SendInformV3Async(IPEndPoint endpoint, string username, IPrivacyProvider privacyProvider, ObjectIdentifier enterprise, uint timestamp, IList<Variable> variables, string contextName, ISnmpTransport transport)

   :type endpoint: ``IPEndPoint``
   :type username: ``String``
   :type privacyProvider: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`
   :type enterprise: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type timestamp: ``UInt32``
   :type variables: ``IList<Variable>``
   :type contextName: ``String``
   :type transport: :dn:iface:`~DotNetSnmp.Transport.ISnmpTransport`

   :rtype: ``Task``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L1495>`__

SendInformV3Async(IPEndPoint, String, IPrivacyProvider, ObjectIdentifier, UInt32, IList<Variable>, String)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.SendInformV3Async(System.Net.IPEndPoint,System.String,DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,System.UInt32,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},System.String)

   Sends inform V3 Async.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public static Task SendInformV3Async(IPEndPoint endpoint, string username, IPrivacyProvider privacyProvider, ObjectIdentifier enterprise, uint timestamp, IList<Variable> variables, string contextName = "")

   :type endpoint: ``IPEndPoint``
   :type username: ``String``
   :type privacyProvider: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`
   :type enterprise: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type timestamp: ``UInt32``
   :type variables: ``IList<Variable>``
   :type contextName: ``String``

   :rtype: ``Task``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L1478>`__

SendTrapV1(EndPoint, IPAddress, OctetString, ObjectIdentifier, GenericCode, Int32, UInt32, IList<Variable>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.SendTrapV1(System.Net.EndPoint,System.Net.IPAddress,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,Lextm.SharpSnmpLib.GenericCode,System.Int32,System.UInt32,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable})

   Sends trap V1.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public static void SendTrapV1(EndPoint receiver, IPAddress agent, OctetString community, ObjectIdentifier enterprise, GenericCode generic, int specific, uint timestamp, IList<Variable> variables)

   :type receiver: ``EndPoint``
   :type agent: ``IPAddress``
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type enterprise: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type generic: :dn:enum:`~Lextm.SharpSnmpLib.GenericCode`
   :type specific: ``Int32``
   :type timestamp: ``UInt32``
   :type variables: ``IList<Variable>``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L1205>`__

SendTrapV1Async(EndPoint, IPAddress, OctetString, ObjectIdentifier, GenericCode, Int32, UInt32, IList<Variable>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.SendTrapV1Async(System.Net.EndPoint,System.Net.IPAddress,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,Lextm.SharpSnmpLib.GenericCode,System.Int32,System.UInt32,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable})

   Sends trap V1 Async.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public static Task SendTrapV1Async(EndPoint receiver, IPAddress agent, OctetString community, ObjectIdentifier enterprise, GenericCode generic, int specific, uint timestamp, IList<Variable> variables)

   :type receiver: ``EndPoint``
   :type agent: ``IPAddress``
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type enterprise: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type generic: :dn:enum:`~Lextm.SharpSnmpLib.GenericCode`
   :type specific: ``Int32``
   :type timestamp: ``UInt32``
   :type variables: ``IList<Variable>``

   :rtype: ``Task``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L1123>`__

SendTrapV1Async(IPEndPoint, IPAddress, OctetString, ObjectIdentifier, GenericCode, Int32, UInt32, IList<Variable>, ISnmpTransport)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.SendTrapV1Async(System.Net.IPEndPoint,System.Net.IPAddress,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,Lextm.SharpSnmpLib.GenericCode,System.Int32,System.UInt32,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},DotNetSnmp.Transport.ISnmpTransport)

   Sends trap V1 Async using the specified transport.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public static Task SendTrapV1Async(IPEndPoint endpoint, IPAddress agent, OctetString community, ObjectIdentifier enterprise, GenericCode generic, int specific, uint timestamp, IList<Variable> variables, ISnmpTransport transport)

   :type endpoint: ``IPEndPoint``
   :type agent: ``IPAddress``
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type enterprise: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type generic: :dn:enum:`~Lextm.SharpSnmpLib.GenericCode`
   :type specific: ``Int32``
   :type timestamp: ``UInt32``
   :type variables: ``IList<Variable>``
   :type transport: :dn:iface:`~DotNetSnmp.Transport.ISnmpTransport`

   :rtype: ``Task``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L1156>`__

SendTrapV2(Int32, VersionCode, EndPoint, OctetString, ObjectIdentifier, UInt32, IList<Variable>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.SendTrapV2(System.Int32,DotNetSnmp.Common.Definitions.VersionCode,System.Net.EndPoint,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,System.UInt32,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable})

   Sends trap V2.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public static void SendTrapV2(int requestId, VersionCode version, EndPoint receiver, OctetString community, ObjectIdentifier enterprise, uint timestamp, IList<Variable> variables)

   :type requestId: ``Int32``
   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type receiver: ``EndPoint``
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type enterprise: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type timestamp: ``UInt32``
   :type variables: ``IList<Variable>``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L1318>`__

SendTrapV2Async(Int32, VersionCode, EndPoint, OctetString, ObjectIdentifier, UInt32, IList<Variable>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.SendTrapV2Async(System.Int32,DotNetSnmp.Common.Definitions.VersionCode,System.Net.EndPoint,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,System.UInt32,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable})

   Sends trap V2 Async.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public static Task SendTrapV2Async(int requestId, VersionCode version, EndPoint receiver, OctetString community, ObjectIdentifier enterprise, uint timestamp, IList<Variable> variables)

   :type requestId: ``Int32``
   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type receiver: ``EndPoint``
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type enterprise: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type timestamp: ``UInt32``
   :type variables: ``IList<Variable>``

   :rtype: ``Task``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L1282>`__

SendTrapV2Async(Int32, VersionCode, IPEndPoint, OctetString, OctetString, ObjectIdentifier, UInt32, IList<Variable>, ISnmpTransport)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.SendTrapV2Async(System.Int32,DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,System.UInt32,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},DotNetSnmp.Transport.ISnmpTransport)

   Sends trap V2 Async using the specified transport.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public static Task SendTrapV2Async(int requestId, VersionCode version, IPEndPoint endpoint, OctetString community, OctetString contextName, ObjectIdentifier enterprise, uint timestamp, IList<Variable> variables, ISnmpTransport transport)

   :type requestId: ``Int32``
   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type endpoint: ``IPEndPoint``
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type contextName: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type enterprise: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type timestamp: ``UInt32``
   :type variables: ``IList<Variable>``
   :type transport: :dn:iface:`~DotNetSnmp.Transport.ISnmpTransport`

   :rtype: ``Task``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L1234>`__

SendTrapV2Async(Int32, VersionCode, IPEndPoint, OctetString, OctetString, ObjectIdentifier, UInt32, IList<Variable>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.SendTrapV2Async(System.Int32,DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,System.UInt32,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable})

   Sends trap V2 Async.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public static Task SendTrapV2Async(int requestId, VersionCode version, IPEndPoint endpoint, OctetString community, OctetString contextName, ObjectIdentifier enterprise, uint timestamp, IList<Variable> variables)

   :type requestId: ``Int32``
   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type endpoint: ``IPEndPoint``
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type contextName: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type enterprise: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type timestamp: ``UInt32``
   :type variables: ``IList<Variable>``

   :rtype: ``Task``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L1224>`__

SendTrapV2V3Async(IPEndPoint, String, IPrivacyProvider, ObjectIdentifier, UInt32, IList<Variable>, String, ISnmpTransport)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.SendTrapV2V3Async(System.Net.IPEndPoint,System.String,DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,System.UInt32,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},System.String,DotNetSnmp.Transport.ISnmpTransport)

   Sends trap V2 V3 Async using the specified transport.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public static Task SendTrapV2V3Async(IPEndPoint endpoint, string username, IPrivacyProvider privacyProvider, ObjectIdentifier enterprise, uint timestamp, IList<Variable> variables, string contextName, ISnmpTransport transport)

   :type endpoint: ``IPEndPoint``
   :type username: ``String``
   :type privacyProvider: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`
   :type enterprise: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type timestamp: ``UInt32``
   :type variables: ``IList<Variable>``
   :type contextName: ``String``
   :type transport: :dn:iface:`~DotNetSnmp.Transport.ISnmpTransport`

   :rtype: ``Task``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L1572>`__

SendTrapV2V3Async(IPEndPoint, String, IPrivacyProvider, ObjectIdentifier, UInt32, IList<Variable>, String)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.SendTrapV2V3Async(System.Net.IPEndPoint,System.String,DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,System.UInt32,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},System.String)

   Sends trap V2 V3 Async.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public static Task SendTrapV2V3Async(IPEndPoint endpoint, string username, IPrivacyProvider privacyProvider, ObjectIdentifier enterprise, uint timestamp, IList<Variable> variables, string contextName = "")

   :type endpoint: ``IPEndPoint``
   :type username: ``String``
   :type privacyProvider: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`
   :type enterprise: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type timestamp: ``UInt32``
   :type variables: ``IList<Variable>``
   :type contextName: ``String``

   :rtype: ``Task``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L1555>`__

Set(VersionCode, IPEndPoint, OctetString, IList<Variable>, Int32, ISnmpTransport)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.Set(DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,DotNetSnmp.Asn1.SyntaxObjects.OctetString,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},System.Int32,DotNetSnmp.Transport.ISnmpTransport)

   Sends updated data using the specified transport.

   .. code-block:: csharp

      public static IList<Variable> Set(VersionCode version, IPEndPoint endpoint, OctetString community, IList<Variable> variables, int timeout, ISnmpTransport transport)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type endpoint: ``IPEndPoint``
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type variables: ``IList<Variable>``
   :type timeout: ``Int32``
   :type transport: :dn:iface:`~DotNetSnmp.Transport.ISnmpTransport`

   :rtype: ``IList<Variable>``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L720>`__

Set(VersionCode, IPEndPoint, OctetString, IList<Variable>, Int32)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.Set(DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,DotNetSnmp.Asn1.SyntaxObjects.OctetString,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},System.Int32)

   Sends updated data.

   .. code-block:: csharp

      public static IList<Variable> Set(VersionCode version, IPEndPoint endpoint, OctetString community, IList<Variable> variables, int timeout)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type endpoint: ``IPEndPoint``
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type variables: ``IList<Variable>``
   :type timeout: ``Int32``

   :rtype: ``IList<Variable>``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L712>`__

SetAsync(VersionCode, IPEndPoint, OctetString, IList<Variable>, ISnmpTransport)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.SetAsync(DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,DotNetSnmp.Asn1.SyntaxObjects.OctetString,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},DotNetSnmp.Transport.ISnmpTransport)

   Performs asynchronous update using the specified transport.

   .. code-block:: csharp

      public static Task<IList<Variable>> SetAsync(VersionCode version, IPEndPoint endpoint, OctetString community, IList<Variable> variables, ISnmpTransport transport)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type endpoint: ``IPEndPoint``
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type variables: ``IList<Variable>``
   :type transport: :dn:iface:`~DotNetSnmp.Transport.ISnmpTransport`

   :rtype: ``Task<IList<Variable>>``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L307>`__

SetAsync(VersionCode, IPEndPoint, OctetString, IList<Variable>)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.SetAsync(DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,DotNetSnmp.Asn1.SyntaxObjects.OctetString,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable})

   Performs asynchronous update.

   .. code-block:: csharp

      public static Task<IList<Variable>> SetAsync(VersionCode version, IPEndPoint endpoint, OctetString community, IList<Variable> variables)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type endpoint: ``IPEndPoint``
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type variables: ``IList<Variable>``

   :rtype: ``Task<IList<Variable>>``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L298>`__

SetV3Async(IPEndPoint, String, IPrivacyProvider, IList<Variable>, String, ISnmpTransport)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.SetV3Async(System.Net.IPEndPoint,System.String,DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},System.String,DotNetSnmp.Transport.ISnmpTransport)

   Sets v3 Async using the specified transport.

   .. code-block:: csharp

      public static Task<IList<Variable>> SetV3Async(IPEndPoint endpoint, string username, IPrivacyProvider privacyProvider, IList<Variable> variables, string contextName, ISnmpTransport transport)

   :type endpoint: ``IPEndPoint``
   :type username: ``String``
   :type privacyProvider: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`
   :type variables: ``IList<Variable>``
   :type contextName: ``String``
   :type transport: :dn:iface:`~DotNetSnmp.Transport.ISnmpTransport`

   :rtype: ``Task<IList<Variable>>``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L352>`__

SetV3Async(IPEndPoint, String, IPrivacyProvider, IList<Variable>, String)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.SetV3Async(System.Net.IPEndPoint,System.String,DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},System.String)

   Sets v3 Async.

   .. code-block:: csharp

      public static Task<IList<Variable>> SetV3Async(IPEndPoint endpoint, string username, IPrivacyProvider privacyProvider, IList<Variable> variables, string contextName = "")

   :type endpoint: ``IPEndPoint``
   :type username: ``String``
   :type privacyProvider: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`
   :type variables: ``IList<Variable>``
   :type contextName: ``String``

   :rtype: ``Task<IList<Variable>>``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L342>`__

Walk(VersionCode, IPEndPoint, OctetString, ObjectIdentifier, IList<Variable>, Int32, WalkMode, ISnmpTransport)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.Walk(DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},System.Int32,Lextm.SharpSnmpLib.Messaging.WalkMode,DotNetSnmp.Transport.ISnmpTransport)

   Performs a walk operation using the specified transport.

   .. code-block:: csharp

      public static int Walk(VersionCode version, IPEndPoint endpoint, OctetString community, ObjectIdentifier table, IList<Variable> list, int timeout, WalkMode mode, ISnmpTransport transport)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type endpoint: ``IPEndPoint``
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type table: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type list: ``IList<Variable>``
   :type timeout: ``Int32``
   :type mode: :dn:enum:`~Lextm.SharpSnmpLib.Messaging.WalkMode`
   :type transport: :dn:iface:`~DotNetSnmp.Transport.ISnmpTransport`

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L742>`__

Walk(VersionCode, IPEndPoint, OctetString, ObjectIdentifier, IList<Variable>, Int32, WalkMode)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.Walk(DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},System.Int32,Lextm.SharpSnmpLib.Messaging.WalkMode)

   Performs a walk operation.

   .. code-block:: csharp

      public static int Walk(VersionCode version, IPEndPoint endpoint, OctetString community, ObjectIdentifier table, IList<Variable> list, int timeout, WalkMode mode)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type endpoint: ``IPEndPoint``
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type table: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type list: ``IList<Variable>``
   :type timeout: ``Int32``
   :type mode: :dn:enum:`~Lextm.SharpSnmpLib.Messaging.WalkMode`

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L734>`__

WalkAsync(VersionCode, IPEndPoint, OctetString, ObjectIdentifier, IList<Variable>, WalkMode, CancellationToken)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.WalkAsync(DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},Lextm.SharpSnmpLib.Messaging.WalkMode,System.Threading.CancellationToken)

   Performs an asynchronous walk operation.

   .. code-block:: csharp

      public static Task<int> WalkAsync(VersionCode version, IPEndPoint endpoint, OctetString community, ObjectIdentifier table, IList<Variable> list, WalkMode mode, CancellationToken cancellationToken)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type endpoint: ``IPEndPoint``
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type table: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type list: ``IList<Variable>``
   :type mode: :dn:enum:`~Lextm.SharpSnmpLib.Messaging.WalkMode`
   :type cancellationToken: ``CancellationToken``

   :rtype: ``Task<Int32>``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L470>`__

WalkAsync(VersionCode, IPEndPoint, OctetString, ObjectIdentifier, IList<Variable>, WalkMode, ISnmpTransport, CancellationToken)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.WalkAsync(DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},Lextm.SharpSnmpLib.Messaging.WalkMode,DotNetSnmp.Transport.ISnmpTransport,System.Threading.CancellationToken)

   Performs an asynchronous walk operation using the specified transport.

   .. code-block:: csharp

      public static Task<int> WalkAsync(VersionCode version, IPEndPoint endpoint, OctetString community, ObjectIdentifier table, IList<Variable> list, WalkMode mode, ISnmpTransport transport, CancellationToken cancellationToken)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type endpoint: ``IPEndPoint``
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type table: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type list: ``IList<Variable>``
   :type mode: :dn:enum:`~Lextm.SharpSnmpLib.Messaging.WalkMode`
   :type transport: :dn:iface:`~DotNetSnmp.Transport.ISnmpTransport`
   :type cancellationToken: ``CancellationToken``

   :rtype: ``Task<Int32>``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L480>`__

WalkAsync(VersionCode, IPEndPoint, OctetString, ObjectIdentifier, IList<Variable>, WalkMode, ISnmpTransport)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.WalkAsync(DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},Lextm.SharpSnmpLib.Messaging.WalkMode,DotNetSnmp.Transport.ISnmpTransport)

   Performs an asynchronous walk operation using the specified transport.

   .. code-block:: csharp

      public static Task<int> WalkAsync(VersionCode version, IPEndPoint endpoint, OctetString community, ObjectIdentifier table, IList<Variable> list, WalkMode mode, ISnmpTransport transport)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type endpoint: ``IPEndPoint``
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type table: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type list: ``IList<Variable>``
   :type mode: :dn:enum:`~Lextm.SharpSnmpLib.Messaging.WalkMode`
   :type transport: :dn:iface:`~DotNetSnmp.Transport.ISnmpTransport`

   :rtype: ``Task<Int32>``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L400>`__

WalkAsync(VersionCode, IPEndPoint, OctetString, ObjectIdentifier, IList<Variable>, WalkMode)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Messenger.WalkAsync(DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,System.Collections.Generic.IList{DotNetSnmp.Asn1.SyntaxObjects.Variable},Lextm.SharpSnmpLib.Messaging.WalkMode)

   Performs an asynchronous walk operation.

   .. code-block:: csharp

      public static Task<int> WalkAsync(VersionCode version, IPEndPoint endpoint, OctetString community, ObjectIdentifier table, IList<Variable> list, WalkMode mode)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type endpoint: ``IPEndPoint``
   :type community: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type table: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type list: ``IList<Variable>``
   :type mode: :dn:enum:`~Lextm.SharpSnmpLib.Messaging.WalkMode`

   :rtype: ``Task<Int32>``

**Source:** `SharpSnmpLib/Messaging/Messenger.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Messenger.cs#L391>`__

