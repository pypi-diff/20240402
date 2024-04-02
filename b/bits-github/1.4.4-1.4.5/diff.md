# Comparing `tmp/bits_github-1.4.4.tar.gz` & `tmp/bits_github-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bits_github-1.4.4.tar", max compression
+gzip compressed data, was "bits_github-1.4.5.tar", max compression
```

## Comparing `bits_github-1.4.4.tar` & `bits_github-1.4.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       45 2024-04-02 15:33:41.329796 bits_github-1.4.4/README.md
--rw-r--r--   0        0        0       65 2024-04-02 15:33:41.329796 bits_github-1.4.4/bits/__init__.py
--rw-r--r--   0        0        0    25792 2024-04-02 15:33:41.333796 bits_github-1.4.4/bits/github/__init__.py
--rw-r--r--   0        0        0     1800 2024-04-02 15:33:41.333796 bits_github-1.4.4/bits/github/app.py
--rw-r--r--   0        0        0    13646 2024-04-02 15:33:41.333796 bits_github-1.4.4/bits/github/auditlogs.py
--rw-r--r--   0        0        0    16434 2024-04-02 15:33:41.333796 bits_github-1.4.4/bits/github/client.py
--rw-r--r--   0        0        0     1899 2024-04-02 15:33:41.333796 bits_github-1.4.4/bits/github/datastore.py
--rw-r--r--   0        0        0    10143 2024-04-02 15:33:41.333796 bits_github-1.4.4/bits/github/firestore.py
--rw-r--r--   0        0        0     6904 2024-04-02 15:33:41.333796 bits_github-1.4.4/bits/github/helpers.py
--rw-r--r--   0        0        0     2719 2024-04-02 15:33:41.333796 bits_github-1.4.4/bits/github/sync.py
--rw-r--r--   0        0        0    24647 2024-04-02 15:33:41.333796 bits_github-1.4.4/bits/github/update.py
--rw-r--r--   0        0        0     1252 2024-04-02 15:33:41.333796 bits_github-1.4.4/pyproject.toml
--rw-r--r--   0        0        0      991 1970-01-01 00:00:00.000000 bits_github-1.4.4/PKG-INFO
+-rw-r--r--   0        0        0       45 2024-04-02 15:58:06.070414 bits_github-1.4.5/README.md
+-rw-r--r--   0        0        0       65 2024-04-02 15:58:06.070414 bits_github-1.4.5/bits/__init__.py
+-rw-r--r--   0        0        0    25797 2024-04-02 15:58:06.070414 bits_github-1.4.5/bits/github/__init__.py
+-rw-r--r--   0        0        0     1800 2024-04-02 15:58:06.070414 bits_github-1.4.5/bits/github/app.py
+-rw-r--r--   0        0        0    13646 2024-04-02 15:58:06.070414 bits_github-1.4.5/bits/github/auditlogs.py
+-rw-r--r--   0        0        0    16434 2024-04-02 15:58:06.070414 bits_github-1.4.5/bits/github/client.py
+-rw-r--r--   0        0        0     1899 2024-04-02 15:58:06.070414 bits_github-1.4.5/bits/github/datastore.py
+-rw-r--r--   0        0        0    10143 2024-04-02 15:58:06.070414 bits_github-1.4.5/bits/github/firestore.py
+-rw-r--r--   0        0        0     6904 2024-04-02 15:58:06.070414 bits_github-1.4.5/bits/github/helpers.py
+-rw-r--r--   0        0        0     2719 2024-04-02 15:58:06.070414 bits_github-1.4.5/bits/github/sync.py
+-rw-r--r--   0        0        0    24647 2024-04-02 15:58:06.070414 bits_github-1.4.5/bits/github/update.py
+-rw-r--r--   0        0        0     1252 2024-04-02 15:58:06.070414 bits_github-1.4.5/pyproject.toml
+-rw-r--r--   0        0        0      991 1970-01-01 00:00:00.000000 bits_github-1.4.5/PKG-INFO
```

### Comparing `bits_github-1.4.4/bits/github/__init__.py` & `bits_github-1.4.5/bits/github/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     CODE_OK = 204
     CODE_NOT_CHANGED = 304
     CODE_NOT_FOUND = 404
 
     def __init__(  # noqa: PLR0913
             self,
             token,
-            org,
+            org=None,
             org_id=None,
             owner_team=None,
             role_team=None,
             role_team_name=None,
             verbose=False,
             app_project=None,
     ):
```

### Comparing `bits_github-1.4.4/bits/github/app.py` & `bits_github-1.4.5/bits/github/app.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.4/bits/github/auditlogs.py` & `bits_github-1.4.5/bits/github/auditlogs.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.4/bits/github/client.py` & `bits_github-1.4.5/bits/github/client.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.4/bits/github/datastore.py` & `bits_github-1.4.5/bits/github/datastore.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.4/bits/github/firestore.py` & `bits_github-1.4.5/bits/github/firestore.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.4/bits/github/helpers.py` & `bits_github-1.4.5/bits/github/helpers.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.4/bits/github/sync.py` & `bits_github-1.4.5/bits/github/sync.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.4/bits/github/update.py` & `bits_github-1.4.5/bits/github/update.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.4/pyproject.toml` & `bits_github-1.4.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 license = "BSD-3-Clause"
 name = "bits-github"
 packages = [
     { include = "bits" },
 ]
 readme = "README.md"
 repository = "https://github.com/broadinstitute/bits-github.git"
-version = "1.4.4"
+version = "1.4.5"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12.1"  # Compatible python versions must be declared here
 
 bits-google = "^1.13.8"
 google-cloud-datastore = "^2.19.0"
 google-cloud-firestore = "^2.15.0"
```

### Comparing `bits_github-1.4.4/PKG-INFO` & `bits_github-1.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bits-github
-Version: 1.4.4
+Version: 1.4.5
 Summary: BITS GitHub Package for Python
 Home-page: https://github.com/broadinstitute/bits-github.git
 License: BSD-3-Clause
 Keywords: bits,github
 Author: Lukas Karlsson
 Author-email: karlsson@broadinstitute.org
 Requires-Python: >=3.9,<3.12.1
```

