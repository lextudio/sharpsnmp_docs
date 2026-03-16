ObjectIdentifier Struct
=======================

.. dn:struct:: DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier

   Represents the ObjectIdentifier type.

   .. code-block:: csharp

      public readonly record struct ObjectIdentifier(string Oid) : IAsnSerializable, IComparable<ObjectIdentifier>, IComparable, IEquatable<ObjectIdentifier>

**Namespace:** ``DotNetSnmp.Asn1.SyntaxObjects``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/ObjectIdentifier.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/ObjectIdentifier.cs#L9>`__

Constructors
------------

ObjectIdentifier(Byte[])
~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier..ctor(System.Byte[])

   Initializes a new instance of ObjectIdentifier.

   .. code-block:: csharp

      public ObjectIdentifier(params byte[] octets)

   :type octets: ``Byte[]``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/ObjectIdentifier.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/ObjectIdentifier.cs#L23>`__

ObjectIdentifier(String)
~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier..ctor(System.String)

   Represents the ObjectIdentifier type.

   .. code-block:: csharp

      public ObjectIdentifier(string Oid)

   :type Oid: ``String``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/ObjectIdentifier.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/ObjectIdentifier.cs#L9>`__

ObjectIdentifier(UInt32[])
~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier..ctor(System.UInt32[])

   Initializes a new instance of ObjectIdentifier.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public ObjectIdentifier(uint[] ids)

   :type ids: ``UInt32[]``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/ObjectIdentifier.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/ObjectIdentifier.cs#L14>`__

Properties
----------

Oid
~~~

.. dn:property:: DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier.Oid

   .. code-block:: csharp

      public string Oid { get; init; }

   :rtype: ``String``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/ObjectIdentifier.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/ObjectIdentifier.cs#L9>`__

Methods
-------

CompareTo(Object?)
~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier.CompareTo(System.Object)

   .. code-block:: csharp

      public readonly int CompareTo(object? obj)

   :type obj: ``Object``

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/ObjectIdentifier.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/ObjectIdentifier.cs#L79>`__

CompareTo(ObjectIdentifier)
~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier.CompareTo(DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier)

   Compares two object identifiers lexicographically by OID segments.

   .. code-block:: csharp

      public readonly int CompareTo(ObjectIdentifier other)

   :type other: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/ObjectIdentifier.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/ObjectIdentifier.cs#L51>`__

ReadFrom(AsnReader)
~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier.ReadFrom(System.Formats.Asn1.AsnReader)

   Reads a value from an ASN.1 reader.

   .. code-block:: csharp

      public static ObjectIdentifier ReadFrom(AsnReader reader)

   :type reader: ``AsnReader``

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/ObjectIdentifier.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/ObjectIdentifier.cs#L37>`__

ToString()
~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier.ToString

   Returns a string representation of the current value.

   .. code-block:: csharp

      public readonly override string ToString()

   :rtype: ``String``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/ObjectIdentifier.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/ObjectIdentifier.cs#L46>`__

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public readonly void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/ObjectIdentifier.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/ObjectIdentifier.cs#L29>`__

Operators
---------

Explicit(Byte[] to ObjectIdentifier)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:operator:: DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier.op_Explicit(System.Byte[])

   Performs a conversion to ObjectIdentifier.

   .. code-block:: csharp

      public static explicit operator ObjectIdentifier(byte[] octets)

   :type octets: ``Byte[]``

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/ObjectIdentifier.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/ObjectIdentifier.cs#L102>`__

Explicit(String to ObjectIdentifier)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:operator:: DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier.op_Explicit(System.String)

   Performs a conversion to ObjectIdentifier.

   .. code-block:: csharp

      public static explicit operator ObjectIdentifier(string oid)

   :type oid: ``String``

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/ObjectIdentifier.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/ObjectIdentifier.cs#L97>`__

GreaterThan(ObjectIdentifier, ObjectIdentifier)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:operator:: DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier.op_GreaterThan(DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier)

   Compares whether left is greater than right.

   .. code-block:: csharp

      public static bool operator>(ObjectIdentifier left, ObjectIdentifier right)

   :type left: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type right: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`

   :rtype: ``Boolean``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/ObjectIdentifier.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/ObjectIdentifier.cs#L107>`__

GreaterThanOrEqual(ObjectIdentifier, ObjectIdentifier)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:operator:: DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier.op_GreaterThanOrEqual(DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier)

   Compares whether left is greater than or equal to right.

   .. code-block:: csharp

      public static bool operator >=(ObjectIdentifier left, ObjectIdentifier right)

   :type left: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type right: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`

   :rtype: ``Boolean``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/ObjectIdentifier.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/ObjectIdentifier.cs#L117>`__

Implicit(ObjectIdentifier to String)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:operator:: DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier.op_Implicit(DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier)

   Performs a conversion to string.

   .. code-block:: csharp

      public static implicit operator string (ObjectIdentifier o)

   :type o: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`

   :rtype: ``String``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/ObjectIdentifier.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/ObjectIdentifier.cs#L92>`__

LessThan(ObjectIdentifier, ObjectIdentifier)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:operator:: DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier.op_LessThan(DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier)

   Compares whether left is less than right.

   .. code-block:: csharp

      public static bool operator <(ObjectIdentifier left, ObjectIdentifier right)

   :type left: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type right: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`

   :rtype: ``Boolean``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/ObjectIdentifier.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/ObjectIdentifier.cs#L112>`__

LessThanOrEqual(ObjectIdentifier, ObjectIdentifier)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:operator:: DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier.op_LessThanOrEqual(DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier)

   Compares whether left is less than or equal to right.

   .. code-block:: csharp

      public static bool operator <=(ObjectIdentifier left, ObjectIdentifier right)

   :type left: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type right: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`

   :rtype: ``Boolean``

**Source:** `SharpSnmpLib/Asn1/SyntaxObjects/ObjectIdentifier.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Asn1/SyntaxObjects/ObjectIdentifier.cs#L122>`__

Extension Methods
-----------------

- :dn:meth:`GetErrorMessage <Lextm.SharpSnmpLib.Messaging.Messenger.GetErrorMessage>`

