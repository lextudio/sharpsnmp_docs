UserRegistry Class
==================

.. dn:class:: Lextm.SharpSnmpLib.Security.UserRegistry

   A repository to store user information for providers.

   .. code-block:: csharp

      public sealed class UserRegistry

**Namespace:** ``Lextm.SharpSnmpLib.Security``

**Inheritance:** Object → ``UserRegistry``

**Source:** `SharpSnmpLib/Security/UserRegistry.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/UserRegistry.cs#L29>`__

Constructors
------------

UserRegistry()
~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Security.UserRegistry..ctor

   Initializes a new instance of UserRegistry.

   .. code-block:: csharp

      public UserRegistry()

**Source:** `SharpSnmpLib/Security/UserRegistry.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/UserRegistry.cs#L53>`__

UserRegistry(User[]?)
~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Security.UserRegistry..ctor(Lextm.SharpSnmpLib.Security.User[])

   Initializes a new instance of UserRegistry.

   .. code-block:: csharp

      public UserRegistry(User[]? users)

   :param users: The users.
   :type users: ``User[]``

**Source:** `SharpSnmpLib/Security/UserRegistry.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/UserRegistry.cs#L37>`__

Properties
----------

Count
~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Security.UserRegistry.Count

   Returns the user count.

   .. code-block:: csharp

      public int Count { get; }

   :rtype: ``Int32``

**Source:** `SharpSnmpLib/Security/UserRegistry.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/UserRegistry.cs#L60>`__

Methods
-------

Add(OctetString, IPrivacyProvider)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Security.UserRegistry.Add(DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider)

   Adds the specified user name.

   .. code-block:: csharp

      public UserRegistry Add(OctetString userName, IPrivacyProvider privacy)

   :param userName: Name of the user.
   :type userName: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :param privacy: The privacy provider.
   :type privacy: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`

   :rtype: :dn:cls:`~Lextm.SharpSnmpLib.Security.UserRegistry`

**Source:** `SharpSnmpLib/Security/UserRegistry.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/UserRegistry.cs#L67>`__

Add(User?)
~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Security.UserRegistry.Add(Lextm.SharpSnmpLib.Security.User)

   Adds the specified user.

   .. code-block:: csharp

      public UserRegistry Add(User? user)

   :param user: The user.
   :type user: :dn:cls:`~Lextm.SharpSnmpLib.Security.User`

   :rtype: :dn:cls:`~Lextm.SharpSnmpLib.Security.UserRegistry`

**Source:** `SharpSnmpLib/Security/UserRegistry.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/UserRegistry.cs#L76>`__

Find(OctetString)
~~~~~~~~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Security.UserRegistry.Find(DotNetSnmp.Asn1.SyntaxObjects.OctetString)

   Finds the specified user name.

   .. code-block:: csharp

      public IPrivacyProvider? Find(OctetString userName)

   :param userName: Name of the user.
   :type userName: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`

   :rtype: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`

**Source:** `SharpSnmpLib/Security/UserRegistry.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/UserRegistry.cs#L97>`__

ToString()
~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Security.UserRegistry.ToString

   Returns a ``String`` that represents this instance.

   .. code-block:: csharp

      public override string ToString()

   :returns: A ``String`` that represents this instance.
   :rtype: ``String``

**Source:** `SharpSnmpLib/Security/UserRegistry.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/UserRegistry.cs#L114>`__

