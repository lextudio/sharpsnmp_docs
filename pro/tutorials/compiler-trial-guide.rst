#SNMP Compiler Pro Trial Version Reviewers' Guide
=================================================

This page shows you a guide on #SNMP Compiler Pro Trial version.

Background
----------
The Trial version can be requested `here <https://www.sharpsnmp.com/#contact-us>`_,
and is packaged up with the latest C# SNMP Library and SharpSnmpPro.Mib.

Evaluation Steps
----------------
To test it out, the default test MIB documents can be found at
`GitHub <https://github.com/lextm/sharpsnmppro-mib>`_ . It can be cloned to a
local folder, such as ``%temp%\sharpsnmppro-mib`` .

.. code-block:: shell

   cd %temp%
   git clone https://github.com/lextm/sharpsnmppro-mib.git

Then the documents can be copied to that folder (``%temp%\sharpsnmppro-mib`` for
example).

Launch the compiler by executing ``Compiler.exe`` and then click
:menuselection:`File --> Open` menu item to navigate to ``%temp%\sharpsnmppro-mib``
folder in Open file dialog.

Change the file extension filter to All files (.), and then select all .txt
files in this folder. Click Open button to open all files in the compiler. The
file names should appear in Solution Explorer panel.

Click Build | Compile menu item to start compiling the files. In a few seconds,
the Object Tree panel should be updated with objects extracted from the files,
while Module List panel shows the loaded modules (as well as pending ones).

The Error List panel should display any error or warnings. The Output panel
contains the diagnostics logging entries.

.. note:: There is a button on the tool bar to control C# code generation.

   If this button is checked, then when ``Compiler.exe`` compiles MIB
   documents, its working directory will add a new folder ``modules`` which
   contains the generated source files.

   To learn the usage of generated files, please refer to
   :doc:`/tutorials/mib2csharp`.

Related Resources
-----------------

- :doc:`/support/purchase`
- `Requesting Trial <https://www.sharpsnmp.com/#contact-us>`_
- :doc:`/getting-started/compiler-features`
- :doc:`/tutorials/compiler-full-guide`
- :doc:`/tutorials/assembly-trial-guide`
- :doc:`/tutorials/assembly-full-guide`
