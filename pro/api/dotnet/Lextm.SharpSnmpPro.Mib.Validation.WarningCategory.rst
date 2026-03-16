WarningCategory Enum
====================

.. dn:enum:: Lextm.SharpSnmpPro.Mib.Validation.WarningCategory

   Warning category.

   .. code-block:: csharp

      public enum WarningCategory

**Namespace:** ``Lextm.SharpSnmpPro.Mib.Validation``

Fields
------

DuplicateEntity
~~~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.WarningCategory.DuplicateEntity

   Duplicate entities are detected.

   .. code-block:: csharp

      DuplicateEntity = 22

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.WarningCategory`

DuplicateModule
~~~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.WarningCategory.DuplicateModule

   Duplicate module is detected.

   .. code-block:: csharp

      [Obsolete("Promoted to error category.")]
      DuplicateModule = 2

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.WarningCategory`

IgnoredEntity
~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.WarningCategory.IgnoredEntity

   An entity is ignored.

   .. code-block:: csharp

      IgnoredEntity = 21

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.WarningCategory`

ImplicitNodeCreation
~~~~~~~~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.WarningCategory.ImplicitNodeCreation

   A node is created implicitly.

   .. code-block:: csharp

      ImplicitNodeCreation = 3

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.WarningCategory`

Obsolete
~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.WarningCategory.Obsolete

   The syntax is obsolete.

   .. code-block:: csharp

      Obsolete = 1

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.WarningCategory`

SematicError
~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.WarningCategory.SematicError

   SMI minor issues. Usually there is a better way to author this element.

   .. code-block:: csharp

      SematicError = 24

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.WarningCategory`

WrongBitName
~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.WarningCategory.WrongBitName

   Bit name should be fixed.

   .. code-block:: csharp

      WrongBitName = 18

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.WarningCategory`

WrongCamelCase
~~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.WarningCategory.WrongCamelCase

   Camel case should be used.

   .. code-block:: csharp

      WrongCamelCase = 19

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.WarningCategory`

WrongChoiceName
~~~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.WarningCategory.WrongChoiceName

   Choice name should be fixed.

   .. code-block:: csharp

      WrongChoiceName = 17

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.WarningCategory`

WrongConstraintName
~~~~~~~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.WarningCategory.WrongConstraintName

   Constraint name should be fixed.

   .. code-block:: csharp

      WrongConstraintName = 16

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.WarningCategory`

WrongEntryName
~~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.WarningCategory.WrongEntryName

   Entry name should be fixed.

   .. code-block:: csharp

      WrongEntryName = 10

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.WarningCategory`

WrongIdentifierName
~~~~~~~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.WarningCategory.WrongIdentifierName

   Identifier name should be fixed.

   .. code-block:: csharp

      WrongIdentifierName = 15

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.WarningCategory`

WrongImpliedIndex
~~~~~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.WarningCategory.WrongImpliedIndex

   The IMPLIED modifier found on wrong item.

   .. code-block:: csharp

      WrongImpliedIndex = 25

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.WarningCategory`

WrongIndexType
~~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.WarningCategory.WrongIndexType

   Index type syntax is not typical.

   .. code-block:: csharp

      WrongIndexType = 26

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.WarningCategory`

WrongMacroName
~~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.WarningCategory.WrongMacroName

   Macro name should be fixed.

   .. code-block:: csharp

      WrongMacroName = 12

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.WarningCategory`

WrongModuleName
~~~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.WarningCategory.WrongModuleName

   Module name should be fixed.

   .. code-block:: csharp

      WrongModuleName = 5

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.WarningCategory`

WrongNumberName
~~~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.WarningCategory.WrongNumberName

   Number name should be fixed.

   .. code-block:: csharp

      WrongNumberName = 14

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.WarningCategory`

WrongObjectName
~~~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.WarningCategory.WrongObjectName

   Object name should be fixed.

   .. code-block:: csharp

      WrongObjectName = 13

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.WarningCategory`

WrongPascelCase
~~~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.WarningCategory.WrongPascelCase

   Pascal case should be used.

   .. code-block:: csharp

      WrongPascelCase = 20

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.WarningCategory`

WrongRevision
~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.WarningCategory.WrongRevision

   Revision time string should be of standard format.

   .. code-block:: csharp

      WrongRevision = 23

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.WarningCategory`

WrongTableName
~~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.WarningCategory.WrongTableName

   Table name should be fixed.

   .. code-block:: csharp

      WrongTableName = 9

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.WarningCategory`

WrongTypeName
~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.WarningCategory.WrongTypeName

   Type name should be fixed.

   .. code-block:: csharp

      WrongTypeName = 11

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.WarningCategory`

