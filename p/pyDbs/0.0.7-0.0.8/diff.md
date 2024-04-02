# Comparing `tmp/pyDbs-0.0.7.tar.gz` & `tmp/pyDbs-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyDbs-0.0.7.tar", last modified: Thu Nov 23 15:00:57 2023, max compression
+gzip compressed data, was "pyDbs-0.0.8.tar", last modified: Tue Apr  2 13:44:10 2024, max compression
```

## Comparing `pyDbs-0.0.7.tar` & `pyDbs-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-11-23 15:00:57.036854 pyDbs-0.0.7/
--rw-rw-rw-   0        0        0     1089 2023-05-01 08:58:42.000000 pyDbs-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      574 2023-11-23 15:00:57.034464 pyDbs-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       77 2023-05-01 08:58:42.000000 pyDbs-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-11-23 15:00:56.993987 pyDbs-0.0.7/pyDbs/
--rw-rw-rw-   0        0        0       49 2023-10-28 14:29:37.000000 pyDbs-0.0.7/pyDbs/__init__.py
--rw-rw-rw-   0        0        0    22134 2023-11-23 14:58:26.000000 pyDbs-0.0.7/pyDbs/base.py
--rw-rw-rw-   0        0        0     8357 2023-11-23 12:44:32.000000 pyDbs-0.0.7/pyDbs/simpleDB.py
-drwxrwxrwx   0        0        0        0 2023-11-23 15:00:57.031906 pyDbs-0.0.7/pyDbs.egg-info/
--rw-rw-rw-   0        0        0      574 2023-11-23 15:00:56.000000 pyDbs-0.0.7/pyDbs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-11-23 15:00:56.000000 pyDbs-0.0.7/pyDbs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-23 15:00:56.000000 pyDbs-0.0.7/pyDbs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-11-23 15:00:56.000000 pyDbs-0.0.7/pyDbs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-11-23 15:00:56.000000 pyDbs-0.0.7/pyDbs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-23 15:00:57.037856 pyDbs-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      672 2023-11-23 14:59:43.000000 pyDbs-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 13:44:10.207263 pyDbs-0.0.8/
+-rw-rw-rw-   0        0        0     1089 2023-05-01 08:58:42.000000 pyDbs-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      574 2024-04-02 13:44:10.206301 pyDbs-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       77 2023-05-01 08:58:42.000000 pyDbs-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 13:44:10.177511 pyDbs-0.0.8/pyDbs/
+-rw-rw-rw-   0        0        0       49 2023-10-28 14:29:37.000000 pyDbs-0.0.8/pyDbs/__init__.py
+-rw-rw-rw-   0        0        0    22293 2024-04-02 13:33:42.000000 pyDbs-0.0.8/pyDbs/base.py
+-rw-rw-rw-   0        0        0     8357 2024-01-16 09:20:38.000000 pyDbs-0.0.8/pyDbs/simpleDB.py
+drwxrwxrwx   0        0        0        0 2024-04-02 13:44:10.203318 pyDbs-0.0.8/pyDbs.egg-info/
+-rw-rw-rw-   0        0        0      574 2024-04-02 13:44:10.000000 pyDbs-0.0.8/pyDbs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2024-04-02 13:44:10.000000 pyDbs-0.0.8/pyDbs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 13:44:10.000000 pyDbs-0.0.8/pyDbs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-04-02 13:44:10.000000 pyDbs-0.0.8/pyDbs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-02 13:44:10.000000 pyDbs-0.0.8/pyDbs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 13:44:10.208266 pyDbs-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      672 2024-04-02 13:42:21.000000 pyDbs-0.0.8/setup.py
```

### Comparing `pyDbs-0.0.7/LICENSE` & `pyDbs-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyDbs-0.0.7/PKG-INFO` & `pyDbs-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDbs
-Version: 0.0.7
+Version: 0.0.8
 Summary: Custom database class (relies on pandas, scipy)
 Home-page: https://github.com/ChampionApe/pyDbs
 Author: Rasmus K. Skjødt Berg
 Author-email: rasmus.kehlet.berg@econ.ku.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
```

### Comparing `pyDbs-0.0.7/pyDbs/base.py` & `pyDbs-0.0.8/pyDbs/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,25 +157,28 @@
 		""" Subset x with index of variable 'name' using linear indexing from self.maps."""
 		return x[self[name]]
 
 	def unloadSol(self, x):
 		return {k: self.get(x, k) for k in self}
 
 	def get(self, x, name, **kwargs):
-		""" __call__ method, but returned as pandas object """
+		""" __call__ method, but returned as pandas object"""
 		return pd.Series(x[self[name]], index = self[name].index, name = name)
-
+		
 	def getr(self, x, name, **kwargs):
 		""" Like the get method, but more robust (adds more potential adjustments to the symbol) """
-		k = adj.rc_pd(self[name], **kwargs)
-		return pd.Series(x[k], index = k.index, name = name)
+		if self.symbols[name] is None: # check if the symbol is a scalar
+			return x[self[name][0]] # return without pandas object
+		else:
+			k = adj.rc_pd(self[name], **kwargs)
+			return pd.Series(x[k], index = k.index, name = name)
 
 	def compile(self):
 		keys, vals = list(self.symbols.keys()), list(self.symbols.values())
-		steps = np.array([0]+[len(x) for x in vals]).cumsum()
+		steps = np.array([0]+[1 if x is None else len(x) for x in vals]).cumsum()
 		self.len = steps[-1]
 		self.maps = {keys[i]: pd.Series(range(steps[i], steps[i+1]), index = getIndex(vals[i])) for i in range(len(keys))}
 
 	def applyMapGlobalIdx(self, symbol, m):
 		return pd.Series(symbol[m.values].values, m.index)
 
 	def addSymFromMap(self, name, symbol, m):
```

### Comparing `pyDbs-0.0.7/pyDbs/simpleDB.py` & `pyDbs-0.0.8/pyDbs/simpleDB.py`

 * *Files identical despite different names*

### Comparing `pyDbs-0.0.7/pyDbs.egg-info/PKG-INFO` & `pyDbs-0.0.8/pyDbs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDbs
-Version: 0.0.7
+Version: 0.0.8
 Summary: Custom database class (relies on pandas, scipy)
 Home-page: https://github.com/ChampionApe/pyDbs
 Author: Rasmus K. Skjødt Berg
 Author-email: rasmus.kehlet.berg@econ.ku.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
```

### Comparing `pyDbs-0.0.7/setup.py` & `pyDbs-0.0.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as file:
   long_description = file.read()
 
 setuptools.setup(
   name="pyDbs",
-  version="0.0.7",
+  version="0.0.8",
   author="Rasmus K. Skjødt Berg",
   author_email="rasmus.kehlet.berg@econ.ku.dk",
   description="Custom database class (relies on pandas, scipy)",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ChampionApe/pyDbs",
   packages=setuptools.find_packages(),
```

