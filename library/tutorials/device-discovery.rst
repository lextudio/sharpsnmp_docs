SNMP Device Discovery
=====================

By `Lex Li`_

This page shows you how SNMP device might be discovered.

.. contents:: In this article:
  :local:
  :depth: 1

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

Simple Device Discovery for v1 and v2c (IPv4)
---------------------------------------------
UDP allows broadcast, so if we broadcast an SNMP GET request with OID
``1.3.6.1.2.1.1.1.0`` using community name ``"public"``, some devices will
reply with their device information. In this way we know both the device IP
address and type from the replies.

.. note:: You should avoid using "public" as community name, as it is so well
   known.

Discovery for v3 (IPv4)
-----------------------
RFC 3414 defines a discovery process for SNMP v3. This gives us a chance to
discover all v3 enabled devices in the same network by broadcasting a simple
discovery request without any credentials.

As in this way the device IP address is revealed, make sure your devices don't
use a common user name and passwords.

Related Resources
-----------------

- :doc:`/samples/command-line-tools`
- :doc:`/tutorials/introduction`
- :doc:`/tutorials/v3-operations`
