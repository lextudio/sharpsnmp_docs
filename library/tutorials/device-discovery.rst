SNMP Device Discovery
=====================

This page shows you how SNMP device might be discovered.

Background
----------
When SNMP was defined and published, there was no official way to discover
SNMP enabled devices in the network. This might be caused by the well known
security issues of SNMP itself, as if you know there is such a device in the
network, you can somehow sniff the wire to get community names. Thus, if you
are a device administrator, make sure you hide the devices if they should not
be discovered.

However, some SNMP products, such as SNMP MIB browsers, might use an
unofficial way to detect devices. Our sample, snmpdiscover, implements one
common approach.

.. attention:: The following device discovery approaches rely on UDP
   broadcasting. THerefore, they are valid only for IPv4. IPv6 does not
   support broadcasting.

.. error:: If you are the network administrators and hit this page, think
   twice whether you need to discover devices. Keep in mind that you are
   supposed to know all the devices and their IP addresses.

Simple Device Discovery for v1 and v2c, IPv4
--------------------------------------------
UDP allows broadcast, so if we broadcast an SNMP GET request with OID
``1.3.6.1.2.1.1.1.0`` using community name ``"public"``, some devices will
reply with their device information. In this way we know both the device IP
address and type from the replies.

.. note:: You should avoid using "public" as community name, as it is so well
   known.

Discovery for v3, IPv4
----------------------
RFC 3414 defines a discovery process for SNMP v3. This gives us a chance to
discover all v3 enabled devices in the same network by broadcasting a simple
discovery request without any credentials.

As in this way the device IP address is revealed, make sure your devices don't
use a common user name and passwords.

Discovery for IPv6
------------------
IPv6 does not support broadcasting, so the above approaches are not valid for
IPv6. However, you can use the SNMP v3 discovery process to discover devices
in the same network if multicast is enabled.

.. note::

   This IPv6 feature was added in release 12.5.5.

Related Resources
-----------------

- :doc:`/samples/command-line-tools`
- :doc:`/tutorials/introduction`
- :doc:`/tutorials/v3-operations`
