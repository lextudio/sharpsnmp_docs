AgentVariable Class
===================

.. dn:class:: Lextm.SharpSnmpLib.Messaging.AgentVariable

   Represents the AgentVariable type.

   .. code-block:: csharp

      public sealed class AgentVariable

**Namespace:** ``Lextm.SharpSnmpLib.Messaging``

**Inheritance:** Object → ``AgentVariable``

**Source:** `SharpSnmpLib/Messaging/Discoverer.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Discoverer.cs#L64>`__

Constructors
------------

AgentVariable(ObjectIdentifier, IAsnSerializable)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Messaging.AgentVariable..ctor(DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier,DotNetSnmp.Asn1.Serialization.IAsnSerializable)

   Initializes a new instance of AgentVariable.

   .. code-block:: csharp

      public AgentVariable(ObjectIdentifier id, IAsnSerializable data)

   :type id: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`
   :type data: :dn:iface:`~DotNetSnmp.Asn1.Serialization.IAsnSerializable`

**Source:** `SharpSnmpLib/Messaging/Discoverer.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Discoverer.cs#L69>`__

Properties
----------

Data
~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.AgentVariable.Data

   Gets data.

   .. code-block:: csharp

      public IAsnSerializable Data { get; }

   :rtype: :dn:iface:`~DotNetSnmp.Asn1.Serialization.IAsnSerializable`

**Source:** `SharpSnmpLib/Messaging/Discoverer.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Discoverer.cs#L83>`__

Id
~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.AgentVariable.Id

   Gets id.

   .. code-block:: csharp

      public ObjectIdentifier Id { get; }

   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.ObjectIdentifier`

**Source:** `SharpSnmpLib/Messaging/Discoverer.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Discoverer.cs#L78>`__

Methods
-------

ToString()
~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Messaging.AgentVariable.ToString

   Returns a string representation of the current value.

   .. code-block:: csharp

      public override string ToString()

   :rtype: ``String``

**Source:** `SharpSnmpLib/Messaging/Discoverer.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Discoverer.cs#L88>`__

