OCTET STRING and Encoding
=========================

By `Lex Li`_

This page shows you how ``OCTET STRING`` type works internally.

.. contents:: In this article:
  :local:
  :depth: 1

Background
----------
If you notice, both SNMP data type ``OCTET STRING`` and ``Opaque`` can be
viewed as byte array type in .NET. Maybe you wonder why ``OCTET STRING`` is
not viewed as ``System.String``, the reason is simple. ``System.String`` does
have an important property that distinguishes itself from a byte array -
encoding. It seems when SNMP was designed, it does not provide a default
encoding for ``OCTET STRING`` explicitly (and sometimes it is even used just
like a byte array when you store MAC address bytes in it).

Therefore, a problem has been there for a long time, "which encoding should be
used there if an OctetString instance comes". In very old revision of #SNMP
Library, the answer was ASCII and there was no way in them to change it to
Unicode or any other encodings. Note that it is recommended you use ASCII if
possible.

In more recent builds of #SNMP Library you can explicitly state which encoding
you prefer.

Important Methods
-----------------
As a reference at first, there are new methods and properties in
``OctetString`` class you should pay attention to,

#. The overloading constructor
   ``public OctetString(string str, Encoding encoding)``. You may provide a
   specific ``Encoding`` so that the internal bytes are what you expect after
   initialization.
#. The overloading method ``public string ToString(Encoding encoding)``.
   According to ``Encoding`` provided, the internal bytes are decoded to a
   correct string.
#. The instance property ``public Encoding Encoding``. This is a read only
   property that illustrates what encoding is assigned to this ``OctetString``
   instance.
#. The static property ``public static Encoding DefaultEncoding``. This is a
   property to define default encoding used for all ``OctetString`` instance
   if no encoding is assigned via the constructor described in item 1. The
   default value of this property is ``Encoding.ASCII``.
#. The overloading constructor ``public OctetString(string str)``.
   ``OctetString.DefaultEncoding`` is used to generate internal bytes from
   ``str``.
#. The overloading method ``public string ToString()``.
   ``OctetString.Encoding`` is used to generate a string from internal bytes.

Scenarios
---------
Now let's review a few common scenarios and discuss what you may do to
customize ``OctetString``'s behaviors.

Default ASCII Way
^^^^^^^^^^^^^^^^^
If you don't touch the properties and methods related to ``Encoding``, then
you are in a pure ASCII way. It should behavior the same as old releases of
#SNMP (0.5, 1.0 and 1.1).

Default Encoding.* Way
^^^^^^^^^^^^^^^^^^^^^^
If you change ``DefaultEncoding`` to any other ``Encoding`` types, and don't
touch the properties and methods related to ``Encoding`` later, you are in a
pure ``Encoding.*`` way.

Basic Hybrid Way
^^^^^^^^^^^^^^^^
If some of your devices require ASCII while others require Unicode (aka
UTF-16), then you may find it a little bit difficult. My suggestions are,

Whenever you need to construct an ``OctetString`` object, specify its
encoding explicitly. Whenever you need to use an ``OctetString`` object, check
its ``Encoding`` before calling ``ToString()``. If the ``Encoding`` is not
correct, call ``ToString(Encoding)`` explicitly.

Last Words
----------
I understand the current implementation is not perfect yet. When #SNMP parses
incoming packets, it always use ``DefaultEncoding`` to construct
``OctetString`` objects from raw bytes. This is not optimal for hybrid cases.
Hope a better way can be found soon.

Related Resources
-----------------

- :doc:`/tutorials/introduction`
- `The API Reference <https://help.sharpsnmp.com>`_
