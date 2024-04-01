# Comparing `tmp/ipcidrtree-1.3.0.tar.gz` & `tmp/ipcidrtree-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipcidrtree-1.3.0.tar", last modified: Mon Oct 30 23:06:30 2023, max compression
+gzip compressed data, was "ipcidrtree-1.3.1.tar", last modified: Mon Apr  1 22:51:36 2024, max compression
```

## Comparing `ipcidrtree-1.3.0.tar` & `ipcidrtree-1.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2023-10-30 23:06:30.066383 ipcidrtree-1.3.0/
--rw-rw-r--   0 steve     (1000) steve     (1000)     1511 2023-10-30 21:16:31.000000 ipcidrtree-1.3.0/LICENSE
--rw-r--r--   0 steve     (1000) steve     (1000)      766 2023-10-30 23:06:30.062383 ipcidrtree-1.3.0/PKG-INFO
--rw-rw-r--   0 steve     (1000) steve     (1000)      225 2023-10-30 23:02:31.000000 ipcidrtree-1.3.0/README.md
--rw-rw-r--   0 steve     (1000) steve     (1000)      615 2023-10-30 23:02:45.000000 ipcidrtree-1.3.0/pyproject.toml
--rw-rw-r--   0 steve     (1000) steve     (1000)       38 2023-10-30 23:06:30.066383 ipcidrtree-1.3.0/setup.cfg
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2023-10-30 23:06:30.062383 ipcidrtree-1.3.0/src/
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2023-10-30 23:06:30.062383 ipcidrtree-1.3.0/src/ipcidrtree/
--rw-rw-r--   0 steve     (1000) steve     (1000)    30844 2023-10-30 23:03:19.000000 ipcidrtree-1.3.0/src/ipcidrtree/__init__.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     3274 2023-10-30 23:03:41.000000 ipcidrtree-1.3.0/src/ipcidrtree/iprange.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     2916 2023-10-30 23:03:29.000000 ipcidrtree-1.3.0/src/ipcidrtree/ipset.py
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2023-10-30 23:06:30.062383 ipcidrtree-1.3.0/src/ipcidrtree.egg-info/
--rw-r--r--   0 steve     (1000) steve     (1000)      766 2023-10-30 23:06:30.000000 ipcidrtree-1.3.0/src/ipcidrtree.egg-info/PKG-INFO
--rw-rw-r--   0 steve     (1000) steve     (1000)      261 2023-10-30 23:06:30.000000 ipcidrtree-1.3.0/src/ipcidrtree.egg-info/SOURCES.txt
--rw-rw-r--   0 steve     (1000) steve     (1000)        1 2023-10-30 23:06:30.000000 ipcidrtree-1.3.0/src/ipcidrtree.egg-info/dependency_links.txt
--rw-rw-r--   0 steve     (1000) steve     (1000)       11 2023-10-30 23:06:30.000000 ipcidrtree-1.3.0/src/ipcidrtree.egg-info/top_level.txt
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2024-04-01 22:51:36.036610 ipcidrtree-1.3.1/
+-rw-rw-r--   0 steve     (1000) steve     (1000)     1511 2023-10-30 21:16:31.000000 ipcidrtree-1.3.1/LICENSE
+-rw-r--r--   0 steve     (1000) steve     (1000)      766 2024-04-01 22:51:36.036610 ipcidrtree-1.3.1/PKG-INFO
+-rw-rw-r--   0 steve     (1000) steve     (1000)      225 2023-10-30 23:02:31.000000 ipcidrtree-1.3.1/README.md
+-rw-rw-r--   0 steve     (1000) steve     (1000)      615 2024-04-01 22:50:11.000000 ipcidrtree-1.3.1/pyproject.toml
+-rw-rw-r--   0 steve     (1000) steve     (1000)       38 2024-04-01 22:51:36.036610 ipcidrtree-1.3.1/setup.cfg
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2024-04-01 22:51:36.036610 ipcidrtree-1.3.1/src/
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2024-04-01 22:51:36.036610 ipcidrtree-1.3.1/src/ipcidrtree/
+-rw-rw-r--   0 steve     (1000) steve     (1000)    30844 2024-04-01 22:50:33.000000 ipcidrtree-1.3.1/src/ipcidrtree/__init__.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     3274 2023-10-30 23:03:41.000000 ipcidrtree-1.3.1/src/ipcidrtree/iprange.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     2916 2023-10-30 23:03:29.000000 ipcidrtree-1.3.1/src/ipcidrtree/ipset.py
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2024-04-01 22:51:36.036610 ipcidrtree-1.3.1/src/ipcidrtree.egg-info/
+-rw-r--r--   0 steve     (1000) steve     (1000)      766 2024-04-01 22:51:36.000000 ipcidrtree-1.3.1/src/ipcidrtree.egg-info/PKG-INFO
+-rw-rw-r--   0 steve     (1000) steve     (1000)      261 2024-04-01 22:51:36.000000 ipcidrtree-1.3.1/src/ipcidrtree.egg-info/SOURCES.txt
+-rw-rw-r--   0 steve     (1000) steve     (1000)        1 2024-04-01 22:51:36.000000 ipcidrtree-1.3.1/src/ipcidrtree.egg-info/dependency_links.txt
+-rw-rw-r--   0 steve     (1000) steve     (1000)       11 2024-04-01 22:51:36.000000 ipcidrtree-1.3.1/src/ipcidrtree.egg-info/top_level.txt
```

### Comparing `ipcidrtree-1.3.0/LICENSE` & `ipcidrtree-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ipcidrtree-1.3.0/PKG-INFO` & `ipcidrtree-1.3.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipcidrtree
-Version: 1.3.0
+Version: 1.3.1
 Summary: Represent IPv4 information in tree structures
 Author-email: Steve Benson <steve@xelphene.net>
 Project-URL: Homepage, https://github.com/xelphene/iptree
 Project-URL: Bug Tracker, https://github.com/xelphene/iptree/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `ipcidrtree-1.3.0/pyproject.toml` & `ipcidrtree-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ipcidrtree"
-version = "1.3.0"
+version = "1.3.1"
 authors = [
   { name="Steve Benson", email="steve@xelphene.net" },
 ]
 description = "Represent IPv4 information in tree structures"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `ipcidrtree-1.3.0/src/ipcidrtree/__init__.py` & `ipcidrtree-1.3.1/src/ipcidrtree/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,17 +71,17 @@
 """
 
 import re
 import types
 import sys
 import math
 
-__version__='1.3.0'
+__version__='1.3.1'
 __author__='Steve Benson'
-__date__='2023-oct-30'
+__date__='2024-apr-01'
 
 def plen2int(plen):
 	"""Takes an integer in 0..32 (a subnet mask expressed in "slash"
 	notation) and returns a 32 bit unsigned integer representing the netmask."""
 	return (2**plen-1) * 2**(32-plen)
 
 def _log2(n):
@@ -243,22 +243,22 @@
 
 	def __init__(self,val):
 
 		"""The address argument can be a string (which will be parsed to an
 		integer via the Parser class), an integer (such that 0 <= i
 		< 2**32), or another Address or subclass.""" 
 
-		if type(val)==bytes:
+		if type(val)==bytes or type(val)==str:
 			(addr,mask) = Parser().parse_i(val)
 			if mask is not None:
 				raise ValueError('string argument "%s" to IPNumber constructor contains a netmask.' % val)
 			#self._set_int(p.parse(val))
 			self._set_int(addr)
 
-		elif type(val)==int or type(val)==int:
+		elif type(val)==int:
 			self._set_int(val)
 		
 		#elif type(val)==types.InstanceType and issubclass(val.__class__,IPNumber):
 		elif isinstance(val, IPNumber):
 			self._ip_int=val._ip_int
 
 		else:
```

### Comparing `ipcidrtree-1.3.0/src/ipcidrtree/iprange.py` & `ipcidrtree-1.3.1/src/ipcidrtree/iprange.py`

 * *Files identical despite different names*

### Comparing `ipcidrtree-1.3.0/src/ipcidrtree/ipset.py` & `ipcidrtree-1.3.1/src/ipcidrtree/ipset.py`

 * *Files identical despite different names*

### Comparing `ipcidrtree-1.3.0/src/ipcidrtree.egg-info/PKG-INFO` & `ipcidrtree-1.3.1/src/ipcidrtree.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipcidrtree
-Version: 1.3.0
+Version: 1.3.1
 Summary: Represent IPv4 information in tree structures
 Author-email: Steve Benson <steve@xelphene.net>
 Project-URL: Homepage, https://github.com/xelphene/iptree
 Project-URL: Bug Tracker, https://github.com/xelphene/iptree/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

