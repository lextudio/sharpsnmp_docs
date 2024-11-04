C# SNM Troubleshooting Guide
============================

This page shows you how to troubleshoot common problems.

General Approach
----------------
Troubleshooting C# SNMP related issues require basic knowledge of the following

* Computer networking (TCP/IP)
* UDP and SNMP specific
* .NET and C#

The steps below can often help determine what might be the cause of an error.

#. Does this problem reproducible? If it is reproducible, move on.
#. Do other libraries behave the same? Please test with
   `Net-SNMP <http://www.net-snmp.org/>`_ which is also open source. If not,
   move on.
#. Does the latest build in the repository work? If not, move on.
#. Is this a known issue? If not, move on.
#. Prepare an error report (with all information you can think of that is
   related) and extra information.
#. SNMP packets related: please provide network packet captures if possible
   following `How to Capture Network Packets`_ .
#. .NET exceptions: please provide stack trace information.

When the cause cannot be determined at this stage, open a bug report with the
log file or packet capture attached following "Reporting a Bug" section in
:doc:/contribute/github .

How to Capture Network Packets
------------------------------

Wireshark
^^^^^^^^^
Use `Wireshark <http://www.wireshark.org/>`_ you can capture network traffic
and analyze the packets.

.. note:: network capture can contain confidential information. Before sharing
   it with others, make sure you strip out such critical data.

System.NET Tracing
^^^^^^^^^^^^^^^^^^
System.Net tracing is another useful way to log network traffic.

.. note:: tracing log can contain confidential information. Before sharing it
   with others, make sure you strip out such critical data.

Windows ETW
^^^^^^^^^^^
Microsoft adds to latest Windows releases a built-in feature to capture
network packets via ETW, which can be enabled easily following
`this guide <https://msdn.microsoft.com/en-us/library/windows/desktop/dd569139(v=vs.85).aspx>`_ .

.. note:: tracing log can contain confidential information. Before sharing it
   with others, make sure you strip out such critical data.
