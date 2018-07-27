Information on AES Privacy
==========================

By `Lex Li`_

This page shows you information regarding AES privacy providers.

.. contents:: In this article:
  :local:
  :depth: 1

Background
----------
SNMP v3 standard defines AES algorithms to be used in user security model.
#SNMP Library 10.0 supports AES 128/192/256.

However, there are platforms that do not have native AES algorithms support,
where an extra NuGet package is required.

Built-in Providers on .NET Core
-------------------------------
Microsoft does have some AES support in .NET Core. However, SNMP AES relies on
CFB mode, which is not supported by .NET Core.

Therefore, the built-in privacy providers (derived from
``AESPrivacyProviderBase`` do not work on .NET Core.

You can check ``AESPrivacyProviderBase.IsSupported`` to see if AES is natively
supported on a platform.

Providers on Bouncy Castle
--------------------------
Bouncy Castle is an open source library that implements many algorithms,
including AES CFB.

The NuGet package ``SharpSnmpLib.BouncyCastle`` ships AES privacy providers
which are based on Bouncy Castle. They can be used on .NET Core.

.. note:: Compared to built-in providers, these are slower due to Bouncy Castle
   implementation. So this extra package should only be used when necessary.

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

Related Resources
-----------------

- :doc:`/tutorials/introduction`
- :doc:`/samples/command-line-tools`
- :doc:`/tutorials/v3-operations`
- `The API Reference <http://help.sharpsnmp.com>`_
