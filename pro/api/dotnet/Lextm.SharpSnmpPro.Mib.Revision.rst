Revision Class
==============

.. dn:class:: Lextm.SharpSnmpPro.Mib.Revision

   Used to store the source control system information.

   .. code-block:: csharp

      public class Revision

**Namespace:** ``Lextm.SharpSnmpPro.Mib``

**Inheritance:** Object → ``Revision``

Constructors
------------

Revision(IToken, String)
~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpPro.Mib.Revision..ctor(Antlr4.Runtime.IToken,System.String)

   Initializes a new instance of the :dn:cls:``~Lextm.SharpSnmpPro.Mib.Revision`` class.

   .. code-block:: csharp

      [CLSCompliant(false)]
      public Revision(IToken revision, string description)

   :param revision: The revision.
   :type revision: ``IToken``
   :param description: The description.
   :type description: ``String``

Properties
----------

Description
~~~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Revision.Description

   Revision description.

   .. code-block:: csharp

      public string Description { get; }

   :rtype: ``String``

Time
~~~~

.. dn:property:: Lextm.SharpSnmpPro.Mib.Revision.Time

   Revision time (expressed in UTC time).

   .. code-block:: csharp

      public DateTime Time { get; }

   :rtype: ``DateTime``

Methods
-------

Validate(ErrorRegistry, String)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpPro.Mib.Revision.Validate(Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry,System.String)

   Validates the format and content of a revision time string and updates the registry with warnings for any detected issues.

   .. code-block:: csharp

      public bool Validate(ErrorRegistry registry, string file)

   :param registry: The :dn:cls:``~Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry`` instance where validation warnings will be recorded.
   :type registry: :dn:cls:`~Lextm.SharpSnmpPro.Mib.Validation.ErrorRegistry`
   :param file: The name of the file associated with the revision time string, used for context in warnings.
   :type file: ``String``

   :returns: ``true`` if the revision time string is valid; otherwise, ``false``.
   :rtype: ``Boolean``

