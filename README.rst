**********************************
Conreality Development Environment
**********************************

.. image:: https://img.shields.io/badge/license-Public%20Domain-blue.svg
   :alt: Project license
   :target: https://unlicense.org/

.. image:: https://img.shields.io/travis/conreality/conreality-devbox/master.svg
   :alt: Travis CI build status
   :target: https://travis-ci.org/conreality/conreality-devbox

|

https://wiki.conreality.org/DevBox

Screenshot
==========

.. image:: https://raw.githubusercontent.com/conreality/conreality-devbox/master/screenshot.jpg
   :alt: Conreality DevBox screenshot

Prerequisites
=============

Build Prerequisites
-------------------

* `Docker <https://www.docker.com/community-edition>`__
* `GNU Make <https://www.gnu.org/software/make/>`__

Features
========

Network Services
----------------

* SSH server (``dropbear``) listening on exposed TCP port 22.
* VNC server (``x11vnc``/``xvfb``) listening on exposed TCP port 5900.
* mDNS server (``avahi-daemon``) listening on UDP port 5353.

Installed Software
------------------

* The VIM, JOE, and nano editors.
* Bash, cURL, Git, GPG, Irssi, Sudo, screen, tmux, xterm, xz.
* OpenCV libraries.
* OpenGL demos (``mesa-demos``).
* PostgreSQL client.
* Avahi tools for mDNS browsing.

Configuration
-------------

* The time zone is UTC (``TZ=UTC``), the locale is UTF-8
  (``LANG=en_US.UTF-8``).

* The default user account is ``admin`` with password ``admin``.

Usage
=====

::

   $ make && make install

   $ make boot                  # Runs a VNC server on 127.0.0.1:5900

See Also
========

* `Conreality Docker Image
   <https://github.com/conreality/conreality-docker>`__

* `Conreality Master Firmware
   <https://github.com/conreality/conreality-master>`__

* `Conreality Slave Firmware
   <https://github.com/conreality/conreality-slave>`__
