# Comparing `tmp/imio.smartweb.locales-1.1.8.tar.gz` & `tmp/imio.smartweb.locales-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/imio.smartweb.locales-1.1.8.tar", last modified: Wed Oct 25 19:31:49 2023, max compression
+gzip compressed data, was "imio.smartweb.locales-1.1.9.tar", last modified: Mon Nov 20 08:12:20 2023, max compression
```

## Comparing `imio.smartweb.locales-1.1.8.tar` & `imio.smartweb.locales-1.1.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/
--rw-r--r--   0 laurent    (501) staff       (20)     4213 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/CHANGES.rst
--rw-r--r--   0 laurent    (501) staff       (20)      106 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/CONTRIBUTORS.rst
--rw-r--r--   0 laurent    (501) staff       (20)    18092 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/LICENSE.GPL
--rw-r--r--   0 laurent    (501) staff       (20)      656 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/LICENSE.rst
--rw-r--r--   0 laurent    (501) staff       (20)       61 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/MANIFEST.in
--rw-r--r--   0 laurent    (501) staff       (20)     7054 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/PKG-INFO
--rw-r--r--   0 laurent    (501) staff       (20)     1696 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/README.rst
--rw-r--r--   0 laurent    (501) staff       (20)      518 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/setup.cfg
--rw-r--r--   0 laurent    (501) staff       (20)     1722 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/setup.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/src/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/src/imio/
--rw-r--r--   0 laurent    (501) staff       (20)       80 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/src/imio/__init__.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/src/imio/smartweb/
--rw-r--r--   0 laurent    (501) staff       (20)       80 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/src/imio/smartweb/__init__.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/src/imio/smartweb/locales/
--rw-r--r--   0 laurent    (501) staff       (20)      151 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/src/imio/smartweb/locales/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)      204 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/src/imio/smartweb/locales/configure.zcml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/src/imio/smartweb/locales/locales/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/src/imio/smartweb/locales/locales/de/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/src/imio/smartweb/locales/locales/de/LC_MESSAGES/
--rw-r--r--   0 laurent    (501) staff       (20)    99901 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/src/imio/smartweb/locales/locales/de/LC_MESSAGES/imio.smartweb.po
--rw-r--r--   0 laurent    (501) staff       (20)     1568 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/src/imio/smartweb/locales/locales/de/LC_MESSAGES/plone.po
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/src/imio/smartweb/locales/locales/fr/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/src/imio/smartweb/locales/locales/fr/LC_MESSAGES/
--rw-r--r--   0 laurent    (501) staff       (20)   101444 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/src/imio/smartweb/locales/locales/fr/LC_MESSAGES/imio.smartweb.po
--rw-r--r--   0 laurent    (501) staff       (20)     1579 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/src/imio/smartweb/locales/locales/fr/LC_MESSAGES/plone.po
--rw-r--r--   0 laurent    (501) staff       (20)    82466 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/src/imio/smartweb/locales/locales/imio.smartweb.pot
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/src/imio/smartweb/locales/locales/nl/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/src/imio/smartweb/locales/locales/nl/LC_MESSAGES/
--rw-r--r--   0 laurent    (501) staff       (20)    82293 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/src/imio/smartweb/locales/locales/nl/LC_MESSAGES/imio.smartweb.po
--rw-r--r--   0 laurent    (501) staff       (20)     1133 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/src/imio/smartweb/locales/locales/nl/LC_MESSAGES/plone.po
--rw-r--r--   0 laurent    (501) staff       (20)     1236 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/src/imio/smartweb/locales/locales/plone-manual.pot
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/src/imio.smartweb.locales.egg-info/
--rw-r--r--   0 laurent    (501) staff       (20)     7054 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/src/imio.smartweb.locales.egg-info/PKG-INFO
--rw-r--r--   0 laurent    (501) staff       (20)     1049 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/src/imio.smartweb.locales.egg-info/SOURCES.txt
--rw-r--r--   0 laurent    (501) staff       (20)        1 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/src/imio.smartweb.locales.egg-info/dependency_links.txt
--rw-r--r--   0 laurent    (501) staff       (20)       19 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/src/imio.smartweb.locales.egg-info/namespace_packages.txt
--rw-r--r--   0 laurent    (501) staff       (20)        1 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/src/imio.smartweb.locales.egg-info/not-zip-safe
--rw-r--r--   0 laurent    (501) staff       (20)       11 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/src/imio.smartweb.locales.egg-info/requires.txt
--rw-r--r--   0 laurent    (501) staff       (20)        5 2023-10-25 19:31:49.000000 imio.smartweb.locales-1.1.8/src/imio.smartweb.locales.egg-info/top_level.txt
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-20 08:12:20.790019 imio.smartweb.locales-1.1.9/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4347 2023-11-20 08:12:20.000000 imio.smartweb.locales-1.1.9/CHANGES.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      106 2023-11-20 08:12:20.000000 imio.smartweb.locales-1.1.9/CONTRIBUTORS.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    18092 2023-11-20 08:12:20.000000 imio.smartweb.locales-1.1.9/LICENSE.GPL
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      656 2023-11-20 08:12:20.000000 imio.smartweb.locales-1.1.9/LICENSE.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       61 2023-11-20 08:12:20.000000 imio.smartweb.locales-1.1.9/MANIFEST.in
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7168 2023-11-20 08:12:20.790019 imio.smartweb.locales-1.1.9/PKG-INFO
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1696 2023-11-20 08:12:20.000000 imio.smartweb.locales-1.1.9/README.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      518 2023-11-20 08:12:20.790019 imio.smartweb.locales-1.1.9/setup.cfg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1722 2023-11-20 08:12:20.000000 imio.smartweb.locales-1.1.9/setup.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-20 08:12:20.786019 imio.smartweb.locales-1.1.9/src/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-20 08:12:20.790019 imio.smartweb.locales-1.1.9/src/imio/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-11-20 08:12:20.000000 imio.smartweb.locales-1.1.9/src/imio/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-20 08:12:20.790019 imio.smartweb.locales-1.1.9/src/imio/smartweb/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-11-20 08:12:20.000000 imio.smartweb.locales-1.1.9/src/imio/smartweb/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-20 08:12:20.790019 imio.smartweb.locales-1.1.9/src/imio/smartweb/locales/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      151 2023-11-20 08:12:20.000000 imio.smartweb.locales-1.1.9/src/imio/smartweb/locales/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      204 2023-11-20 08:12:20.000000 imio.smartweb.locales-1.1.9/src/imio/smartweb/locales/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-20 08:12:20.790019 imio.smartweb.locales-1.1.9/src/imio/smartweb/locales/locales/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-20 08:12:20.786019 imio.smartweb.locales-1.1.9/src/imio/smartweb/locales/locales/de/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-20 08:12:20.790019 imio.smartweb.locales-1.1.9/src/imio/smartweb/locales/locales/de/LC_MESSAGES/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)   100284 2023-11-20 08:12:20.000000 imio.smartweb.locales-1.1.9/src/imio/smartweb/locales/locales/de/LC_MESSAGES/imio.smartweb.po
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1568 2023-11-20 08:12:20.000000 imio.smartweb.locales-1.1.9/src/imio/smartweb/locales/locales/de/LC_MESSAGES/plone.po
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-20 08:12:20.786019 imio.smartweb.locales-1.1.9/src/imio/smartweb/locales/locales/fr/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-20 08:12:20.790019 imio.smartweb.locales-1.1.9/src/imio/smartweb/locales/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)   101882 2023-11-20 08:12:20.000000 imio.smartweb.locales-1.1.9/src/imio/smartweb/locales/locales/fr/LC_MESSAGES/imio.smartweb.po
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1579 2023-11-20 08:12:20.000000 imio.smartweb.locales-1.1.9/src/imio/smartweb/locales/locales/fr/LC_MESSAGES/plone.po
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    82889 2023-11-20 08:12:20.000000 imio.smartweb.locales-1.1.9/src/imio/smartweb/locales/locales/imio.smartweb.pot
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-20 08:12:20.786019 imio.smartweb.locales-1.1.9/src/imio/smartweb/locales/locales/nl/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-20 08:12:20.790019 imio.smartweb.locales-1.1.9/src/imio/smartweb/locales/locales/nl/LC_MESSAGES/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    82716 2023-11-20 08:12:20.000000 imio.smartweb.locales-1.1.9/src/imio/smartweb/locales/locales/nl/LC_MESSAGES/imio.smartweb.po
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1133 2023-11-20 08:12:20.000000 imio.smartweb.locales-1.1.9/src/imio/smartweb/locales/locales/nl/LC_MESSAGES/plone.po
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1236 2023-11-20 08:12:20.000000 imio.smartweb.locales-1.1.9/src/imio/smartweb/locales/locales/plone-manual.pot
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-11-20 08:12:20.790019 imio.smartweb.locales-1.1.9/src/imio.smartweb.locales.egg-info/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7168 2023-11-20 08:12:20.000000 imio.smartweb.locales-1.1.9/src/imio.smartweb.locales.egg-info/PKG-INFO
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1049 2023-11-20 08:12:20.000000 imio.smartweb.locales-1.1.9/src/imio.smartweb.locales.egg-info/SOURCES.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2023-11-20 08:12:20.000000 imio.smartweb.locales-1.1.9/src/imio.smartweb.locales.egg-info/dependency_links.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       19 2023-11-20 08:12:20.000000 imio.smartweb.locales-1.1.9/src/imio.smartweb.locales.egg-info/namespace_packages.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2023-11-20 08:12:20.000000 imio.smartweb.locales-1.1.9/src/imio.smartweb.locales.egg-info/not-zip-safe
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       11 2023-11-20 08:12:20.000000 imio.smartweb.locales-1.1.9/src/imio.smartweb.locales.egg-info/requires.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        5 2023-11-20 08:12:20.000000 imio.smartweb.locales-1.1.9/src/imio.smartweb.locales.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `imio.smartweb.locales-1.1.8/CHANGES.rst` & `imio.smartweb.locales-1.1.9/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 Changelog
 =========
 
 
+1.1.9 (2023-11-20)
+------------------
+
+- WEB-4018 : Add missing French translations (new termes in directory vocabulary)
+  [boulch]
+
+
 1.1.8 (2023-10-25)
 ------------------
 
 - Add missing French translations
   [laulaz]
```

### Comparing `imio.smartweb.locales-1.1.8/LICENSE.GPL` & `imio.smartweb.locales-1.1.9/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `imio.smartweb.locales-1.1.8/LICENSE.rst` & `imio.smartweb.locales-1.1.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `imio.smartweb.locales-1.1.8/PKG-INFO` & `imio.smartweb.locales-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: imio.smartweb.locales
-Version: 1.1.8
+Version: 1.1.9
 Summary: Locales for iMio smartweb packages
 Home-page: https://github.com/imio/imio.smartweb.locales
 Author: iMio
 Author-email: christophe.boulanger@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/imio.smartweb.locales
 Project-URL: Source, https://github.com/imio/imio.smartweb.locales
 Project-URL: Tracker, https://github.com/imio/imio.smartweb.locales/issues
 Keywords: Python Plone CMS
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 5.2
 Classifier: Framework :: Plone :: 6.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -114,14 +113,21 @@
 - Affinitic, laurent.lasudry@affinitic.be
 
 
 Changelog
 =========
 
 
+1.1.9 (2023-11-20)
+------------------
+
+- WEB-4018 : Add missing French translations (new termes in directory vocabulary)
+  [boulch]
+
+
 1.1.8 (2023-10-25)
 ------------------
 
 - Add missing French translations
   [laulaz]
 
 
@@ -413,9 +419,7 @@
 
 
 1.0a1 (2021-04-19)
 ------------------
 
 - Initial release.
   [boulch]
-
-
```

### Comparing `imio.smartweb.locales-1.1.8/README.rst` & `imio.smartweb.locales-1.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `imio.smartweb.locales-1.1.8/setup.cfg` & `imio.smartweb.locales-1.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.locales-1.1.8/setup.py` & `imio.smartweb.locales-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="imio.smartweb.locales",
-    version="1.1.8",
+    version="1.1.9",
     description="Locales for iMio smartweb packages",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
```

### Comparing `imio.smartweb.locales-1.1.8/src/imio/smartweb/locales/locales/de/LC_MESSAGES/imio.smartweb.po` & `imio.smartweb.locales-1.1.9/src/imio/smartweb/locales/locales/de/LC_MESSAGES/imio.smartweb.po`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
 msgstr ""
 
 #: imio/smartweb/common/behaviors/configure.zcml:13
 msgid "Add topics on content types."
 msgstr "Ajouter une thématique transversale sur le contenu."
 
 #: imio/smartweb/common/interfaces.py:30
-#: imio/smartweb/core/contents/sections/contact/macros.pt:96
+#: imio/smartweb/core/contents/sections/contact/macros.pt:97
 #: imio/smartweb/core/vocabularies.py:175
 msgid "Address"
 msgstr "Adresse"
 
 #: imio/smartweb/common/vocabularies.py:108
 msgid "Affiche"
 msgstr ""
@@ -227,15 +227,15 @@
 msgid "Allow to select quick access elements for current context."
 msgstr "Permet de sélectionner des éléments Accès Direct pour l'élément courant."
 
 #: imio/smartweb/core/contents/sections/slide/content.py:53
 msgid "Alternatively as a picture"
 msgstr "Comme alternative à une image"
 
-#: imio/smartweb/core/contents/folder/views.py:134
+#: imio/smartweb/core/contents/folder/views.py:135
 msgid "Apply"
 msgstr "Appliquer"
 
 #: imio/smartweb/core/viewlets/toolbar.py:169
 msgid "Ask a question"
 msgstr "Stelle eine Frage"
 
@@ -264,15 +264,15 @@
 msgid "Bad URL format '${val}' (good format sample: https://www.imio.be)."
 msgstr "Mauvais format d'URL pour '${val}' (format correct: https://www.imio.be)."
 
 #: imio/directory/core/browser/import.py:90
 msgid "Bad mail format '${val}' (good format sample: noreply@imio.be)."
 msgstr "Mauvais format d'email pour '${val}' (format correct: noreply@imio.be)."
 
-#: imio/directory/core/contents/contact/content.py:47
+#: imio/directory/core/contents/contact/content.py:65
 msgid "Bad phone format"
 msgstr "Mauvais format de téléphone"
 
 #: imio/directory/core/browser/import.py:72
 msgid "Bad phone format '${val}' (good format sample: +32444556677)."
 msgstr "Mauvais format de numéro de téléphone pour '${val}' (format correct: +32444556677)."
 
@@ -300,18 +300,22 @@
 msgid "Block view with images"
 msgstr "Affichage blocs avec images"
 
 #: imio/smartweb/core/profiles/icons/contenttypes/registry.xml
 msgid "BlockLink content type icon"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/content.py:35
+#: imio/smartweb/core/contents/sections/contact/content.py:36
 msgid "Blocks that will be displayed in contact"
 msgstr "Blocs qui vont être affichés dans le contact"
 
+#: imio/directory/core/vocabularies.py:89
+msgid "Bottle bubbles"
+msgstr ""
+
 #: imio/smartweb/core/vocabularies.py:311
 msgid "Bottom"
 msgstr "Bas"
 
 #: imio/smartweb/core/upgrades/configure.zcml:68
 msgid "By default, Plone open external (Section text / Tiny) links in new tab"
 msgstr ""
@@ -486,15 +490,15 @@
 msgstr "Choisissez d'accepter ou de refuser certains cookies.<br/>Notre <a href=\"${policy_url}\">politique en matière de cookies</a> peut vous aider à faire ce choix."
 
 #: imio/smartweb/core/behaviors/minisite.py:48
 #: imio/smartweb/core/behaviors/subsite.py:40
 msgid "Choose your display mode"
 msgstr "Choisissez votre mode d'affichage"
 
-#: imio/smartweb/core/contents/sections/contact/content.py:56
+#: imio/smartweb/core/contents/sections/contact/content.py:52
 msgid "Choose your gallery layout mode"
 msgstr "Choisissez votre mode d'affichage de galerie"
 
 #: imio/directory/core/contents/entity/content.py:23
 #: imio/events/core/contents/entity/content.py:19
 #: imio/news/core/contents/entity/content.py:19
 msgid "Choose zip codes for this entity"
@@ -601,18 +605,22 @@
 msgid "Click to preview content (without editor actions)."
 msgstr "Prévisualiser le contenu (sans les boutons d'édition)."
 
 #: imio/smartweb/core/viewlets/navigation.py:85
 msgid "Close"
 msgstr "Fermer"
 
-#: imio/smartweb/core/contents/sections/contact/utils.py:239
+#: imio/smartweb/core/contents/sections/contact/utils.py:244
 msgid "Closed"
 msgstr "Fermé"
 
+#: imio/directory/core/vocabularies.py:90
+msgid "Clothing bubbles"
+msgstr ""
+
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionCollection.xml
 msgid "Collection section"
 msgstr "Section collection"
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionCollection.xml
 msgid "Collection section for a page"
 msgstr "Section collection pour une page"
@@ -652,15 +660,15 @@
 msgid "Contact"
 msgstr "Contact"
 
 #: imio/directory/core/profiles/default/types/imio.directory.Contact.xml
 msgid "Contact content type"
 msgstr "Contact"
 
-#: imio/directory/core/contents/contact/content.py:137
+#: imio/directory/core/contents/contact/content.py:155
 #: imio/smartweb/core/vocabularies.py:174
 msgid "Contact informations"
 msgstr "Coordonnées"
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionContact.xml
 msgid "Contact section"
 msgstr "Section contact"
@@ -673,14 +681,18 @@
 msgid "Contact title is missing."
 msgstr "Le titre du contact est manquant."
 
 #: imio/directory/core/browser/import.py:201
 msgid "Contact type is missing."
 msgstr "Le type de contact est manquant."
 
+#: imio/directory/core/vocabularies.py:91
+msgid "Container parks"
+msgstr ""
+
 #: imio/smartweb/common/browser/privacy/form.py:12
 msgid "Cookies choice"
 msgstr "Choix des cookies"
 
 #: imio/smartweb/common/viewlets/colophon.pt:19
 msgid "Cookies preferences"
 msgstr "Gestion des cookies"
@@ -725,15 +737,15 @@
 msgid "Define number of levels in menu navigation subsite"
 msgstr "Définir un nombre de niveaux pour le menu de navigation du sous-site"
 
 #: imio/smartweb/core/contents/sections/macros.pt:53
 msgid "Delete section"
 msgstr "Supprimer la section"
 
-#: imio/directory/core/contents/contact/content.py:240
+#: imio/directory/core/contents/contact/content.py:258
 #: imio/events/core/contents/event/content.py:56
 #: imio/news/core/contents/newsitem/content.py:42
 msgid "Description"
 msgstr "Description"
 
 #: imio/smartweb/core/browser/controlpanel.py:72
 msgid "Directory SolR Core ID"
@@ -801,29 +813,29 @@
 msgid "Display map"
 msgstr ""
 
 #: imio/directory/core/vocabularies.py:85
 msgid "Drinking water point"
 msgstr "Points d'eau potable"
 
-#: imio/directory/core/contents/contact/content.py:263
+#: imio/directory/core/contents/contact/content.py:281
 #: imio/events/core/contents/event/content.py:80
 #: imio/news/core/contents/newsitem/content.py:66
 msgid "Dutch translations"
 msgstr "Traductions néerlandophones"
 
 #: imio/smartweb/core/contents/pages/procedure/content.py:21
 msgid "E-Guichet procedure"
 msgstr "Lien vers la démarche dans l'e-guichet iMio"
 
-#: imio/directory/core/contents/contact/content.py:112
+#: imio/directory/core/contents/contact/content.py:130
 msgid "E-mail"
 msgstr "Adresse e-mail"
 
-#: imio/directory/core/contents/contact/content.py:152
+#: imio/directory/core/contents/contact/content.py:170
 msgid "E-mails"
 msgstr ""
 
 #: imio/smartweb/common/vocabularies.py:22
 msgid "Economics"
 msgstr "Économie"
 
@@ -855,15 +867,15 @@
 msgid "Enable minisite"
 msgstr "Activer le mode site partenaire"
 
 #: imio/smartweb/core/profiles/default/actions.xml
 msgid "Enable subsite"
 msgstr "Activer le mode sous-site"
 
-#: imio/directory/core/contents/contact/content.py:246
+#: imio/directory/core/contents/contact/content.py:264
 #: imio/events/core/contents/event/content.py:63
 #: imio/news/core/contents/newsitem/content.py:49
 msgid "English translations"
 msgstr "Traductions anglophones"
 
 #: imio/smartweb/core/browser/controlpanel.py:17
 msgid "Enter the language code. Ex.: en"
@@ -969,15 +981,15 @@
 msgid "Example : namur.be (SMARTWEB_PLAUSIBLE_SITE varenv has precedence over this.)"
 msgstr "Beispiel :  namur.be (SMARTWEB_PLAUSIBLE_SITE varenv hat hier Vorrang.)"
 
 #: imio/smartweb/core/browser/controlpanel.py:146
 msgid "Example : plausible.imio.be (SMARTWEB_PLAUSIBLE_URL varenv has precedence over this.)"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:300
+#: imio/directory/core/contents/contact/content.py:318
 msgid "Example : shop, service, association logo"
 msgstr "Exemple : Logo d'un magasin ou d'un service ou d'une association"
 
 #: imio/smartweb/core/behaviors/listing.py:19
 msgid "Exclude from parent listing"
 msgstr "Exclure dans l'affichage listing du parent"
 
@@ -1021,39 +1033,39 @@
 msgid "Facebook url for this event"
 msgstr "Lien facebook pour cet événement"
 
 #: imio/news/core/contents/newsitem/content.py:101
 msgid "Facebook url for this news"
 msgstr "Lien facebook pour cette actualité"
 
-#: imio/smartweb/core/browser/faceted/configure.zcml:67
+#: imio/smartweb/core/browser/faceted/configure.zcml:81
 msgid "Faceted block view"
 msgstr "Affichage blocs"
 
-#: imio/smartweb/core/browser/faceted/configure.zcml:74
+#: imio/smartweb/core/browser/faceted/configure.zcml:88
 msgid "Faceted block view with images"
 msgstr "Affichage blocs avec images"
 
 #: imio/smartweb/core/browser/faceted/configure.zcml:16
 msgid "Faceted items preview"
 msgstr ""
 
-#: imio/smartweb/core/browser/faceted/configure.zcml:97
+#: imio/smartweb/core/browser/faceted/configure.zcml:111
 msgid "Faceted map"
 msgstr "Affichage plan"
 
-#: imio/smartweb/core/browser/faceted/configure.zcml:81
+#: imio/smartweb/core/browser/faceted/configure.zcml:95
 msgid "Faceted summary view"
 msgstr "Affichage liste"
 
-#: imio/smartweb/core/browser/faceted/configure.zcml:88
+#: imio/smartweb/core/browser/faceted/configure.zcml:102
 msgid "Faceted summary view with images"
 msgstr "Affichage liste avec images"
 
-#: imio/directory/core/contents/contact/content.py:317
+#: imio/directory/core/contents/contact/content.py:335
 msgid "Facilities"
 msgstr "Facilités"
 
 #: imio/events/core/contents/event/content.py:154
 #: imio/events/core/contents/event/view.pt:57
 msgid "Facilities for person with reduced mobility"
 msgstr "Accessible aux personnes à mobilité réduite"
@@ -1134,15 +1146,15 @@
 msgid "Footer has been successfully added"
 msgstr "Le pied de page a été ajouté avec succès"
 
 #: imio/smartweb/core/contents/folder/content.py:26
 msgid "For the anonymous visitor, the folder and the selected item are one. When he clicks on the folder, the item is displayed."
 msgstr "Pour le visiteur anonyme, le dossier et l'élément sélectionné ne font qu'un. Lorsqu'il clique sur le dossier, l'élément s'affiche."
 
-#: imio/smartweb/core/contents/folder/views.py:105
+#: imio/smartweb/core/contents/folder/views.py:106
 msgid "Form to choose item to be displayed as the home page of the folder"
 msgstr "Formulaire de choix de l'élément à afficher comme page d'accueil du dossier"
 
 #: imio/directory/core/vocabularies.py:88
 msgid "Free WIFI"
 msgstr "Wifi gratuit"
 
@@ -1163,27 +1175,27 @@
 msgid "Full width"
 msgstr "Pleine page"
 
 #: imio/smartweb/core/vocabularies.py:180
 msgid "Gallery"
 msgstr "Galerie"
 
-#: imio/smartweb/core/contents/sections/contact/content.py:55
+#: imio/smartweb/core/contents/sections/contact/content.py:51
 msgid "Gallery mode"
 msgstr "Mode de galerie"
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionGallery.xml
 msgid "Gallery section"
 msgstr "Section galerie"
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionGallery.xml
 msgid "Gallery section for a page"
 msgstr "Création d'une section galerie qui affichera ses images dans votre page. "
 
-#: imio/directory/core/contents/contact/content.py:229
+#: imio/directory/core/contents/contact/content.py:247
 #: imio/events/core/contents/event/content.py:46
 #: imio/news/core/contents/newsitem/content.py:32
 msgid "German translations"
 msgstr "Traductions germanophones"
 
 #: imio/smartweb/core/contents/sections/events/content.py:37
 msgid "Get priory on related agenda for these specifics events."
@@ -1321,15 +1333,15 @@
 msgid "Image orientation"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/gallery/content.py:16
 msgid "Image scale for images"
 msgstr "Echelle d'images"
 
-#: imio/smartweb/core/contents/sections/contact/content.py:77
+#: imio/smartweb/core/contents/sections/contact/content.py:73
 msgid "Image scale for images (only for gallery mode)"
 msgstr "Echelle d'images (seulement en mode galerie)"
 
 #: imio/smartweb/core/contents/sections/text/content.py:24
 msgid "Image size"
 msgstr "Taille de l'image"
 
@@ -1352,15 +1364,15 @@
 msgstr "Important! Ces catégories sont utilisées pour créer des listes accessibles via le menu navigation"
 
 #: imio/events/core/contents/event/content.py:178
 #: imio/news/core/contents/newsitem/content.py:133
 msgid "Important! These categories are used to supplement the information provided by the topics"
 msgstr "Important! Ces catégories permettent de compléter l'information apportée par les thématiques"
 
-#: imio/directory/core/contents/contact/content.py:318
+#: imio/directory/core/contents/contact/content.py:336
 msgid "Important! These categories make it possible to highlight and geolocate certain basic services"
 msgstr "Important! Ces catégories permettent de mettre en avant et de géolocaliser certains services de base"
 
 #: imio/smartweb/common/behaviors/topics.py:17
 msgid "Important! Topics are used to filter search results and create lists"
 msgstr "Important! Les thématiques sont utilisées pour filtrer les résultats de la recherche et créer des listes"
 
@@ -1390,28 +1402,28 @@
 msgid "Installs the imio.events.policy add-on."
 msgstr ""
 
 #: imio/news/policy/configure.zcml:36
 msgid "Installs the imio.news.policy add-on."
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:210
+#: imio/directory/core/contents/contact/content.py:228
 msgid "Internal note"
 msgstr "Note interne"
 
 #: imio/events/core/vocabularies.py:25
 msgid "Internships and courses"
 msgstr "Stages et cours"
 
 #: imio/smartweb/core/contents/folder/content.py:25
 msgid "Item(s) that can be selected as the folder default page."
 msgstr "Elément(s) pouvant être sélectionné(s) comme page d'accueil du dossier."
 
 #: imio/events/core/contents/event/views.py:77
-#: imio/smartweb/core/contents/sections/contact/macros.pt:111
+#: imio/smartweb/core/contents/sections/contact/macros.pt:112
 #: imio/smartweb/core/contents/sections/contact/utils.py:56
 msgid "Itinerary"
 msgstr "Itinéraire"
 
 #: imio/news/core/vocabularies.py:17
 msgid "Job offer"
 msgstr "Emploi"
@@ -1425,19 +1437,19 @@
 msgstr "Journaliste"
 
 #: imio/events/core/contents/event/view.pt:107
 #: imio/news/core/contents/newsitem/view.pt:64
 msgid "Keywords"
 msgstr "Mots-clés"
 
-#: imio/directory/core/contents/contact/content.py:100
+#: imio/directory/core/contents/contact/content.py:118
 msgid "Label (Secretariat, Manager office, Sales,...)"
 msgstr "Intitulé (Secrétariat, Bureau de la direction, Ventes, ...)"
 
-#: imio/directory/core/contents/contact/content.py:79
+#: imio/directory/core/contents/contact/content.py:97
 msgid "Label (direction, Main number,...)"
 msgstr "Intitulé (direction, numéro principal, ...)"
 
 #: imio/smartweb/core/browser/controlpanel.py:16
 msgid "Language (en, fr,...)"
 msgstr "Langue (en, fr, ...)"
 
@@ -1519,30 +1531,30 @@
 msgid "List of news categories values available for this entity (one per line)"
 msgstr "Liste de catégories spécifiques d'actualités disponibes pour cette entité (une par ligne)"
 
 #: imio/smartweb/common/vocabularies.py:110
 msgid "Liste"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:299
+#: imio/directory/core/contents/contact/content.py:317
 #: imio/smartweb/core/behaviors/minisite.py:41
 #: imio/smartweb/core/behaviors/subsite.py:33
 msgid "Logo"
 msgstr "Logo"
 
 #: imio/smartweb/core/vocabularies.py:159
 msgid "Logo and title"
 msgstr "Logo et titre"
 
 #: imio/smartweb/core/behaviors/minisite.py:47
 #: imio/smartweb/core/behaviors/subsite.py:39
 msgid "Logo display"
 msgstr "Type d'affichage du logo"
 
-#: imio/smartweb/core/contents/sections/contact/utils.py:269
+#: imio/smartweb/core/contents/sections/contact/utils.py:274
 msgid "Lunch time"
 msgstr "Heure du midi"
 
 #: imio/smartweb/core/contents/sections/macros.pt:42
 msgid "Manage section contents"
 msgstr "Modifier contenu"
 
@@ -1564,19 +1576,19 @@
 
 #: imio/smartweb/core/contents/sections/collection/content.py:48
 #: imio/smartweb/core/contents/sections/events/content.py:70
 #: imio/smartweb/core/contents/sections/news/content.py:70
 msgid "Maximum number of batches to display"
 msgstr "Nombre maximum de lots à afficher"
 
-#: imio/smartweb/core/contents/sections/contact/content.py:69
+#: imio/smartweb/core/contents/sections/contact/content.py:65
 msgid "Maximum number of contacts by line"
 msgstr "Nombre maximum de contacts par ligne"
 
-#: imio/smartweb/core/contents/sections/contact/content.py:70
+#: imio/smartweb/core/contents/sections/contact/content.py:66
 msgid "Maximum number of contacts by line (on PC)"
 msgstr "Nombre maximum de contacts par ligne (sur un écran d'ordinateur)"
 
 #: imio/smartweb/core/behaviors/subsite.py:48
 msgid "Menu depth"
 msgstr "Profondeur du menu"
 
@@ -1697,25 +1709,25 @@
 msgid "Not allowed to add Files or Images in imio.directory.Entity"
 msgstr ""
 
 #: imio/smartweb/common/interfaces.py:34
 msgid "Number"
 msgstr "Numéro"
 
-#: imio/directory/core/contents/contact/content.py:92
+#: imio/directory/core/contents/contact/content.py:110
 msgid "Number (format: +32475010203)"
 msgstr "Numéro (format: +32475010203)"
 
 #: imio/smartweb/core/contents/sections/collection/content.py:41
 #: imio/smartweb/core/contents/sections/events/content.py:63
 #: imio/smartweb/core/contents/sections/files/content.py:15
 msgid "Number of items per batch"
 msgstr "Nombre d'éléments par lot"
 
-#: imio/smartweb/core/contents/sections/contact/content.py:62
+#: imio/smartweb/core/contents/sections/contact/content.py:58
 msgid "Number of items per batch (only for carousel mode)"
 msgstr "Nombre d'éléments par lot (seulement en mode carrousel)"
 
 #: imio/smartweb/core/contents/rest/directory/content.py:25
 #: imio/smartweb/core/contents/rest/events/content.py:30
 #: imio/smartweb/core/contents/rest/news/content.py:21
 msgid "Number of items to display"
@@ -1737,19 +1749,19 @@
 msgid "Only one procedure field can be filled !"
 msgstr "Un seul champ \"démarche\" peut être rempli !"
 
 #: imio/smartweb/core/contents/blocks/link/content.py:34
 msgid "Only used in table view (takes precedence over image)"
 msgstr "Utilisée uniquement dans l'affichage tableau (prend la priorité sur l'image)"
 
-#: imio/smartweb/core/contents/sections/contact/utils.py:246
+#: imio/smartweb/core/contents/sections/contact/utils.py:251
 msgid "Open"
 msgstr "Ouvert"
 
-#: imio/smartweb/core/contents/sections/contact/utils.py:263
+#: imio/smartweb/core/contents/sections/contact/utils.py:268
 msgid "Open at "
 msgstr "Ouvre à "
 
 #: imio/smartweb/core/contents/blocks/link/content.py:23
 #: imio/smartweb/core/contents/sections/slide/content.py:66
 msgid "Open in a new tab"
 msgstr "Ouvrir dans un nouvel onglet"
@@ -1818,30 +1830,34 @@
 msgid "Party and folklore"
 msgstr "Fête et folklore"
 
 #: imio/smartweb/common/upgrades/configure.zcml:69
 msgid "Patch (Remove select2) eea.facetednavigation jquery"
 msgstr ""
 
-#: imio/smartweb/core/vocabularies.py:142
+#: imio/smartweb/core/vocabularies.py:141
 msgid "Paysage"
 msgstr ""
 
 #: imio/directory/core/vocabularies.py:53
 msgid "Personal email"
 msgstr "Adresse e-mail personnelle"
 
 #: imio/directory/core/vocabularies.py:39
 msgid "Personal phone"
 msgstr "Numéro de téléphone personnel"
 
-#: imio/directory/core/contents/contact/content.py:142
+#: imio/directory/core/contents/contact/content.py:160
 msgid "Phones"
 msgstr "Téléphones"
 
+#: imio/smartweb/core/browser/faceted/configure.zcml:37
+msgid "Photo gallery"
+msgstr ""
+
 #: imio/smartweb/core/contents/sections/slide/content.py:41
 msgid "Picture will be displayed as slide background"
 msgstr "L'image est affichée en background du slide"
 
 #: imio/directory/core/vocabularies.py:68
 msgid "Pinterest"
 msgstr ""
@@ -1898,15 +1914,15 @@
 msgid "Portal Page content type to print informations"
 msgstr "Page Portail pour afficher de l'information"
 
 #: imio/smartweb/core/profiles/icons/contenttypes/registry.xml
 msgid "PortalPage content type icon"
 msgstr ""
 
-#: imio/smartweb/core/vocabularies.py:141
+#: imio/smartweb/core/vocabularies.py:142
 msgid "Portrait"
 msgstr ""
 
 #: imio/directory/core/vocabularies.py:20
 msgid "Position (mayor, alderman, advisor, director, head of department, etc.)"
 msgstr "Fonction (bourgmestre, échevin, conseiller, directeur, chef de service, etc.)"
 
@@ -1932,15 +1948,15 @@
 msgid "Presse"
 msgstr "Presse"
 
 #: imio/smartweb/core/profiles/default/actions.xml
 msgid "Preview"
 msgstr "Prévisualiser"
 
-#: imio/directory/core/contents/contact/content.py:175
+#: imio/directory/core/contents/contact/content.py:193
 msgid "Private contact informations"
 msgstr "Coordonnées privées"
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.Procedure.xml
 msgid "Procedure"
 msgstr "Démarche"
 
@@ -2001,15 +2017,15 @@
 msgid "Refuse all"
 msgstr "Tout refuser"
 
 #: imio/smartweb/core/contents/sections/events/content.py:30
 msgid "Related agenda"
 msgstr "Agenda lié"
 
-#: imio/smartweb/core/contents/sections/contact/content.py:23
+#: imio/smartweb/core/contents/sections/contact/content.py:24
 msgid "Related contacts"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/news/content.py:30
 msgid "Related news folder"
 msgstr "Dossier d'actualités lié"
 
@@ -2030,14 +2046,18 @@
 msgid "Remove plone.patternslib deprecated bundles"
 msgstr ""
 
 #: imio/news/policy/upgrades/configure.zcml:12
 msgid "Remove ugly IImioEventsPolicyLayer"
 msgstr ""
 
+#: imio/smartweb/policy/upgrades/configure.zcml:148
+msgid "Restore removed behaviors on Collection type"
+msgstr ""
+
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionText.xml
 msgid "Rich text section for a page"
 msgstr "Création d'une section de texte dans votre page."
 
 #: imio/smartweb/core/vocabularies.py:310
 msgid "Right"
 msgstr "Droite"
@@ -2050,15 +2070,15 @@
 msgid "Saturday"
 msgstr "Samedi"
 
 #: imio/smartweb/common/browser/privacy/form.py:27
 msgid "Save my choices"
 msgstr "Enregistrer mes choix"
 
-#: imio/smartweb/core/contents/sections/contact/macros.pt:121
+#: imio/smartweb/core/contents/sections/contact/macros.pt:122
 #: imio/smartweb/core/vocabularies.py:177
 msgid "Schedule"
 msgstr "Horaires"
 
 #: imio/smartweb/core/viewlets/searchbox.pt:9
 msgid "Search"
 msgstr "Rechercher"
@@ -2167,19 +2187,19 @@
 msgid "Select agenda to display"
 msgstr "Sélectionnez l'agenda à afficher"
 
 #: imio/events/core/contents/event/content.py:168
 msgid "Select agendas where this event will be displayed. Current agenda is always selected."
 msgstr "Sélectionnez les agendas dans lesquels cet événement sera affiché. L'agenda courant sera toujours sélectionné."
 
-#: imio/smartweb/core/contents/sections/contact/content.py:24
+#: imio/smartweb/core/contents/sections/contact/content.py:25
 msgid "Select contacts. If you can't find contacts you want, make sure it exists in the directory and that its \"state\" is published."
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:308
+#: imio/directory/core/contents/contact/content.py:326
 msgid "Select entities where this contact will be displayed. Current entity will always be selected."
 msgstr "Sélectionnez les entités dans lesquelles ce contact sera affiché. L'entité courante sera toujours sélectionnée."
 
 #: imio/smartweb/core/contents/sections/text/content.py:25
 msgid "Select image size"
 msgstr "Sélectionnez la taille de l'image"
 
@@ -2211,15 +2231,15 @@
 msgid "Selected agenda"
 msgstr "Agenda sélectionné"
 
 #: imio/events/core/contents/event/content.py:167
 msgid "Selected agendas"
 msgstr "Agendas concernés"
 
-#: imio/directory/core/contents/contact/content.py:307
+#: imio/directory/core/contents/contact/content.py:325
 msgid "Selected entities"
 msgstr "Entités concernées"
 
 #: imio/smartweb/core/contents/rest/events/content.py:17
 msgid "Selected event types"
 msgstr "Types d'événements sélectionnés"
 
@@ -2392,15 +2412,15 @@
 msgid "Subsite has been disabled"
 msgstr "Le mode sous-site a été désactivé"
 
 #: imio/smartweb/core/browser/subsite/settings.py:25
 msgid "Subsite has been successfully activated"
 msgstr "Le mode sous-site a été activé avec succès"
 
-#: imio/directory/core/contents/contact/content.py:239
+#: imio/directory/core/contents/contact/content.py:257
 #: imio/smartweb/core/contents/sections/postit/content.py:26
 msgid "Subtitle"
 msgstr "Sous-titre"
 
 #: imio/smartweb/core/contents/folder/configure.zcml:72
 msgid "Summary view"
 msgstr "Affichage liste"
@@ -2409,18 +2429,14 @@
 msgid "Summary view with images"
 msgstr "Affichage liste avec images"
 
 #: imio/smartweb/core/contents/sections/contact/utils.py:106
 msgid "Sunday"
 msgstr "Dimanche"
 
-#: imio/smartweb/core/contents/sections/contact/content.py:51
-msgid "Switch lead image to portrait mode"
-msgstr "Passer l'image de garde en mode portrait"
-
 #: imio/smartweb/core/contents/sections/links/configure.zcml:15
 #: imio/smartweb/core/contents/sections/selections/configure.zcml:15
 msgid "Table view"
 msgstr "Affichage tableau"
 
 #: imio/smartweb/core/viewlets/toolbar.py:183
 msgid "Take part of workshop"
@@ -2500,15 +2516,15 @@
 msgid "Third page"
 msgstr "Tiers de la page"
 
 #: imio/smartweb/common/privacy.py:70
 msgid "This feature requires cookies acceptation.<br/><a class=\"pat-plone-modal\" href=\"${consent_url}\">Review your cookies preferences</a>."
 msgstr "Cette fonctionnalité nécessite l'acceptation des cookies.<br/><a class=\"pat-plone-modal\" href=\"${consent_url}\">Modifier vos préférences en matière de cookies</a>."
 
-#: imio/directory/core/contents/contact/content.py:234
+#: imio/directory/core/contents/contact/content.py:252
 #: imio/events/core/contents/event/content.py:51
 #: imio/news/core/contents/newsitem/content.py:37
 msgid "This field is required if the content must be available in this language"
 msgstr "Ce champ est requis si le contenu doit être disponible dans cette langue"
 
 #: imio/smartweb/core/browser/controlpanel.py:91
 msgid "This information is used for search results redirection"
@@ -2531,15 +2547,15 @@
 msgid "Ticket url"
 msgstr "Billeterie"
 
 #: imio/events/core/contents/event/content.py:118
 msgid "Ticket url to subscribe to this event"
 msgstr "Lien de la billeterie pour s'inscrire à cet événement"
 
-#: imio/directory/core/contents/contact/content.py:233
+#: imio/directory/core/contents/contact/content.py:251
 #: imio/events/core/contents/event/content.py:50
 #: imio/news/core/contents/newsitem/content.py:36
 msgid "Title"
 msgstr "Titre"
 
 #: imio/smartweb/core/vocabularies.py:173
 msgid "Title and Subtitle"
@@ -2593,23 +2609,23 @@
 msgid "Twitter url for this news"
 msgstr "Lien Twitter pour cette actualité"
 
 #: imio/smartweb/core/vocabularies.py:127
 msgid "Two third of width"
 msgstr "Deux tiers de la page"
 
-#: imio/directory/core/contents/contact/content.py:85
+#: imio/directory/core/contents/contact/content.py:103
 msgid "Type"
 msgstr ""
 
 #: imio/smartweb/core/contents/blocks/link/content.py:26
 msgid "URL"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:162
+#: imio/directory/core/contents/contact/content.py:180
 msgid "URLs"
 msgstr ""
 
 #: imio/directory/policy/configure.zcml:44
 msgid "Uninstalls the imio.directory.policy add-on."
 msgstr ""
 
@@ -2842,14 +2858,18 @@
 msgid "Upgrade policy 1029 to 1030"
 msgstr ""
 
 #: imio/smartweb/policy/upgrades/configure.zcml:140
 msgid "Upgrade policy 1030 to 1031"
 msgstr ""
 
+#: imio/smartweb/policy/upgrades/configure.zcml:148
+msgid "Upgrade policy 1031 to 1032"
+msgstr ""
+
 #: imio/directory/policy/upgrades/configure.zcml:12
 #: imio/events/policy/upgrades/configure.zcml:12
 msgid "Upgrade policy from 1000 to 1001"
 msgstr ""
 
 #: imio/events/policy/upgrades/configure.zcml:20
 #: imio/news/policy/upgrades/configure.zcml:20
@@ -2873,15 +2893,15 @@
 msgid "Upgrade policy from 1026 to 1027"
 msgstr ""
 
 #: imio/smartweb/policy/upgrades/configure.zcml:124
 msgid "Upgrade policy from 1028 to 1029"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:123
+#: imio/directory/core/contents/contact/content.py:141
 msgid "Url"
 msgstr "URL"
 
 #: imio/smartweb/core/browser/controlpanel.py:25
 msgid "Url to get forms from your e-guichet"
 msgstr "Url de récupération des démarches de votre e-guichet"
 
@@ -2907,15 +2927,15 @@
 msgid "Use custom spotlight to avoid bad gallery refresh"
 msgstr ""
 
 #: imio/directory/core/vocabularies.py:86
 msgid "Useful numbers"
 msgstr "Numéros utiles"
 
-#: imio/directory/core/contents/contact/content.py:140
+#: imio/directory/core/contents/contact/content.py:158
 msgid "VAT number"
 msgstr "Numéro d'entreprise / TVA"
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionVideo.xml
 msgid "Video section"
 msgstr "Section vidéo"
 
@@ -2947,15 +2967,15 @@
 msgid "View - News"
 msgstr "Vue - Actualités"
 
 #: imio/smartweb/common/vocabularies.py:109
 msgid "Vignette"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/content.py:34
+#: imio/smartweb/core/contents/sections/contact/content.py:35
 msgid "Visible blocks"
 msgstr "Blocs visibles"
 
 #: imio/smartweb/core/browser/controlpanel.py:116
 msgid "Vocabulary term"
 msgstr "Terme du vocabulaire"
```

### Comparing `imio.smartweb.locales-1.1.8/src/imio/smartweb/locales/locales/de/LC_MESSAGES/plone.po` & `imio.smartweb.locales-1.1.9/src/imio/smartweb/locales/locales/de/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `imio.smartweb.locales-1.1.8/src/imio/smartweb/locales/locales/fr/LC_MESSAGES/imio.smartweb.po` & `imio.smartweb.locales-1.1.9/src/imio/smartweb/locales/locales/fr/LC_MESSAGES/imio.smartweb.po`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
 msgstr ""
 
 #: imio/smartweb/common/behaviors/configure.zcml:13
 msgid "Add topics on content types."
 msgstr "Ajouter une thématique transversale sur le contenu."
 
 #: imio/smartweb/common/interfaces.py:30
-#: imio/smartweb/core/contents/sections/contact/macros.pt:96
+#: imio/smartweb/core/contents/sections/contact/macros.pt:97
 #: imio/smartweb/core/vocabularies.py:175
 msgid "Address"
 msgstr "Adresse"
 
 #: imio/smartweb/common/vocabularies.py:108
 msgid "Affiche"
 msgstr "Affiche"
@@ -227,15 +227,15 @@
 msgid "Allow to select quick access elements for current context."
 msgstr "Permet de sélectionner des éléments Accès Direct pour l'élément courant."
 
 #: imio/smartweb/core/contents/sections/slide/content.py:53
 msgid "Alternatively as a picture"
 msgstr "Comme alternative à une image"
 
-#: imio/smartweb/core/contents/folder/views.py:134
+#: imio/smartweb/core/contents/folder/views.py:135
 msgid "Apply"
 msgstr "Appliquer"
 
 #: imio/smartweb/core/viewlets/toolbar.py:169
 msgid "Ask a question"
 msgstr "Poser une question"
 
@@ -264,15 +264,15 @@
 msgid "Bad URL format '${val}' (good format sample: https://www.imio.be)."
 msgstr "Mauvais format d'URL pour '${val}' (format correct: https://www.imio.be)."
 
 #: imio/directory/core/browser/import.py:90
 msgid "Bad mail format '${val}' (good format sample: noreply@imio.be)."
 msgstr "Mauvais format d'email pour '${val}' (format correct: noreply@imio.be)."
 
-#: imio/directory/core/contents/contact/content.py:47
+#: imio/directory/core/contents/contact/content.py:65
 msgid "Bad phone format"
 msgstr "Mauvais format de téléphone"
 
 #: imio/directory/core/browser/import.py:72
 msgid "Bad phone format '${val}' (good format sample: +32444556677)."
 msgstr "Mauvais format de numéro de téléphone pour '${val}' (format correct: +32444556677)."
 
@@ -300,18 +300,22 @@
 msgid "Block view with images"
 msgstr "Affichage blocs avec images"
 
 #: imio/smartweb/core/profiles/icons/contenttypes/registry.xml
 msgid "BlockLink content type icon"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/content.py:35
+#: imio/smartweb/core/contents/sections/contact/content.py:36
 msgid "Blocks that will be displayed in contact"
 msgstr "Blocs qui vont être affichés dans le contact"
 
+#: imio/directory/core/vocabularies.py:89
+msgid "Bottle bubbles"
+msgstr "Bulles à verres"
+
 #: imio/smartweb/core/vocabularies.py:311
 msgid "Bottom"
 msgstr "Bas"
 
 #: imio/smartweb/core/upgrades/configure.zcml:68
 msgid "By default, Plone open external (Section text / Tiny) links in new tab"
 msgstr ""
@@ -486,15 +490,15 @@
 msgstr "Choisissez d'accepter ou de refuser certains cookies.<br/>Notre <a href=\"${policy_url}\">politique en matière de cookies</a> peut vous aider à faire ce choix."
 
 #: imio/smartweb/core/behaviors/minisite.py:48
 #: imio/smartweb/core/behaviors/subsite.py:40
 msgid "Choose your display mode"
 msgstr "Choisissez votre mode d'affichage"
 
-#: imio/smartweb/core/contents/sections/contact/content.py:56
+#: imio/smartweb/core/contents/sections/contact/content.py:52
 msgid "Choose your gallery layout mode"
 msgstr "Choisissez votre mode d'affichage de galerie"
 
 #: imio/directory/core/contents/entity/content.py:23
 #: imio/events/core/contents/entity/content.py:19
 #: imio/news/core/contents/entity/content.py:19
 msgid "Choose zip codes for this entity"
@@ -601,18 +605,22 @@
 msgid "Click to preview content (without editor actions)."
 msgstr "Prévisualiser le contenu (sans les boutons d'édition)."
 
 #: imio/smartweb/core/viewlets/navigation.py:85
 msgid "Close"
 msgstr "Fermer"
 
-#: imio/smartweb/core/contents/sections/contact/utils.py:239
+#: imio/smartweb/core/contents/sections/contact/utils.py:244
 msgid "Closed"
 msgstr "Fermé"
 
+#: imio/directory/core/vocabularies.py:90
+msgid "Clothing bubbles"
+msgstr "Bulles à vêtements"
+
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionCollection.xml
 msgid "Collection section"
 msgstr "Section collection"
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionCollection.xml
 msgid "Collection section for a page"
 msgstr "Section collection pour une page"
@@ -652,15 +660,15 @@
 msgid "Contact"
 msgstr "Contact"
 
 #: imio/directory/core/profiles/default/types/imio.directory.Contact.xml
 msgid "Contact content type"
 msgstr "Contact"
 
-#: imio/directory/core/contents/contact/content.py:137
+#: imio/directory/core/contents/contact/content.py:155
 #: imio/smartweb/core/vocabularies.py:174
 msgid "Contact informations"
 msgstr "Coordonnées"
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionContact.xml
 msgid "Contact section"
 msgstr "Section contact"
@@ -673,14 +681,18 @@
 msgid "Contact title is missing."
 msgstr "Le titre du contact est manquant."
 
 #: imio/directory/core/browser/import.py:201
 msgid "Contact type is missing."
 msgstr "Le type de contact est manquant."
 
+#: imio/directory/core/vocabularies.py:91
+msgid "Container parks"
+msgstr "Parcs à conteneurs"
+
 #: imio/smartweb/common/browser/privacy/form.py:12
 msgid "Cookies choice"
 msgstr "Choix des cookies"
 
 #: imio/smartweb/common/viewlets/colophon.pt:19
 msgid "Cookies preferences"
 msgstr "Gestion des cookies"
@@ -725,15 +737,15 @@
 msgid "Define number of levels in menu navigation subsite"
 msgstr "Définir un nombre de niveaux pour le menu de navigation du sous-site"
 
 #: imio/smartweb/core/contents/sections/macros.pt:53
 msgid "Delete section"
 msgstr "Supprimer la section"
 
-#: imio/directory/core/contents/contact/content.py:240
+#: imio/directory/core/contents/contact/content.py:258
 #: imio/events/core/contents/event/content.py:56
 #: imio/news/core/contents/newsitem/content.py:42
 msgid "Description"
 msgstr "Description"
 
 #: imio/smartweb/core/browser/controlpanel.py:72
 msgid "Directory SolR Core ID"
@@ -801,29 +813,29 @@
 msgid "Display map"
 msgstr "Afficher la carte"
 
 #: imio/directory/core/vocabularies.py:85
 msgid "Drinking water point"
 msgstr "Points d'eau potable"
 
-#: imio/directory/core/contents/contact/content.py:263
+#: imio/directory/core/contents/contact/content.py:281
 #: imio/events/core/contents/event/content.py:80
 #: imio/news/core/contents/newsitem/content.py:66
 msgid "Dutch translations"
 msgstr "Traductions néerlandophones"
 
 #: imio/smartweb/core/contents/pages/procedure/content.py:21
 msgid "E-Guichet procedure"
 msgstr "Lien vers la démarche dans l'e-guichet iMio"
 
-#: imio/directory/core/contents/contact/content.py:112
+#: imio/directory/core/contents/contact/content.py:130
 msgid "E-mail"
 msgstr "Adresse e-mail"
 
-#: imio/directory/core/contents/contact/content.py:152
+#: imio/directory/core/contents/contact/content.py:170
 msgid "E-mails"
 msgstr "E-mails"
 
 #: imio/smartweb/common/vocabularies.py:22
 msgid "Economics"
 msgstr "Économie"
 
@@ -855,15 +867,15 @@
 msgid "Enable minisite"
 msgstr "Activer le mode site partenaire"
 
 #: imio/smartweb/core/profiles/default/actions.xml
 msgid "Enable subsite"
 msgstr "Activer le mode sous-site"
 
-#: imio/directory/core/contents/contact/content.py:246
+#: imio/directory/core/contents/contact/content.py:264
 #: imio/events/core/contents/event/content.py:63
 #: imio/news/core/contents/newsitem/content.py:49
 msgid "English translations"
 msgstr "Traductions anglophones"
 
 #: imio/smartweb/core/browser/controlpanel.py:17
 msgid "Enter the language code. Ex.: en"
@@ -969,15 +981,15 @@
 msgid "Example : namur.be (SMARTWEB_PLAUSIBLE_SITE varenv has precedence over this.)"
 msgstr "Exemple : namur.be (SMARTWEB_PLAUSIBLE_SITE varenv a la priorité sur cette valeur.)"
 
 #: imio/smartweb/core/browser/controlpanel.py:146
 msgid "Example : plausible.imio.be (SMARTWEB_PLAUSIBLE_URL varenv has precedence over this.)"
 msgstr "Exemple : plausible.imio.be (SMARTWEB_PLAUSIBLE_URL varenv a la priorité sur cette valeur.)"
 
-#: imio/directory/core/contents/contact/content.py:300
+#: imio/directory/core/contents/contact/content.py:318
 msgid "Example : shop, service, association logo"
 msgstr "Exemple : Logo d'un magasin ou d'un service ou d'une association"
 
 #: imio/smartweb/core/behaviors/listing.py:19
 msgid "Exclude from parent listing"
 msgstr "Exclure dans l'affichage listing du parent"
 
@@ -1021,39 +1033,39 @@
 msgid "Facebook url for this event"
 msgstr "Lien facebook pour cet événement"
 
 #: imio/news/core/contents/newsitem/content.py:101
 msgid "Facebook url for this news"
 msgstr "Lien facebook pour cette actualité"
 
-#: imio/smartweb/core/browser/faceted/configure.zcml:67
+#: imio/smartweb/core/browser/faceted/configure.zcml:81
 msgid "Faceted block view"
 msgstr "Affichage blocs"
 
-#: imio/smartweb/core/browser/faceted/configure.zcml:74
+#: imio/smartweb/core/browser/faceted/configure.zcml:88
 msgid "Faceted block view with images"
 msgstr "Affichage blocs avec images"
 
 #: imio/smartweb/core/browser/faceted/configure.zcml:16
 msgid "Faceted items preview"
 msgstr ""
 
-#: imio/smartweb/core/browser/faceted/configure.zcml:97
+#: imio/smartweb/core/browser/faceted/configure.zcml:111
 msgid "Faceted map"
 msgstr "Affichage plan"
 
-#: imio/smartweb/core/browser/faceted/configure.zcml:81
+#: imio/smartweb/core/browser/faceted/configure.zcml:95
 msgid "Faceted summary view"
 msgstr "Affichage liste"
 
-#: imio/smartweb/core/browser/faceted/configure.zcml:88
+#: imio/smartweb/core/browser/faceted/configure.zcml:102
 msgid "Faceted summary view with images"
 msgstr "Affichage liste avec images"
 
-#: imio/directory/core/contents/contact/content.py:317
+#: imio/directory/core/contents/contact/content.py:335
 msgid "Facilities"
 msgstr "Facilités"
 
 #: imio/events/core/contents/event/content.py:154
 #: imio/events/core/contents/event/view.pt:57
 msgid "Facilities for person with reduced mobility"
 msgstr "Accessible aux personnes à mobilité réduite"
@@ -1134,15 +1146,15 @@
 msgid "Footer has been successfully added"
 msgstr "Le pied de page a été ajouté avec succès"
 
 #: imio/smartweb/core/contents/folder/content.py:26
 msgid "For the anonymous visitor, the folder and the selected item are one. When he clicks on the folder, the item is displayed."
 msgstr "Pour le visiteur anonyme, le dossier et l'élément sélectionné ne font qu'un. Lorsqu'il clique sur le dossier, l'élément s'affiche."
 
-#: imio/smartweb/core/contents/folder/views.py:105
+#: imio/smartweb/core/contents/folder/views.py:106
 msgid "Form to choose item to be displayed as the home page of the folder"
 msgstr "Formulaire de choix de l'élément à afficher comme page d'accueil du dossier"
 
 #: imio/directory/core/vocabularies.py:88
 msgid "Free WIFI"
 msgstr "Wifi gratuit"
 
@@ -1163,27 +1175,27 @@
 msgid "Full width"
 msgstr "Pleine page"
 
 #: imio/smartweb/core/vocabularies.py:180
 msgid "Gallery"
 msgstr "Galerie"
 
-#: imio/smartweb/core/contents/sections/contact/content.py:55
+#: imio/smartweb/core/contents/sections/contact/content.py:51
 msgid "Gallery mode"
 msgstr "Mode de galerie"
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionGallery.xml
 msgid "Gallery section"
 msgstr "Section galerie"
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionGallery.xml
 msgid "Gallery section for a page"
 msgstr "Création d'une section galerie qui affichera ses images dans votre page. "
 
-#: imio/directory/core/contents/contact/content.py:229
+#: imio/directory/core/contents/contact/content.py:247
 #: imio/events/core/contents/event/content.py:46
 #: imio/news/core/contents/newsitem/content.py:32
 msgid "German translations"
 msgstr "Traductions germanophones"
 
 #: imio/smartweb/core/contents/sections/events/content.py:37
 msgid "Get priory on related agenda for these specifics events."
@@ -1321,15 +1333,15 @@
 msgid "Image orientation"
 msgstr "Orientation de l'image"
 
 #: imio/smartweb/core/contents/sections/gallery/content.py:16
 msgid "Image scale for images"
 msgstr "Echelle d'images"
 
-#: imio/smartweb/core/contents/sections/contact/content.py:77
+#: imio/smartweb/core/contents/sections/contact/content.py:73
 msgid "Image scale for images (only for gallery mode)"
 msgstr "Echelle d'images (seulement en mode galerie)"
 
 #: imio/smartweb/core/contents/sections/text/content.py:24
 msgid "Image size"
 msgstr "Taille de l'image"
 
@@ -1352,15 +1364,15 @@
 msgstr "Important! Ces catégories sont utilisées pour créer des listes accessibles via le menu navigation"
 
 #: imio/events/core/contents/event/content.py:178
 #: imio/news/core/contents/newsitem/content.py:133
 msgid "Important! These categories are used to supplement the information provided by the topics"
 msgstr "Important! Ces catégories permettent de compléter l'information apportée par les thématiques"
 
-#: imio/directory/core/contents/contact/content.py:318
+#: imio/directory/core/contents/contact/content.py:336
 msgid "Important! These categories make it possible to highlight and geolocate certain basic services"
 msgstr "Important! Ces catégories permettent de mettre en avant et de géolocaliser certains services de base"
 
 #: imio/smartweb/common/behaviors/topics.py:17
 msgid "Important! Topics are used to filter search results and create lists"
 msgstr "Important! Les thématiques sont utilisées pour filtrer les résultats de la recherche et créer des listes"
 
@@ -1390,28 +1402,28 @@
 msgid "Installs the imio.events.policy add-on."
 msgstr ""
 
 #: imio/news/policy/configure.zcml:36
 msgid "Installs the imio.news.policy add-on."
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:210
+#: imio/directory/core/contents/contact/content.py:228
 msgid "Internal note"
 msgstr "Note interne"
 
 #: imio/events/core/vocabularies.py:25
 msgid "Internships and courses"
 msgstr "Stages et cours"
 
 #: imio/smartweb/core/contents/folder/content.py:25
 msgid "Item(s) that can be selected as the folder default page."
 msgstr "Elément(s) pouvant être sélectionné(s) comme page d'accueil du dossier."
 
 #: imio/events/core/contents/event/views.py:77
-#: imio/smartweb/core/contents/sections/contact/macros.pt:111
+#: imio/smartweb/core/contents/sections/contact/macros.pt:112
 #: imio/smartweb/core/contents/sections/contact/utils.py:56
 msgid "Itinerary"
 msgstr "Itinéraire"
 
 #: imio/news/core/vocabularies.py:17
 msgid "Job offer"
 msgstr "Emploi"
@@ -1425,19 +1437,19 @@
 msgstr "Journaliste"
 
 #: imio/events/core/contents/event/view.pt:107
 #: imio/news/core/contents/newsitem/view.pt:64
 msgid "Keywords"
 msgstr "Mots-clés"
 
-#: imio/directory/core/contents/contact/content.py:100
+#: imio/directory/core/contents/contact/content.py:118
 msgid "Label (Secretariat, Manager office, Sales,...)"
 msgstr "Intitulé (Secrétariat, Bureau de la direction, Ventes, ...)"
 
-#: imio/directory/core/contents/contact/content.py:79
+#: imio/directory/core/contents/contact/content.py:97
 msgid "Label (direction, Main number,...)"
 msgstr "Intitulé (direction, numéro principal, ...)"
 
 #: imio/smartweb/core/browser/controlpanel.py:16
 msgid "Language (en, fr,...)"
 msgstr "Langue (en, fr, ...)"
 
@@ -1519,30 +1531,30 @@
 msgid "List of news categories values available for this entity (one per line)"
 msgstr "Liste de catégories spécifiques d'actualités disponibes pour cette entité (une par ligne)"
 
 #: imio/smartweb/common/vocabularies.py:110
 msgid "Liste"
 msgstr "Liste"
 
-#: imio/directory/core/contents/contact/content.py:299
+#: imio/directory/core/contents/contact/content.py:317
 #: imio/smartweb/core/behaviors/minisite.py:41
 #: imio/smartweb/core/behaviors/subsite.py:33
 msgid "Logo"
 msgstr "Logo"
 
 #: imio/smartweb/core/vocabularies.py:159
 msgid "Logo and title"
 msgstr "Logo et titre"
 
 #: imio/smartweb/core/behaviors/minisite.py:47
 #: imio/smartweb/core/behaviors/subsite.py:39
 msgid "Logo display"
 msgstr "Type d'affichage du logo"
 
-#: imio/smartweb/core/contents/sections/contact/utils.py:269
+#: imio/smartweb/core/contents/sections/contact/utils.py:274
 msgid "Lunch time"
 msgstr "Heure du midi"
 
 #: imio/smartweb/core/contents/sections/macros.pt:42
 msgid "Manage section contents"
 msgstr "Modifier contenu"
 
@@ -1564,19 +1576,19 @@
 
 #: imio/smartweb/core/contents/sections/collection/content.py:48
 #: imio/smartweb/core/contents/sections/events/content.py:70
 #: imio/smartweb/core/contents/sections/news/content.py:70
 msgid "Maximum number of batches to display"
 msgstr "Nombre maximum de lots à afficher"
 
-#: imio/smartweb/core/contents/sections/contact/content.py:69
+#: imio/smartweb/core/contents/sections/contact/content.py:65
 msgid "Maximum number of contacts by line"
 msgstr "Nombre maximum de contacts par ligne"
 
-#: imio/smartweb/core/contents/sections/contact/content.py:70
+#: imio/smartweb/core/contents/sections/contact/content.py:66
 msgid "Maximum number of contacts by line (on PC)"
 msgstr "Nombre maximum de contacts par ligne (sur un écran d'ordinateur)"
 
 #: imio/smartweb/core/behaviors/subsite.py:48
 msgid "Menu depth"
 msgstr "Profondeur du menu"
 
@@ -1697,25 +1709,25 @@
 msgid "Not allowed to add Files or Images in imio.directory.Entity"
 msgstr ""
 
 #: imio/smartweb/common/interfaces.py:34
 msgid "Number"
 msgstr "Numéro"
 
-#: imio/directory/core/contents/contact/content.py:92
+#: imio/directory/core/contents/contact/content.py:110
 msgid "Number (format: +32475010203)"
 msgstr "Numéro (format: +32475010203)"
 
 #: imio/smartweb/core/contents/sections/collection/content.py:41
 #: imio/smartweb/core/contents/sections/events/content.py:63
 #: imio/smartweb/core/contents/sections/files/content.py:15
 msgid "Number of items per batch"
 msgstr "Nombre d'éléments par lot"
 
-#: imio/smartweb/core/contents/sections/contact/content.py:62
+#: imio/smartweb/core/contents/sections/contact/content.py:58
 msgid "Number of items per batch (only for carousel mode)"
 msgstr "Nombre d'éléments par lot (seulement en mode carrousel)"
 
 #: imio/smartweb/core/contents/rest/directory/content.py:25
 #: imio/smartweb/core/contents/rest/events/content.py:30
 #: imio/smartweb/core/contents/rest/news/content.py:21
 msgid "Number of items to display"
@@ -1737,19 +1749,19 @@
 msgid "Only one procedure field can be filled !"
 msgstr "Un seul champ \"démarche\" peut être rempli !"
 
 #: imio/smartweb/core/contents/blocks/link/content.py:34
 msgid "Only used in table view (takes precedence over image)"
 msgstr "Utilisée uniquement dans l'affichage tableau (prend la priorité sur l'image)"
 
-#: imio/smartweb/core/contents/sections/contact/utils.py:246
+#: imio/smartweb/core/contents/sections/contact/utils.py:251
 msgid "Open"
 msgstr "Ouvert"
 
-#: imio/smartweb/core/contents/sections/contact/utils.py:263
+#: imio/smartweb/core/contents/sections/contact/utils.py:268
 msgid "Open at "
 msgstr "Ouvre à "
 
 #: imio/smartweb/core/contents/blocks/link/content.py:23
 #: imio/smartweb/core/contents/sections/slide/content.py:66
 msgid "Open in a new tab"
 msgstr "Ouvrir dans un nouvel onglet"
@@ -1818,30 +1830,34 @@
 msgid "Party and folklore"
 msgstr "Fête et folklore"
 
 #: imio/smartweb/common/upgrades/configure.zcml:69
 msgid "Patch (Remove select2) eea.facetednavigation jquery"
 msgstr ""
 
-#: imio/smartweb/core/vocabularies.py:142
+#: imio/smartweb/core/vocabularies.py:141
 msgid "Paysage"
 msgstr "Paysage"
 
 #: imio/directory/core/vocabularies.py:53
 msgid "Personal email"
 msgstr "Adresse e-mail personnelle"
 
 #: imio/directory/core/vocabularies.py:39
 msgid "Personal phone"
 msgstr "Numéro de téléphone personnel"
 
-#: imio/directory/core/contents/contact/content.py:142
+#: imio/directory/core/contents/contact/content.py:160
 msgid "Phones"
 msgstr "Téléphones"
 
+#: imio/smartweb/core/browser/faceted/configure.zcml:37
+msgid "Photo gallery"
+msgstr ""
+
 #: imio/smartweb/core/contents/sections/slide/content.py:41
 msgid "Picture will be displayed as slide background"
 msgstr "L'image est affichée en background du slide"
 
 #: imio/directory/core/vocabularies.py:68
 msgid "Pinterest"
 msgstr ""
@@ -1898,15 +1914,15 @@
 msgid "Portal Page content type to print informations"
 msgstr "Page Portail pour afficher de l'information"
 
 #: imio/smartweb/core/profiles/icons/contenttypes/registry.xml
 msgid "PortalPage content type icon"
 msgstr ""
 
-#: imio/smartweb/core/vocabularies.py:141
+#: imio/smartweb/core/vocabularies.py:142
 msgid "Portrait"
 msgstr "Portrait"
 
 #: imio/directory/core/vocabularies.py:20
 msgid "Position (mayor, alderman, advisor, director, head of department, etc.)"
 msgstr "Fonction (bourgmestre, échevin, conseiller, directeur, chef de service, etc.)"
 
@@ -1932,15 +1948,15 @@
 msgid "Presse"
 msgstr "Presse"
 
 #: imio/smartweb/core/profiles/default/actions.xml
 msgid "Preview"
 msgstr "Prévisualiser"
 
-#: imio/directory/core/contents/contact/content.py:175
+#: imio/directory/core/contents/contact/content.py:193
 msgid "Private contact informations"
 msgstr "Coordonnées privées"
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.Procedure.xml
 msgid "Procedure"
 msgstr "Démarche"
 
@@ -2001,15 +2017,15 @@
 msgid "Refuse all"
 msgstr "Tout refuser"
 
 #: imio/smartweb/core/contents/sections/events/content.py:30
 msgid "Related agenda"
 msgstr "Agenda lié"
 
-#: imio/smartweb/core/contents/sections/contact/content.py:23
+#: imio/smartweb/core/contents/sections/contact/content.py:24
 msgid "Related contacts"
 msgstr "Contacts liés"
 
 #: imio/smartweb/core/contents/sections/news/content.py:30
 msgid "Related news folder"
 msgstr "Dossier d'actualités lié"
 
@@ -2030,14 +2046,18 @@
 msgid "Remove plone.patternslib deprecated bundles"
 msgstr ""
 
 #: imio/news/policy/upgrades/configure.zcml:12
 msgid "Remove ugly IImioEventsPolicyLayer"
 msgstr ""
 
+#: imio/smartweb/policy/upgrades/configure.zcml:148
+msgid "Restore removed behaviors on Collection type"
+msgstr ""
+
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionText.xml
 msgid "Rich text section for a page"
 msgstr "Création d'une section de texte dans votre page."
 
 #: imio/smartweb/core/vocabularies.py:310
 msgid "Right"
 msgstr "Droite"
@@ -2050,15 +2070,15 @@
 msgid "Saturday"
 msgstr "Samedi"
 
 #: imio/smartweb/common/browser/privacy/form.py:27
 msgid "Save my choices"
 msgstr "Enregistrer mes choix"
 
-#: imio/smartweb/core/contents/sections/contact/macros.pt:121
+#: imio/smartweb/core/contents/sections/contact/macros.pt:122
 #: imio/smartweb/core/vocabularies.py:177
 msgid "Schedule"
 msgstr "Horaires"
 
 #: imio/smartweb/core/viewlets/searchbox.pt:9
 msgid "Search"
 msgstr "Rechercher"
@@ -2167,19 +2187,19 @@
 msgid "Select agenda to display"
 msgstr "Sélectionnez l'agenda à afficher"
 
 #: imio/events/core/contents/event/content.py:168
 msgid "Select agendas where this event will be displayed. Current agenda is always selected."
 msgstr "Sélectionnez les agendas dans lesquels cet événement sera affiché. L'agenda courant sera toujours sélectionné."
 
-#: imio/smartweb/core/contents/sections/contact/content.py:24
+#: imio/smartweb/core/contents/sections/contact/content.py:25
 msgid "Select contacts. If you can't find contacts you want, make sure it exists in the directory and that its \"state\" is published."
 msgstr "Sélectionnez les contacts. Si vous ne trouvez pas les contacts que vous souhaitez, assurez-vous qu'ils existent dans l'annuaire et qu'ils sont bien publié!"
 
-#: imio/directory/core/contents/contact/content.py:308
+#: imio/directory/core/contents/contact/content.py:326
 msgid "Select entities where this contact will be displayed. Current entity will always be selected."
 msgstr "Sélectionnez les entités dans lesquelles ce contact sera affiché. L'entité courante sera toujours sélectionnée."
 
 #: imio/smartweb/core/contents/sections/text/content.py:25
 msgid "Select image size"
 msgstr "Sélectionnez la taille de l'image"
 
@@ -2211,15 +2231,15 @@
 msgid "Selected agenda"
 msgstr "Agenda sélectionné"
 
 #: imio/events/core/contents/event/content.py:167
 msgid "Selected agendas"
 msgstr "Agendas concernés"
 
-#: imio/directory/core/contents/contact/content.py:307
+#: imio/directory/core/contents/contact/content.py:325
 msgid "Selected entities"
 msgstr "Entités concernées"
 
 #: imio/smartweb/core/contents/rest/events/content.py:17
 msgid "Selected event types"
 msgstr "Types d'événements sélectionnés"
 
@@ -2392,15 +2412,15 @@
 msgid "Subsite has been disabled"
 msgstr "Le mode sous-site a été désactivé"
 
 #: imio/smartweb/core/browser/subsite/settings.py:25
 msgid "Subsite has been successfully activated"
 msgstr "Le mode sous-site a été activé avec succès"
 
-#: imio/directory/core/contents/contact/content.py:239
+#: imio/directory/core/contents/contact/content.py:257
 #: imio/smartweb/core/contents/sections/postit/content.py:26
 msgid "Subtitle"
 msgstr "Sous-titre"
 
 #: imio/smartweb/core/contents/folder/configure.zcml:72
 msgid "Summary view"
 msgstr "Affichage liste"
@@ -2409,18 +2429,14 @@
 msgid "Summary view with images"
 msgstr "Affichage liste avec images"
 
 #: imio/smartweb/core/contents/sections/contact/utils.py:106
 msgid "Sunday"
 msgstr "Dimanche"
 
-#: imio/smartweb/core/contents/sections/contact/content.py:51
-msgid "Switch lead image to portrait mode"
-msgstr "Passer l'image de garde en mode portrait"
-
 #: imio/smartweb/core/contents/sections/links/configure.zcml:15
 #: imio/smartweb/core/contents/sections/selections/configure.zcml:15
 msgid "Table view"
 msgstr "Affichage tableau"
 
 #: imio/smartweb/core/viewlets/toolbar.py:183
 msgid "Take part of workshop"
@@ -2500,15 +2516,15 @@
 msgid "Third page"
 msgstr "Tiers de la page"
 
 #: imio/smartweb/common/privacy.py:70
 msgid "This feature requires cookies acceptation.<br/><a class=\"pat-plone-modal\" href=\"${consent_url}\">Review your cookies preferences</a>."
 msgstr "Cette fonctionnalité nécessite l'acceptation des cookies.<br/><a class=\"pat-plone-modal\" href=\"${consent_url}\">Modifier vos préférences en matière de cookies</a>."
 
-#: imio/directory/core/contents/contact/content.py:234
+#: imio/directory/core/contents/contact/content.py:252
 #: imio/events/core/contents/event/content.py:51
 #: imio/news/core/contents/newsitem/content.py:37
 msgid "This field is required if the content must be available in this language"
 msgstr "Ce champ est requis si le contenu doit être disponible dans cette langue"
 
 #: imio/smartweb/core/browser/controlpanel.py:91
 msgid "This information is used for search results redirection"
@@ -2531,15 +2547,15 @@
 msgid "Ticket url"
 msgstr "Billeterie"
 
 #: imio/events/core/contents/event/content.py:118
 msgid "Ticket url to subscribe to this event"
 msgstr "Lien de la billeterie pour s'inscrire à cet événement"
 
-#: imio/directory/core/contents/contact/content.py:233
+#: imio/directory/core/contents/contact/content.py:251
 #: imio/events/core/contents/event/content.py:50
 #: imio/news/core/contents/newsitem/content.py:36
 msgid "Title"
 msgstr "Titre"
 
 #: imio/smartweb/core/vocabularies.py:173
 msgid "Title and Subtitle"
@@ -2593,23 +2609,23 @@
 msgid "Twitter url for this news"
 msgstr "Lien Twitter pour cette actualité"
 
 #: imio/smartweb/core/vocabularies.py:127
 msgid "Two third of width"
 msgstr "Deux tiers de la page"
 
-#: imio/directory/core/contents/contact/content.py:85
+#: imio/directory/core/contents/contact/content.py:103
 msgid "Type"
 msgstr ""
 
 #: imio/smartweb/core/contents/blocks/link/content.py:26
 msgid "URL"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:162
+#: imio/directory/core/contents/contact/content.py:180
 msgid "URLs"
 msgstr ""
 
 #: imio/directory/policy/configure.zcml:44
 msgid "Uninstalls the imio.directory.policy add-on."
 msgstr ""
 
@@ -2842,14 +2858,18 @@
 msgid "Upgrade policy 1029 to 1030"
 msgstr ""
 
 #: imio/smartweb/policy/upgrades/configure.zcml:140
 msgid "Upgrade policy 1030 to 1031"
 msgstr ""
 
+#: imio/smartweb/policy/upgrades/configure.zcml:148
+msgid "Upgrade policy 1031 to 1032"
+msgstr ""
+
 #: imio/directory/policy/upgrades/configure.zcml:12
 #: imio/events/policy/upgrades/configure.zcml:12
 msgid "Upgrade policy from 1000 to 1001"
 msgstr ""
 
 #: imio/events/policy/upgrades/configure.zcml:20
 #: imio/news/policy/upgrades/configure.zcml:20
@@ -2873,15 +2893,15 @@
 msgid "Upgrade policy from 1026 to 1027"
 msgstr ""
 
 #: imio/smartweb/policy/upgrades/configure.zcml:124
 msgid "Upgrade policy from 1028 to 1029"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:123
+#: imio/directory/core/contents/contact/content.py:141
 msgid "Url"
 msgstr "URL"
 
 #: imio/smartweb/core/browser/controlpanel.py:25
 msgid "Url to get forms from your e-guichet"
 msgstr "Url de récupération des démarches de votre e-guichet"
 
@@ -2907,15 +2927,15 @@
 msgid "Use custom spotlight to avoid bad gallery refresh"
 msgstr ""
 
 #: imio/directory/core/vocabularies.py:86
 msgid "Useful numbers"
 msgstr "Numéros utiles"
 
-#: imio/directory/core/contents/contact/content.py:140
+#: imio/directory/core/contents/contact/content.py:158
 msgid "VAT number"
 msgstr "Numéro d'entreprise / TVA"
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionVideo.xml
 msgid "Video section"
 msgstr "Section vidéo"
 
@@ -2947,15 +2967,15 @@
 msgid "View - News"
 msgstr "Vue - Actualités"
 
 #: imio/smartweb/common/vocabularies.py:109
 msgid "Vignette"
 msgstr "Vignette"
 
-#: imio/smartweb/core/contents/sections/contact/content.py:34
+#: imio/smartweb/core/contents/sections/contact/content.py:35
 msgid "Visible blocks"
 msgstr "Blocs visibles"
 
 #: imio/smartweb/core/browser/controlpanel.py:116
 msgid "Vocabulary term"
 msgstr "Terme du vocabulaire"
```

### Comparing `imio.smartweb.locales-1.1.8/src/imio/smartweb/locales/locales/fr/LC_MESSAGES/plone.po` & `imio.smartweb.locales-1.1.9/src/imio/smartweb/locales/locales/fr/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `imio.smartweb.locales-1.1.8/src/imio/smartweb/locales/locales/imio.smartweb.pot` & `imio.smartweb.locales-1.1.9/src/imio/smartweb/locales/locales/imio.smartweb.pot`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #--- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 #SOME DESCRIPTIVE TITLE.
 #FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2023-10-25 15:55+0000\n"
+"POT-Creation-Date: 2023-11-20 08:01+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "Language-Code: en\n"
 "Language-Name: English\n"
 "Preferred-Encodings: utf-8 latin1\n"
 "Domain: imio.smartweb\n"
 
-#: imio/directory/core/contents/contact/content.py:80
+#: imio/directory/core/contents/contact/content.py:98
 msgid ""
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/base.py:85
 msgid "<div class=\"section_error_txt\">Error in section : \"{}\" <a href=\"{}/edit\">[edit]</a></div>"
 msgstr ""
 
@@ -187,15 +187,15 @@
 msgstr ""
 
 #: imio/smartweb/common/behaviors/configure.zcml:13
 msgid "Add topics on content types."
 msgstr ""
 
 #: imio/smartweb/common/interfaces.py:30
-#: imio/smartweb/core/contents/sections/contact/macros.pt:96
+#: imio/smartweb/core/contents/sections/contact/macros.pt:97
 #: imio/smartweb/core/vocabularies.py:175
 msgid "Address"
 msgstr ""
 
 #: imio/smartweb/common/vocabularies.py:108
 msgid "Affiche"
 msgstr ""
@@ -232,15 +232,15 @@
 msgid "Allow to select quick access elements for current context."
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/slide/content.py:53
 msgid "Alternatively as a picture"
 msgstr ""
 
-#: imio/smartweb/core/contents/folder/views.py:134
+#: imio/smartweb/core/contents/folder/views.py:135
 msgid "Apply"
 msgstr ""
 
 #: imio/smartweb/core/viewlets/toolbar.py:169
 msgid "Ask a question"
 msgstr ""
 
@@ -269,15 +269,15 @@
 msgid "Bad URL format '${val}' (good format sample: https://www.imio.be)."
 msgstr ""
 
 #: imio/directory/core/browser/import.py:90
 msgid "Bad mail format '${val}' (good format sample: noreply@imio.be)."
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:47
+#: imio/directory/core/contents/contact/content.py:65
 msgid "Bad phone format"
 msgstr ""
 
 #: imio/directory/core/browser/import.py:72
 msgid "Bad phone format '${val}' (good format sample: +32444556677)."
 msgstr ""
 
@@ -305,18 +305,22 @@
 msgid "Block view with images"
 msgstr ""
 
 #: imio/smartweb/core/profiles/icons/contenttypes/registry.xml
 msgid "BlockLink content type icon"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/content.py:35
+#: imio/smartweb/core/contents/sections/contact/content.py:36
 msgid "Blocks that will be displayed in contact"
 msgstr ""
 
+#: imio/directory/core/vocabularies.py:89
+msgid "Bottle bubbles"
+msgstr ""
+
 #: imio/smartweb/core/vocabularies.py:311
 msgid "Bottom"
 msgstr ""
 
 #: imio/smartweb/core/upgrades/configure.zcml:68
 msgid "By default, Plone open external (Section text / Tiny) links in new tab"
 msgstr ""
@@ -491,15 +495,15 @@
 msgstr ""
 
 #: imio/smartweb/core/behaviors/minisite.py:48
 #: imio/smartweb/core/behaviors/subsite.py:40
 msgid "Choose your display mode"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/content.py:56
+#: imio/smartweb/core/contents/sections/contact/content.py:52
 msgid "Choose your gallery layout mode"
 msgstr ""
 
 #: imio/directory/core/contents/entity/content.py:23
 #: imio/events/core/contents/entity/content.py:19
 #: imio/news/core/contents/entity/content.py:19
 msgid "Choose zip codes for this entity"
@@ -606,18 +610,22 @@
 msgid "Click to preview content (without editor actions)."
 msgstr ""
 
 #: imio/smartweb/core/viewlets/navigation.py:85
 msgid "Close"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/utils.py:239
+#: imio/smartweb/core/contents/sections/contact/utils.py:244
 msgid "Closed"
 msgstr ""
 
+#: imio/directory/core/vocabularies.py:90
+msgid "Clothing bubbles"
+msgstr ""
+
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionCollection.xml
 msgid "Collection section"
 msgstr ""
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionCollection.xml
 msgid "Collection section for a page"
 msgstr ""
@@ -657,15 +665,15 @@
 msgid "Contact"
 msgstr ""
 
 #: imio/directory/core/profiles/default/types/imio.directory.Contact.xml
 msgid "Contact content type"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:137
+#: imio/directory/core/contents/contact/content.py:155
 #: imio/smartweb/core/vocabularies.py:174
 msgid "Contact informations"
 msgstr ""
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionContact.xml
 msgid "Contact section"
 msgstr ""
@@ -678,14 +686,18 @@
 msgid "Contact title is missing."
 msgstr ""
 
 #: imio/directory/core/browser/import.py:201
 msgid "Contact type is missing."
 msgstr ""
 
+#: imio/directory/core/vocabularies.py:91
+msgid "Container parks"
+msgstr ""
+
 #: imio/smartweb/common/browser/privacy/form.py:12
 msgid "Cookies choice"
 msgstr ""
 
 #: imio/smartweb/common/viewlets/colophon.pt:19
 msgid "Cookies preferences"
 msgstr ""
@@ -730,15 +742,15 @@
 msgid "Define number of levels in menu navigation subsite"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/macros.pt:53
 msgid "Delete section"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:240
+#: imio/directory/core/contents/contact/content.py:258
 #: imio/events/core/contents/event/content.py:56
 #: imio/news/core/contents/newsitem/content.py:42
 msgid "Description"
 msgstr ""
 
 #: imio/smartweb/core/browser/controlpanel.py:72
 msgid "Directory SolR Core ID"
@@ -806,29 +818,29 @@
 msgid "Display map"
 msgstr ""
 
 #: imio/directory/core/vocabularies.py:85
 msgid "Drinking water point"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:263
+#: imio/directory/core/contents/contact/content.py:281
 #: imio/events/core/contents/event/content.py:80
 #: imio/news/core/contents/newsitem/content.py:66
 msgid "Dutch translations"
 msgstr ""
 
 #: imio/smartweb/core/contents/pages/procedure/content.py:21
 msgid "E-Guichet procedure"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:112
+#: imio/directory/core/contents/contact/content.py:130
 msgid "E-mail"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:152
+#: imio/directory/core/contents/contact/content.py:170
 msgid "E-mails"
 msgstr ""
 
 #: imio/smartweb/common/vocabularies.py:22
 msgid "Economics"
 msgstr ""
 
@@ -860,15 +872,15 @@
 msgid "Enable minisite"
 msgstr ""
 
 #: imio/smartweb/core/profiles/default/actions.xml
 msgid "Enable subsite"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:246
+#: imio/directory/core/contents/contact/content.py:264
 #: imio/events/core/contents/event/content.py:63
 #: imio/news/core/contents/newsitem/content.py:49
 msgid "English translations"
 msgstr ""
 
 #: imio/smartweb/core/browser/controlpanel.py:17
 msgid "Enter the language code. Ex.: en"
@@ -974,15 +986,15 @@
 msgid "Example : namur.be (SMARTWEB_PLAUSIBLE_SITE varenv has precedence over this.)"
 msgstr ""
 
 #: imio/smartweb/core/browser/controlpanel.py:146
 msgid "Example : plausible.imio.be (SMARTWEB_PLAUSIBLE_URL varenv has precedence over this.)"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:300
+#: imio/directory/core/contents/contact/content.py:318
 msgid "Example : shop, service, association logo"
 msgstr ""
 
 #: imio/smartweb/core/behaviors/listing.py:19
 msgid "Exclude from parent listing"
 msgstr ""
 
@@ -1026,39 +1038,39 @@
 msgid "Facebook url for this event"
 msgstr ""
 
 #: imio/news/core/contents/newsitem/content.py:101
 msgid "Facebook url for this news"
 msgstr ""
 
-#: imio/smartweb/core/browser/faceted/configure.zcml:67
+#: imio/smartweb/core/browser/faceted/configure.zcml:81
 msgid "Faceted block view"
 msgstr ""
 
-#: imio/smartweb/core/browser/faceted/configure.zcml:74
+#: imio/smartweb/core/browser/faceted/configure.zcml:88
 msgid "Faceted block view with images"
 msgstr ""
 
 #: imio/smartweb/core/browser/faceted/configure.zcml:16
 msgid "Faceted items preview"
 msgstr ""
 
-#: imio/smartweb/core/browser/faceted/configure.zcml:97
+#: imio/smartweb/core/browser/faceted/configure.zcml:111
 msgid "Faceted map"
 msgstr ""
 
-#: imio/smartweb/core/browser/faceted/configure.zcml:81
+#: imio/smartweb/core/browser/faceted/configure.zcml:95
 msgid "Faceted summary view"
 msgstr ""
 
-#: imio/smartweb/core/browser/faceted/configure.zcml:88
+#: imio/smartweb/core/browser/faceted/configure.zcml:102
 msgid "Faceted summary view with images"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:317
+#: imio/directory/core/contents/contact/content.py:335
 msgid "Facilities"
 msgstr ""
 
 #: imio/events/core/contents/event/content.py:154
 #: imio/events/core/contents/event/view.pt:57
 msgid "Facilities for person with reduced mobility"
 msgstr ""
@@ -1139,15 +1151,15 @@
 msgid "Footer has been successfully added"
 msgstr ""
 
 #: imio/smartweb/core/contents/folder/content.py:26
 msgid "For the anonymous visitor, the folder and the selected item are one. When he clicks on the folder, the item is displayed."
 msgstr ""
 
-#: imio/smartweb/core/contents/folder/views.py:105
+#: imio/smartweb/core/contents/folder/views.py:106
 msgid "Form to choose item to be displayed as the home page of the folder"
 msgstr ""
 
 #: imio/directory/core/vocabularies.py:88
 msgid "Free WIFI"
 msgstr ""
 
@@ -1168,27 +1180,27 @@
 msgid "Full width"
 msgstr ""
 
 #: imio/smartweb/core/vocabularies.py:180
 msgid "Gallery"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/content.py:55
+#: imio/smartweb/core/contents/sections/contact/content.py:51
 msgid "Gallery mode"
 msgstr ""
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionGallery.xml
 msgid "Gallery section"
 msgstr ""
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionGallery.xml
 msgid "Gallery section for a page"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:229
+#: imio/directory/core/contents/contact/content.py:247
 #: imio/events/core/contents/event/content.py:46
 #: imio/news/core/contents/newsitem/content.py:32
 msgid "German translations"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/events/content.py:37
 msgid "Get priory on related agenda for these specifics events."
@@ -1326,15 +1338,15 @@
 msgid "Image orientation"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/gallery/content.py:16
 msgid "Image scale for images"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/content.py:77
+#: imio/smartweb/core/contents/sections/contact/content.py:73
 msgid "Image scale for images (only for gallery mode)"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/text/content.py:24
 msgid "Image size"
 msgstr ""
 
@@ -1357,15 +1369,15 @@
 msgstr ""
 
 #: imio/events/core/contents/event/content.py:178
 #: imio/news/core/contents/newsitem/content.py:133
 msgid "Important! These categories are used to supplement the information provided by the topics"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:318
+#: imio/directory/core/contents/contact/content.py:336
 msgid "Important! These categories make it possible to highlight and geolocate certain basic services"
 msgstr ""
 
 #: imio/smartweb/common/behaviors/topics.py:17
 msgid "Important! Topics are used to filter search results and create lists"
 msgstr ""
 
@@ -1395,28 +1407,28 @@
 msgid "Installs the imio.events.policy add-on."
 msgstr ""
 
 #: imio/news/policy/configure.zcml:36
 msgid "Installs the imio.news.policy add-on."
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:210
+#: imio/directory/core/contents/contact/content.py:228
 msgid "Internal note"
 msgstr ""
 
 #: imio/events/core/vocabularies.py:25
 msgid "Internships and courses"
 msgstr ""
 
 #: imio/smartweb/core/contents/folder/content.py:25
 msgid "Item(s) that can be selected as the folder default page."
 msgstr ""
 
 #: imio/events/core/contents/event/views.py:77
-#: imio/smartweb/core/contents/sections/contact/macros.pt:111
+#: imio/smartweb/core/contents/sections/contact/macros.pt:112
 #: imio/smartweb/core/contents/sections/contact/utils.py:56
 msgid "Itinerary"
 msgstr ""
 
 #: imio/news/core/vocabularies.py:17
 msgid "Job offer"
 msgstr ""
@@ -1430,19 +1442,19 @@
 msgstr ""
 
 #: imio/events/core/contents/event/view.pt:107
 #: imio/news/core/contents/newsitem/view.pt:64
 msgid "Keywords"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:100
+#: imio/directory/core/contents/contact/content.py:118
 msgid "Label (Secretariat, Manager office, Sales,...)"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:79
+#: imio/directory/core/contents/contact/content.py:97
 msgid "Label (direction, Main number,...)"
 msgstr ""
 
 #: imio/smartweb/core/browser/controlpanel.py:16
 msgid "Language (en, fr,...)"
 msgstr ""
 
@@ -1524,30 +1536,30 @@
 msgid "List of news categories values available for this entity (one per line)"
 msgstr ""
 
 #: imio/smartweb/common/vocabularies.py:110
 msgid "Liste"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:299
+#: imio/directory/core/contents/contact/content.py:317
 #: imio/smartweb/core/behaviors/minisite.py:41
 #: imio/smartweb/core/behaviors/subsite.py:33
 msgid "Logo"
 msgstr ""
 
 #: imio/smartweb/core/vocabularies.py:159
 msgid "Logo and title"
 msgstr ""
 
 #: imio/smartweb/core/behaviors/minisite.py:47
 #: imio/smartweb/core/behaviors/subsite.py:39
 msgid "Logo display"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/utils.py:269
+#: imio/smartweb/core/contents/sections/contact/utils.py:274
 msgid "Lunch time"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/macros.pt:42
 msgid "Manage section contents"
 msgstr ""
 
@@ -1569,19 +1581,19 @@
 
 #: imio/smartweb/core/contents/sections/collection/content.py:48
 #: imio/smartweb/core/contents/sections/events/content.py:70
 #: imio/smartweb/core/contents/sections/news/content.py:70
 msgid "Maximum number of batches to display"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/content.py:69
+#: imio/smartweb/core/contents/sections/contact/content.py:65
 msgid "Maximum number of contacts by line"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/content.py:70
+#: imio/smartweb/core/contents/sections/contact/content.py:66
 msgid "Maximum number of contacts by line (on PC)"
 msgstr ""
 
 #: imio/smartweb/core/behaviors/subsite.py:48
 msgid "Menu depth"
 msgstr ""
 
@@ -1702,25 +1714,25 @@
 msgid "Not allowed to add Files or Images in imio.directory.Entity"
 msgstr ""
 
 #: imio/smartweb/common/interfaces.py:34
 msgid "Number"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:92
+#: imio/directory/core/contents/contact/content.py:110
 msgid "Number (format: +32475010203)"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/collection/content.py:41
 #: imio/smartweb/core/contents/sections/events/content.py:63
 #: imio/smartweb/core/contents/sections/files/content.py:15
 msgid "Number of items per batch"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/content.py:62
+#: imio/smartweb/core/contents/sections/contact/content.py:58
 msgid "Number of items per batch (only for carousel mode)"
 msgstr ""
 
 #: imio/smartweb/core/contents/rest/directory/content.py:25
 #: imio/smartweb/core/contents/rest/events/content.py:30
 #: imio/smartweb/core/contents/rest/news/content.py:21
 msgid "Number of items to display"
@@ -1742,19 +1754,19 @@
 msgid "Only one procedure field can be filled !"
 msgstr ""
 
 #: imio/smartweb/core/contents/blocks/link/content.py:34
 msgid "Only used in table view (takes precedence over image)"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/utils.py:246
+#: imio/smartweb/core/contents/sections/contact/utils.py:251
 msgid "Open"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/utils.py:263
+#: imio/smartweb/core/contents/sections/contact/utils.py:268
 msgid "Open at "
 msgstr ""
 
 #: imio/smartweb/core/contents/blocks/link/content.py:23
 #: imio/smartweb/core/contents/sections/slide/content.py:66
 msgid "Open in a new tab"
 msgstr ""
@@ -1823,30 +1835,34 @@
 msgid "Party and folklore"
 msgstr ""
 
 #: imio/smartweb/common/upgrades/configure.zcml:69
 msgid "Patch (Remove select2) eea.facetednavigation jquery"
 msgstr ""
 
-#: imio/smartweb/core/vocabularies.py:142
+#: imio/smartweb/core/vocabularies.py:141
 msgid "Paysage"
 msgstr ""
 
 #: imio/directory/core/vocabularies.py:53
 msgid "Personal email"
 msgstr ""
 
 #: imio/directory/core/vocabularies.py:39
 msgid "Personal phone"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:142
+#: imio/directory/core/contents/contact/content.py:160
 msgid "Phones"
 msgstr ""
 
+#: imio/smartweb/core/browser/faceted/configure.zcml:37
+msgid "Photo gallery"
+msgstr ""
+
 #: imio/smartweb/core/contents/sections/slide/content.py:41
 msgid "Picture will be displayed as slide background"
 msgstr ""
 
 #: imio/directory/core/vocabularies.py:68
 msgid "Pinterest"
 msgstr ""
@@ -1903,15 +1919,15 @@
 msgid "Portal Page content type to print informations"
 msgstr ""
 
 #: imio/smartweb/core/profiles/icons/contenttypes/registry.xml
 msgid "PortalPage content type icon"
 msgstr ""
 
-#: imio/smartweb/core/vocabularies.py:141
+#: imio/smartweb/core/vocabularies.py:142
 msgid "Portrait"
 msgstr ""
 
 #: imio/directory/core/vocabularies.py:20
 msgid "Position (mayor, alderman, advisor, director, head of department, etc.)"
 msgstr ""
 
@@ -1937,15 +1953,15 @@
 msgid "Presse"
 msgstr ""
 
 #: imio/smartweb/core/profiles/default/actions.xml
 msgid "Preview"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:175
+#: imio/directory/core/contents/contact/content.py:193
 msgid "Private contact informations"
 msgstr ""
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.Procedure.xml
 msgid "Procedure"
 msgstr ""
 
@@ -2006,15 +2022,15 @@
 msgid "Refuse all"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/events/content.py:30
 msgid "Related agenda"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/content.py:23
+#: imio/smartweb/core/contents/sections/contact/content.py:24
 msgid "Related contacts"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/news/content.py:30
 msgid "Related news folder"
 msgstr ""
 
@@ -2035,14 +2051,18 @@
 msgid "Remove plone.patternslib deprecated bundles"
 msgstr ""
 
 #: imio/news/policy/upgrades/configure.zcml:12
 msgid "Remove ugly IImioEventsPolicyLayer"
 msgstr ""
 
+#: imio/smartweb/policy/upgrades/configure.zcml:148
+msgid "Restore removed behaviors on Collection type"
+msgstr ""
+
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionText.xml
 msgid "Rich text section for a page"
 msgstr ""
 
 #: imio/smartweb/core/vocabularies.py:310
 msgid "Right"
 msgstr ""
@@ -2055,15 +2075,15 @@
 msgid "Saturday"
 msgstr ""
 
 #: imio/smartweb/common/browser/privacy/form.py:27
 msgid "Save my choices"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/macros.pt:121
+#: imio/smartweb/core/contents/sections/contact/macros.pt:122
 #: imio/smartweb/core/vocabularies.py:177
 msgid "Schedule"
 msgstr ""
 
 #: imio/smartweb/core/viewlets/searchbox.pt:9
 msgid "Search"
 msgstr ""
@@ -2172,19 +2192,19 @@
 msgid "Select agenda to display"
 msgstr ""
 
 #: imio/events/core/contents/event/content.py:168
 msgid "Select agendas where this event will be displayed. Current agenda is always selected."
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/content.py:24
+#: imio/smartweb/core/contents/sections/contact/content.py:25
 msgid "Select contacts. If you can't find contacts you want, make sure it exists in the directory and that its \"state\" is published."
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:308
+#: imio/directory/core/contents/contact/content.py:326
 msgid "Select entities where this contact will be displayed. Current entity will always be selected."
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/text/content.py:25
 msgid "Select image size"
 msgstr ""
 
@@ -2216,15 +2236,15 @@
 msgid "Selected agenda"
 msgstr ""
 
 #: imio/events/core/contents/event/content.py:167
 msgid "Selected agendas"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:307
+#: imio/directory/core/contents/contact/content.py:325
 msgid "Selected entities"
 msgstr ""
 
 #: imio/smartweb/core/contents/rest/events/content.py:17
 msgid "Selected event types"
 msgstr ""
 
@@ -2397,15 +2417,15 @@
 msgid "Subsite has been disabled"
 msgstr ""
 
 #: imio/smartweb/core/browser/subsite/settings.py:25
 msgid "Subsite has been successfully activated"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:239
+#: imio/directory/core/contents/contact/content.py:257
 #: imio/smartweb/core/contents/sections/postit/content.py:26
 msgid "Subtitle"
 msgstr ""
 
 #: imio/smartweb/core/contents/folder/configure.zcml:72
 msgid "Summary view"
 msgstr ""
@@ -2414,18 +2434,14 @@
 msgid "Summary view with images"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/contact/utils.py:106
 msgid "Sunday"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/content.py:51
-msgid "Switch lead image to portrait mode"
-msgstr ""
-
 #: imio/smartweb/core/contents/sections/links/configure.zcml:15
 #: imio/smartweb/core/contents/sections/selections/configure.zcml:15
 msgid "Table view"
 msgstr ""
 
 #: imio/smartweb/core/viewlets/toolbar.py:183
 msgid "Take part of workshop"
@@ -2505,15 +2521,15 @@
 msgid "Third page"
 msgstr ""
 
 #: imio/smartweb/common/privacy.py:70
 msgid "This feature requires cookies acceptation.<br/><a class=\"pat-plone-modal\" href=\"${consent_url}\">Review your cookies preferences</a>."
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:234
+#: imio/directory/core/contents/contact/content.py:252
 #: imio/events/core/contents/event/content.py:51
 #: imio/news/core/contents/newsitem/content.py:37
 msgid "This field is required if the content must be available in this language"
 msgstr ""
 
 #: imio/smartweb/core/browser/controlpanel.py:91
 msgid "This information is used for search results redirection"
@@ -2536,15 +2552,15 @@
 msgid "Ticket url"
 msgstr ""
 
 #: imio/events/core/contents/event/content.py:118
 msgid "Ticket url to subscribe to this event"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:233
+#: imio/directory/core/contents/contact/content.py:251
 #: imio/events/core/contents/event/content.py:50
 #: imio/news/core/contents/newsitem/content.py:36
 msgid "Title"
 msgstr ""
 
 #: imio/smartweb/core/vocabularies.py:173
 msgid "Title and Subtitle"
@@ -2598,23 +2614,23 @@
 msgid "Twitter url for this news"
 msgstr ""
 
 #: imio/smartweb/core/vocabularies.py:127
 msgid "Two third of width"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:85
+#: imio/directory/core/contents/contact/content.py:103
 msgid "Type"
 msgstr ""
 
 #: imio/smartweb/core/contents/blocks/link/content.py:26
 msgid "URL"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:162
+#: imio/directory/core/contents/contact/content.py:180
 msgid "URLs"
 msgstr ""
 
 #: imio/directory/policy/configure.zcml:44
 msgid "Uninstalls the imio.directory.policy add-on."
 msgstr ""
 
@@ -2847,14 +2863,18 @@
 msgid "Upgrade policy 1029 to 1030"
 msgstr ""
 
 #: imio/smartweb/policy/upgrades/configure.zcml:140
 msgid "Upgrade policy 1030 to 1031"
 msgstr ""
 
+#: imio/smartweb/policy/upgrades/configure.zcml:148
+msgid "Upgrade policy 1031 to 1032"
+msgstr ""
+
 #: imio/directory/policy/upgrades/configure.zcml:12
 #: imio/events/policy/upgrades/configure.zcml:12
 msgid "Upgrade policy from 1000 to 1001"
 msgstr ""
 
 #: imio/events/policy/upgrades/configure.zcml:20
 #: imio/news/policy/upgrades/configure.zcml:20
@@ -2878,15 +2898,15 @@
 msgid "Upgrade policy from 1026 to 1027"
 msgstr ""
 
 #: imio/smartweb/policy/upgrades/configure.zcml:124
 msgid "Upgrade policy from 1028 to 1029"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:123
+#: imio/directory/core/contents/contact/content.py:141
 msgid "Url"
 msgstr ""
 
 #: imio/smartweb/core/browser/controlpanel.py:25
 msgid "Url to get forms from your e-guichet"
 msgstr ""
 
@@ -2912,15 +2932,15 @@
 msgid "Use custom spotlight to avoid bad gallery refresh"
 msgstr ""
 
 #: imio/directory/core/vocabularies.py:86
 msgid "Useful numbers"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:140
+#: imio/directory/core/contents/contact/content.py:158
 msgid "VAT number"
 msgstr ""
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionVideo.xml
 msgid "Video section"
 msgstr ""
 
@@ -2952,15 +2972,15 @@
 msgid "View - News"
 msgstr ""
 
 #: imio/smartweb/common/vocabularies.py:109
 msgid "Vignette"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/content.py:34
+#: imio/smartweb/core/contents/sections/contact/content.py:35
 msgid "Visible blocks"
 msgstr ""
 
 #: imio/smartweb/core/browser/controlpanel.py:116
 msgid "Vocabulary term"
 msgstr ""
```

### Comparing `imio.smartweb.locales-1.1.8/src/imio/smartweb/locales/locales/nl/LC_MESSAGES/imio.smartweb.po` & `imio.smartweb.locales-1.1.9/src/imio/smartweb/locales/locales/nl/LC_MESSAGES/imio.smartweb.po`

 * *Files 2% similar despite different names*

```diff
@@ -181,15 +181,15 @@
 msgstr ""
 
 #: imio/smartweb/common/behaviors/configure.zcml:13
 msgid "Add topics on content types."
 msgstr ""
 
 #: imio/smartweb/common/interfaces.py:30
-#: imio/smartweb/core/contents/sections/contact/macros.pt:96
+#: imio/smartweb/core/contents/sections/contact/macros.pt:97
 #: imio/smartweb/core/vocabularies.py:175
 msgid "Address"
 msgstr ""
 
 #: imio/smartweb/common/vocabularies.py:108
 msgid "Affiche"
 msgstr ""
@@ -226,15 +226,15 @@
 msgid "Allow to select quick access elements for current context."
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/slide/content.py:53
 msgid "Alternatively as a picture"
 msgstr ""
 
-#: imio/smartweb/core/contents/folder/views.py:134
+#: imio/smartweb/core/contents/folder/views.py:135
 msgid "Apply"
 msgstr ""
 
 #: imio/smartweb/core/viewlets/toolbar.py:169
 msgid "Ask a question"
 msgstr ""
 
@@ -263,15 +263,15 @@
 msgid "Bad URL format '${val}' (good format sample: https://www.imio.be)."
 msgstr ""
 
 #: imio/directory/core/browser/import.py:90
 msgid "Bad mail format '${val}' (good format sample: noreply@imio.be)."
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:47
+#: imio/directory/core/contents/contact/content.py:65
 msgid "Bad phone format"
 msgstr ""
 
 #: imio/directory/core/browser/import.py:72
 msgid "Bad phone format '${val}' (good format sample: +32444556677)."
 msgstr ""
 
@@ -299,18 +299,22 @@
 msgid "Block view with images"
 msgstr ""
 
 #: imio/smartweb/core/profiles/icons/contenttypes/registry.xml
 msgid "BlockLink content type icon"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/content.py:35
+#: imio/smartweb/core/contents/sections/contact/content.py:36
 msgid "Blocks that will be displayed in contact"
 msgstr ""
 
+#: imio/directory/core/vocabularies.py:89
+msgid "Bottle bubbles"
+msgstr ""
+
 #: imio/smartweb/core/vocabularies.py:311
 msgid "Bottom"
 msgstr ""
 
 #: imio/smartweb/core/upgrades/configure.zcml:68
 msgid "By default, Plone open external (Section text / Tiny) links in new tab"
 msgstr ""
@@ -485,15 +489,15 @@
 msgstr ""
 
 #: imio/smartweb/core/behaviors/minisite.py:48
 #: imio/smartweb/core/behaviors/subsite.py:40
 msgid "Choose your display mode"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/content.py:56
+#: imio/smartweb/core/contents/sections/contact/content.py:52
 msgid "Choose your gallery layout mode"
 msgstr ""
 
 #: imio/directory/core/contents/entity/content.py:23
 #: imio/events/core/contents/entity/content.py:19
 #: imio/news/core/contents/entity/content.py:19
 msgid "Choose zip codes for this entity"
@@ -600,18 +604,22 @@
 msgid "Click to preview content (without editor actions)."
 msgstr ""
 
 #: imio/smartweb/core/viewlets/navigation.py:85
 msgid "Close"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/utils.py:239
+#: imio/smartweb/core/contents/sections/contact/utils.py:244
 msgid "Closed"
 msgstr ""
 
+#: imio/directory/core/vocabularies.py:90
+msgid "Clothing bubbles"
+msgstr ""
+
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionCollection.xml
 msgid "Collection section"
 msgstr ""
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionCollection.xml
 msgid "Collection section for a page"
 msgstr ""
@@ -651,15 +659,15 @@
 msgid "Contact"
 msgstr ""
 
 #: imio/directory/core/profiles/default/types/imio.directory.Contact.xml
 msgid "Contact content type"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:137
+#: imio/directory/core/contents/contact/content.py:155
 #: imio/smartweb/core/vocabularies.py:174
 msgid "Contact informations"
 msgstr ""
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionContact.xml
 msgid "Contact section"
 msgstr ""
@@ -672,14 +680,18 @@
 msgid "Contact title is missing."
 msgstr ""
 
 #: imio/directory/core/browser/import.py:201
 msgid "Contact type is missing."
 msgstr ""
 
+#: imio/directory/core/vocabularies.py:91
+msgid "Container parks"
+msgstr ""
+
 #: imio/smartweb/common/browser/privacy/form.py:12
 msgid "Cookies choice"
 msgstr ""
 
 #: imio/smartweb/common/viewlets/colophon.pt:19
 msgid "Cookies preferences"
 msgstr ""
@@ -724,15 +736,15 @@
 msgid "Define number of levels in menu navigation subsite"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/macros.pt:53
 msgid "Delete section"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:240
+#: imio/directory/core/contents/contact/content.py:258
 #: imio/events/core/contents/event/content.py:56
 #: imio/news/core/contents/newsitem/content.py:42
 msgid "Description"
 msgstr ""
 
 #: imio/smartweb/core/browser/controlpanel.py:72
 msgid "Directory SolR Core ID"
@@ -800,29 +812,29 @@
 msgid "Display map"
 msgstr ""
 
 #: imio/directory/core/vocabularies.py:85
 msgid "Drinking water point"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:263
+#: imio/directory/core/contents/contact/content.py:281
 #: imio/events/core/contents/event/content.py:80
 #: imio/news/core/contents/newsitem/content.py:66
 msgid "Dutch translations"
 msgstr ""
 
 #: imio/smartweb/core/contents/pages/procedure/content.py:21
 msgid "E-Guichet procedure"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:112
+#: imio/directory/core/contents/contact/content.py:130
 msgid "E-mail"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:152
+#: imio/directory/core/contents/contact/content.py:170
 msgid "E-mails"
 msgstr ""
 
 #: imio/smartweb/common/vocabularies.py:22
 msgid "Economics"
 msgstr ""
 
@@ -854,15 +866,15 @@
 msgid "Enable minisite"
 msgstr ""
 
 #: imio/smartweb/core/profiles/default/actions.xml
 msgid "Enable subsite"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:246
+#: imio/directory/core/contents/contact/content.py:264
 #: imio/events/core/contents/event/content.py:63
 #: imio/news/core/contents/newsitem/content.py:49
 msgid "English translations"
 msgstr ""
 
 #: imio/smartweb/core/browser/controlpanel.py:17
 msgid "Enter the language code. Ex.: en"
@@ -968,15 +980,15 @@
 msgid "Example : namur.be (SMARTWEB_PLAUSIBLE_SITE varenv has precedence over this.)"
 msgstr ""
 
 #: imio/smartweb/core/browser/controlpanel.py:146
 msgid "Example : plausible.imio.be (SMARTWEB_PLAUSIBLE_URL varenv has precedence over this.)"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:300
+#: imio/directory/core/contents/contact/content.py:318
 msgid "Example : shop, service, association logo"
 msgstr ""
 
 #: imio/smartweb/core/behaviors/listing.py:19
 msgid "Exclude from parent listing"
 msgstr ""
 
@@ -1020,39 +1032,39 @@
 msgid "Facebook url for this event"
 msgstr ""
 
 #: imio/news/core/contents/newsitem/content.py:101
 msgid "Facebook url for this news"
 msgstr ""
 
-#: imio/smartweb/core/browser/faceted/configure.zcml:67
+#: imio/smartweb/core/browser/faceted/configure.zcml:81
 msgid "Faceted block view"
 msgstr ""
 
-#: imio/smartweb/core/browser/faceted/configure.zcml:74
+#: imio/smartweb/core/browser/faceted/configure.zcml:88
 msgid "Faceted block view with images"
 msgstr ""
 
 #: imio/smartweb/core/browser/faceted/configure.zcml:16
 msgid "Faceted items preview"
 msgstr ""
 
-#: imio/smartweb/core/browser/faceted/configure.zcml:97
+#: imio/smartweb/core/browser/faceted/configure.zcml:111
 msgid "Faceted map"
 msgstr ""
 
-#: imio/smartweb/core/browser/faceted/configure.zcml:81
+#: imio/smartweb/core/browser/faceted/configure.zcml:95
 msgid "Faceted summary view"
 msgstr ""
 
-#: imio/smartweb/core/browser/faceted/configure.zcml:88
+#: imio/smartweb/core/browser/faceted/configure.zcml:102
 msgid "Faceted summary view with images"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:317
+#: imio/directory/core/contents/contact/content.py:335
 msgid "Facilities"
 msgstr ""
 
 #: imio/events/core/contents/event/content.py:154
 #: imio/events/core/contents/event/view.pt:57
 msgid "Facilities for person with reduced mobility"
 msgstr ""
@@ -1133,15 +1145,15 @@
 msgid "Footer has been successfully added"
 msgstr ""
 
 #: imio/smartweb/core/contents/folder/content.py:26
 msgid "For the anonymous visitor, the folder and the selected item are one. When he clicks on the folder, the item is displayed."
 msgstr ""
 
-#: imio/smartweb/core/contents/folder/views.py:105
+#: imio/smartweb/core/contents/folder/views.py:106
 msgid "Form to choose item to be displayed as the home page of the folder"
 msgstr ""
 
 #: imio/directory/core/vocabularies.py:88
 msgid "Free WIFI"
 msgstr ""
 
@@ -1162,27 +1174,27 @@
 msgid "Full width"
 msgstr ""
 
 #: imio/smartweb/core/vocabularies.py:180
 msgid "Gallery"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/content.py:55
+#: imio/smartweb/core/contents/sections/contact/content.py:51
 msgid "Gallery mode"
 msgstr ""
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionGallery.xml
 msgid "Gallery section"
 msgstr ""
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionGallery.xml
 msgid "Gallery section for a page"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:229
+#: imio/directory/core/contents/contact/content.py:247
 #: imio/events/core/contents/event/content.py:46
 #: imio/news/core/contents/newsitem/content.py:32
 msgid "German translations"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/events/content.py:37
 msgid "Get priory on related agenda for these specifics events."
@@ -1320,15 +1332,15 @@
 msgid "Image orientation"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/gallery/content.py:16
 msgid "Image scale for images"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/content.py:77
+#: imio/smartweb/core/contents/sections/contact/content.py:73
 msgid "Image scale for images (only for gallery mode)"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/text/content.py:24
 msgid "Image size"
 msgstr ""
 
@@ -1351,15 +1363,15 @@
 msgstr ""
 
 #: imio/events/core/contents/event/content.py:178
 #: imio/news/core/contents/newsitem/content.py:133
 msgid "Important! These categories are used to supplement the information provided by the topics"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:318
+#: imio/directory/core/contents/contact/content.py:336
 msgid "Important! These categories make it possible to highlight and geolocate certain basic services"
 msgstr ""
 
 #: imio/smartweb/common/behaviors/topics.py:17
 msgid "Important! Topics are used to filter search results and create lists"
 msgstr ""
 
@@ -1389,28 +1401,28 @@
 msgid "Installs the imio.events.policy add-on."
 msgstr ""
 
 #: imio/news/policy/configure.zcml:36
 msgid "Installs the imio.news.policy add-on."
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:210
+#: imio/directory/core/contents/contact/content.py:228
 msgid "Internal note"
 msgstr ""
 
 #: imio/events/core/vocabularies.py:25
 msgid "Internships and courses"
 msgstr ""
 
 #: imio/smartweb/core/contents/folder/content.py:25
 msgid "Item(s) that can be selected as the folder default page."
 msgstr ""
 
 #: imio/events/core/contents/event/views.py:77
-#: imio/smartweb/core/contents/sections/contact/macros.pt:111
+#: imio/smartweb/core/contents/sections/contact/macros.pt:112
 #: imio/smartweb/core/contents/sections/contact/utils.py:56
 msgid "Itinerary"
 msgstr ""
 
 #: imio/news/core/vocabularies.py:17
 msgid "Job offer"
 msgstr ""
@@ -1424,19 +1436,19 @@
 msgstr ""
 
 #: imio/events/core/contents/event/view.pt:107
 #: imio/news/core/contents/newsitem/view.pt:64
 msgid "Keywords"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:100
+#: imio/directory/core/contents/contact/content.py:118
 msgid "Label (Secretariat, Manager office, Sales,...)"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:79
+#: imio/directory/core/contents/contact/content.py:97
 msgid "Label (direction, Main number,...)"
 msgstr ""
 
 #: imio/smartweb/core/browser/controlpanel.py:16
 msgid "Language (en, fr,...)"
 msgstr ""
 
@@ -1518,30 +1530,30 @@
 msgid "List of news categories values available for this entity (one per line)"
 msgstr ""
 
 #: imio/smartweb/common/vocabularies.py:110
 msgid "Liste"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:299
+#: imio/directory/core/contents/contact/content.py:317
 #: imio/smartweb/core/behaviors/minisite.py:41
 #: imio/smartweb/core/behaviors/subsite.py:33
 msgid "Logo"
 msgstr ""
 
 #: imio/smartweb/core/vocabularies.py:159
 msgid "Logo and title"
 msgstr ""
 
 #: imio/smartweb/core/behaviors/minisite.py:47
 #: imio/smartweb/core/behaviors/subsite.py:39
 msgid "Logo display"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/utils.py:269
+#: imio/smartweb/core/contents/sections/contact/utils.py:274
 msgid "Lunch time"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/macros.pt:42
 msgid "Manage section contents"
 msgstr ""
 
@@ -1563,19 +1575,19 @@
 
 #: imio/smartweb/core/contents/sections/collection/content.py:48
 #: imio/smartweb/core/contents/sections/events/content.py:70
 #: imio/smartweb/core/contents/sections/news/content.py:70
 msgid "Maximum number of batches to display"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/content.py:69
+#: imio/smartweb/core/contents/sections/contact/content.py:65
 msgid "Maximum number of contacts by line"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/content.py:70
+#: imio/smartweb/core/contents/sections/contact/content.py:66
 msgid "Maximum number of contacts by line (on PC)"
 msgstr ""
 
 #: imio/smartweb/core/behaviors/subsite.py:48
 msgid "Menu depth"
 msgstr ""
 
@@ -1696,25 +1708,25 @@
 msgid "Not allowed to add Files or Images in imio.directory.Entity"
 msgstr ""
 
 #: imio/smartweb/common/interfaces.py:34
 msgid "Number"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:92
+#: imio/directory/core/contents/contact/content.py:110
 msgid "Number (format: +32475010203)"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/collection/content.py:41
 #: imio/smartweb/core/contents/sections/events/content.py:63
 #: imio/smartweb/core/contents/sections/files/content.py:15
 msgid "Number of items per batch"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/content.py:62
+#: imio/smartweb/core/contents/sections/contact/content.py:58
 msgid "Number of items per batch (only for carousel mode)"
 msgstr ""
 
 #: imio/smartweb/core/contents/rest/directory/content.py:25
 #: imio/smartweb/core/contents/rest/events/content.py:30
 #: imio/smartweb/core/contents/rest/news/content.py:21
 msgid "Number of items to display"
@@ -1736,19 +1748,19 @@
 msgid "Only one procedure field can be filled !"
 msgstr ""
 
 #: imio/smartweb/core/contents/blocks/link/content.py:34
 msgid "Only used in table view (takes precedence over image)"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/utils.py:246
+#: imio/smartweb/core/contents/sections/contact/utils.py:251
 msgid "Open"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/utils.py:263
+#: imio/smartweb/core/contents/sections/contact/utils.py:268
 msgid "Open at "
 msgstr ""
 
 #: imio/smartweb/core/contents/blocks/link/content.py:23
 #: imio/smartweb/core/contents/sections/slide/content.py:66
 msgid "Open in a new tab"
 msgstr ""
@@ -1817,30 +1829,34 @@
 msgid "Party and folklore"
 msgstr ""
 
 #: imio/smartweb/common/upgrades/configure.zcml:69
 msgid "Patch (Remove select2) eea.facetednavigation jquery"
 msgstr ""
 
-#: imio/smartweb/core/vocabularies.py:142
+#: imio/smartweb/core/vocabularies.py:141
 msgid "Paysage"
 msgstr ""
 
 #: imio/directory/core/vocabularies.py:53
 msgid "Personal email"
 msgstr ""
 
 #: imio/directory/core/vocabularies.py:39
 msgid "Personal phone"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:142
+#: imio/directory/core/contents/contact/content.py:160
 msgid "Phones"
 msgstr ""
 
+#: imio/smartweb/core/browser/faceted/configure.zcml:37
+msgid "Photo gallery"
+msgstr ""
+
 #: imio/smartweb/core/contents/sections/slide/content.py:41
 msgid "Picture will be displayed as slide background"
 msgstr ""
 
 #: imio/directory/core/vocabularies.py:68
 msgid "Pinterest"
 msgstr ""
@@ -1897,15 +1913,15 @@
 msgid "Portal Page content type to print informations"
 msgstr ""
 
 #: imio/smartweb/core/profiles/icons/contenttypes/registry.xml
 msgid "PortalPage content type icon"
 msgstr ""
 
-#: imio/smartweb/core/vocabularies.py:141
+#: imio/smartweb/core/vocabularies.py:142
 msgid "Portrait"
 msgstr ""
 
 #: imio/directory/core/vocabularies.py:20
 msgid "Position (mayor, alderman, advisor, director, head of department, etc.)"
 msgstr ""
 
@@ -1931,15 +1947,15 @@
 msgid "Presse"
 msgstr ""
 
 #: imio/smartweb/core/profiles/default/actions.xml
 msgid "Preview"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:175
+#: imio/directory/core/contents/contact/content.py:193
 msgid "Private contact informations"
 msgstr ""
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.Procedure.xml
 msgid "Procedure"
 msgstr ""
 
@@ -2000,15 +2016,15 @@
 msgid "Refuse all"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/events/content.py:30
 msgid "Related agenda"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/content.py:23
+#: imio/smartweb/core/contents/sections/contact/content.py:24
 msgid "Related contacts"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/news/content.py:30
 msgid "Related news folder"
 msgstr ""
 
@@ -2029,14 +2045,18 @@
 msgid "Remove plone.patternslib deprecated bundles"
 msgstr ""
 
 #: imio/news/policy/upgrades/configure.zcml:12
 msgid "Remove ugly IImioEventsPolicyLayer"
 msgstr ""
 
+#: imio/smartweb/policy/upgrades/configure.zcml:148
+msgid "Restore removed behaviors on Collection type"
+msgstr ""
+
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionText.xml
 msgid "Rich text section for a page"
 msgstr ""
 
 #: imio/smartweb/core/vocabularies.py:310
 msgid "Right"
 msgstr ""
@@ -2049,15 +2069,15 @@
 msgid "Saturday"
 msgstr ""
 
 #: imio/smartweb/common/browser/privacy/form.py:27
 msgid "Save my choices"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/macros.pt:121
+#: imio/smartweb/core/contents/sections/contact/macros.pt:122
 #: imio/smartweb/core/vocabularies.py:177
 msgid "Schedule"
 msgstr ""
 
 #: imio/smartweb/core/viewlets/searchbox.pt:9
 msgid "Search"
 msgstr ""
@@ -2166,19 +2186,19 @@
 msgid "Select agenda to display"
 msgstr ""
 
 #: imio/events/core/contents/event/content.py:168
 msgid "Select agendas where this event will be displayed. Current agenda is always selected."
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/content.py:24
+#: imio/smartweb/core/contents/sections/contact/content.py:25
 msgid "Select contacts. If you can't find contacts you want, make sure it exists in the directory and that its \"state\" is published."
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:308
+#: imio/directory/core/contents/contact/content.py:326
 msgid "Select entities where this contact will be displayed. Current entity will always be selected."
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/text/content.py:25
 msgid "Select image size"
 msgstr ""
 
@@ -2210,15 +2230,15 @@
 msgid "Selected agenda"
 msgstr ""
 
 #: imio/events/core/contents/event/content.py:167
 msgid "Selected agendas"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:307
+#: imio/directory/core/contents/contact/content.py:325
 msgid "Selected entities"
 msgstr ""
 
 #: imio/smartweb/core/contents/rest/events/content.py:17
 msgid "Selected event types"
 msgstr ""
 
@@ -2391,15 +2411,15 @@
 msgid "Subsite has been disabled"
 msgstr ""
 
 #: imio/smartweb/core/browser/subsite/settings.py:25
 msgid "Subsite has been successfully activated"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:239
+#: imio/directory/core/contents/contact/content.py:257
 #: imio/smartweb/core/contents/sections/postit/content.py:26
 msgid "Subtitle"
 msgstr ""
 
 #: imio/smartweb/core/contents/folder/configure.zcml:72
 msgid "Summary view"
 msgstr ""
@@ -2408,18 +2428,14 @@
 msgid "Summary view with images"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/contact/utils.py:106
 msgid "Sunday"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/content.py:51
-msgid "Switch lead image to portrait mode"
-msgstr ""
-
 #: imio/smartweb/core/contents/sections/links/configure.zcml:15
 #: imio/smartweb/core/contents/sections/selections/configure.zcml:15
 msgid "Table view"
 msgstr ""
 
 #: imio/smartweb/core/viewlets/toolbar.py:183
 msgid "Take part of workshop"
@@ -2499,15 +2515,15 @@
 msgid "Third page"
 msgstr ""
 
 #: imio/smartweb/common/privacy.py:70
 msgid "This feature requires cookies acceptation.<br/><a class=\"pat-plone-modal\" href=\"${consent_url}\">Review your cookies preferences</a>."
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:234
+#: imio/directory/core/contents/contact/content.py:252
 #: imio/events/core/contents/event/content.py:51
 #: imio/news/core/contents/newsitem/content.py:37
 msgid "This field is required if the content must be available in this language"
 msgstr ""
 
 #: imio/smartweb/core/browser/controlpanel.py:91
 msgid "This information is used for search results redirection"
@@ -2530,15 +2546,15 @@
 msgid "Ticket url"
 msgstr ""
 
 #: imio/events/core/contents/event/content.py:118
 msgid "Ticket url to subscribe to this event"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:233
+#: imio/directory/core/contents/contact/content.py:251
 #: imio/events/core/contents/event/content.py:50
 #: imio/news/core/contents/newsitem/content.py:36
 msgid "Title"
 msgstr ""
 
 #: imio/smartweb/core/vocabularies.py:173
 msgid "Title and Subtitle"
@@ -2592,23 +2608,23 @@
 msgid "Twitter url for this news"
 msgstr ""
 
 #: imio/smartweb/core/vocabularies.py:127
 msgid "Two third of width"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:85
+#: imio/directory/core/contents/contact/content.py:103
 msgid "Type"
 msgstr ""
 
 #: imio/smartweb/core/contents/blocks/link/content.py:26
 msgid "URL"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:162
+#: imio/directory/core/contents/contact/content.py:180
 msgid "URLs"
 msgstr ""
 
 #: imio/directory/policy/configure.zcml:44
 msgid "Uninstalls the imio.directory.policy add-on."
 msgstr ""
 
@@ -2841,14 +2857,18 @@
 msgid "Upgrade policy 1029 to 1030"
 msgstr ""
 
 #: imio/smartweb/policy/upgrades/configure.zcml:140
 msgid "Upgrade policy 1030 to 1031"
 msgstr ""
 
+#: imio/smartweb/policy/upgrades/configure.zcml:148
+msgid "Upgrade policy 1031 to 1032"
+msgstr ""
+
 #: imio/directory/policy/upgrades/configure.zcml:12
 #: imio/events/policy/upgrades/configure.zcml:12
 msgid "Upgrade policy from 1000 to 1001"
 msgstr ""
 
 #: imio/events/policy/upgrades/configure.zcml:20
 #: imio/news/policy/upgrades/configure.zcml:20
@@ -2872,15 +2892,15 @@
 msgid "Upgrade policy from 1026 to 1027"
 msgstr ""
 
 #: imio/smartweb/policy/upgrades/configure.zcml:124
 msgid "Upgrade policy from 1028 to 1029"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:123
+#: imio/directory/core/contents/contact/content.py:141
 msgid "Url"
 msgstr ""
 
 #: imio/smartweb/core/browser/controlpanel.py:25
 msgid "Url to get forms from your e-guichet"
 msgstr ""
 
@@ -2906,15 +2926,15 @@
 msgid "Use custom spotlight to avoid bad gallery refresh"
 msgstr ""
 
 #: imio/directory/core/vocabularies.py:86
 msgid "Useful numbers"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:140
+#: imio/directory/core/contents/contact/content.py:158
 msgid "VAT number"
 msgstr ""
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionVideo.xml
 msgid "Video section"
 msgstr ""
 
@@ -2946,15 +2966,15 @@
 msgid "View - News"
 msgstr ""
 
 #: imio/smartweb/common/vocabularies.py:109
 msgid "Vignette"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/content.py:34
+#: imio/smartweb/core/contents/sections/contact/content.py:35
 msgid "Visible blocks"
 msgstr ""
 
 #: imio/smartweb/core/browser/controlpanel.py:116
 msgid "Vocabulary term"
 msgstr ""
```

### Comparing `imio.smartweb.locales-1.1.8/src/imio/smartweb/locales/locales/nl/LC_MESSAGES/plone.po` & `imio.smartweb.locales-1.1.9/src/imio/smartweb/locales/locales/nl/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `imio.smartweb.locales-1.1.8/src/imio/smartweb/locales/locales/plone-manual.pot` & `imio.smartweb.locales-1.1.9/src/imio/smartweb/locales/locales/plone-manual.pot`

 * *Files identical despite different names*

### Comparing `imio.smartweb.locales-1.1.8/src/imio.smartweb.locales.egg-info/PKG-INFO` & `imio.smartweb.locales-1.1.9/src/imio.smartweb.locales.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: imio.smartweb.locales
-Version: 1.1.8
+Version: 1.1.9
 Summary: Locales for iMio smartweb packages
 Home-page: https://github.com/imio/imio.smartweb.locales
 Author: iMio
 Author-email: christophe.boulanger@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/imio.smartweb.locales
 Project-URL: Source, https://github.com/imio/imio.smartweb.locales
 Project-URL: Tracker, https://github.com/imio/imio.smartweb.locales/issues
 Keywords: Python Plone CMS
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 5.2
 Classifier: Framework :: Plone :: 6.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -114,14 +113,21 @@
 - Affinitic, laurent.lasudry@affinitic.be
 
 
 Changelog
 =========
 
 
+1.1.9 (2023-11-20)
+------------------
+
+- WEB-4018 : Add missing French translations (new termes in directory vocabulary)
+  [boulch]
+
+
 1.1.8 (2023-10-25)
 ------------------
 
 - Add missing French translations
   [laulaz]
 
 
@@ -413,9 +419,7 @@
 
 
 1.0a1 (2021-04-19)
 ------------------
 
 - Initial release.
   [boulch]
-
-
```

### Comparing `imio.smartweb.locales-1.1.8/src/imio.smartweb.locales.egg-info/SOURCES.txt` & `imio.smartweb.locales-1.1.9/src/imio.smartweb.locales.egg-info/SOURCES.txt`

 * *Files identical despite different names*

