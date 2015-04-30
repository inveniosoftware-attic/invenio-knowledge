===================
 Invenio Knowledge
===================

.. image:: https://img.shields.io/coveralls/coagulant/coveralls-python.svg
        :target: https://coveralls.io/r/inveniosoftware/invenio-knowledge

.. image:: https://travis-ci.org/inveniosoftware/invenio-knowledge.png?branch=master
        :target: https://travis-ci.org/inveniosoftware/invenio-knowledge

.. image:: https://pypip.in/d/invenio-knowledge/badge.png
        :target: https://pypi.python.org/pypi/invenio-knowledge


Invenio module that adds support for knowledge base storage.

The Knowledge module provides tools for cataloguers to manage "knowledge bases",
"authority files" and "ontologies".
Knowledge contains information for standardisation and record quality checking.

Typical examples:

1. Field author institute is often written as "Odd University Strange Research
   Lab" though it is officially (canonically) known as "StrangeLab of the Odd
   University".
2. If field "author email" contains "@strange.odd.edu" the author institute
   should be "StrangeLab of the Odd University".
3. Ontology files contain information about the hierarchy of key words.

There are three four types of knowledge bases:

1. "map_from" "map_to": this is the typical case, the knowledge base is
   essentially a list of left side - right side pairs.
   Like "Genf" -> "Geneva" or "Odd University Strange Research Lab" ->
   "StrangeLab of the Odd University".
   The abbreviation for this type is kbr (for reference).
2. "authority only": this kind of knowledge base only lists the canonical
   values.
   Example: "Geneva", "StrangeLab of the Odd University".
   It is a special case of "map_from" "map_to", where left side and right side
   are identical.
   The abbreviation for this type is kba (for authority).
3. "dynamic": these knowledge bases are "authority only" knowledge bases that
   are built dynamically using a search expression.
   Example: if the author institute is stored in field 100__u, a dynamic
   knowledge base that uses this field, returns all the values of 100__u.
   The abbreviation for this type is kbd (for dynamic).
4. "taxonomy" (or ontology): an RDF (resource description framework) file can
   be uploaded into invenio and used as a knowledge base.

* Free software: GPLv2 license
* Documentation: https://invenio-knowledge.readthedocs.org.

Features
--------

- dynamic knowledge bases
- REST API
