ErrorException Class
====================

.. dn:class:: Lextm.SharpSnmpLib.ErrorException

   Represents the ErrorException type.

   .. code-block:: csharp

      public sealed class ErrorException : SnmpException, ISerializable

**Namespace:** ``Lextm.SharpSnmpLib``

**Inheritance:** Object → Exception → SnmpException → ``ErrorException``

**Source:** `SharpSnmpLib/SnmpException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SnmpException.cs#L37>`__

Properties
----------

Address
~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.ErrorException.Address

   Gets address.

   .. code-block:: csharp

      public IPAddress Address { get; }

   :rtype: ``IPAddress``

**Source:** `SharpSnmpLib/SnmpException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SnmpException.cs#L49>`__

Response
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.ErrorException.Response

   Gets response.

   .. code-block:: csharp

      public ISnmpMessage Response { get; }

   :rtype: :dn:iface:`~DotNetSnmp.Common.Definitions.ISnmpMessage`

**Source:** `SharpSnmpLib/SnmpException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SnmpException.cs#L54>`__

Methods
-------

Create(String, IPAddress, ISnmpMessage)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.ErrorException.Create(System.String,System.Net.IPAddress,DotNetSnmp.Common.Definitions.ISnmpMessage)

   Creates an :dn:cls:``~Lextm.SharpSnmpLib.ErrorException`` for a failed SNMP response.

   .. code-block:: csharp

      public static ErrorException Create(string message, IPAddress address, ISnmpMessage response)

   :type message: ``String``
   :type address: ``IPAddress``
   :type response: :dn:iface:`~DotNetSnmp.Common.Definitions.ISnmpMessage`

   :rtype: :dn:cls:`~Lextm.SharpSnmpLib.ErrorException`

**Source:** `SharpSnmpLib/SnmpException.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/SnmpException.cs#L59>`__

