# Comparing `tmp/trame-3.5.4.tar.gz` & `tmp/trame-3.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-3.5.4.tar", last modified: Thu Mar 21 15:10:39 2024, max compression
+gzip compressed data, was "trame-3.5.5.tar", last modified: Tue Apr  2 21:23:11 2024, max compression
```

## Comparing `trame-3.5.4.tar` & `trame-3.5.5.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 15:10:39.288133 trame-3.5.4/
--rw-r--r--   0 root         (0) root         (0)      552 2024-03-21 15:10:34.000000 trame-3.5.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-21 15:10:34.000000 trame-3.5.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7169 2024-03-21 15:10:39.288133 trame-3.5.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6431 2024-03-21 15:10:34.000000 trame-3.5.4/README.rst
--rw-r--r--   0 root         (0) root         (0)      922 2024-03-21 15:10:39.288133 trame-3.5.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-21 15:10:34.000000 trame-3.5.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 15:10:39.280133 trame-3.5.4/trame/
--rw-r--r--   0 root         (0) root         (0)      552 2024-03-21 15:10:34.000000 trame-3.5.4/trame/LICENSE
--rw-r--r--   0 root         (0) root         (0)       65 2024-03-21 15:10:34.000000 trame-3.5.4/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 15:10:39.284133 trame-3.5.4/trame/app/
--rw-r--r--   0 root         (0) root         (0)     3132 2024-03-21 15:10:34.000000 trame-3.5.4/trame/app/__init__.py
--rw-r--r--   0 root         (0) root         (0)      271 2024-03-21 15:10:34.000000 trame-3.5.4/trame/app/asynchronous.py
--rw-r--r--   0 root         (0) root         (0)     2089 2024-03-21 15:10:34.000000 trame-3.5.4/trame/app/demo.py
--rw-r--r--   0 root         (0) root         (0)     1490 2024-03-21 15:10:34.000000 trame-3.5.4/trame/app/dev.py
--rw-r--r--   0 root         (0) root         (0)     1731 2024-03-21 15:10:34.000000 trame-3.5.4/trame/app/file_upload.py
--rw-r--r--   0 root         (0) root         (0)     2320 2024-03-21 15:10:34.000000 trame-3.5.4/trame/app/jupyter.py
--rw-r--r--   0 root         (0) root         (0)     1309 2024-03-21 15:10:34.000000 trame-3.5.4/trame/app/mimetypes.py
--rw-r--r--   0 root         (0) root         (0)      577 2024-03-21 15:10:34.000000 trame-3.5.4/trame/app/singleton.py
--rw-r--r--   0 root         (0) root         (0)     1677 2024-03-21 15:10:34.000000 trame-3.5.4/trame/app/testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 15:10:39.284133 trame-3.5.4/trame/assets/
--rw-r--r--   0 root         (0) root         (0)       65 2024-03-21 15:10:34.000000 trame-3.5.4/trame/assets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4337 2024-03-21 15:10:34.000000 trame-3.5.4/trame/assets/local.py
--rw-r--r--   0 root         (0) root         (0)     4362 2024-03-21 15:10:34.000000 trame-3.5.4/trame/assets/remote.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 15:10:39.284133 trame-3.5.4/trame/decorators/
--rw-r--r--   0 root         (0) root         (0)      184 2024-03-21 15:10:34.000000 trame-3.5.4/trame/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)       86 2024-03-21 15:10:34.000000 trame-3.5.4/trame/decorators/dev.py
--rw-r--r--   0 root         (0) root         (0)     5665 2024-03-21 15:10:34.000000 trame-3.5.4/trame/decorators/klass.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 15:10:39.284133 trame-3.5.4/trame/env/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-21 15:10:34.000000 trame-3.5.4/trame/env/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1863 2024-03-21 15:10:34.000000 trame-3.5.4/trame/env/paraview.py
--rw-r--r--   0 root         (0) root         (0)     3930 2024-03-21 15:10:34.000000 trame-3.5.4/trame/env/utils.py
--rw-r--r--   0 root         (0) root         (0)     1311 2024-03-21 15:10:34.000000 trame-3.5.4/trame/env/venv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 15:10:39.288133 trame-3.5.4/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2024-03-21 15:10:34.000000 trame-3.5.4/trame/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 15:10:39.288133 trame-3.5.4/trame/tools/
--rw-r--r--   0 root         (0) root         (0)       65 2024-03-21 15:10:34.000000 trame-3.5.4/trame/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1417 2024-03-21 15:10:34.000000 trame-3.5.4/trame/tools/app.py
--rw-r--r--   0 root         (0) root         (0)     4461 2024-03-21 15:10:34.000000 trame-3.5.4/trame/tools/serve.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 15:10:39.288133 trame-3.5.4/trame/tools/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-21 15:10:34.000000 trame-3.5.4/trame/tools/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      597 2024-03-21 15:10:34.000000 trame-3.5.4/trame/tools/widgets/__main__.py
--rw-r--r--   0 root         (0) root         (0)    13960 2024-03-21 15:10:34.000000 trame-3.5.4/trame/tools/widgets/generator.py
--rw-r--r--   0 root         (0) root         (0)      603 2024-03-21 15:10:34.000000 trame-3.5.4/trame/tools/widgets/utils.py
--rw-r--r--   0 root         (0) root         (0)     3071 2024-03-21 15:10:34.000000 trame-3.5.4/trame/tools/www.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 15:10:39.288133 trame-3.5.4/trame/ui/
--rw-r--r--   0 root         (0) root         (0)       65 2024-03-21 15:10:34.000000 trame-3.5.4/trame/ui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 15:10:39.288133 trame-3.5.4/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2024-03-21 15:10:34.000000 trame-3.5.4/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      934 2024-03-21 15:10:34.000000 trame-3.5.4/trame/widgets/helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 15:10:39.284133 trame-3.5.4/trame.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7169 2024-03-21 15:10:39.000000 trame-3.5.4/trame.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      957 2024-03-21 15:10:39.000000 trame-3.5.4/trame.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-21 15:10:39.000000 trame-3.5.4/trame.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2024-03-21 15:10:39.000000 trame-3.5.4/trame.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-03-21 15:10:39.000000 trame-3.5.4/trame.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 21:23:11.127314 trame-3.5.5/
+-rw-r--r--   0 root         (0) root         (0)      552 2024-04-02 21:23:07.000000 trame-3.5.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 21:23:07.000000 trame-3.5.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7169 2024-04-02 21:23:11.127314 trame-3.5.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6431 2024-04-02 21:23:07.000000 trame-3.5.5/README.rst
+-rw-r--r--   0 root         (0) root         (0)      928 2024-04-02 21:23:11.127314 trame-3.5.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 21:23:07.000000 trame-3.5.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 21:23:11.119315 trame-3.5.5/trame/
+-rw-r--r--   0 root         (0) root         (0)      552 2024-04-02 21:23:07.000000 trame-3.5.5/trame/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-02 21:23:07.000000 trame-3.5.5/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 21:23:11.123314 trame-3.5.5/trame/app/
+-rw-r--r--   0 root         (0) root         (0)     3132 2024-04-02 21:23:07.000000 trame-3.5.5/trame/app/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      271 2024-04-02 21:23:07.000000 trame-3.5.5/trame/app/asynchronous.py
+-rw-r--r--   0 root         (0) root         (0)     2089 2024-04-02 21:23:07.000000 trame-3.5.5/trame/app/demo.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2024-04-02 21:23:07.000000 trame-3.5.5/trame/app/dev.py
+-rw-r--r--   0 root         (0) root         (0)     1731 2024-04-02 21:23:07.000000 trame-3.5.5/trame/app/file_upload.py
+-rw-r--r--   0 root         (0) root         (0)     2320 2024-04-02 21:23:07.000000 trame-3.5.5/trame/app/jupyter.py
+-rw-r--r--   0 root         (0) root         (0)     1309 2024-04-02 21:23:07.000000 trame-3.5.5/trame/app/mimetypes.py
+-rw-r--r--   0 root         (0) root         (0)      577 2024-04-02 21:23:07.000000 trame-3.5.5/trame/app/singleton.py
+-rw-r--r--   0 root         (0) root         (0)     1677 2024-04-02 21:23:07.000000 trame-3.5.5/trame/app/testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 21:23:11.123314 trame-3.5.5/trame/assets/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-02 21:23:07.000000 trame-3.5.5/trame/assets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4337 2024-04-02 21:23:07.000000 trame-3.5.5/trame/assets/local.py
+-rw-r--r--   0 root         (0) root         (0)     4362 2024-04-02 21:23:07.000000 trame-3.5.5/trame/assets/remote.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 21:23:11.123314 trame-3.5.5/trame/decorators/
+-rw-r--r--   0 root         (0) root         (0)      184 2024-04-02 21:23:07.000000 trame-3.5.5/trame/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       86 2024-04-02 21:23:07.000000 trame-3.5.5/trame/decorators/dev.py
+-rw-r--r--   0 root         (0) root         (0)     5665 2024-04-02 21:23:07.000000 trame-3.5.5/trame/decorators/klass.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 21:23:11.127314 trame-3.5.5/trame/env/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 21:23:07.000000 trame-3.5.5/trame/env/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2024-04-02 21:23:07.000000 trame-3.5.5/trame/env/paraview.py
+-rw-r--r--   0 root         (0) root         (0)     3930 2024-04-02 21:23:07.000000 trame-3.5.5/trame/env/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1311 2024-04-02 21:23:07.000000 trame-3.5.5/trame/env/venv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 21:23:11.127314 trame-3.5.5/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-02 21:23:07.000000 trame-3.5.5/trame/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 21:23:11.127314 trame-3.5.5/trame/tools/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-02 21:23:07.000000 trame-3.5.5/trame/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1417 2024-04-02 21:23:07.000000 trame-3.5.5/trame/tools/app.py
+-rw-r--r--   0 root         (0) root         (0)     4461 2024-04-02 21:23:07.000000 trame-3.5.5/trame/tools/serve.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 21:23:11.127314 trame-3.5.5/trame/tools/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 21:23:07.000000 trame-3.5.5/trame/tools/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      597 2024-04-02 21:23:07.000000 trame-3.5.5/trame/tools/widgets/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    13960 2024-04-02 21:23:07.000000 trame-3.5.5/trame/tools/widgets/generator.py
+-rw-r--r--   0 root         (0) root         (0)      603 2024-04-02 21:23:07.000000 trame-3.5.5/trame/tools/widgets/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3071 2024-04-02 21:23:07.000000 trame-3.5.5/trame/tools/www.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 21:23:11.127314 trame-3.5.5/trame/ui/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-02 21:23:07.000000 trame-3.5.5/trame/ui/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 21:23:11.127314 trame-3.5.5/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-02 21:23:07.000000 trame-3.5.5/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      934 2024-04-02 21:23:07.000000 trame-3.5.5/trame/widgets/helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 21:23:11.123314 trame-3.5.5/trame.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7169 2024-04-02 21:23:11.000000 trame-3.5.5/trame.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      957 2024-04-02 21:23:11.000000 trame-3.5.5/trame.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 21:23:11.000000 trame-3.5.5/trame.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2024-04-02 21:23:11.000000 trame-3.5.5/trame.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-02 21:23:11.000000 trame-3.5.5/trame.egg-info/top_level.txt
```

### Comparing `trame-3.5.4/LICENSE` & `trame-3.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-3.5.4/PKG-INFO` & `trame-3.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame
-Version: 3.5.4
+Version: 3.5.5
 Summary: Trame, a framework to build applications in plain Python
 Author: Kitware Inc.
 License: Apache License 2.0
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-3.5.4/README.rst` & `trame-3.5.5/README.rst`

 * *Files identical despite different names*

### Comparing `trame-3.5.4/setup.cfg` & `trame-3.5.5/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame
-version = 3.5.4
+version = 3.5.5
 description = Trame, a framework to build applications in plain Python
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = Apache License 2.0
 classifiers = 
 	Development Status :: 5 - Production/Stable
@@ -22,16 +22,16 @@
 	Application
 	Framework
 
 [options]
 packages = find:
 include_package_data = True
 install_requires = 
-	trame-server>=2.13.1
-	trame-client>=2.14.0
+	trame-server>=2.13.1,<3
+	trame-client>=2.14.0,<3
 
 [semantic_release]
 version_pattern = setup.cfg:version = (\d+\.\d+\.\d+)
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `trame-3.5.4/trame/LICENSE` & `trame-3.5.5/trame/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-3.5.4/trame/app/__init__.py` & `trame-3.5.5/trame/app/__init__.py`

 * *Files identical despite different names*

### Comparing `trame-3.5.4/trame/app/demo.py` & `trame-3.5.5/trame/app/demo.py`

 * *Files identical despite different names*

### Comparing `trame-3.5.4/trame/app/dev.py` & `trame-3.5.5/trame/app/dev.py`

 * *Files identical despite different names*

### Comparing `trame-3.5.4/trame/app/file_upload.py` & `trame-3.5.5/trame/app/file_upload.py`

 * *Files identical despite different names*

### Comparing `trame-3.5.4/trame/app/jupyter.py` & `trame-3.5.5/trame/app/jupyter.py`

 * *Files identical despite different names*

### Comparing `trame-3.5.4/trame/app/mimetypes.py` & `trame-3.5.5/trame/app/mimetypes.py`

 * *Files identical despite different names*

### Comparing `trame-3.5.4/trame/app/singleton.py` & `trame-3.5.5/trame/app/singleton.py`

 * *Files identical despite different names*

### Comparing `trame-3.5.4/trame/app/testing.py` & `trame-3.5.5/trame/app/testing.py`

 * *Files identical despite different names*

### Comparing `trame-3.5.4/trame/assets/local.py` & `trame-3.5.5/trame/assets/local.py`

 * *Files identical despite different names*

### Comparing `trame-3.5.4/trame/assets/remote.py` & `trame-3.5.5/trame/assets/remote.py`

 * *Files identical despite different names*

### Comparing `trame-3.5.4/trame/decorators/klass.py` & `trame-3.5.5/trame/decorators/klass.py`

 * *Files identical despite different names*

### Comparing `trame-3.5.4/trame/env/paraview.py` & `trame-3.5.5/trame/env/paraview.py`

 * *Files identical despite different names*

### Comparing `trame-3.5.4/trame/env/utils.py` & `trame-3.5.5/trame/env/utils.py`

 * *Files identical despite different names*

### Comparing `trame-3.5.4/trame/env/venv.py` & `trame-3.5.5/trame/env/venv.py`

 * *Files identical despite different names*

### Comparing `trame-3.5.4/trame/tools/app.py` & `trame-3.5.5/trame/tools/app.py`

 * *Files identical despite different names*

### Comparing `trame-3.5.4/trame/tools/serve.py` & `trame-3.5.5/trame/tools/serve.py`

 * *Files identical despite different names*

### Comparing `trame-3.5.4/trame/tools/widgets/__main__.py` & `trame-3.5.5/trame/tools/widgets/__main__.py`

 * *Files identical despite different names*

### Comparing `trame-3.5.4/trame/tools/widgets/generator.py` & `trame-3.5.5/trame/tools/widgets/generator.py`

 * *Files identical despite different names*

### Comparing `trame-3.5.4/trame/tools/widgets/utils.py` & `trame-3.5.5/trame/tools/widgets/utils.py`

 * *Files identical despite different names*

### Comparing `trame-3.5.4/trame/tools/www.py` & `trame-3.5.5/trame/tools/www.py`

 * *Files identical despite different names*

### Comparing `trame-3.5.4/trame/widgets/helper.py` & `trame-3.5.5/trame/widgets/helper.py`

 * *Files identical despite different names*

### Comparing `trame-3.5.4/trame.egg-info/PKG-INFO` & `trame-3.5.5/trame.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame
-Version: 3.5.4
+Version: 3.5.5
 Summary: Trame, a framework to build applications in plain Python
 Author: Kitware Inc.
 License: Apache License 2.0
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-3.5.4/trame.egg-info/SOURCES.txt` & `trame-3.5.5/trame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

