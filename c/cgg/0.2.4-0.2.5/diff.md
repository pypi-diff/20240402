# Comparing `tmp/cgg-0.2.4.tar.gz` & `tmp/cgg-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgg-0.2.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cgg-0.2.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cgg-0.2.4.tar` & `cgg-0.2.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1095 2024-01-21 23:59:42.278418 cgg-0.2.4/LICENSE
--rw-r--r--   0        0        0     3808 2024-03-07 01:00:59.889331 cgg-0.2.4/README.md
--rw-r--r--   0        0        0      742 2024-03-16 00:59:38.709223 cgg-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     7152 2024-03-16 01:03:41.861909 cgg-0.2.4/src/cgg/__init__.py
--rw-r--r--   0        0        0     4250 1970-01-01 00:00:00.000000 cgg-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-01-21 23:59:42.278418 cgg-0.2.5/LICENSE
+-rw-r--r--   0        0        0     3808 2024-04-01 23:24:44.183118 cgg-0.2.5/README.md
+-rw-r--r--   0        0        0      742 2024-03-16 00:59:38.709223 cgg-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     4922 2024-04-01 23:24:17.137439 cgg-0.2.5/src/cgg/__init__.py
+-rw-r--r--   0        0        0     4250 1970-01-01 00:00:00.000000 cgg-0.2.5/PKG-INFO
```

### Comparing `cgg-0.2.4/LICENSE` & `cgg-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cgg-0.2.4/README.md` & `cgg-0.2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -111,9 +111,9 @@
 ```
 cgg pp
 ```
 
 #### website
 Click [gguf.us](https://gguf.us) or launch it straight from console by:
 ```
-cgg go
+cgg us
 ```
```

### Comparing `cgg-0.2.4/pyproject.toml` & `cgg-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cgg-0.2.4/PKG-INFO` & `cgg-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgg
-Version: 0.2.4
+Version: 0.2.5
 Summary: cgg is a short form of call gguf model/file; cgg is a cmd-based app built on gguf-connector, which allows users interacting with large language model (i.e., chatgpt) via a simple command without coding a long long syntax
 Author-email: calcuis <info@calcu.io>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: gguf-connector >=0.7.22
 Project-URL: Homepage, https://github.com/calcuis/cgg
 Project-URL: Issues, https://github.com/calcuis/cgg/issues
@@ -122,9 +122,9 @@
 ```
 cgg pp
 ```
 
 #### website
 Click [gguf.us](https://gguf.us) or launch it straight from console by:
 ```
-cgg go
+cgg us
 ```
```

