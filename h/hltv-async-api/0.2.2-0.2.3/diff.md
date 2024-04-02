# Comparing `tmp/hltv-async-api-0.2.2.tar.gz` & `tmp/hltv-async-api-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hltv-async-api-0.2.2.tar", last modified: Tue Apr  2 14:42:41 2024, max compression
+gzip compressed data, was "hltv-async-api-0.2.3.tar", last modified: Tue Apr  2 14:45:53 2024, max compression
```

## Comparing `hltv-async-api-0.2.2.tar` & `hltv-async-api-0.2.3.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 14:42:41.157002 hltv-async-api-0.2.2/
--rw-rw-rw-   0        0        0     1091 2024-04-02 00:22:12.000000 hltv-async-api-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     2357 2024-04-02 14:42:41.155003 hltv-async-api-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1734 2024-04-02 13:35:07.000000 hltv-async-api-0.2.2/README.md
--rw-rw-rw-   0        0        0      537 2024-04-02 14:30:55.000000 hltv-async-api-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-02 14:42:41.157002 hltv-async-api-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      955 2024-04-02 14:42:38.000000 hltv-async-api-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 14:42:41.125996 hltv-async-api-0.2.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-02 14:42:41.134001 hltv-async-api-0.2.2/src/hltv-async-api/
--rw-rw-rw-   0        0        0      124 2024-04-02 14:35:58.000000 hltv-async-api-0.2.2/src/hltv-async-api/__init__.py
--rw-rw-rw-   0        0        0    24378 2024-04-02 13:43:04.000000 hltv-async-api-0.2.2/src/hltv-async-api/aiohltv.py
-drwxrwxrwx   0        0        0        0 2024-04-02 14:42:41.153001 hltv-async-api-0.2.2/src/hltv_async_api.egg-info/
--rw-rw-rw-   0        0        0     2357 2024-04-02 14:42:41.000000 hltv-async-api-0.2.2/src/hltv_async_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2024-04-02 14:42:41.000000 hltv-async-api-0.2.2/src/hltv_async_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 14:42:41.000000 hltv-async-api-0.2.2/src/hltv_async_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-02 14:42:41.000000 hltv-async-api-0.2.2/src/hltv_async_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 14:45:53.694322 hltv-async-api-0.2.3/
+-rw-rw-rw-   0        0        0     1091 2024-04-02 00:22:12.000000 hltv-async-api-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     2357 2024-04-02 14:45:53.692406 hltv-async-api-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1734 2024-04-02 13:35:07.000000 hltv-async-api-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 14:45:53.663637 hltv-async-api-0.2.3/hltv-async-api/
+-rw-rw-rw-   0        0        0      124 2024-04-02 14:45:39.000000 hltv-async-api-0.2.3/hltv-async-api/__init__.py
+-rw-rw-rw-   0        0        0    24378 2024-04-02 13:43:04.000000 hltv-async-api-0.2.3/hltv-async-api/aiohltv.py
+drwxrwxrwx   0        0        0        0 2024-04-02 14:45:53.690898 hltv-async-api-0.2.3/hltv_async_api.egg-info/
+-rw-rw-rw-   0        0        0     2357 2024-04-02 14:45:53.000000 hltv-async-api-0.2.3/hltv_async_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-04-02 14:45:53.000000 hltv-async-api-0.2.3/hltv_async_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 14:45:53.000000 hltv-async-api-0.2.3/hltv_async_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-02 14:45:53.000000 hltv-async-api-0.2.3/hltv_async_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      537 2024-04-02 14:45:49.000000 hltv-async-api-0.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-02 14:45:53.694911 hltv-async-api-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      925 2024-04-02 14:45:42.000000 hltv-async-api-0.2.3/setup.py
```

### Comparing `hltv-async-api-0.2.2/LICENSE` & `hltv-async-api-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hltv-async-api-0.2.2/PKG-INFO` & `hltv-async-api-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hltv-async-api
-Version: 0.2.2
+Version: 0.2.3
 Summary: Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python
 Home-page: https://github.com/akimerslys/aiohltv
 Author: akimerslys
 Author-email: Akim Slys <akimslys2003@gmail.com>
 Project-URL: Homepage, https://github.com/akimerslys/aiohltv
 Project-URL: Issues, https://github.com/akimerslys/aiohltv/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hltv-async-api-0.2.2/README.md` & `hltv-async-api-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `hltv-async-api-0.2.2/pyproject.toml` & `hltv-async-api-0.2.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hltv-async-api"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   { name="Akim Slys", email="akimslys2003@gmail.com" },
 ]
 description = "Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `hltv-async-api-0.2.2/setup.py` & `hltv-async-api-0.2.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name='hltv-async-api',
-    version='0.2.2',
+    version='0.2.3',
     author='akimerslys',
     author_email='akimslys2003@gmail.com',
     description='Hltv-aio: An unofficial asynchronous HLTV API Wrapper for Python',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/akimerslys/aiohltv',
-    package_dir={'': 'src'},
     packages=['hltv-async-api'],
 
     install_requires=[
         'aiohttp==3.9.3',
         'aiosignal==1.3.1',
         'attrs==23.2.0',
         'beautifulsoup4==4.12.3',
```

### Comparing `hltv-async-api-0.2.2/src/hltv-async-api/aiohltv.py` & `hltv-async-api-0.2.3/hltv-async-api/aiohltv.py`

 * *Files identical despite different names*

### Comparing `hltv-async-api-0.2.2/src/hltv_async_api.egg-info/PKG-INFO` & `hltv-async-api-0.2.3/hltv_async_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hltv-async-api
-Version: 0.2.2
+Version: 0.2.3
 Summary: Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python
 Home-page: https://github.com/akimerslys/aiohltv
 Author: akimerslys
 Author-email: Akim Slys <akimslys2003@gmail.com>
 Project-URL: Homepage, https://github.com/akimerslys/aiohltv
 Project-URL: Issues, https://github.com/akimerslys/aiohltv/issues
 Classifier: Programming Language :: Python :: 3
```

