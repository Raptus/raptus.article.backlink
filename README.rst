Introduction
============

raptus.article.backlink provides support for adding a back link to articles.

The following features for raptus.article are provided by this package:

Components
----------
    * raptus.article.backlink

Dependencies
------------
    * raptus.article.core
    * raptus.backlink

Installation
============

To install raptus.article.backlink into your Plone instance, locate the file
buildout.cfg in the root of your Plone instance directory on the file system,
and open it in a text editor.

Add the actual raptus.article.backlink add-on to the "eggs" section of
buildout.cfg. Look for the section that looks like this::

    eggs =
        Plone

This section might have additional lines if you have other add-ons already
installed. Just add the raptus.article.teaser on a separate line, like this::

    eggs =
        Plone
        raptus.article.backlink

Note that you have to run buildout like this::

    $ bin/buildout

Then go to the "Add-ons" control panel in Plone as an administrator, and
install or reinstall the "raptus.article.default" product.

Note that if you do not use the raptus.article.default package you have to
include the zcml of raptus.article.teaser either by adding it
to the zcml list in your buildout or by including it in another package's
configure.zcml.

Usage
=====

Components
----------
Navigate to the "Components" tab of your article, select the backlink component
and press "save and view".

Copyright and credits
=====================

raptus.article is copyrighted by `Raptus AG <http://raptus.com>`_ and licensed under the GPL. 
See LICENSE.txt for details.
