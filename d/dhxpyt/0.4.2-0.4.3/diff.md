# Comparing `tmp/dhxpyt-0.4.2.tar.gz` & `tmp/dhxpyt-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhxpyt-0.4.2.tar", last modified: Tue Apr  2 01:33:21 2024, max compression
+gzip compressed data, was "dhxpyt-0.4.3.tar", last modified: Tue Apr  2 14:14:25 2024, max compression
```

## Comparing `dhxpyt-0.4.2.tar` & `dhxpyt-0.4.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:33:21.795452 dhxpyt-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-02 01:33:13.000000 dhxpyt-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-02 01:33:21.791452 dhxpyt-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 01:33:13.000000 dhxpyt-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:33:21.791452 dhxpyt-0.4.2/dhxpyt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 01:33:13.000000 dhxpyt-0.4.2/dhxpyt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-02 01:33:13.000000 dhxpyt-0.4.2/dhxpyt/accordion.py
--rw-r--r--   0 runner    (1001) docker     (127)    97035 2024-04-02 01:33:13.000000 dhxpyt-0.4.2/dhxpyt/form.py
--rw-r--r--   0 runner    (1001) docker     (127)    35424 2024-04-02 01:33:13.000000 dhxpyt-0.4.2/dhxpyt/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)    15948 2024-04-02 01:33:13.000000 dhxpyt-0.4.2/dhxpyt/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-04-02 01:33:13.000000 dhxpyt-0.4.2/dhxpyt/sidebar.py
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-04-02 01:33:13.000000 dhxpyt-0.4.2/dhxpyt/toolbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     8562 2024-04-02 01:33:13.000000 dhxpyt-0.4.2/dhxpyt/window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:33:21.791452 dhxpyt-0.4.2/dhxpyt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-02 01:33:21.000000 dhxpyt-0.4.2/dhxpyt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-02 01:33:21.000000 dhxpyt-0.4.2/dhxpyt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 01:33:21.000000 dhxpyt-0.4.2/dhxpyt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-02 01:33:21.000000 dhxpyt-0.4.2/dhxpyt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-02 01:33:21.000000 dhxpyt-0.4.2/dhxpyt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 01:33:21.795452 dhxpyt-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-02 01:33:13.000000 dhxpyt-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:14:25.768025 dhxpyt-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 14:14:13.000000 dhxpyt-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-02 14:14:25.768025 dhxpyt-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 14:14:13.000000 dhxpyt-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:14:25.768025 dhxpyt-0.4.3/dhxpyt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:14:13.000000 dhxpyt-0.4.3/dhxpyt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-02 14:14:13.000000 dhxpyt-0.4.3/dhxpyt/accordion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    97035 2024-04-02 14:14:13.000000 dhxpyt-0.4.3/dhxpyt/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35424 2024-04-02 14:14:13.000000 dhxpyt-0.4.3/dhxpyt/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15948 2024-04-02 14:14:13.000000 dhxpyt-0.4.3/dhxpyt/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-04-02 14:14:13.000000 dhxpyt-0.4.3/dhxpyt/sidebar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-04-02 14:14:13.000000 dhxpyt-0.4.3/dhxpyt/toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8562 2024-04-02 14:14:13.000000 dhxpyt-0.4.3/dhxpyt/window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:14:25.768025 dhxpyt-0.4.3/dhxpyt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-02 14:14:25.000000 dhxpyt-0.4.3/dhxpyt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-02 14:14:25.000000 dhxpyt-0.4.3/dhxpyt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 14:14:25.000000 dhxpyt-0.4.3/dhxpyt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-02 14:14:25.000000 dhxpyt-0.4.3/dhxpyt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-02 14:14:25.000000 dhxpyt-0.4.3/dhxpyt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 14:14:25.768025 dhxpyt-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-02 14:14:13.000000 dhxpyt-0.4.3/setup.py
```

### Comparing `dhxpyt-0.4.2/dhxpyt/accordion.py` & `dhxpyt-0.4.3/dhxpyt/accordion.py`

 * *Files identical despite different names*

### Comparing `dhxpyt-0.4.2/dhxpyt/form.py` & `dhxpyt-0.4.3/dhxpyt/form.py`

 * *Files identical despite different names*

### Comparing `dhxpyt-0.4.2/dhxpyt/grid.py` & `dhxpyt-0.4.3/dhxpyt/grid.py`

 * *Files identical despite different names*

### Comparing `dhxpyt-0.4.2/dhxpyt/layout.py` & `dhxpyt-0.4.3/dhxpyt/layout.py`

 * *Files identical despite different names*

### Comparing `dhxpyt-0.4.2/dhxpyt/sidebar.py` & `dhxpyt-0.4.3/dhxpyt/sidebar.py`

 * *Files identical despite different names*

### Comparing `dhxpyt-0.4.2/dhxpyt/toolbar.py` & `dhxpyt-0.4.3/dhxpyt/toolbar.py`

 * *Files identical despite different names*

### Comparing `dhxpyt-0.4.2/dhxpyt/window.py` & `dhxpyt-0.4.3/dhxpyt/window.py`

 * *Files identical despite different names*

### Comparing `dhxpyt-0.4.2/setup.py` & `dhxpyt-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     install_requires = reqs.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='dhxpyt',
-    version='0.4.2',
+    version='0.4.3',
     description=(
         'DHTMLX widgetset'
     ),
     url="https://github.com/pytincture/dhx_pytincture_widgetset",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages = find_packages(),
```

