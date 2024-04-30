Security Notice
===============

This page shows you information about security notices.

Overview
--------
Recent changes in security related areas make many SNMP building blocks deprecated. For example, MD5 and SHA-1 have been widely considered obsolete due to possible colisions. DES/3DES are in a similar case.

So to configure your SNMP agents and remedy security risks, it is recommended to choose authentication/privacy providers that use more modern algorithms, such as SHA-2 and AES.

Built-in Providers
------------------
#SNMP Library built-in providers are,

==============================  ====================
Authentication Providers    
==============================  ====================
`MD5AuthenticationProvider`     Obsolete
`SHA1AuthenticationProvider`    Obsolete
`SHA256AuthenticationProvider`
`SHA384AuthenticationProvider`
`SHA512AuthenticationProvider`
==============================  ====================

==============================  ====================
Privacy Providers    
==============================  ====================
`DESPrivacyProvider`            Obsolete
`TripleDESPrivacyProvider`      Obsolete
`AESPrivacyProvider`
`AES192PrivacyProvider`
`AES256PrivacyProvider`
==============================  ====================

Related Resources
-----------------

- :doc:`/tutorials/aes`
- :doc:`/tutorials/v3-operations`
- `The API Reference <https://help.sharpsnmp.com>`_
