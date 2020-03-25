SharpSnmpPro.Mib Assembly Trial Version Reviewers' Guide
========================================================

By `Lex Li`_

This page shows you a guide on SharpSnmpPro.Mib assembly trial version.

.. contents:: In this article:
  :local:
  :depth: 1

Background
----------
The Trial Edition can be requested `here <https://www.sharpsnmp.com/#contact-us>`_ , and is packaged up with the latest #SNMP Library. So below are the assemblies in the ZIP package,

* SharpSnmpPro.Mib.Trial.dll
* SharpSnmpLib.dll
* SharpSnmpPro.Mib.Trial.2.0.0.nupkg

.. note:: For 1.2 release, the following are included in the ZIP package,

  * SharpSnmpPro.Mib.Trial.dll
  * SharpSnmpLib.Full.dll
  * SharpSnmpLib.Portable.dll

Supported Platforms
-------------------
Unlike the Compiler Pro which requires .NET 4.5 and Windows, this assembly can be used on multiple platforms,

* .NET Framework 4.5.2 and above
* Mono 5.0 and above (via .NET Standard 2.0)
* Xamarin.iOS Unified (via .NET Standard 2.0)
* Xamarin.Android (via .NET Standard 2.0)
* Xamarin.Mac (via .NET Standard 2.0)

Evaluation Steps
----------------
To test it out, the default test projects can be found at `GitHub <https://github.com/lextm/lextudio/sharpsnmppro-samples.git>`_ . 
It can be cloned to a local folder, such as ``D:\lextudio\sharpsnmppro-samples`` .

.. code-block:: shell

  git clone https://github.com/lextm/lextudio/sharpsnmppro-samples.git
  git checkout release_2.0

.. note:: For 1.2 release, execute the following commands,

  .. code-block:: shell

    git clone https://github.com/lextm/lextudio/sharpsnmppro-samples.git
    git checkout release_1.2

Then extract all the files from the ZIP package to that folder (``D:\lextudio\sharpsnmppro-samples`` for example).

Lastly, execute an extra script to prepare the NuGet local feed,

  .. code-block:: shell

    install.nuget.bat

.. note:: For 1.2 release, there is no ``install.nuget.bat``.

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

#. Include a text file named ``sharpsnmppro.txt``.
#. The text file must contain exactly "#SNMP MIB Compiler Pro" (without quotes).
#. Build Action for this text file must be set as Embedded Resource.

Without this text file, the Trial Edition should give you an exception with error message "This assembly is not licensed to you. Please buy a license from LeXtudio...".

The API reference documentation can be found on `the help site <https://help.sharpsnmp.com>`_ .

Related Resources
-----------------

- :doc:`/support/purchase`
- `API Documentation <https://help.sharpsnmp.com>`_
- `Requesting Trial <https://www.sharpsnmp.com/#contact-us>`_
- :doc:`/getting-started/assembly-features`
- :doc:`/tutorials/assembly-full-guide`
- :doc:`/tutorials/compiler-trial-guide`
- :doc:`/tutorials/compiler-full-guide`
