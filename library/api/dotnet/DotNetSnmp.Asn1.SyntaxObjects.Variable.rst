Variable Struct
===============

.. dn:struct:: DotNetSnmp.Asn1.SyntaxObjects.Variable

   Represents the Variable type.

   .. code-block:: csharp

      public readonly record struct Variable : IAsnSerializable, IEquatable<Variable>

**Namespace:** ``DotNetSnmp.Asn1.SyntaxObjects``

**Source:** `SharpSnmpLib/Common/VarBind.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/VarBind.cs#L8>`__

Constructors
------------

Variable(String, IAsnSerializable?)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Asn1.SyntaxObjects.Variable..ctor(System.String,DotNetSnmp.Asn1.Serialization.IAsnSerializable)

   Initializes a new instance of Variable.

   .. code-block:: csharp

      public Variable(string oid, IAsnSerializable? value = null)

   :type oid: ``String``
   :type value: :dn:iface:`~DotNetSnmp.Asn1.Serialization.IAsnSerializable`

**Source:** `SharpSnmpLib/Common/VarBind.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/VarBind.cs#L23>`__

Properties
----------

Data
~~~~

.. dn:property:: DotNetSnmp.Asn1.SyntaxObjects.Variable.Data

   Gets data.

   .. code-block:: csharp

      public IAsnSerializable Data { get; }

   :rtype: :dn:iface:`~DotNetSnmp.Asn1.Serialization.IAsnSerializable`

**Source:** `SharpSnmpLib/Common/VarBind.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/VarBind.cs#L18>`__

Id
~~

.. dn:property:: DotNetSnmp.Asn1.SyntaxObjects.Variable.Id

   Gets id.

   .. code-block:: csharp

      public ObjectIdentifier Id { get; }

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`

**Source:** `SharpSnmpLib/Common/VarBind.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/VarBind.cs#L13>`__

Methods
-------

Deconstruct(out String, out Object)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.Variable.Deconstruct(System.String@,System.Object@)

   Deconstructs the value into its components.

   .. code-block:: csharp

      public readonly void Deconstruct(scoped out string name, scoped out object value)

   :type name: ``String``
   :type value: ``Object``

**Source:** `SharpSnmpLib/Common/VarBind.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/VarBind.cs#L50>`__

ToString()
~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.Variable.ToString

   Returns a string representation of the current value.

   .. code-block:: csharp

      public readonly override string ToString()

   :rtype: ``String``

**Source:** `SharpSnmpLib/Common/VarBind.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/VarBind.cs#L59>`__

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.Variable.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public readonly void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/Common/VarBind.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/VarBind.cs#L30>`__

Operators
---------

Explicit(String to Variable)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:operator:: DotNetSnmp.Asn1.SyntaxObjects.Variable.op_Explicit(System.String)

   Performs a conversion to Variable.

   .. code-block:: csharp

      public static explicit operator Variable(string oid)

   :type oid: ``String``

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.Variable`

**Source:** `SharpSnmpLib/Common/VarBind.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/VarBind.cs#L67>`__

