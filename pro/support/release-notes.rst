SharpSnmpPro.Mib Release Notes
==============================

By `Lex Li`_

This page documents major releases of SharpSnmpPro.Mib.

.. contents:: In this article:
  :local:
  :depth: 1

Releases
-------------------------

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
1.2.0   Jan ?, 2017       N/A
1.1.3   Oct 1, 2016       N/A
1.1.2   Sep 15, 2016      Oct 1, 2017
1.1.1   Jul 14, 2016      Sep 15, 2017
1.1.0   Feb 22, 2015      Jul 14, 2017
1.0.0   Feb 3, 2014       Feb 22, 2016
======= ================= ================

Related Resources
-----------------

- :doc:`/support/purchase`
- `API Documentation <https://help.sharpsnmp.com>`_
- `Requesting Trial <https://sharpsnmp.com/Home/Send>`_
- :doc:`/getting-started/compiler-features`
- :doc:`/getting-started/assembly-features`
