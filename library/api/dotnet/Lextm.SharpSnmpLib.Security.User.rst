User Class
==========

.. dn:class:: Lextm.SharpSnmpLib.Security.User

   User class.

   .. code-block:: csharp

      public sealed class User

**Namespace:** ``Lextm.SharpSnmpLib.Security``

**Inheritance:** Object → ``User``

**Source:** `SharpSnmpLib/Security/User.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/User.cs#L28>`__

Constructors
------------

User(OctetString, IPrivacyProvider)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. dn:constructor:: Lextm.SharpSnmpLib.Security.User..ctor(DotNetSnmp.Asn1.SyntaxObjects.OctetString,DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider)

   Initializes a new instance of User.

   .. code-block:: csharp

      public User(OctetString name, IPrivacyProvider privacy)

   :param name: The name.
   :type name: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`
   :param privacy: The privacy provider.
   :type privacy: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`

**Source:** `SharpSnmpLib/Security/User.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/User.cs#L35>`__

Properties
----------

Name
~~~~

.. dn:property:: Lextm.SharpSnmpLib.Security.User.Name

   Gets name.

   .. code-block:: csharp

      public OctetString Name { get; }

   :returns: The name.
   :rtype: :dn:struct:`~DotNetSnmp.Asn1.SyntaxObjects.OctetString`

**Source:** `SharpSnmpLib/Security/User.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/User.cs#L45>`__

Privacy
~~~~~~~

.. dn:property:: Lextm.SharpSnmpLib.Security.User.Privacy

   Gets privacy.

   .. code-block:: csharp

      public IPrivacyProvider Privacy { get; }

   :returns: The provider.
   :rtype: :dn:iface:`~DotNetSnmp.Protocol.V3.Security.Privacy.IPrivacyProvider`

**Source:** `SharpSnmpLib/Security/User.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/User.cs#L51>`__

Methods
-------

ToString()
~~~~~~~~~~

.. dn:method:: Lextm.SharpSnmpLib.Security.User.ToString

   Returns a ``String`` that represents this instance.

   .. code-block:: csharp

      public override string ToString()

   :returns: A ``String`` that represents this instance.
   :rtype: ``String``

**Source:** `SharpSnmpLib/Security/User.cs <https://github.com/lextudio/sharpsnmplib/blob/release-13.0/SharpSnmpLib/Security/User.cs#L59>`__

