.. DHCPAP documentation master file, created by
   sphinx-quickstart on Fri Aug 18 01:10:31 2017.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.


.. image:: ./images/dhcpcanon.*
    :scale: 50%

Welcome to DHCPAP's documentation!
==================================

DH-What?!
----------

`DHCP <https://en.wikipedia.org/wiki/DHCP>`__ stands for
**Dynamic Host Configuration Protocol**. It's a
`network protocol <https://en.wikipedia.org/wiki/Network_protocol>`__ used to
get network configuration parameters, such as
`IP addresses <https://en.wikipedia.org/wiki/IP_address>`__ automatically.

Every time a device, such as a laptop or mobile connects to a Wifi
network in a cafe, office, home, etc., it send a DHCP request.

Some DHCP options carry unique identifiers that can enable device tracking and
fingerprinting.

**AP** stands for `Anonymity Profiles <https://tools.ietf.org/html/rfc7844.html>`__,
an standard that provide guidelines on the composition of DHCP messages,
designed to minimize disclosure of identifying information.

**Important**: if you run a DHCP client implementing the Anonymity Profiles, the
hardware address (`MAC <https://en.wikipedia.org/wiki/MAC_address>`__) should
be randomized.
You can use `macchanger <https://github.com/alobbs/macchanger>`__,
`macouflage <https://github.com/subgraph/macouflage>`__ or other.

For users
----------

`dhcpcanon <https://dhcpcanon.readthedocs.io/>`__ is a DHCP client implementing
the Anonymity Profiles.

It's tested in Debian/Ubuntu, other Linux distributions coming soon, as well as
Gnome Network Manager integration.

Windows 10 has a privative implementation of the Anonymity Profiles.

For educational purposes
------------------------

`dhcpcfp <https://dhcpcfp.readthedocs.io/>`__ is a DHCP scanner,
intended to be run in controlled networks to show how is possible to
fingerprint devices.

For developers
---------------

(Look the two sections above).

``systemd`` implements its own DHCP client and now it also implements the
Anonymity profiles (`branch <https://github.com/juga0/systemd/tree/features/rfc7844>`__
merged in upstream).
Refer to the documentation on how to run systemd DHCP client and
`systemd modifications <http://systemd-dhcpap-notes.readthedocs.io>`__
(`source <https://github.com/juga0/systemd>`__)

`Comments on the RFC 7844 <https://rfc7844-comments.readthedocs.io>`__
(`source <https://github.com/juga0/rfc7844-comments>`__)

Slides:

* `Bornhack slides <https://dhcpap.github.io/dhcpap_hax_slides/>`__
  (`source <https://github.com/DHCPAP/dhcpap_hax_slides>`__)
* `PrototypeFund slides <https://dhcpap.github.io/dhcpcanon_p_slides/>`__
  (`source <https://github.com/DHCPAP/dhcpcanon_p_slides>`__)

Others
--------

.. toctree::
   :maxdepth: 2

   glossary
   links

* :ref:`search`
