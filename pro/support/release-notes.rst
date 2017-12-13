SharpSnmpPro.Mib Release Notes
==============================

By `Lex Li`_

This page documents major releases of SharpSnmpPro.Mib.

.. contents:: In this article:
  :local:
  :depth: 1

Releases
--------

2.0.0
^^^^^
This is a major release with new platform support. Major changes:

Bug fixes

* `Compiler performance and stability is improved <https://github.com/lextm/sharpsnmppro-sample/issues/15>`_ .

New Features

* `.NET Standard 2.0 support is added <https://github.com/lextm/sharpsnmppro-sample/issues/10>`_ .
* `RFC 2578 descriptor prefix is supported <https://github.com/lextm/sharpsnmppro-sample/issues/11>`_ .
* `RFC 2578 restriction on imported items is applied <https://github.com/lextm/sharpsnmppro-sample/issues/12>`_ .
* `RFC 1155 support is improved <https://github.com/lextm/sharpsnmppro-sample/issues/13>`_ .
* `Moved a few classes to new namespaces <https://github.com/lextm/sharpsnmppro-sample/issues/14>`_ .
* `Added overloading methods to ObjectRegistryBase support OID input <https://github.com/lextm/sharpsnmppro-sample/issues/16>`_ .

1.2.0
^^^^^
This is a bug fix release with some new APIs. Major changes:

Bug fixes

* `zeroDotZero DisplayEntity.GetObjectIdentifier is fixed <https://github.com/lextm/sharpsnmppro-sample/issues/5>`_ .
* `jmgt DisplayEntity.GetObjectIdentifier is fixed <https://github.com/lextm/sharpsnmppro-sample/issues/6>`_ .
* `Table index verification is improved to avoid false alarms <https://github.com/lextm/sharpsnmppro-sample/issues/7>`_ .
* `Special SMIv1 -> SMIv2 converted TRAP items are properly handled <https://github.com/lextm/sharpsnmppro-sample/issues/8>`_ .
* `OID resolution is revised to work better with multiple references to the same tree node <https://github.com/lextm/sharpsnmppro-sample/issues/9>`_ .

New features

* `A new Index type is added and implied flag is supported <https://github.com/lextm/sharpsnmppro-sample/issues/2>`_ .
* A new Augments type is added.
* New types such as ContraintedType are added to provide initial constraint related support.

Tutorials on the new features will be added to related sections.

.. note:: This release depends on `#SNMP Library 9.0.5 <https://github.com/lextm/sharpsnmplib/releases/tag/9.0.5>`_ and above.

1.1.3
^^^^^
This is a bug fix release. Major changes:

* `Parser2.Compile exceptions are handled properly. <https://github.com/lextm/sharpsnmppro-sample/issues/4>`_ 

1.1.2
^^^^^
This is a bug fix release. Major changes:

* `Assistance OIDs are no longer generated. <https://github.com/lextm/sharpsnmppro-sample/issues/1>`_ 
* `Duplicate module detection is added. <https://github.com/lextm/sharpsnmppro-sample/issues/3>`_ 

1.1.1
^^^^^
This is a bug fix release. Major changes:

* .NET Framework 4.0 is no longer supported. .NET 4.5 and above is required.

1.1.0
^^^^^
This is a bug fix release. Major change:

* More internal types are now exposed as public.

1.0.0
^^^^^
Initial release.

Product Lifecycle
-----------------
The lifecycle of the releases are listed below,

======= ================= ================
Version Release Date      End-of-life Date
======= ================= ================
2.0.0   Dec 31, 2017      N/A             
1.2.0   Jan 16, 2017      Mar 31, 2018    
1.1.3   Oct 1, 2016       Apr 16, 2017    
1.1.2   Sep 15, 2016      Oct 1, 2017     
1.1.1   Jul 14, 2016      Sep 15, 2017    
1.1.0   Feb 22, 2015      Jul 14, 2017    
1.0.0   Feb 3, 2014       Feb 22, 2016    
======= ================= ================

The old rule (1.0.0-1.1.2) is that any release will be actively supported till its next release becomes one year old.

The new rule (1.1.3 and above) is that any release will be actively supported till its next release becomes three months old. This change is to match our more frequent release cycles.

Users of expired releases must upgrade to an active supported release before contacing technical support team.

Related Resources
-----------------

- :doc:`/support/purchase`
- `API Documentation <https://help.sharpsnmp.com>`_
- `Requesting Trial <https://sharpsnmp.com/Home/Send>`_
- :doc:`/getting-started/compiler-features`
- :doc:`/getting-started/assembly-features`
