# Comparing `tmp/SQLAlchemyExample-0.1.8.tar.gz` & `tmp/SQLAlchemyExample-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SQLAlchemyExample-0.1.8.tar", last modified: Tue Aug  8 15:28:14 2023, max compression
+gzip compressed data, was "SQLAlchemyExample-0.1.9.tar", last modified: Wed Aug  9 00:03:59 2023, max compression
```

## Comparing `SQLAlchemyExample-0.1.8.tar` & `SQLAlchemyExample-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:28:14.498442 SQLAlchemyExample-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-08 15:27:59.000000 SQLAlchemyExample-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-08 15:27:59.000000 SQLAlchemyExample-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9015 2023-08-08 15:28:14.498442 SQLAlchemyExample-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8390 2023-08-08 15:27:59.000000 SQLAlchemyExample-0.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-08-08 15:27:59.000000 SQLAlchemyExample-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-08 15:27:59.000000 SQLAlchemyExample-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-08 15:28:14.498442 SQLAlchemyExample-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:28:14.494442 SQLAlchemyExample-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:28:14.498442 SQLAlchemyExample-0.1.8/src/SQLAlchemyExample.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9015 2023-08-08 15:28:14.000000 SQLAlchemyExample-0.1.8/src/SQLAlchemyExample.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-08 15:28:14.000000 SQLAlchemyExample-0.1.8/src/SQLAlchemyExample.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 15:28:14.000000 SQLAlchemyExample-0.1.8/src/SQLAlchemyExample.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-08 15:28:14.000000 SQLAlchemyExample-0.1.8/src/SQLAlchemyExample.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 15:28:14.000000 SQLAlchemyExample-0.1.8/src/SQLAlchemyExample.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:28:14.498442 SQLAlchemyExample-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-08-08 15:27:59.000000 SQLAlchemyExample-0.1.8/tests/test_otm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-08-08 15:27:59.000000 SQLAlchemyExample-0.1.8/tests/test_otm_sti.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-08-08 15:27:59.000000 SQLAlchemyExample-0.1.8/tests/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-08-08 15:27:59.000000 SQLAlchemyExample-0.1.8/tests/test_sti.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:03:59.365372 SQLAlchemyExample-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-09 00:03:44.000000 SQLAlchemyExample-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-09 00:03:44.000000 SQLAlchemyExample-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-08-09 00:03:59.365372 SQLAlchemyExample-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-08-09 00:03:44.000000 SQLAlchemyExample-0.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-08-09 00:03:44.000000 SQLAlchemyExample-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-08-09 00:03:44.000000 SQLAlchemyExample-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-09 00:03:59.369372 SQLAlchemyExample-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:03:59.361372 SQLAlchemyExample-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:03:59.365372 SQLAlchemyExample-0.1.9/src/SQLAlchemyExample.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-08-09 00:03:59.000000 SQLAlchemyExample-0.1.9/src/SQLAlchemyExample.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-09 00:03:59.000000 SQLAlchemyExample-0.1.9/src/SQLAlchemyExample.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 00:03:59.000000 SQLAlchemyExample-0.1.9/src/SQLAlchemyExample.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-09 00:03:59.000000 SQLAlchemyExample-0.1.9/src/SQLAlchemyExample.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 00:03:59.000000 SQLAlchemyExample-0.1.9/src/SQLAlchemyExample.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:03:59.365372 SQLAlchemyExample-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-08-09 00:03:44.000000 SQLAlchemyExample-0.1.9/tests/test_otm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-08-09 00:03:44.000000 SQLAlchemyExample-0.1.9/tests/test_otm_sti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-08-09 00:03:44.000000 SQLAlchemyExample-0.1.9/tests/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-08-09 00:03:44.000000 SQLAlchemyExample-0.1.9/tests/test_sti.py
```

### Comparing `SQLAlchemyExample-0.1.8/LICENSE` & `SQLAlchemyExample-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `SQLAlchemyExample-0.1.8/PKG-INFO` & `SQLAlchemyExample-0.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLAlchemyExample
-Version: 0.1.8
+Version: 0.1.9
 Summary: Exploring SQLAlchemy
 Author: Hendrik du Toit
 Author-email: hendrik@brightedge.co.za
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Database
@@ -88,40 +88,49 @@
 #. File names
     #. Not knowing what's to come and what will be added, it is difficult to determine a naming convention for source, test and other file names.  The owner will therefore be a "benevolent dictator" to rename and change names.
     #. Link the file name of the source code and the test so that it is easily linked.
 #. Branch names
     "enhancement" | "bug" | "hotfix"/< ticket_nr>_<description>
 
     where
+        enhancement - Planned improvement or addition to functionality; non-urgent.
 
-    ticket_nr: Ticket number assigned to the issue in GitHub.  Once an issue is registered, the owner will assign a ticket.
+        bug - An error or defect causing incorrect or unexpected behavior; typically fixed in regular development cycles.
 
-    description: GitHub issue title or combination of titles is more than one issue is addressed.
+        hotfix - An urgent, critical fix applied directly to the live environment, often bypassing regular development cycles.
+
+        ticket_nr: Ticket number assigned to the issue in GitHub.  Once an issue is registered, the owner will assign a ticket.
+
+        description: GitHub issue title or combination of titles is more than one issue is addressed.
 
 
 Releasing
 ~~~~~~~~~
 For the purpose of push and release of code two script files are included.  Use there two files to files to make life a
 bit easier.  The scripts make use of the ``gitit`` module to simplify tasks.
 
 #. ``push.bat`` - Use this script to push branches to GitHub repository.  In principle it does the following:
 
     usage: push message
 
+    e.g. push "Changed the Infinite Improbability Drive"
+
     #. .rst syntax check
     #. git add -A
     #. git commit -m message (with `pre-commit` including `black` and `flake8`)
     #. git push --all
 
 #. ``release.bat`` - Use this script to push a new tag and release to the GitHub repository.  Remember to change the version number in the setup.cfg else the workflow will fail.
 
     usage: release version  The version will match the release and the tag. Only issue a release once a push.bat was successful.  In principle it does the following:
 
+    e.g. relase 1.2.3
+
     #. Commit the changes
-    #. Create and push the release tag
+    #. Create and push the release tag with the correct naming conventions.
     #. Checkout master since it assumes that the branch is now merged with master and will be deleted.
     #. display a list of all the current branches as a reminder to delete the branch on completion.
 
 
 .. General
 
 .. |maintenance_n| image:: https://img.shields.io/badge/Maintenance%20Intended-✖-red.svg?style=flat-square
```

### Comparing `SQLAlchemyExample-0.1.8/README.rst` & `SQLAlchemyExample-0.1.9/src/SQLAlchemyExample.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: SQLAlchemyExample
+Version: 0.1.9
+Summary: Exploring SQLAlchemy
+Author: Hendrik du Toit
+Author-email: hendrik@brightedge.co.za
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development
+Classifier: Topic :: Database
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 ====================
 Exploring SQLAlchemy
 ====================
 
 +-------------------+---------------------------------------------------------------------------------------------+
 | **General**       | |maintenance_y| |semver| |license|                                                          |
 +-------------------+---------------------------------------------------------------------------------------------+
@@ -70,40 +88,49 @@
 #. File names
     #. Not knowing what's to come and what will be added, it is difficult to determine a naming convention for source, test and other file names.  The owner will therefore be a "benevolent dictator" to rename and change names.
     #. Link the file name of the source code and the test so that it is easily linked.
 #. Branch names
     "enhancement" | "bug" | "hotfix"/< ticket_nr>_<description>
 
     where
+        enhancement - Planned improvement or addition to functionality; non-urgent.
+
+        bug - An error or defect causing incorrect or unexpected behavior; typically fixed in regular development cycles.
+
+        hotfix - An urgent, critical fix applied directly to the live environment, often bypassing regular development cycles.
 
-    ticket_nr: Ticket number assigned to the issue in GitHub.  Once an issue is registered, the owner will assign a ticket.
+        ticket_nr: Ticket number assigned to the issue in GitHub.  Once an issue is registered, the owner will assign a ticket.
 
-    description: GitHub issue title or combination of titles is more than one issue is addressed.
+        description: GitHub issue title or combination of titles is more than one issue is addressed.
 
 
 Releasing
 ~~~~~~~~~
 For the purpose of push and release of code two script files are included.  Use there two files to files to make life a
 bit easier.  The scripts make use of the ``gitit`` module to simplify tasks.
 
 #. ``push.bat`` - Use this script to push branches to GitHub repository.  In principle it does the following:
 
     usage: push message
 
+    e.g. push "Changed the Infinite Improbability Drive"
+
     #. .rst syntax check
     #. git add -A
     #. git commit -m message (with `pre-commit` including `black` and `flake8`)
     #. git push --all
 
 #. ``release.bat`` - Use this script to push a new tag and release to the GitHub repository.  Remember to change the version number in the setup.cfg else the workflow will fail.
 
     usage: release version  The version will match the release and the tag. Only issue a release once a push.bat was successful.  In principle it does the following:
 
+    e.g. relase 1.2.3
+
     #. Commit the changes
-    #. Create and push the release tag
+    #. Create and push the release tag with the correct naming conventions.
     #. Checkout master since it assumes that the branch is now merged with master and will be deleted.
     #. display a list of all the current branches as a reminder to delete the branch on completion.
 
 
 .. General
 
 .. |maintenance_n| image:: https://img.shields.io/badge/Maintenance%20Intended-✖-red.svg?style=flat-square
```

### Comparing `SQLAlchemyExample-0.1.8/pyproject.toml` & `SQLAlchemyExample-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SQLAlchemyExample-0.1.8/setup.cfg` & `SQLAlchemyExample-0.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = SQLAlchemyExample
-version = 0.1.8
+version = 0.1.9
 author = Hendrik du Toit
 author_email = hendrik@brightedge.co.za
 description = Exploring SQLAlchemy
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 classifiers = 
 	Development Status :: 4 - Beta
```

### Comparing `SQLAlchemyExample-0.1.8/src/SQLAlchemyExample.egg-info/PKG-INFO` & `SQLAlchemyExample-0.1.9/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: SQLAlchemyExample
-Version: 0.1.8
-Summary: Exploring SQLAlchemy
-Author: Hendrik du Toit
-Author-email: hendrik@brightedge.co.za
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development
-Classifier: Topic :: Database
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 ====================
 Exploring SQLAlchemy
 ====================
 
 +-------------------+---------------------------------------------------------------------------------------------+
 | **General**       | |maintenance_y| |semver| |license|                                                          |
 +-------------------+---------------------------------------------------------------------------------------------+
@@ -88,40 +70,49 @@
 #. File names
     #. Not knowing what's to come and what will be added, it is difficult to determine a naming convention for source, test and other file names.  The owner will therefore be a "benevolent dictator" to rename and change names.
     #. Link the file name of the source code and the test so that it is easily linked.
 #. Branch names
     "enhancement" | "bug" | "hotfix"/< ticket_nr>_<description>
 
     where
+        enhancement - Planned improvement or addition to functionality; non-urgent.
+
+        bug - An error or defect causing incorrect or unexpected behavior; typically fixed in regular development cycles.
+
+        hotfix - An urgent, critical fix applied directly to the live environment, often bypassing regular development cycles.
 
-    ticket_nr: Ticket number assigned to the issue in GitHub.  Once an issue is registered, the owner will assign a ticket.
+        ticket_nr: Ticket number assigned to the issue in GitHub.  Once an issue is registered, the owner will assign a ticket.
 
-    description: GitHub issue title or combination of titles is more than one issue is addressed.
+        description: GitHub issue title or combination of titles is more than one issue is addressed.
 
 
 Releasing
 ~~~~~~~~~
 For the purpose of push and release of code two script files are included.  Use there two files to files to make life a
 bit easier.  The scripts make use of the ``gitit`` module to simplify tasks.
 
 #. ``push.bat`` - Use this script to push branches to GitHub repository.  In principle it does the following:
 
     usage: push message
 
+    e.g. push "Changed the Infinite Improbability Drive"
+
     #. .rst syntax check
     #. git add -A
     #. git commit -m message (with `pre-commit` including `black` and `flake8`)
     #. git push --all
 
 #. ``release.bat`` - Use this script to push a new tag and release to the GitHub repository.  Remember to change the version number in the setup.cfg else the workflow will fail.
 
     usage: release version  The version will match the release and the tag. Only issue a release once a push.bat was successful.  In principle it does the following:
 
+    e.g. relase 1.2.3
+
     #. Commit the changes
-    #. Create and push the release tag
+    #. Create and push the release tag with the correct naming conventions.
     #. Checkout master since it assumes that the branch is now merged with master and will be deleted.
     #. display a list of all the current branches as a reminder to delete the branch on completion.
 
 
 .. General
 
 .. |maintenance_n| image:: https://img.shields.io/badge/Maintenance%20Intended-✖-red.svg?style=flat-square
```

### Comparing `SQLAlchemyExample-0.1.8/tests/test_otm.py` & `SQLAlchemyExample-0.1.9/tests/test_otm.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemyExample-0.1.8/tests/test_otm_sti.py` & `SQLAlchemyExample-0.1.9/tests/test_otm_sti.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemyExample-0.1.8/tests/test_simple.py` & `SQLAlchemyExample-0.1.9/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemyExample-0.1.8/tests/test_sti.py` & `SQLAlchemyExample-0.1.9/tests/test_sti.py`

 * *Files identical despite different names*

