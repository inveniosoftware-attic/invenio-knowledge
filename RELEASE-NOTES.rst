==========================
 Invenio-Knowledge v0.1.1
==========================

Invenio-Knowledge v0.1.1 was released on October 7, 2015.

About
-----

Invenio module for knowledge base management.

*This is an experimental development preview release.*

Incompatible changes
--------------------

- Removes legacy upgrade recipes. You **MUST** upgrade to the latest
  Invenio 2.1 before upgrading Invenio-Upgrader.

Bug fixes
---------

- Removes dependencies to invenio.testsuite and replaces them with
  invenio_testing.
- Removes calls to PluginManager consider_setuptools_entrypoints()
  removed in PyTest 2.8.0.
- Adds missing `invenio_base` dependency.

Installation
------------

   $ pip install invenio-knowledge==0.1.1

Documentation
-------------

   http://invenio-knowledge.readthedocs.org/en/v0.1.1

Happy hacking and thanks for flying Invenio-Knowledge.

| Invenio Development Team
|   Email: info@invenio-software.org
|   IRC: #invenio on irc.freenode.net
|   Twitter: http://twitter.com/inveniosoftware
|   GitHub: https://github.com/inveniosoftware/invenio-knowledge
|   URL: http://invenio-software.org
