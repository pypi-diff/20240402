# Comparing `tmp/hltv-async-api-0.2.3.tar.gz` & `tmp/hltv_async_api-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hltv-async-api-0.2.3.tar", last modified: Tue Apr  2 14:45:53 2024, max compression
+gzip compressed data, was "hltv_async_api-0.2.4.tar", last modified: Tue Apr  2 14:54:09 2024, max compression
```

## Comparing `hltv-async-api-0.2.3.tar` & `hltv_async_api-0.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 14:45:53.694322 hltv-async-api-0.2.3/
--rw-rw-rw-   0        0        0     1091 2024-04-02 00:22:12.000000 hltv-async-api-0.2.3/LICENSE
--rw-rw-rw-   0        0        0     2357 2024-04-02 14:45:53.692406 hltv-async-api-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1734 2024-04-02 13:35:07.000000 hltv-async-api-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 14:45:53.663637 hltv-async-api-0.2.3/hltv-async-api/
--rw-rw-rw-   0        0        0      124 2024-04-02 14:45:39.000000 hltv-async-api-0.2.3/hltv-async-api/__init__.py
--rw-rw-rw-   0        0        0    24378 2024-04-02 13:43:04.000000 hltv-async-api-0.2.3/hltv-async-api/aiohltv.py
-drwxrwxrwx   0        0        0        0 2024-04-02 14:45:53.690898 hltv-async-api-0.2.3/hltv_async_api.egg-info/
--rw-rw-rw-   0        0        0     2357 2024-04-02 14:45:53.000000 hltv-async-api-0.2.3/hltv_async_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-04-02 14:45:53.000000 hltv-async-api-0.2.3/hltv_async_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 14:45:53.000000 hltv-async-api-0.2.3/hltv_async_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-02 14:45:53.000000 hltv-async-api-0.2.3/hltv_async_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      537 2024-04-02 14:45:49.000000 hltv-async-api-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-02 14:45:53.694911 hltv-async-api-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      925 2024-04-02 14:45:42.000000 hltv-async-api-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 14:54:09.763562 hltv_async_api-0.2.4/
+-rw-rw-rw-   0        0        0     1091 2024-04-02 00:22:12.000000 hltv_async_api-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0     2357 2024-04-02 14:54:09.761565 hltv_async_api-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1734 2024-04-02 13:35:07.000000 hltv_async_api-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 14:54:09.740564 hltv_async_api-0.2.4/hltv_async_api/
+-rw-rw-rw-   0        0        0      124 2024-04-02 14:45:39.000000 hltv_async_api-0.2.4/hltv_async_api/__init__.py
+-rw-rw-rw-   0        0        0    24378 2024-04-02 13:43:04.000000 hltv_async_api-0.2.4/hltv_async_api/aiohltv.py
+drwxrwxrwx   0        0        0        0 2024-04-02 14:54:09.760561 hltv_async_api-0.2.4/hltv_async_api.egg-info/
+-rw-rw-rw-   0        0        0     2357 2024-04-02 14:54:09.000000 hltv_async_api-0.2.4/hltv_async_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-04-02 14:54:09.000000 hltv_async_api-0.2.4/hltv_async_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 14:54:09.000000 hltv_async_api-0.2.4/hltv_async_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-02 14:54:09.000000 hltv_async_api-0.2.4/hltv_async_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      537 2024-04-02 14:53:47.000000 hltv_async_api-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-02 14:54:09.763562 hltv_async_api-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      922 2024-04-02 14:54:05.000000 hltv_async_api-0.2.4/setup.py
```

### Comparing `hltv-async-api-0.2.3/LICENSE` & `hltv_async_api-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hltv-async-api-0.2.3/PKG-INFO` & `hltv_async_api-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hltv-async-api
-Version: 0.2.3
+Name: hltv_async_api
+Version: 0.2.4
 Summary: Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python
 Home-page: https://github.com/akimerslys/aiohltv
 Author: akimerslys
 Author-email: Akim Slys <akimslys2003@gmail.com>
 Project-URL: Homepage, https://github.com/akimerslys/aiohltv
 Project-URL: Issues, https://github.com/akimerslys/aiohltv/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hltv-async-api-0.2.3/README.md` & `hltv_async_api-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `hltv-async-api-0.2.3/hltv-async-api/aiohltv.py` & `hltv_async_api-0.2.4/hltv_async_api/aiohltv.py`

 * *Files identical despite different names*

### Comparing `hltv-async-api-0.2.3/hltv_async_api.egg-info/PKG-INFO` & `hltv_async_api-0.2.4/hltv_async_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hltv-async-api
-Version: 0.2.3
+Name: hltv_async_api
+Version: 0.2.4
 Summary: Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python
 Home-page: https://github.com/akimerslys/aiohltv
 Author: akimerslys
 Author-email: Akim Slys <akimslys2003@gmail.com>
 Project-URL: Homepage, https://github.com/akimerslys/aiohltv
 Project-URL: Issues, https://github.com/akimerslys/aiohltv/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hltv-async-api-0.2.3/pyproject.toml` & `hltv_async_api-0.2.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
-name = "hltv-async-api"
-version = "0.2.3"
+name = "hltv_async_api"
+version = "0.2.4"
 authors = [
   { name="Akim Slys", email="akimslys2003@gmail.com" },
 ]
 description = "Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `hltv-async-api-0.2.3/setup.py` & `hltv_async_api-0.2.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
-    name='hltv-async-api',
-    version='0.2.3',
+    name='hltv_async_api',
+    version='0.2.4',
     author='akimerslys',
     author_email='akimslys2003@gmail.com',
     description='Hltv-aio: An unofficial asynchronous HLTV API Wrapper for Python',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/akimerslys/aiohltv',
-    packages=['hltv-async-api'],
+    packages=find_packages(),
 
     install_requires=[
         'aiohttp==3.9.3',
         'aiosignal==1.3.1',
         'attrs==23.2.0',
         'beautifulsoup4==4.12.3',
         'frozenlist==1.4.1',
```

