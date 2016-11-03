=====================
diazotheme.bootswatch
=====================


Introduction
============

``diazotheme.bootswatch`` is a collection of Diazo themes meant to serve as parent themes. 
Most of these themes are molding the plone html into a framework compliant html.

The "plone" theme is the exception to the rule. As a theme it adds html 
structures to the plone sunburst theme. It also contains a lot of utilities, 
like different colors and sizes of the plone logo and icons, and more.

This package provides diazo themes based on many *CSS framework* using the **theming** and 
**packaging** features available for create Diazo_ theme using `plone.app.theming`_.

``diazotheme.bootswatch`` package contains the following css framework implementations: 

- `Twitter Bootstrap CSS framework`_.


Extending
=========


How to create a child theme
---------------------------

Any of the themes folders can be used to create your own child theme, 
based on `diazotheme.bootswatch`_. You can either wrap the theme up in a package 
or you can create a zip file of the folder and upload that to the theme panel.

There are two ways of creating a child theme.


The package way
^^^^^^^^^^^^^^^

For this example, lets assume we are creating a package called
``diazotheme.newtheme`` and we will copy the ``bootstrap`` theme in this 
package.

1. Created the ``diazotheme.newtheme`` package (for instance through ``paster`` script).

2. Copy ``diazotheme.bootswatch/diazotheme/bootswatch/bootstrap`` to
   ``diazotheme.newtheme/diazotheme/newtheme/static`` (arbitrary
   name).

3. Remove ``diazotheme.bootswatch/diazotheme/bootswatch/bootstrap/examples`` directory.

4. Add `<plone:static directory="static" name="newtheme" type="theme"/>`
   to ``diazotheme.newtheme/diazotheme/newtheme/configure.zcml``.

5. Change ``diazotheme.newtheme/diazotheme/newtheme/static/manifest.cfg``
   to reflect the changes, so: ::

        [theme]
        title = New theme
        description = Describe the new theme
        rules = /++theme++newtheme/rules.xml
        prefix = /++theme++newtheme
        doctype = <!DOCTYPE html>
        preview = preview.png


The zip file way
^^^^^^^^^^^^^^^^

Again, lets assume we use the ``bootstrap`` theme and we want to end up
with the ``newtheme`` name.

1. Copy ``diazotheme.bootswatch/diazotheme/bootswatch/bootstrap`` to your file system.

2. Rename ``bootstrap`` to ``newtheme`` (the folder name will become the
   theme name in the theme panel)

3. Remove ``diazotheme.bootswatch/diazotheme/bootswatch/bootstrap/examples`` directory.

4. Change ``newtheme/manifest.cfg``
   to reflect the changes, so: ::

        [theme]
        title = New theme
        description = Describe the new theme
        rules = /++theme++newtheme/rules.xml
        prefix = /++theme++newtheme
        doctype = <!DOCTYPE html>
        preview = preview.png

4. Customize your theme.

5. When you are finished customizing, create a zip archive of the 
   ``newtheme`` folder.

6. Upload the ``newtheme.zip`` in the plone theme panel.


Screenshots
===========

Bootswatch Amelia Theme
-----------------------

Layout of the site when viewed in a computer resolution:

.. image:: https://github.com/collective/diazotheme.bootswatch/raw/master/diazotheme/bootswatch/amelia/preview.png
  :alt: Bootswatch Amelia Theme
  :align: center


Bootswatch Amelia Narrow Theme
------------------------------

Layout of the site when viewed in a computer resolution:

.. image:: https://github.com/collective/diazotheme.bootswatch/raw/master/diazotheme/bootswatch/amelia-narrow/preview.png
  :alt: Bootswatch Amelia Narrow Theme
  :align: center


Bootswatch Cerulean Theme
-------------------------

Layout of the site when viewed in a computer resolution:

.. image:: https://github.com/collective/diazotheme.bootswatch/raw/master/diazotheme/bootswatch/cerulean/preview.png
  :alt: Bootswatch Cerulean Theme
  :align: center


Bootswatch Cerulean Narrow Theme
--------------------------------

Layout of the site when viewed in a computer resolution:

.. image:: https://github.com/collective/diazotheme.bootswatch/raw/master/diazotheme/bootswatch/cerulean-narrow/preview.png
  :alt: Bootswatch Cerulean Narrow Theme
  :align: center


Bootswatch Cosmo Theme
----------------------

Layout of the site when viewed in a computer resolution:

.. image:: https://github.com/collective/diazotheme.bootswatch/raw/master/diazotheme/bootswatch/cosmo/preview.png
  :alt: Bootswatch Cosmo Theme
  :align: center


Bootswatch Cosmo Narrow Theme
-----------------------------

Layout of the site when viewed in a computer resolution:

.. image:: https://github.com/collective/diazotheme.bootswatch/raw/master/diazotheme/bootswatch/cosmo-narrow/preview.png
  :alt: Bootswatch Cosmo Narrow Theme
  :align: center


Bootswatch Cyborg Theme
-----------------------

Layout of the site when viewed in a computer resolution:

.. image:: https://github.com/collective/diazotheme.bootswatch/raw/master/diazotheme/bootswatch/cyborg/preview.png
  :alt: Bootswatch Cyborg Theme
  :align: center


Bootswatch Cyborg Narrow Theme
------------------------------

Layout of the site when viewed in a computer resolution:

.. image:: https://github.com/collective/diazotheme.bootswatch/raw/master/diazotheme/bootswatch/cyborg-narrow/preview.png
  :alt: Bootswatch Cyborg Narrow Theme
  :align: center


Bootswatch Journal Theme
------------------------

Layout of the site when viewed in a computer resolution:

.. image:: https://github.com/collective/diazotheme.bootswatch/raw/master/diazotheme/bootswatch/journal/preview.png
  :alt: Bootswatch Journal Theme
  :align: center


Bootswatch Journal Narrow Theme
-------------------------------

Layout of the site when viewed in a computer resolution:

.. image:: https://github.com/collective/diazotheme.bootswatch/raw/master/diazotheme/bootswatch/journal-narrow/preview.png
  :alt: Bootswatch Journal Narrow Theme
  :align: center


Bootswatch Readable Theme
-------------------------

Layout of the site when viewed in a computer resolution:

.. image:: https://github.com/collective/diazotheme.bootswatch/raw/master/diazotheme/bootswatch/readable/preview.png
  :alt: Bootswatch Readable Theme
  :align: center


Bootswatch Readable Narrow Theme
--------------------------------

Layout of the site when viewed in a computer resolution:

.. image:: https://github.com/collective/diazotheme.bootswatch/raw/master/diazotheme/bootswatch/readable-narrow/preview.png
  :alt: Bootswatch Readable Narrow Theme
  :align: center


Bootswatch Simplex Theme
------------------------

Layout of the site when viewed in a computer resolution:

.. image:: https://github.com/collective/diazotheme.bootswatch/raw/master/diazotheme/bootswatch/simplex/preview.png
  :alt: Bootswatch Simplex Theme
  :align: center


Bootswatch Simple Narrow Theme
------------------------------

Layout of the site when viewed in a computer resolution:

.. image:: https://github.com/collective/diazotheme.bootswatch/raw/master/diazotheme/bootswatch/simplex-narrow/preview.png
  :alt: Bootswatch Simple Narrow Theme
  :align: center


Bootswatch Slate Theme
----------------------

Layout of the site when viewed in a computer resolution:

.. image:: https://github.com/collective/diazotheme.bootswatch/raw/master/diazotheme/bootswatch/slate/preview.png
  :alt: Bootswatch Slate Theme
  :align: center


Bootswatch Slate Narrow Theme
-----------------------------

Layout of the site when viewed in a computer resolution:

.. image:: https://github.com/collective/diazotheme.bootswatch/raw/master/diazotheme/bootswatch/slate-narrow/preview.png
  :alt: Bootswatch Slate Narrow Theme
  :align: center


Bootswatch Spacelab Theme
-------------------------

Layout of the site when viewed in a computer resolution:

.. image:: https://github.com/collective/diazotheme.bootswatch/raw/master/diazotheme/bootswatch/spacelab/preview.png
  :alt: Bootswatch Spacelab Theme
  :align: center


Bootswatch Spacelab Narrow Theme
--------------------------------

Layout of the site when viewed in a computer resolution:

.. image:: https://github.com/collective/diazotheme.bootswatch/raw/master/diazotheme/bootswatch/spacelab-narrow/preview.png
  :alt: Bootswatch Spacelab Narrow Theme
  :align: center


Bootswatch Spruce Theme
-----------------------

Layout of the site when viewed in a computer resolution:

.. image:: https://github.com/collective/diazotheme.bootswatch/raw/master/diazotheme/bootswatch/spruce/preview.png
  :alt: Bootswatch Spruce Theme
  :align: center


Bootswatch Spruce Narrow Theme
------------------------------

Layout of the site when viewed in a computer resolution:

.. image:: https://github.com/collective/diazotheme.bootswatch/raw/master/diazotheme/bootswatch/spruce-narrow/preview.png
  :alt: Bootswatch Spruce Narrow Theme
  :align: center


Bootswatch Superhero Theme
--------------------------

Layout of the site when viewed in a computer resolution:

.. image:: https://github.com/collective/diazotheme.bootswatch/raw/master/diazotheme/bootswatch/superhero/preview.png
  :alt: Bootswatch Superhero Theme
  :align: center


Bootswatch Superhero Narrow Theme
---------------------------------

Layout of the site when viewed in a computer resolution:

.. image:: https://github.com/collective/diazotheme.bootswatch/raw/master/diazotheme/bootswatch/superhero-narrow/preview.png
  :alt: Bootswatch Superhero Narrow Theme
  :align: center


Bootswatch United Theme
-----------------------

Layout of the site when viewed in a computer resolution:

.. image:: https://github.com/collective/diazotheme.bootswatch/raw/master/diazotheme/bootswatch/united/preview.png
  :alt: Bootswatch United Theme
  :align: center


Bootswatch United Narrow Theme
------------------------------

Layout of the site when viewed in a computer resolution:

.. image:: https://github.com/collective/diazotheme.bootswatch/raw/master/diazotheme/bootswatch/united-narrow/preview.png
  :alt: Bootswatch United Narrow Theme
  :align: center


Requirements
============

- From the Plone 4.1.x To the Plone 4.3 latest version (https://plone.org/download)
- The ``plone.app.theming`` package (*You will need enable it to use this package*)


Features
========

- Provides the diazo rules for *Bootswatch* theme.
- Provides the diazo rules for *Bootswatch Amelia* theme.
- Provides the diazo rules for *Bootswatch Amelia Narrow* theme.
- Provides the diazo rules for *Bootswatch Cerulean* theme.
- Provides the diazo rules for *Bootswatch Cerulean Narrow* theme.
- Provides the diazo rules for *Bootswatch Cosmo* theme.
- Provides the diazo rules for *Bootswatch Cosmo Narrow* theme.
- Provides the diazo rules for *Bootswatch Cyborg* theme.
- Provides the diazo rules for *Bootswatch Cyborg Narrow* theme.
- Provides the diazo rules for *Bootswatch Journal* theme.
- Provides the diazo rules for *Bootswatch Journal Narrow* theme.
- Provides the diazo rules for *Bootswatch Readable* theme.
- Provides the diazo rules for *Bootswatch Readable Narrow* theme.
- Provides the diazo rules for *Bootswatch Simplex* theme.
- Provides the diazo rules for *Bootswatch Simplex Narrow* theme.
- Provides the diazo rules for *Bootswatch Slate* theme.
- Provides the diazo rules for *Bootswatch Slate Narrow* theme.
- Provides the diazo rules for *Bootswatch Spacelab* theme.
- Provides the diazo rules for *Bootswatch Spacelab Narrow* theme.
- Provides the diazo rules for *Bootswatch Spruce* theme.
- Provides the diazo rules for *Bootswatch Spruce Narrow* theme.
- Provides the diazo rules for *Bootswatch Superhero* theme.
- Provides the diazo rules for *Bootswatch Superhero Narrow* theme.
- Provides the diazo rules for *Bootswatch United* theme.
- Provides the diazo rules for *Bootswatch United Narrow* theme.


Installation
============


Buildout
--------

If you are a developer, you might enjoy installing it via buildout.

For install ``diazotheme.bootswatch`` package add it to your ``buildout`` section's 
*eggs* parameter e.g.: ::

   [buildout]
    ...
    eggs =
        ...
        diazotheme.bootswatch


and then running ``bin/buildout``.

Or, you can add it as a dependency on your own product ``setup.py`` file: ::

    install_requires=[
        ...
        'diazotheme.bootswatch',
    ],

Enabling the theme
------------------

To apply any of these themes, in site setup:

- Install "Diazo theme support" under Add-on
- Select "Sunburst Theme" as Default themes under Themes

  To apply the ..., in site setup:
  - Enable "... (...)" under Diazo themes


Resources
=========

This package is the parent of all Plone diazo themes and 
provides rule that are practical to use in other diazo themes.


Bootswatch Theme
----------------

The resources of this theme can be reached through

- **Bootswatch Theme**
    ``/++theme++bootswatch``

There are placed at ``diazotheme.bootswatch/diazotheme/bootswatch/bootswatch`` 
directory with following resources files:

::

    _ bootswatch
      Provides the resources from "Bootswatch Theme".
      _ css
        _ font-awesome.min.css
        _ plone.css
      _ font
        _ fontawesome-webfont.eot
        _ fontawesome-webfont.svg
        _ fontawesome-webfont.fft
        _ fontawesome-webfont.woff
        _ FontAwesome.otf
      _ rules
        _ head-base.xml


Bootswatch Amelia
-----------------

The resources of this theme can be reached through

- **Bootswatch Amelia Theme**
    ``/++theme++amelia``

There are placed at ``diazotheme.bootswatch/diazotheme/bootswatch/bootstrap/amelia`` 
directory with following resources files:

::

    _ amelia
      Provides the resources from "Bootswatch Amelia".
      _ css
        _ bootstrap.css
        _ bootstrap.min.css
      _ manifest.cfg
      _ preview.png
      _ rules.xml


Bootswatch Amelia Narrow
------------------------

The resources of this theme can be reached through

- **Bootswatch Amelia Narrow Theme**
    ``/++theme++amelia-narrow``

There are placed at ``diazotheme.bootswatch/diazotheme/bootswatch/bootstrap/amelia-narrow`` 
directory with following resources files:

::

    _ amelia-narrow
      Provides the resources from "Bootswatch Amelia Narrow".
      _ manifest.cfg
      _ preview.png
      _ rules.xml


Bootswatch Cerulean
-------------------

The resources of this theme can be reached through

- **Bootswatch Cerulean Theme**
    ``/++theme++cerulean``

There are placed at ``diazotheme.bootswatch/diazotheme/bootswatch/bootstrap/cerulean`` 
directory with following resources files:

::

    _ cerulean
      Provides the resources from "Bootswatch Cerulean".
      _ css
        _ bootstrap.css
        _ bootstrap.min.css
      _ manifest.cfg
      _ preview.png
      _ rules.xml


Bootswatch Cerulean Narrow
--------------------------

The resources of this theme can be reached through

- **Bootswatch Cerulean Narrow Theme**
    ``/++theme++cerulean-narrow``

There are placed at ``diazotheme.bootswatch/diazotheme/bootswatch/bootstrap/cerulean-narrow`` 
directory with following resources files:

::

    _ cerulean-narrow
      Provides the resources from "Bootswatch Cerulean Narrow".
      _ manifest.cfg
      _ preview.png
      _ rules.xml


Bootswatch Cosmo
----------------

The resources of this theme can be reached through

- **Bootswatch Cosmo Theme**
    ``/++theme++cosmo``

There are placed at ``diazotheme.bootswatch/diazotheme/bootswatch/bootstrap/cosmo`` 
directory with following resources files:

::

    _ cosmo
      Provides the resources from "Bootswatch Cosmo".
      _ css
        _ bootstrap.css
        _ bootstrap.min.css
      _ manifest.cfg
      _ preview.png
      _ rules.xml


Bootswatch Cosmo Narrow
-----------------------

The resources of this theme can be reached through

- **Bootswatch Cosmo Narrow Theme**
    ``/++theme++cosmo-narrow``

There are placed at ``diazotheme.bootswatch/diazotheme/bootswatch/bootstrap/cosmo-narrow`` 
directory with following resources files:

::

    _ cosmo-narrow
      Provides the resources from "Bootswatch Cosmo Narrow".
      _ manifest.cfg
      _ preview.png
      _ rules.xml


Bootswatch Cyborg
-----------------

The resources of this theme can be reached through

- **Bootswatch Cyborg Theme**
    ``/++theme++cyborg``

There are placed at ``diazotheme.bootswatch/diazotheme/bootswatch/bootstrap/cyborg`` 
directory with following resources files:

::

    _ cyborg
      Provides the resources from "Bootswatch Cyborg".
      _ css
        _ bootstrap.css
        _ bootstrap.min.css
      _ manifest.cfg
      _ preview.png
      _ rules.xml


Bootswatch Cyborg Narrow
------------------------

The resources of this theme can be reached through

- **Bootswatch Cyborg Narrow Theme**
    ``/++theme++cyborg-narrow``

There are placed at ``diazotheme.bootswatch/diazotheme/bootswatch/bootstrap/cyborg-narrow`` 
directory with following resources files:

::

    _ cyborg-narrow
      Provides the resources from "Bootswatch Cyborg Narrow".
      _ manifest.cfg
      _ preview.png
      _ rules.xml


Bootswatch Journal
------------------

The resources of this theme can be reached through

- **Bootswatch Journal Theme**
    ``/++theme++journal``

There are placed at ``diazotheme.bootswatch/diazotheme/bootswatch/bootstrap/journal`` 
directory with following resources files:

::

    _ journal
      Provides the resources from "Bootswatch Journal".
      _ css
        _ bootstrap.css
        _ bootstrap.min.css
      _ manifest.cfg
      _ preview.png
      _ rules.xml


Bootswatch Journal Narrow
-------------------------

The resources of this theme can be reached through

- **Bootswatch Journal Narrow Theme**
    ``/++theme++journal-narrow``

There are placed at ``diazotheme.bootswatch/diazotheme/bootswatch/bootstrap/journal-narrow`` 
directory with following resources files:

::

    _ journal-narrow
      Provides the resources from "Bootswatch Journal Narrow".
      _ manifest.cfg
      _ preview.png
      _ rules.xml


Bootswatch Readable
-------------------

The resources of this theme can be reached through

- **Bootswatch Readable Theme**
    ``/++theme++readable``

There are placed at ``diazotheme.bootswatch/diazotheme/bootswatch/bootstrap/readable`` 
directory with following resources files:

::

    _ readable
      Provides the resources from "Bootswatch Readable".
      _ css
        _ bootstrap.css
        _ bootstrap.min.css
      _ manifest.cfg
      _ preview.png
      _ rules.xml


Bootswatch Readable Narrow
--------------------------

The resources of this theme can be reached through

- **Bootswatch Readable Narrow Theme**
    ``/++theme++readable-narrow``

There are placed at ``diazotheme.bootswatch/diazotheme/bootswatch/bootstrap/readable-narrow`` 
directory with following resources files:

::

    _ readable-narrow
      Provides the resources from "Bootswatch Readable Narrow".
      _ manifest.cfg
      _ preview.png
      _ rules.xml


Bootswatch Simplex
------------------

The resources of this theme can be reached through

- **Bootswatch Simplex Theme**
    ``/++theme++simplex``

There are placed at ``diazotheme.bootswatch/diazotheme/bootswatch/bootstrap/simplex`` 
directory with following resources files:

::

    _ simplex
      Provides the resources from "Bootswatch Simplex".
      _ css
        _ bootstrap.css
        _ bootstrap.min.css
      _ manifest.cfg
      _ preview.png
      _ rules.xml


Bootswatch Simplex Narrow
-------------------------

The resources of this theme can be reached through

- **Bootswatch Simplex Narrow Theme**
    ``/++theme++simplex-narrow``

There are placed at ``diazotheme.bootswatch/diazotheme/bootswatch/bootstrap/simplex-narrow`` 
directory with following resources files:

::

    _ simplex-narrow
      Provides the resources from "Bootswatch Simplex Narrow".
      _ manifest.cfg
      _ preview.png
      _ rules.xml


Bootswatch Slate
----------------

The resources of this theme can be reached through

- **Bootswatch Slate Theme**
    ``/++theme++slate``

There are placed at ``diazotheme.bootswatch/diazotheme/bootswatch/bootstrap/slate`` 
directory with following resources files:

::

    _ slate
      Provides the resources from "Bootswatch Slate".
      _ css
        _ bootstrap.css
        _ bootstrap.min.css
      _ manifest.cfg
      _ preview.png
      _ rules.xml


Bootswatch Slate Narrow
-----------------------

The resources of this theme can be reached through

- **Bootswatch Slate Narrow Theme**
    ``/++theme++slate-narrow``

There are placed at ``diazotheme.bootswatch/diazotheme/bootswatch/bootstrap/slate-narrow`` 
directory with following resources files:

::

    _ slate-narrow
      Provides the resources from "Bootswatch Slate Narrow".
      _ manifest.cfg
      _ preview.png
      _ rules.xml


Bootswatch Spacelab
-------------------

The resources of this theme can be reached through

- **Bootswatch Spacelab Theme**
    ``/++theme++spacelab``

There are placed at ``diazotheme.bootswatch/diazotheme/bootswatch/bootstrap/spacelab`` 
directory with following resources files:

::

    _ spacelab
      Provides the resources from "Bootswatch Spacelab".
      _ css
        _ bootstrap.css
        _ bootstrap.min.css
      _ manifest.cfg
      _ preview.png
      _ rules.xml


Bootswatch Spacelab Narrow
--------------------------

The resources of this theme can be reached through

- **Bootswatch Spacelab Narrow Theme**
    ``/++theme++spacelab-narrow``

There are placed at ``diazotheme.bootswatch/diazotheme/bootswatch/bootstrap/spacelab-narrow`` 
directory with following resources files:

::

    _ spacelab-narrow
      Provides the resources from "Bootswatch Spacelab Narrow".
      _ manifest.cfg
      _ preview.png
      _ rules.xml


Bootswatch Spruce
-----------------

The resources of this theme can be reached through

- **Bootswatch Spruce Theme**
    ``/++theme++spruce``

There are placed at ``diazotheme.bootswatch/diazotheme/bootswatch/bootstrap/spruce`` 
directory with following resources files:

::

    _ spruce
      Provides the resources from "Bootswatch Spruce".
      _ css
        _ bootstrap.css
        _ bootstrap.min.css
      _ manifest.cfg
      _ preview.png
      _ rules.xml


Bootswatch Spruce Narrow
------------------------

The resources of this theme can be reached through

- **Bootswatch Spruce Narrow Theme**
    ``/++theme++spruce-narrow``

There are placed at ``diazotheme.bootswatch/diazotheme/bootswatch/bootstrap/spruce-narrow`` 
directory with following resources files:

::

    _ spruce-narrow
      Provides the resources from "Bootswatch Spruce Narrow".
      _ manifest.cfg
      _ preview.png
      _ rules.xml


Bootswatch Superhero
--------------------

The resources of this theme can be reached through

- **Bootswatch Superhero Theme**
    ``/++theme++superhero``

There are placed at ``diazotheme.bootswatch/diazotheme/bootswatch/bootstrap/superhero`` 
directory with following resources files:

::

    _ superhero
      Provides the resources from "Bootswatch Superhero".
      _ css
        _ bootstrap.css
        _ bootstrap.min.css
      _ manifest.cfg
      _ preview.png
      _ rules.xml


Bootswatch Superhero Narrow
---------------------------

The resources of this theme can be reached through

- **Bootswatch Superhero Narrow Theme**
    ``/++theme++superhero-narrow``

There are placed at ``diazotheme.bootswatch/diazotheme/bootswatch/bootstrap/superhero-narrow`` 
directory with following resources files:

::

    _ superhero-narrow
      Provides the resources from "Bootswatch Superhero Narrow".
      _ manifest.cfg
      _ preview.png
      _ rules.xml


Bootswatch United
-----------------

The resources of this theme can be reached through

- **Bootswatch United Theme**
    ``/++theme++united``

There are placed at ``diazotheme.bootswatch/diazotheme/bootswatch/bootstrap/united`` 
directory with following resources files:

::

    _ united
      Provides the resources from "Bootswatch United".
      _ css
        _ bootstrap.css
        _ bootstrap.min.css
      _ manifest.cfg
      _ preview.png
      _ rules.xml


Bootswatch United Narrow
------------------------

The resources of this theme can be reached through

- **Bootswatch United Narrow Theme**
    ``/++theme++united-narrow``

There are placed at ``diazotheme.bootswatch/diazotheme/bootswatch/bootstrap/united-narrow`` 
directory with following resources files:

::

    _ united-narrow
      Provides the resources from "Bootswatch United Narrow".
      _ manifest.cfg
      _ preview.png
      _ rules.xml


This is the Bootstrap Theme applied through Diazo.

To apply this theme, in site setup:
- Install "Diazo theme support" under Add-on
- Select "(Unstyles)" as Default themes under Themes
- Enable "Bootstrap Theme (bootstrap)" under Diazo themes


Upgrading
=========

To upgrade the contained themes to the latest version, use the
``upgrade.sh`` script in this directory::

   ./upgrade.sh 2.3.2

where the first argument is the version to upgrade to.  This script
will download the relevant archive, unpack it, and replace the stored
CSS files.

After this, add a change note, and use git to commit and push the updates.

Please note the upgrade script will not create any new themes that
might have been added on Bootswatch. Similarly, any themes that may happen
to have been removed will not be updated. 

Notes
=====

* Because of the way that Bootswatch themes operate with icons (relative 
  URLs, expecting icons to live next to the CSS), the relative
  paths have been modified accordingly.  By default, they look like this::

      ../img/glyphicons-halflings.png

  which refers to "the ``img`` folder next to my parent folder". 
  For a resource like ``++theme++spacelab/css/bootstrap.min.css`` this ends
  up attempting to resolve to
  ``++theme++spacelab/img/glyphicons-halflings.png``. In Plone,
  because the Bootstrap ``img`` folder is kept separate under a different
  theme resource path, this relative URL fails.

  At present, a solution has been to adjust these relative URLs inside
  each theme to look like::

      ../../++theme++bootstrap-framework/img/glyphicons-halflings.png

  This works for the test cases (standard install; virtual hosted; both
  development and production modes), but is somewhat brittle in the fact the
  same directory structure must be maintained for this theme, and for the
  Bootstrap resources.

  The ``upgrade.sh`` script performs this adjustment accordingly.
  
  A more bullet-proof solution is welcomed, if possible.  Note that using
  an absolute path (being a ``/`` at the start of the path) is not workable
  since Plone sites can be virtual hosted on different paths.


Contribute
==========

- Issue Tracker: https://github.com/collective/diazotheme.bootswatch/issues
- Source Code: https://github.com/collective/diazotheme.bootswatch


License
=======

The project is licensed under the GPLv2.


Credits
-------

- Thijs Jonkman (t.jonkman at gmail dot com).


Amazing contributions
---------------------

- Leonardo J. Caballero G. aka macagua (leonardocaballero at gmail dot com).

You can find an updated list of package contributors on https://github.com/collective/diazotheme.bootswatch/contributors

.. _`Twitter Bootstrap CSS framework`: http://twitter.github.io/
.. _`diazotheme.bootswatch`: https://github.com/collective/diazotheme.bootswatch
.. _`Diazo`: http://diazo.org
.. _`plone.app.theming`: https://pypi.org/project/plone.app.theming/
