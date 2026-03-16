ErrorCode Enum
==============

.. dn:enum:: DotNetSnmp.Common.Definitions.ErrorCode

   Error code for SNMP operations. (0-5 are first defined in SNMP v1, and others are added in v2)

   .. code-block:: csharp

      [DataContract]
      public enum ErrorCode : byte

**Namespace:** ``DotNetSnmp.Common.Definitions``

**Source:** `SharpSnmpLib/Common/PduErrorStatus.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/PduErrorStatus.cs#L7>`__

Fields
------

AuthorizationError
~~~~~~~~~~~~~~~~~~

.. dn:field:: DotNetSnmp.Common.Definitions.ErrorCode.AuthorizationError

   An SNMP command could not be authenticated; in other words, someone has supplied an incorrect community string.

   .. code-block:: csharp

      AuthorizationError = 16

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.ErrorCode`

**Source:** `SharpSnmpLib/Common/PduErrorStatus.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/PduErrorStatus.cs#L93>`__

BadValue
~~~~~~~~

.. dn:field:: DotNetSnmp.Common.Definitions.ErrorCode.BadValue

   A read-write or write-only object was set to an inconsistent value.

   .. code-block:: csharp

      BadValue = 3

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.ErrorCode`

**Source:** `SharpSnmpLib/Common/PduErrorStatus.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/PduErrorStatus.cs#L28>`__

CommitFailed
~~~~~~~~~~~~

.. dn:field:: DotNetSnmp.Common.Definitions.ErrorCode.CommitFailed

   This is a catch-all error for set failures.

   .. code-block:: csharp

      CommitFailed = 14

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.ErrorCode`

**Source:** `SharpSnmpLib/Common/PduErrorStatus.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/PduErrorStatus.cs#L83>`__

GenError
~~~~~~~~

.. dn:field:: DotNetSnmp.Common.Definitions.ErrorCode.GenError

   This is a catch-all error. If an error occurs for which none of the previous messages is appropriate, a genError is issued.

   .. code-block:: csharp

      GenError = 5

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.ErrorCode`

**Source:** `SharpSnmpLib/Common/PduErrorStatus.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/PduErrorStatus.cs#L38>`__

InconsistentName
~~~~~~~~~~~~~~~~

.. dn:field:: DotNetSnmp.Common.Definitions.ErrorCode.InconsistentName

   You attempted to set a variable, but that attempt failed because the variable was in some kind of inconsistent state.

   .. code-block:: csharp

      InconsistentName = 18

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.ErrorCode`

**Source:** `SharpSnmpLib/Common/PduErrorStatus.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/PduErrorStatus.cs#L103>`__

InconsistentValue
~~~~~~~~~~~~~~~~~

.. dn:field:: DotNetSnmp.Common.Definitions.ErrorCode.InconsistentValue

   A MIB variable is in an inconsistent state, and is not accepting any set requests.

   .. code-block:: csharp

      InconsistentValue = 12

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.ErrorCode`

**Source:** `SharpSnmpLib/Common/PduErrorStatus.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/PduErrorStatus.cs#L73>`__

NoAccess
~~~~~~~~

.. dn:field:: DotNetSnmp.Common.Definitions.ErrorCode.NoAccess

   A set to an inaccessible variable was attempted. This typically occurs when the variable has an ACCESS type of not-accessible.

   .. code-block:: csharp

      NoAccess = 6

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.ErrorCode`

**Source:** `SharpSnmpLib/Common/PduErrorStatus.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/PduErrorStatus.cs#L43>`__

NoCreation
~~~~~~~~~~

.. dn:field:: DotNetSnmp.Common.Definitions.ErrorCode.NoCreation

   You tried to set a nonexistent variable or create a variable that doesn&apos;t exist in the MIB.

   .. code-block:: csharp

      NoCreation = 11

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.ErrorCode`

**Source:** `SharpSnmpLib/Common/PduErrorStatus.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/PduErrorStatus.cs#L68>`__

NoError
~~~~~~~

.. dn:field:: DotNetSnmp.Common.Definitions.ErrorCode.NoError

   There was no problem performing the request.

   .. code-block:: csharp

      NoError = 0

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.ErrorCode`

**Source:** `SharpSnmpLib/Common/PduErrorStatus.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/PduErrorStatus.cs#L13>`__

NoSuchName
~~~~~~~~~~

.. dn:field:: DotNetSnmp.Common.Definitions.ErrorCode.NoSuchName

   An agent was asked to get or set an OID that it can&apos;t find; i.e., the OID doesn&apos;t exist.

   .. code-block:: csharp

      NoSuchName = 2

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.ErrorCode`

**Source:** `SharpSnmpLib/Common/PduErrorStatus.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/PduErrorStatus.cs#L23>`__

NotWritable
~~~~~~~~~~~

.. dn:field:: DotNetSnmp.Common.Definitions.ErrorCode.NotWritable

   A variable will not accept a set, even though it is supposed to.

   .. code-block:: csharp

      NotWritable = 17

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.ErrorCode`

**Source:** `SharpSnmpLib/Common/PduErrorStatus.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/PduErrorStatus.cs#L98>`__

ReadOnly
~~~~~~~~

.. dn:field:: DotNetSnmp.Common.Definitions.ErrorCode.ReadOnly

   This error is generally not used. The noSuchName error is equivalent to this one.

   .. code-block:: csharp

      ReadOnly = 4

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.ErrorCode`

**Source:** `SharpSnmpLib/Common/PduErrorStatus.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/PduErrorStatus.cs#L33>`__

ResourceUnavailable
~~~~~~~~~~~~~~~~~~~

.. dn:field:: DotNetSnmp.Common.Definitions.ErrorCode.ResourceUnavailable

   No system resources are available to perform a set.

   .. code-block:: csharp

      ResourceUnavailable = 13

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.ErrorCode`

**Source:** `SharpSnmpLib/Common/PduErrorStatus.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/PduErrorStatus.cs#L78>`__

TooBig
~~~~~~

.. dn:field:: DotNetSnmp.Common.Definitions.ErrorCode.TooBig

   The response to your request was too big to fit into one response.

   .. code-block:: csharp

      TooBig = 1

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.ErrorCode`

**Source:** `SharpSnmpLib/Common/PduErrorStatus.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/PduErrorStatus.cs#L18>`__

UndoFailed
~~~~~~~~~~

.. dn:field:: DotNetSnmp.Common.Definitions.ErrorCode.UndoFailed

   A set failed and the agent was unable to roll back all the previous sets up until the point of failure.

   .. code-block:: csharp

      UndoFailed = 15

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.ErrorCode`

**Source:** `SharpSnmpLib/Common/PduErrorStatus.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/PduErrorStatus.cs#L88>`__

WrongEncoding
~~~~~~~~~~~~~

.. dn:field:: DotNetSnmp.Common.Definitions.ErrorCode.WrongEncoding

   A set operation was attempted using the wrong encoding for the object being set.

   .. code-block:: csharp

      WrongEncoding = 9

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.ErrorCode`

**Source:** `SharpSnmpLib/Common/PduErrorStatus.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/PduErrorStatus.cs#L58>`__

WrongLength
~~~~~~~~~~~

.. dn:field:: DotNetSnmp.Common.Definitions.ErrorCode.WrongLength

   An object&apos;s value was set to something other than what it calls for. For instance, a string can be defined to have a maximum character size. This error occurs if you try to set a string object to a value that exceeds its maximum length.

   .. code-block:: csharp

      WrongLength = 8

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.ErrorCode`

**Source:** `SharpSnmpLib/Common/PduErrorStatus.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/PduErrorStatus.cs#L53>`__

WrongType
~~~~~~~~~

.. dn:field:: DotNetSnmp.Common.Definitions.ErrorCode.WrongType

   An object was set to a type that is different from its definition. This error will occur if you try to set an object that is of type INTEGER to a string, for example.

   .. code-block:: csharp

      WrongType = 7

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.ErrorCode`

**Source:** `SharpSnmpLib/Common/PduErrorStatus.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/PduErrorStatus.cs#L48>`__

WrongValue
~~~~~~~~~~

.. dn:field:: DotNetSnmp.Common.Definitions.ErrorCode.WrongValue

   A variable was set to a value it doesn&apos;t understand. This can occur when a read-write is defined as an enumeration, and you try to set it to a value that is not one of the enumerated types.

   .. code-block:: csharp

      WrongValue = 10

   :rtype: :dn:enum:`~DotNetSnmp.Common.Definitions.ErrorCode`

**Source:** `SharpSnmpLib/Common/PduErrorStatus.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/PduErrorStatus.cs#L63>`__

