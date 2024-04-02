# Comparing `tmp/redocmx-0.0.1.tar.gz` & `tmp/redocmx-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redocmx-0.0.1.tar", last modified: Sat Mar 23 16:31:46 2024, max compression
+gzip compressed data, was "redocmx-0.0.2.tar", last modified: Tue Apr  2 20:29:07 2024, max compression
```

## Comparing `redocmx-0.0.1.tar` & `redocmx-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:31:46.923420 redocmx-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-23 16:31:38.000000 redocmx-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-03-23 16:31:46.923420 redocmx-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-03-23 16:31:38.000000 redocmx-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:31:46.923420 redocmx-0.0.1/redocmx/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-23 16:31:38.000000 redocmx-0.0.1/redocmx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-03-23 16:31:38.000000 redocmx-0.0.1/redocmx/cfdi.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-23 16:31:38.000000 redocmx-0.0.1/redocmx/pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-23 16:31:38.000000 redocmx-0.0.1/redocmx/redoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-03-23 16:31:38.000000 redocmx-0.0.1/redocmx/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:31:46.923420 redocmx-0.0.1/redocmx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-03-23 16:31:46.000000 redocmx-0.0.1/redocmx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-23 16:31:46.000000 redocmx-0.0.1/redocmx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 16:31:46.000000 redocmx-0.0.1/redocmx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-23 16:31:46.000000 redocmx-0.0.1/redocmx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-23 16:31:46.000000 redocmx-0.0.1/redocmx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-23 16:31:46.923420 redocmx-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-23 16:31:38.000000 redocmx-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:29:07.155188 redocmx-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-02 20:28:58.000000 redocmx-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-04-02 20:29:07.155188 redocmx-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-04-02 20:28:58.000000 redocmx-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:29:07.151188 redocmx-0.0.2/redocmx/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-02 20:28:58.000000 redocmx-0.0.2/redocmx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-02 20:28:58.000000 redocmx-0.0.2/redocmx/addenda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-02 20:28:58.000000 redocmx-0.0.2/redocmx/cfdi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-02 20:28:58.000000 redocmx-0.0.2/redocmx/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 20:28:58.000000 redocmx-0.0.2/redocmx/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-02 20:28:58.000000 redocmx-0.0.2/redocmx/redoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-02 20:28:58.000000 redocmx-0.0.2/redocmx/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:29:07.155188 redocmx-0.0.2/redocmx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-04-02 20:29:07.000000 redocmx-0.0.2/redocmx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-02 20:29:07.000000 redocmx-0.0.2/redocmx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 20:29:07.000000 redocmx-0.0.2/redocmx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 20:29:07.000000 redocmx-0.0.2/redocmx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 20:29:07.000000 redocmx-0.0.2/redocmx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 20:29:07.155188 redocmx-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-02 20:28:58.000000 redocmx-0.0.2/setup.py
```

### Comparing `redocmx-0.0.1/LICENSE` & `redocmx-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `redocmx-0.0.1/PKG-INFO` & `redocmx-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redocmx
-Version: 0.0.1
+Version: 0.0.2
 Summary: Conversión CFDI a PDF
 Home-page: https://github.com/redocmx/client-python
 Author: redoc.mx
 Author-email: soporte@redoc.mx
 License: MIT
 Keywords: cfdi a pdf,cfdi,cfdi to pdf,conversión cfdi a pdf,sat mexico,mexico
 Classifier: Programming Language :: Python :: 3
```

### Comparing `redocmx-0.0.1/README.md` & `redocmx-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `redocmx-0.0.1/redocmx/cfdi.py` & `redocmx-0.0.2/redocmx/cfdi.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,42 @@
 from .pdf import Pdf
 from .service import Service
-from pathlib import Path
+from .file import File
+from .addenda import Addenda
 
-class Cfdi:
+class Cfdi(File):
     def __init__(self):
+        super().__init__()
         self.pdf = None
         self.addenda = None
-        self.file_path = None
-        self.file_content = None
+        self.addenda_replace_values = None
         self.service = Service.get_instance()
 
-    def from_file(self, file_path):
-        self.file_path = file_path
-        return self
-
-    def from_string(self, file_content):
-        self.file_content = file_content
-        return self
+    def set_addenda(self, addenda, replace_values=None):
+        if addenda and not isinstance(addenda, Addenda):
+            raise TypeError('addenda must be an instance of Addenda.')
+        if replace_values and not isinstance(replace_values, dict):
+            raise TypeError('Addenda replace values must be a valid key-value object.')
+
+        self.addenda = addenda
+        self.addenda_replace_values = replace_values
 
     def to_pdf(self, payload={}):
         if self.pdf:
             return self.pdf
+        
+        if not isinstance(payload, dict):
+            raise TypeError('toPdf function only accepts an object as a parameter.')
 
-        file_content = self._get_xml_content()
-        payload['format'] = 'pdf'
+        file = self.get_file()
 
         if self.addenda:
-            payload['addenda'] = self.addenda
+            addenda_content = self.addenda.get_file_content(self.addenda_replace_values)
+            payload['addenda'] = addenda_content
 
-        result = self.service.cfdis_convert(file_content, payload)
+        payload['format'] = 'pdf'
+
+        result = self.service.cfdis_convert(file['content'], payload)
         self.pdf = Pdf(result)
 
         return self.pdf
 
-    def _get_xml_content(self):
-        if self.file_content:
-            return self.file_content
-        elif self.file_path:
-            path = Path(self.file_path)
-            if not path.exists() or not path.is_file():
-                raise FileNotFoundError(f"Failed to read XML content from file: {self.file_path}. The file does not exist.")
-            return path.read_text()
-        else:
-            raise ValueError("XML content for the CFDI must be provided.")
-
-    def set_addenda(self, addenda):
-        if not isinstance(addenda, str):
-            raise TypeError("setAddenda function only accepts a string parameter.")
-        self.addenda = addenda
```

### Comparing `redocmx-0.0.1/redocmx/pdf.py` & `redocmx-0.0.2/redocmx/pdf.py`

 * *Files identical despite different names*

### Comparing `redocmx-0.0.1/redocmx/service.py` & `redocmx-0.0.2/redocmx/service.py`

 * *Files identical despite different names*

### Comparing `redocmx-0.0.1/redocmx.egg-info/PKG-INFO` & `redocmx-0.0.2/redocmx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redocmx
-Version: 0.0.1
+Version: 0.0.2
 Summary: Conversión CFDI a PDF
 Home-page: https://github.com/redocmx/client-python
 Author: redoc.mx
 Author-email: soporte@redoc.mx
 License: MIT
 Keywords: cfdi a pdf,cfdi,cfdi to pdf,conversión cfdi a pdf,sat mexico,mexico
 Classifier: Programming Language :: Python :: 3
```

### Comparing `redocmx-0.0.1/setup.py` & `redocmx-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='redocmx',
-    version='0.0.1',
+    version='0.0.2',
     author='redoc.mx',
     author_email='soporte@redoc.mx',
     packages=find_packages(),
     install_requires=[
         'requests'
     ],
     description='Conversión CFDI a PDF',
```

