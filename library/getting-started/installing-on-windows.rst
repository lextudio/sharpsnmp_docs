Installing #SNMP Library
========================

By `Lex Li`_

This page shows you how to install #SNMP Library to your project on Windows.
The usage on other platforms (macOS and Linux) should be quite similar.

.. contents:: In this article:
  :local:
  :depth: 1

Install #SNMP Library via NuGet
-------------------------------

The easiest way to get started building applications with #SNMP Library is to
install via NuGet in the latest version of Visual Studio 2015 (including the
free Community edition).

1. Install `Visual Studio 2015
   <https://go.microsoft.com/fwlink/?LinkId=532606>`_.

   Be sure to specify that you include the Windows and Web Development.

2. Install latest `NuGet Package Manager
   <https://docs.nuget.org/consume/installing-nuget>`_.

   This will install the latest NuGet tooling.

3. Open/create an empty Windows Forms project.

4. Install #SNMP Library NuGet packages following `NuGet conventions
   <https://docs.nuget.org/Consume/Package-Manager-Dialog>`_.

The latest package can be found at,

* `Main Library <https://www.nuget.org/packages/Lextm.SharpSnmpLib/>`_.
* `Platform Extensions
  <https://www.nuget.org/packages/Lextm.SharpSnmpLib.Extensions/>`_
  (Required by release 10.0.0. Not required by release 10.0.1 and above.)
* `DES/AES Privacy Providers via Bouncy Castle
  <https://www.nuget.org/packages/Lextm.SharpSnmpLib.BouncyCastle/>`_
  (Required by platforms without native DES/AES support, like .NET Core/UWP.
  Obsolete in 11.1.0 and above).

.. note:: In 10.0.0 release, the platform extensions package is required for
   .NET Framework, Xamarin.iOS, and Xamarin.Android applications so as to use
   DES/AES encryption. **This package is no longer needed in release 10.0.1 and
   above.**

.. note:: In 10.0.9 release, AES privacy providers based on Bouncy Castle are
   shipped in a new package for .NET Core/UWP scenarios. As Bouncy Castle AES
   algorithms are slower than native AES in general, **if you are targeting a
   platform with native AES support, such as .NET Framework/Mono/Xamarin, this
   package should not be used.**

.. note:: DES privacy provider based on Bouncy Castle would be available in
   10.0.10 release.

.. note:: Starting from 11.1.0 release, ``Lextm.SharpSnmpLib.BouncyCastle``
   package is obsolete, and no longer published. You can compile your own copy
   using the source code from `the samples <https://github.com/lextudio/sharpsnmplib-samples>`_ .

Install #SNMP Library via source code
-------------------------------------

#SNMP Library source code can be directly used in your project.

#. Download the source code from `GitHub
   <https://github.com/lextudio/sharpsnmplib/releases>`_, or clone the repo
   directly.
#. Run ``prepare.bat`` on Windows (or ``prepare.sh`` on non-Windows platforms)
   to prepare the code base for compilation.

   .. note:: This step is no longer needed in release 10.0.10 and above.

#. Open/create a empty Windows Forms project in a solution.

#. Add SharpSnmpLib.csproj (release 10.0 and above), and
   SharpSnmpLib.Full.csproj (10.0.0) in ``SharpSnmpLib`` directory to your
   solution.

.. note:: SharpSnmpLib.Android.csproj and SharpSnmpLib.iOS.csproj might be used
   to target Xamarin platforms for release 10.0.0. They are no longer needed
   for 10.0.1 release and above.

.. note:: Other projects (``SharpSnmpLib.BouncyCastle.csproj``) are optional.

Sample projects for #SNMP Library are available in their own
`repo <https://github.com/lextudio/sharpsnmplib-samples>`_ .

Related Resources
-----------------

- :doc:`/tutorials/introduction`
- :doc:`/tutorials/v3-operations`
- :doc:`/samples/command-line-tools`
- :doc:`/samples/agent-development`
