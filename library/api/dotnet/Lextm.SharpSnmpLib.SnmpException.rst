SnmpException Class
===================

.. dn:class:: Lextm.SharpSnmpLib.SnmpException

   Base exception type of #SNMP.

   .. code-block:: csharp

      public class SnmpException : Exception, ISerializable

**Namespace:** ``Lextm.SharpSnmpLib``

**Inheritance:** Object → Exception → ``SnmpException``

**Source:** `SharpSnmpLib/SnmpException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SnmpException.cs#L8>`__

Constructors
------------

SnmpException()
~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.SnmpException..ctor

   Initializes a new instance of SnmpException.

   .. code-block:: csharp

      public SnmpException()

**Source:** `SharpSnmpLib/SnmpException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SnmpException.cs#L13>`__

SnmpException(String, Exception)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.SnmpException..ctor(System.String,System.Exception)

   Initializes a new instance of SnmpException.

   .. code-block:: csharp

      public SnmpException(string message, Exception innerException)

   :type message: ``String``
   :type innerException: ``Exception``

**Source:** `SharpSnmpLib/SnmpException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SnmpException.cs#L28>`__

SnmpException(String)
~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.SnmpException..ctor(System.String)

   Initializes a new instance of SnmpException.

   .. code-block:: csharp

      public SnmpException(string message)

   :type message: ``String``

**Source:** `SharpSnmpLib/SnmpException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SnmpException.cs#L20>`__

