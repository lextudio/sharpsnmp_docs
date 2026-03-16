ErrorCategory Enum
==================

.. dn:enum:: Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory

   Error category.

   .. code-block:: csharp

      public enum ErrorCategory

**Namespace:** ``Lextm.SharpSnmpPro.Mib.Validation``

Fields
------

DescriptorCollision
~~~~~~~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory.DescriptorCollision

   Collision for imported descriptors.

   .. code-block:: csharp

      DescriptorCollision = 16

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory`

DuplicateEntities
~~~~~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory.DuplicateEntities

   Duplicate entity definitions are found.

   .. code-block:: csharp

      DuplicateEntities = 8

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory`

DuplicateModule
~~~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory.DuplicateModule

   Duplicate module.

   .. code-block:: csharp

      DuplicateModule = 14

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory`

DuplicateTypes
~~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory.DuplicateTypes

   Duplicate type definitions are found.

   .. code-block:: csharp

      DuplicateTypes = 7

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory`

ForbiddenImportedSymbol
~~~~~~~~~~~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory.ForbiddenImportedSymbol

   Symbols that are not allowed to import.

   .. code-block:: csharp

      ForbiddenImportedSymbol = 15

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory`

MissingDependency
~~~~~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory.MissingDependency

   A module cannot be imported.

   .. code-block:: csharp

      MissingDependency = 6

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory`

MissingEnterprise
~~~~~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory.MissingEnterprise

   Enterprise is missing for TRAP.

   .. code-block:: csharp

      MissingEnterprise = 10

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory`

MissingEntityType
~~~~~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory.MissingEntityType

   Entity type cannot be resolved.

   .. code-block:: csharp

      MissingEntityType = 4

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory`

MissingImportedSymbol
~~~~~~~~~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory.MissingImportedSymbol

   A symbol cannot be imported from module.

   .. code-block:: csharp

      MissingImportedSymbol = 2

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory`

MissingIndex
~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory.MissingIndex

   No index is found for table entry.

   .. code-block:: csharp

      MissingIndex = 9

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory`

MissingParent
~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory.MissingParent

   Parent node is missing.

   .. code-block:: csharp

      MissingParent = 3

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory`

MissingParentId
~~~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory.MissingParentId

   Parent OID is missing.

   .. code-block:: csharp

      MissingParentId = 13

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory`

MissingVariable
~~~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory.MissingVariable

   Variable is missing for TRAP.

   .. code-block:: csharp

      MissingVariable = 11

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory`

SematicError
~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory.SematicError

   Sematic error.

   .. code-block:: csharp

      SematicError = 1

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory`

TypeExpansionFailed
~~~~~~~~~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory.TypeExpansionFailed

   Error occurred during type expansion.

   .. code-block:: csharp

      TypeExpansionFailed = 5

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory`

WrongParent
~~~~~~~~~~~

.. dn:field:: Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory.WrongParent

   Table entry&apos;s parent is not a table.

   .. code-block:: csharp

      WrongParent = 12

   :rtype: :dn:enum:`~Lextm.SharpSnmpPro.Mib.Validation.ErrorCategory`

