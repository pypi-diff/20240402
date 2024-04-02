# Comparing `tmp/thors-project-123-0.1.4.tar.gz` & `tmp/thors-project-123-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thors-project-123-0.1.4.tar", last modified: Tue Apr  2 13:01:31 2024, max compression
+gzip compressed data, was "thors-project-123-0.1.5.tar", last modified: Tue Apr  2 13:13:28 2024, max compression
```

## Comparing `thors-project-123-0.1.4.tar` & `thors-project-123-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:01:31.265575 thors-project-123-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-04-02 13:01:15.000000 thors-project-123-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14588 2024-04-02 13:01:31.265575 thors-project-123-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-02 13:01:15.000000 thors-project-123-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-02 13:01:15.000000 thors-project-123-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 13:01:31.265575 thors-project-123-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:01:31.261575 thors-project-123-0.1.4/thors_project_123/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-02 13:01:15.000000 thors-project-123-0.1.4/thors_project_123/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:01:15.000000 thors-project-123-0.1.4/thors_project_123/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-02 13:01:15.000000 thors-project-123-0.1.4/thors_project_123/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:01:31.261575 thors-project-123-0.1.4/thors_project_123.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14588 2024-04-02 13:01:31.000000 thors-project-123-0.1.4/thors_project_123.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-02 13:01:31.000000 thors-project-123-0.1.4/thors_project_123.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:01:31.000000 thors-project-123-0.1.4/thors_project_123.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-02 13:01:31.000000 thors-project-123-0.1.4/thors_project_123.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 13:01:31.000000 thors-project-123-0.1.4/thors_project_123.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:13:28.916771 thors-project-123-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-04-02 13:13:14.000000 thors-project-123-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14588 2024-04-02 13:13:28.916771 thors-project-123-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-02 13:13:14.000000 thors-project-123-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-02 13:13:14.000000 thors-project-123-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 13:13:28.916771 thors-project-123-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:13:28.912770 thors-project-123-0.1.5/thors_project_123/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-02 13:13:14.000000 thors-project-123-0.1.5/thors_project_123/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:13:14.000000 thors-project-123-0.1.5/thors_project_123/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-02 13:13:14.000000 thors-project-123-0.1.5/thors_project_123/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:13:28.912770 thors-project-123-0.1.5/thors_project_123.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14588 2024-04-02 13:13:28.000000 thors-project-123-0.1.5/thors_project_123.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-02 13:13:28.000000 thors-project-123-0.1.5/thors_project_123.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:13:28.000000 thors-project-123-0.1.5/thors_project_123.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-02 13:13:28.000000 thors-project-123-0.1.5/thors_project_123.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 13:13:28.000000 thors-project-123-0.1.5/thors_project_123.egg-info/top_level.txt
```

### Comparing `thors-project-123-0.1.4/LICENSE` & `thors-project-123-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `thors-project-123-0.1.4/PKG-INFO` & `thors-project-123-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thors-project-123
-Version: 0.1.4
+Version: 0.1.5
 Author-email: Allen Institute for Artificial Intelligence <contact@allenai.org>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `thors-project-123-0.1.4/pyproject.toml` & `thors-project-123-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thors-project-123-0.1.4/thors_project_123.egg-info/PKG-INFO` & `thors-project-123-0.1.5/thors_project_123.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thors-project-123
-Version: 0.1.4
+Version: 0.1.5
 Author-email: Allen Institute for Artificial Intelligence <contact@allenai.org>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

