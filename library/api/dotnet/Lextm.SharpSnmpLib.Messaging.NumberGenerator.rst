NumberGenerator Class
=====================

.. dn:class:: Lextm.SharpSnmpLib.Messaging.NumberGenerator

   A counter that generates IDs.

   .. code-block:: csharp

      public sealed class NumberGenerator

**Namespace:** ``Lextm.SharpSnmpLib.Messaging``

**Inheritance:** Object → ``NumberGenerator``

**Source:** `SharpSnmpLib/Messaging/NumberGenerator.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/NumberGenerator.cs#L5>`__

Constructors
------------

NumberGenerator(Int32, Int32)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Messaging.NumberGenerator..ctor(System.Int32,System.Int32)

   Initializes a new instance of NumberGenerator.

   .. code-block:: csharp

      public NumberGenerator(int min, int max)

   :param min: The minimum generated value.
   :type min: ``Int32``
   :param max: The maximum generated value.
   :type max: ``Int32``

**Source:** `SharpSnmpLib/Messaging/NumberGenerator.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/NumberGenerator.cs#L17>`__

Properties
----------

NextId
~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.NumberGenerator.NextId

   Returns the next ID.

   .. code-block:: csharp

      public int NextId { get; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Messaging/NumberGenerator.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/NumberGenerator.cs#L27>`__

