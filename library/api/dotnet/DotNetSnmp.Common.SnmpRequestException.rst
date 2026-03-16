SnmpRequestException Class
==========================

.. dn:class:: DotNetSnmp.Common.SnmpRequestException

   Represents the SnmpRequestException type.

   .. code-block:: csharp

      public class SnmpRequestException : Exception, ISerializable

**Namespace:** ``DotNetSnmp.Common``

**Inheritance:** Object → Exception → ``SnmpRequestException``

**Source:** `SharpSnmpLib/Common/SnmpRequestException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/SnmpRequestException.cs#L7>`__

Constructors
------------

SnmpRequestException(ErrorCode, Int32)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Common.SnmpRequestException..ctor(DotNetSnmp.Common.Definitions.ErrorCode,System.Int32)

   Initializes a new instance of SnmpRequestException.

   .. code-block:: csharp

      public SnmpRequestException(ErrorCode err, int errIdx)

   :type err: :dn:enum:`~DotNetSnmp.Common.Definitions.ErrorCode`
   :type errIdx: ``Int32``

**Source:** `SharpSnmpLib/Common/SnmpRequestException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/SnmpRequestException.cs#L12>`__

