# Comparing `tmp/particle_tracking_manager-0.7.1.tar.gz` & `tmp/particle_tracking_manager-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "particle_tracking_manager-0.7.1.tar", last modified: Wed Feb 21 22:01:42 2024, max compression
+gzip compressed data, was "particle_tracking_manager-0.8.0.tar", last modified: Tue Apr  2 18:01:25 2024, max compression
```

## Comparing `particle_tracking_manager-0.7.1.tar` & `particle_tracking_manager-0.8.0.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:01:42.567842 particle_tracking_manager-0.7.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:01:42.559842 particle_tracking_manager-0.7.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:01:42.563842 particle_tracking_manager-0.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-02-21 22:01:42.567842 particle_tracking_manager-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:01:42.563842 particle_tracking_manager-0.7.1/ci/
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/ci/environment-py3.10.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/ci/environment-py3.11.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/ci/environment-py3.9.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:01:42.563842 particle_tracking_manager-0.7.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     9569 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/docs/configuration.md
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/docs/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/docs/more_examples.md
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/docs/quick_start.md
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/docs/whats_new.md
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:01:42.563842 particle_tracking_manager-0.7.1/particle_tracking_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/particle_tracking_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/particle_tracking_manager/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:01:42.563842 particle_tracking_manager-0.7.1/particle_tracking_manager/models/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/particle_tracking_manager/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:01:42.567842 particle_tracking_manager-0.7.1/particle_tracking_manager/models/opendrift/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/particle_tracking_manager/models/opendrift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/particle_tracking_manager/models/opendrift/config.json
--rw-r--r--   0 runner    (1001) docker     (127)    43749 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/particle_tracking_manager/models/opendrift/opendrift.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/particle_tracking_manager/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    24255 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/particle_tracking_manager/the_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/particle_tracking_manager/the_manager_config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:01:42.567842 particle_tracking_manager-0.7.1/particle_tracking_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-02-21 22:01:42.000000 particle_tracking_manager-0.7.1/particle_tracking_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-02-21 22:01:42.000000 particle_tracking_manager-0.7.1/particle_tracking_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 22:01:42.000000 particle_tracking_manager-0.7.1/particle_tracking_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-21 22:01:42.000000 particle_tracking_manager-0.7.1/particle_tracking_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-21 22:01:42.000000 particle_tracking_manager-0.7.1/particle_tracking_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-21 22:01:42.000000 particle_tracking_manager-0.7.1/particle_tracking_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-02-21 22:01:42.567842 particle_tracking_manager-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:01:42.567842 particle_tracking_manager-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10606 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    13513 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/tests/test_opendrift.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/tests/test_realistic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-02-21 22:01:37.000000 particle_tracking_manager-0.7.1/tests/test_seeding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:01:25.341570 particle_tracking_manager-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:01:25.337570 particle_tracking_manager-0.8.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:01:25.337570 particle_tracking_manager-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-02 18:01:25.341570 particle_tracking_manager-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:01:25.337570 particle_tracking_manager-0.8.0/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/ci/environment-py3.10.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/ci/environment-py3.11.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/ci/environment-py3.9.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:01:25.337570 particle_tracking_manager-0.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9569 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/docs/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/docs/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/docs/more_examples.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/docs/quick_start.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/docs/whats_new.md
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:01:25.341570 particle_tracking_manager-0.8.0/particle_tracking_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/particle_tracking_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-02 18:01:25.000000 particle_tracking_manager-0.8.0/particle_tracking_manager/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/particle_tracking_manager/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:01:25.341570 particle_tracking_manager-0.8.0/particle_tracking_manager/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/particle_tracking_manager/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:01:25.341570 particle_tracking_manager-0.8.0/particle_tracking_manager/models/opendrift/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/particle_tracking_manager/models/opendrift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/particle_tracking_manager/models/opendrift/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)    46883 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/particle_tracking_manager/models/opendrift/opendrift.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/particle_tracking_manager/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24426 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/particle_tracking_manager/the_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/particle_tracking_manager/the_manager_config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:01:25.341570 particle_tracking_manager-0.8.0/particle_tracking_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-02 18:01:25.000000 particle_tracking_manager-0.8.0/particle_tracking_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-02 18:01:25.000000 particle_tracking_manager-0.8.0/particle_tracking_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 18:01:25.000000 particle_tracking_manager-0.8.0/particle_tracking_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-02 18:01:25.000000 particle_tracking_manager-0.8.0/particle_tracking_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 18:01:25.000000 particle_tracking_manager-0.8.0/particle_tracking_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-02 18:01:25.000000 particle_tracking_manager-0.8.0/particle_tracking_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-02 18:01:25.341570 particle_tracking_manager-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:01:25.341570 particle_tracking_manager-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10701 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13513 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/tests/test_opendrift.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/tests/test_realistic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/tests/test_seeding.py
```

### Comparing `particle_tracking_manager-0.7.1/.github/workflows/release.yaml` & `particle_tracking_manager-0.8.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.7.1/.github/workflows/test.yaml` & `particle_tracking_manager-0.8.0/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.7.1/.gitignore` & `particle_tracking_manager-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.7.1/.pre-commit-config.yaml` & `particle_tracking_manager-0.8.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.7.1/LICENSE.txt` & `particle_tracking_manager-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.7.1/PKG-INFO` & `particle_tracking_manager-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: particle_tracking_manager
-Version: 0.7.1
+Version: 0.8.0
 Summary: Manager for particle tracking simulations.
 Home-page: https://github.com/axiom-data-science/particle-tracking-manager
 Author: axiom-data-science
 Author-email: kristen@axds.co
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `particle_tracking_manager-0.7.1/README.md` & `particle_tracking_manager-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.7.1/ci/environment-py3.10.yml` & `particle_tracking_manager-0.8.0/ci/environment-py3.10.yml`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.7.1/ci/environment-py3.11.yml` & `particle_tracking_manager-0.8.0/ci/environment-py3.11.yml`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.7.1/ci/environment-py3.9.yml` & `particle_tracking_manager-0.8.0/ci/environment-py3.9.yml`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.7.1/docs/Makefile` & `particle_tracking_manager-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.7.1/docs/conf.py` & `particle_tracking_manager-0.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.7.1/docs/configuration.md` & `particle_tracking_manager-0.8.0/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.7.1/docs/environment.yml` & `particle_tracking_manager-0.8.0/docs/environment.yml`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.7.1/docs/index.rst` & `particle_tracking_manager-0.8.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.7.1/docs/more_examples.md` & `particle_tracking_manager-0.8.0/docs/more_examples.md`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.7.1/docs/quick_start.md` & `particle_tracking_manager-0.8.0/docs/quick_start.md`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.7.1/docs/whats_new.md` & `particle_tracking_manager-0.8.0/docs/whats_new.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,22 @@
 # What's New
 
+## v0.8.0 (April 2, 2024)
+
+* `time_step_output` behavior has changed — 1 hour by default
+* `time_step` is now 5 min by default
+* added `Dcrit` parameter for accurately finding where drifters are stranded in tidal flats
+* `vertical_mixing` is True by default now
+* added seafloor_action option
+* fixed some Leeway/3D handling and log messaging
+* export_variables are specific to drift_model as needed
+* do not drop zeta anymore since used in opendrift
+* output_file is now an option
+
+
 ## v0.7.1 (February 21, 2024)
 
 * Small fix to some attributes to be less verbose
 * Fix setup.cfg to have correct config path since name changed
 
 
 ## v0.7.0 (February 21, 2024)
```

### Comparing `particle_tracking_manager-0.7.1/particle_tracking_manager/cli.py` & `particle_tracking_manager-0.8.0/particle_tracking_manager/cli.py`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.7.1/particle_tracking_manager/models/opendrift/config.json` & `particle_tracking_manager-0.8.0/particle_tracking_manager/models/opendrift/config.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9470009157509158%*

 * *Differences: {"'Dcrit'": "OrderedDict([('default', 0.1), ('od_mapping', 'general:seafloor_action_dcrit'), "*

 * *            "('ptm_level', 3)])",*

 * * "'export_variables'": "{'default': {insert: [(1, 'origin_marker')]}}",*

 * * "'radius'": "{'default': 1000.0}",*

 * * "'seafloor_action'": "OrderedDict([('default', 'previous'), ('od_mapping', "*

 * *                      "'general:seafloor_action'), ('ptm_level', 1)])"}*

```diff
@@ -1,8 +1,13 @@
 {
+    "Dcrit": {
+        "default": 0.1,
+        "od_mapping": "general:seafloor_action_dcrit",
+        "ptm_level": 3
+    },
     "biodegradation": {
         "default": true,
         "od_mapping": "processes:biodegradation",
         "ptm_level": 1
     },
     "coastline_action": {
         "default": "previous",
@@ -69,15 +74,16 @@
     "evaporation": {
         "default": true,
         "od_mapping": "processes:evaporation",
         "ptm_level": 1
     },
     "export_variables": {
         "default": [
-            "z"
+            "z",
+            "origin_marker"
         ],
         "description": "List of variables to export. Options available with `m.all_export_variables` for a given `drift_model`. ['lon', 'lat', 'ID', 'status'] will always be exported.",
         "ptm_level": 2,
         "type": "list"
     },
     "hatched": {
         "default": 0,
@@ -135,28 +141,33 @@
     },
     "oil_type": {
         "default": "GENERIC MEDIUM CRUDE",
         "od_mapping": "seed:oil_type",
         "ptm_level": 1
     },
     "radius": {
-        "default": 0.0,
+        "default": 1000.0,
         "description": "Radius around each lon-lat pair, within which particles will be randomly seeded. This is used by function `seed_elements`.",
         "max": 1000000,
         "min": 0.0,
         "ptm_level": 1,
         "type": "float",
         "units": "m"
     },
     "radius_type": {
         "default": "gaussian",
         "description": "If 'gaussian' (default), the radius is the standard deviation in x-y-directions. If 'uniform', elements are spread evenly and always inside a circle with the given radius. This is used by function `seed_elements`.",
         "ptm_level": 2,
         "type": "enum - gaussian - uniform"
     },
+    "seafloor_action": {
+        "default": "previous",
+        "od_mapping": "general:seafloor_action",
+        "ptm_level": 1
+    },
     "stage_fraction": {
         "default": 0.0,
         "od_mapping": "seed:stage_fraction",
         "ptm_level": 2
     },
     "stokes_drift": {
         "default": true,
```

### Comparing `particle_tracking_manager-0.7.1/particle_tracking_manager/models/opendrift/opendrift.py` & `particle_tracking_manager-0.8.0/particle_tracking_manager/models/opendrift/opendrift.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,17 @@
 
         The latter two configurations are not additionally set in OpenDriftModel since they are already the default once stokes_drift is True.
     mixed_layer_depth : float
         Fallback value for ocean_mixed_layer_thickness if not available from any reader. This is used in the calculation of vertical diffusivity.
     coastline_action : str, optional
         Action to perform if a drifter hits the coastline, by default "previous". Options
         are 'stranding', 'previous'.
+    seafloor_action : str, optional
+        Action to perform if a drifter hits the seafloor, by default "deactivate". Options
+        are 'deactivate', 'previous', 'lift_to_seafloor'.
     max_speed : int
         Typical maximum speed of elements, used to estimate reader buffer size.
     wind_drift_factor : float
         Elements at surface are moved with this fraction of the wind vector, in addition to currents and Stokes drift.
     wind_drift_depth : float
         The direct wind drift (windage) is linearly decreasing from the surface value (wind_drift_factor) until 0 at this depth.
     vertical_mixing_timestep : float
@@ -169,14 +172,15 @@
         current_uncertainty: float = config_model["current_uncertainty"]["default"],
         wind_uncertainty: float = config_model["wind_uncertainty"]["default"],
         use_auto_landmask: bool = config_model["use_auto_landmask"]["default"],
         diffusivitymodel: str = config_model["diffusivitymodel"]["default"],
         stokes_drift: bool = config_model["stokes_drift"]["default"],
         mixed_layer_depth: float = config_model["mixed_layer_depth"]["default"],
         coastline_action: str = config_model["coastline_action"]["default"],
+        seafloor_action: str = config_model["seafloor_action"]["default"],
         max_speed: int = config_model["max_speed"]["default"],
         wind_drift_factor: float = config_model["wind_drift_factor"]["default"],
         wind_drift_depth: float = config_model["wind_drift_depth"]["default"],
         vertical_mixing_timestep: float = config_model["vertical_mixing_timestep"][
             "default"
         ],
         object_type: str = config_model["object_type"]["default"],
@@ -315,33 +319,41 @@
             # and name != "config_model"
             # and name != "config_ptm"
             and name in self.config_model.keys()
         ):
             self.config_model[name]["value"] = value
         self._update_config()
 
+        if name == "ocean_model":
+            if value == "NWGOA":
+                self.Dcrit = 0.5
+            elif "CIOFS" in value:
+                self.Dcrit = 0.3
+            else:
+                self.Dcrit = 0.1
+            self.logger.info(f"For ocean_model {value}, setting Dcrit to {self.Dcrit}.")
+
         if name in ["ocean_model", "horizontal_diffusivity"]:
 
             # just set the value and move on if purposely setting a non-None value
             # of horizontal_diffusivity; specifying this for clarity (already set
             # value above).
             if name == "horizontal_diffusivity" and value is not None:
                 self.logger.info(
                     f"Setting horizontal_diffusivity to user-selected value {value}."
                 )
 
             # in all other cases that ocean_model is a known model, want to use the
             # grid-dependent value
             elif self.ocean_model in _KNOWN_MODELS:
-                print(name, value)
-                self.logger.info(
-                    "Setting horizontal_diffusivity parameter to one tuned to reader model"
-                )
 
                 hdiff = self.calc_known_horizontal_diffusivity()
+                self.logger.info(
+                    f"Setting horizontal_diffusivity parameter to one tuned to reader model of value {hdiff}."
+                )
                 # when editing the __dict__ directly have to also update config_model
                 self.__dict__["horizontal_diffusivity"] = hdiff
                 self.config_model["horizontal_diffusivity"]["value"] = hdiff
 
             # if user not using a known ocean_model, change horizontal_diffusivity from None to 0
             # so it has a value. User can subsequently overwrite it too.
             elif (
@@ -377,17 +389,29 @@
                 is not None
             ):
                 self.logger.info("Un-truncating model output below 0.5 m.")
                 self.o.set_config("drift:truncate_ocean_model_below_m", None)
 
         # Leeway doesn't have this option available
         if name == "do3D" and not value and self.drift_model != "Leeway":
+            self.logger.info("do3D is False so disabling vertical motion.")
             self.o.disable_vertical_motion()
-        elif name == "do3D" and value:
+        elif name == "do3D" and not value and self.drift_model == "Leeway":
+            self.logger.info(
+                "do3D is False but drift_model is Leeway so doing nothing."
+            )
+
+        if name == "do3D" and value and self.drift_model != "Leeway":
+            self.logger.info("do3D is True so turning on vertical advection.")
             self.o.set_config("drift:vertical_advection", True)
+        elif name == "do3D" and value and self.drift_model == "Leeway":
+            self.logger.info(
+                "do3D is True but drift_model is Leeway so " "changing do3D to False."
+            )
+            self.do3D = False
 
         # Make sure vertical_mixing_timestep equals default value if vertical_mixing False
         if name in ["vertical_mixing", "vertical_mixing_timestep"]:
             vmtdef = self.config_model["vertical_mixing_timestep"]["default"]
             if (
                 not self.vertical_mixing
                 and self.vertical_mixing_timestep != vmtdef
@@ -460,14 +484,33 @@
             if self.drift_model == "Leeway" and self.stokes_drift:
                 self.logger.info(
                     "stokes_drift cannot be used with Leeway model, so changing to False."
                 )
                 self.__dict__["stokes_drift"] = False
                 self.config_model["stokes_drift"]["value"] = False
 
+        # Add export variables for certain drift_model values
+        # drift_model is always set initially only
+        if name == "export_variables" and self.drift_model == "OpenOil":
+            oil_vars = [
+                "mass_oil",
+                "density",
+                "mass_evaporated",
+                "mass_dispersed",
+                "mass_biodegraded",
+                "viscosity",
+                "water_fraction",
+            ]
+            self.__dict__["export_variables"] += oil_vars
+            self.config_model["export_variables"]["value"] += oil_vars
+        elif name == "export_variables" and self.drift_model == "Leeway":
+            vars = ["object_type"]
+            self.__dict__["export_variables"] += vars
+            self.config_model["export_variables"]["value"] += vars
+
         self._update_config()
 
     def run_add_reader(
         self,
         ds=None,
         name=None,
         oceanmodel_lon0_360=False,
@@ -613,22 +656,21 @@
                 )
 
             elif "CIOFS" in self.ocean_model:
                 oceanmodel_lon0_360 = False
 
                 drop_vars += [
                     "wetdry_mask_psi",
-                    "zeta",
                 ]
                 if self.ocean_model == "CIOFS":
 
                     loc_local = "/mnt/vault/ciofs/HINDCAST/ciofs_kerchunk.parq"
                     loc_remote = "http://xpublish-ciofs.srv.axds.co/datasets/ciofs_hindcast/zarr/"
 
-                elif self.ocean_model.upper() == "CIOFSOP":
+                elif self.ocean_model == "CIOFSOP":
 
                     standard_name_mapping.update(
                         {
                             "u_eastward": "x_sea_water_velocity",
                             "v_northward": "y_sea_water_velocity",
                         }
                     )
@@ -670,24 +712,30 @@
                         ds = xr.open_zarr(
                             loc_remote, chunks={}, drop_variables=drop_vars
                         )
 
             # For NWGOA, need to calculate wetdry mask from a variable
             if self.ocean_model == "NWGOA" and not self.use_static_masks:
                 ds["wetdry_mask_rho"] = (~ds.zeta.isnull()).astype(int)
-                ds.drop_vars("zeta", inplace=True)
 
             # For CIOFSOP need to rename u/v to have "East" and "North" in the variable names
             # so they aren't rotated in the ROMS reader (the standard names have to be x/y not east/north)
             elif self.ocean_model == "CIOFSOP":
                 ds = ds.rename_vars({"urot": "u_eastward", "vrot": "v_northward"})
                 # grid = xr.open_dataset("/mnt/vault/ciofs/HINDCAST/nos.ciofs.romsgrid.nc")
                 # ds["angle"] = grid["angle"]
 
-            units_date = pd.Timestamp(ds.ocean_time.attrs["units"].split("since ")[1])
+            try:
+                units_date = pd.Timestamp(
+                    ds.ocean_time.attrs["units"].split("since ")[1]
+                )
+            except KeyError:  # for remote
+                units_date = pd.Timestamp(
+                    ds.ocean_time.encoding["units"].split("since ")[0]
+                )
             # use reader start time if not otherwise input
             if self.start_time is None:
                 self.logger.info("setting reader start_time as simulation start_time")
                 # self.start_time = reader.start_time
                 # convert using pandas instead of netCDF4
                 self.start_time = units_date + pd.to_timedelta(
                     ds.ocean_time[0].values, unit="s"
@@ -783,19 +831,26 @@
         # drop non-OpenDrift parameters now so they aren't brought into simulation (they mess up the write step)
         full_config = copy.deepcopy(self._config)  # save
         config_input_to_opendrift = {
             k: full_config[k] for k in self._config_orig.keys()
         }
 
         self.o._config = config_input_to_opendrift  # only OpenDrift config
+
+        output_file = (
+            self.output_file
+            or f"output-results_{datetime.datetime.utcnow():%Y-%m-%dT%H%M:%SZ}.nc"
+        )
+
         self.o.run(
             time_step=timedir * self.time_step,
+            time_step_output=self.time_step_output,
             steps=self.steps,
             export_variables=self.export_variables,
-            outfile=f"output-results_{datetime.datetime.utcnow():%Y-%m-%dT%H%M:%SZ}.nc",
+            outfile=output_file,
         )
 
         self.o._config = full_config  # reinstate config
 
     @property
     def _config(self):
         """Surface the model configuration."""
@@ -898,14 +953,38 @@
         return vars
 
     def export_variables(self):
         """Output list of all actual export variables."""
 
         return self.o.export_variables
 
+    def drift_model_config(self, ptm_level=[1, 2, 3], prefix=""):
+        """Show config for this drift model selection.
+
+        This shows all PTM-controlled parameters for the OpenDrift
+        drift model selected and their current values, at the selected ptm_level
+        of importance.
+
+        Parameters
+        ----------
+        ptm_level : int, list, optional
+            Options are 1, 2, 3, or lists of combinations. Use [1,2,3] for all.
+            Default is 1.
+        prefix : str, optional
+            prefix to search config for, only for OpenDrift parameters (not PTM).
+        """
+
+        return [
+            (key, value_dict["value"])
+            for key, value_dict in self.show_config(
+                substring=":", ptm_level=ptm_level, level=[1, 2, 3], prefix=prefix
+            ).items()
+            if "value" in value_dict
+        ]
+
     def get_configspec(self, prefix, substring, excludestring, level, ptm_level):
         """Copied from OpenDrift, then modified."""
 
         if not isinstance(level, list) and level is not None:
             level = [level]
         if not isinstance(ptm_level, list) and ptm_level is not None:
             ptm_level = [ptm_level]
```

### Comparing `particle_tracking_manager-0.7.1/particle_tracking_manager/plotting.py` & `particle_tracking_manager-0.8.0/particle_tracking_manager/plotting.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Some extra plotting code."""
 
 import opendrift
 
 
-def plot_dest(o):
+def plot_dest(o, filename):
     """This is copied from an opendrift example."""
 
     import cmocean
 
     cmap = cmocean.tools.crop_by_percent(cmocean.cm.amp, 20, which="max", N=None)
 
     od = opendrift.open_xarray(o.outfile_name)
@@ -20,8 +20,10 @@
         background=density,
         clabel="Probability of final location [%]",
         markersize=0.5,
         lalpha=0.02,
         vmin=0,
         vmax=vmax,
         cmap=cmap,
+        fast=True,
+        filename=filename,
     )
```

### Comparing `particle_tracking_manager-0.7.1/particle_tracking_manager/the_manager.py` & `particle_tracking_manager-0.8.0/particle_tracking_manager/the_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,18 +67,18 @@
     number : int
         Number of drifters to simulate. Default is 100.
     start_time : Optional[str,datetime.datetime,pd.Timestamp], optional
         Start time of simulation, by default None
     run_forward : bool, optional
         True to run forward in time, False to run backward, by default True
     time_step : int, optional
-        Time step in seconds, options >0, <86400 (1 day in seconds), by default 3600
-    time_step_output : int, optional
-        How often to output model output, in seconds. Should be a multiple of time_step.
-        By default will take the value of time_step (this change occurs in the model).
+        Time step in seconds, options >0, <86400 (1 day in seconds), by default 300.
+    time_step_output : int, Timedelta, optional
+        How often to output model output. Should be a multiple of time_step.
+        By default 3600.
     steps : int, optional
         Number of time steps to run in simulation. Options >0.
         steps, end_time, or duration must be input by user. By default steps is 3 and
         duration and end_time are None. Only one of steps, end_time, or duration can be
         non-None at initialization time. If one of steps, end_time, or duration is input
         later, it will be used to overwrite the three parameters according to that newest
         parameter.
@@ -125,14 +125,16 @@
         ``surface_only==True``.
     use_static_masks : bool, optional
         Set to True to use static masks ocean_model output when ROMS wetdry masks are available, by default False.
         This is relevant for all of the available known models. If you want to use static masks
         with a user-input ocean_model, you can drop the wetdry_mask_rho etc variables from the
         dataset before inputting to PTM. Setting this to True may save computation time but
         will be less accurate, especially in the tidal flat regions of the model.
+    output_file : Optional[str], optional
+        Name of output file to save, by default None. If None, default is set in the model.
 
     Notes
     -----
     Configuration happens at initialization time for the child model. There is currently
     no separate configuration step.
     """
 
@@ -172,14 +174,15 @@
         # universal inputs
         ocean_model: Optional[str] = config_ptm["ocean_model"]["default"],
         ocean_model_local: Optional[bool] = config_ptm["ocean_model_local"]["default"],
         surface_only: Optional[bool] = config_ptm["surface_only"]["default"],
         do3D: bool = config_ptm["do3D"]["default"],
         vertical_mixing: bool = config_ptm["vertical_mixing"]["default"],
         use_static_masks: bool = config_ptm["use_static_masks"]["default"],
+        output_file: Optional[str] = config_ptm["output_file"]["default"],
         **kw,
     ) -> None:
         """Inputs necessary for any particle tracking."""
 
         # get all named parameters input to ParticleTrackingManager class
         from inspect import signature
 
@@ -324,15 +327,15 @@
             # deal with if input longitudes need to be shifted due to model
             if name == "oceanmodel_lon0_360" and value:
                 if self.ocean_model is not "test" and self.lon is not None:
                     # move longitude to be 0 to 360 for this model
                     # this is not a user-defined option
                     if -180 < self.lon < 0:
                         self.__dict__["lon"] += 360
-                        self.config_ptm["lon"]["value"] = False
+                        self.config_ptm["lon"]["value"] += 360  # this isn't really used
 
             if name == "surface_only" and value:
                 self.logger.info(
                     "Overriding values for do3D, z, and vertical_mixing because surface_only is True (to False, 0, False)."
                 )
                 self.do3D = False
                 self.z = 0
```

### Comparing `particle_tracking_manager-0.7.1/particle_tracking_manager/the_manager_config.json` & `particle_tracking_manager-0.8.0/particle_tracking_manager/the_manager_config.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9458874458874459%*

 * *Differences: {"'output_file'": "OrderedDict([('type', 'str'), ('default', 'None'), ('description', 'Name of "*

 * *                  "file to write output to. If None, default name is used.'), ('ptm_level', 3)])",*

 * * "'time_step'": "{'default': 300, 'ptm_level': 2}",*

 * * "'time_step_output'": "{'default': 3600}",*

 * * "'vertical_mixing'": "{'default': True}"}*

```diff
@@ -74,14 +74,20 @@
     },
     "ocean_model_local": {
         "default": false,
         "description": "Set to True to use local version of known `ocean_model` instead of remote version.",
         "ptm_level": 3,
         "type": "bool"
     },
+    "output_file": {
+        "default": "None",
+        "description": "Name of file to write output to. If None, default name is used.",
+        "ptm_level": 3,
+        "type": "str"
+    },
     "run_forward": {
         "default": true,
         "description": "Run forward in time.",
         "ptm_level": 1,
         "type": "bool"
     },
     "seed_flag": {
@@ -120,27 +126,27 @@
     "surface_only": {
         "default": "None",
         "description": "Set to True to keep drifters at the surface, by default None. If this flag is set to not-None, it overrides do3D to False, vertical_mixing to False, and the z value(s) 0. If True, this flag also turns off reading model output below 0.5m if drift_model is not Leeway to save time.",
         "ptm_level": 1,
         "type": "bool"
     },
     "time_step": {
-        "default": 3600,
+        "default": 300,
         "description": "Interval between particles updates, in seconds or as timedelta.",
         "max": 86400,
         "min": 1,
-        "ptm_level": 1,
+        "ptm_level": 2,
         "type": [
             "float",
             "datetime.timedelta"
         ],
         "units": "seconds"
     },
     "time_step_output": {
-        "default": "None",
+        "default": 3600,
         "description": "Time step at which element properties are stored and eventually written to file.",
         "max": 604800,
         "min": 1,
         "ptm_level": 2,
         "type": [
             "float",
             "datetime.timedelta"
@@ -150,15 +156,15 @@
     "use_static_masks": {
         "default": false,
         "description": "Set to True to use static masks for known models instead of wetdry masks. If False, the masks are change in time.",
         "ptm_level": 2,
         "type": "bool"
     },
     "vertical_mixing": {
-        "default": false,
+        "default": true,
         "od_mapping": "drift:vertical_mixing",
         "ptm_level": 1
     },
     "z": {
         "default": 0,
         "od_mapping": "seed:z",
         "ptm_level": 1
```

### Comparing `particle_tracking_manager-0.7.1/particle_tracking_manager.egg-info/PKG-INFO` & `particle_tracking_manager-0.8.0/particle_tracking_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: particle_tracking_manager
-Version: 0.7.1
+Version: 0.8.0
 Summary: Manager for particle tracking simulations.
 Home-page: https://github.com/axiom-data-science/particle-tracking-manager
 Author: axiom-data-science
 Author-email: kristen@axds.co
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `particle_tracking_manager-0.7.1/particle_tracking_manager.egg-info/SOURCES.txt` & `particle_tracking_manager-0.8.0/particle_tracking_manager.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 docs/configuration.md
 docs/environment.yml
 docs/index.rst
 docs/more_examples.md
 docs/quick_start.md
 docs/whats_new.md
 particle_tracking_manager/__init__.py
+particle_tracking_manager/_version.py
 particle_tracking_manager/cli.py
 particle_tracking_manager/plotting.py
 particle_tracking_manager/the_manager.py
 particle_tracking_manager/the_manager_config.json
 particle_tracking_manager.egg-info/PKG-INFO
 particle_tracking_manager.egg-info/SOURCES.txt
 particle_tracking_manager.egg-info/dependency_links.txt
```

### Comparing `particle_tracking_manager-0.7.1/pyproject.toml` & `particle_tracking_manager-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.7.1/setup.cfg` & `particle_tracking_manager-0.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.7.1/tests/conftest.py` & `particle_tracking_manager-0.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.7.1/tests/test_cli.py` & `particle_tracking_manager-0.8.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.7.1/tests/test_config.py` & `particle_tracking_manager-0.8.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.7.1/tests/test_manager.py` & `particle_tracking_manager-0.8.0/tests/test_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,18 +93,19 @@
     mock_reader_metadata.return_value = datetime(2000, 1, 1)
 
     m = ptm.OpenDriftModel()
     with pytest.raises(AssertionError):
         m.has_added_reader = True
 
 
+@pytest.mark.slow
 def test_parameter_passing():
     """make sure parameters passed into package make it to simulation runtime."""
 
-    ts = 2 * 3600
+    ts = 5
     diffmodel = "windspeed_Sundby1983"
     use_auto_landmask = True
     vertical_mixing = True
     do3D = True
 
     seed_kws = dict(
         lon=4.0,
@@ -219,29 +220,34 @@
             steps=4,
             duration=pd.Timedelta("24h"),
             end_time=pd.Timestamp("1970-01-01T02:00"),
         )
 
 
 def test_changing_end_of_simulation():
-    """change end_time, steps, and duration and make sure others are updated accordingly."""
+    """change end_time, steps, and duration
+
+    and make sure others are updated accordingly.
+    This accounts for the default time_step of 300 seconds.
+
+    """
 
     m = ptm.OpenDriftModel(start_time=pd.Timestamp("2000-1-1"))
     m.start_time = pd.Timestamp("2000-1-2")
     m.end_time = pd.Timestamp("2000-1-3")
-    assert m.steps == 24
+    assert m.steps == 288
     assert m.duration == pd.Timedelta("1 days 00:00:00")
 
     m.steps = 48
-    assert m.end_time == pd.Timestamp("2000-1-4")
-    assert m.duration == pd.Timedelta("2 days 00:00:00")
+    assert m.end_time == pd.Timestamp("2000-01-02 04:00:00")
+    assert m.duration == pd.Timedelta("0 days 04:00:00")
 
     m.duration = pd.Timedelta("2 days 12:00:00")
     assert m.end_time == pd.Timestamp("2000-01-04 12:00:00")
-    assert m.steps == 60
+    assert m.steps == 720
 
 
 class TestTheManager(unittest.TestCase):
     def setUp(self):
         self.m = ptm.OpenDriftModel()
         self.m.reader_metadata = mock.MagicMock(
             side_effect=lambda x: {
```

### Comparing `particle_tracking_manager-0.7.1/tests/test_opendrift.py` & `particle_tracking_manager-0.8.0/tests/test_opendrift.py`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.7.1/tests/test_realistic.py` & `particle_tracking_manager-0.8.0/tests/test_realistic.py`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.7.1/tests/test_seeding.py` & `particle_tracking_manager-0.8.0/tests/test_seeding.py`

 * *Files identical despite different names*

