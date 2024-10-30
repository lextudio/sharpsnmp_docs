Command Line Tools
==================

This page shows you what are the command line tools shipped.

How to Acquire The Command Line Tools
-------------------------------------

.. note:: The sample projects have been moved to
   `a new location <https://github.com/lextudio/sharpsnmplib-samples>`_.

Please acquire the source code and then launch Visual Studio 2017 to open
``SharpSnmpLib.Samples.sln``.

The sample projects are under the "Samples" folder and divided into two
languages, C# and VB.NET. Compile them and then they can be executed.

Typical Commands
----------------
Below describes typical commands for #SNMP command line tools. For more
information on each tools, you may refer to the source code.

SNMPGET
^^^^^^^
For SNMP v1 and v2c, typical commands are

.. code-block:: shell

  snmpget -c=public -v=1 localhost 1.3.6.1.2.1.1.1.0
  snmpget -c=public -v=2 localhost 1.3.6.1.2.1.1.1.0

For SNMP v3, typical commands are

.. code-block:: shell

  snmpget -v=3 -l=noAuthNoPriv -u=neither localhost 1.3.6.1.2.1.1.1.0
  snmpget -v=3 -l=authNoPriv -a=MD5 -A=authentication -u=authen localhost 1.3.6.1.2.1.1.1.0
  snmpget -v=3 -l=authPriv -a=MD5 -A=authentication -x=DES -X=privacyphrase -u=privacy localhost 1.3.6.1.2.1.1.1.0

SNMPSET
^^^^^^^
For SNMP v1 and v2c, typical commands are

.. code-block:: shell

  snmpset -c=public -v=1 localhost 1.3.6.1.2.1.1.6.0 s Shanghai
  snmpset -c=public -v=2 localhost 1.3.6.1.2.1.1.6.0 s Shanghai

For SNMP v3, typical commands are

.. code-block:: shell

  snmpset -v=3 -l=noAuthNoPriv -u=neither localhost 1.3.6.1.2.1.1.6.0 s Shanghai
  snmpset -v=3 -l=authNoPriv -a=MD5 -A=authentication -u=authen localhost 1.3.6.1.2.1.1.6.0 s Shanghai
  snmpset -v=3 -l=authPriv -a=MD5 -A=authentication -x=DES -X=privacyphrase -u=privacy localhost 1.3.6.1.2.1.1.6.0 s Shanghai

SNMPBULKGET
^^^^^^^^^^^
For SNMP v2c, typical command is

.. code-block:: shell

  snmpbulkget -v=2 -c=public -Cr=10 localhost 1.3.6.1.2.1.1.1.0

For SNMP v3, typical commands are

.. code-block:: shell

  snmpbulkget -v=3 -l=noAuthNoPriv -u=neither -Cr=10 localhost 1.3.6.1.2.1.1.1.0
  snmpbulkget -v=3 -l=authNoPriv -a=MD5 -A=authentication -u=authen -Cr=10 localhost 1.3.6.1.2.1.1.1.0
  snmpbulkget -v=3 -l=authPriv -a=MD5 -A=authentication -x=DES -X=privacyphrase -u=privacy -Cr=10 localhost 1.3.6.1.2.1.1.1.0

SNMPGETNEXT
^^^^^^^^^^^
For SNMP v1 and v2c, typical commands are

.. code-block:: shell

  snmpgetnext -c=public -v=1 localhost 1.3.6.1.2.1.1.1.0
  snmpgetnext -c=public -v=2 localhost 1.3.6.1.2.1.1.1.0

For SNMP v3, typical commands are

.. code-block:: shell

  snmpgetnext -v=3 -l=noAuthNoPriv -u=neither localhost 1.3.6.1.2.1.1.1.0
  snmpgetnext -v=3 -l=authNoPriv -a=MD5 -A=authentication -u=authen localhost 1.3.6.1.2.1.1.1.0
  snmpgetnext -v=3 -l=authPriv -a=MD5 -A=authentication -x=DES -X=privacyphrase -u=privacy localhost 1.3.6.1.2.1.1.1.0

SNMPWALK
^^^^^^^^
For SNMP v1, typical command is

.. code-block:: shell

  snmpwalk -c=public -v=1 -m=subtree localhost 1.3.6.1.2.1.1

For SNMP v2c, typical command is

.. code-block:: shell

  snmpwalk -v=2 -c=public -Cr=10 -m=subtree localhost 1.3.6.1.2.1.1

For SNMP v3, typical commands are

.. code-block:: shell

  snmpwalk -v=3 -l=noAuthNoPriv -u=neither -m=subtree -Cr=10 localhost 1.3.6.1.2.1.1
  snmpwalk -v=3 -l=authNoPriv -a=MD5 -A=authentication -u=authen -m=subtree -Cr=10 localhost 1.3.6.1.2.1.1
  snmpwalk -v=3 -l=authPriv -a=MD5 -A=authentication -x=DES -X=privacyphrase -u=privacy -m=subtree -Cr=10 localhost 1.3.6.1.2.1.1

Built-in community names and users for snmpd
--------------------------------------------
Credentials to communicate with snmpd have been revised to match PySNMP, so you
can refer to `this article <https://docs.lextudio.com/snmp/snmp-simulation-service>`
for details.

Checkout
--------
The samples can be used to carry out basic SNMP operations. So if you are going
to learn the basics, you should follow them.

Pairing the SNMP test agent and the manager side tools
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Run snmpd.exe as administrator and click "Start listening" button without
modifying any settings. This allows the test SNMP agent to hook to port 161 on
all network interfaces (IP v4 and v6).

Information about the agent builtin community names and user accounts can be
found above in `Built-in community names and users for snmpd`_ .

Then the command line utilities can be run at command prompt with
`Typical Commands`_ . The agent will respond with correct packets.

Pairing the SNMP test agent and the trap listener tool
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Run snmptrapd.exe at command prompt as administrator. It will hook to port 162
and monitor incoming trap messages.

Click the "Sent Trap v1", "Send Trap v2", "Send Inform v2" and "Send Inform v3"
buttons on the test agent panel. See those messages are captured by the trap
listener tool.

Above setup assumes that all tools are running on the same machine. If you want
to test out agent and manager sides each on a dedicate machine, make sure you
open the firewall ports and allow SNMP packets to go through.

Related Resources
-----------------

- :doc:`/tutorials/introduction`
- :doc:`/tutorials/v3-operations`
- :doc:`/getting-started/license-notice`
