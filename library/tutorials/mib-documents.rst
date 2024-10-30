Beginners's Guide on MIB Documents
==================================

This page shows you which roles MIB documents play in SNMP communication.

.. important:: It is highly recommended that you buy a book such as
   `Understanding SNMP MIBs <http://www.amazon.com/Understanding-SNMP-MIBs-David-Perkins/dp/0134377087>`_
   to learn from the masters of this art.

Background
----------
MIB documents can be found from SNMP RFC documents, product manuals, and
Internet downloads. So why do they exist and do I need them? The answer varies
for each roles you play.

Device Vendors
--------------
If you are going to sell an SNMP enabled device, you need to prepare user
manuals and also provide the MIB documents to your customers. Your developers
have implemented management objects in the agent software, which is invisible
to everyone else.

The customers can only learn how to manage the device via the MIB documents
you provide.

Device Administrators
---------------------
If you bought an SNMP enabled device from a vendor, make sure you grab the MIB
documents and learn carefully which objects are exposed.

You can import the MIB documents to a monitor software, or write your own
software to monitor the objects.

SNMP OIDs, Data Types, and Descriptions
---------------------------------------
From the MIB documents you know what are the management objects that can be used,
their identifiers (OIDs), data types, and descriptions. That information can then
be put down to papers.

When your application uses C# SNMP Library to perform SNMP operations, only OIDs
are required in most cases, and basic data types are needed when performing SET
operations. The descriptions help you understand the meaning of the data you get
from the agent but they are not used anywhere in typical SNMP applications.

However, if your application requires more advanced features, such as strict data
validation based on complex data types defined in MIB documents (often are
textual conventions), then you need to parse MIB documents on-the-fly and
enable the validation rules. We have a commercial product line,
`#SNMP Pro <https://pro.sharpsnmp.com>`, which contains the functionality you
need.

Related Resources
-----------------

- `#SNMP MIB Compiler Pro <https://pro.sharpsnmp.com/getting-started/compiler-features.html>`_
- `SharpSnmpPro.Mib Assembly <https://pro.sharpsnmp.com/getting-started/assembly-features.html>`_
