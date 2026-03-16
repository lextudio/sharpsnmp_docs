AgentFoundEventArgs Class
=========================

.. dn:class:: Lextm.SharpSnmpLib.Messaging.AgentFoundEventArgs

   Represents the AgentFoundEventArgs type.

   .. code-block:: csharp

      public sealed class AgentFoundEventArgs : EventArgs

**Namespace:** ``Lextm.SharpSnmpLib.Messaging``

**Inheritance:** Object → EventArgs → ``AgentFoundEventArgs``

**Source:** `SharpSnmpLib/Messaging/Discoverer.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Discoverer.cs#L39>`__

Constructors
------------

AgentFoundEventArgs(IPEndPoint, AgentVariable?)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Messaging.AgentFoundEventArgs..ctor(System.Net.IPEndPoint,Lextm.SharpSnmpLib.Messaging.AgentVariable)

   Initializes a new instance of AgentFoundEventArgs.

   .. code-block:: csharp

      public AgentFoundEventArgs(IPEndPoint agent, AgentVariable? variable)

   :type agent: ``IPEndPoint``
   :type variable: :dn:cls:`~Lextm.SharpSnmpLib.Messaging.AgentVariable`

**Source:** `SharpSnmpLib/Messaging/Discoverer.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Discoverer.cs#L44>`__

Properties
----------

Agent
~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.AgentFoundEventArgs.Agent

   Gets agent.

   .. code-block:: csharp

      public IPEndPoint Agent { get; }

   :rtype: ``IPEndPoint``

**Source:** `SharpSnmpLib/Messaging/Discoverer.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Discoverer.cs#L53>`__

Variable
~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.AgentFoundEventArgs.Variable

   Gets variable.

   .. code-block:: csharp

      public AgentVariable? Variable { get; }

   :rtype: :dn:cls:`~Lextm.SharpSnmpLib.Messaging.AgentVariable`

**Source:** `SharpSnmpLib/Messaging/Discoverer.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/Discoverer.cs#L58>`__

