UdpEndpoint Class
=================

.. dn:class:: DotNetSnmp.Transport.UdpEndpoint

   Represents the UdpEndpoint type.

   .. code-block:: csharp

      public class UdpEndpoint : IAsnSerializable

**Namespace:** ``DotNetSnmp.Transport``

**Inheritance:** Object → ``UdpEndpoint``

**Source:** `SharpSnmpLib/Transport/UdpEndpoint.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/UdpEndpoint.cs#L11>`__

Constructors
------------

UdpEndpoint(Int32)
~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Transport.UdpEndpoint..ctor(System.Int32)

   Initializes a new instance of UdpEndpoint.

   .. code-block:: csharp

      public UdpEndpoint(int port)

   :type port: ``Int32``

**Source:** `SharpSnmpLib/Transport/UdpEndpoint.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/UdpEndpoint.cs#L27>`__

UdpEndpoint(IPEndPoint)
~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Transport.UdpEndpoint..ctor(System.Net.IPEndPoint)

   Initializes a new instance of UdpEndpoint.

   .. code-block:: csharp

      public UdpEndpoint(IPEndPoint endpoint)

   :type endpoint: ``IPEndPoint``

**Source:** `SharpSnmpLib/Transport/UdpEndpoint.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/UdpEndpoint.cs#L35>`__

UdpEndpoint(String, Int32)
~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Transport.UdpEndpoint..ctor(System.String,System.Int32)

   Initializes a new instance of UdpEndpoint.

   .. code-block:: csharp

      public UdpEndpoint(string address, int port)

   :type address: ``String``
   :type port: ``Int32``

**Source:** `SharpSnmpLib/Transport/UdpEndpoint.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/UdpEndpoint.cs#L43>`__

UdpEndpoint(String)
~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Transport.UdpEndpoint..ctor(System.String)

   Initializes a new instance of UdpEndpoint.

   .. code-block:: csharp

      public UdpEndpoint(string address)

   :type address: ``String``

**Source:** `SharpSnmpLib/Transport/UdpEndpoint.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/UdpEndpoint.cs#L52>`__

Properties
----------

Port
~~~~

.. dn:property:: DotNetSnmp.Transport.UdpEndpoint.Port

   Represents this member.

   .. code-block:: csharp

      public int Port { get; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Transport/UdpEndpoint.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/UdpEndpoint.cs#L18>`__

Methods
-------

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Transport.UdpEndpoint.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/Transport/UdpEndpoint.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Transport/UdpEndpoint.cs#L81>`__

