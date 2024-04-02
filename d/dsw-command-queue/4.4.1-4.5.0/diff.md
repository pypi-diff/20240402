# Comparing `tmp/dsw-command-queue-4.4.1.tar.gz` & `tmp/dsw-command-queue-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsw-command-queue-4.4.1.tar", last modified: Tue Mar 19 11:37:06 2024, max compression
+gzip compressed data, was "dsw-command-queue-4.5.0.tar", last modified: Tue Apr  2 10:28:57 2024, max compression
```

## Comparing `dsw-command-queue-4.4.1.tar` & `dsw-command-queue-4.5.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:37:06.730807 dsw-command-queue-4.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-03-19 11:37:02.000000 dsw-command-queue-4.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-03-19 11:37:06.730807 dsw-command-queue-4.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-03-19 11:37:02.000000 dsw-command-queue-4.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:37:06.726807 dsw-command-queue-4.4.1/dsw/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:37:06.730807 dsw-command-queue-4.4.1/dsw/command_queue/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-19 11:37:02.000000 dsw-command-queue-4.4.1/dsw/command_queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-19 11:37:06.000000 dsw-command-queue-4.4.1/dsw/command_queue/build_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-03-19 11:37:02.000000 dsw-command-queue-4.4.1/dsw/command_queue/command_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-03-19 11:37:02.000000 dsw-command-queue-4.4.1/dsw/command_queue/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:37:06.730807 dsw-command-queue-4.4.1/dsw_command_queue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-03-19 11:37:06.000000 dsw-command-queue-4.4.1/dsw_command_queue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-19 11:37:06.000000 dsw-command-queue-4.4.1/dsw_command_queue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 11:37:06.000000 dsw-command-queue-4.4.1/dsw_command_queue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 11:37:06.000000 dsw-command-queue-4.4.1/dsw_command_queue.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-19 11:37:06.000000 dsw-command-queue-4.4.1/dsw_command_queue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-19 11:37:06.000000 dsw-command-queue-4.4.1/dsw_command_queue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-03-19 11:37:02.000000 dsw-command-queue-4.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 11:37:06.730807 dsw-command-queue-4.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 11:37:02.000000 dsw-command-queue-4.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:28:57.871791 dsw-command-queue-4.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-04-02 10:28:53.000000 dsw-command-queue-4.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-02 10:28:57.871791 dsw-command-queue-4.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-02 10:28:53.000000 dsw-command-queue-4.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:28:57.867790 dsw-command-queue-4.5.0/dsw/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:28:57.867790 dsw-command-queue-4.5.0/dsw/command_queue/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-02 10:28:53.000000 dsw-command-queue-4.5.0/dsw/command_queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-02 10:28:57.000000 dsw-command-queue-4.5.0/dsw/command_queue/build_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-04-02 10:28:53.000000 dsw-command-queue-4.5.0/dsw/command_queue/command_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-02 10:28:53.000000 dsw-command-queue-4.5.0/dsw/command_queue/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:28:57.871791 dsw-command-queue-4.5.0/dsw_command_queue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-02 10:28:57.000000 dsw-command-queue-4.5.0/dsw_command_queue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-02 10:28:57.000000 dsw-command-queue-4.5.0/dsw_command_queue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 10:28:57.000000 dsw-command-queue-4.5.0/dsw_command_queue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 10:28:57.000000 dsw-command-queue-4.5.0/dsw_command_queue.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-02 10:28:57.000000 dsw-command-queue-4.5.0/dsw_command_queue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-02 10:28:57.000000 dsw-command-queue-4.5.0/dsw_command_queue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-02 10:28:53.000000 dsw-command-queue-4.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 10:28:57.871791 dsw-command-queue-4.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 10:28:53.000000 dsw-command-queue-4.5.0/setup.py
```

### Comparing `dsw-command-queue-4.4.1/LICENSE` & `dsw-command-queue-4.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dsw-command-queue-4.4.1/PKG-INFO` & `dsw-command-queue-4.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-command-queue
-Version: 4.4.1
+Version: 4.5.0
 Summary: Library for working with command queue and persistent commands
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,subscriber,publisher,database,queue,processing
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
 Requires-Python: <4,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: dsw-database==4.4.1
+Requires-Dist: dsw-database==4.5.0
 
 # Data Stewardship Wizard: Command Queue
 
 [![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/ds-wizard/engine-tools)](https://github.com/ds-wizard/engine-tools/releases)
 [![PyPI](https://img.shields.io/pypi/v/dsw-command-queue)](https://pypi.org/project/dsw-command-queue/)
 [![LICENSE](https://img.shields.io/github/license/ds-wizard/engine-tools)](LICENSE)
 [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/4975/badge)](https://bestpractices.coreinfrastructure.org/projects/4975)
```

### Comparing `dsw-command-queue-4.4.1/README.md` & `dsw-command-queue-4.5.0/README.md`

 * *Files identical despite different names*

### Comparing `dsw-command-queue-4.4.1/dsw/command_queue/command_queue.py` & `dsw-command-queue-4.5.0/dsw/command_queue/command_queue.py`

 * *Files identical despite different names*

### Comparing `dsw-command-queue-4.4.1/dsw/command_queue/query.py` & `dsw-command-queue-4.5.0/dsw/command_queue/query.py`

 * *Files identical despite different names*

### Comparing `dsw-command-queue-4.4.1/dsw_command_queue.egg-info/PKG-INFO` & `dsw-command-queue-4.5.0/dsw_command_queue.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-command-queue
-Version: 4.4.1
+Version: 4.5.0
 Summary: Library for working with command queue and persistent commands
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,subscriber,publisher,database,queue,processing
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
 Requires-Python: <4,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: dsw-database==4.4.1
+Requires-Dist: dsw-database==4.5.0
 
 # Data Stewardship Wizard: Command Queue
 
 [![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/ds-wizard/engine-tools)](https://github.com/ds-wizard/engine-tools/releases)
 [![PyPI](https://img.shields.io/pypi/v/dsw-command-queue)](https://pypi.org/project/dsw-command-queue/)
 [![LICENSE](https://img.shields.io/github/license/ds-wizard/engine-tools)](LICENSE)
 [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/4975/badge)](https://bestpractices.coreinfrastructure.org/projects/4975)
```

### Comparing `dsw-command-queue-4.4.1/pyproject.toml` & `dsw-command-queue-4.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'dsw-command-queue'
-version = "4.4.1"
+version = "4.5.0"
 description = 'Library for working with command queue and persistent commands'
 readme = 'README.md'
 keywords = ['dsw', 'subscriber', 'publisher', 'database', 'queue', 'processing']
 license = { text = 'Apache License 2.0' }
 authors = [
     { name = 'Marek Suchánek', email = 'marek.suchanek@ds-wizard.org' }
 ]
@@ -21,15 +21,15 @@
     'Topic :: Database',
     'Topic :: Text Processing',
     'Topic :: Utilities',
 ]
 requires-python = '>=3.10, <4'
 dependencies = [
     # DSW
-    "dsw-database==4.4.1",
+    "dsw-database==4.5.0",
 ]
 
 [project.urls]
 Homepage = 'https://ds-wizard.org'
 Repository = 'https://github.com/ds-wizard/engine-tools'
 Documentation = 'https://guide.ds-wizard.org'
```

