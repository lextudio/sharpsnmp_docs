ClassNumber Class
=================

.. dn:class:: Lextm.SharpSnmpPro.Mib.ClassNumber

   Represents a class number, which may be constructed from a string or a :dn:cls:``~Lextm.SharpSnmpPro.Mib.DefinedValue``.

   .. code-block:: csharp

      public class ClassNumber

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``ClassNumber``

Constructors
------------

ClassNumber(DefinedValue)
~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.ClassNumber..ctor(Lextm.SharpSnmpPro.Mib.DefinedValue)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.ClassNumber`` class from a :dn:cls:``~Lextm.SharpSnmpPro.Mib.DefinedValue``.

   .. code-block:: csharp

      public ClassNumber(DefinedValue definedValue)

   :param definedValue: The :dn:cls:``~Lextm.SharpSnmpPro.Mib.DefinedValue`` to use for initialization.
   :type definedValue: :dn:cls:`~Lextm.SharpSnmpPro.Mib.DefinedValue`

ClassNumber(String)
~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.ClassNumber..ctor(System.String)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.ClassNumber`` class with the specified text.

   .. code-block:: csharp

      public ClassNumber(string text)

   :param text: The text representation of the class number.
   :type text: ``String``

Properties
----------

Module
~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ClassNumber.Module

   Gets the module associated with the class number.

   .. code-block:: csharp

      public string Module { get; }

   :rtype: ``String``

Text
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.ClassNumber.Text

   Gets or sets the text representation of the class number.

   .. code-block:: csharp

      public string Text { get; set; }

   :rtype: ``String``

