# Comparing `tmp/imio.smartweb.core-1.2.8.tar.gz` & `tmp/imio.smartweb.core-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/imio.smartweb.core-1.2.8.tar", last modified: Thu Nov 23 08:27:28 2023, max compression
+gzip compressed data, was "imio.smartweb.core-1.2.9.tar", last modified: Fri Nov 24 10:12:17 2023, max compression
```

## Comparing `imio.smartweb.core-1.2.8.tar` & `imio.smartweb.core-1.2.9.tar`

### file list

```diff
@@ -1,862 +1,862 @@
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/
--rw-r--r--   0 laurent    (501) staff       (20)    38853 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/CHANGES.rst
--rw-r--r--   0 laurent    (501) staff       (20)      169 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/CONTRIBUTORS.rst
--rw-r--r--   0 laurent    (501) staff       (20)      522 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/DEVELOP.rst
--rw-r--r--   0 laurent    (501) staff       (20)    18092 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/LICENSE.GPL
--rw-r--r--   0 laurent    (501) staff       (20)      653 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/LICENSE.rst
--rw-r--r--   0 laurent    (501) staff       (20)      188 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/MANIFEST.in
--rw-r--r--   0 laurent    (501) staff       (20)    43707 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/PKG-INFO
--rw-r--r--   0 laurent    (501) staff       (20)     3610 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/README.rst
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/docs/
--rw-r--r--   0 laurent    (501) staff       (20)     7994 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/docs/conf.py
--rw-r--r--   0 laurent    (501) staff       (20)       63 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/docs/index.rst
--rw-r--r--   0 laurent    (501) staff       (20)       64 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/requirements.txt
--rw-r--r--   0 laurent    (501) staff       (20)      518 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/setup.cfg
--rw-r--r--   0 laurent    (501) staff       (20)     3010 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/setup.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/
--rw-r--r--   0 laurent    (501) staff       (20)       80 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/__init__.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/
--rw-r--r--   0 laurent    (501) staff       (20)       80 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/__init__.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/
--rw-r--r--   0 laurent    (501) staff       (20)       24 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/__init__.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/behaviors/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/behaviors/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)     1677 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/behaviors/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)      760 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/behaviors/listing.py
--rw-r--r--   0 laurent    (501) staff       (20)     1865 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/behaviors/minisite.py
--rw-r--r--   0 laurent    (501) staff       (20)      557 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/behaviors/orientation.py
--rw-r--r--   0 laurent    (501) staff       (20)     1063 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/behaviors/quickaccess.py
--rw-r--r--   0 laurent    (501) staff       (20)     1707 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/behaviors/subsite.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/__init__.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/banner/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/banner/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)      389 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/banner/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)      947 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/banner/settings.py
--rw-r--r--   0 laurent    (501) staff       (20)     2811 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     5361 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/controlpanel.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/dashboards/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/dashboards/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)      523 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/dashboards/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     1107 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/dashboards/plausible.pt
--rw-r--r--   0 laurent    (501) staff       (20)      651 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/dashboards/plausible.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/faceted/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/faceted/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)     1987 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/faceted/block_view.pt
--rw-r--r--   0 laurent    (501) staff       (20)     3289 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/faceted/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     2951 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/faceted/macros.pt
--rw-r--r--   0 laurent    (501) staff       (20)     4434 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/faceted/map.pt
--rw-r--r--   0 laurent    (501) staff       (20)     1504 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/faceted/map.py
--rw-r--r--   0 laurent    (501) staff       (20)     1931 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/faceted/summary_view.pt
--rw-r--r--   0 laurent    (501) staff       (20)     1460 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/faceted/views.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/faceted/widgets/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/faceted/widgets/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)      449 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/faceted/widgets/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     2459 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/faceted/widgets/select.pt
--rw-r--r--   0 laurent    (501) staff       (20)      221 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/faceted/widgets/select.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/footer/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/footer/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)      388 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/footer/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     2492 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/footer/settings.py
--rw-r--r--   0 laurent    (501) staff       (20)     1089 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/forms.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/herobanner/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/herobanner/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)      400 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/herobanner/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     2884 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/herobanner/settings.py
--rw-r--r--   0 laurent    (501) staff       (20)     2065 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/icons.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/instancebehaviors/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/instancebehaviors/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)      632 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/instancebehaviors/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     3052 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/instancebehaviors/form.py
--rw-r--r--   0 laurent    (501) staff       (20)      742 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/instancebehaviors/utils.py
--rw-r--r--   0 laurent    (501) staff       (20)     2066 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/layout.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/minisite/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/minisite/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)      417 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/minisite/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     2766 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/minisite/settings.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/overrides/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/overrides/.gitkeep
--rw-r--r--   0 laurent    (501) staff       (20)     2111 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/overrides/plone.app.content.browser.contents.templates.properties.pt
--rw-r--r--   0 laurent    (501) staff       (20)      978 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/overrides/plone.app.layout.viewlets.sections.pt
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/search/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/search/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)      423 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/search/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)      450 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/search/search.pt
--rw-r--r--   0 laurent    (501) staff       (20)     2369 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/search/search.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/.gitkeep
--rw-r--r--   0 laurent    (501) staff       (20)      350 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/Makefile
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/
--rw-r--r--   0 laurent    (501) staff       (20)      873 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/action-e-guichet.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      274 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/action-email.svg
--rw-r--r--   0 laurent    (501) staff       (20)     1355 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/action-engagement.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      483 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/action-nous-contacter.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      409 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/action-nous-rejoindre.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      307 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/action-organiser-un-evenement.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      787 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/action-signaler-un-probleme.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      414 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/action-voir-plan.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      313 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/categorie-associations.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      313 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/categorie-avis-et-enquetes.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      458 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/categorie-cinema.svg
--rw-r--r--   0 laurent    (501) staff       (20)     1787 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/categorie-commerce.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      508 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/categorie-concert.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      367 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/categorie-culture.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      426 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/categorie-demarches.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)     1011 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/categorie-enfance.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      673 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/categorie-enseignement.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      252 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/categorie-environnement-gestion-des-dechets.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      284 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/categorie-exposition.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      245 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/categorie-horaires.svg
--rw-r--r--   0 laurent    (501) staff       (20)      453 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/categorie-infos-travaux.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      692 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/categorie-mandataires.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      561 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/categorie-mobilite.svg
--rw-r--r--   0 laurent    (501) staff       (20)      302 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/categorie-mon-dossier.svg
--rw-r--r--   0 laurent    (501) staff       (20)      318 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/categorie-parc-de-stationnement.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      419 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/categorie-parcs-et-jardins.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      662 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/categorie-primes.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      397 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/categorie-sport-courir.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      514 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/categorie-sport-trophee.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      925 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/categorie-sport-velo.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      713 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/categorie-theatre.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      390 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/categorie-tourisme.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      294 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/organisation-academie-musique.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      522 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/organisation-bibliotheque.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      739 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/organisation-centre-sportif.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      879 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/organisation-cpas.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      625 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/organisation-ecole-des-arts.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      302 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/organisation-ecole.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      614 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/organisation-mobilite.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      451 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/organisation-police.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)     2086 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/reseausocial-facebook-pouce.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      421 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/reseausocial-facebook.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)     1999 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/reseausocial-instagram.svg
--rw-r--r--   0 laurent    (501) staff       (20)     1039 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/reseausocial-twitter.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      826 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/reseausocial-vimeo.svg
--rw-r--r--   0 laurent    (501) staff       (20)      542 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/reseausocial-youtube.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      350 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/vue-actualites.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      339 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/vue-agenda.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      497 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/vue-annuaire.svg
--rw-r--r--   0 laurent    (501) staff       (20)      695 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/package.json
--rw-r--r--   0 laurent    (501) staff       (20)      863 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/smartweb-edit-compiled.css
--rw-r--r--   0 laurent    (501) staff       (20)     1137 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/smartweb-edit-compiled.js
--rw-r--r--   0 laurent    (501) staff       (20)      608 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/smartweb-swiperconfig-compiled.js
--rw-r--r--   0 laurent    (501) staff       (20)     2702 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/smartweb-view-compiled.css
--rw-r--r--   0 laurent    (501) staff       (20)     2060 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/smartweb-view-compiled.js
--rw-r--r--   0 laurent    (501) staff       (20)    19615 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/spotlight-bundle.js
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/src/
--rw-r--r--   0 laurent    (501) staff       (20)     1783 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/src/edit.js
--rw-r--r--   0 laurent    (501) staff       (20)     1089 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/src/edit.less
--rw-r--r--   0 laurent    (501) staff       (20)     1285 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/src/swiper-config.js
--rw-r--r--   0 laurent    (501) staff       (20)     2980 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/src/view.js
--rw-r--r--   0 laurent    (501) staff       (20)     2843 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/src/view.less
--rw-r--r--   0 laurent    (501) staff       (20)    17908 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/swiper-bundle.min.css
--rw-r--r--   0 laurent    (501) staff       (20)   137031 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/swiper-bundle.min.js
--rw-r--r--   0 laurent    (501) staff       (20)     1079 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/webpack.config.js
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/subsite/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/subsite/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)      414 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/subsite/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     1601 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/subsite/settings.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/templates/
--rw-r--r--   0 laurent    (501) staff       (20)     2808 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/templates/link_input.pt
--rw-r--r--   0 laurent    (501) staff       (20)     4160 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/utils.py
--rw-r--r--   0 laurent    (501) staff       (20)      337 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/config.py
--rw-r--r--   0 laurent    (501) staff       (20)     1429 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/configure.zcml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/
--rw-r--r--   0 laurent    (501) staff       (20)     3308 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/__init__.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/blocks/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/blocks/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)      732 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/blocks/configure.zcml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/blocks/link/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/blocks/link/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)      552 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/blocks/link/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     1407 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/blocks/link/content.py
--rw-r--r--   0 laurent    (501) staff       (20)      479 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/blocks/link/fields.py
--rw-r--r--   0 laurent    (501) staff       (20)      703 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/blocks/link/icons_input.pt
--rw-r--r--   0 laurent    (501) staff       (20)      330 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/blocks/subscriber.py
--rw-r--r--   0 laurent    (501) staff       (20)      807 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     1465 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/cropping.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/folder/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/folder/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)     1511 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/folder/block_view.pt
--rw-r--r--   0 laurent    (501) staff       (20)     2961 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/folder/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     3377 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/folder/content.py
--rw-r--r--   0 laurent    (501) staff       (20)      342 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/folder/element_view.pt
--rw-r--r--   0 laurent    (501) staff       (20)     1743 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/folder/macros.pt
--rw-r--r--   0 laurent    (501) staff       (20)     1172 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/folder/summary_view.pt
--rw-r--r--   0 laurent    (501) staff       (20)     5682 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/folder/views.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/__init__.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/cirkwi/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/cirkwi/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)      378 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/cirkwi/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)      664 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/cirkwi/content.py
--rw-r--r--   0 laurent    (501) staff       (20)      392 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/cirkwi/view.pt
--rw-r--r--   0 laurent    (501) staff       (20)      482 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/cirkwi/view.py
--rw-r--r--   0 laurent    (501) staff       (20)     2252 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/configure.zcml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/footer/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/footer/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)       70 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/footer/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     1374 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/footer/content.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/herobanner/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/herobanner/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)       70 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/herobanner/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     1077 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/herobanner/content.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/page/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/page/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)       70 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/page/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)      465 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/page/content.py
--rw-r--r--   0 laurent    (501) staff       (20)      464 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/pages.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/portal_page/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/portal_page/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)      352 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/portal_page/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)      336 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/portal_page/content.py
--rw-r--r--   0 laurent    (501) staff       (20)      147 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/portal_page/view.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/procedure/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/procedure/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)      356 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/procedure/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     1297 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/procedure/content.py
--rw-r--r--   0 laurent    (501) staff       (20)     1291 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/procedure/utils.py
--rw-r--r--   0 laurent    (501) staff       (20)      408 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/procedure/view.py
--rw-r--r--   0 laurent    (501) staff       (20)      961 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/subscriber.py
--rw-r--r--   0 laurent    (501) staff       (20)     3127 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/view.pt
--rw-r--r--   0 laurent    (501) staff       (20)     1345 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/view_section.pt
--rw-r--r--   0 laurent    (501) staff       (20)     4852 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/views.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)     2146 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/base.py
--rw-r--r--   0 laurent    (501) staff       (20)      200 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/configure.zcml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/directory/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/directory/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)     1035 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/directory/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     1100 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/directory/content.py
--rw-r--r--   0 laurent    (501) staff       (20)     2962 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/directory/endpoint.py
--rw-r--r--   0 laurent    (501) staff       (20)      750 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/directory/view.pt
--rw-r--r--   0 laurent    (501) staff       (20)      384 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/directory/view.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/events/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/events/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)     1017 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/events/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     1277 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/events/content.py
--rw-r--r--   0 laurent    (501) staff       (20)     2735 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/events/endpoint.py
--rw-r--r--   0 laurent    (501) staff       (20)      751 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/events/view.pt
--rw-r--r--   0 laurent    (501) staff       (20)      375 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/events/view.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/news/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/news/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)     1005 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/news/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)      753 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/news/content.py
--rw-r--r--   0 laurent    (501) staff       (20)     2668 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/news/endpoint.py
--rw-r--r--   0 laurent    (501) staff       (20)      696 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/news/view.pt
--rw-r--r--   0 laurent    (501) staff       (20)      287 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/news/view.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/search/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/search/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)      951 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/search/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     9796 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/search/endpoint.py
--rw-r--r--   0 laurent    (501) staff       (20)      798 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/view.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)     2486 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/base.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/collection/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/collection/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)      920 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/collection/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     2379 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/collection/content.py
--rw-r--r--   0 laurent    (501) staff       (20)     1470 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/collection/views.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/common_templates/
--rw-r--r--   0 laurent    (501) staff       (20)     5393 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/common_templates/carousel.pt
--rw-r--r--   0 laurent    (501) staff       (20)     6402 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/common_templates/table.pt
--rw-r--r--   0 laurent    (501) staff       (20)     2242 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/configure.zcml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/contact/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/contact/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)     1591 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/contact/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     2661 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/contact/content.py
--rw-r--r--   0 laurent    (501) staff       (20)     1387 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/contact/forms.py
--rw-r--r--   0 laurent    (501) staff       (20)     9523 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/contact/macros.pt
--rw-r--r--   0 laurent    (501) staff       (20)    11619 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/contact/utils.py
--rw-r--r--   0 laurent    (501) staff       (20)     1170 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/contact/view.pt
--rw-r--r--   0 laurent    (501) staff       (20)     1422 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/contact/view.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/events/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/events/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)     1117 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/events/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     2914 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/events/content.py
--rw-r--r--   0 laurent    (501) staff       (20)     1522 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/events/macros.pt
--rw-r--r--   0 laurent    (501) staff       (20)     3637 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/events/view.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/external_content/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/external_content/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)      727 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/external_content/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     1096 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/external_content/content.py
--rw-r--r--   0 laurent    (501) staff       (20)     1234 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/external_content/view.pt
--rw-r--r--   0 laurent    (501) staff       (20)     4895 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/external_content/view_arcgis.pt
--rw-r--r--   0 laurent    (501) staff       (20)     8764 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/external_content/views.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/files/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/files/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)      501 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/files/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)      871 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/files/content.py
--rw-r--r--   0 laurent    (501) staff       (20)     1196 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/files/view.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/gallery/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/gallery/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)      424 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/gallery/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)      780 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/gallery/content.py
--rw-r--r--   0 laurent    (501) staff       (20)     2058 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/gallery/view.pt
--rw-r--r--   0 laurent    (501) staff       (20)      451 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/gallery/views.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/html/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/html/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)      413 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/html/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     1352 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/html/content.py
--rw-r--r--   0 laurent    (501) staff       (20)     1140 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/html/view.pt
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/links/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/links/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)      918 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/links/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     1051 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/links/content.py
--rw-r--r--   0 laurent    (501) staff       (20)     1375 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/links/view.py
--rw-r--r--   0 laurent    (501) staff       (20)     4092 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/macros.pt
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/map/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/map/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)      412 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/map/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)      372 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/map/content.py
--rw-r--r--   0 laurent    (501) staff       (20)     1278 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/map/view.pt
--rw-r--r--   0 laurent    (501) staff       (20)      614 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/map/views.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/news/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/news/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)      880 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/news/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     2911 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/news/content.py
--rw-r--r--   0 laurent    (501) staff       (20)     3260 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/news/view.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/postit/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/postit/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)      504 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/postit/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     2239 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/postit/content.py
--rw-r--r--   0 laurent    (501) staff       (20)      936 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/postit/view.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/selections/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/selections/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)      949 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/selections/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     1375 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/selections/content.py
--rw-r--r--   0 laurent    (501) staff       (20)     1510 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/selections/view.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/sendinblue/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/sendinblue/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)      433 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/sendinblue/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     1088 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/sendinblue/content.py
--rw-r--r--   0 laurent    (501) staff       (20)     1180 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/sendinblue/view.pt
--rw-r--r--   0 laurent    (501) staff       (20)     1731 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/sendinblue/views.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/slide/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/slide/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)      417 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/slide/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     2181 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/slide/content.py
--rw-r--r--   0 laurent    (501) staff       (20)     2440 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/slide/view.pt
--rw-r--r--   0 laurent    (501) staff       (20)      784 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/slide/view.py
--rw-r--r--   0 laurent    (501) staff       (20)      642 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/subscriber.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/text/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/text/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)     1257 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/text/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     1118 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/text/content.py
--rw-r--r--   0 laurent    (501) staff       (20)     1818 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/text/forms.py
--rw-r--r--   0 laurent    (501) staff       (20)     1576 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/text/view.pt
--rw-r--r--   0 laurent    (501) staff       (20)      383 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/text/views.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/video/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/video/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)      418 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/video/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)      978 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/video/content.py
--rw-r--r--   0 laurent    (501) staff       (20)     1105 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/video/view.pt
--rw-r--r--   0 laurent    (501) staff       (20)      342 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/video/views.py
--rw-r--r--   0 laurent    (501) staff       (20)     2832 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/views.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/faceted/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/faceted/__init__.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/faceted/config/
--rw-r--r--   0 laurent    (501) staff       (20)     2906 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/faceted/config/collection.xml
--rw-r--r--   0 laurent    (501) staff       (20)      826 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/faceted/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)      395 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/faceted/layout.py
--rw-r--r--   0 laurent    (501) staff       (20)      295 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/faceted/menu.py
--rw-r--r--   0 laurent    (501) staff       (20)     3887 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/indexers.py
--rw-r--r--   0 laurent    (501) staff       (20)      968 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/indexers.zcml
--rw-r--r--   0 laurent    (501) staff       (20)      971 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/interfaces.py
--rw-r--r--   0 laurent    (501) staff       (20)     1777 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/permissions.zcml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/
--rw-r--r--   0 laurent    (501) staff       (20)     5877 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/actions.xml
--rw-r--r--   0 laurent    (501) staff       (20)      179 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/browserlayer.xml
--rw-r--r--   0 laurent    (501) staff       (20)      864 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/catalog.xml
--rw-r--r--   0 laurent    (501) staff       (20)      400 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/controlpanel.xml
--rw-r--r--   0 laurent    (501) staff       (20)     1218 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/metadata.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/registry/
--rw-r--r--   0 laurent    (501) staff       (20)     2562 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/registry/bundles.xml
--rw-r--r--   0 laurent    (501) staff       (20)     1251 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/registry/geolocation.xml
--rw-r--r--   0 laurent    (501) staff       (20)     2400 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/registry/plone.xml
--rw-r--r--   0 laurent    (501) staff       (20)      253 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/registry/smartweb.xml
--rw-r--r--   0 laurent    (501) staff       (20)      183 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/repositorytool.xml
--rw-r--r--   0 laurent    (501) staff       (20)     2726 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/rolemap.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/taxonomies/
--rw-r--r--   0 laurent    (501) staff       (20)      310 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/taxonomies/page_category.cfg
--rw-r--r--   0 laurent    (501) staff       (20)     2059 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/taxonomies/page_category.xml
--rw-r--r--   0 laurent    (501) staff       (20)      320 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/taxonomies/procedure_category.cfg
--rw-r--r--   0 laurent    (501) staff       (20)     3436 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/taxonomies/procedure_category.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/
--rw-r--r--   0 laurent    (501) staff       (20)     1402 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.BlockLink.xml
--rw-r--r--   0 laurent    (501) staff       (20)     1471 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.CirkwiView.xml
--rw-r--r--   0 laurent    (501) staff       (20)     1557 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.DirectoryView.xml
--rw-r--r--   0 laurent    (501) staff       (20)     1542 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.EventsView.xml
--rw-r--r--   0 laurent    (501) staff       (20)     2557 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.Folder.xml
--rw-r--r--   0 laurent    (501) staff       (20)     1730 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.Footer.xml
--rw-r--r--   0 laurent    (501) staff       (20)     1604 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.HeroBanner.xml
--rw-r--r--   0 laurent    (501) staff       (20)     1525 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.NewsView.xml
--rw-r--r--   0 laurent    (501) staff       (20)     2483 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.Page.xml
--rw-r--r--   0 laurent    (501) staff       (20)     2659 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.PortalPage.xml
--rw-r--r--   0 laurent    (501) staff       (20)     2480 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.Procedure.xml
--rw-r--r--   0 laurent    (501) staff       (20)     1506 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionCollection.xml
--rw-r--r--   0 laurent    (501) staff       (20)     1183 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionContact.xml
--rw-r--r--   0 laurent    (501) staff       (20)     1484 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionEvents.xml
--rw-r--r--   0 laurent    (501) staff       (20)     1284 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionExternalContent.xml
--rw-r--r--   0 laurent    (501) staff       (20)     1490 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionFiles.xml
--rw-r--r--   0 laurent    (501) staff       (20)     1349 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionGallery.xml
--rw-r--r--   0 laurent    (501) staff       (20)     1232 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionHTML.xml
--rw-r--r--   0 laurent    (501) staff       (20)     1595 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionLinks.xml
--rw-r--r--   0 laurent    (501) staff       (20)     1142 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionMap.xml
--rw-r--r--   0 laurent    (501) staff       (20)     1478 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionNews.xml
--rw-r--r--   0 laurent    (501) staff       (20)     1129 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionPostit.xml
--rw-r--r--   0 laurent    (501) staff       (20)     1506 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionSelections.xml
--rw-r--r--   0 laurent    (501) staff       (20)     1142 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionSendinblue.xml
--rw-r--r--   0 laurent    (501) staff       (20)     1127 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionSlide.xml
--rw-r--r--   0 laurent    (501) staff       (20)     1241 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionText.xml
--rw-r--r--   0 laurent    (501) staff       (20)     1167 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionVideo.xml
--rw-r--r--   0 laurent    (501) staff       (20)     2040 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types.xml
--rw-r--r--   0 laurent    (501) staff       (20)     1069 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/workflows.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/icons/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/icons/basic/
--rw-r--r--   0 laurent    (501) staff       (20)    17858 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/icons/basic/registry.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/icons/contenttypes/
--rw-r--r--   0 laurent    (501) staff       (20)     8766 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/icons/contenttypes/registry.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/last_compilation/
--rw-r--r--   0 laurent    (501) staff       (20)      852 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/last_compilation/registry.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/testing/
--rw-r--r--   0 laurent    (501) staff       (20)      227 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/testing/metadata.xml
--rw-r--r--   0 laurent    (501) staff       (20)      706 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/testing/registry.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/testing/types/
--rw-r--r--   0 laurent    (501) staff       (20)      517 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/testing/types/Collection.xml
--rw-r--r--   0 laurent    (501) staff       (20)      215 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/testing/types/Document.xml
--rw-r--r--   0 laurent    (501) staff       (20)      213 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/testing/types/Folder.xml
--rw-r--r--   0 laurent    (501) staff       (20)      163 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/testing/types.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/uninstall/
--rw-r--r--   0 laurent    (501) staff       (20)      128 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 laurent    (501) staff       (20)     2028 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles.zcml
--rw-r--r--   0 laurent    (501) staff       (20)      932 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/setuphandlers.py
--rw-r--r--   0 laurent    (501) staff       (20)     3940 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/subscribers.py
--rw-r--r--   0 laurent    (501) staff       (20)     1016 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/subscribers.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     3636 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/testing.py
--rw-r--r--   0 laurent    (501) staff       (20)      172 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/testing.zcml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/__init__.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/
--rw-r--r--   0 laurent    (501) staff       (20)      150 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/cirkwi_bad_widget_mock.html
--rw-r--r--   0 laurent    (501) staff       (20)   333252 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/cirkwi_good_widget_mock.html
--rw-r--r--   0 laurent    (501) staff       (20)      369 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_auth_sources_directory_entity.json
--rw-r--r--   0 laurent    (501) staff       (20)      363 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_auth_sources_events_entity.json
--rw-r--r--   0 laurent    (501) staff       (20)      359 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_auth_sources_news_entity.json
--rw-r--r--   0 laurent    (501) staff       (20)     3454 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_contact_category_raw_mock.json
--rw-r--r--   0 laurent    (501) staff       (20)     4820 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_contact_empty_schedule_raw_mock.json
--rw-r--r--   0 laurent    (501) staff       (20)      771 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_contact_images_raw_mock.json
--rw-r--r--   0 laurent    (501) staff       (20)      156 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_contact_no_image_raw_mock.json
--rw-r--r--   0 laurent    (501) staff       (20)    12224 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_contact_raw_mock.json
--rw-r--r--   0 laurent    (501) staff       (20)      921 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_contacts_raw_mock.json
--rw-r--r--   0 laurent    (501) staff       (20)      749 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_directory_entities_raw_mock.json
--rw-r--r--   0 laurent    (501) staff       (20)      769 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_events_agendas_raw_mock.json
--rw-r--r--   0 laurent    (501) staff       (20)      441 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_events_entities_raw_mock.json
--rw-r--r--   0 laurent    (501) staff       (20)      390 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_events_types_raw_mock.json
--rw-r--r--   0 laurent    (501) staff       (20)      726 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_news_entities_raw_mock.json
--rw-r--r--   0 laurent    (501) staff       (20)      783 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_news_newsfolder_raw_mock.json
--rw-r--r--   0 laurent    (501) staff       (20)      127 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_no_contact_raw_mock.json
--rw-r--r--   0 laurent    (501) staff       (20)      168 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_no_newsfolder_raw_mock.json
--rw-r--r--   0 laurent    (501) staff       (20)     3217 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_procedures_raw_mock.json
--rw-r--r--   0 laurent    (501) staff       (20)    42421 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_rest_directory.json
--rw-r--r--   0 laurent    (501) staff       (20)    46365 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_rest_events.json
--rw-r--r--   0 laurent    (501) staff       (20)     5002 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_rest_events_with_breadcrumbs.json
--rw-r--r--   0 laurent    (501) staff       (20)    45966 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_rest_news.json
--rw-r--r--   0 laurent    (501) staff       (20)     1107 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_rest_specific_events.json
--rw-r--r--   0 laurent    (501) staff       (20)     2064 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_rest_specific_news.json
--rw-r--r--   0 laurent    (501) staff       (20)      369 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_search_one_news_entity.json
--rw-r--r--   0 laurent    (501) staff       (20)      205 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_used_iam_vocabularies_jobseeker_tourist.json
--rw-r--r--   0 laurent    (501) staff       (20)    24753 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/plone.png
--rw-r--r--   0 laurent    (501) staff       (20)     3823 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/plone.svg
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/robot/
--rw-r--r--   0 laurent    (501) staff       (20)     2596 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/robot/test_ct_folder.robot
--rw-r--r--   0 laurent    (501) staff       (20)     2548 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/robot/test_ct_page.robot
--rw-r--r--   0 laurent    (501) staff       (20)     2712 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/robot/test_ct_procedure.robot
--rw-r--r--   0 laurent    (501) staff       (20)     2003 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/robot/test_example.robot
--rw-r--r--   0 laurent    (501) staff       (20)     7838 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_banner.py
--rw-r--r--   0 laurent    (501) staff       (20)     5950 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_behaviors.py
--rw-r--r--   0 laurent    (501) staff       (20)     2012 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_categories.py
--rw-r--r--   0 laurent    (501) staff       (20)     1161 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_chatbot.py
--rw-r--r--   0 laurent    (501) staff       (20)     4921 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_cirkwiview.py
--rw-r--r--   0 laurent    (501) staff       (20)     6500 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_cropping.py
--rw-r--r--   0 laurent    (501) staff       (20)    12109 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_default_pages.py
--rw-r--r--   0 laurent    (501) staff       (20)     5994 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_faceted.py
--rw-r--r--   0 laurent    (501) staff       (20)    13527 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_folder.py
--rw-r--r--   0 laurent    (501) staff       (20)    10970 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_footer.py
--rw-r--r--   0 laurent    (501) staff       (20)     5940 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_herobanner.py
--rw-r--r--   0 laurent    (501) staff       (20)     2788 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_icons.py
--rw-r--r--   0 laurent    (501) staff       (20)    10784 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_indexes.py
--rw-r--r--   0 laurent    (501) staff       (20)     4274 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_instance_behaviors.py
--rw-r--r--   0 laurent    (501) staff       (20)     4997 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_local_roles.py
--rw-r--r--   0 laurent    (501) staff       (20)     2425 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_logo.py
--rw-r--r--   0 laurent    (501) staff       (20)    16640 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_minisite.py
--rw-r--r--   0 laurent    (501) staff       (20)     6799 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_navigation.py
--rw-r--r--   0 laurent    (501) staff       (20)    10699 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_page.py
--rw-r--r--   0 laurent    (501) staff       (20)     3229 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_plausibleview.py
--rw-r--r--   0 laurent    (501) staff       (20)     7215 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_portal_page.py
--rw-r--r--   0 laurent    (501) staff       (20)     6474 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_procedure.py
--rw-r--r--   0 laurent    (501) staff       (20)    14609 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_rest.py
--rw-r--r--   0 laurent    (501) staff       (20)      926 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_robot.py
--rw-r--r--   0 laurent    (501) staff       (20)     2182 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_search.py
--rw-r--r--   0 laurent    (501) staff       (20)    23198 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_section_contact.py
--rw-r--r--   0 laurent    (501) staff       (20)     6690 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_section_events.py
--rw-r--r--   0 laurent    (501) staff       (20)     6872 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_section_external_content.py
--rw-r--r--   0 laurent    (501) staff       (20)     6804 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_section_news.py
--rw-r--r--   0 laurent    (501) staff       (20)     2661 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_section_sendinblue.py
--rw-r--r--   0 laurent    (501) staff       (20)    23691 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_sections.py
--rw-r--r--   0 laurent    (501) staff       (20)     2092 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_setup.py
--rw-r--r--   0 laurent    (501) staff       (20)     3046 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_social.py
--rw-r--r--   0 laurent    (501) staff       (20)     9016 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_subsite.py
--rw-r--r--   0 laurent    (501) staff       (20)     4652 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_text.py
--rw-r--r--   0 laurent    (501) staff       (20)     3823 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_toolbar.py
--rw-r--r--   0 laurent    (501) staff       (20)     4125 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_utils.py
--rw-r--r--   0 laurent    (501) staff       (20)    14234 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_vocabularies.py
--rw-r--r--   0 laurent    (501) staff       (20)     2374 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/utils.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)    23756 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/configure.zcml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1015_to_1016/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1015_to_1016/registry/
--rw-r--r--   0 laurent    (501) staff       (20)      481 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1015_to_1016/registry/e-guichet-icon.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1016_to_1017/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1016_to_1017/registry/
--rw-r--r--   0 laurent    (501) staff       (20)      478 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1016_to_1017/registry/shop-icon.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1020_to_1021/
--rw-r--r--   0 laurent    (501) staff       (20)      538 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1020_to_1021/rolemap.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1020_to_1021/types/
--rw-r--r--   0 laurent    (501) staff       (20)      244 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1020_to_1021/types/imio.smartweb.SectionHTML.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1021_to_1022/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1021_to_1022/registry/
--rw-r--r--   0 laurent    (501) staff       (20)      457 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1021_to_1022/registry/hero-banner.xml
--rw-r--r--   0 laurent    (501) staff       (20)      298 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1021_to_1022/rolemap.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1022_to_1023/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1022_to_1023/registry/
--rw-r--r--   0 laurent    (501) staff       (20)      838 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1022_to_1023/registry/icons.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1023_to_1024/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1023_to_1024/types/
--rw-r--r--   0 laurent    (501) staff       (20)      306 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1023_to_1024/types/imio.smartweb.Page.xml
--rw-r--r--   0 laurent    (501) staff       (20)      312 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1023_to_1024/types/imio.smartweb.PortalPage.xml
--rw-r--r--   0 laurent    (501) staff       (20)      311 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1023_to_1024/types/imio.smartweb.Procedure.xml
--rw-r--r--   0 laurent    (501) staff       (20)     1157 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1023_to_1024/types/imio.smartweb.SectionPostit.xml
--rw-r--r--   0 laurent    (501) staff       (20)      180 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1023_to_1024/types.xml
--rw-r--r--   0 laurent    (501) staff       (20)      173 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1023_to_1024/workflows.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1025_to_1026/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1025_to_1026/registry/
--rw-r--r--   0 laurent    (501) staff       (20)      249 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1025_to_1026/registry/propose-urls.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1027_to_1028/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1027_to_1028/registry/
--rw-r--r--   0 laurent    (501) staff       (20)      318 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1027_to_1028/registry/open-external-link-in-new-tab.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1029_to_1030/
--rw-r--r--   0 laurent    (501) staff       (20)      463 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1029_to_1030/actions.xml
--rw-r--r--   0 laurent    (501) staff       (20)      256 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1029_to_1030/rolemap.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1030_to_1031/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1030_to_1031/registry/
--rw-r--r--   0 laurent    (501) staff       (20)     1425 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1030_to_1031/registry/resources.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1031_to_1032/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1031_to_1032/registry/
--rw-r--r--   0 laurent    (501) staff       (20)      562 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1031_to_1032/registry/spotlight.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/
--rw-r--r--   0 laurent    (501) staff       (20)      257 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.BlockLink.xml
--rw-r--r--   0 laurent    (501) staff       (20)      252 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.DirectoryView.xml
--rw-r--r--   0 laurent    (501) staff       (20)      252 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.EventsView.xml
--rw-r--r--   0 laurent    (501) staff       (20)      241 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.Folder.xml
--rw-r--r--   0 laurent    (501) staff       (20)      250 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.Footer.xml
--rw-r--r--   0 laurent    (501) staff       (20)      247 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.HeroBanner.xml
--rw-r--r--   0 laurent    (501) staff       (20)      245 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.NewsView.xml
--rw-r--r--   0 laurent    (501) staff       (20)      244 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.Page.xml
--rw-r--r--   0 laurent    (501) staff       (20)      256 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.PortalPage.xml
--rw-r--r--   0 laurent    (501) staff       (20)      256 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.Procedure.xml
--rw-r--r--   0 laurent    (501) staff       (20)      255 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionCollection.xml
--rw-r--r--   0 laurent    (501) staff       (20)      253 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionContact.xml
--rw-r--r--   0 laurent    (501) staff       (20)      246 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionEvents.xml
--rw-r--r--   0 laurent    (501) staff       (20)      249 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionFiles.xml
--rw-r--r--   0 laurent    (501) staff       (20)      248 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionGallery.xml
--rw-r--r--   0 laurent    (501) staff       (20)      249 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionHTML.xml
--rw-r--r--   0 laurent    (501) staff       (20)      250 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionLinks.xml
--rw-r--r--   0 laurent    (501) staff       (20)      241 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionMap.xml
--rw-r--r--   0 laurent    (501) staff       (20)      248 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionNews.xml
--rw-r--r--   0 laurent    (501) staff       (20)      249 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionPostit.xml
--rw-r--r--   0 laurent    (501) staff       (20)      254 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionSelections.xml
--rw-r--r--   0 laurent    (501) staff       (20)      249 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionSendinblue.xml
--rw-r--r--   0 laurent    (501) staff       (20)      246 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionSlide.xml
--rw-r--r--   0 laurent    (501) staff       (20)      248 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionText.xml
--rw-r--r--   0 laurent    (501) staff       (20)      249 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionVideo.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1034_to_1035/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1034_to_1035/types/
--rw-r--r--   0 laurent    (501) staff       (20)      325 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1034_to_1035/types/imio.smartweb.DirectoryView.xml
--rw-r--r--   0 laurent    (501) staff       (20)      322 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1034_to_1035/types/imio.smartweb.EventsView.xml
--rw-r--r--   0 laurent    (501) staff       (20)      318 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1034_to_1035/types/imio.smartweb.Folder.xml
--rw-r--r--   0 laurent    (501) staff       (20)      320 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1034_to_1035/types/imio.smartweb.NewsView.xml
--rw-r--r--   0 laurent    (501) staff       (20)      316 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1034_to_1035/types/imio.smartweb.Page.xml
--rw-r--r--   0 laurent    (501) staff       (20)      322 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1034_to_1035/types/imio.smartweb.PortalPage.xml
--rw-r--r--   0 laurent    (501) staff       (20)      321 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1034_to_1035/types/imio.smartweb.Procedure.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1035_to_1036/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1035_to_1036/registry/
--rw-r--r--   0 laurent    (501) staff       (20)      403 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1035_to_1036/registry/plone.xml
--rw-r--r--   0 laurent    (501) staff       (20)      298 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1035_to_1036/rolemap.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1035_to_1036/types/
--rw-r--r--   0 laurent    (501) staff       (20)     1471 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1035_to_1036/types/imio.smartweb.CirkwiView.xml
--rw-r--r--   0 laurent    (501) staff       (20)      305 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1035_to_1036/types/imio.smartweb.Folder.xml
--rw-r--r--   0 laurent    (501) staff       (20)      177 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1035_to_1036/types.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1036_to_1037/
--rw-r--r--   0 laurent    (501) staff       (20)      440 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1036_to_1037/actions.xml
--rw-r--r--   0 laurent    (501) staff       (20)      275 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1036_to_1037/rolemap.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1037_to_1038/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1037_to_1038/registry/
--rw-r--r--   0 laurent    (501) staff       (20)      249 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1037_to_1038/registry/plausible.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1038_to_1039/
--rw-r--r--   0 laurent    (501) staff       (20)      293 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1038_to_1039/rolemap.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1038_to_1039/types/
--rw-r--r--   0 laurent    (501) staff       (20)      315 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1038_to_1039/types/imio.smartweb.Page.xml
--rw-r--r--   0 laurent    (501) staff       (20)      321 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1038_to_1039/types/imio.smartweb.PortalPage.xml
--rw-r--r--   0 laurent    (501) staff       (20)      320 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1038_to_1039/types/imio.smartweb.Procedure.xml
--rw-r--r--   0 laurent    (501) staff       (20)     1286 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1038_to_1039/types/imio.smartweb.SectionExternalContent.xml
--rw-r--r--   0 laurent    (501) staff       (20)      189 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1038_to_1039/types.xml
--rw-r--r--   0 laurent    (501) staff       (20)      182 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1038_to_1039/workflows.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1039_to_1040/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1039_to_1040/types/
--rw-r--r--   0 laurent    (501) staff       (20)      397 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1039_to_1040/types/imio.smartweb.SectionSlide.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1040_to_1041/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1040_to_1041/types/
--rw-r--r--   0 laurent    (501) staff       (20)      514 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1040_to_1041/types/imio.smartweb.SectionText.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1041_to_1042/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1041_to_1042/types/
--rw-r--r--   0 laurent    (501) staff       (20)      399 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1041_to_1042/types/imio.smartweb.SectionContact.xml
--rw-r--r--   0 laurent    (501) staff       (20)      398 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1041_to_1042/types/imio.smartweb.SectionEvents.xml
--rw-r--r--   0 laurent    (501) staff       (20)      451 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1041_to_1042/types/imio.smartweb.SectionExternalContent.xml
--rw-r--r--   0 laurent    (501) staff       (20)      397 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1041_to_1042/types/imio.smartweb.SectionFiles.xml
--rw-r--r--   0 laurent    (501) staff       (20)      443 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1041_to_1042/types/imio.smartweb.SectionGallery.xml
--rw-r--r--   0 laurent    (501) staff       (20)      397 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1041_to_1042/types/imio.smartweb.SectionLinks.xml
--rw-r--r--   0 laurent    (501) staff       (20)      431 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1041_to_1042/types/imio.smartweb.SectionMap.xml
--rw-r--r--   0 laurent    (501) staff       (20)      396 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1041_to_1042/types/imio.smartweb.SectionNews.xml
--rw-r--r--   0 laurent    (501) staff       (20)      398 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1041_to_1042/types/imio.smartweb.SectionPostit.xml
--rw-r--r--   0 laurent    (501) staff       (20)      402 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1041_to_1042/types/imio.smartweb.SectionSelections.xml
--rw-r--r--   0 laurent    (501) staff       (20)      402 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1041_to_1042/types/imio.smartweb.SectionSendinblue.xml
--rw-r--r--   0 laurent    (501) staff       (20)      441 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1041_to_1042/types/imio.smartweb.SectionVideo.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1045_to_1046/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1045_to_1046/registry/
--rw-r--r--   0 laurent    (501) staff       (20)      562 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1045_to_1046/registry/plone.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1045_to_1046/types/
--rw-r--r--   0 laurent    (501) staff       (20)      490 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1045_to_1046/types/imio.smartweb.SectionExternalContent.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1046_to_1047/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1046_to_1047/types/
--rw-r--r--   0 laurent    (501) staff       (20)      768 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1046_to_1047/types/imio.smartweb.Folder.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/registry/
--rw-r--r--   0 laurent    (501) staff       (20)      562 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/registry/plone.xml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/types/
--rw-r--r--   0 laurent    (501) staff       (20)      904 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/types/imio.smartweb.DirectoryView.xml
--rw-r--r--   0 laurent    (501) staff       (20)      901 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/types/imio.smartweb.EventsView.xml
--rw-r--r--   0 laurent    (501) staff       (20)      873 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/types/imio.smartweb.Folder.xml
--rw-r--r--   0 laurent    (501) staff       (20)      899 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/types/imio.smartweb.NewsView.xml
--rw-r--r--   0 laurent    (501) staff       (20)      451 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/types/imio.smartweb.SectionCollection.xml
--rw-r--r--   0 laurent    (501) staff       (20)      448 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/types/imio.smartweb.SectionContact.xml
--rw-r--r--   0 laurent    (501) staff       (20)      447 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/types/imio.smartweb.SectionEvents.xml
--rw-r--r--   0 laurent    (501) staff       (20)      539 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/types/imio.smartweb.SectionExternalContent.xml
--rw-r--r--   0 laurent    (501) staff       (20)      446 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/types/imio.smartweb.SectionLinks.xml
--rw-r--r--   0 laurent    (501) staff       (20)      445 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/types/imio.smartweb.SectionNews.xml
--rw-r--r--   0 laurent    (501) staff       (20)      451 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/types/imio.smartweb.SectionSelections.xml
--rw-r--r--   0 laurent    (501) staff       (20)     8295 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/upgrades.py
--rw-r--r--   0 laurent    (501) staff       (20)     5483 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/utils.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)      661 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/actions.py
--rw-r--r--   0 laurent    (501) staff       (20)     3428 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/arcgis_header.pt
--rw-r--r--   0 laurent    (501) staff       (20)     1277 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/banner.pt
--rw-r--r--   0 laurent    (501) staff       (20)     2302 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/banner.py
--rw-r--r--   0 laurent    (501) staff       (20)      103 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/category.pt
--rw-r--r--   0 laurent    (501) staff       (20)      308 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/category.py
--rw-r--r--   0 laurent    (501) staff       (20)      611 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/chatbot.pt
--rw-r--r--   0 laurent    (501) staff       (20)      329 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/chatbot.py
--rw-r--r--   0 laurent    (501) staff       (20)    12313 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)      531 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/default_page_warning.pt
--rw-r--r--   0 laurent    (501) staff       (20)      421 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/external_content.py
--rw-r--r--   0 laurent    (501) staff       (20)      872 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/footer.pt
--rw-r--r--   0 laurent    (501) staff       (20)     3229 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/footer.py
--rw-r--r--   0 laurent    (501) staff       (20)      367 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/header.py
--rw-r--r--   0 laurent    (501) staff       (20)      577 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/header_actions.pt
--rw-r--r--   0 laurent    (501) staff       (20)      129 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/header_actions_viewlet.pt
--rw-r--r--   0 laurent    (501) staff       (20)      137 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/header_top_viewlet.pt
--rw-r--r--   0 laurent    (501) staff       (20)      688 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/herobanner.pt
--rw-r--r--   0 laurent    (501) staff       (20)     1359 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/herobanner.py
--rw-r--r--   0 laurent    (501) staff       (20)      498 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/interfaces.py
--rw-r--r--   0 laurent    (501) staff       (20)      318 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/lead_image.py
--rw-r--r--   0 laurent    (501) staff       (20)      738 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/logo.pt
--rw-r--r--   0 laurent    (501) staff       (20)     2213 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/logo.py
--rw-r--r--   0 laurent    (501) staff       (20)      308 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/menu.py
--rw-r--r--   0 laurent    (501) staff       (20)      872 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/messages.py
--rw-r--r--   0 laurent    (501) staff       (20)      648 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/minisite.py
--rw-r--r--   0 laurent    (501) staff       (20)      370 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/minisite_link.pt
--rw-r--r--   0 laurent    (501) staff       (20)     7284 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/navigation.py
--rw-r--r--   0 laurent    (501) staff       (20)      533 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/offcanvas.pt
--rw-r--r--   0 laurent    (501) staff       (20)      129 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/offcanvas.py
--rw-r--r--   0 laurent    (501) staff       (20)      602 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/procedure.pt
--rw-r--r--   0 laurent    (501) staff       (20)      633 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/procedure.py
--rw-r--r--   0 laurent    (501) staff       (20)      403 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/searchbox.pt
--rw-r--r--   0 laurent    (501) staff       (20)      207 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/social.py
--rw-r--r--   0 laurent    (501) staff       (20)     4218 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/subsite.py
--rw-r--r--   0 laurent    (501) staff       (20)      137 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/subsite_header_viewlet.pt
--rw-r--r--   0 laurent    (501) staff       (20)      503 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/subsite_logo.pt
--rw-r--r--   0 laurent    (501) staff       (20)      163 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/subsite_navigation.pt
--rw-r--r--   0 laurent    (501) staff       (20)     6556 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/toolbar.py
--rw-r--r--   0 laurent    (501) staff       (20)    20506 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/vocabularies.py
--rw-r--r--   0 laurent    (501) staff       (20)     5264 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/vocabularies.zcml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/
--rw-r--r--   0 laurent    (501) staff       (20)      343 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/.eslintrc.json
--rw-r--r--   0 laurent    (501) staff       (20)       92 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/.npmrc
--rw-r--r--   0 laurent    (501) staff       (20)       67 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/.prettierrc.json
--rw-r--r--   0 laurent    (501) staff       (20)      621 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/Makefile
--rw-r--r--   0 laurent    (501) staff       (20)       31 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/README.md
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)      194 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/babel.config.json
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/assets/
--rw-r--r--   0 laurent    (501) staff       (20)     1259 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/assets/layers-2x.8f2c4d11474275fbc1614b9098334eae.png
--rw-r--r--   0 laurent    (501) staff       (20)      696 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/assets/layers.416d91365b44e4b4f4777663e6f009f3.png
--rw-r--r--   0 laurent    (501) staff       (20)      348 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/assets/location-bla.1423bcce16ddcb21141430cac1428dc1.svg
--rw-r--r--   0 laurent    (501) staff       (20)     1466 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/assets/marker-icon.2b3e1faf89f94a4835397e7a43b4f77d.png
--rw-r--r--   0 laurent    (501) staff       (20)      628 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/assets/next-react-white.819cb069ac8eec300a9db6a7707712d6.svg
--rw-r--r--   0 laurent    (501) staff       (20)      628 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/assets/next-react.17bc43ff4a6a86f4520f5782f6a89a72.svg
--rw-r--r--   0 laurent    (501) staff       (20)      433 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/assets/oeil-big.f32cd1df1274a9593de0c4bd8e344216.svg
--rw-r--r--   0 laurent    (501) staff       (20)      330 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/assets/pin-react-active.07d154037a15be5525b823fdc626cf29.svg
--rw-r--r--   0 laurent    (501) staff       (20)      336 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/assets/pin-react.fda934b5daf26dd4da2a71a7e7e44431.svg
--rw-r--r--   0 laurent    (501) staff       (20)      426 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/assets/search.57bdbf5b191499cd77514097d1c4972c.svg
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/css/
--rw-r--r--   0 laurent    (501) staff       (20)    20468 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/css/267.smartweb-webcomponents-compiled.css
--rw-r--r--   0 laurent    (501) staff       (20)     2546 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/css/323.smartweb-webcomponents-compiled.css
--rw-r--r--   0 laurent    (501) staff       (20)    20093 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/css/552.smartweb-webcomponents-compiled.css
--rw-r--r--   0 laurent    (501) staff       (20)     3786 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/css/779.smartweb-webcomponents-compiled.css
--rw-r--r--   0 laurent    (501) staff       (20)     5304 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/css/smartweb-webcomponents-compiled.css
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/js/
--rw-r--r--   0 laurent    (501) staff       (20)    17480 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/js/144.smartweb-webcomponents-compiled.js
--rw-r--r--   0 laurent    (501) staff       (20)       59 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/js/144.smartweb-webcomponents-compiled.js.LICENSE.txt
--rw-r--r--   0 laurent    (501) staff       (20)   171258 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/js/212.smartweb-webcomponents-compiled.js
--rw-r--r--   0 laurent    (501) staff       (20)      361 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/js/212.smartweb-webcomponents-compiled.js.LICENSE.txt
--rw-r--r--   0 laurent    (501) staff       (20)    32641 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/js/267.smartweb-webcomponents-compiled.js
--rw-r--r--   0 laurent    (501) staff       (20)    26778 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/js/323.smartweb-webcomponents-compiled.js
--rw-r--r--   0 laurent    (501) staff       (20)      149 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/js/323.smartweb-webcomponents-compiled.js.LICENSE.txt
--rw-r--r--   0 laurent    (501) staff       (20)    58085 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/js/552.smartweb-webcomponents-compiled.js
--rw-r--r--   0 laurent    (501) staff       (20)      149 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/js/552.smartweb-webcomponents-compiled.js.LICENSE.txt
--rw-r--r--   0 laurent    (501) staff       (20)   131048 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/js/565.smartweb-webcomponents-compiled.js
--rw-r--r--   0 laurent    (501) staff       (20)    16627 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/js/612.smartweb-webcomponents-compiled.js
--rw-r--r--   0 laurent    (501) staff       (20)      149 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/js/612.smartweb-webcomponents-compiled.js.LICENSE.txt
--rw-r--r--   0 laurent    (501) staff       (20)    26369 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/js/779.smartweb-webcomponents-compiled.js
--rw-r--r--   0 laurent    (501) staff       (20)   159426 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/js/9.smartweb-webcomponents-compiled.js
--rw-r--r--   0 laurent    (501) staff       (20)      153 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/js/9.smartweb-webcomponents-compiled.js.LICENSE.txt
--rw-r--r--   0 laurent    (501) staff       (20)   363925 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/js/969.smartweb-webcomponents-compiled.js
--rw-r--r--   0 laurent    (501) staff       (20)    15195 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/js/969.smartweb-webcomponents-compiled.js.LICENSE.txt
--rw-r--r--   0 laurent    (501) staff       (20)   409442 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/js/smartweb-webcomponents-compiled.js
--rw-r--r--   0 laurent    (501) staff       (20)     1035 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/js/smartweb-webcomponents-compiled.js.LICENSE.txt
--rw-r--r--   0 laurent    (501) staff       (20)      263 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/configure.zcml
--rw-r--r--   0 laurent    (501) staff       (20)     2624 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/package.json
--rw-r--r--   0 laurent    (501) staff       (20)   255013 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/pnpm-lock.yaml
--rw-r--r--   0 laurent    (501) staff       (20)      101 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/postcss.config.js
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/assets/
--rw-r--r--   0 laurent    (501) staff       (20)      478 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/assets/close.svg
--rw-r--r--   0 laurent    (501) staff       (20)      799 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/assets/facebook-news.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)     9538 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/assets/img-placeholder-bla.png
--rwxr-xr-x   0 laurent    (501) staff       (20)      369 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/assets/location-active-bla.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      348 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/assets/location-bla.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      628 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/assets/next-react-white.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      628 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/assets/next-react.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      433 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/assets/oeil-big.svg
--rw-r--r--   0 laurent    (501) staff       (20)      884 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/assets/pin-active.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      330 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/assets/pin-react-active.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      336 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/assets/pin-react.svg
--rw-r--r--   0 laurent    (501) staff       (20)      890 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/assets/pin.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      426 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/assets/search.svg
--rwxr-xr-x   0 laurent    (501) staff       (20)      453 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/assets/skeleton.svg
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/
--rw-r--r--   0 laurent    (501) staff       (20)     8946 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Annuaire.jsx
--rw-r--r--   0 laurent    (501) staff       (20)     8871 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Annuaire.scss
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactCard/
--rw-r--r--   0 laurent    (501) staff       (20)     5154 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactCard/ContactCard.jsx
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactContent/
--rw-r--r--   0 laurent    (501) staff       (20)    26943 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactContent/ContactContent.jsx
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactList/
--rw-r--r--   0 laurent    (501) staff       (20)     1678 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactList/ContactList.jsx
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactMap/
--rw-r--r--   0 laurent    (501) staff       (20)     5770 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactMap/ContactMap.jsx
--rw-r--r--   0 laurent    (501) staff       (20)       73 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactMap/ContactMap.scss
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Filters/
--rw-r--r--   0 laurent    (501) staff       (20)     7637 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Filters/Filter.jsx
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Skeleton/
--rw-r--r--   0 laurent    (501) staff       (20)      217 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Skeleton/LoaderCss.jsx
--rw-r--r--   0 laurent    (501) staff       (20)      656 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Skeleton/Skeleton.jsx
--rw-r--r--   0 laurent    (501) staff       (20)       97 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/index.js
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Events/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Events/ContactCard/
--rw-r--r--   0 laurent    (501) staff       (20)     1990 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Events/ContactCard/ContactCard.jsx
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Events/ContactContent/
--rw-r--r--   0 laurent    (501) staff       (20)    16920 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Events/ContactContent/ContactContent.jsx
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Events/ContactList/
--rw-r--r--   0 laurent    (501) staff       (20)     1675 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Events/ContactList/ContactList.jsx
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Events/ContactMap/
--rw-r--r--   0 laurent    (501) staff       (20)     5725 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Events/ContactMap/ContactMap.jsx
--rw-r--r--   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Events/ContactMap/ContactMap.scss
--rw-r--r--   0 laurent    (501) staff       (20)     9025 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Events/Events.jsx
--rw-r--r--   0 laurent    (501) staff       (20)     9045 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Events/Events.scss
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Events/Filters/
--rw-r--r--   0 laurent    (501) staff       (20)     6272 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Events/Filters/Filter.jsx
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Events/Skeleton/
--rw-r--r--   0 laurent    (501) staff       (20)      656 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Events/Skeleton/Skeleton.jsx
--rw-r--r--   0 laurent    (501) staff       (20)       95 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Events/index.js
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/News/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/News/ContactCard/
--rw-r--r--   0 laurent    (501) staff       (20)     3116 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/News/ContactCard/ContactCard.jsx
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/News/ContactContent/
--rw-r--r--   0 laurent    (501) staff       (20)    12536 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/News/ContactContent/ContactContent.jsx
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/News/ContactList/
--rw-r--r--   0 laurent    (501) staff       (20)     1493 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/News/ContactList/ContactList.jsx
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/News/ContactMap/
--rw-r--r--   0 laurent    (501) staff       (20)     4216 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/News/ContactMap/ContactMap.jsx
--rw-r--r--   0 laurent    (501) staff       (20)       42 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/News/ContactMap/ContactMap.scss
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/News/Filters/
--rw-r--r--   0 laurent    (501) staff       (20)     6249 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/News/Filters/Filter.jsx
--rw-r--r--   0 laurent    (501) staff       (20)     6850 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/News/News.jsx
--rw-r--r--   0 laurent    (501) staff       (20)     3293 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/News/News.scss
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/News/Skeleton/
--rw-r--r--   0 laurent    (501) staff       (20)      656 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/News/Skeleton/Skeleton.jsx
--rw-r--r--   0 laurent    (501) staff       (20)       93 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/News/index.js
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Search/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Search/ContactResult/
--rw-r--r--   0 laurent    (501) staff       (20)     2447 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Search/ContactResult/ContactResult.jsx
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Search/EventsResult/
--rw-r--r--   0 laurent    (501) staff       (20)     2445 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Search/EventsResult/EventsResult.jsx
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Search/Filters/
--rw-r--r--   0 laurent    (501) staff       (20)     6510 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Search/Filters/Filter.jsx
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Search/NewsResult/
--rw-r--r--   0 laurent    (501) staff       (20)     2472 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Search/NewsResult/NewsResult.jsx
--rw-r--r--   0 laurent    (501) staff       (20)     2271 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Search/Search.jsx
--rw-r--r--   0 laurent    (501) staff       (20)     2735 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Search/Search.scss
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Search/Skeleton/
--rw-r--r--   0 laurent    (501) staff       (20)      656 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Search/Skeleton/Skeleton.jsx
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Search/WebResult/
--rw-r--r--   0 laurent    (501) staff       (20)     1831 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Search/WebResult/WebResult.jsx
--rw-r--r--   0 laurent    (501) staff       (20)       95 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Search/index.js
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/hooks/
--rw-r--r--   0 laurent    (501) staff       (20)     1215 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/hooks/useAxios.js
--rw-r--r--   0 laurent    (501) staff       (20)      223 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/hooks/useFilterQuery.js
--rw-r--r--   0 laurent    (501) staff       (20)      757 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/index.jsx
--rw-r--r--   0 laurent    (501) staff       (20)     5511 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/index.scss
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/utils/
--rw-r--r--   0 laurent    (501) staff       (20)     2694 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/utils/translation.js
--rw-r--r--   0 laurent    (501) staff       (20)      244 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/utils/url.js
--rw-r--r--   0 laurent    (501) staff       (20)     6852 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/webpack.config.js
--rw-r--r--   0 laurent    (501) staff       (20)     2226 2023-11-23 08:27:27.000000 imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/webpackPlonePlugin.js
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio.smartweb.core.egg-info/
--rw-r--r--   0 laurent    (501) staff       (20)    43707 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio.smartweb.core.egg-info/PKG-INFO
--rw-r--r--   0 laurent    (501) staff       (20)    44100 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio.smartweb.core.egg-info/SOURCES.txt
--rw-r--r--   0 laurent    (501) staff       (20)        1 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio.smartweb.core.egg-info/dependency_links.txt
--rw-r--r--   0 laurent    (501) staff       (20)       19 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio.smartweb.core.egg-info/namespace_packages.txt
--rw-r--r--   0 laurent    (501) staff       (20)        1 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio.smartweb.core.egg-info/not-zip-safe
--rw-r--r--   0 laurent    (501) staff       (20)      623 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio.smartweb.core.egg-info/requires.txt
--rw-r--r--   0 laurent    (501) staff       (20)        5 2023-11-23 08:27:28.000000 imio.smartweb.core-1.2.8/src/imio.smartweb.core.egg-info/top_level.txt
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.924090 imio.smartweb.core-1.2.9/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    38963 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/CHANGES.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      169 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/CONTRIBUTORS.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      522 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/DEVELOP.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    18092 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/LICENSE.GPL
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      653 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/LICENSE.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      188 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/MANIFEST.in
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    43797 2023-11-24 10:12:17.924090 imio.smartweb.core-1.2.9/PKG-INFO
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3610 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/README.rst
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.868089 imio.smartweb.core-1.2.9/docs/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7994 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/docs/conf.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       63 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/docs/index.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       64 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/requirements.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      518 2023-11-24 10:12:17.924090 imio.smartweb.core-1.2.9/setup.cfg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3010 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/setup.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.852089 imio.smartweb.core-1.2.9/src/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.868089 imio.smartweb.core-1.2.9/src/imio/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.868089 imio.smartweb.core-1.2.9/src/imio/smartweb/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.872089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       24 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.872089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/behaviors/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/behaviors/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1677 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/behaviors/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      760 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/behaviors/listing.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1865 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/behaviors/minisite.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      557 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/behaviors/orientation.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1063 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/behaviors/quickaccess.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1707 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/behaviors/subsite.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.872089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.872089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/banner/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/banner/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      389 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/banner/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      947 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/banner/settings.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2811 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5361 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/controlpanel.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.872089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/dashboards/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/dashboards/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      523 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/dashboards/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1107 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/dashboards/plausible.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      651 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/dashboards/plausible.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.872089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/faceted/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/faceted/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1987 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/faceted/block_view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3289 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/faceted/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2951 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/faceted/macros.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4434 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/faceted/map.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1504 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/faceted/map.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1931 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/faceted/summary_view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1460 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/faceted/views.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.872089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/faceted/widgets/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/faceted/widgets/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      449 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/faceted/widgets/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2459 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/faceted/widgets/select.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      221 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/faceted/widgets/select.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.872089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/footer/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/footer/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      388 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/footer/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2492 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/footer/settings.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1089 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/forms.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.872089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/herobanner/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/herobanner/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      400 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/herobanner/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2884 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/herobanner/settings.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2065 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/icons.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.876089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/instancebehaviors/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/instancebehaviors/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      632 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/instancebehaviors/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3052 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/instancebehaviors/form.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      742 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/instancebehaviors/utils.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2066 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/layout.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.876089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/minisite/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/minisite/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      417 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/minisite/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2766 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/minisite/settings.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.876089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/overrides/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/overrides/.gitkeep
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2111 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/overrides/plone.app.content.browser.contents.templates.properties.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      978 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/overrides/plone.app.layout.viewlets.sections.pt
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.876089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/search/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/search/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      423 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/search/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      450 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/search/search.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2369 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/search/search.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.876089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/.gitkeep
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      350 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/Makefile
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.880089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      873 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/action-e-guichet.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      274 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/action-email.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1355 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/action-engagement.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      483 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/action-nous-contacter.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      409 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/action-nous-rejoindre.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      307 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/action-organiser-un-evenement.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      787 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/action-signaler-un-probleme.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      414 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/action-voir-plan.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      313 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/categorie-associations.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      313 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/categorie-avis-et-enquetes.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      458 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/categorie-cinema.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1787 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/categorie-commerce.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      508 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/categorie-concert.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      367 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/categorie-culture.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      426 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/categorie-demarches.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)     1011 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/categorie-enfance.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      673 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/categorie-enseignement.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      252 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/categorie-environnement-gestion-des-dechets.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      284 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/categorie-exposition.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      245 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/categorie-horaires.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      453 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/categorie-infos-travaux.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      692 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/categorie-mandataires.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      561 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/categorie-mobilite.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      302 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/categorie-mon-dossier.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      318 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/categorie-parc-de-stationnement.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      419 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/categorie-parcs-et-jardins.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      662 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/categorie-primes.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      397 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/categorie-sport-courir.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      514 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/categorie-sport-trophee.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      925 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/categorie-sport-velo.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      713 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/categorie-theatre.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      390 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/categorie-tourisme.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      294 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/organisation-academie-musique.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      522 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/organisation-bibliotheque.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      739 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/organisation-centre-sportif.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      879 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/organisation-cpas.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      625 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/organisation-ecole-des-arts.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      302 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/organisation-ecole.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      614 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/organisation-mobilite.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      451 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/organisation-police.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)     2086 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/reseausocial-facebook-pouce.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      421 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/reseausocial-facebook.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)     1999 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/reseausocial-instagram.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1039 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/reseausocial-twitter.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      826 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/reseausocial-vimeo.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      542 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/reseausocial-youtube.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      350 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/vue-actualites.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      339 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/vue-agenda.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      497 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/vue-annuaire.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      695 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/package.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      863 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/smartweb-edit-compiled.css
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1137 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/smartweb-edit-compiled.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      608 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/smartweb-swiperconfig-compiled.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2702 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/smartweb-view-compiled.css
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2060 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/smartweb-view-compiled.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    19615 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/spotlight-bundle.js
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.880089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/src/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1783 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/src/edit.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1089 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/src/edit.less
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1285 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/src/swiper-config.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2980 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/src/view.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2843 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/src/view.less
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    17908 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/swiper-bundle.min.css
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)   137031 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/swiper-bundle.min.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1079 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/webpack.config.js
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.880089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/subsite/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/subsite/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      414 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/subsite/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1601 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/subsite/settings.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.880089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/templates/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2808 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/templates/link_input.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4160 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/utils.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      337 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/config.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1429 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.880089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3308 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.880089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/blocks/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/blocks/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      732 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/blocks/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.880089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/blocks/link/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/blocks/link/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      552 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/blocks/link/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1407 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/blocks/link/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      479 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/blocks/link/fields.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      703 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/blocks/link/icons_input.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      330 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/blocks/subscriber.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      807 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1465 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/cropping.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.880089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/folder/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/folder/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1511 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/folder/block_view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2961 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/folder/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3377 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/folder/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      342 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/folder/element_view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1743 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/folder/macros.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1172 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/folder/summary_view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5682 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/folder/views.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.884089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.884089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/cirkwi/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/cirkwi/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      378 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/cirkwi/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      664 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/cirkwi/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      392 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/cirkwi/view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      482 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/cirkwi/view.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2252 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.884089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/footer/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/footer/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/footer/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1374 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/footer/content.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.884089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/herobanner/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/herobanner/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/herobanner/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1077 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/herobanner/content.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.884089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/page/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/page/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/page/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      465 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/page/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      464 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/pages.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.884089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/portal_page/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/portal_page/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      352 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/portal_page/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      336 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/portal_page/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      147 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/portal_page/view.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.884089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/procedure/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/procedure/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      356 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/procedure/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1297 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/procedure/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1291 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/procedure/utils.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      408 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/procedure/view.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      961 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/subscriber.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3127 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1345 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/view_section.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4852 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/views.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.884089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2146 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/base.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      200 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.884089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/directory/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/directory/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1035 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/directory/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1100 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/directory/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2962 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/directory/endpoint.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      750 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/directory/view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      384 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/directory/view.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.884089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/events/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/events/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1017 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/events/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1277 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/events/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2735 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/events/endpoint.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      751 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/events/view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      375 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/events/view.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.884089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/news/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/news/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1005 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/news/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      753 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/news/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2668 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/news/endpoint.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      696 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/news/view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      287 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/news/view.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.884089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/search/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/search/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      951 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/search/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     9796 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/search/endpoint.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      798 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/view.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.888089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2486 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/base.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.888089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/collection/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/collection/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      920 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/collection/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2379 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/collection/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1470 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/collection/views.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.888089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/common_templates/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5393 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/common_templates/carousel.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6402 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/common_templates/table.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2242 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.888089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/contact/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/contact/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1591 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/contact/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2661 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/contact/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1387 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/contact/forms.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     9523 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/contact/macros.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    11619 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/contact/utils.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1170 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/contact/view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1422 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/contact/view.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.888089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/events/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/events/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1117 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/events/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2914 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/events/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1522 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/events/macros.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3637 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/events/view.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.888089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/external_content/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/external_content/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      727 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/external_content/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1096 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/external_content/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1234 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/external_content/view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4895 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/external_content/view_arcgis.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8764 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/external_content/views.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.888089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/files/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/files/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      501 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/files/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      871 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/files/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1249 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/files/view.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.888089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/gallery/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/gallery/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      424 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/gallery/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      780 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/gallery/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2058 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/gallery/view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      451 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/gallery/views.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.888089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/html/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/html/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      413 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/html/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1352 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/html/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1140 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/html/view.pt
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.888089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/links/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/links/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      918 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/links/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1051 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/links/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1375 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/links/view.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4092 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/macros.pt
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.892089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/map/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/map/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      412 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/map/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      372 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/map/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1278 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/map/view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      614 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/map/views.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.892089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/news/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/news/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      880 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/news/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2911 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/news/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3260 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/news/view.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.892089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/postit/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/postit/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      504 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/postit/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2239 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/postit/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      936 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/postit/view.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.892089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/selections/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/selections/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      949 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/selections/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1375 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/selections/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1510 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/selections/view.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.892089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/sendinblue/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/sendinblue/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      433 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/sendinblue/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1088 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/sendinblue/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1180 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/sendinblue/view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1731 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/sendinblue/views.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.892089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/slide/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/slide/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      417 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/slide/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2181 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/slide/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2440 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/slide/view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      784 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/slide/view.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      642 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/subscriber.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.892089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/text/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/text/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1257 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/text/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1118 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/text/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1818 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/text/forms.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1576 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/text/view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      383 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/text/views.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.892089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/video/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/video/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      418 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/video/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      978 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/video/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1105 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/video/view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      342 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/video/views.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2832 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/views.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.892089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/faceted/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/faceted/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.892089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/faceted/config/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2906 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/faceted/config/collection.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      826 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/faceted/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      395 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/faceted/layout.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      295 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/faceted/menu.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3887 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/indexers.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      968 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/indexers.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      971 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/interfaces.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1777 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/permissions.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.860089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.892089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5877 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/actions.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      179 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/browserlayer.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      864 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/catalog.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      400 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/controlpanel.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1218 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/metadata.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.892089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2562 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/registry/bundles.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1251 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/registry/geolocation.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2400 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/registry/plone.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      253 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/registry/smartweb.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      183 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/repositorytool.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2726 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/rolemap.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.896089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/taxonomies/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      310 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/taxonomies/page_category.cfg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2059 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/taxonomies/page_category.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      320 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/taxonomies/procedure_category.cfg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3436 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/taxonomies/procedure_category.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.896089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1402 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.BlockLink.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1471 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.CirkwiView.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1557 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.DirectoryView.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1542 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.EventsView.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2557 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.Folder.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1730 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.Footer.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1604 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.HeroBanner.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1525 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.NewsView.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2483 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.Page.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2659 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.PortalPage.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2480 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.Procedure.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1506 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionCollection.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1183 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionContact.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1484 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionEvents.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1284 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionExternalContent.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1490 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionFiles.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1349 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionGallery.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1232 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionHTML.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1595 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionLinks.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1142 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionMap.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1478 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionNews.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1129 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionPostit.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1506 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionSelections.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1142 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionSendinblue.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1127 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionSlide.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1241 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionText.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1167 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionVideo.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2040 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1069 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/workflows.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.860089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/icons/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.896089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/icons/basic/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    17858 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/icons/basic/registry.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.896089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/icons/contenttypes/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8766 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/icons/contenttypes/registry.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.896089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/last_compilation/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      852 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/last_compilation/registry.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.896089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/testing/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      227 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/testing/metadata.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      706 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/testing/registry.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.896089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/testing/types/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      517 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/testing/types/Collection.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      215 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/testing/types/Document.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      213 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/testing/types/Folder.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      163 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/testing/types.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.896089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/uninstall/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      128 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2028 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      932 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/setuphandlers.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3940 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/subscribers.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1016 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/subscribers.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3636 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/testing.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      172 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/testing.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.900089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.904089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      150 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/cirkwi_bad_widget_mock.html
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)   333252 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/cirkwi_good_widget_mock.html
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      369 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_auth_sources_directory_entity.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      363 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_auth_sources_events_entity.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      359 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_auth_sources_news_entity.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3454 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_contact_category_raw_mock.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4820 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_contact_empty_schedule_raw_mock.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      771 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_contact_images_raw_mock.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      156 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_contact_no_image_raw_mock.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    12224 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_contact_raw_mock.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      921 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_contacts_raw_mock.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      749 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_directory_entities_raw_mock.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      769 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_events_agendas_raw_mock.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      441 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_events_entities_raw_mock.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      390 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_events_types_raw_mock.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      726 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_news_entities_raw_mock.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      783 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_news_newsfolder_raw_mock.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      127 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_no_contact_raw_mock.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      168 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_no_newsfolder_raw_mock.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3217 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_procedures_raw_mock.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    42421 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_rest_directory.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    46365 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_rest_events.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5002 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_rest_events_with_breadcrumbs.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    45966 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_rest_news.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1107 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_rest_specific_events.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2064 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_rest_specific_news.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      369 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_search_one_news_entity.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      205 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_used_iam_vocabularies_jobseeker_tourist.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    24753 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/plone.png
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3823 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/plone.svg
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.904089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/robot/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2596 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/robot/test_ct_folder.robot
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2548 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/robot/test_ct_page.robot
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2712 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/robot/test_ct_procedure.robot
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2003 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/robot/test_example.robot
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7838 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_banner.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5950 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_behaviors.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2012 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_categories.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1161 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_chatbot.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4921 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_cirkwiview.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6500 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_cropping.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    12109 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_default_pages.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5994 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_faceted.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    13527 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_folder.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    10970 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_footer.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5940 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_herobanner.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2788 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_icons.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    10784 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_indexes.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4274 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_instance_behaviors.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4997 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_local_roles.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2425 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_logo.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    16640 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_minisite.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6799 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_navigation.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    10699 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_page.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3229 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_plausibleview.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7215 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_portal_page.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6474 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_procedure.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    14609 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_rest.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      926 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_robot.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2182 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_search.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    23198 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_section_contact.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6690 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_section_events.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6872 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_section_external_content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6804 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_section_news.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2661 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_section_sendinblue.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    23691 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_sections.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2092 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_setup.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3046 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_social.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     9016 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_subsite.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4652 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_text.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3823 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_toolbar.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4125 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_utils.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    14234 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_vocabularies.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2374 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/utils.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.904089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    23756 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.864089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.860089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1015_to_1016/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.904089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1015_to_1016/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      481 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1015_to_1016/registry/e-guichet-icon.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.860089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1016_to_1017/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.904089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1016_to_1017/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      478 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1016_to_1017/registry/shop-icon.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.904089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1020_to_1021/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      538 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1020_to_1021/rolemap.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.904089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1020_to_1021/types/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      244 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1020_to_1021/types/imio.smartweb.SectionHTML.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.904089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1021_to_1022/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.904089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1021_to_1022/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      457 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1021_to_1022/registry/hero-banner.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      298 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1021_to_1022/rolemap.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.860089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1022_to_1023/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.904089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1022_to_1023/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      838 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1022_to_1023/registry/icons.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.904089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1023_to_1024/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.904089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1023_to_1024/types/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      306 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1023_to_1024/types/imio.smartweb.Page.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      312 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1023_to_1024/types/imio.smartweb.PortalPage.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      311 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1023_to_1024/types/imio.smartweb.Procedure.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1157 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1023_to_1024/types/imio.smartweb.SectionPostit.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      180 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1023_to_1024/types.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      173 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1023_to_1024/workflows.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.860089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1025_to_1026/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.904089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1025_to_1026/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      249 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1025_to_1026/registry/propose-urls.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.860089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1027_to_1028/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.904089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1027_to_1028/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      318 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1027_to_1028/registry/open-external-link-in-new-tab.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.904089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1029_to_1030/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      463 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1029_to_1030/actions.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      256 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1029_to_1030/rolemap.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.864089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1030_to_1031/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.904089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1030_to_1031/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1425 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1030_to_1031/registry/resources.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.864089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1031_to_1032/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.904089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1031_to_1032/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      562 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1031_to_1032/registry/spotlight.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.864089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.908089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      257 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.BlockLink.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      252 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.DirectoryView.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      252 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.EventsView.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      241 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.Folder.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      250 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.Footer.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      247 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.HeroBanner.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      245 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.NewsView.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      244 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.Page.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      256 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.PortalPage.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      256 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.Procedure.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      255 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionCollection.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      253 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionContact.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      246 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionEvents.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      249 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionFiles.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      248 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionGallery.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      249 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionHTML.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      250 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionLinks.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      241 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionMap.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      248 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionNews.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      249 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionPostit.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      254 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionSelections.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      249 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionSendinblue.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      246 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionSlide.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      248 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionText.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      249 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionVideo.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.864089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1034_to_1035/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.908089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1034_to_1035/types/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      325 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1034_to_1035/types/imio.smartweb.DirectoryView.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      322 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1034_to_1035/types/imio.smartweb.EventsView.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      318 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1034_to_1035/types/imio.smartweb.Folder.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      320 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1034_to_1035/types/imio.smartweb.NewsView.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      316 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1034_to_1035/types/imio.smartweb.Page.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      322 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1034_to_1035/types/imio.smartweb.PortalPage.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      321 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1034_to_1035/types/imio.smartweb.Procedure.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.908089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1035_to_1036/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.908089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1035_to_1036/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      403 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1035_to_1036/registry/plone.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      298 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1035_to_1036/rolemap.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.908089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1035_to_1036/types/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1471 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1035_to_1036/types/imio.smartweb.CirkwiView.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      305 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1035_to_1036/types/imio.smartweb.Folder.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      177 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1035_to_1036/types.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.908089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1036_to_1037/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      440 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1036_to_1037/actions.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      275 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1036_to_1037/rolemap.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.864089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1037_to_1038/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.908089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1037_to_1038/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      249 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1037_to_1038/registry/plausible.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.908089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1038_to_1039/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      293 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1038_to_1039/rolemap.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.908089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1038_to_1039/types/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      315 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1038_to_1039/types/imio.smartweb.Page.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      321 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1038_to_1039/types/imio.smartweb.PortalPage.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      320 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1038_to_1039/types/imio.smartweb.Procedure.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1286 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1038_to_1039/types/imio.smartweb.SectionExternalContent.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      189 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1038_to_1039/types.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      182 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1038_to_1039/workflows.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.864089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1039_to_1040/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.908089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1039_to_1040/types/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      397 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1039_to_1040/types/imio.smartweb.SectionSlide.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.864089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1040_to_1041/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.908089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1040_to_1041/types/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      514 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1040_to_1041/types/imio.smartweb.SectionText.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.864089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1041_to_1042/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.908089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1041_to_1042/types/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      399 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1041_to_1042/types/imio.smartweb.SectionContact.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      398 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1041_to_1042/types/imio.smartweb.SectionEvents.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      451 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1041_to_1042/types/imio.smartweb.SectionExternalContent.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      397 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1041_to_1042/types/imio.smartweb.SectionFiles.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      443 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1041_to_1042/types/imio.smartweb.SectionGallery.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      397 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1041_to_1042/types/imio.smartweb.SectionLinks.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      431 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1041_to_1042/types/imio.smartweb.SectionMap.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      396 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1041_to_1042/types/imio.smartweb.SectionNews.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      398 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1041_to_1042/types/imio.smartweb.SectionPostit.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      402 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1041_to_1042/types/imio.smartweb.SectionSelections.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      402 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1041_to_1042/types/imio.smartweb.SectionSendinblue.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      441 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1041_to_1042/types/imio.smartweb.SectionVideo.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.864089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1045_to_1046/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.912089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1045_to_1046/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      562 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1045_to_1046/registry/plone.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.912089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1045_to_1046/types/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      490 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1045_to_1046/types/imio.smartweb.SectionExternalContent.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.864089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1046_to_1047/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.912089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1046_to_1047/types/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      768 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1046_to_1047/types/imio.smartweb.Folder.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.864089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.912089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      562 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/registry/plone.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.912089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/types/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      904 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/types/imio.smartweb.DirectoryView.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      901 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/types/imio.smartweb.EventsView.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      873 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/types/imio.smartweb.Folder.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      899 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/types/imio.smartweb.NewsView.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      451 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/types/imio.smartweb.SectionCollection.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      448 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/types/imio.smartweb.SectionContact.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      447 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/types/imio.smartweb.SectionEvents.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      539 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/types/imio.smartweb.SectionExternalContent.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      446 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/types/imio.smartweb.SectionLinks.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      445 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/types/imio.smartweb.SectionNews.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      451 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/types/imio.smartweb.SectionSelections.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8295 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/upgrades.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5483 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/utils.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.916089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      661 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/actions.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3428 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/arcgis_header.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1277 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/banner.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2302 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/banner.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      103 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/category.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      308 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/category.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      611 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/chatbot.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      329 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/chatbot.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    12313 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      531 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/default_page_warning.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      421 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/external_content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      872 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/footer.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3229 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/footer.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      367 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/header.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      577 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/header_actions.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      129 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/header_actions_viewlet.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      137 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/header_top_viewlet.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      688 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/herobanner.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1359 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/herobanner.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      498 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/interfaces.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      318 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/lead_image.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      738 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/logo.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2213 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/logo.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      308 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/menu.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      872 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/messages.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      648 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/minisite.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      370 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/minisite_link.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7284 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/navigation.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      533 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/offcanvas.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      129 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/offcanvas.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      602 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/procedure.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      633 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/procedure.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      403 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/searchbox.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      207 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/social.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4218 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/subsite.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      137 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/subsite_header_viewlet.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      503 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/subsite_logo.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      163 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/subsite_navigation.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6556 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/toolbar.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    20506 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/vocabularies.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5264 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/vocabularies.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.916089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      343 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/.eslintrc.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       92 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/.npmrc
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       67 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/.prettierrc.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      621 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/Makefile
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       31 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/README.md
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      194 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/babel.config.json
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.864089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.916089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/assets/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1259 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/assets/layers-2x.8f2c4d11474275fbc1614b9098334eae.png
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      696 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/assets/layers.416d91365b44e4b4f4777663e6f009f3.png
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      348 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/assets/location-bla.1423bcce16ddcb21141430cac1428dc1.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1466 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/assets/marker-icon.2b3e1faf89f94a4835397e7a43b4f77d.png
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      628 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/assets/next-react-white.819cb069ac8eec300a9db6a7707712d6.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      628 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/assets/next-react.17bc43ff4a6a86f4520f5782f6a89a72.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      433 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/assets/oeil-big.f32cd1df1274a9593de0c4bd8e344216.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      330 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/assets/pin-react-active.07d154037a15be5525b823fdc626cf29.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      336 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/assets/pin-react.fda934b5daf26dd4da2a71a7e7e44431.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      426 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/assets/search.57bdbf5b191499cd77514097d1c4972c.svg
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.916089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/css/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    20468 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/css/267.smartweb-webcomponents-compiled.css
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2546 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/css/323.smartweb-webcomponents-compiled.css
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    20093 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/css/552.smartweb-webcomponents-compiled.css
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3786 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/css/779.smartweb-webcomponents-compiled.css
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5304 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/css/smartweb-webcomponents-compiled.css
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.920089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/js/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    17480 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/js/144.smartweb-webcomponents-compiled.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       59 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/js/144.smartweb-webcomponents-compiled.js.LICENSE.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)   171258 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/js/212.smartweb-webcomponents-compiled.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      361 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/js/212.smartweb-webcomponents-compiled.js.LICENSE.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    32641 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/js/267.smartweb-webcomponents-compiled.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    26778 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/js/323.smartweb-webcomponents-compiled.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      149 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/js/323.smartweb-webcomponents-compiled.js.LICENSE.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    58085 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/js/552.smartweb-webcomponents-compiled.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      149 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/js/552.smartweb-webcomponents-compiled.js.LICENSE.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)   131048 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/js/565.smartweb-webcomponents-compiled.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    16627 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/js/612.smartweb-webcomponents-compiled.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      149 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/js/612.smartweb-webcomponents-compiled.js.LICENSE.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    26369 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/js/779.smartweb-webcomponents-compiled.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)   159426 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/js/9.smartweb-webcomponents-compiled.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      153 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/js/9.smartweb-webcomponents-compiled.js.LICENSE.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)   363925 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/js/969.smartweb-webcomponents-compiled.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    15195 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/js/969.smartweb-webcomponents-compiled.js.LICENSE.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)   409442 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/js/smartweb-webcomponents-compiled.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1035 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/js/smartweb-webcomponents-compiled.js.LICENSE.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      263 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2624 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/package.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)   255013 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/pnpm-lock.yaml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      101 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/postcss.config.js
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.920089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.920089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/assets/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      478 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/assets/close.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      799 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/assets/facebook-news.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)     9538 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/assets/img-placeholder-bla.png
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      369 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/assets/location-active-bla.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      348 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/assets/location-bla.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      628 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/assets/next-react-white.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      628 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/assets/next-react.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      433 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/assets/oeil-big.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      884 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/assets/pin-active.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      330 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/assets/pin-react-active.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      336 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/assets/pin-react.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      890 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/assets/pin.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      426 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/assets/search.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      453 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/assets/skeleton.svg
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.868089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.920089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8946 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Annuaire.jsx
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8871 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Annuaire.scss
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.920089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactCard/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5154 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactCard/ContactCard.jsx
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.920089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactContent/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    26943 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactContent/ContactContent.jsx
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.920089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactList/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1678 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactList/ContactList.jsx
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.920089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactMap/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5770 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactMap/ContactMap.jsx
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       73 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactMap/ContactMap.scss
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.920089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Filters/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7637 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Filters/Filter.jsx
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.920089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Skeleton/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      217 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Skeleton/LoaderCss.jsx
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      656 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Skeleton/Skeleton.jsx
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       97 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/index.js
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.920089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Events/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.920089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Events/ContactCard/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1990 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Events/ContactCard/ContactCard.jsx
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.920089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Events/ContactContent/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    16920 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Events/ContactContent/ContactContent.jsx
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.920089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Events/ContactList/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1675 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Events/ContactList/ContactList.jsx
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.920089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Events/ContactMap/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5725 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Events/ContactMap/ContactMap.jsx
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Events/ContactMap/ContactMap.scss
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     9025 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Events/Events.jsx
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     9045 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Events/Events.scss
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.920089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Events/Filters/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6272 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Events/Filters/Filter.jsx
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.920089 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Events/Skeleton/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      656 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Events/Skeleton/Skeleton.jsx
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       95 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Events/index.js
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.924090 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/News/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.924090 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/News/ContactCard/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3116 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/News/ContactCard/ContactCard.jsx
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.924090 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/News/ContactContent/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    12536 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/News/ContactContent/ContactContent.jsx
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.924090 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/News/ContactList/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1493 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/News/ContactList/ContactList.jsx
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.924090 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/News/ContactMap/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4216 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/News/ContactMap/ContactMap.jsx
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       42 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/News/ContactMap/ContactMap.scss
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.924090 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/News/Filters/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6249 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/News/Filters/Filter.jsx
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6850 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/News/News.jsx
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3293 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/News/News.scss
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.924090 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/News/Skeleton/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      656 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/News/Skeleton/Skeleton.jsx
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       93 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/News/index.js
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.924090 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Search/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.924090 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Search/ContactResult/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2447 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Search/ContactResult/ContactResult.jsx
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.924090 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Search/EventsResult/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2445 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Search/EventsResult/EventsResult.jsx
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.924090 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Search/Filters/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6510 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Search/Filters/Filter.jsx
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.924090 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Search/NewsResult/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2472 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Search/NewsResult/NewsResult.jsx
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2271 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Search/Search.jsx
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2735 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Search/Search.scss
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.924090 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Search/Skeleton/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      656 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Search/Skeleton/Skeleton.jsx
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.924090 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Search/WebResult/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1831 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Search/WebResult/WebResult.jsx
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       95 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Search/index.js
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.924090 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/hooks/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1215 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/hooks/useAxios.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      223 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/hooks/useFilterQuery.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      757 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/index.jsx
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5511 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/index.scss
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.924090 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/utils/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2694 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/utils/translation.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      244 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/utils/url.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6852 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/webpack.config.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2226 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/webpackPlonePlugin.js
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-24 10:12:17.868089 imio.smartweb.core-1.2.9/src/imio.smartweb.core.egg-info/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    43797 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio.smartweb.core.egg-info/PKG-INFO
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    44100 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio.smartweb.core.egg-info/SOURCES.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio.smartweb.core.egg-info/dependency_links.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       19 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio.smartweb.core.egg-info/namespace_packages.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio.smartweb.core.egg-info/not-zip-safe
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      623 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio.smartweb.core.egg-info/requires.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        5 2023-11-24 10:12:17.000000 imio.smartweb.core-1.2.9/src/imio.smartweb.core.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `imio.smartweb.core-1.2.8/CHANGES.rst` & `imio.smartweb.core-1.2.9/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 Changelog
 =========
 
 
+1.2.9 (2023-11-24)
+------------------
+
+- WEB-4021 : Fix lead image displaying with files section
+  [boulch]
+
+
 1.2.8 (2023-11-23)
 ------------------
 
 - Fix (lead) image sizes URLs for text section & migrate old values
   [boulch, laulaz]
```

### Comparing `imio.smartweb.core-1.2.8/DEVELOP.rst` & `imio.smartweb.core-1.2.9/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/LICENSE.GPL` & `imio.smartweb.core-1.2.9/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/LICENSE.rst` & `imio.smartweb.core-1.2.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/PKG-INFO` & `imio.smartweb.core-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: imio.smartweb.core
-Version: 1.2.8
+Version: 1.2.9
 Summary: Core product for iMio websites
 Home-page: https://github.com/imio/imio.smartweb.core
 Author: Christophe Boulanger
 Author-email: christophe.boulanger@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/imio.smartweb.core
 Project-URL: Source, https://github.com/imio/imio.smartweb.core
 Project-URL: Tracker, https://github.com/imio/imio.smartweb.core/issues
 Keywords: Python Plone CMS
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 6.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -155,14 +154,21 @@
 - Thomas Lambert, thomas.lambert@imio.be
 
 
 Changelog
 =========
 
 
+1.2.9 (2023-11-24)
+------------------
+
+- WEB-4021 : Fix lead image displaying with files section
+  [boulch]
+
+
 1.2.8 (2023-11-23)
 ------------------
 
 - Fix (lead) image sizes URLs for text section & migrate old values
   [boulch, laulaz]
 
 
@@ -2011,9 +2017,7 @@
 
 
 1.0a1 (2021-04-19)
 ------------------
 
 - Initial release.
   [boulch]
-
-
```

### Comparing `imio.smartweb.core-1.2.8/README.rst` & `imio.smartweb.core-1.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/docs/conf.py` & `imio.smartweb.core-1.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/setup.cfg` & `imio.smartweb.core-1.2.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/setup.py` & `imio.smartweb.core-1.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="imio.smartweb.core",
-    version="1.2.8",
+    version="1.2.9",
     description="Core product for iMio websites",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/behaviors/configure.zcml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/behaviors/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/behaviors/listing.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/behaviors/listing.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/behaviors/minisite.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/behaviors/minisite.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/behaviors/orientation.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/behaviors/orientation.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/behaviors/quickaccess.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/behaviors/quickaccess.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/behaviors/subsite.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/behaviors/subsite.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/banner/settings.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/banner/settings.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/configure.zcml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/controlpanel.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/dashboards/configure.zcml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/dashboards/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/dashboards/plausible.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/dashboards/plausible.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/dashboards/plausible.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/dashboards/plausible.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/faceted/block_view.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/faceted/block_view.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/faceted/configure.zcml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/faceted/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/faceted/macros.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/faceted/macros.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/faceted/map.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/faceted/map.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/faceted/map.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/faceted/map.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/faceted/summary_view.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/faceted/summary_view.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/faceted/views.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/faceted/views.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/faceted/widgets/select.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/faceted/widgets/select.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/footer/settings.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/footer/settings.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/forms.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/forms.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/herobanner/settings.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/herobanner/settings.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/icons.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/icons.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/instancebehaviors/configure.zcml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/instancebehaviors/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/instancebehaviors/form.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/instancebehaviors/form.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/instancebehaviors/utils.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/instancebehaviors/utils.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/layout.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/layout.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/minisite/settings.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/minisite/settings.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/overrides/plone.app.content.browser.contents.templates.properties.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/overrides/plone.app.content.browser.contents.templates.properties.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/overrides/plone.app.layout.viewlets.sections.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/overrides/plone.app.layout.viewlets.sections.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/search/search.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/search/search.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/action-e-guichet.svg` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/action-e-guichet.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/action-engagement.svg` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/action-engagement.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/action-signaler-un-probleme.svg` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/action-signaler-un-probleme.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/categorie-commerce.svg` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/categorie-commerce.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/categorie-enfance.svg` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/categorie-enfance.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/categorie-enseignement.svg` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/categorie-enseignement.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/categorie-mandataires.svg` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/categorie-mandataires.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/categorie-mobilite.svg` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/categorie-mobilite.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/categorie-primes.svg` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/categorie-primes.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/categorie-sport-trophee.svg` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/categorie-sport-trophee.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/categorie-sport-velo.svg` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/categorie-sport-velo.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/categorie-theatre.svg` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/categorie-theatre.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/organisation-bibliotheque.svg` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/organisation-bibliotheque.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/organisation-centre-sportif.svg` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/organisation-centre-sportif.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/organisation-cpas.svg` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/organisation-cpas.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/organisation-ecole-des-arts.svg` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/organisation-ecole-des-arts.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/organisation-mobilite.svg` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/organisation-mobilite.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/reseausocial-facebook-pouce.svg` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/reseausocial-facebook-pouce.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/reseausocial-instagram.svg` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/reseausocial-instagram.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/reseausocial-twitter.svg` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/reseausocial-twitter.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/reseausocial-vimeo.svg` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/reseausocial-vimeo.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/icons/reseausocial-youtube.svg` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/icons/reseausocial-youtube.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/package.json` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/package.json`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/smartweb-edit-compiled.css` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/smartweb-edit-compiled.css`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/smartweb-edit-compiled.js` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/smartweb-edit-compiled.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/smartweb-swiperconfig-compiled.js` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/smartweb-swiperconfig-compiled.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/smartweb-view-compiled.css` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/smartweb-view-compiled.css`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/smartweb-view-compiled.js` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/smartweb-view-compiled.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/spotlight-bundle.js` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/spotlight-bundle.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/src/edit.js` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/src/edit.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/src/edit.less` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/src/edit.less`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/src/swiper-config.js` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/src/swiper-config.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/src/view.js` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/src/view.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/src/view.less` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/src/view.less`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/swiper-bundle.min.css` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/swiper-bundle.min.css`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/swiper-bundle.min.js` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/swiper-bundle.min.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/static/webpack.config.js` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/static/webpack.config.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/subsite/settings.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/subsite/settings.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/templates/link_input.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/templates/link_input.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/browser/utils.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/browser/utils.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/configure.zcml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/__init__.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/__init__.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/blocks/configure.zcml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/blocks/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/blocks/link/configure.zcml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/blocks/link/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/blocks/link/content.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/blocks/link/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/blocks/link/icons_input.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/blocks/link/icons_input.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/configure.zcml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/cropping.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/cropping.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/folder/block_view.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/folder/block_view.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/folder/configure.zcml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/folder/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/folder/content.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/folder/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/folder/macros.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/folder/macros.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/folder/summary_view.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/folder/summary_view.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/folder/views.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/folder/views.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/cirkwi/content.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/cirkwi/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/configure.zcml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/footer/content.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/footer/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/herobanner/content.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/herobanner/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/procedure/content.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/procedure/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/procedure/utils.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/procedure/utils.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/subscriber.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/subscriber.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/view.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/view.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/view_section.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/view_section.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/pages/views.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/pages/views.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/base.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/base.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/directory/configure.zcml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/directory/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/directory/content.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/directory/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/directory/endpoint.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/directory/endpoint.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/directory/view.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/directory/view.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/events/configure.zcml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/events/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/events/content.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/events/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/events/endpoint.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/events/endpoint.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/events/view.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/events/view.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/news/configure.zcml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/news/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/news/content.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/news/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/news/endpoint.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/news/endpoint.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/news/view.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/news/view.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/search/configure.zcml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/search/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/search/endpoint.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/search/endpoint.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/rest/view.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/rest/view.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/base.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/base.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/collection/configure.zcml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/collection/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/collection/content.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/collection/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/collection/views.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/collection/views.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/common_templates/carousel.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/common_templates/carousel.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/common_templates/table.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/common_templates/table.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/configure.zcml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/contact/configure.zcml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/contact/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/contact/content.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/contact/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/contact/forms.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/contact/forms.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/contact/macros.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/contact/macros.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/contact/utils.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/contact/utils.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/contact/view.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/contact/view.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/contact/view.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/contact/view.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/events/configure.zcml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/events/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/events/content.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/events/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/events/macros.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/events/macros.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/events/view.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/events/view.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/external_content/configure.zcml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/external_content/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/external_content/content.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/external_content/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/external_content/view.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/external_content/view.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/external_content/view_arcgis.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/external_content/view_arcgis.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/external_content/views.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/external_content/views.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/files/content.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/files/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/files/view.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/files/view.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,17 @@
         image_scale = self.image_scale
         items = self.context.listFolderContents()
         results = []
         for item in items:
             url = item.absolute_url()
             has_image = True if getattr(item.aq_base, "image", None) else False
             file_view = queryMultiAdapter((item, self.request), name="file_view")
-            scale_url = get_scale_url(item, self.request, "image", image_scale)
+            scale_url = get_scale_url(
+                item, self.request, "image", image_scale, orientation="paysage"
+            )
             results.append(
                 {
                     "title": item.title,
                     "description": item.description,
                     "url": url,
                     "image": scale_url,
                     "has_image": has_image,
```

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/gallery/content.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/gallery/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/gallery/view.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/gallery/view.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/html/content.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/html/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/html/view.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/html/view.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/links/configure.zcml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/links/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/links/content.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/links/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/links/view.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/links/view.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/macros.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/macros.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/map/view.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/map/view.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/map/views.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/map/views.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/news/configure.zcml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/news/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/news/content.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/news/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/news/view.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/news/view.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/postit/content.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/postit/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/postit/view.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/postit/view.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/selections/configure.zcml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/selections/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/selections/content.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/selections/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/selections/view.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/selections/view.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/sendinblue/content.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/sendinblue/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/sendinblue/view.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/sendinblue/view.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/sendinblue/views.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/sendinblue/views.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/slide/content.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/slide/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/slide/view.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/slide/view.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/slide/view.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/slide/view.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/subscriber.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/subscriber.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/text/configure.zcml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/text/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/text/content.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/text/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/text/forms.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/text/forms.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/text/view.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/text/view.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/video/content.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/video/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/video/view.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/video/view.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/contents/sections/views.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/contents/sections/views.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/faceted/config/collection.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/faceted/config/collection.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/faceted/configure.zcml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/faceted/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/indexers.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/indexers.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/indexers.zcml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/indexers.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/interfaces.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/interfaces.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/permissions.zcml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/permissions.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/actions.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/catalog.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/catalog.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/metadata.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/metadata.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/registry/bundles.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/registry/bundles.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/registry/geolocation.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/registry/geolocation.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/registry/plone.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/registry/plone.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/rolemap.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/taxonomies/page_category.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/taxonomies/page_category.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/taxonomies/procedure_category.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/taxonomies/procedure_category.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.BlockLink.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.BlockLink.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.CirkwiView.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.CirkwiView.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.DirectoryView.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.DirectoryView.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.EventsView.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.EventsView.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.Folder.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.Folder.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.Footer.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.Footer.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.HeroBanner.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.HeroBanner.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.NewsView.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.NewsView.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.Page.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.Page.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.PortalPage.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.PortalPage.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.Procedure.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.Procedure.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionCollection.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionCollection.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionContact.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionContact.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionEvents.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionEvents.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionExternalContent.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionExternalContent.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionFiles.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionFiles.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionGallery.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionGallery.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionHTML.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionHTML.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionLinks.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionLinks.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionMap.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionMap.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionNews.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionNews.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionPostit.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionPostit.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionSelections.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionSelections.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionSendinblue.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionSendinblue.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionSlide.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionSlide.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionText.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionText.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionVideo.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionVideo.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/types.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/types.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/default/workflows.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/default/workflows.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/icons/basic/registry.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/icons/basic/registry.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/icons/contenttypes/registry.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/icons/contenttypes/registry.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/last_compilation/registry.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/last_compilation/registry.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/testing/registry.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/testing/registry.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles/testing/types/Collection.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles/testing/types/Collection.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/profiles.zcml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/profiles.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/setuphandlers.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/subscribers.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/subscribers.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/subscribers.zcml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/subscribers.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/testing.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/testing.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/cirkwi_good_widget_mock.html` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/cirkwi_good_widget_mock.html`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_contact_category_raw_mock.json` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_contact_category_raw_mock.json`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_contact_empty_schedule_raw_mock.json` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_contact_empty_schedule_raw_mock.json`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_contact_images_raw_mock.json` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_contact_images_raw_mock.json`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_contact_raw_mock.json` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_contact_raw_mock.json`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_contacts_raw_mock.json` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_contacts_raw_mock.json`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_directory_entities_raw_mock.json` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_directory_entities_raw_mock.json`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_events_agendas_raw_mock.json` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_events_agendas_raw_mock.json`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_news_entities_raw_mock.json` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_news_entities_raw_mock.json`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_news_newsfolder_raw_mock.json` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_news_newsfolder_raw_mock.json`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_procedures_raw_mock.json` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_procedures_raw_mock.json`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_rest_directory.json` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_rest_directory.json`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_rest_events.json` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_rest_events.json`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_rest_events_with_breadcrumbs.json` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_rest_events_with_breadcrumbs.json`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_rest_news.json` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_rest_news.json`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_rest_specific_events.json` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_rest_specific_events.json`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/json_rest_specific_news.json` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/json_rest_specific_news.json`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/plone.png` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/plone.png`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/resources/plone.svg` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/resources/plone.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/robot/test_ct_folder.robot` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/robot/test_ct_folder.robot`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/robot/test_ct_page.robot` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/robot/test_ct_page.robot`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/robot/test_ct_procedure.robot` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/robot/test_ct_procedure.robot`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/robot/test_example.robot` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_banner.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_banner.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_behaviors.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_behaviors.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_categories.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_categories.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_chatbot.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_chatbot.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_cirkwiview.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_cirkwiview.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_cropping.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_cropping.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_default_pages.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_default_pages.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_faceted.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_faceted.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_folder.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_folder.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_footer.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_footer.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_herobanner.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_herobanner.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_icons.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_icons.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_indexes.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_indexes.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_instance_behaviors.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_instance_behaviors.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_local_roles.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_local_roles.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_logo.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_logo.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_minisite.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_minisite.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_navigation.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_navigation.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_page.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_page.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_plausibleview.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_plausibleview.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_portal_page.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_portal_page.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_procedure.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_procedure.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_rest.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_rest.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_robot.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_search.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_section_contact.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_section_contact.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_section_events.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_section_events.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_section_external_content.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_section_external_content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_section_news.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_section_news.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_section_sendinblue.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_section_sendinblue.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_sections.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_sections.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_setup.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_social.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_social.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_subsite.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_subsite.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_text.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_toolbar.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_toolbar.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_utils.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/test_vocabularies.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/test_vocabularies.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/tests/utils.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/tests/utils.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/configure.zcml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1020_to_1021/rolemap.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1020_to_1021/rolemap.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1022_to_1023/registry/icons.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1022_to_1023/registry/icons.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1023_to_1024/types/imio.smartweb.SectionPostit.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1023_to_1024/types/imio.smartweb.SectionPostit.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1030_to_1031/registry/resources.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1030_to_1031/registry/resources.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1031_to_1032/registry/spotlight.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1031_to_1032/registry/spotlight.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1035_to_1036/types/imio.smartweb.CirkwiView.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1035_to_1036/types/imio.smartweb.CirkwiView.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1038_to_1039/types/imio.smartweb.SectionExternalContent.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1038_to_1039/types/imio.smartweb.SectionExternalContent.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1040_to_1041/types/imio.smartweb.SectionText.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1040_to_1041/types/imio.smartweb.SectionText.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1045_to_1046/registry/plone.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1045_to_1046/registry/plone.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1046_to_1047/types/imio.smartweb.Folder.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1046_to_1047/types/imio.smartweb.Folder.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/registry/plone.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/registry/plone.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/types/imio.smartweb.DirectoryView.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/types/imio.smartweb.DirectoryView.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/types/imio.smartweb.EventsView.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/types/imio.smartweb.EventsView.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/types/imio.smartweb.Folder.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/types/imio.smartweb.Folder.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/types/imio.smartweb.NewsView.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/types/imio.smartweb.NewsView.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/types/imio.smartweb.SectionExternalContent.xml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/profiles/1047_to_1048/types/imio.smartweb.SectionExternalContent.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/upgrades/upgrades.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/upgrades/upgrades.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/utils.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/utils.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/actions.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/actions.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/arcgis_header.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/arcgis_header.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/banner.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/banner.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/banner.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/banner.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/chatbot.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/chatbot.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/configure.zcml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/default_page_warning.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/default_page_warning.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/footer.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/footer.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/footer.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/footer.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/header_actions.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/header_actions.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/herobanner.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/herobanner.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/herobanner.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/herobanner.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/logo.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/logo.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/logo.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/logo.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/messages.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/messages.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/minisite.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/minisite.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/navigation.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/navigation.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/offcanvas.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/offcanvas.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/procedure.pt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/procedure.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/procedure.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/procedure.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/subsite.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/subsite.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/viewlets/toolbar.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/viewlets/toolbar.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/vocabularies.py` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/vocabularies.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/vocabularies.zcml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/vocabularies.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/Makefile` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/Makefile`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/assets/layers-2x.8f2c4d11474275fbc1614b9098334eae.png` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/assets/layers-2x.8f2c4d11474275fbc1614b9098334eae.png`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/assets/layers.416d91365b44e4b4f4777663e6f009f3.png` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/assets/layers.416d91365b44e4b4f4777663e6f009f3.png`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/assets/marker-icon.2b3e1faf89f94a4835397e7a43b4f77d.png` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/assets/marker-icon.2b3e1faf89f94a4835397e7a43b4f77d.png`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/assets/next-react-white.819cb069ac8eec300a9db6a7707712d6.svg` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/assets/next-react-white.819cb069ac8eec300a9db6a7707712d6.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/assets/next-react.17bc43ff4a6a86f4520f5782f6a89a72.svg` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/assets/next-react.17bc43ff4a6a86f4520f5782f6a89a72.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/css/267.smartweb-webcomponents-compiled.css` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/css/267.smartweb-webcomponents-compiled.css`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/css/323.smartweb-webcomponents-compiled.css` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/css/323.smartweb-webcomponents-compiled.css`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/css/552.smartweb-webcomponents-compiled.css` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/css/552.smartweb-webcomponents-compiled.css`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/css/779.smartweb-webcomponents-compiled.css` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/css/779.smartweb-webcomponents-compiled.css`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/css/smartweb-webcomponents-compiled.css` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/css/smartweb-webcomponents-compiled.css`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/js/144.smartweb-webcomponents-compiled.js` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/js/144.smartweb-webcomponents-compiled.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/js/212.smartweb-webcomponents-compiled.js` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/js/212.smartweb-webcomponents-compiled.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/js/267.smartweb-webcomponents-compiled.js` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/js/267.smartweb-webcomponents-compiled.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/js/323.smartweb-webcomponents-compiled.js` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/js/323.smartweb-webcomponents-compiled.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/js/552.smartweb-webcomponents-compiled.js` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/js/552.smartweb-webcomponents-compiled.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/js/565.smartweb-webcomponents-compiled.js` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/js/565.smartweb-webcomponents-compiled.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/js/612.smartweb-webcomponents-compiled.js` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/js/612.smartweb-webcomponents-compiled.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/js/779.smartweb-webcomponents-compiled.js` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/js/779.smartweb-webcomponents-compiled.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/js/9.smartweb-webcomponents-compiled.js` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/js/9.smartweb-webcomponents-compiled.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/js/969.smartweb-webcomponents-compiled.js` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/js/969.smartweb-webcomponents-compiled.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/js/969.smartweb-webcomponents-compiled.js.LICENSE.txt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/js/969.smartweb-webcomponents-compiled.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/js/smartweb-webcomponents-compiled.js` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/js/smartweb-webcomponents-compiled.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/build/js/smartweb-webcomponents-compiled.js.LICENSE.txt` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/build/js/smartweb-webcomponents-compiled.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/package.json` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/package.json`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/pnpm-lock.yaml` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/pnpm-lock.yaml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/assets/facebook-news.svg` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/assets/facebook-news.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/assets/img-placeholder-bla.png` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/assets/img-placeholder-bla.png`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/assets/next-react-white.svg` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/assets/next-react-white.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/assets/next-react.svg` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/assets/next-react.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/assets/pin-active.svg` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/assets/pin-active.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/assets/pin.svg` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/assets/pin.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Annuaire.jsx` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Annuaire.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Annuaire.scss` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Annuaire.scss`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactCard/ContactCard.jsx` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactCard/ContactCard.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactContent/ContactContent.jsx` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactContent/ContactContent.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactList/ContactList.jsx` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactList/ContactList.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactMap/ContactMap.jsx` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactMap/ContactMap.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Filters/Filter.jsx` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Filters/Filter.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Skeleton/Skeleton.jsx` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Skeleton/Skeleton.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Events/ContactCard/ContactCard.jsx` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Events/ContactCard/ContactCard.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Events/ContactContent/ContactContent.jsx` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Events/ContactContent/ContactContent.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Events/ContactList/ContactList.jsx` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Events/ContactList/ContactList.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Events/ContactMap/ContactMap.jsx` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Events/ContactMap/ContactMap.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Events/Events.jsx` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Events/Events.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Events/Events.scss` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Events/Events.scss`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Events/Filters/Filter.jsx` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Events/Filters/Filter.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Events/Skeleton/Skeleton.jsx` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Events/Skeleton/Skeleton.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/News/ContactCard/ContactCard.jsx` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/News/ContactCard/ContactCard.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/News/ContactContent/ContactContent.jsx` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/News/ContactContent/ContactContent.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/News/ContactList/ContactList.jsx` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/News/ContactList/ContactList.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/News/ContactMap/ContactMap.jsx` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/News/ContactMap/ContactMap.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/News/Filters/Filter.jsx` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/News/Filters/Filter.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/News/News.jsx` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/News/News.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/News/News.scss` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/News/News.scss`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/News/Skeleton/Skeleton.jsx` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/News/Skeleton/Skeleton.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Search/ContactResult/ContactResult.jsx` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Search/ContactResult/ContactResult.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Search/EventsResult/EventsResult.jsx` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Search/EventsResult/EventsResult.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Search/Filters/Filter.jsx` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Search/Filters/Filter.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Search/NewsResult/NewsResult.jsx` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Search/NewsResult/NewsResult.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Search/Search.jsx` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Search/Search.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Search/Search.scss` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Search/Search.scss`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Search/Skeleton/Skeleton.jsx` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Search/Skeleton/Skeleton.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/components/Search/WebResult/WebResult.jsx` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/components/Search/WebResult/WebResult.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/hooks/useAxios.js` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/hooks/useAxios.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/index.jsx` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/index.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/index.scss` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/index.scss`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/src/utils/translation.js` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/src/utils/translation.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/webpack.config.js` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/webpack.config.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio/smartweb/core/webcomponents/webpackPlonePlugin.js` & `imio.smartweb.core-1.2.9/src/imio/smartweb/core/webcomponents/webpackPlonePlugin.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio.smartweb.core.egg-info/PKG-INFO` & `imio.smartweb.core-1.2.9/src/imio.smartweb.core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: imio.smartweb.core
-Version: 1.2.8
+Version: 1.2.9
 Summary: Core product for iMio websites
 Home-page: https://github.com/imio/imio.smartweb.core
 Author: Christophe Boulanger
 Author-email: christophe.boulanger@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/imio.smartweb.core
 Project-URL: Source, https://github.com/imio/imio.smartweb.core
 Project-URL: Tracker, https://github.com/imio/imio.smartweb.core/issues
 Keywords: Python Plone CMS
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 6.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -155,14 +154,21 @@
 - Thomas Lambert, thomas.lambert@imio.be
 
 
 Changelog
 =========
 
 
+1.2.9 (2023-11-24)
+------------------
+
+- WEB-4021 : Fix lead image displaying with files section
+  [boulch]
+
+
 1.2.8 (2023-11-23)
 ------------------
 
 - Fix (lead) image sizes URLs for text section & migrate old values
   [boulch, laulaz]
 
 
@@ -2011,9 +2017,7 @@
 
 
 1.0a1 (2021-04-19)
 ------------------
 
 - Initial release.
   [boulch]
-
-
```

### Comparing `imio.smartweb.core-1.2.8/src/imio.smartweb.core.egg-info/SOURCES.txt` & `imio.smartweb.core-1.2.9/src/imio.smartweb.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.2.8/src/imio.smartweb.core.egg-info/requires.txt` & `imio.smartweb.core-1.2.9/src/imio.smartweb.core.egg-info/requires.txt`

 * *Files identical despite different names*

