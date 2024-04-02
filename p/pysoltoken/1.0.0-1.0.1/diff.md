# Comparing `tmp/pysoltoken-1.0.0.tar.gz` & `tmp/pysoltoken-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysoltoken-1.0.0.tar", last modified: Tue Apr  2 04:46:41 2024, max compression
+gzip compressed data, was "pysoltoken-1.0.1.tar", last modified: Tue Apr  2 04:50:35 2024, max compression
```

## Comparing `pysoltoken-1.0.0.tar` & `pysoltoken-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 04:46:41.972780 pysoltoken-1.0.0/
--rw-rw-rw-   0        0        0     1091 2024-04-02 03:41:34.000000 pysoltoken-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      558 2024-04-02 04:46:41.970781 pysoltoken-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      174 2024-04-02 03:41:20.000000 pysoltoken-1.0.0/README.md
--rw-rw-rw-   0        0        0      517 2024-04-02 04:46:14.000000 pysoltoken-1.0.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-02 04:46:41.960781 pysoltoken-1.0.0/pysoltoken/
--rw-rw-rw-   0        0        0        0 2024-04-02 03:37:44.000000 pysoltoken-1.0.0/pysoltoken/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-02 03:38:05.000000 pysoltoken-1.0.0/pysoltoken/example.py
-drwxrwxrwx   0        0        0        0 2024-04-02 04:46:41.969781 pysoltoken-1.0.0/pysoltoken.egg-info/
--rw-rw-rw-   0        0        0      558 2024-04-02 04:46:41.000000 pysoltoken-1.0.0/pysoltoken.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2024-04-02 04:46:41.000000 pysoltoken-1.0.0/pysoltoken.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 04:46:41.000000 pysoltoken-1.0.0/pysoltoken.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-02 04:46:41.000000 pysoltoken-1.0.0/pysoltoken.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 04:46:41.973781 pysoltoken-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-02 04:50:35.488991 pysoltoken-1.0.1/
+-rw-rw-rw-   0        0        0     1091 2024-04-02 03:41:34.000000 pysoltoken-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      558 2024-04-02 04:50:35.486991 pysoltoken-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2024-04-02 03:41:20.000000 pysoltoken-1.0.1/README.md
+-rw-rw-rw-   0        0        0      517 2024-04-02 04:50:19.000000 pysoltoken-1.0.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-02 04:50:35.475991 pysoltoken-1.0.1/pysoltoken/
+-rw-rw-rw-   0        0        0        0 2024-04-02 03:37:44.000000 pysoltoken-1.0.1/pysoltoken/__init__.py
+-rw-rw-rw-   0        0        0    29184 2024-04-02 04:09:14.000000 pysoltoken-1.0.1/pysoltoken/client.py
+-rw-rw-rw-   0        0        0    26290 2024-04-02 04:10:28.000000 pysoltoken-1.0.1/pysoltoken/core.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:50:35.484992 pysoltoken-1.0.1/pysoltoken.egg-info/
+-rw-rw-rw-   0        0        0      558 2024-04-02 04:50:35.000000 pysoltoken-1.0.1/pysoltoken.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2024-04-02 04:50:35.000000 pysoltoken-1.0.1/pysoltoken.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 04:50:35.000000 pysoltoken-1.0.1/pysoltoken.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-02 04:50:35.000000 pysoltoken-1.0.1/pysoltoken.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 04:50:35.488991 pysoltoken-1.0.1/setup.cfg
```

### Comparing `pysoltoken-1.0.0/LICENSE` & `pysoltoken-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysoltoken-1.0.0/PKG-INFO` & `pysoltoken-1.0.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysoltoken
-Version: 1.0.0
+Version: 1.0.1
 Summary: A small example package
 Author-email: solana_dev <solana_client@proton.me>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pysoltoken-1.0.0/pyproject.toml` & `pysoltoken-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pysoltoken"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="solana_dev", email="solana_client@proton.me" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pysoltoken-1.0.0/pysoltoken.egg-info/PKG-INFO` & `pysoltoken-1.0.1/pysoltoken.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysoltoken
-Version: 1.0.0
+Version: 1.0.1
 Summary: A small example package
 Author-email: solana_dev <solana_client@proton.me>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

