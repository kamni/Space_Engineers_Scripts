#######################
Space Engineers Scripts
#######################

Scripts I've written for the Space Engineers in-game API.
Many are incorporated into the ships I build.

Check out my Steam Workshop page:
`SJ_Omega <https://steamcommunity.com/profiles/76561198025391137/myworkshopfiles/>`_

Documentation for the scripts is hosted on `Github Pages`_.


***********
Development
***********

Docs
====

The documentation for these projects is located in the ``docs`` folder
and is generated using `Sphinx <https://www.sphinx-doc.org>`_.

To install Sphinx with Python 3:

.. code:: shell

   python3 -m venv .venv
   source .venv/bin/activate
   pip install sphinx==8.1.3 sphinx-rtd-theme==3.0.2

The `RST <https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html>`_
files are located in ``docs/source``.
To build the documentation:

.. code:: shell

   sphinx-build -M html docs/source/ docs/build/
   cp -r docs/build/* docs/

After you push the docs to github, they should be available as
`Github Pages`_.

.. _Github Pages: https://madbillyblack.github.io/Space_Engineers_Scripts/
