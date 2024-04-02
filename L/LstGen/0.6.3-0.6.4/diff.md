# Comparing `tmp/LstGen-0.6.3.tar.gz` & `tmp/LstGen-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LstGen-0.6.3.tar", last modified: Fri Oct 13 11:44:44 2023, max compression
+gzip compressed data, was "LstGen-0.6.4.tar", last modified: Tue Apr  2 11:24:21 2024, max compression
```

## Comparing `LstGen-0.6.3.tar` & `LstGen-0.6.4.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 jenner    (1000) jenner    (1000)        0 2023-10-13 11:44:44.180000 LstGen-0.6.3/
--rw-r--r--   0 jenner    (1000) jenner    (1000)     1522 2023-10-13 11:43:22.000000 LstGen-0.6.3/CHANGES.md
-drwxr-xr-x   0 jenner    (1000) jenner    (1000)        0 2023-10-13 11:44:44.180000 LstGen-0.6.3/LstGen.egg-info/
--rw-r--r--   0 jenner    (1000) jenner    (1000)    10049 2023-10-13 11:44:44.000000 LstGen-0.6.3/LstGen.egg-info/PKG-INFO
--rw-r--r--   0 jenner    (1000) jenner    (1000)      676 2023-10-13 11:44:44.000000 LstGen-0.6.3/LstGen.egg-info/SOURCES.txt
--rw-r--r--   0 jenner    (1000) jenner    (1000)        1 2023-10-13 11:44:44.000000 LstGen-0.6.3/LstGen.egg-info/dependency_links.txt
--rw-r--r--   0 jenner    (1000) jenner    (1000)       55 2023-10-13 11:44:44.000000 LstGen-0.6.3/LstGen.egg-info/entry_points.txt
--rw-r--r--   0 jenner    (1000) jenner    (1000)        1 2022-01-13 13:23:17.000000 LstGen-0.6.3/LstGen.egg-info/not-zip-safe
--rw-r--r--   0 jenner    (1000) jenner    (1000)       53 2023-10-13 11:44:44.000000 LstGen-0.6.3/LstGen.egg-info/requires.txt
--rw-r--r--   0 jenner    (1000) jenner    (1000)        7 2023-10-13 11:44:44.000000 LstGen-0.6.3/LstGen.egg-info/top_level.txt
--rw-r--r--   0 jenner    (1000) jenner    (1000)       79 2022-10-17 11:19:47.000000 LstGen-0.6.3/MANIFEST.in
--rw-r--r--   0 jenner    (1000) jenner    (1000)    10049 2023-10-13 11:44:44.180000 LstGen-0.6.3/PKG-INFO
--rw-r--r--   0 jenner    (1000) jenner    (1000)     5510 2022-10-17 12:12:20.000000 LstGen-0.6.3/README.md
-drwxr-xr-x   0 jenner    (1000) jenner    (1000)        0 2023-10-13 11:44:44.180000 LstGen-0.6.3/lstgen/
--rw-r--r--   0 jenner    (1000) jenner    (1000)     9809 2022-01-13 13:21:55.000000 LstGen-0.6.3/lstgen/__init__.py
--rw-r--r--   0 jenner    (1000) jenner    (1000)     5192 2022-10-17 11:59:58.000000 LstGen-0.6.3/lstgen/cli.py
-drwxr-xr-x   0 jenner    (1000) jenner    (1000)        0 2023-10-13 11:44:44.180000 LstGen-0.6.3/lstgen/generators/
--rw-r--r--   0 jenner    (1000) jenner    (1000)      528 2022-10-17 12:01:11.000000 LstGen-0.6.3/lstgen/generators/__init__.py
--rw-r--r--   0 jenner    (1000) jenner    (1000)     7708 2022-01-13 13:21:55.000000 LstGen-0.6.3/lstgen/generators/ast2code.py
--rw-r--r--   0 jenner    (1000) jenner    (1000)     4874 2022-01-13 13:21:55.000000 LstGen-0.6.3/lstgen/generators/base.py
-drwxr-xr-x   0 jenner    (1000) jenner    (1000)        0 2023-10-13 11:44:44.180000 LstGen-0.6.3/lstgen/generators/golang/
--rw-r--r--   0 jenner    (1000) jenner    (1000)     1633 2023-10-13 11:41:59.000000 LstGen-0.6.3/lstgen/generators/golang/BigDecimal.go
--rw-r--r--   0 jenner    (1000) jenner    (1000)    11180 2022-10-17 11:19:47.000000 LstGen-0.6.3/lstgen/generators/golang/__init__.py
--rw-r--r--   0 jenner    (1000) jenner    (1000)     3827 2022-01-13 13:21:55.000000 LstGen-0.6.3/lstgen/generators/java.py
--rw-r--r--   0 jenner    (1000) jenner    (1000)     4795 2022-10-17 11:53:48.000000 LstGen-0.6.3/lstgen/generators/javascript.py
-drwxr-xr-x   0 jenner    (1000) jenner    (1000)        0 2023-10-13 11:44:44.180000 LstGen-0.6.3/lstgen/generators/php/
--rw-r--r--   0 jenner    (1000) jenner    (1000)     1801 2022-01-13 13:21:55.000000 LstGen-0.6.3/lstgen/generators/php/BigDecimal.php
--rw-r--r--   0 jenner    (1000) jenner    (1000)     8445 2022-01-13 13:21:55.000000 LstGen-0.6.3/lstgen/generators/php/__init__.py
-drwxr-xr-x   0 jenner    (1000) jenner    (1000)        0 2023-10-13 11:44:44.180000 LstGen-0.6.3/lstgen/generators/python/
--rw-r--r--   0 jenner    (1000) jenner    (1000)     6365 2022-10-17 11:46:39.000000 LstGen-0.6.3/lstgen/generators/python/__init__.py
--rw-r--r--   0 jenner    (1000) jenner    (1000)     1269 2022-01-13 13:21:55.000000 LstGen-0.6.3/lstgen/generators/python/bd.py
--rw-r--r--   0 jenner    (1000) jenner    (1000)     4539 2023-08-24 11:04:34.000000 LstGen-0.6.3/lstgen/pap.py
--rw-r--r--   0 jenner    (1000) jenner    (1000)      136 2023-10-13 11:44:44.180000 LstGen-0.6.3/setup.cfg
--rw-r--r--   0 jenner    (1000) jenner    (1000)     1561 2023-10-13 11:43:30.000000 LstGen-0.6.3/setup.py
--rw-r--r--   0 jenner    (1000) jenner    (1000)      828 2022-01-13 13:21:55.000000 LstGen-0.6.3/tox.ini
+drwxr-xr-x   0 jenner    (1000) jenner    (1000)        0 2024-04-02 11:24:21.454630 LstGen-0.6.4/
+-rw-r--r--   0 jenner    (1000) jenner    (1000)     1574 2024-04-02 11:19:10.000000 LstGen-0.6.4/CHANGES.md
+-rw-r--r--   0 jenner    (1000) jenner    (1000)     1077 2022-01-13 13:21:55.000000 LstGen-0.6.4/LICENSE
+drwxr-xr-x   0 jenner    (1000) jenner    (1000)        0 2024-04-02 11:24:21.454630 LstGen-0.6.4/LstGen.egg-info/
+-rw-r--r--   0 jenner    (1000) jenner    (1000)     7816 2024-04-02 11:24:21.000000 LstGen-0.6.4/LstGen.egg-info/PKG-INFO
+-rw-r--r--   0 jenner    (1000) jenner    (1000)      684 2024-04-02 11:24:21.000000 LstGen-0.6.4/LstGen.egg-info/SOURCES.txt
+-rw-r--r--   0 jenner    (1000) jenner    (1000)        1 2024-04-02 11:24:21.000000 LstGen-0.6.4/LstGen.egg-info/dependency_links.txt
+-rw-r--r--   0 jenner    (1000) jenner    (1000)       55 2024-04-02 11:24:21.000000 LstGen-0.6.4/LstGen.egg-info/entry_points.txt
+-rw-r--r--   0 jenner    (1000) jenner    (1000)        1 2022-01-13 13:23:17.000000 LstGen-0.6.4/LstGen.egg-info/not-zip-safe
+-rw-r--r--   0 jenner    (1000) jenner    (1000)       53 2024-04-02 11:24:21.000000 LstGen-0.6.4/LstGen.egg-info/requires.txt
+-rw-r--r--   0 jenner    (1000) jenner    (1000)        7 2024-04-02 11:24:21.000000 LstGen-0.6.4/LstGen.egg-info/top_level.txt
+-rw-r--r--   0 jenner    (1000) jenner    (1000)       79 2022-10-17 11:19:47.000000 LstGen-0.6.4/MANIFEST.in
+-rw-r--r--   0 jenner    (1000) jenner    (1000)     7816 2024-04-02 11:24:21.454630 LstGen-0.6.4/PKG-INFO
+-rw-r--r--   0 jenner    (1000) jenner    (1000)     5510 2022-10-17 12:12:20.000000 LstGen-0.6.4/README.md
+drwxr-xr-x   0 jenner    (1000) jenner    (1000)        0 2024-04-02 11:24:21.454630 LstGen-0.6.4/lstgen/
+-rw-r--r--   0 jenner    (1000) jenner    (1000)     9809 2022-01-13 13:21:55.000000 LstGen-0.6.4/lstgen/__init__.py
+-rw-r--r--   0 jenner    (1000) jenner    (1000)     5192 2022-10-17 11:59:58.000000 LstGen-0.6.4/lstgen/cli.py
+drwxr-xr-x   0 jenner    (1000) jenner    (1000)        0 2024-04-02 11:24:21.454630 LstGen-0.6.4/lstgen/generators/
+-rw-r--r--   0 jenner    (1000) jenner    (1000)      528 2022-10-17 12:01:11.000000 LstGen-0.6.4/lstgen/generators/__init__.py
+-rw-r--r--   0 jenner    (1000) jenner    (1000)     7708 2022-01-13 13:21:55.000000 LstGen-0.6.4/lstgen/generators/ast2code.py
+-rw-r--r--   0 jenner    (1000) jenner    (1000)     4874 2022-01-13 13:21:55.000000 LstGen-0.6.4/lstgen/generators/base.py
+drwxr-xr-x   0 jenner    (1000) jenner    (1000)        0 2024-04-02 11:24:21.454630 LstGen-0.6.4/lstgen/generators/golang/
+-rw-r--r--   0 jenner    (1000) jenner    (1000)     1633 2023-10-13 11:41:59.000000 LstGen-0.6.4/lstgen/generators/golang/BigDecimal.go
+-rw-r--r--   0 jenner    (1000) jenner    (1000)    11180 2022-10-17 11:19:47.000000 LstGen-0.6.4/lstgen/generators/golang/__init__.py
+-rw-r--r--   0 jenner    (1000) jenner    (1000)     3827 2022-01-13 13:21:55.000000 LstGen-0.6.4/lstgen/generators/java.py
+-rw-r--r--   0 jenner    (1000) jenner    (1000)     4795 2022-10-17 11:53:48.000000 LstGen-0.6.4/lstgen/generators/javascript.py
+drwxr-xr-x   0 jenner    (1000) jenner    (1000)        0 2024-04-02 11:24:21.454630 LstGen-0.6.4/lstgen/generators/php/
+-rw-r--r--   0 jenner    (1000) jenner    (1000)     1801 2022-01-13 13:21:55.000000 LstGen-0.6.4/lstgen/generators/php/BigDecimal.php
+-rw-r--r--   0 jenner    (1000) jenner    (1000)     8445 2022-01-13 13:21:55.000000 LstGen-0.6.4/lstgen/generators/php/__init__.py
+drwxr-xr-x   0 jenner    (1000) jenner    (1000)        0 2024-04-02 11:24:21.454630 LstGen-0.6.4/lstgen/generators/python/
+-rw-r--r--   0 jenner    (1000) jenner    (1000)     6365 2022-10-17 11:46:39.000000 LstGen-0.6.4/lstgen/generators/python/__init__.py
+-rw-r--r--   0 jenner    (1000) jenner    (1000)     1269 2022-01-13 13:21:55.000000 LstGen-0.6.4/lstgen/generators/python/bd.py
+-rw-r--r--   0 jenner    (1000) jenner    (1000)     4684 2024-04-02 11:17:48.000000 LstGen-0.6.4/lstgen/pap.py
+-rw-r--r--   0 jenner    (1000) jenner    (1000)      136 2024-04-02 11:24:21.454630 LstGen-0.6.4/setup.cfg
+-rw-r--r--   0 jenner    (1000) jenner    (1000)     1561 2024-04-02 11:19:20.000000 LstGen-0.6.4/setup.py
+-rw-r--r--   0 jenner    (1000) jenner    (1000)      828 2022-01-13 13:21:55.000000 LstGen-0.6.4/tox.ini
```

### Comparing `LstGen-0.6.3/CHANGES.md` & `LstGen-0.6.4/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # Changes
 
+## 0.6.4
+* Added 2024 PAP (thanks antonio-masotti)
+
 ## 0.6.3
 * Added fix for rounding in BigDecimal.SetScale for golang. (thanks Markus)
 
 ## 0.6.2
 * Added 2023 PAP from July
 
 ## 0.6.1
```

### Comparing `LstGen-0.6.3/LstGen.egg-info/SOURCES.txt` & `LstGen-0.6.4/LstGen.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 CHANGES.md
+LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 tox.ini
 LstGen.egg-info/PKG-INFO
 LstGen.egg-info/SOURCES.txt
```

### Comparing `LstGen-0.6.3/README.md` & `LstGen-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `LstGen-0.6.3/lstgen/__init__.py` & `LstGen-0.6.4/lstgen/__init__.py`

 * *Files identical despite different names*

### Comparing `LstGen-0.6.3/lstgen/cli.py` & `LstGen-0.6.4/lstgen/cli.py`

 * *Files identical despite different names*

### Comparing `LstGen-0.6.3/lstgen/generators/__init__.py` & `LstGen-0.6.4/lstgen/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `LstGen-0.6.3/lstgen/generators/ast2code.py` & `LstGen-0.6.4/lstgen/generators/ast2code.py`

 * *Files identical despite different names*

### Comparing `LstGen-0.6.3/lstgen/generators/base.py` & `LstGen-0.6.4/lstgen/generators/base.py`

 * *Files identical despite different names*

### Comparing `LstGen-0.6.3/lstgen/generators/golang/BigDecimal.go` & `LstGen-0.6.4/lstgen/generators/golang/BigDecimal.go`

 * *Files identical despite different names*

### Comparing `LstGen-0.6.3/lstgen/generators/golang/__init__.py` & `LstGen-0.6.4/lstgen/generators/golang/__init__.py`

 * *Files identical despite different names*

### Comparing `LstGen-0.6.3/lstgen/generators/java.py` & `LstGen-0.6.4/lstgen/generators/java.py`

 * *Files identical despite different names*

### Comparing `LstGen-0.6.3/lstgen/generators/javascript.py` & `LstGen-0.6.4/lstgen/generators/javascript.py`

 * *Files identical despite different names*

### Comparing `LstGen-0.6.3/lstgen/generators/php/BigDecimal.php` & `LstGen-0.6.4/lstgen/generators/php/BigDecimal.php`

 * *Files identical despite different names*

### Comparing `LstGen-0.6.3/lstgen/generators/php/__init__.py` & `LstGen-0.6.4/lstgen/generators/php/__init__.py`

 * *Files identical despite different names*

### Comparing `LstGen-0.6.3/lstgen/generators/python/__init__.py` & `LstGen-0.6.4/lstgen/generators/python/__init__.py`

 * *Files identical despite different names*

### Comparing `LstGen-0.6.3/lstgen/generators/python/bd.py` & `LstGen-0.6.4/lstgen/generators/python/bd.py`

 * *Files identical despite different names*

### Comparing `LstGen-0.6.3/lstgen/pap.py` & `LstGen-0.6.4/lstgen/pap.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,18 @@
         '/interface/2023Version1.xhtml',
         '/javax.faces.resource/daten/xmls/Lohnsteuer2023.xml.xhtml'
     )),
     ('2023_3', PapResource(
         '/interface/2023AbJuliVersion1.xhtml',
         '/javax.faces.resource/daten/xmls/Lohnsteuer2023AbJuli.xml.xhtml'
     )),
+    ('2024_1', PapResource(
+        '/interface/2024Version1.xhtml',
+        '/javax.faces.resource/daten/xmls/Lohnsteuer2024.xml.xhtml'
+    )),
 ))
 
 
 def get_pap_xml(pap_resource_name):
     """ Fetch PAP XML from bmf-steuerrechner.de and return
         it as a string.
     """
```

### Comparing `LstGen-0.6.3/setup.py` & `LstGen-0.6.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ]
 testing_extras = requires + [
     'nose',
     'coverage',
 ]
 
 setup(name='LstGen',
-    version='0.6.3',
+    version='0.6.4',
     description='LstGen',
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.4",
```

### Comparing `LstGen-0.6.3/tox.ini` & `LstGen-0.6.4/tox.ini`

 * *Files identical despite different names*

