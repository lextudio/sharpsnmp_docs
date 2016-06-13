#SNMP Compiler Pro Trial Version Reviewers' Guide
=================================================

By `Lex Li`_

This page shows you a guide on #SNMP Compiler Pro Trial version.

.. contents:: In this article:
  :local:
  :depth: 1

Background
----------
The Trial version can be requested `here <http://sharpsnmp.com/Home/Send>`_ , and is packaged up with #SNMP Library 8.5 and the latest SharpSnmpPro.Mib.

Evaluation Steps
----------------
To test it out, the default test MIB documents can be found at `GitHub <https://github.com/lextm/sharpsnmppro-mib>`_ . It can be cloned to a local folder, such as ``D:\sharpsnmppro-mib`` .

.. code-block:: shell

  git clone https://github.com/lextm/sharpsnmppro-mib.git

Then the documents can be copied to that folder (``D:\sharpsnmppro-mib`` for example).

Launch the compiler by executing ``Compiler.exe`` and then click File | Open menu item to navigate to ``D:\sharpsnmppro-mib`` folder in Open file dialog.

Change the file extension filter to All files (.), and then select all .txt files in this folder. Click Open button to open all files in the compiler. The file names should appear in Solution Explorer panel.

Click Build | Compile menu item to start compiling the files. In a few seconds, the Object Tree panel should be updated with objects extracted from the files, while Module List panel shows the loaded modules (as well as pending ones). 
The Error List panel should display any error or warnings. The Output panel contains the diagnostics logging entries.

Related Resources
-----------------

- :doc:`/support/purchase`
- `Requesting Trial <https://sharpsnmp.com/Home/Send>`_
- :doc:`/getting-started/compiler-features`
- :doc:`/tutorials/compiler-full-guide`
- :doc:`/tutorials/assembly-trial-guide`
- :doc:`/tutorials/assembly-full-guide`
