Information on DES/AES Privacy Providers
========================================

By `Lex Li`_

This page shows you information regarding DES/AES privacy providers.

.. contents:: In this article:
  :local:
  :depth: 1

Background
----------
SNMP v3 standard defines DES/AES algorithms to be used in user security model.
#SNMP Library 10.0 and above supports DES and AES 128/192/256.

However, some platforms do not have native DES/AES algorithms support, where
BouncyCastle can be used.

Built-in Providers on .NET Core
-------------------------------
Microsoft does have some DES/AES support in .NET Core. However,

* DES is not part of .NET Standard 1.3.
* SNMP AES relies on CFB mode, which is not supported by .NET Core.

Therefore, the built-in DES/AES privacy providers (derived from
``AESPrivacyProviderBase``) do not work well on .NET Core.

You can check ``DESPrivacyProvider.IsSupported`` to see if DES is natively
supported on a platform.

You can check ``AESPrivacyProviderBase.IsSupported`` to see if AES is natively
supported on a platform.

Providers on Bouncy Castle
--------------------------
Bouncy Castle is an open source library that implements many algorithms,
including DES and AES(CFB).

The sample projects show how to use ``Samples.BouncyCastle``(12.1 and above) or
``SharpSnmpLib.BouncyCastle``(10.0-12.0) to enable DES/AES privacy providers
based on Bouncy Castle. They can be used on platforms such as .NET Core.

.. note:: Compared to built-in providers, these are slower due to Bouncy Castle
   implementation. So such should only be used when necessary.

.. note:: AES privacy providers are available in 10.0.9 release.

.. note:: DES privacy provider is available for 10.0.10 release.

.. note:: Starting from 11.0.0 release, such extra providers are shipped in
   source code only, and as part of the samples repository.

The following code shows how to test native AES support, and choose the right
provider.

.. code-block:: csharp

    IPrivacyProvider aes;
    if (AESPrivacyProviderBase.IsSupported)
    {
        aes = new AESPrivacyProvider(...
    }
    else
    {
        aes = new BouncyCastleAESPrivacyProvider(...
    }

Similar code snippet can be used for DES,

.. code-block:: csharp

    IPrivacyProvider des;
    if (DESPrivacyProvider.IsSupported)
    {
        des = new DESPrivacyProvider(...
    }
    else
    {
        des = new BouncyCastleDESPrivacyProvider(...
    }

Related Resources
-----------------

- :doc:`/tutorials/introduction`
- :doc:`/samples/command-line-tools`
- :doc:`/tutorials/v3-operations`
- `The API Reference <https://help.sharpsnmp.com>`_
