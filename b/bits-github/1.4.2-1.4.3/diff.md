# Comparing `tmp/bits_github-1.4.2.tar.gz` & `tmp/bits_github-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bits_github-1.4.2.tar", max compression
+gzip compressed data, was "bits_github-1.4.3.tar", max compression
```

## Comparing `bits_github-1.4.2.tar` & `bits_github-1.4.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       45 2024-04-01 21:43:01.646447 bits_github-1.4.2/README.md
--rw-r--r--   0        0        0       65 2024-04-01 21:43:01.646447 bits_github-1.4.2/bits/__init__.py
--rw-r--r--   0        0        0    25773 2024-04-01 21:43:01.646447 bits_github-1.4.2/bits/github/__init__.py
--rw-r--r--   0        0        0     1800 2024-04-01 21:43:01.646447 bits_github-1.4.2/bits/github/app.py
--rw-r--r--   0        0        0    13646 2024-04-01 21:43:01.646447 bits_github-1.4.2/bits/github/auditlogs.py
--rw-r--r--   0        0        0    16434 2024-04-01 21:43:01.646447 bits_github-1.4.2/bits/github/client.py
--rw-r--r--   0        0        0     1899 2024-04-01 21:43:01.646447 bits_github-1.4.2/bits/github/datastore.py
--rw-r--r--   0        0        0    10143 2024-04-01 21:43:01.646447 bits_github-1.4.2/bits/github/firestore.py
--rw-r--r--   0        0        0     6904 2024-04-01 21:43:01.646447 bits_github-1.4.2/bits/github/helpers.py
--rw-r--r--   0        0        0     2719 2024-04-01 21:43:01.646447 bits_github-1.4.2/bits/github/sync.py
--rw-r--r--   0        0        0    24647 2024-04-01 21:43:01.646447 bits_github-1.4.2/bits/github/update.py
--rw-r--r--   0        0        0     1201 2024-04-01 21:43:01.646447 bits_github-1.4.2/pyproject.toml
--rw-r--r--   0        0        0     1108 1970-01-01 00:00:00.000000 bits_github-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0       45 2024-04-01 21:51:22.552290 bits_github-1.4.3/README.md
+-rw-r--r--   0        0        0       65 2024-04-01 21:51:22.552290 bits_github-1.4.3/bits/__init__.py
+-rw-r--r--   0        0        0    25774 2024-04-01 21:51:22.552290 bits_github-1.4.3/bits/github/__init__.py
+-rw-r--r--   0        0        0     1800 2024-04-01 21:51:22.552290 bits_github-1.4.3/bits/github/app.py
+-rw-r--r--   0        0        0    13646 2024-04-01 21:51:22.556290 bits_github-1.4.3/bits/github/auditlogs.py
+-rw-r--r--   0        0        0    16434 2024-04-01 21:51:22.556290 bits_github-1.4.3/bits/github/client.py
+-rw-r--r--   0        0        0     1899 2024-04-01 21:51:22.556290 bits_github-1.4.3/bits/github/datastore.py
+-rw-r--r--   0        0        0    10143 2024-04-01 21:51:22.556290 bits_github-1.4.3/bits/github/firestore.py
+-rw-r--r--   0        0        0     6904 2024-04-01 21:51:22.556290 bits_github-1.4.3/bits/github/helpers.py
+-rw-r--r--   0        0        0     2719 2024-04-01 21:51:22.556290 bits_github-1.4.3/bits/github/sync.py
+-rw-r--r--   0        0        0    24647 2024-04-01 21:51:22.556290 bits_github-1.4.3/bits/github/update.py
+-rw-r--r--   0        0        0     1201 2024-04-01 21:51:22.556290 bits_github-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0     1108 1970-01-01 00:00:00.000000 bits_github-1.4.3/PKG-INFO
```

### Comparing `bits_github-1.4.2/bits/github/__init__.py` & `bits_github-1.4.3/bits/github/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,18 @@
             role_team_name=None,
             verbose=False,
             app_project=None,
     ):
         """Initialize an GitHub class instance."""
         # set the base url
         self.base_url = "https://api.github.com"
+
+        # set the headers for authorized requests
+        self.headers = {"Authorization": f"token {self.token}"}
+
         # set github token
         self.token = token
 
         # set github organization name
         self.org = org
         self.org_id = org_id
         if org and not org_id:
@@ -46,17 +50,14 @@
         # enable verbosity
         self.verbose = verbose
 
         # set the other urls
         self.org_base_url = f"{self.base_url}/orgs/{self.org}"
         self.org_id_base_url = f"{self.base_url}/organizations/{self.org_id}"
 
-        # set the headers for authorized requests
-        self.headers = {"Authorization": f"token {self.token}"}
-
         self.app_project = app_project
 
     #
     # Sub Classes
     #
     def app(self, auth=None):
         """Return an App instance."""
```

### Comparing `bits_github-1.4.2/bits/github/app.py` & `bits_github-1.4.3/bits/github/app.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.2/bits/github/auditlogs.py` & `bits_github-1.4.3/bits/github/auditlogs.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.2/bits/github/client.py` & `bits_github-1.4.3/bits/github/client.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.2/bits/github/datastore.py` & `bits_github-1.4.3/bits/github/datastore.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.2/bits/github/firestore.py` & `bits_github-1.4.3/bits/github/firestore.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.2/bits/github/helpers.py` & `bits_github-1.4.3/bits/github/helpers.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.2/bits/github/sync.py` & `bits_github-1.4.3/bits/github/sync.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.2/bits/github/update.py` & `bits_github-1.4.3/bits/github/update.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.2/pyproject.toml` & `bits_github-1.4.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 license = "BSD-3-Clause"
 name = "bits-github"
 packages = [
     { include = "bits" },
 ]
 readme = "README.md"
 repository = "https://github.com/broadinstitute/bits-github.git"
-version = "1.4.2"
+version = "1.4.3"
 
 [tool.poetry.dependencies]
 python = "^3.9"  # Compatible python versions must be declared here
 
 bits-google = "^1.13.8"
 google-cloud-datastore = "^2.19.0"
 google-cloud-firestore = "^2.15.0"
```

### Comparing `bits_github-1.4.2/PKG-INFO` & `bits_github-1.4.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bits-github
-Version: 1.4.2
+Version: 1.4.3
 Summary: BITS GitHub Package for Python
 Home-page: https://github.com/broadinstitute/bits-github.git
 License: BSD-3-Clause
 Keywords: bits,github
 Author: Lukas Karlsson
 Author-email: karlsson@broadinstitute.org
 Requires-Python: >=3.9,<4.0
```

