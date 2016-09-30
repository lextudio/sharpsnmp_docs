Supported Platforms
===================

By `Lex Li`_

This page describes for major releases of #SNMP, which version(s) of .NET Framework and Mono are supported.

.. contents:: In this article:
  :local:
  :depth: 1

.NET Framework
--------------

.NET 1.0/.NET 1.1
^^^^^^^^^^^^^^^^^
These .NET Framework releases are end of life.

#SNMP does not support them.

.NET 2.0 RTM/.NET 2.0 SP1/.NET 2.0 SP2/.NET 3.0 RTM/.NET 3.0 SP1/.NET 3.0 SP2/.NET 3.5 RTM
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
These .NET Framework releases are end of life.

#SNMP does not support them.

.NET 3.5 SP1
^^^^^^^^^^^^
According to `Microsoft support policies <https://support.microsoft.com/en-us/lifecycle#gp/Framework_FAQ>`_ , this .NET Framework release is still supported.

`#SNMP 8.0 release (code name TritonMate) <https://sharpsnmplib.codeplex.com/releases/view/79079>`_ was the last release for this platform.

It is recommended to upgrade to .NET 4.5.2/.NET 4.6/.NET 4.6.1.

.NET 4/.NET 4.5/.NET 4.5.1
^^^^^^^^^^^^^^^^^^^^^^^^^^
These .NET Framework releases are end of life.

#SNMP does not support them.

.NET 4.5.2/.NET 4.6/.NET 4.6.1
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
According to `Microsoft support policies <https://support.microsoft.com/en-us/lifecycle#gp/Framework_FAQ>`_, these releases are still supported.

`#SNMP 8.5 release (code name TritonMate Refresh) <https://sharpsnmplib.codeplex.com/releases/view/118578>`_ and above can be used on these platforms.

.NET Compact Framework
----------------------
Support for .NET Compact Framework 3.5 and above is still experimental.

Mono
----
`#SNMP 8.5 release (code name TritonMate Refresh) <https://sharpsnmplib.codeplex.com/releases/view/118578>`_ and above can be used on Mono.

The following operating systems are tested,

* OS X
* Ubuntu
* Fedora Core

It is recommended to use latest Mono release, such as 4.2.1 and above.

.NET Core
---------
Microsoft has released .NET Core 1.0, but this new platform still lacks of certain APIs for this library to consume.

#SNMP will support this platform officially once it becomes more mature.
