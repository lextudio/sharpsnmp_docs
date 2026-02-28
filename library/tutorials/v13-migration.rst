Upgrading to C# SNMP v13
=========================

By `Lex Li`_

This guide helps you upgrade from C# SNMP v12 to v13, highlighting key changes and providing
step-by-step instructions for a smooth migration.

What's New in v13
-----------------

C# SNMP v13 represents a major modernization of the library, built on `System.Formats.Asn1
<https://learn.microsoft.com/en-us/dotnet/api/system.formats.asn1>`_ and targeting
modern .NET versions (8.0 and above).

Key improvements:

- **System.Formats.Asn1**: Replaced custom ASN.1 implementation with Microsoft's modern, 
  performant parser.
- **Modern .NET Only**: Targets .NET 8+, allowing use of the latest language features and 
  runtime optimizations.
- **Performance**: Reduced memory allocations and improved async/await handling.
- **Refined Security**: Updated security provider architecture for auth and privacy operations.

Before You Start
----------------

Before upgrading, ensure:

- Your project targets **.NET 8.0 or later** (v12 supported older frameworks; v13 does not).
- You have reviewed the :doc:`/getting-started/platforms` page.
- You have backed up your code or are using version control.

Breaking Changes Summary
------------------------

*To be populated with high-level summary of breaking changes.*

Step-by-Step Migration
----------------------

1. Update NuGet Package Reference
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Replace your v12 package reference with v13:

.. code-block:: bash

   # Via NuGet Package Manager (Visual Studio)
   Install-Package Lextm.SharpSnmpLib -Version 13.0.0-beta.2

   # Or via .NET CLI
   dotnet add package Lextm.SharpSnmpLib --version 13.0.0-beta.2

2. Update Namespace Imports
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

*To be populated with namespace changes, if any.*

3. Verify Target Framework
^^^^^^^^^^^^^^^^^^^^^^^^^^^

Ensure your project file specifies a supported framework:

.. code-block:: xml

   <TargetFramework>net8.0</TargetFramework>
   <!-- or -->
   <TargetFramework>net9.0</TargetFramework>
   <!-- or -->
   <TargetFramework>net10.0</TargetFramework>

4. Update API Calls
^^^^^^^^^^^^^^^^^^^

*To be populated with common API migration examples.*

5. Test Security Operations
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

If your application uses SNMP v3 with authentication or privacy:

*To be populated with testing guidance for auth/privacy operations.*

Migration by Scenario
---------------------

SNMP v1 Operations
^^^^^^^^^^^^^^^^^^

*To be populated with v1-specific migration guidance.*

SNMP v2c Operations
^^^^^^^^^^^^^^^^^^^^

*To be populated with v2c-specific migration guidance.*

SNMP v3 Operations (Auth/Privacy)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

*To be populated with v3-specific migration guidance and security provider updates.*

Common Errors and Solutions
----------------------------

*To be populated with common migration errors and troubleshooting steps.*

Performance Considerations
---------------------------

v13 is generally more performant than v12 due to:

- More efficient ASN.1 parsing via System.Formats.Asn1
- Better memory allocation patterns
- Improved async/await handling

For detailed performance comparisons, see the
`performance documentation <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/docs/performance.md>`_.

Testing After Upgrade
---------------------

After upgrading, test:

- Basic Get/Set operations against your SNMP devices
- Walk and BulkWalk operations
- v3 authentication and privacy (if used)
- Any custom middleware or security providers

Getting Help
------------

If you encounter issues:

1. Check the `incompatibility tracker <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/docs/incompatibility.md>`_
2. Search or file an issue on `GitHub <https://github.com/lextudio/sharpsnmplib/issues>`_
3. Consult the :doc:`/tutorials/index` for usage examples

Related Resources
-----------------

- :doc:`/getting-started/history`
- :doc:`/getting-started/platforms`
- :doc:`/support/release-notes`
- `Release Notes on GitHub <https://github.com/lextudio/sharpsnmplib/releases>`_
