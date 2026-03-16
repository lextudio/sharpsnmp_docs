VarBindList Class
=================

.. dn:class:: DotNetSnmp.Asn1.SyntaxObjects.VarBindList

   Represents the VarBindList type.

   .. code-block:: csharp

      public class VarBindList : IAsnSerializable, IEnumerable<Variable>, IEnumerable

**Namespace:** ``DotNetSnmp.Asn1.SyntaxObjects``

**Inheritance:** Object → ``VarBindList``

**Source:** `SharpSnmpLib/Common/VarBindList.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/VarBindList.cs#L10>`__

Constructors
------------

VarBindList()
~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Asn1.SyntaxObjects.VarBindList..ctor

   Initializes a new instance of VarBindList.

   .. code-block:: csharp

      public VarBindList()

**Source:** `SharpSnmpLib/Common/VarBindList.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/VarBindList.cs#L25>`__

VarBindList(ObjectIdentifier[])
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Asn1.SyntaxObjects.VarBindList..ctor(DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier[])

   Initializes a new instance of VarBindList.

   .. code-block:: csharp

      public VarBindList(params ObjectIdentifier[] oids)

   :type oids: ``ObjectIdentifier[]``

**Source:** `SharpSnmpLib/Common/VarBindList.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/VarBindList.cs#L50>`__

VarBindList(String[])
~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Asn1.SyntaxObjects.VarBindList..ctor(System.String[])

   Initializes a new instance of VarBindList.

   .. code-block:: csharp

      public VarBindList(params string[] oids)

   :type oids: ``String[]``

**Source:** `SharpSnmpLib/Common/VarBindList.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/VarBindList.cs#L41>`__

VarBindList(VarBindList)
~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Asn1.SyntaxObjects.VarBindList..ctor(DotNetSnmp.Asn1.SyntaxObjects.VarBindList)

   Initializes a new instance of VarBindList.

   .. code-block:: csharp

      public VarBindList(VarBindList other)

   :type other: :dn:cls:`~DotNetSnmp.Asn1.SyntaxObjects.VarBindList`

**Source:** `SharpSnmpLib/Common/VarBindList.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/VarBindList.cs#L58>`__

VarBindList(Variable[])
~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: DotNetSnmp.Asn1.SyntaxObjects.VarBindList..ctor(DotNetSnmp.Asn1.SyntaxObjects.Variable[])

   Initializes a new instance of VarBindList.

   .. code-block:: csharp

      public VarBindList(params Variable[] bindings)

   :type bindings: ``Variable[]``

**Source:** `SharpSnmpLib/Common/VarBindList.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/VarBindList.cs#L33>`__

Properties
----------

IsEmpty
~~~~~~~

.. dn:property:: DotNetSnmp.Asn1.SyntaxObjects.VarBindList.IsEmpty

   Gets a value indicating whether this list has no variable bindings.

   .. code-block:: csharp

      public bool IsEmpty { get; }

   :rtype: ``Boolean``

**Source:** `SharpSnmpLib/Common/VarBindList.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/VarBindList.cs#L20>`__

Methods
-------

Add(Variable)
~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.VarBindList.Add(DotNetSnmp.Asn1.SyntaxObjects.Variable)

   Adds a variable binding to the end of the list.

   .. code-block:: csharp

      public VarBindList Add(Variable varBind)

   :type varBind: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.Variable`

   :rtype: :dn:cls:`~DotNetSnmp.Asn1.SyntaxObjects.VarBindList`

**Source:** `SharpSnmpLib/Common/VarBindList.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/VarBindList.cs#L66>`__

Clear()
~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.VarBindList.Clear

   Removes all variable bindings from the list.

   .. code-block:: csharp

      public void Clear()

**Source:** `SharpSnmpLib/Common/VarBindList.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/VarBindList.cs#L100>`__

GetEnumerator()
~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.VarBindList.GetEnumerator

   Gets enumerator.

   .. code-block:: csharp

      public IEnumerator<Variable> GetEnumerator()

   :rtype: ``IEnumerator<Variable>``

**Source:** `SharpSnmpLib/Common/VarBindList.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/VarBindList.cs#L257>`__

IEnumerable.GetEnumerator()
~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.VarBindList.System.Collections.IEnumerable.GetEnumerator

   .. code-block:: csharp

      IEnumerator IEnumerable.GetEnumerator()

   :rtype: ``IEnumerator``

**Source:** `SharpSnmpLib/Common/VarBindList.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/VarBindList.cs#L263>`__

Insert(Int32, Variable)
~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.VarBindList.Insert(System.Int32,DotNetSnmp.Asn1.SyntaxObjects.Variable)

   Inserts a variable binding at the specified index.

   .. code-block:: csharp

      public VarBindList Insert(int index, Variable varBind)

   :type index: ``Int32``
   :type varBind: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.Variable`

   :rtype: :dn:cls:`~DotNetSnmp.Asn1.SyntaxObjects.VarBindList`

**Source:** `SharpSnmpLib/Common/VarBindList.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/VarBindList.cs#L81>`__

ReadFrom(AsnReader)
~~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.VarBindList.ReadFrom(System.Formats.Asn1.AsnReader)

   Reads a value from an ASN.1 reader.

   .. code-block:: csharp

      public static VarBindList ReadFrom(AsnReader reader)

   :type reader: ``AsnReader``

   :rtype: :dn:cls:`~DotNetSnmp.Asn1.SyntaxObjects.VarBindList`

**Source:** `SharpSnmpLib/Common/VarBindList.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/VarBindList.cs#L126>`__

Remove(Int32)
~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.VarBindList.Remove(System.Int32)

   Removes and returns the variable binding at the specified index.

   .. code-block:: csharp

      public Variable Remove(int index)

   :type index: ``Int32``

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.Variable`

**Source:** `SharpSnmpLib/Common/VarBindList.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/VarBindList.cs#L90>`__

WriteTo(AsnWriter)
~~~~~~~~~~~~~~~~~~

.. dn:method:: DotNetSnmp.Asn1.SyntaxObjects.VarBindList.WriteTo(System.Formats.Asn1.AsnWriter)

   Writes this value to the supplied ASN.1 writer.

   .. code-block:: csharp

      public void WriteTo(AsnWriter writer)

   :param writer: The writer that receives the encoded value.
   :type writer: ``AsnWriter``

**Source:** `SharpSnmpLib/Common/VarBindList.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Common/VarBindList.cs#L106>`__

