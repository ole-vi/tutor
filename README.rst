.. _readme_intro_start:

This image is customized for Treehouses
========================================================================

Requirement
----------
1. Raspberry Pi4 with 8gb RAM
2. At least 32GB MicroSD
3. Treehouses
  * Download from `here <http://dev.ole.org/>`_
  * Download treehouse-[number].img.gz (Download the latest version, which means the numebr is the biggest)

Quickstart for Treehouses
----------

**Do not execute Tutor command as root user**

1. Install the `latest stable release <https://github.com/treehouses/openedx/releases>`_ of Tutor
2. Check out Tor is starting 
  1. if command ``treehouses tor`` shows you onion address, Tor is starting
  2. If not, type
    1. ``treehouses tor add 80``
    2. ``treehouses tor start``
3. Run ``tutor local quickstartfortreehouses``
4. You're done!

Start OpenEdx via Treehouses services
----------

**Execute Treehouses services command as root user**

On your Treehouses image, get Treehouses CLI repository

1. ``git clone https://github.com/treehouses/cli``
2. ``cd cli``
3. ``git checkout neo-add-tutor``
4. Check out Tor as showing at the above Quickstart for Treehouses
5. ``./cli.sh services openedx install`` -> make configuration
6. ``./cli.sh services openedx up`` -> download all Docker images and start containers

Tutor: the docker-based Open edX distribution designed for peace of mind
========================================================================

|

.. image:: https://overhang.io/static/img/tutor-logo.svg
  :alt: Tutor logo
  :width: 500px
  :align: center

|

.. image:: https://img.shields.io/travis/overhangio/tutor.svg?label=Release%20build&style=flat-square
    :alt: Release build status
    :target: https://travis-ci.org/overhangio/tutor

.. image:: https://img.shields.io/badge/docs-current-blue.svg?style=flat-square
    :alt: Documentation
    :target: https://docs.tutor.overhang.io

.. image:: https://img.shields.io/github/issues/overhangio/tutor.svg?style=flat-square
    :alt: GitHub issues
    :target: https://github.com/overhangio/tutor/issues

.. image:: https://img.shields.io/github/issues-closed/overhangio/tutor.svg?colorB=brightgreen&style=flat-square
    :alt: GitHub closed issues
    :target: https://github.com/overhangio/tutor/issues?q=is%3Aclosed

.. image:: https://img.shields.io/github/license/overhangio/tutor.svg?style=flat-square
    :alt: AGPL License
    :target: https://www.gnu.org/licenses/agpl-3.0.en.html


**Tutor** is a docker-based `Open edX <https://openedx.org>`_ distribution, both for production and local development. The goal of Tutor is to make it easy to deploy, customize, upgrade and scale Open edX. Tutor is reliable, fast, extensible, and it is already used by dozens of Open edX platforms around the world.

Do you need professional assistance setting up or managing your Open edX platform? Overhang.IO provides online support as part of its `Long Term Support (LTS) offering <https://overhang.io/tutor/lts>`__.

Features
--------

* 100% `open source <https://github.com/overhangio/tutor>`__
* Runs entirely on Docker
* World-famous 1-click `installation and upgrades <https://docs.tutor.overhang.io/install.html>`__
* Comes with batteries included: `theming <https://github.com/overhangio/indigo>`__, `SCORM <https://github.com/overhangio/openedx-scorm-xblock>`__, `HTTPS <https://docs.tutor.overhang.io/configuration.html#ssl-tls-certificates-for-https-access>`__, `web-based administration interface <https://docs.tutor.overhang.io/extra.html#web-ui>`__, `mobile app <https://docs.tutor.overhang.io/extra.html#mobile-android-application>`__, `custom translations <https://docs.tutor.overhang.io/configuration.html#adding-custom-translations>`__...
* Extensible architecture with `plugins <https://docs.tutor.overhang.io/plugins.html>`__
* Works with `Kubernetes <https://docs.tutor.overhang.io/k8s.html>`__
* No technical skill required with the `1-click Tutor AWS image <https://docs.tutor.overhang.io/install.html#cloud-deployment>`__
* Professional support and premium plugins available with `Tutor Long Term Support (LTS) <https://overhang.io/tutor/lts>`__

.. _readme_intro_end:

.. image:: ./docs/img/quickstart.gif
    :alt: Tutor local quickstart
    :target: https://terminalizer.com/view/91b0bfdd557

Quickstart
----------

1. Install the `latest stable release <https://github.com/overhangio/tutor/releases>`_ of Tutor
2. Run ``tutor local quickstart``
3. You're done!

Documentation
-------------

Extensive documentation is available online: https://docs.tutor.overhang.io/

.. _readme_support_start:

Support
-------

To get community support, go to the official discussion forums: https://discuss.overhang.io. For official support, please subscribe to a Long Term Support (LTS) license at https://overhang.io/tutor/lts.

.. _readme_support_end:

.. _readme_contributing_start:

Contributing
------------

We are very much open to new ideas and features for Tutor. If you have an improvement idea, feel free to first discuss it on the `Tutor forums <https://discuss.overhang.io>`_. If you are not quite familiar with Open edX or if you need technical advice, the forums are a great place to start, too. Did you find an issue with Tutor? Please first make sure that it's related to Tutor, and not an upstream issue with Open edX. Then, `open an issue on Github <https://github.com/overhangio/tutor/issues/new/choose>`_. `Pull requests <https://github.com/overhangio/tutor/pulls>`_ will be happily examined, too!

.. _readme_contributing_end:
