Signature of Binaries
=====================

By `Lex Li`_

This article describes how to verify that you are using official releases of
#SNMP.

.. contents:: In this article:
  :local:
  :depth: 1

Release 10.0.10 and Above
-------------------------

Both the NuGet packages and assemblies inside would be signed using Lex Li's
personal code sign certificate, so digitial signature is embedded.

You can use ``signtool`` and NuGet CLI to verify the signature. For example,

.. code-block:: text

    signtool verify /pa /q SharpSnmpLib.dll
    nuget verify -All Lextm.SharpSnmpLib.nupkg

The certificate was issued by DigiCert, and its serial number is
``‎04 d8 f7 b9 b4 ba 0c 54 4b b4 8b 87 1c 3b 1c 26``, and its thumbprint is
``‎46 b0 b0 1a be ec 5a 04 1c a8 6e 6b 28 8a 86 6b c7 34 9e ad``.

Release 10.0.9 and Below
------------------------

As the files have no digital signature, you can only verify the strong names.

The assemblies were signed by a private key, and their ``PublicKeyToken``
should be ``4c00852d3788e005``. For example,

.. code-block:: text

   SharpSnmpLib, Version=10.0.3.0, Culture=neutral,
   PublicKeyToken=4c00852d3788e005

Related Resources
-----------------

- :doc:`/getting-started/installing-on-windows`
