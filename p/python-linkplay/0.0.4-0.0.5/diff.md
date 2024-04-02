# Comparing `tmp/python_linkplay-0.0.4.tar.gz` & `tmp/python_linkplay-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_linkplay-0.0.4.tar", last modified: Thu Mar 21 10:53:21 2024, max compression
+gzip compressed data, was "python_linkplay-0.0.5.tar", last modified: Tue Apr  2 12:26:12 2024, max compression
```

## Comparing `python_linkplay-0.0.4.tar` & `python_linkplay-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:53:21.446751 python_linkplay-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-21 10:53:17.000000 python_linkplay-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-03-21 10:53:21.446751 python_linkplay-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-03-21 10:53:17.000000 python_linkplay-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-21 10:53:17.000000 python_linkplay-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-21 10:53:21.446751 python_linkplay-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-21 10:53:17.000000 python_linkplay-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:53:21.438751 python_linkplay-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:53:21.442751 python_linkplay-0.0.4/src/linkplay/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-21 10:53:17.000000 python_linkplay-0.0.4/src/linkplay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-03-21 10:53:17.000000 python_linkplay-0.0.4/src/linkplay/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-21 10:53:17.000000 python_linkplay-0.0.4/src/linkplay/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10948 2024-03-21 10:53:17.000000 python_linkplay-0.0.4/src/linkplay/bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-03-21 10:53:17.000000 python_linkplay-0.0.4/src/linkplay/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-03-21 10:53:17.000000 python_linkplay-0.0.4/src/linkplay/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-03-21 10:53:17.000000 python_linkplay-0.0.4/src/linkplay/discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-21 10:53:17.000000 python_linkplay-0.0.4/src/linkplay/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-03-21 10:53:17.000000 python_linkplay-0.0.4/src/linkplay/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:53:21.442751 python_linkplay-0.0.4/src/python_linkplay.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-03-21 10:53:21.000000 python_linkplay-0.0.4/src/python_linkplay.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-21 10:53:21.000000 python_linkplay-0.0.4/src/python_linkplay.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 10:53:21.000000 python_linkplay-0.0.4/src/python_linkplay.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 10:53:21.000000 python_linkplay-0.0.4/src/python_linkplay.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-03-21 10:53:21.000000 python_linkplay-0.0.4/src/python_linkplay.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-21 10:53:21.000000 python_linkplay-0.0.4/src/python_linkplay.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:26:12.514842 python_linkplay-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-02 12:26:08.000000 python_linkplay-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-02 12:26:12.510842 python_linkplay-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-02 12:26:08.000000 python_linkplay-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-02 12:26:08.000000 python_linkplay-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-02 12:26:12.514842 python_linkplay-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-02 12:26:08.000000 python_linkplay-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:26:12.506842 python_linkplay-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:26:12.510842 python_linkplay-0.0.5/src/linkplay/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-02 12:26:08.000000 python_linkplay-0.0.5/src/linkplay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-02 12:26:08.000000 python_linkplay-0.0.5/src/linkplay/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 12:26:08.000000 python_linkplay-0.0.5/src/linkplay/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10948 2024-04-02 12:26:08.000000 python_linkplay-0.0.5/src/linkplay/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-02 12:26:08.000000 python_linkplay-0.0.5/src/linkplay/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-02 12:26:08.000000 python_linkplay-0.0.5/src/linkplay/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-02 12:26:08.000000 python_linkplay-0.0.5/src/linkplay/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-02 12:26:08.000000 python_linkplay-0.0.5/src/linkplay/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-02 12:26:08.000000 python_linkplay-0.0.5/src/linkplay/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:26:12.510842 python_linkplay-0.0.5/src/python_linkplay.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-02 12:26:12.000000 python_linkplay-0.0.5/src/python_linkplay.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-02 12:26:12.000000 python_linkplay-0.0.5/src/python_linkplay.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 12:26:12.000000 python_linkplay-0.0.5/src/python_linkplay.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 12:26:12.000000 python_linkplay-0.0.5/src/python_linkplay.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-02 12:26:12.000000 python_linkplay-0.0.5/src/python_linkplay.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 12:26:12.000000 python_linkplay-0.0.5/src/python_linkplay.egg-info/top_level.txt
```

### Comparing `python_linkplay-0.0.4/LICENSE` & `python_linkplay-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python_linkplay-0.0.4/PKG-INFO` & `python_linkplay-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: python_linkplay
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python Library for Seamless LinkPlay Device Control
 Author: Velleman Group nv
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: async-timeout==4.0.3
-Requires-Dist: aiohttp==3.9.1
-Requires-Dist: async_upnp_client==0.38.0
+Requires-Dist: async-timeout>=4.0.3
+Requires-Dist: aiohttp>=3.8.5
+Requires-Dist: async_upnp_client>=0.36.2
 Provides-Extra: testing
 Requires-Dist: pytest>=7.3.1; extra == "testing"
 Requires-Dist: pytest-cov>=4.1.0; extra == "testing"
 Requires-Dist: pytest-mock>=3.10.0; extra == "testing"
 Requires-Dist: pytest-asyncio>=0.23.3; extra == "testing"
 Requires-Dist: mypy>=1.3.0; extra == "testing"
 Requires-Dist: flake8>=6.0.0; extra == "testing"
```

### Comparing `python_linkplay-0.0.4/README.md` & `python_linkplay-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `python_linkplay-0.0.4/pyproject.toml` & `python_linkplay-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python_linkplay-0.0.4/setup.cfg` & `python_linkplay-0.0.5/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 license = MIT
 classifiers = 
 	Programming Language :: Python :: 3
 
 [options]
 packages = find_namespace:
 install_requires = 
-	async-timeout==4.0.3
-	aiohttp==3.9.1
-	async_upnp_client==0.38.0
+	async-timeout>=4.0.3
+	aiohttp>=3.8.5
+	async_upnp_client>=0.36.2
 python_requires = >=3.11
 package_dir = 
 	=src
 zip_safe = no
 
 [options.package_data]
 linkplay = py.typed
```

### Comparing `python_linkplay-0.0.4/src/linkplay/bridge.py` & `python_linkplay-0.0.5/src/linkplay/bridge.py`

 * *Files identical despite different names*

### Comparing `python_linkplay-0.0.4/src/linkplay/consts.py` & `python_linkplay-0.0.5/src/linkplay/consts.py`

 * *Files identical despite different names*

### Comparing `python_linkplay-0.0.4/src/linkplay/controller.py` & `python_linkplay-0.0.5/src/linkplay/controller.py`

 * *Files identical despite different names*

### Comparing `python_linkplay-0.0.4/src/linkplay/discovery.py` & `python_linkplay-0.0.5/src/linkplay/discovery.py`

 * *Files identical despite different names*

### Comparing `python_linkplay-0.0.4/src/linkplay/utils.py` & `python_linkplay-0.0.5/src/linkplay/utils.py`

 * *Files identical despite different names*

### Comparing `python_linkplay-0.0.4/src/python_linkplay.egg-info/PKG-INFO` & `python_linkplay-0.0.5/src/python_linkplay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: python_linkplay
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python Library for Seamless LinkPlay Device Control
 Author: Velleman Group nv
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: async-timeout==4.0.3
-Requires-Dist: aiohttp==3.9.1
-Requires-Dist: async_upnp_client==0.38.0
+Requires-Dist: async-timeout>=4.0.3
+Requires-Dist: aiohttp>=3.8.5
+Requires-Dist: async_upnp_client>=0.36.2
 Provides-Extra: testing
 Requires-Dist: pytest>=7.3.1; extra == "testing"
 Requires-Dist: pytest-cov>=4.1.0; extra == "testing"
 Requires-Dist: pytest-mock>=3.10.0; extra == "testing"
 Requires-Dist: pytest-asyncio>=0.23.3; extra == "testing"
 Requires-Dist: mypy>=1.3.0; extra == "testing"
 Requires-Dist: flake8>=6.0.0; extra == "testing"
```

### Comparing `python_linkplay-0.0.4/src/python_linkplay.egg-info/SOURCES.txt` & `python_linkplay-0.0.5/src/python_linkplay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

