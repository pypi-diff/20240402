# Comparing `tmp/bits_github-1.4.3.tar.gz` & `tmp/bits_github-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bits_github-1.4.3.tar", max compression
+gzip compressed data, was "bits_github-1.4.4.tar", max compression
```

## Comparing `bits_github-1.4.3.tar` & `bits_github-1.4.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       45 2024-04-01 21:51:22.552290 bits_github-1.4.3/README.md
--rw-r--r--   0        0        0       65 2024-04-01 21:51:22.552290 bits_github-1.4.3/bits/__init__.py
--rw-r--r--   0        0        0    25774 2024-04-01 21:51:22.552290 bits_github-1.4.3/bits/github/__init__.py
--rw-r--r--   0        0        0     1800 2024-04-01 21:51:22.552290 bits_github-1.4.3/bits/github/app.py
--rw-r--r--   0        0        0    13646 2024-04-01 21:51:22.556290 bits_github-1.4.3/bits/github/auditlogs.py
--rw-r--r--   0        0        0    16434 2024-04-01 21:51:22.556290 bits_github-1.4.3/bits/github/client.py
--rw-r--r--   0        0        0     1899 2024-04-01 21:51:22.556290 bits_github-1.4.3/bits/github/datastore.py
--rw-r--r--   0        0        0    10143 2024-04-01 21:51:22.556290 bits_github-1.4.3/bits/github/firestore.py
--rw-r--r--   0        0        0     6904 2024-04-01 21:51:22.556290 bits_github-1.4.3/bits/github/helpers.py
--rw-r--r--   0        0        0     2719 2024-04-01 21:51:22.556290 bits_github-1.4.3/bits/github/sync.py
--rw-r--r--   0        0        0    24647 2024-04-01 21:51:22.556290 bits_github-1.4.3/bits/github/update.py
--rw-r--r--   0        0        0     1201 2024-04-01 21:51:22.556290 bits_github-1.4.3/pyproject.toml
--rw-r--r--   0        0        0     1108 1970-01-01 00:00:00.000000 bits_github-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0       45 2024-04-02 15:33:41.329796 bits_github-1.4.4/README.md
+-rw-r--r--   0        0        0       65 2024-04-02 15:33:41.329796 bits_github-1.4.4/bits/__init__.py
+-rw-r--r--   0        0        0    25792 2024-04-02 15:33:41.333796 bits_github-1.4.4/bits/github/__init__.py
+-rw-r--r--   0        0        0     1800 2024-04-02 15:33:41.333796 bits_github-1.4.4/bits/github/app.py
+-rw-r--r--   0        0        0    13646 2024-04-02 15:33:41.333796 bits_github-1.4.4/bits/github/auditlogs.py
+-rw-r--r--   0        0        0    16434 2024-04-02 15:33:41.333796 bits_github-1.4.4/bits/github/client.py
+-rw-r--r--   0        0        0     1899 2024-04-02 15:33:41.333796 bits_github-1.4.4/bits/github/datastore.py
+-rw-r--r--   0        0        0    10143 2024-04-02 15:33:41.333796 bits_github-1.4.4/bits/github/firestore.py
+-rw-r--r--   0        0        0     6904 2024-04-02 15:33:41.333796 bits_github-1.4.4/bits/github/helpers.py
+-rw-r--r--   0        0        0     2719 2024-04-02 15:33:41.333796 bits_github-1.4.4/bits/github/sync.py
+-rw-r--r--   0        0        0    24647 2024-04-02 15:33:41.333796 bits_github-1.4.4/bits/github/update.py
+-rw-r--r--   0        0        0     1252 2024-04-02 15:33:41.333796 bits_github-1.4.4/pyproject.toml
+-rw-r--r--   0        0        0      991 1970-01-01 00:00:00.000000 bits_github-1.4.4/PKG-INFO
```

### Comparing `bits_github-1.4.3/bits/github/__init__.py` & `bits_github-1.4.4/bits/github/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """GitHub class file."""
-
 import datetime
 from urllib.parse import urlencode
 
 import requests
 
 
 class GitHub:
@@ -12,52 +11,46 @@
     CODE_OK = 204
     CODE_NOT_CHANGED = 304
     CODE_NOT_FOUND = 404
 
     def __init__(  # noqa: PLR0913
             self,
             token,
-            org=None,
+            org,
             org_id=None,
             owner_team=None,
             role_team=None,
             role_team_name=None,
             verbose=False,
             app_project=None,
     ):
         """Initialize an GitHub class instance."""
         # set the base url
         self.base_url = "https://api.github.com"
-
-        # set the headers for authorized requests
-        self.headers = {"Authorization": f"token {self.token}"}
-
         # set github token
         self.token = token
-
+        # set the headers for authorized requests
+        self.headers = {"Authorization": f"token {self.token}"}
         # set github organization name
         self.org = org
         self.org_id = org_id
         if org and not org_id:
             self.get_org_id()
 
         # set a team to include all owners
         self.owner_team = owner_team
-
         # set a team to include all role accounts
         self.role_team = role_team
         self.role_team_name = role_team_name
-
         # enable verbosity
         self.verbose = verbose
-
         # set the other urls
         self.org_base_url = f"{self.base_url}/orgs/{self.org}"
         self.org_id_base_url = f"{self.base_url}/organizations/{self.org_id}"
-
+        # set the project name
         self.app_project = app_project
 
     #
     # Sub Classes
     #
     def app(self, auth=None):
         """Return an App instance."""
```

### Comparing `bits_github-1.4.3/bits/github/app.py` & `bits_github-1.4.4/bits/github/app.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.3/bits/github/auditlogs.py` & `bits_github-1.4.4/bits/github/auditlogs.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.3/bits/github/client.py` & `bits_github-1.4.4/bits/github/client.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.3/bits/github/datastore.py` & `bits_github-1.4.4/bits/github/datastore.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.3/bits/github/firestore.py` & `bits_github-1.4.4/bits/github/firestore.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.3/bits/github/helpers.py` & `bits_github-1.4.4/bits/github/helpers.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.3/bits/github/sync.py` & `bits_github-1.4.4/bits/github/sync.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.3/bits/github/update.py` & `bits_github-1.4.4/bits/github/update.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.3/pyproject.toml` & `bits_github-1.4.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -14,27 +14,29 @@
 license = "BSD-3-Clause"
 name = "bits-github"
 packages = [
     { include = "bits" },
 ]
 readme = "README.md"
 repository = "https://github.com/broadinstitute/bits-github.git"
-version = "1.4.3"
+version = "1.4.4"
 
 [tool.poetry.dependencies]
-python = "^3.9"  # Compatible python versions must be declared here
+python = ">=3.9,<3.12.1"  # Compatible python versions must be declared here
 
 bits-google = "^1.13.8"
 google-cloud-datastore = "^2.19.0"
 google-cloud-firestore = "^2.15.0"
 python-dateutil = "^2.9.0.post0"
 pytz = "*"
+
+[tool.poetry.group.dev.dependencies]
+green = "^4.0.1"
+responses = "^0.25.0"
 testtools = "^2.7.1"
-twine = "^5.0.0"
-wheel = "^0.43.0"
 
 [tool.ruff]
 line-length = 120
 
 [tool.ruff.format]
 # Prefer double quotes over single quotes.
 quote-style = "double"
```

### Comparing `bits_github-1.4.3/PKG-INFO` & `bits_github-1.4.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 Metadata-Version: 2.1
 Name: bits-github
-Version: 1.4.3
+Version: 1.4.4
 Summary: BITS GitHub Package for Python
 Home-page: https://github.com/broadinstitute/bits-github.git
 License: BSD-3-Clause
 Keywords: bits,github
 Author: Lukas Karlsson
 Author-email: karlsson@broadinstitute.org
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.9,<3.12.1
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: bits-google (>=1.13.8,<2.0.0)
 Requires-Dist: google-cloud-datastore (>=2.19.0,<3.0.0)
 Requires-Dist: google-cloud-firestore (>=2.15.0,<3.0.0)
 Requires-Dist: python-dateutil (>=2.9.0.post0,<3.0.0)
 Requires-Dist: pytz
-Requires-Dist: testtools (>=2.7.1,<3.0.0)
-Requires-Dist: twine (>=5.0.0,<6.0.0)
-Requires-Dist: wheel (>=0.43.0,<0.44.0)
 Project-URL: Repository, https://github.com/broadinstitute/bits-github.git
 Description-Content-Type: text/markdown
 
 # bits-github
 BITS GitHub package for python
```

