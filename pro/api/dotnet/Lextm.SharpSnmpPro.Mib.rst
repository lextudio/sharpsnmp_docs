Lextm.SharpSnmpPro.Mib Namespace
================================

.. dn:namespace:: Lextm.SharpSnmpPro.Mib

Classes
-------

.. list-table::
   :header-rows: 1
   :widths: 30 70

   * - Type
     - Description
   * - :doc:`AgentCapabilitiesMacro <Lextm.SharpSnmpPro.Mib.AgentCapabilitiesMacro>`
     - Represents an AGENT-CAPABILITIES macro in a MIB module.
   * - :doc:`AgentCapabilitiesModule <Lextm.SharpSnmpPro.Mib.AgentCapabilitiesModule>`
     - Represents an agent capabilities module in an SNMP MIB.
   * - :doc:`AllExceptConstraintElement <Lextm.SharpSnmpPro.Mib.AllExceptConstraintElement>`
     - Represents a constraint element that matches all values except those specified by the given constraint.
   * - :doc:`AnyType <Lextm.SharpSnmpPro.Mib.AnyType>`
     - Represents a generic type in the MIB module.
   * - :doc:`Augments <Lextm.SharpSnmpPro.Mib.Augments>`
     - Represents the AUGMENTS clause in the MIB module, which specifies the augmentation of a table.
   * - :doc:`BitStringType <Lextm.SharpSnmpPro.Mib.BitStringType>`
     - Represents a BIT STRING type in SMI (Structure of Management Information).
   * - :doc:`BitsType <Lextm.SharpSnmpPro.Mib.BitsType>`
     - Represents a BITS type in SMI, which is a derived type with named bits.
   * - :doc:`Categories <Lextm.SharpSnmpPro.Mib.Categories>`
     - Represents a set of SNMP MIB categories.
   * - :doc:`CharacterStringType <Lextm.SharpSnmpPro.Mib.CharacterStringType>`
     - Represents a character string SMI type.
   * - :doc:`CharDefinition <Lextm.SharpSnmpPro.Mib.CharDefinition>`
     - Represents a character definition in the MIB.
   * - :doc:`CharDefinitionListValue <Lextm.SharpSnmpPro.Mib.CharDefinitionListValue>`
     - Represents a list of :dn:cls:``~Lextm.SharpSnmpPro.Mib.CharDefinition`` values.
   * - :doc:`ChoiceType <Lextm.SharpSnmpPro.Mib.ChoiceType>`
     - Represents a CHOICE type in SMI, which allows one of several types.
   * - :doc:`ChoiceValue <Lextm.SharpSnmpPro.Mib.ChoiceValue>`
     - Represents a choice value in an SMI (Structure of Management Information) context.
   * - :doc:`ClassNumber <Lextm.SharpSnmpPro.Mib.ClassNumber>`
     - Represents a class number, which may be constructed from a string or a :dn:cls:``~Lextm.SharpSnmpPro.Mib.DefinedValue``.
   * - :doc:`Compliance <Lextm.SharpSnmpPro.Mib.Compliance>`
     - Represents a compliance statement for an SNMP MIB module.
   * - :doc:`Constraint <Lextm.SharpSnmpPro.Mib.Constraint>`
     - Represents a constraint that can be applied to SNMP data, consisting of element set specifications and exception specifications.
   * - :doc:`ConstraintedType <Lextm.SharpSnmpPro.Mib.ConstraintedType>`
     - Represents a type with constraints in a MIB module.
   * - :doc:`ConstraintElement <Lextm.SharpSnmpPro.Mib.ConstraintElement>`
     - Represents an abstract base class for SNMP constraint elements.
   * - :doc:`Counter32Type <Lextm.SharpSnmpPro.Mib.Counter32Type>`
     - Represents the Counter32 SMI type.
   * - :doc:`Counter64Type <Lextm.SharpSnmpPro.Mib.Counter64Type>`
     - Represents the Counter64 SMI type.
   * - :doc:`DecoderRegistry <Lextm.SharpSnmpPro.Mib.DecoderRegistry>`
     - Registry for decoders.
   * - :doc:`DefinedValue <Lextm.SharpSnmpPro.Mib.DefinedValue>`
     - Represents a value defined in a specific module.
   * - :doc:`Document <Lextm.SharpSnmpPro.Mib.Document>`
     - MIB document.
   * - :doc:`ElementSetConstraintElement <Lextm.SharpSnmpPro.Mib.ElementSetConstraintElement>`
     - Represents a constraint element that wraps another :dn:cls:``~Lextm.SharpSnmpPro.Mib.ConstraintElement`` as part of an element set.
   * - :doc:`ElementSetRange <Lextm.SharpSnmpPro.Mib.ElementSetRange>`
     - Represents a range of constraint elements, optionally containing an ellipsis.
   * - :doc:`ElementType <Lextm.SharpSnmpPro.Mib.ElementType>`
     - Represents an element type in a MIB module.
   * - :doc:`EmbeddedType <Lextm.SharpSnmpPro.Mib.EmbeddedType>`
     - Represents an embedded SMI type within a MIB module.
   * - :doc:`EntityExtensions <Lextm.SharpSnmpPro.Mib.EntityExtensions>`
     - Extension methods of :dn:iface:``~Lextm.SharpSnmpPro.Mib.IEntity``.
   * - :doc:`EntityStatusExtensions <Lextm.SharpSnmpPro.Mib.EntityStatusExtensions>`
     - Extension methods for the :dn:enum:``~Lextm.SharpSnmpPro.Mib.EntityStatus`` enumeration.
   * - :doc:`EnumType <Lextm.SharpSnmpPro.Mib.EnumType>`
     - Represents an enumeration type in a MIB module.
   * - :doc:`ErrorMacro <Lextm.SharpSnmpPro.Mib.ErrorMacro>`
     - Represents an ERROR MACRO type in a MIB module.
   * - :doc:`ExceptionSpec <Lextm.SharpSnmpPro.Mib.ExceptionSpec>`
     - Represents an exception specification for SNMP MIB values.
   * - :doc:`Exports <Lextm.SharpSnmpPro.Mib.Exports>`
     - Represents a collection of exported symbols from a MIB module.
   * - :doc:`FromConstraintElement <Lextm.SharpSnmpPro.Mib.FromConstraintElement>`
     - Represents a constraint element that is constructed from a :dn:prop:``~Lextm.SharpSnmpPro.Mib.FromConstraintElement.Constraint`` instance.
   * - :doc:`FullQualifiedValue <Lextm.SharpSnmpPro.Mib.FullQualifiedValue>`
     - Represents a fully qualified value in the MIB (Management Information Base).
   * - :doc:`Gauge32Type <Lextm.SharpSnmpPro.Mib.Gauge32Type>`
     - Represents the Gauge32 SMI type.
   * - :doc:`IdComponent <Lextm.SharpSnmpPro.Mib.IdComponent>`
     - Represents a component of an object identifier (OID) in a MIB.
   * - :doc:`IdComponentList <Lextm.SharpSnmpPro.Mib.IdComponentList>`
     - Represents a list of identifier components, optionally associated with a defined value.
   * - :doc:`IdListValue <Lextm.SharpSnmpPro.Mib.IdListValue>`
     - Represents a value consisting of a list of identifier strings.
   * - :doc:`Import <Lextm.SharpSnmpPro.Mib.Import>`
     - IMPORT statement.
   * - :doc:`IncludeTypeConstraintElement <Lextm.SharpSnmpPro.Mib.IncludeTypeConstraintElement>`
     - Represents a constraint element that includes or excludes a specific SMI type.
   * - :doc:`Index <Lextm.SharpSnmpPro.Mib.Index>`
     - Represents an index in a MIB table, including its type and whether it is implied.
   * - :doc:`IntegerType <Lextm.SharpSnmpPro.Mib.IntegerType>`
     - Represents the INTEGER type in SMI, supporting named numbers and constraints.
   * - :doc:`InvalidEntityException <Lextm.SharpSnmpPro.Mib.InvalidEntityException>`
     - The exception that is thrown when an invalid entity is encountered in the MIB.
   * - :doc:`IpAddressType <Lextm.SharpSnmpPro.Mib.IpAddressType>`
     - Represents the IpAddress SMI type.
   * - :doc:`Module <Lextm.SharpSnmpPro.Mib.Module>`
     - MIB module.
   * - :doc:`ModuleCompliance <Lextm.SharpSnmpPro.Mib.ModuleCompliance>`
     - Represents a module compliance statement in an SNMP MIB.
   * - :doc:`ModuleComplianceMacro <Lextm.SharpSnmpPro.Mib.ModuleComplianceMacro>`
     - Represents the MODULE-COMPLIANCE macro in an SNMP MIB module.
   * - :doc:`ModuleIdentityMacro <Lextm.SharpSnmpPro.Mib.ModuleIdentityMacro>`
     - Represents the MODULE-IDENTITY macro in a MIB module.
   * - :doc:`NamedBit <Lextm.SharpSnmpPro.Mib.NamedBit>`
     - Represents a named bit value in an SNMP MIB.
   * - :doc:`NamedConstraintElement <Lextm.SharpSnmpPro.Mib.NamedConstraintElement>`
     - Represents a named constraint element for SNMP, which can be present, absent, or optional, and may have an associated constraint.
   * - :doc:`NamedNumber <Lextm.SharpSnmpPro.Mib.NamedNumber>`
     - Represents a named number, which associates a name with a numeric or defined value.
   * - :doc:`NamedValue <Lextm.SharpSnmpPro.Mib.NamedValue>`
     - Represents a named value pair for SNMP MIB entities.
   * - :doc:`NormalConstraintElement <Lextm.SharpSnmpPro.Mib.NormalConstraintElement>`
     - Represents a normal constraint element that can combine multiple constraints using union, bar, or intersect logic.
   * - :doc:`NotificationGroupMacro <Lextm.SharpSnmpPro.Mib.NotificationGroupMacro>`
     - Represents a NOTIFICATION-GROUP macro in an SNMP MIB.
   * - :doc:`NotificationTypeMacro <Lextm.SharpSnmpPro.Mib.NotificationTypeMacro>`
     - Represents a NOTIFICATION-TYPE macro in a MIB module.
   * - :doc:`NotResolvedException <Lextm.SharpSnmpPro.Mib.NotResolvedException>`
     - Exception raised when type resolution fails.
   * - :doc:`NumberLiteralValue <Lextm.SharpSnmpPro.Mib.NumberLiteralValue>`
     - Represents a numeric literal value for SMI (Structure of Management Information).
   * - :doc:`ObjectGroupMacro <Lextm.SharpSnmpPro.Mib.ObjectGroupMacro>`
     - Object group macro.
   * - :doc:`ObjectIdentifierMacro <Lextm.SharpSnmpPro.Mib.ObjectIdentifierMacro>`
     - Represents an OBJECT IDENTIFIER macro in a MIB module.
   * - :doc:`ObjectIdentityMacro <Lextm.SharpSnmpPro.Mib.ObjectIdentityMacro>`
     - Represents the OBJECT-IDENTITY macro in a MIB module.
   * - :doc:`ObjectTypeMacro <Lextm.SharpSnmpPro.Mib.ObjectTypeMacro>`
     - Object type macro.
   * - :doc:`OctetStringType <Lextm.SharpSnmpPro.Mib.OctetStringType>`
     - Represents the OCTET STRING type in SMI, with optional BITS support.
   * - :doc:`OperationMacro <Lextm.SharpSnmpPro.Mib.OperationMacro>`
     - Represents an OPERATION macro in SMI, describing an operation with argument and result types, error list, and linked operations.
   * - :doc:`PatternConstraintElement <Lextm.SharpSnmpPro.Mib.PatternConstraintElement>`
     - Represents a constraint element that enforces a pattern on SNMP values.
   * - :doc:`QuadValue <Lextm.SharpSnmpPro.Mib.QuadValue>`
     - Represents a value composed of four :dn:cls:``~Lextm.SharpSnmpPro.Mib.NumberLiteralValue`` instances.
   * - :doc:`Revision <Lextm.SharpSnmpPro.Mib.Revision>`
     - Used to store the source control system information.
   * - :doc:`SelectionType <Lextm.SharpSnmpPro.Mib.SelectionType>`
     - Represents a selection type in SMI (Structure of Management Information).
   * - :doc:`SemanticException <Lextm.SharpSnmpPro.Mib.SemanticException>`
     - Semantic exception.
   * - :doc:`SequenceOfType <Lextm.SharpSnmpPro.Mib.SequenceOfType>`
     - Represents an SMI SEQUENCE OF type.
   * - :doc:`SequenceOfValue <Lextm.SharpSnmpPro.Mib.SequenceOfValue>`
     - Represents a sequence of :dn:iface:``~Lextm.SharpSnmpPro.Mib.ISmiValue`` objects.
   * - :doc:`SequenceType <Lextm.SharpSnmpPro.Mib.SequenceType>`
     - Represents an SMI SEQUENCE type, which is a collection of element types.
   * - :doc:`SequenceValue <Lextm.SharpSnmpPro.Mib.SequenceValue>`
     - Represents a sequence value consisting of a collection of named values.
   * - :doc:`SetOfType <Lextm.SharpSnmpPro.Mib.SetOfType>`
     - Represents a SET OF type in SMI, which is a collection of elements of a specified subtype.
   * - :doc:`SetType <Lextm.SharpSnmpPro.Mib.SetType>`
     - Represents an SMI SET type, which is a collection of element types.
   * - :doc:`SizeConstraintElement <Lextm.SharpSnmpPro.Mib.SizeConstraintElement>`
     - Represents a size constraint element for SNMP data.
   * - :doc:`SmiTypeExtensions <Lextm.SharpSnmpPro.Mib.SmiTypeExtensions>`
     - Provides extension methods for working with :dn:iface:``~Lextm.SharpSnmpPro.Mib.ISmiType`` objects, enabling operations such as verification, decoding, and type resolution.
   * - :doc:`Symbol <Lextm.SharpSnmpPro.Mib.Symbol>`
     - Symbol in IMPORTS statement.
   * - :doc:`Tag <Lextm.SharpSnmpPro.Mib.Tag>`
     - Represents a tag with a type and a class number in the SNMP MIB context.
   * - :doc:`TaggedElementType <Lextm.SharpSnmpPro.Mib.TaggedElementType>`
     - Represents a tagged element type in the MIB, which is derived from another type and can be validated.
   * - :doc:`TaggedType <Lextm.SharpSnmpPro.Mib.TaggedType>`
     - Represents a tagged type in an SMI module, such as those using [APPLICATION n] or [IMPLICIT].
   * - :doc:`TextualConventionMacro <Lextm.SharpSnmpPro.Mib.TextualConventionMacro>`
     - Represents a TEXTUAL-CONVENTION macro in an SMI module.
   * - :doc:`TimeTicksType <Lextm.SharpSnmpPro.Mib.TimeTicksType>`
     - Represents the TimeTicks basic type in SNMP MIBs.
   * - :doc:`TrapTypeMacro <Lextm.SharpSnmpPro.Mib.TrapTypeMacro>`
     - Trap type macro.
   * - :doc:`TupleValue <Lextm.SharpSnmpPro.Mib.TupleValue>`
     - Represents a tuple of two :dn:cls:``~Lextm.SharpSnmpPro.Mib.NumberLiteralValue`` values.
   * - :doc:`TypeAssignment <Lextm.SharpSnmpPro.Mib.TypeAssignment>`
     - Represents a type assignment in a MIB module.
   * - :doc:`TypeOrValue <Lextm.SharpSnmpPro.Mib.TypeOrValue>`
     - Represents either an SMI type or an SMI value.
   * - :doc:`UnknownType <Lextm.SharpSnmpPro.Mib.UnknownType>`
     - Represents an unknown derived type in the MIB.
   * - :doc:`ValueRange <Lextm.SharpSnmpPro.Mib.ValueRange>`
     - Represents a value range with optional minimum and maximum values and comparison options.
   * - :doc:`ValueRangeConstraintElement <Lextm.SharpSnmpPro.Mib.ValueRangeConstraintElement>`
     - Represents a constraint element that verifies whether SNMP data falls within a specified value range.
   * - :doc:`Variantion <Lextm.SharpSnmpPro.Mib.Variantion>`
     - Represents a variation of an SMI (Structure of Management Information) object.
   * - :doc:`WithComponentConstraintElement <Lextm.SharpSnmpPro.Mib.WithComponentConstraintElement>`
     - Represents a constraint element with a component constraint in SNMP MIB definitions.
   * - :doc:`WithComponentsConstraintElement <Lextm.SharpSnmpPro.Mib.WithComponentsConstraintElement>`
     - Represents a WITH COMPONENTS constraint element in SNMP MIB definitions.

Interfaces
----------

.. list-table::
   :header-rows: 1
   :widths: 30 70

   * - Type
     - Description
   * - :doc:`IConstruct <Lextm.SharpSnmpPro.Mib.IConstruct>`
     - Construct interface.
   * - :doc:`IDecoder <Lextm.SharpSnmpPro.Mib.IDecoder>`
     - Decoder interface.
   * - :doc:`IEntity <Lextm.SharpSnmpPro.Mib.IEntity>`
     - Entity interface.
   * - :doc:`IObjectTypeMacro <Lextm.SharpSnmpPro.Mib.IObjectTypeMacro>`
     - OBJECT-TYPE macro interface.
   * - :doc:`ISmiType <Lextm.SharpSnmpPro.Mib.ISmiType>`
     - Represents an SMI (Structure of Management Information) type.
   * - :doc:`ISmiValue <Lextm.SharpSnmpPro.Mib.ISmiValue>`
     - SMI value interface.
   * - :doc:`IValidatable <Lextm.SharpSnmpPro.Mib.IValidatable>`
     - Validable interface.

Enums
-----

.. list-table::
   :header-rows: 1
   :widths: 30 70

   * - Type
     - Description
   * - :doc:`Access <Lextm.SharpSnmpPro.Mib.Access>`
     - Access modifier.
   * - :doc:`CharacterSet <Lextm.SharpSnmpPro.Mib.CharacterSet>`
     - Represents the character sets supported by the MIB parser.
   * - :doc:`DefinitionType <Lextm.SharpSnmpPro.Mib.DefinitionType>`
     - Definition type.
   * - :doc:`EntityStatus <Lextm.SharpSnmpPro.Mib.EntityStatus>`
     - Status enumeration for entities.
   * - :doc:`PibAccess <Lextm.SharpSnmpPro.Mib.PibAccess>`
     - Specifies the access level for a Protocol Information Base (PIB) object.
   * - :doc:`SmiVersion <Lextm.SharpSnmpPro.Mib.SmiVersion>`
     - SMI version.
   * - :doc:`Status <Lextm.SharpSnmpPro.Mib.Status>`
     - Status enum.
   * - :doc:`TagDefault <Lextm.SharpSnmpPro.Mib.TagDefault>`
     - Specifies the default tagging mode for ASN.1 types.
   * - :doc:`VerificationStatus <Lextm.SharpSnmpPro.Mib.VerificationStatus>`
     - Represents the verification status of an entity.

