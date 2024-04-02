# Comparing `tmp/muti.numer-0.0.3.tar.gz` & `tmp/muti.numer-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muti.numer-0.0.3.tar", last modified: Tue Apr  2 06:50:10 2024, max compression
+gzip compressed data, was "muti.numer-0.0.4.tar", last modified: Tue Apr  2 07:19:34 2024, max compression
```

## Comparing `muti.numer-0.0.3.tar` & `muti.numer-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 06:50:10.013462 muti.numer-0.0.3/
--rw-rw-rw-   0        0        0     1089 2024-03-22 08:37:41.000000 muti.numer-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      767 2024-04-02 06:50:10.012216 muti.numer-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      346 2024-03-29 10:24:16.000000 muti.numer-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 06:50:10.012216 muti.numer-0.0.3/muti.numer.egg-info/
--rw-rw-rw-   0        0        0      767 2024-04-02 06:50:09.000000 muti.numer-0.0.3/muti.numer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2024-04-02 06:50:09.000000 muti.numer-0.0.3/muti.numer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 06:50:09.000000 muti.numer-0.0.3/muti.numer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-02 06:50:09.000000 muti.numer-0.0.3/muti.numer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-02 06:50:10.011218 muti.numer-0.0.3/numer/
--rw-rw-rw-   0        0        0     1300 2024-04-02 06:48:06.000000 muti.numer-0.0.3/numer/__deps__.py
--rw-rw-rw-   0        0        0      562 2024-04-02 06:49:33.000000 muti.numer-0.0.3/numer/__init__.py
--rw-rw-rw-   0        0        0     2326 2024-04-02 06:48:19.000000 muti.numer-0.0.3/numer/depLam.py
--rw-rw-rw-   0        0        0      903 2024-04-02 06:49:59.000000 muti.numer-0.0.3/numer/iniLam.py
--rw-rw-rw-   0        0        0     1748 2024-04-02 06:49:13.000000 muti.numer-0.0.3/numer/modLas.py
--rw-rw-rw-   0        0        0    11574 2024-04-02 06:48:45.000000 muti.numer-0.0.3/numer/shfLam.py
--rw-rw-rw-   0        0        0       42 2024-04-02 06:50:10.013462 muti.numer-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      653 2024-04-02 06:49:58.000000 muti.numer-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 07:19:34.824556 muti.numer-0.0.4/
+-rw-rw-rw-   0        0        0     1089 2024-03-22 08:37:41.000000 muti.numer-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      767 2024-04-02 07:19:34.823556 muti.numer-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2024-03-29 10:24:16.000000 muti.numer-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 07:19:34.823556 muti.numer-0.0.4/muti.numer.egg-info/
+-rw-rw-rw-   0        0        0      767 2024-04-02 07:19:34.000000 muti.numer-0.0.4/muti.numer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2024-04-02 07:19:34.000000 muti.numer-0.0.4/muti.numer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 07:19:34.000000 muti.numer-0.0.4/muti.numer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-02 07:19:34.000000 muti.numer-0.0.4/muti.numer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 07:19:34.822557 muti.numer-0.0.4/numer/
+-rw-rw-rw-   0        0        0     1300 2024-04-02 06:48:06.000000 muti.numer-0.0.4/numer/__deps__.py
+-rw-rw-rw-   0        0        0      562 2024-04-02 06:49:33.000000 muti.numer-0.0.4/numer/__init__.py
+-rw-rw-rw-   0        0        0     2326 2024-04-02 06:48:19.000000 muti.numer-0.0.4/numer/depLam.py
+-rw-rw-rw-   0        0        0      903 2024-04-02 06:49:59.000000 muti.numer-0.0.4/numer/iniLam.py
+-rw-rw-rw-   0        0        0     1762 2024-04-02 07:18:35.000000 muti.numer-0.0.4/numer/modLas.py
+-rw-rw-rw-   0        0        0    11574 2024-04-02 06:48:45.000000 muti.numer-0.0.4/numer/shfLam.py
+-rw-rw-rw-   0        0        0       42 2024-04-02 07:19:34.824556 muti.numer-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      653 2024-04-02 07:19:24.000000 muti.numer-0.0.4/setup.py
```

### Comparing `muti.numer-0.0.3/LICENSE` & `muti.numer-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `muti.numer-0.0.3/PKG-INFO` & `muti.numer-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muti.numer
-Version: 0.0.3
+Version: 0.0.4
 Summary: utils for math-numer
 Home-page: https://github.com/E-C-Ares/
 Author: E.C.Ares
 Author-email: E.C.Ares@outlook.com
 License: MIT DIVIƷON
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `muti.numer-0.0.3/muti.numer.egg-info/PKG-INFO` & `muti.numer-0.0.4/muti.numer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muti.numer
-Version: 0.0.3
+Version: 0.0.4
 Summary: utils for math-numer
 Home-page: https://github.com/E-C-Ares/
 Author: E.C.Ares
 Author-email: E.C.Ares@outlook.com
 License: MIT DIVIƷON
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `muti.numer-0.0.3/numer/__deps__.py` & `muti.numer-0.0.4/numer/__deps__.py`

 * *Files identical despite different names*

### Comparing `muti.numer-0.0.3/numer/__init__.py` & `muti.numer-0.0.4/numer/__init__.py`

 * *Files identical despite different names*

### Comparing `muti.numer-0.0.3/numer/depLam.py` & `muti.numer-0.0.4/numer/depLam.py`

 * *Files identical despite different names*

### Comparing `muti.numer-0.0.3/numer/iniLam.py` & `muti.numer-0.0.4/numer/iniLam.py`

 * *Files identical despite different names*

### Comparing `muti.numer-0.0.3/numer/modLas.py` & `muti.numer-0.0.4/numer/modLas.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,9 +34,11 @@
         pass
 
     def addnMod(self, mod, nym): return self.add_module(nym, mod)
     def getrWrd(self,*i)       : return self.forward(*i)
     def set_dmm(self,mm)       : shftLai(self, mm) # gpu cpu ipu cuda 123 empty sbe called before constructing optimizer
     def set_rmm(self,nm='c')   : nRnm(self.module(), nm) # test, train(mode), eval, run
     def getrPat(self, rec=True): return self.parameters(recurse=rec) # self.get_parameter()
-    def detrMod(self)          : (for child in self.children(): yield child)
-    def getrChi(self)          : (for child in self.children(): yield child)
+    def detrMod(self)          :
+        for child in self.children(): yield child
+    def getrChi(self)          :
+        for child in self.children(): yield child
```

### Comparing `muti.numer-0.0.3/numer/shfLam.py` & `muti.numer-0.0.4/numer/shfLam.py`

 * *Files identical despite different names*

### Comparing `muti.numer-0.0.3/setup.py` & `muti.numer-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   url          = "https://github.com/E-C-Ares/",
   name         = "muti.numer",
-  version      = "0.0.3",
+  version      = "0.0.4",
   author       = "E.C.Ares",
   author_email = "E.C.Ares@outlook.com",
   license      = 'MIT DIVIƷON',
   description  = "utils for math-numer",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages     = setuptools.find_packages(),
```

