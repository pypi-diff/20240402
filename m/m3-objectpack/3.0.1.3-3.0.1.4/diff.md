# Comparing `tmp/m3-objectpack-3.0.1.3.tar.gz` & `tmp/m3-objectpack-3.0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/m3-objectpack-3.0.1.3.tar", last modified: Thu Feb 12 12:59:22 2015, max compression
+gzip compressed data, was "dist/m3-objectpack-3.0.1.4.tar", last modified: Wed Feb 18 08:23:37 2015, max compression
```

## Comparing `m3-objectpack-3.0.1.3.tar` & `m3-objectpack-3.0.1.4.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-12 12:59:22.000000 m3-objectpack-3.0.1.3/
--rw-rw-r--   0 travis    (1000) travis    (1000)       59 2015-02-12 12:59:22.000000 m3-objectpack-3.0.1.3/setup.cfg
--rw-rw-r--   0 travis    (1000) travis    (1000)      718 2015-02-12 12:59:22.000000 m3-objectpack-3.0.1.3/PKG-INFO
--rw-rw-r--   0 travis    (1000) travis    (1000)      971 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/setup.py
--rw-rw-r--   0 travis    (1000) travis    (1000)        0 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/README.rst
-lrwxrwxrwx   0 travis    (1000) travis    (1000)        0 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/README -> README.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)      133 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/MANIFEST.in
--rw-rw-r--   0 travis    (1000) travis    (1000)      121 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/DESCRIPTION
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-12 12:59:22.000000 m3-objectpack-3.0.1.3/src/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-12 12:59:22.000000 m3-objectpack-3.0.1.3/src/objectpack/
--rw-rw-r--   0 travis    (1000) travis    (1000)      249 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/version.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    45179 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/ui.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    15692 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/tools.py
--rw-rw-r--   0 travis    (1000) travis    (1000)      411 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/tests.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    20879 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/models.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    14450 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/filters.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1065 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/exceptions.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    11164 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/desktop.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1081 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/column_filters.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    80329 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/actions.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1655 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/__init__.py
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-12 12:59:22.000000 m3-objectpack-3.0.1.3/src/objectpack/tree_object_pack/
--rw-rw-r--   0 travis    (1000) travis    (1000)     1357 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/tree_object_pack/ui.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     5297 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/tree_object_pack/actions.py
--rw-rw-r--   0 travis    (1000) travis    (1000)      217 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/tree_object_pack/__init__.py
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-12 12:59:22.000000 m3-objectpack-3.0.1.3/src/objectpack/templates/
--rw-rw-r--   0 travis    (1000) travis    (1000)      271 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/templates/tabbed-window.js
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-12 12:59:22.000000 m3-objectpack-3.0.1.3/src/objectpack/static/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-12 12:59:22.000000 m3-objectpack-3.0.1.3/src/objectpack/static/js/
--rw-rw-r--   0 travis    (1000) travis    (1000)     2814 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/static/js/tree-select-window.js
--rw-rw-r--   0 travis    (1000) travis    (1000)     3318 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/static/js/objectpack-select-window.js
--rw-rw-r--   0 travis    (1000) travis    (1000)     5405 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/static/js/objectpack-multi-select-window.js
--rw-rw-r--   0 travis    (1000) travis    (1000)     1887 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/static/js/objectpack-master-detail-window.js
--rw-rw-r--   0 travis    (1000) travis    (1000)    94840 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/static/js/jquery-1.7.2.min.js
--rw-rw-r--   0 travis    (1000) travis    (1000)     9298 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/static/js/GridFilters.js
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-12 12:59:22.000000 m3-objectpack-3.0.1.3/src/objectpack/static/js/menu/
--rw-rw-r--   0 travis    (1000) travis    (1000)     2953 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/static/js/menu/TreeMenu.js
--rw-rw-r--   0 travis    (1000) travis    (1000)     1987 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/static/js/menu/RangeMenu.js
--rw-rw-r--   0 travis    (1000) travis    (1000)     3137 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/static/js/menu/ListMenu.js
--rw-rw-r--   0 travis    (1000) travis    (1000)     1600 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/static/js/menu/EditableItem.js
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-12 12:59:22.000000 m3-objectpack-3.0.1.3/src/objectpack/static/js/filter/
--rw-rw-r--   0 travis    (1000) travis    (1000)     1265 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/static/js/filter/StringFilter.js
--rw-rw-r--   0 travis    (1000) travis    (1000)     1244 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/static/js/filter/NumericFilter.js
--rw-rw-r--   0 travis    (1000) travis    (1000)      948 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/static/js/filter/ListFilter.js
--rw-rw-r--   0 travis    (1000) travis    (1000)     3726 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/static/js/filter/Filter.js
--rw-rw-r--   0 travis    (1000) travis    (1000)     3317 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/static/js/filter/DateFilter.js
--rw-rw-r--   0 travis    (1000) travis    (1000)     1196 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/static/js/filter/BooleanFilter.js
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-12 12:59:22.000000 m3-objectpack-3.0.1.3/src/objectpack/static/css/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-12 12:59:22.000000 m3-objectpack-3.0.1.3/src/objectpack/static/css/filter/
--rw-rw-r--   0 travis    (1000) travis    (1000)     1132 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/static/css/filter/style.css
--rw-rw-r--   0 travis    (1000) travis    (1000)    13131 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/static/css/filter/sort_filtered_desc.gif
--rw-rw-r--   0 travis    (1000) travis    (1000)    13129 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/static/css/filter/sort_filtered_asc.gif
--rw-rw-r--   0 travis    (1000) travis    (1000)      354 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/static/css/filter/less_then.png
--rw-rw-r--   0 travis    (1000) travis    (1000)       58 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/static/css/filter/header_bg.gif
--rw-rw-r--   0 travis    (1000) travis    (1000)      607 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/static/css/filter/hd-btn.gif
--rw-rw-r--   0 travis    (1000) travis    (1000)      359 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/static/css/filter/greater_then.png
--rw-rw-r--   0 travis    (1000) travis    (1000)      659 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/static/css/filter/find.png
--rw-rw-r--   0 travis    (1000) travis    (1000)      217 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/static/css/filter/equals.png
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-12 12:59:22.000000 m3-objectpack-3.0.1.3/src/objectpack/slave_object_pack/
--rwxrwxr-x   0 travis    (1000) travis    (1000)     3090 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/slave_object_pack/actions.py
--rwxrwxr-x   0 travis    (1000) travis    (1000)       71 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/slave_object_pack/__init__.py
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-12 12:59:22.000000 m3-objectpack-3.0.1.3/src/objectpack/observer/
--rw-rw-r--   0 travis    (1000) travis    (1000)      854 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/observer/tools.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    18477 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/observer/base.py
--rw-rw-r--   0 travis    (1000) travis    (1000)      273 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/observer/__init__.py
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-12 12:59:22.000000 m3-objectpack-3.0.1.3/src/objectpack/locale/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-12 12:59:22.000000 m3-objectpack-3.0.1.3/src/objectpack/locale/en/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-12 12:59:22.000000 m3-objectpack-3.0.1.3/src/objectpack/locale/en/LC_MESSAGES/
--rw-rw-r--   0 travis    (1000) travis    (1000)     2075 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/locale/en/LC_MESSAGES/django.po
--rw-rw-r--   0 travis    (1000) travis    (1000)     1209 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/locale/en/LC_MESSAGES/django.mo
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-12 12:59:22.000000 m3-objectpack-3.0.1.3/src/objectpack/dictionary_object_pack/
--rw-rw-r--   0 travis    (1000) travis    (1000)     1115 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/dictionary_object_pack/actions.py
--rw-rw-r--   0 travis    (1000) travis    (1000)      129 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/dictionary_object_pack/__init__.py
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-12 12:59:22.000000 m3-objectpack-3.0.1.3/src/objectpack/demo/
--rw-rw-r--   0 travis    (1000) travis    (1000)     1542 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/demo/ui.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     6003 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/demo/models.py
--rw-rw-r--   0 travis    (1000) travis    (1000)      742 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/demo/controller.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1052 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/demo/app_meta.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     8698 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/demo/actions.py
--rw-rw-r--   0 travis    (1000) travis    (1000)      119 2015-02-12 12:59:14.000000 m3-objectpack-3.0.1.3/src/objectpack/demo/__init__.py
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-12 12:59:22.000000 m3-objectpack-3.0.1.3/src/m3_objectpack.egg-info/
--rw-rw-r--   0 travis    (1000) travis    (1000)       11 2015-02-12 12:59:22.000000 m3-objectpack-3.0.1.3/src/m3_objectpack.egg-info/top_level.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)        1 2015-02-12 12:59:22.000000 m3-objectpack-3.0.1.3/src/m3_objectpack.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)     2421 2015-02-12 12:59:22.000000 m3-objectpack-3.0.1.3/src/m3_objectpack.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)      718 2015-02-12 12:59:22.000000 m3-objectpack-3.0.1.3/src/m3_objectpack.egg-info/PKG-INFO
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-18 08:23:37.000000 m3-objectpack-3.0.1.4/
+-rw-rw-r--   0 travis    (1000) travis    (1000)      971 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/setup.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)        0 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/README.rst
+-rw-rw-r--   0 travis    (1000) travis    (1000)       59 2015-02-18 08:23:37.000000 m3-objectpack-3.0.1.4/setup.cfg
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-18 08:23:37.000000 m3-objectpack-3.0.1.4/src/
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-18 08:23:37.000000 m3-objectpack-3.0.1.4/src/m3_objectpack.egg-info/
+-rw-rw-r--   0 travis    (1000) travis    (1000)        1 2015-02-18 08:23:37.000000 m3-objectpack-3.0.1.4/src/m3_objectpack.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (1000) travis    (1000)     2421 2015-02-18 08:23:37.000000 m3-objectpack-3.0.1.4/src/m3_objectpack.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (1000) travis    (1000)       11 2015-02-18 08:23:37.000000 m3-objectpack-3.0.1.4/src/m3_objectpack.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (1000) travis    (1000)      718 2015-02-18 08:23:37.000000 m3-objectpack-3.0.1.4/src/m3_objectpack.egg-info/PKG-INFO
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-18 08:23:37.000000 m3-objectpack-3.0.1.4/src/objectpack/
+-rw-rw-r--   0 travis    (1000) travis    (1000)    14457 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/filters.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)      411 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/tests.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    45183 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/ui.py
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-18 08:23:37.000000 m3-objectpack-3.0.1.4/src/objectpack/locale/
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-18 08:23:37.000000 m3-objectpack-3.0.1.4/src/objectpack/locale/en/
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-18 08:23:37.000000 m3-objectpack-3.0.1.4/src/objectpack/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 travis    (1000) travis    (1000)     2075 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/locale/en/LC_MESSAGES/django.po
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1209 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/locale/en/LC_MESSAGES/django.mo
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-18 08:23:37.000000 m3-objectpack-3.0.1.4/src/objectpack/slave_object_pack/
+-rwxrwxr-x   0 travis    (1000) travis    (1000)     3090 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/slave_object_pack/actions.py
+-rwxrwxr-x   0 travis    (1000) travis    (1000)       71 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/slave_object_pack/__init__.py
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-18 08:23:37.000000 m3-objectpack-3.0.1.4/src/objectpack/templates/
+-rw-rw-r--   0 travis    (1000) travis    (1000)      271 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/templates/tabbed-window.js
+-rw-rw-r--   0 travis    (1000) travis    (1000)    80283 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/actions.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    20879 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/models.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1655 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/__init__.py
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-18 08:23:37.000000 m3-objectpack-3.0.1.4/src/objectpack/demo/
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1052 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/demo/app_meta.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1542 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/demo/ui.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     8698 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/demo/actions.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     6003 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/demo/models.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)      119 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/demo/__init__.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)      742 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/demo/controller.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    11164 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/desktop.py
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-18 08:23:37.000000 m3-objectpack-3.0.1.4/src/objectpack/tree_object_pack/
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1357 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/tree_object_pack/ui.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     5297 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/tree_object_pack/actions.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)      217 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/tree_object_pack/__init__.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    15669 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/tools.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)      249 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/version.py
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-18 08:23:37.000000 m3-objectpack-3.0.1.4/src/objectpack/static/
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-18 08:23:37.000000 m3-objectpack-3.0.1.4/src/objectpack/static/js/
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-18 08:23:37.000000 m3-objectpack-3.0.1.4/src/objectpack/static/js/filter/
+-rw-rw-r--   0 travis    (1000) travis    (1000)      948 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/static/js/filter/ListFilter.js
+-rw-rw-r--   0 travis    (1000) travis    (1000)     3726 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/static/js/filter/Filter.js
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1196 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/static/js/filter/BooleanFilter.js
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1244 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/static/js/filter/NumericFilter.js
+-rw-rw-r--   0 travis    (1000) travis    (1000)     3317 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/static/js/filter/DateFilter.js
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1265 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/static/js/filter/StringFilter.js
+-rw-rw-r--   0 travis    (1000) travis    (1000)     9298 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/static/js/GridFilters.js
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-18 08:23:37.000000 m3-objectpack-3.0.1.4/src/objectpack/static/js/menu/
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1987 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/static/js/menu/RangeMenu.js
+-rw-rw-r--   0 travis    (1000) travis    (1000)     2953 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/static/js/menu/TreeMenu.js
+-rw-rw-r--   0 travis    (1000) travis    (1000)     3137 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/static/js/menu/ListMenu.js
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1600 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/static/js/menu/EditableItem.js
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1887 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/static/js/objectpack-master-detail-window.js
+-rw-rw-r--   0 travis    (1000) travis    (1000)     3318 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/static/js/objectpack-select-window.js
+-rw-rw-r--   0 travis    (1000) travis    (1000)    94840 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/static/js/jquery-1.7.2.min.js
+-rw-rw-r--   0 travis    (1000) travis    (1000)     2814 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/static/js/tree-select-window.js
+-rw-rw-r--   0 travis    (1000) travis    (1000)     5405 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/static/js/objectpack-multi-select-window.js
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-18 08:23:37.000000 m3-objectpack-3.0.1.4/src/objectpack/static/css/
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-18 08:23:37.000000 m3-objectpack-3.0.1.4/src/objectpack/static/css/filter/
+-rw-rw-r--   0 travis    (1000) travis    (1000)      607 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/static/css/filter/hd-btn.gif
+-rw-rw-r--   0 travis    (1000) travis    (1000)       58 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/static/css/filter/header_bg.gif
+-rw-rw-r--   0 travis    (1000) travis    (1000)    13129 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/static/css/filter/sort_filtered_asc.gif
+-rw-rw-r--   0 travis    (1000) travis    (1000)      659 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/static/css/filter/find.png
+-rw-rw-r--   0 travis    (1000) travis    (1000)      217 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/static/css/filter/equals.png
+-rw-rw-r--   0 travis    (1000) travis    (1000)      354 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/static/css/filter/less_then.png
+-rw-rw-r--   0 travis    (1000) travis    (1000)      359 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/static/css/filter/greater_then.png
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1132 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/static/css/filter/style.css
+-rw-rw-r--   0 travis    (1000) travis    (1000)    13131 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/static/css/filter/sort_filtered_desc.gif
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1065 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/exceptions.py
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-18 08:23:37.000000 m3-objectpack-3.0.1.4/src/objectpack/dictionary_object_pack/
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1115 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/dictionary_object_pack/actions.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)      129 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/dictionary_object_pack/__init__.py
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-02-18 08:23:37.000000 m3-objectpack-3.0.1.4/src/objectpack/observer/
+-rw-rw-r--   0 travis    (1000) travis    (1000)      273 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/observer/__init__.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)      854 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/observer/tools.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    18477 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/observer/base.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1081 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/src/objectpack/column_filters.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)      133 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/MANIFEST.in
+-rw-rw-r--   0 travis    (1000) travis    (1000)      718 2015-02-18 08:23:37.000000 m3-objectpack-3.0.1.4/PKG-INFO
+lrwxrwxrwx   0 travis    (1000) travis    (1000)        0 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/README -> README.rst
+-rw-rw-r--   0 travis    (1000) travis    (1000)      121 2015-02-18 08:23:28.000000 m3-objectpack-3.0.1.4/DESCRIPTION
```

### Comparing `m3-objectpack-3.0.1.3/PKG-INFO` & `m3-objectpack-3.0.1.4/src/m3_objectpack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: m3-objectpack
-Version: 3.0.1.3
+Version: 3.0.1.4
 Summary: Инструментарий для упрощения разработки реестров и справочников
 
 Home-page: https://bitbucket.org/barsgroup/objectpack
 Author: Alexey Pirogov
 Author-email: pirogov@bars-open.ru
 License: MIT
 Description: UNKNOWN
```

### Comparing `m3-objectpack-3.0.1.3/setup.py` & `m3-objectpack-3.0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     try:
         return open(os.path.join(os.path.dirname(__file__), fname)).read()
     except IOError:
         return ''
 
 setup(
     name="m3-objectpack",
-    version="3.0.1.3",
+    version="3.0.1.4",
     license='MIT',
     description=read('DESCRIPTION'),
     author="Alexey Pirogov",
     author_email="pirogov@bars-open.ru",
     url="https://bitbucket.org/barsgroup/objectpack",
     classifiers=[
         'Intended Audience :: Developers',
```

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/ui.py` & `m3-objectpack-3.0.1.4/src/objectpack/ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -775,15 +775,15 @@
         params = {'format': 'd.m.Y'}
         params.update(kwargs)
         ctl = ext.ExtDateField(**params)
 
     elif isinstance(f, django_models.TimeField):
         params = {'format': 'H:i', 'increment': 5}
         params.update(kwargs)
-        ctl = ExtTimeField(**params)
+        ctl = ext.ExtTimeField(**params)
 
     elif isinstance(f, django_models.ForeignKey):
         ctl = _create_dict_select_field(f, model_register, **kwargs)
 
     elif isinstance(f, django_models.ImageField):
         ctl = ext.ExtImageUploadField(**kwargs)
```

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/tools.py` & `m3-objectpack-3.0.1.4/src/objectpack/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -387,19 +387,16 @@
 # =============================================================================
 # istraversable - проверка на "обходимость"
 # =============================================================================
 def istraversable(obj):
     """
     возвращает True, если объект :attr:`obj` позволяет обход себя в цикле `for`
     """
-    return (
-        hasattr(obj, '__iter__')
-        or hasattr(obj, '__next__')
-        or hasattr(obj, '__getitem__')
-    )
+    return hasattr(obj, '__iter__') or hasattr(obj, '__next__') or hasattr(
+        obj, '__getitem__')
 
 
 # =============================================================================
 # Кэширующий декоратор
 # =============================================================================
 def cached_to(attr_name):
     """
```

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/models.py` & `m3-objectpack-3.0.1.4/src/objectpack/models.py`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/filters.py` & `m3-objectpack-3.0.1.4/src/objectpack/filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,15 +243,15 @@
         self._tooltip = tooltip
         self._field_fabric_params = field_fabric_params
         for bases, parser_key, default_lookup in self.parsers_map:
             if isinstance(self.field, bases):
                 self._parser = DeclarativeActionContext._parsers[parser_key]
                 break
         else:
-            raise TypeError('Unsupported field type: %r' % fld)
+            raise TypeError('Unsupported field type: %r' % self.field)
         lookup = lookup or default_lookup
         if lookup:
             # шаблонизация лукапа, если петтерн указан
             if not callable(lookup) and '%s' in lookup:
                 lookup = lookup % field_name
         else:
             lookup = lambda x: models.Q(**{field_name: x})
```

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/exceptions.py` & `m3-objectpack-3.0.1.4/src/objectpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/desktop.py` & `m3-objectpack-3.0.1.4/src/objectpack/desktop.py`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/column_filters.py` & `m3-objectpack-3.0.1.4/src/objectpack/column_filters.py`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/actions.py` & `m3-objectpack-3.0.1.4/src/objectpack/actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,17 +92,15 @@
         Если определен perm_code, то необходимость проверки прав
         будет зависеть от присутствия perm_code среди sub_permissions пака
         и соответствующего флага пака
 
         :rtype: bool
         """
         if self.perm_code is not None:
-            result = (
-                self.parent.need_check_permission
-                and
+            result = self.parent.need_check_permission and (
                 self.perm_code in self.parent.sub_permissions
             )
         else:
             result = False
         return result
 
     @staticmethod
@@ -1233,16 +1231,16 @@
             #: Экшен сохранения объекта
             self.save_action = ObjectSaveAction()
             self.actions.append(self.save_action)
         else:
             self.save_action = None
 
         if self.can_delete is None:
-            self.can_delete = (self.add_window
-                               or self.edit_window) and not self.read_only
+            self.can_delete = (
+                self.add_window or self.edit_window) and not self.read_only
         if self.can_delete:
             #: Экшен удаления объектовы
             self.delete_action = ObjectDeleteAction()
             self.actions.append(self.delete_action)
         else:
             self.delete_action = None
```

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/__init__.py` & `m3-objectpack-3.0.1.4/src/objectpack/__init__.py`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/tree_object_pack/ui.py` & `m3-objectpack-3.0.1.4/src/objectpack/tree_object_pack/ui.py`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/tree_object_pack/actions.py` & `m3-objectpack-3.0.1.4/src/objectpack/tree_object_pack/actions.py`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/static/js/tree-select-window.js` & `m3-objectpack-3.0.1.4/src/objectpack/static/js/tree-select-window.js`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/static/js/objectpack-select-window.js` & `m3-objectpack-3.0.1.4/src/objectpack/static/js/objectpack-select-window.js`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/static/js/objectpack-multi-select-window.js` & `m3-objectpack-3.0.1.4/src/objectpack/static/js/objectpack-multi-select-window.js`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/static/js/objectpack-master-detail-window.js` & `m3-objectpack-3.0.1.4/src/objectpack/static/js/objectpack-master-detail-window.js`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/static/js/jquery-1.7.2.min.js` & `m3-objectpack-3.0.1.4/src/objectpack/static/js/jquery-1.7.2.min.js`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/static/js/GridFilters.js` & `m3-objectpack-3.0.1.4/src/objectpack/static/js/GridFilters.js`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/static/js/menu/TreeMenu.js` & `m3-objectpack-3.0.1.4/src/objectpack/static/js/menu/TreeMenu.js`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/static/js/menu/RangeMenu.js` & `m3-objectpack-3.0.1.4/src/objectpack/static/js/menu/RangeMenu.js`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/static/js/menu/ListMenu.js` & `m3-objectpack-3.0.1.4/src/objectpack/static/js/menu/ListMenu.js`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/static/js/menu/EditableItem.js` & `m3-objectpack-3.0.1.4/src/objectpack/static/js/menu/EditableItem.js`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/static/js/filter/StringFilter.js` & `m3-objectpack-3.0.1.4/src/objectpack/static/js/filter/StringFilter.js`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/static/js/filter/NumericFilter.js` & `m3-objectpack-3.0.1.4/src/objectpack/static/js/filter/NumericFilter.js`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/static/js/filter/ListFilter.js` & `m3-objectpack-3.0.1.4/src/objectpack/static/js/filter/ListFilter.js`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/static/js/filter/Filter.js` & `m3-objectpack-3.0.1.4/src/objectpack/static/js/filter/Filter.js`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/static/js/filter/DateFilter.js` & `m3-objectpack-3.0.1.4/src/objectpack/static/js/filter/DateFilter.js`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/static/js/filter/BooleanFilter.js` & `m3-objectpack-3.0.1.4/src/objectpack/static/js/filter/BooleanFilter.js`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/static/css/filter/style.css` & `m3-objectpack-3.0.1.4/src/objectpack/static/css/filter/style.css`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/static/css/filter/sort_filtered_desc.gif` & `m3-objectpack-3.0.1.4/src/objectpack/static/css/filter/sort_filtered_desc.gif`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/static/css/filter/sort_filtered_asc.gif` & `m3-objectpack-3.0.1.4/src/objectpack/static/css/filter/sort_filtered_asc.gif`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/static/css/filter/hd-btn.gif` & `m3-objectpack-3.0.1.4/src/objectpack/static/css/filter/hd-btn.gif`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/static/css/filter/find.png` & `m3-objectpack-3.0.1.4/src/objectpack/static/css/filter/find.png`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/slave_object_pack/actions.py` & `m3-objectpack-3.0.1.4/src/objectpack/slave_object_pack/actions.py`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/observer/tools.py` & `m3-objectpack-3.0.1.4/src/objectpack/observer/tools.py`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/observer/base.py` & `m3-objectpack-3.0.1.4/src/objectpack/observer/base.py`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/locale/en/LC_MESSAGES/django.po` & `m3-objectpack-3.0.1.4/src/objectpack/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/locale/en/LC_MESSAGES/django.mo` & `m3-objectpack-3.0.1.4/src/objectpack/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/dictionary_object_pack/actions.py` & `m3-objectpack-3.0.1.4/src/objectpack/dictionary_object_pack/actions.py`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/demo/ui.py` & `m3-objectpack-3.0.1.4/src/objectpack/demo/ui.py`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/demo/models.py` & `m3-objectpack-3.0.1.4/src/objectpack/demo/models.py`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/demo/controller.py` & `m3-objectpack-3.0.1.4/src/objectpack/demo/controller.py`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/demo/app_meta.py` & `m3-objectpack-3.0.1.4/src/objectpack/demo/app_meta.py`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/objectpack/demo/actions.py` & `m3-objectpack-3.0.1.4/src/objectpack/demo/actions.py`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/m3_objectpack.egg-info/SOURCES.txt` & `m3-objectpack-3.0.1.4/src/m3_objectpack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `m3-objectpack-3.0.1.3/src/m3_objectpack.egg-info/PKG-INFO` & `m3-objectpack-3.0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: m3-objectpack
-Version: 3.0.1.3
+Version: 3.0.1.4
 Summary: Инструментарий для упрощения разработки реестров и справочников
 
 Home-page: https://bitbucket.org/barsgroup/objectpack
 Author: Alexey Pirogov
 Author-email: pirogov@bars-open.ru
 License: MIT
 Description: UNKNOWN
```

