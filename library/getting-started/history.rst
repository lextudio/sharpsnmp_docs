History of C# SNMP Library
==========================

By `Lex Li`_

This article describes the history of C# SNMP (#SNMP) Library.

The Road to 1.0 Release
-----------------------
Microsoft introduced .NET Framework to developers in 2000. While this platform
has built-in support for many network protocols such as HTTP, FTP, and SMTP,
it lacks of SNMP protocol support. Many third party solutions were developed
to fill the gap, but most of them are commercial products.

Lex Li did an evaluation report of the existing libraries in 2008 for a 
project [1]_. He was quite satisfied with some of the commercial solutions, but
felt that there should be a need to have an open source implementation. Based
on the code base from Malcolm Crowe [2]_, Lex was able to start a new open
source project called C# SNMP Library [3]_ in April 2008 (#SNMP for short).

It was challenging a task to design an easy-to-use SNMP API, and also difficult
a mission to study the SNMP protocol details. Remember the facts that Lex just
graduated in 2007, and only had one year experience on programming professional
projects. But luckily all initial problems (such as message parsing) were
solved via experiments, and even features such as MIB parsing was developed in
a way [4]_ . By using TDD approach, every major features are covered by unit
test cases to ensure that regression bugs can be easily tracked down and fixed.

Near the final release of 1.0, two more products were added (the MIB browser
and MIB compiler), so the project was renamed to #SNMP Suite.

The 1.0 release (code name UnicornHorn) was finally released in July 2008 [5]_
, four months after the project launch. It features basic SNMP v1 and v2c
support.

SNMP v3 Support and Beyond
--------------------------
Steve Santacroce joined the project development in August 2008 [6]_ , and Lex
joined Microsoft in October 2008. The efforts required to drive #SNMP forward
were so overwhelming that Lex had to drop another open source project [7]_ .

The next major release of #SNMP Suite was 1.5 (code name TwinTower) in January
2009 [8]_ . It provides refined API surface, and many bugfixes over the initial
release. The 2.0 release (code name CrossRoad) was released in April 2009 [9]_,
which finished all tasks except SNMP v3 support.

SNMP v3 is a monster to conquer, because it introduced fundamental changes to
the message format (and different agent side behaviors). Thus, many API
elements have to be completely rewritten. But things became easier as another
open source SNMP implementation named SNMP#NET was published by Milan
Sinadinovic [10]_ . By reusing the encryption code, C# SNMP Library soon
started to support SNMP v3 packets. The 3.0 release (code name Trident) was
released in August 2009 with initial SNMP v3 support.

The next major task was to implement an SNMP agent that can process incoming
requests. Fortunately Lex was working on ASP.NET/IIS at Microsoft at that time,
so he reused many ideas he learned from ASP.NET request pipeline and designed
a similar pipeline for SNMP messages [11]_ . The 4.0 release (code name
SquareRoot) shipped the initial result in March 2010 with SNMP v1 and v2c
message support [12]_ . SNMP v3 message support only arrived in 5.0 release
(code name CatPaw) [13]_ in May 2010. Mono support was also included for the
first time as Lex revised DockPanel Suite [14]_ .

The 6.0 release (code name HoneyCell) in November 2010 was the first major
release that ships no big change [15]_ . #SNMP Suite had become more mature.

New Releases and License Changes
--------------------------------
The 7.0 release (code name BigDipper) was released in October 2011 [16]_ was
mainly a bug fix release.

The 8.0 release (code name TritonMate) was released in April 2013 [17]_ . It
featured a new compiler based on ANTLR [18]_ , which was under BSD 3 Clause.
This indicated a move to more permissive licenses. The SNMP pipeline code was
changed to MIT/X11 in the same release [19]_ . After the final release, the
code base had been updated to support Xamarin's mobile platforms.

A serious bug in SNMP v3 was found and fixed [20]_ so that affected releases
were updated with patches.

A significant license change was announced too, which released the Library code
under MIT/X11 [21]_, which means all source code then was released under
permissive licenses.

Following the license change, #SNMP Pro was announced, which forms a group of
commercial products from LeXtudio [22]_ . Many issues once reported to the open
source MIB compiler were finally fixed in the Pro edition by the new compiler
design.

The open source project was renamed back to C# SNMP Library. Its latest release
8.5 was published in February 2015 [23]_ . This release featured full support
for Windows, OS X, Linux, and Xamarin platforms.

The 9.x release in 2016 is code named LordGate [24]_ . This release was aiming
to complete async/await support and .NET Core support. The release cycle became
more flexible.

The 10.x release finally embraced .NET Standard support. It also completed AES
support (adding AES 192/256). To support platforms where native AES is missing,
a new ``SharpSnmpLib.BouncyCastle`` package is added.

The 11.x release separated the samples to a new repository and fixed a few long
standing issues.

The 12.x release revised supported platforms to better align with modern .NET.
It has been optimized to utilize new socket features introduced in .NET 6, and
also added type annotations to the code base.

The 13.x Era - Building on Recent .NET Modernization
----------------------------------------------------

In recent years, Microsoft invested heavily in modernizing the .NET runtime and standard
library. Key initiatives included the development of span-based APIs (``Span<T>``,
``ReadOnlySpan<T>``), the introduction of `System.Formats.Asn1
<https://learn.microsoft.com/en-us/dotnet/api/system.formats.asn1>`_ for binary protocol
parsing, the ``System.Threading.Channels`` API for high-performance async communication,
and numerous other improvements that benefit all networking stacks running on .NET, not
just web services like ASP.NET Core.

These investments opened opportunity for the SNMP ecosystem. The first major exploration
was the now-abandoned `DotNetSnmp <https://github.com/lextudio/DotNetSnmp>`_ project, which
demonstrated how to apply modern .NET patterns to SNMP protocol implementation. Building
on those lessons, C# SNMP Library v13 (started in 2024) adopts the same principles to bring
the main library into the modern .NET era.

The 13.x release represents a comprehensive redesign, replacing the custom ASN.1 parser
that had served the library since its 1.0 release (2008) with Microsoft's modern
``System.Formats.Asn1`` implementation. This change eliminated a significant burden of
maintenance while gaining the performance, memory efficiency, and maintainability benefits
of using span-based APIs and the latest language features.

Key improvements in v13:

- **System.Formats.Asn1**: Leverages Microsoft's modern, thoroughly-tested ASN.1 parser,
  introducing ``ReadOnlySpan<T>``, efficient buffer handling, and reduced allocations.
- **Modern .NET Only**: Targets .NET 8.0 and above (net8.0, net9.0, net10.0+), allowing
  full use of modern language features, runtime optimizations, and the latest LTS releases.
- **Performance**: Reduced memory pressure through span-based APIs and modern .NET primitives,
  enabling better scalability in high-throughput SNMP operations.
- **Improved Async Support**: Enhanced async/await patterns throughout the library, taking
  advantage of ``System.Threading.Channels`` and other modern async utilities.
- **SNMP over TCP**: Added support for SNMP over TCP, leveraging .NET's modern socket APIs for improved
  reliability and performance in environments to supplement traditional UDP transport.

This transformation ensures that C# SNMP Library remains aligned with modern .NET development
practices and empowered by the same infrastructure investments that benefit the broader
.NET ecosystem. It also sets the stage for continued innovation in SNMP protocol support
as Microsoft continues to evolve .NET.

For users upgrading from v12, refer to the :doc:`/tutorials/v13-migration` guide
for detailed migration instructions and best practices.

.. rubric:: Footnotes

.. [1] https://blog.lextudio.com/2007/12/product-review-snmp-libraries-for-net-evaluation-report/
.. [2] http://cis.uws.ac.uk/crow-ci0/
.. [3] https://sharpsnmplib.codeplex.com
.. [4] https://blog.lextudio.com/2008/05/snmp-design-build-my-own-lexer/
.. [5] https://blog.lextudio.com/2008/07/snmp-design-unicornhorn-and-known-issues/
.. [6] https://blog.lextudio.com/2008/08/snmp-design-joint-forces/
.. [7] https://blog.lextudio.com/2008/11/candycan-opener-bad-news-at-prime-time/
.. [8] https://blog.lextudio.com/2009/01/snmp-design-here-comes-1-5-final-release-twintower/
.. [9] https://blog.lextudio.com/2009/04/snmp-design-shipping-the-package-of-crossroad/
.. [10] https://blog.lextudio.com/2009/05/trident-sign-another-open-source-snmp-library-via-c/
.. [11] https://blog.lextudio.com/2010/11/honeycell-drops-snmp-pipeline-and-our-agent-demo/
.. [12] https://blog.lextudio.com/2010/03/squareroot-puzzle-4-0-final-kick-off/
.. [13] https://blog.lextudio.com/2010/05/catpaw-rumors-release-notes-for-5-0-release/
.. [14] https://blog.lextudio.com/2010/05/dockpanel-suite-tip-5-we-could-go-mono/
.. [15] https://blog.lextudio.com/2010/11/honeycell-drops-final-release-on-nov-12/
.. [16] https://blog.lextudio.com/2011/10/bigdipper-light-rtm-post/
.. [17] https://blog.lextudio.com/2013/04/tritonmate-words-8-0-release/
.. [18] https://blog.lextudio.com/2012/02/tritonmate-words-upcoming-change-to-sharpsnmplib-mib-dll-license/
.. [19] https://blog.lextudio.com/2012/04/tritonmate-words-license-change-on-snmp-engine-support/
.. [20] https://blog.lextudio.com/2012/12/tritonmate-words-story-on-rfc-3414-support/
.. [21] https://blog.lextudio.com/2013/01/tritonmate-words-important-change-on-snmp-library-license/
.. [22] https://blog.lextudio.com/2013/04/tritonmate-words-the-upcoming-snmp-pro-editions/
.. [23] https://blog.lextudio.com/2015/02/snmp-pro-release-1-1-is-out/
.. [24] https://blog.lextudio.com/2015/05/tritonmate-words-snmp-9-0-plan/
