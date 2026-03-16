ExceptionRaisedEventArgs Class
==============================

.. dn:class:: Lextm.SharpSnmpLib.Messaging.ExceptionRaisedEventArgs

   Provides data for exception raised event.

   .. code-block:: csharp

      public sealed class ExceptionRaisedEventArgs : EventArgs

**Namespace:** ``Lextm.SharpSnmpLib.Messaging``

**Inheritance:** Object → EventArgs → ``ExceptionRaisedEventArgs``

**Source:** `SharpSnmpLib/Messaging/ExceptionRaisedEventArgs.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/ExceptionRaisedEventArgs.cs#L5>`__

Constructors
------------

ExceptionRaisedEventArgs(Exception)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Messaging.ExceptionRaisedEventArgs..ctor(System.Exception)

   Creates an :dn:cls:``~Lextm.SharpSnmpLib.Messaging.ExceptionRaisedEventArgs``.

   .. code-block:: csharp

      public ExceptionRaisedEventArgs(Exception ex)

   :param ex: Exception.
   :type ex: ``Exception``

**Source:** `SharpSnmpLib/Messaging/ExceptionRaisedEventArgs.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/ExceptionRaisedEventArgs.cs#L11>`__

Properties
----------

Exception
~~~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Messaging.ExceptionRaisedEventArgs.Exception

   Exception.

   .. code-block:: csharp

      public Exception Exception { get; }

   :rtype: ``Exception``

**Source:** `SharpSnmpLib/Messaging/ExceptionRaisedEventArgs.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Messaging/ExceptionRaisedEventArgs.cs#L19>`__

