Command Line Tools
==================
By `Lex Li`_

This page shows you what are the command line tools shipped.

.. contents:: In this article
   :local:
   :depth: 1

Typical Commands
----------------
Below describes typical commands for #SNMP command line tools. For more information on each tools, you may refer to the source code.

SNMPGET
^^^^^^^
For SNMP v1 and v2c, typical command is

.. code-block:: shell

  snmpget -v=1 -c=public localhost 1.3.6.1.2.1.1.1.0

For SNMP v3, typical command is

.. code-block:: shell

  snmpget -v=3 -l=authPriv -a=MD5 -A=authentication -x=DES -X=privacyphrase -u=privacy localhost 1.3.6.1.2.1.1.1.0

SNMPSET
^^^^^^^
For SNMP v1 and v2c, typical command is

.. code-block:: shell

  snmpset -v=1 -c=public localhost 1.3.6.1.2.1.1.6.0 s Shanghai

For SNMP v3, typical command is

.. code-block:: shell

  snmpset -v=3 -l=authPriv -a=MD5 -A=authentication -x=DES -X=privacyphrase -u=privacy localhost 1.3.6.1.2.1.1.1.0 s Shanghai

SNMPBULKGET
^^^^^^^^^^^
For SNMP v2c, typical command is

.. code-block:: shell

  snmpbulkget -v=2 -c=public -Cr=10 localhost 1.3.6.1.2.1.1.1.0

For SNMP v3, typical command is

.. code-block:: shell

  snmpbulkget -v=3 -l=authPriv -a=MD5 -A=authentication -x=DES -X=privacyphrase -u=privacy -Cr=10 localhost 1.3.6.1.2.1.1.1.0

SNMPGETNEXT
^^^^^^^^^^^
For SNMP v1 and v2c, typical command is

.. code-block:: shell

  snmpgetnext -v=1 -c=public localhost 1.3.6.1.2.1.1.1.0

For SNMP v3, typical command is

.. code-block:: shell

  snmpgetnext -v=3 -l=authPriv -a=MD5 -A=authentication -x=DES -X=privacyphrase -u=privacy localhost 1.3.6.1.2.1.1.1.0

SNMPWALK
^^^^^^^^
For SNMP v1, typical command is

.. code-block:: shell

  snmpwalk -v=1 -c=public -m=subtree localhost 1.3.6.1.2.1.1

For SNMP v2c, typical command is

.. code-block:: shell

  snmpwalk -v=2 -c=public -Cr=10 -m=subtree localhost 1.3.6.1.2.1.1

For SNMP v3, typical command is

.. code-block:: shell

  snmpwalk -v=3 -l=authPriv -a=MD5 -A=authentication -x=DES -X=privacyphrase -u=privacy -Cr=10 -m=subtree localhost 1.3.6.1.2.1.1

Built-in community names and users for snmpd
--------------------------------------------
SNMP v1 and v2c
^^^^^^^^^^^^^^^
==================  ==================
Get community name	Set community name
==================  ==================
public              public
==================  ==================

SNMP v3
^^^^^^^
Community names are obsolete in SNMP v3, so snmpd.exe supports three users (to match three modes).

=========  =============  =======================  =====================  ================  ==============
User name  Security mode  Authentication provider  Authentication phrase  Privacy provider  Privacy phrase
=========  =============  =======================  =====================  ================  ==============
neither	   noAuthNoPriv	  default                  N/A	                  default           N/A
authen	   authNoPriv     MD5                      authentication         default           N/A
privacy	   authPriv       MD5                      authentication	        DES               privacyphrase
=========  =============  =======================  =====================  ================  ==============

Checkout
--------
The samples can be used to carry out basic SNMP operations. So if you are going to learn the basics, you should follow them.

Pairing the SNMP test agent and the manager side tools
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Run snmpd.exe as administrator and click "Start listening" button without modifying any settings. This allows the test SNMP agent to hook to port 161 on all network interfaces (IP v4 and v6).

Information about the agent builtin community names and user accounts can be found above in `Built-in community names and users for snmpd`_ .

Then the command line utilities can be run at command prompt with `Typical Commands`_ . The agent will respond with correct packets.

Pairing the SNMP test agent and the trap listener tool
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Run snmptrapd.exe at command prompt as administrator. It will hook to port 162 and monitor incoming trap messages.

Click the "Sent Trap v1", "Send Trap v2", "Send Inform v2" and "Send Inform v3" buttons on the test agent panel. See those messages are captured by the trap listener tool.

Above setup assumes that all tools are running on the same machine. If you want to test out agent and manager sides each on a dedicate machine, make sure you open the firewall ports and allow 
SNMP packets to go through.

Related Resources
-----------------

- :doc:`/tutorials/introduction`
- :doc:`/tutorials/v3-operations`
