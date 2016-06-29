SharpSnmpPro.Mib Assembly Full Version Reviewers' Guide
=======================================================

By `Lex Li`_

This page shows you a guide on SharpSnmpPro.Mib assembly full version.

.. contents:: In this article:
  :local:
  :depth: 1

Background
----------
The Full version is sent to registered users only via emails, and is packaged up with latest #SNMP Library. So below are the assemblies in the ZIP package,

* SharpSnmpPro.Mib.dll
* SharpSnmpLib.Full.dll
* SharpSnmpLib.Portable.dll

Supported Platforms
-------------------
Unlike the Compiler Pro which requires .NET 4.5 and Windows, this assembly can be used on multiple platforms,

* .NET Framework 4.5.2 and above
* Mono 4.2.1 and above
* Xamarin.iOS Unified
* Xamarin.Android
* Xamarin.Mac

Complete Sample Project
-----------------------
You learn how SNMP operations can be done by consuming the open source SNMP API. A question then is what values MIB documents provide, as they are said to be an important part 
of SNMP protocol but not seem to be utilized anywhere if we solely use #SNMP Library.

Well, a rough answer is MIB documents mean everything,

* They tell what each object identifiers (OID) mean.
* They tell which OID is for a table, a row, and a column.
* They tell which kind of data we should expect for an object, ``OCTET STRING`` or any other valid types.

Thus, a MIB specific library such as SharpSnmpPro.Mib can help build a much more powerful SNMP manager.

.. image:: _static/mib.png

To test it out, we reuse the default test projects for Trial version, which can be found at `GitHub <https://github.com/lextm/sharpsnmppro-sample.git>`_. It can be cloned to a local folder, such as ``D:\sharpsnmppro-sample`` .

.. code-block:: shell

  git clone https://github.com/lextm/sharpsnmppro-sample.git
  git checkout release_1.1

Then the assemblies can be copied to that folder (``D:\sharpsnmppro-sample`` for example).

``Tests.csproj`` is an NUnit project that shows the below,

* How to compile and load MIB documents.
* How to query entity by name.
* How to check description of entities.
* How to verify data against entities. (note that the trial edition only support simple entities, while the full edition supports all entities).
* How to check OBJECT-TYPE macro specific properties.

To make the test project work with Full version, the following changes need to be made,

#. Remove the original reference to ``SharpSnmpPro.Mib.Trial.dll``.
#. Add a new reference to ``SharpSnmpPro.Mib.dll``.
#. Modify ``sharpsnmppro.txt`` following the instructions in the email.
#. Remove ``TRIAL`` from "Conditional compilation symbols", which then enables Full version only test cases.

Related Resources
-----------------

- :doc:`/support/purchase`
- `Requesting Trial <https://sharpsnmp.com/Home/Send>`_
- :doc:`/getting-started/assembly-features`
- :doc:`/tutorials/assembly-trial-guide`
- :doc:`/tutorials/compiler-trial-guide`
- :doc:`/tutorials/compiler-full-guide`
