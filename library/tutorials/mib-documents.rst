Beginners's Guide on MIB Documents
==================================

By `Lex Li`_

This page shows you which roles MIB documents play in SNMP communication. 

.. important:: It is highly recommended that you buy a book such as `Understanding SNMP MIBs <http://www.amazon.com/Understanding-SNMP-MIBs-David-Perkins/dp/0134377087>`_ to learn from the masters of this art.

.. contents:: In this article:
  :local:
  :depth: 1

Background
----------
MIB documents can be found from SNMP RFC documents, product manuals, and Internet downloads. So why do they exist and do I need them? The answer varies for each roles you play.

Device Vendors
--------------
If you are going to sell an SNMP enabled device, you need to prepare user manuals and also provide the MIB documents to your customers. Your developers have implemented management 
objects in the agent software, which is invisible to everyone else. 

The customers can only learn how to manage the device via the MIB documents you provide.

Device Administrators
---------------------
If you bought an SNMP enabled device from a vendor, make sure you grab the MIB documents and learn carefully which objects are exposed.

You can import the MIB documents to a monitor software, or write your own software to monitor the objects.

SNMP OID, Data Type, and Description
------------------------------------
From the MIB documents you know the identifiers (OID) of the management objects, their data types, and descriptions. That information can then be put down to papers.

You can use #SNMP Library with MIB documents, as only OID is required during request construction in most cases. Of course data type is needed when performing SET operations. 
The descriptions help you understand the meaning of the data you get from the agent.

Related Resources
-----------------

- `#SNMP MIB Compiler Pro <http://pro.sharpsnmp.com/en/latest/getting-started/compiler-features.html>`_
- `SharpSnmpPro.Mib Assembly <http://pro.sharpsnmp.com/en/latest/getting-started/assembly-features.html>`_
