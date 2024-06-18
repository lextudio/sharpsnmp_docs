MIB-to-C# Compilation
=====================

This page shows you information about how to enable MIB-to-C# compilation.

Background
----------
#SNMP Library has a sample project that can work as a test agent. The agent can
be manually extended to support more management objects, but it is possible to
compile MIB documents to C# classes so as to simplify the process.

Evaluation Steps
----------------

Generating C# Source files
^^^^^^^^^^^^^^^^^^^^^^^^^^
To test it out with #SNMP MIB Compiler Pro, make sure that the menu item
"Generate C# source files from MIB documents" is checked on the tool bar. Then
C# source files will be generated when MIB documents are compiled, and saved to
a child folder called ``modules`` in the folder that contains ``Compiler.exe``.

To test out the same with SharpSnmpPro.Mib assembly,

#. Clone the extensions assembly from
   `GitHub <https://github.com/lextudio/sharpsnmppro.mib.extensions>`_ .
#. Replace the project reference to ``SharpSnmpPro.Mib`` with a NuGet package
   reference to ``SharpSnmpPro.Mib``.
#. Use ``ObjectTree.GenerateSourceFiles(string outputFolder)`` method to
   generate C# source files.

.. warning: This GitHub repo does not work with the Trial edition of `SharpSnmpPro.Mib`.

Extending Test Agent
^^^^^^^^^^^^^^^^^^^^
Once the source files are generated (in ``modules`` folder for example), a
C# project called ``Objects.csproj`` can be found in the same folder.

Open ``snmpd.csproj`` in #SNMP Library source code, and add a reference to this
new project, and the generated management objects can be added to the agent for
testing.

Limitations
-----------
This article is provided as it is, and the goal is to show what extra features
are possible to be implemented based on #SNMP Pro.

There is no break-fix support to use either the test agent or the generated C#
classes for production usage, but we sell consulting services if you need some
specific assistance with your project.

Related Resources
-----------------

- :doc:`/support/purchase`
- `Requesting Trial <https://www.sharpsnmp.com/#contact-us>`_
- :doc:`/getting-started/compiler-features`
- :doc:`/tutorials/compiler-full-guide`
- :doc:`/tutorials/assembly-trial-guide`
- :doc:`/tutorials/assembly-full-guide`
