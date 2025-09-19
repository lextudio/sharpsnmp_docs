MIB-to-C# Compilation
=====================

This page explains how to turn SNMP MIB documents into strongly-typed C# code
via a source generator. The generated code can then be consumed by any .NET
application that needs to model, expose, validate, or simulate SNMP objects.

Background
----------
Modern .NET SDKs support source generators, which can emit C# during the build
process. We leverage this to translate selected MIB documents into partial
classes and helper types. You can plug the output into many scenarios:

* Building a simulated SNMP agent (lab / demo environments)
* Creating conformance or regression test fixtures
* Generating strongly-typed wrappers for application logic (instead of manual OID handling)
* Producing training / educational samples
* Rapid prototyping before implementing full agent back ends

Throughout this article the C# SNMP Test Agent sample is referenced only as an
illustrative example of how to wire the generated files into a runnable host.
The same workflow applies to any project style that can compile C# source.

Use Cases
---------
The generator output is intentionally decoupled from any specific hosting
model. Typical integration patterns include:

* Console / service host that exposes an SNMP agent for lab simulation
* Unit / integration test projects that need stable OID-backed fixtures
* Middleware translating between SNMP operations and internal telemetry
* Educational samples demonstrating MIB structures in managed code
* Tooling that performs static analysis or validation against expected values
* Prototyping microservices that later evolve into production agents

If your scenario only needs to read or validate variable values (and not answer
GET / WALK requests), you can still reuse the type-safe representations without
hosting an SNMP engine.

How It Works
^^^^^^^^^^^^

The workflow below uses the sample repository purely as an example of project
layout; you can replicate the pattern in any solution:

- `C# SNMP Sample Agent <https://github.com/lextudio/sharpsnmplib-samples/tree/master/Samples/CSharpCore/snmpd>`_

In the example, three MIB documents are selected for generation:

* IP-MIB
* IF-MIB
* SNMPv2-MIB

Keep the original MIB documents in a dedicated `Mibs` (or similarly named)
folder, and specify which should be compiled via a `.mibs` manifest file:

- `Mibs/.mibs file <https://github.com/lextudio/sharpsnmplib-samples/blob/master/Samples/CSharpCore/snmpd/Mibs/.mibs>`_

The source generator automatically compiles all listed MIB documents.

.. note::
   
   Supporting files are configured as additional files in the project file:

   - `snmpd.csproj <https://github.com/lextudio/sharpsnmplib-samples/blob/master/Samples/CSharpCore/snmpd/snmpd.csproj>`_

For each MIB document in the `.mibs` file, by default two C# files are generated:
`.g.cs` and `.Generated.g.cs`.

.. note::

   You can review these files in Visual Studio to understand the generated code.

   In short, `.Generated.g.cs` contains the skeleton of the objects. Thus,
   there is never a need to modify `.Generated.g.cs` files.

   `.g.cs` includes the implementation of these objects, such as what data
   should be served to incoming SNMP requests.

If you only require the default (auto-generated) behavior, you can stop here.

Customization
^^^^^^^^^^^^^

When default values are insufficient (for simulation logic, validation rules,
stateful counters, or dynamic data retrieval), configure the generator to skip
its own `.g.cs` implementation for selected MIBs.

This is done using the `.customized` file:

- `Customized/.customized file <https://github.com/lextudio/sharpsnmplib-samples/blob/master/Samples/CSharpCore/snmpd/Customized/.customized>`_

For documents listed in `.customized`, you must provide corresponding `.g.cs`
files (for example under a `Customized` folder) so the build includes your
implementations instead of the default ones.

.. note::
   
   The generator still produces `.Generated.g.cs` files for all MIBs, including
   those listed in `.customized`. This ensures that all type definitions remain
   consistent, even when you provide custom implementations.

.. note::

   While you can handcraft your own `.g.cs` files, we recommend the following
   steps to get started quickly:

   1. Start by leaving the `.customized` file empty. This allows the source
      generator to create default `.g.cs` files for all MIB documents.
   2. Review the generated `.g.cs` files in Visual Studio and copy their contents
      aside if you wish to customize them.
   3. Once you have fully customized the files and include in your project, list
      the corresponding MIB document names in the `.customized` file.

   These steps easily use source generator to bootstrap your customization.

Limitations
-----------

* The generator focuses on structural translation (types, OIDs, basic value
  scaffolding). Advanced runtime semantics (persistence, real device state,
  security instrumentation) remain your responsibility.
* Generated code is intended as a starting point; review and adapt before
  production use.
* Performance characteristics depend on how customized files implement data
  retrieval and caching.
* Neither the sample host nor your generated classes are covered by break-fix
  support contracts; consulting services are available for tailored guidance.

Related Resources
-----------------

- :doc:`/support/purchase`
- `Requesting Trial <https://www.sharpsnmp.com/#contact-us>`_
- :doc:`/tutorials/assembly-trial-guide`
- :doc:`/tutorials/assembly-full-guide`
