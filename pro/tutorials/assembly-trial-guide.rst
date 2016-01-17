SharpSnmpPro.Mib Assembly Trial Version Reviewers' Guide
========================================================

By `Lex Li`_

This page shows you a guide on SharpSnmpPro.Mib assembly trial version.

.. contents:: In this article:
  :local:
  :depth: 1

Background
----------
The Trial Edition can be requested `here <http://sharpsnmp.com/Home/Send>`_ , and is packaged up with #SNMP Library 8.5. So below are the assemblies in the ZIP package,

* SharpSnmpPro.Mib.Trial.dll
* SharpSnmpLib.Full.dll
* SharpSnmpLib.Portable.dll

Evaluation Steps
----------------
To test it out, the default test projects can be found at `GitHub <https://github.com/lextm/sharpsnmppro-sample.git>`_ . It can be cloned to a local folder, such as ``D:\sharpsnmppro-sample`` .

.. code-block:: shell

  git clone https://github.com/lextm/sharpsnmppro-sample.git

Then the assemblies can be copied to that folder (``D:\sharpsnmppro-sample`` for example).

In Visual Studio you can analyze the two projects in ``Tests.sln``.

``Tests.csproj`` is an NUnit project that shows the below,

* How to compile and load MIB documents.
* How to query entity by name.
* How to check description of entities.
* How to verify data against entities.
* How to check ``OBJECT-TYPE`` macro specific properties.

.. note:: The trial edition only support simple entities, while the full edition supports all entities.

``snmptranslate.csproj`` is a console application project that illustrates how to translate OIDs to strings (and vice versa) based on compiled MIB documents.

If new projects are going to be created to test out the Trial Edition, please note that you need to follow the provided samples to,

1. Include a text file named ``sharpsnmppro.txt``.
1. The text file must contain exactly "#SNMP MIB Compiler Pro" (without quotes).
1. Build Action for this text file must be set as Embedded Resource.

Without this text file, the Trial Edition should give you an exception with error message "This assembly is not licensed to you. Please buy a license from LeXtudio...".

The API reference documentation can be found on `the help site <http://help.sharpsnmp.com>`_ .

Related Resources
-----------------

- :doc:`/tutorials/assembly-full-guide`
