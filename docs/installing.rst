Installation
============

Install the package (or add it to your ``requirements.txt`` file):

.. code:: console

    $ pip install sphinx_govbr_theme

In your ``conf.py`` file:

.. code:: python

    import sphinx_govbr_theme

    extensions = [
        ...
        'sphinx_govbr_theme',
    ]

    html_theme = "sphinx_govbr_theme"

.. seealso::
    :ref:`supported-browsers`
        Officially supported and tested browser/operating system combinations

    :ref:`supported-dependencies`
        Officially Supported versions of Python, Sphinx, and other dependencies.

.. note::

   Adding this theme as an extension is what enables localization of theme
   strings in your translated output. If these strings are not translated in
   your output, either we lack the localized strings for your locale, or you
   are using an old version of the theme.

Via Git or Download
-------------------

.. warning::

   Installing directly from the repository source is deprecated and is not
   recommended. Static assets won't be included in the repository starting in
   release :ref:`3.0.0`.

Symlink or subtree the ``sphinx_govbr_theme/sphinx_govbr_theme`` repository into your documentation at
``docs/_themes/sphinx_govbr_theme`` then add the following two settings to your Sphinx
``conf.py`` file:

.. code:: python

    html_theme = "sphinx_govbr_theme"
    html_theme_path = ["_themes", ]
