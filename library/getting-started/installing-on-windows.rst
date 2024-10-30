Installing C# SNMP Library
==========================

By `Lex Li`_

This page shows you how to install C# SNMP Library to your project on Windows.
The usage on other platforms (macOS and Linux) should be quite similar.

.. contents:: In this article:
  :local:
  :depth: 1

Install C# SNMP Library via NuGet
---------------------------------

The easiest way to get started building applications with C# SNMP Library is to
install via NuGet in the latest version of Visual Studio 2015 (including the
free Community edition).

1. Install `Visual Studio 2015
   <https://go.microsoft.com/fwlink/?LinkId=532606>`_ or above.

   Be sure to specify that you include the Windows and Web Development.

2. Install latest `NuGet Package Manager
   <https://docs.nuget.org/consume/installing-nuget>`_.

   This will install the latest NuGet tooling.

3. Open/create an empty Windows Forms project.

4. Install C# SNMP Library NuGet packages following `NuGet conventions
   <https://docs.nuget.org/Consume/Package-Manager-Dialog>`_.

The latest package can be found at,

* `NuGet.org <https://www.nuget.org/packages/Lextm.SharpSnmpLib/>`_.

Install C# SNMP Library via source code
---------------------------------------

C# SNMP Library source code can be directly used in your project.

#. Download the source code from `GitHub
   <https://github.com/lextudio/sharpsnmplib/releases>`_, or clone the repo
   directly.
#. Open/create a empty Windows Forms project in a solution.
#. Add SharpSnmpLib.csproj in ``SharpSnmpLib`` directory to your
   solution.

Sample projects for C# SNMP Library are available in their own
`repo <https://github.com/lextudio/sharpsnmplib-samples>`_ .

Related Resources
-----------------

- :doc:`/tutorials/introduction`
- :doc:`/tutorials/v3-operations`
- :doc:`/samples/command-line-tools`
- :doc:`/samples/agent-development`
