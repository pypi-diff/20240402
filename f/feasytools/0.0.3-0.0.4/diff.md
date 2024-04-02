# Comparing `tmp/feasytools-0.0.3.tar.gz` & `tmp/feasytools-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\feasytools-0.0.3.tar", last modified: Tue Apr  2 03:01:41 2024, max compression
+gzip compressed data, was "dist\feasytools-0.0.4.tar", last modified: Tue Apr  2 04:13:03 2024, max compression
```

## Comparing `feasytools-0.0.3.tar` & `feasytools-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 03:01:41.000000 feasytools-0.0.3/
-drwxrwxrwx   0        0        0        0 2024-04-02 03:01:41.000000 feasytools-0.0.3/feasytools/
--rw-rw-rw-   0        0        0     3708 2024-04-02 02:59:22.000000 feasytools-0.0.3/feasytools/argchk.py
--rw-rw-rw-   0        0        0     5348 2024-03-28 11:46:52.000000 feasytools-0.0.3/feasytools/pq.py
--rw-rw-rw-   0        0        0     1897 2024-03-23 07:36:53.000000 feasytools-0.0.3/feasytools/rangelist.py
--rw-rw-rw-   0        0        0    17755 2024-03-23 07:46:48.000000 feasytools-0.0.3/feasytools/table.py
--rw-rw-rw-   0        0        0     8469 2024-03-28 11:21:46.000000 feasytools-0.0.3/feasytools/tfunc.py
--rw-rw-rw-   0        0        0      255 2024-03-23 06:37:28.000000 feasytools-0.0.3/feasytools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 03:01:41.000000 feasytools-0.0.3/feasytools.egg-info/
--rw-rw-rw-   0        0        0        1 2024-04-02 03:01:41.000000 feasytools-0.0.3/feasytools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      835 2024-04-02 03:01:41.000000 feasytools-0.0.3/feasytools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       14 2024-04-02 03:01:41.000000 feasytools-0.0.3/feasytools.egg-info/requires.txt
--rw-rw-rw-   0        0        0      312 2024-04-02 03:01:41.000000 feasytools-0.0.3/feasytools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       11 2024-04-02 03:01:41.000000 feasytools-0.0.3/feasytools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      835 2024-04-02 03:01:41.000000 feasytools-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      316 2024-03-23 07:58:23.000000 feasytools-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-02 03:01:41.000000 feasytools-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      683 2024-03-30 15:04:44.000000 feasytools-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:13:03.000000 feasytools-0.0.4/
+drwxrwxrwx   0        0        0        0 2024-04-02 04:13:03.000000 feasytools-0.0.4/feasytools/
+-rw-rw-rw-   0        0        0     3770 2024-04-02 04:11:37.000000 feasytools-0.0.4/feasytools/argchk.py
+-rw-rw-rw-   0        0        0     5348 2024-03-28 11:46:52.000000 feasytools-0.0.4/feasytools/pq.py
+-rw-rw-rw-   0        0        0     1897 2024-03-23 07:36:53.000000 feasytools-0.0.4/feasytools/rangelist.py
+-rw-rw-rw-   0        0        0    17755 2024-03-23 07:46:48.000000 feasytools-0.0.4/feasytools/table.py
+-rw-rw-rw-   0        0        0     8469 2024-03-28 11:21:46.000000 feasytools-0.0.4/feasytools/tfunc.py
+-rw-rw-rw-   0        0        0      255 2024-03-23 06:37:28.000000 feasytools-0.0.4/feasytools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:13:03.000000 feasytools-0.0.4/feasytools.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-04-02 04:13:03.000000 feasytools-0.0.4/feasytools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      835 2024-04-02 04:13:03.000000 feasytools-0.0.4/feasytools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2024-04-02 04:13:03.000000 feasytools-0.0.4/feasytools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      312 2024-04-02 04:13:03.000000 feasytools-0.0.4/feasytools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       11 2024-04-02 04:13:03.000000 feasytools-0.0.4/feasytools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      835 2024-04-02 04:13:03.000000 feasytools-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2024-03-23 07:58:23.000000 feasytools-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-02 04:13:03.000000 feasytools-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      683 2024-04-02 04:12:53.000000 feasytools-0.0.4/setup.py
```

### Comparing `feasytools-0.0.3/feasytools/argchk.py` & `feasytools-0.0.4/feasytools/argchk.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,16 +61,18 @@
                 raise ValueError(f"无效参数'{v}'")
         if cur_key != None: ret[cur_key] = True
         return ret
 
     def __init__(self, pars:'Union[None,str,dict[str,Any]]' = None):
         if pars is None:
             self.__args = ArgChecker.get_dict()
-        elif isinstance(pars, (str, dict)):
+        elif isinstance(pars, str):
             self.__args = ArgChecker.get_dict(pars)
+        elif isinstance(pars, dict):
+            self.__args = pars
         else:
             raise TypeError("参数类型错误")
     
     def pop_bool(self, key:str) -> bool:
         if self.__args.pop(key, False): return True
         return False
```

### Comparing `feasytools-0.0.3/feasytools/pq.py` & `feasytools-0.0.4/feasytools/pq.py`

 * *Files identical despite different names*

### Comparing `feasytools-0.0.3/feasytools/rangelist.py` & `feasytools-0.0.4/feasytools/rangelist.py`

 * *Files identical despite different names*

### Comparing `feasytools-0.0.3/feasytools/table.py` & `feasytools-0.0.4/feasytools/table.py`

 * *Files identical despite different names*

### Comparing `feasytools-0.0.3/feasytools/tfunc.py` & `feasytools-0.0.4/feasytools/tfunc.py`

 * *Files identical despite different names*

### Comparing `feasytools-0.0.3/feasytools.egg-info/PKG-INFO` & `feasytools-0.0.4/feasytools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feasytools
-Version: 0.0.3
+Version: 0.0.4
 Summary: A set of tools for data processing, including Time Function, Table, Priority Queue, Range List, etc.
 Home-page: UNKNOWN
 Author: fmy_xfk
 License: UNKNOWN
 Description: # FEasyTools: Some useful components
         - dprov: Data provider as time functions
         - argchk: Argument parser with type checking
```

### Comparing `feasytools-0.0.3/PKG-INFO` & `feasytools-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feasytools
-Version: 0.0.3
+Version: 0.0.4
 Summary: A set of tools for data processing, including Time Function, Table, Priority Queue, Range List, etc.
 Home-page: UNKNOWN
 Author: fmy_xfk
 License: UNKNOWN
 Description: # FEasyTools: Some useful components
         - dprov: Data provider as time functions
         - argchk: Argument parser with type checking
```

### Comparing `feasytools-0.0.3/setup.py` & `feasytools-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="feasytools",
-    version="0.0.3",
+    version="0.0.4",
     author="fmy_xfk",
     packages=find_packages(),
     description="A set of tools for data processing, including Time Function, Table, Priority Queue, Range List, etc.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
```

