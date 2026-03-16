Discoverer Class
================

.. dn:class:: Lextm.SharpSnmpLib.Messaging.Discoverer

   Discoverer class to discover SNMP agents in the same network.

   .. code-block:: csharp

      public sealed class Discoverer

**Namespace:** ``Lextm.SharpSnmpLib.Messaging``

**Inheritance:** Object → ``Discoverer``

**Source:** `SharpSnmpLib/Messaging/Discoverer.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Discoverer.cs#L97>`__

Methods
-------

Discover(VersionCode, IPEndPoint, Nullable<OctetString>, Int32, ISnmpTransport)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Discoverer.Discover(DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,System.Nullable{DotNetSnmp.Asn1.SyntaxObjects.OctetString},System.Int32,DotNetSnmp.Transport.ISnmpTransport)

   Discovers agents of the specified version using the specified transport.

   .. code-block:: csharp

      public void Discover(VersionCode version, IPEndPoint endpoint, OctetString? community, int timeout, ISnmpTransport transport)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type endpoint: ``IPEndPoint``
   :type community: ``Nullable<OctetString>``
   :type timeout: ``Int32``
   :type transport: :dn:iface:`~DotNetSnmp.Transport.ISnmpTransport`

**Source:** `SharpSnmpLib/Messaging/Discoverer.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Discoverer.cs#L123>`__

Discover(VersionCode, IPEndPoint, Nullable<OctetString>, Int32, OctetString, ISnmpTransport)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Discoverer.Discover(DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,System.Nullable{DotNetSnmp.Asn1.SyntaxObjects.OctetString},System.Int32,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Transport.ISnmpTransport)

   Discovers agents of the specified version using the specified transport.

   .. code-block:: csharp

      public void Discover(VersionCode version, IPEndPoint endpoint, OctetString? community, int timeout, OctetString contextName, ISnmpTransport transport)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type endpoint: ``IPEndPoint``
   :type community: ``Nullable<OctetString>``
   :type timeout: ``Int32``
   :type contextName: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type transport: :dn:iface:`~DotNetSnmp.Transport.ISnmpTransport`

**Source:** `SharpSnmpLib/Messaging/Discoverer.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Discoverer.cs#L131>`__

Discover(VersionCode, IPEndPoint, Nullable<OctetString>, Int32, OctetString)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Discoverer.Discover(DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,System.Nullable{DotNetSnmp.Asn1.SyntaxObjects.OctetString},System.Int32,DotNetSnmp.Asn1.SyntaxObjects.OctetString)

   Discovers agents of the specified version in a specific time interval.

   .. code-block:: csharp

      public void Discover(VersionCode version, IPEndPoint broadcastAddress, OctetString? community, int timeout, OctetString contextName)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type broadcastAddress: ``IPEndPoint``
   :type community: ``Nullable<OctetString>``
   :type timeout: ``Int32``
   :type contextName: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`

**Source:** `SharpSnmpLib/Messaging/Discoverer.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Discoverer.cs#L115>`__

Discover(VersionCode, IPEndPoint, Nullable<OctetString>, Int32)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Discoverer.Discover(DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,System.Nullable{DotNetSnmp.Asn1.SyntaxObjects.OctetString},System.Int32)

   Discovers agents of the specified version in a specific time interval.

   .. code-block:: csharp

      public void Discover(VersionCode version, IPEndPoint broadcastAddress, OctetString? community, int timeout)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type broadcastAddress: ``IPEndPoint``
   :type community: ``Nullable<OctetString>``
   :type timeout: ``Int32``

**Source:** `SharpSnmpLib/Messaging/Discoverer.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Discoverer.cs#L107>`__

DiscoverAsync(VersionCode, IPEndPoint, Nullable<OctetString>, Int32, ISnmpTransport)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Discoverer.DiscoverAsync(DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,System.Nullable{DotNetSnmp.Asn1.SyntaxObjects.OctetString},System.Int32,DotNetSnmp.Transport.ISnmpTransport)

   Discovers agents of the specified version using the specified transport.

   .. code-block:: csharp

      public Task DiscoverAsync(VersionCode version, IPEndPoint endpoint, OctetString? community, int timeout, ISnmpTransport transport)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type endpoint: ``IPEndPoint``
   :type community: ``Nullable<OctetString>``
   :type timeout: ``Int32``
   :type transport: :dn:iface:`~DotNetSnmp.Transport.ISnmpTransport`

   :rtype: ``Task``

**Source:** `SharpSnmpLib/Messaging/Discoverer.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Discoverer.cs#L151>`__

DiscoverAsync(VersionCode, IPEndPoint, Nullable<OctetString>, Int32, OctetString, ISnmpTransport)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Discoverer.DiscoverAsync(DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,System.Nullable{DotNetSnmp.Asn1.SyntaxObjects.OctetString},System.Int32,DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Transport.ISnmpTransport)

   Discovers agents of the specified version using the specified transport.

   .. code-block:: csharp

      public Task DiscoverAsync(VersionCode version, IPEndPoint endpoint, OctetString? community, int timeout, OctetString contextName, ISnmpTransport transport)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type endpoint: ``IPEndPoint``
   :type community: ``Nullable<OctetString>``
   :type timeout: ``Int32``
   :type contextName: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :type transport: :dn:iface:`~DotNetSnmp.Transport.ISnmpTransport`

   :rtype: ``Task``

**Source:** `SharpSnmpLib/Messaging/Discoverer.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Discoverer.cs#L238>`__

DiscoverAsync(VersionCode, IPEndPoint, Nullable<OctetString>, Int32, OctetString)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Discoverer.DiscoverAsync(DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,System.Nullable{DotNetSnmp.Asn1.SyntaxObjects.OctetString},System.Int32,DotNetSnmp.Asn1.SyntaxObjects.OctetString)

   Discovers agents of the specified version in a specific time interval.

   .. code-block:: csharp

      public Task DiscoverAsync(VersionCode version, IPEndPoint broadcastAddress, OctetString? community, int timeout, OctetString contextName)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type broadcastAddress: ``IPEndPoint``
   :type community: ``Nullable<OctetString>``
   :type timeout: ``Int32``
   :type contextName: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`

   :rtype: ``Task``

**Source:** `SharpSnmpLib/Messaging/Discoverer.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Discoverer.cs#L164>`__

DiscoverAsync(VersionCode, IPEndPoint, Nullable<OctetString>, Int32)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.Discoverer.DiscoverAsync(DotNetSnmp.Common.Definitions.VersionCode,System.Net.IPEndPoint,System.Nullable{DotNetSnmp.Asn1.SyntaxObjects.OctetString},System.Int32)

   Discovers agents of the specified version in a specific time interval.

   .. code-block:: csharp

      public Task DiscoverAsync(VersionCode version, IPEndPoint broadcastAddress, OctetString? community, int timeout)

   :type version: :dn:enum:`~DotNetSnmp.Common.Definitions.VersionCode`
   :type broadcastAddress: ``IPEndPoint``
   :type community: ``Nullable<OctetString>``
   :type timeout: ``Int32``

   :rtype: ``Task``

**Source:** `SharpSnmpLib/Messaging/Discoverer.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Discoverer.cs#L139>`__

Events
------

AgentFound
~~~~~~~~~~

.. dn:event:: Lextm.SharpSnmpLib.Messaging.Discoverer.AgentFound

   Occurs when an SNMP agent is found.

   .. code-block:: csharp

      public event EventHandler<AgentFoundEventArgs>? AgentFound

   :rtype: ``EventHandler<AgentFoundEventArgs>``

**Source:** `SharpSnmpLib/Messaging/Discoverer.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Discoverer.cs#L102>`__

