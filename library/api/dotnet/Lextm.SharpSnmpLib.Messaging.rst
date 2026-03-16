Lextm.SharpSnmpLib.Messaging Namespace
======================================

.. dn:namespace:: Lextm.SharpSnmpLib.Messaging

Classes
-------

.. list-table::
   :header-rows: 1
   :widths: 30 70

   * - Type
     - Description
   * - :doc:`AgentFoundEventArgs <Lextm.SharpSnmpLib.Messaging.AgentFoundEventArgs>`
     - Represents the AgentFoundEventArgs type.
   * - :doc:`AgentVariable <Lextm.SharpSnmpLib.Messaging.AgentVariable>`
     - Represents the AgentVariable type.
   * - :doc:`Discoverer <Lextm.SharpSnmpLib.Messaging.Discoverer>`
     - Discoverer class to discover SNMP agents in the same network.
   * - :doc:`Discovery <Lextm.SharpSnmpLib.Messaging.Discovery>`
     - Discovery class that participates in SNMP v3 discovery process.
   * - :doc:`ExceptionRaisedEventArgs <Lextm.SharpSnmpLib.Messaging.ExceptionRaisedEventArgs>`
     - Provides data for exception raised event.
   * - :doc:`GetBulkRequestMessage <Lextm.SharpSnmpLib.Messaging.GetBulkRequestMessage>`
     - Legacy compatibility wrapper for SNMP GET-BULK request messages.
   * - :doc:`GetNextRequestMessage <Lextm.SharpSnmpLib.Messaging.GetNextRequestMessage>`
     - Legacy compatibility wrapper for SNMP GET-NEXT request messages.
   * - :doc:`GetRequestMessage <Lextm.SharpSnmpLib.Messaging.GetRequestMessage>`
     - Legacy compatibility wrapper for SNMP v3 GET request message.
   * - :doc:`InformRequestMessage <Lextm.SharpSnmpLib.Messaging.InformRequestMessage>`
     - Legacy compatibility wrapper for SNMP INFORM request messages.
   * - :doc:`LegacyPdu <Lextm.SharpSnmpLib.Messaging.LegacyPdu>`
     - Legacy PDU facade exposed by compatibility APIs.
   * - :doc:`MessageFactory <Lextm.SharpSnmpLib.Messaging.MessageFactory>`
     - Factory that creates :dn:iface:``~DotNetSnmp.Common.Definitions.ISnmpMessage`` instances from byte format.
   * - :doc:`MessageFactoryException <Lextm.SharpSnmpLib.Messaging.MessageFactoryException>`
     - Exception raised when message parsing fails.
   * - :doc:`Messenger <Lextm.SharpSnmpLib.Messaging.Messenger>`
     - Messenger class contains all static helper methods you need to send out SNMP messages.
   * - :doc:`NumberGenerator <Lextm.SharpSnmpLib.Messaging.NumberGenerator>`
     - A counter that generates IDs.
   * - :doc:`PortInUseException <Lextm.SharpSnmpLib.Messaging.PortInUseException>`
     - Exception raised when an endpoint is already in use.
   * - :doc:`ReportMessage <Lextm.SharpSnmpLib.Messaging.ReportMessage>`
     - REPORT message wrapper for compatibility APIs.
   * - :doc:`ResponseMessage <Lextm.SharpSnmpLib.Messaging.ResponseMessage>`
     - Legacy compatibility wrapper for SNMP response messages.
   * - :doc:`SetRequestMessage <Lextm.SharpSnmpLib.Messaging.SetRequestMessage>`
     - Legacy compatibility wrapper for SNMP SET request messages.
   * - :doc:`SnmpMessageCompatibilityExtensions <Lextm.SharpSnmpLib.Messaging.SnmpMessageCompatibilityExtensions>`
     - Provides helper methods for SnmpMessageCompatibilityExtensions.
   * - :doc:`SnmpMessageExtension <Lextm.SharpSnmpLib.Messaging.SnmpMessageExtension>`
     - Backward-compatible entry point for legacy extension APIs.
   * - :doc:`TimeoutException <Lextm.SharpSnmpLib.Messaging.TimeoutException>`
     - Exception raised when an SNMP operation times out.
   * - :doc:`TrapV1Message <Lextm.SharpSnmpLib.Messaging.TrapV1Message>`
     - Legacy compatibility wrapper for SNMP TRAP v1 messages.
   * - :doc:`TrapV2Message <Lextm.SharpSnmpLib.Messaging.TrapV2Message>`
     - Legacy compatibility wrapper for TrapV2 message sending.

Enums
-----

.. list-table::
   :header-rows: 1
   :widths: 30 70

   * - Type
     - Description
   * - :doc:`WalkMode <Lextm.SharpSnmpLib.Messaging.WalkMode>`
     - Walk mode.

