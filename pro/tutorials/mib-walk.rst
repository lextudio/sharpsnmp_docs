Enhanced SNMP WALK
==================

This page shows you information about how to utilize MIB documents to enhance
SNMP WALK operations.

Background
----------
C# SNMP Library has a sample project ``snmpd`` that can work as a test agent.

If we use ``snmpwalk`` sample to query all objects from this agent, the following
information can be seen,

.. code-block:: text

   > ./snmpwalk.exe -c=public -v=1 -m=subtree localhost 1.3.6
   Variable: Id: 1.3.6.1.2.1.1.1.0; Data: #SNMP Agent on .NET Standard
   Variable: Id: 1.3.6.1.2.1.1.2.0; Data: 1.3.6.1
   Variable: Id: 1.3.6.1.2.1.1.3.0; Data: 00:04:20.9500000
   Variable: Id: 1.3.6.1.2.1.1.4.0; Data: UNKNOWN
   Variable: Id: 1.3.6.1.2.1.1.5.0; Data: UNKNOWN
   Variable: Id: 1.3.6.1.2.1.1.6.0; Data:
   Variable: Id: 1.3.6.1.2.1.1.7.0; Data: 72
   Variable: Id: 1.3.6.1.2.1.1.8.0; Data: 00:00:00
   Variable: Id: 1.3.6.1.2.1.1.9.1.1.1; Data: 1
   Variable: Id: 1.3.6.1.2.1.1.9.1.1.2; Data: 2
   Variable: Id: 1.3.6.1.2.1.1.9.1.2.1; Data: 1.3
   Variable: Id: 1.3.6.1.2.1.1.9.1.2.2; Data: 1.4
   Variable: Id: 1.3.6.1.2.1.1.9.1.3.1; Data: Test1
   Variable: Id: 1.3.6.1.2.1.1.9.1.3.2; Data: Test2
   Variable: Id: 1.3.6.1.2.1.1.9.1.4.1; Data: 00:00:00.0100000
   Variable: Id: 1.3.6.1.2.1.1.9.1.4.2; Data: 00:00:00.0200000
   Variable: Id: 1.3.6.1.2.1.2.1.0; Data: 3
   Variable: Id: 1.3.6.1.2.1.2.2.1.1.1; Data: 1
   Variable: Id: 1.3.6.1.2.1.2.2.1.1.2; Data: 2
   Variable: Id: 1.3.6.1.2.1.2.2.1.1.3; Data: 3
   Variable: Id: 1.3.6.1.2.1.2.2.1.2.1; Data: Microsoft Hyper-V Network Adapter
   Variable: Id: 1.3.6.1.2.1.2.2.1.2.2; Data: Microsoft Hyper-V Network Adapter #2
   Variable: Id: 1.3.6.1.2.1.2.2.1.2.3; Data: Software Loopback Interface 1
   Variable: Id: 1.3.6.1.2.1.2.2.1.3.1; Data: 6
   Variable: Id: 1.3.6.1.2.1.2.2.1.3.2; Data: 6
   Variable: Id: 1.3.6.1.2.1.2.2.1.3.3; Data: 24
   Variable: Id: 1.3.6.1.2.1.2.2.1.4.1; Data: 1500
   Variable: Id: 1.3.6.1.2.1.2.2.1.4.2; Data: 1500
   Variable: Id: 1.3.6.1.2.1.2.2.1.4.3; Data: -1
   Variable: Id: 1.3.6.1.2.1.2.2.1.5.1; Data: 1410065408
   Variable: Id: 1.3.6.1.2.1.2.2.1.5.2; Data: 866700000
   Variable: Id: 1.3.6.1.2.1.2.2.1.5.3; Data: 1073741824
   Variable: Id: 1.3.6.1.2.1.2.2.1.6.1; Data:  §☺☺
   Variable: Id: 1.3.6.1.2.1.2.2.1.6.2; Data:  §☻☺
   Variable: Id: 1.3.6.1.2.1.2.2.1.6.3; Data:
   Variable: Id: 1.3.6.1.2.1.2.2.1.7.1; Data: 1
   Variable: Id: 1.3.6.1.2.1.2.2.1.7.2; Data: 1
   Variable: Id: 1.3.6.1.2.1.2.2.1.7.3; Data: 1
   Variable: Id: 1.3.6.1.2.1.2.2.1.8.1; Data: 1
   Variable: Id: 1.3.6.1.2.1.2.2.1.8.2; Data: 1
   Variable: Id: 1.3.6.1.2.1.2.2.1.8.3; Data: 1
   Variable: Id: 1.3.6.1.2.1.2.2.1.9.1; Data: 00:00:00
   Variable: Id: 1.3.6.1.2.1.2.2.1.9.2; Data: 00:00:00
   Variable: Id: 1.3.6.1.2.1.2.2.1.9.3; Data: 00:00:00
   Variable: Id: 1.3.6.1.2.1.2.2.1.10.1; Data: 7168160
   Variable: Id: 1.3.6.1.2.1.2.2.1.10.2; Data: 49028
   Variable: Id: 1.3.6.1.2.1.2.2.1.10.3; Data: 0
   Variable: Id: 1.3.6.1.2.1.2.2.1.11.1; Data: 6362
   Variable: Id: 1.3.6.1.2.1.2.2.1.11.2; Data: 208
   Variable: Id: 1.3.6.1.2.1.2.2.1.11.3; Data: 0
   Variable: Id: 1.3.6.1.2.1.2.2.1.12.1; Data: 92
   Variable: Id: 1.3.6.1.2.1.2.2.1.12.2; Data: 104
   Variable: Id: 1.3.6.1.2.1.2.2.1.12.3; Data: 0
   Variable: Id: 1.3.6.1.2.1.2.2.1.13.1; Data: 0
   Variable: Id: 1.3.6.1.2.1.2.2.1.13.2; Data: 0
   Variable: Id: 1.3.6.1.2.1.2.2.1.13.3; Data: 0
   Variable: Id: 1.3.6.1.2.1.2.2.1.14.1; Data: 0
   Variable: Id: 1.3.6.1.2.1.2.2.1.14.2; Data: 0
   Variable: Id: 1.3.6.1.2.1.2.2.1.14.3; Data: 0
   Variable: Id: 1.3.6.1.2.1.2.2.1.15.1; Data: 0
   Variable: Id: 1.3.6.1.2.1.2.2.1.15.2; Data: 0
   Variable: Id: 1.3.6.1.2.1.2.2.1.15.3; Data: 0
   Variable: Id: 1.3.6.1.2.1.2.2.1.16.1; Data: 1131548
   Variable: Id: 1.3.6.1.2.1.2.2.1.16.2; Data: 32719
   Variable: Id: 1.3.6.1.2.1.2.2.1.16.3; Data: 0
   Variable: Id: 1.3.6.1.2.1.2.2.1.17.1; Data: 4480
   Variable: Id: 1.3.6.1.2.1.2.2.1.17.2; Data: 203
   Variable: Id: 1.3.6.1.2.1.2.2.1.17.3; Data: 0
   Variable: Id: 1.3.6.1.2.1.2.2.1.18.1; Data: 213
   Variable: Id: 1.3.6.1.2.1.2.2.1.18.2; Data: 156
   Variable: Id: 1.3.6.1.2.1.2.2.1.18.3; Data: 0
   Variable: Id: 1.3.6.1.2.1.2.2.1.19.1; Data: 0
   Variable: Id: 1.3.6.1.2.1.2.2.1.19.2; Data: 0
   Variable: Id: 1.3.6.1.2.1.2.2.1.19.3; Data: 0
   Variable: Id: 1.3.6.1.2.1.2.2.1.20.1; Data: 0
   Variable: Id: 1.3.6.1.2.1.2.2.1.20.2; Data: 0
   Variable: Id: 1.3.6.1.2.1.2.2.1.20.3; Data: 0
   Variable: Id: 1.3.6.1.2.1.2.2.1.21.1; Data: 0
   Variable: Id: 1.3.6.1.2.1.2.2.1.21.2; Data: 0
   Variable: Id: 1.3.6.1.2.1.2.2.1.21.3; Data: 0
   Variable: Id: 1.3.6.1.2.1.2.2.1.22.1; Data: 0.0
   Variable: Id: 1.3.6.1.2.1.2.2.1.22.2; Data: 0.0
   Variable: Id: 1.3.6.1.2.1.2.2.1.22.3; Data: 0.0

The output has several issues that you can easily identify,

* All OIDs are in numeric form.
* Special encoded data such as MAC addresses (like ``1.3.6.1.2.1.2.2.1.6.1``),
  bits (such as ``1.3.6.1.2.1.2.2.1.7.1``) are displayed in raw format.

Utilizing MIB Documents
-----------------------
If we switch to an enhanced version of ``snmpwalk``, then the output looks like
this,

.. code-block:: text

   > ./snmpwalk.exe -c=public -v=1 -m=subtree localhost 1.3.6
   Variable: Id: SNMPv2-MIB::sysDescr.0; Data: #SNMP Agent on .NET Standard
   Variable: Id: SNMPv2-MIB::sysObjectID.0; Data: 1.3.6.1
   Variable: Id: SNMPv2-MIB::sysUpTime.0; Data: 00:10:54
   Variable: Id: SNMPv2-MIB::sysContact.0; Data: UNKNOWN
   Variable: Id: SNMPv2-MIB::sysName.0; Data: UNKNOWN
   Variable: Id: SNMPv2-MIB::sysLocation.0; Data:
   Variable: Id: SNMPv2-MIB::sysServices.0; Data: 72
   Variable: Id: SNMPv2-MIB::sysORLastChange.0; Data: 00:00:00
   Variable: Id: SNMPv2-MIB::sysORIndex.1; Data: 1
   Variable: Id: SNMPv2-MIB::sysORIndex.2; Data: 2
   Variable: Id: SNMPv2-MIB::sysORID.1; Data: 1.3
   Variable: Id: SNMPv2-MIB::sysORID.2; Data: 1.4
   Variable: Id: SNMPv2-MIB::sysORDescr.1; Data: Test1
   Variable: Id: SNMPv2-MIB::sysORDescr.2; Data: Test2
   Variable: Id: SNMPv2-MIB::sysORUpTime.1; Data: 00:00:00.0100000
   Variable: Id: SNMPv2-MIB::sysORUpTime.2; Data: 00:00:00.0200000
   Variable: Id: IF-MIB::ifNumber.0; Data: 3
   Variable: Id: IF-MIB::ifIndex.1; Data: 1
   Variable: Id: IF-MIB::ifIndex.2; Data: 2
   Variable: Id: IF-MIB::ifIndex.3; Data: 3
   Variable: Id: IF-MIB::ifDescr.1; Data: Microsoft Hyper-V Network Adapter
   Variable: Id: IF-MIB::ifDescr.2; Data: Microsoft Hyper-V Network Adapter #2
   Variable: Id: IF-MIB::ifDescr.3; Data: Software Loopback Interface 1
   Variable: Id: IF-MIB::ifType.1; Data: ethernetCsmacd(6)
   Variable: Id: IF-MIB::ifType.2; Data: ethernetCsmacd(6)
   Variable: Id: IF-MIB::ifType.3; Data: softwareLoopback(24)
   Variable: Id: IF-MIB::ifMtu.1; Data: 1500
   Variable: Id: IF-MIB::ifMtu.2; Data: 1500
   Variable: Id: IF-MIB::ifMtu.3; Data: -1
   Variable: Id: IF-MIB::ifSpeed.1; Data: 1410065408
   Variable: Id: IF-MIB::ifSpeed.2; Data: 866700000
   Variable: Id: IF-MIB::ifSpeed.3; Data: 1073741824
   Variable: Id: IF-MIB::ifPhysAddress.1; Data: 00-15-5D-01-08-01
   Variable: Id: IF-MIB::ifPhysAddress.2; Data: 00-15-5D-01-08-02
   Variable: Id: IF-MIB::ifPhysAddress.3; Data:
   Variable: Id: IF-MIB::ifAdminStatus.1; Data: up(1)
   Variable: Id: IF-MIB::ifAdminStatus.2; Data: up(1)
   Variable: Id: IF-MIB::ifAdminStatus.3; Data: up(1)
   Variable: Id: IF-MIB::ifOperStatus.1; Data: up(1)
   Variable: Id: IF-MIB::ifOperStatus.2; Data: up(1)
   Variable: Id: IF-MIB::ifOperStatus.3; Data: up(1)
   Variable: Id: IF-MIB::ifLastChange.1; Data: 00:00:00
   Variable: Id: IF-MIB::ifLastChange.2; Data: 00:00:00
   Variable: Id: IF-MIB::ifLastChange.3; Data: 00:00:00
   Variable: Id: IF-MIB::ifInOctets.1; Data: 10431787
   Variable: Id: IF-MIB::ifInOctets.2; Data: 60373
   Variable: Id: IF-MIB::ifInOctets.3; Data: 0
   Variable: Id: IF-MIB::ifInUcastPkts.1; Data: 8868
   Variable: Id: IF-MIB::ifInUcastPkts.2; Data: 277
   Variable: Id: IF-MIB::ifInUcastPkts.3; Data: 0
   Variable: Id: IF-MIB::ifInNUcastPkts.1; Data: 93
   Variable: Id: IF-MIB::ifInNUcastPkts.2; Data: 139
   Variable: Id: IF-MIB::ifInNUcastPkts.3; Data: 0
   Variable: Id: IF-MIB::ifInDiscards.1; Data: 0
   Variable: Id: IF-MIB::ifInDiscards.2; Data: 0
   Variable: Id: IF-MIB::ifInDiscards.3; Data: 0
   Variable: Id: IF-MIB::ifInErrors.1; Data: 0
   Variable: Id: IF-MIB::ifInErrors.2; Data: 0
   Variable: Id: IF-MIB::ifInErrors.3; Data: 0
   Variable: Id: IF-MIB::ifInUnknownProtos.1; Data: 0
   Variable: Id: IF-MIB::ifInUnknownProtos.2; Data: 0
   Variable: Id: IF-MIB::ifInUnknownProtos.3; Data: 0
   Variable: Id: IF-MIB::ifOutOctets.1; Data: 1341284
   Variable: Id: IF-MIB::ifOutOctets.2; Data: 37650
   Variable: Id: IF-MIB::ifOutOctets.3; Data: 0
   Variable: Id: IF-MIB::ifOutUcastPkts.1; Data: 6057
   Variable: Id: IF-MIB::ifOutUcastPkts.2; Data: 272
   Variable: Id: IF-MIB::ifOutUcastPkts.3; Data: 0
   Variable: Id: IF-MIB::ifOutNUcastPkts.1; Data: 213
   Variable: Id: IF-MIB::ifOutNUcastPkts.2; Data: 156
   Variable: Id: IF-MIB::ifOutNUcastPkts.3; Data: 0
   Variable: Id: IF-MIB::ifOutDiscards.1; Data: 0
   Variable: Id: IF-MIB::ifOutDiscards.2; Data: 0
   Variable: Id: IF-MIB::ifOutDiscards.3; Data: 0
   Variable: Id: IF-MIB::ifOutErrors.1; Data: 0
   Variable: Id: IF-MIB::ifOutErrors.2; Data: 0
   Variable: Id: IF-MIB::ifOutErrors.3; Data: 0
   Variable: Id: IF-MIB::ifOutQLen.1; Data: 0
   Variable: Id: IF-MIB::ifOutQLen.2; Data: 0
   Variable: Id: IF-MIB::ifOutQLen.3; Data: 0
   Variable: Id: IF-MIB::ifSpecific.1; Data: 0.0
   Variable: Id: IF-MIB::ifSpecific.2; Data: 0.0
   Variable: Id: IF-MIB::ifSpecific.3; Data: 0.0

Not only all OIDs are displayed in textual form, but also we see MAC addresses
and bits in correct format (like ``00-15-5D-01-08-01`` and ``up(1)``).

You can find the sample code at `GitHub <https://github.com/lextudio/sharpsnmppro-samples/tree/release_2.1/snmpwalk_cs>`_.

Related Resources
-----------------

- :doc:`/support/purchase`
- `Requesting Trial <https://www.sharpsnmp.com/#contact-us>`_
- :doc:`/tutorials/assembly-trial-guide`
- :doc:`/tutorials/assembly-full-guide`
