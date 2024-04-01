# Comparing `tmp/crm1-0.0.7.tar.gz` & `tmp/crm1-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crm1-0.0.7.tar", max compression
+gzip compressed data, was "crm1-0.0.8.tar", max compression
```

## Comparing `crm1-0.0.7.tar` & `crm1-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1064 2024-04-01 21:50:09.575339 crm1-0.0.7/LICENSE
--rw-r--r--   0        0        0     4110 2024-04-01 21:50:09.575339 crm1-0.0.7/README.md
--rw-r--r--   0        0        0      152 2024-04-01 21:50:09.575339 crm1-0.0.7/crm1/__init__.py
--rw-r--r--   0        0        0      394 2024-04-01 21:50:09.575339 crm1-0.0.7/crm1/autorepotools.py
--rw-r--r--   0        0        0        0 2024-04-01 21:50:09.575339 crm1-0.0.7/crm1/helpers/__init__.py
--rw-r--r--   0        0        0     6824 2024-04-01 21:50:09.575339 crm1-0.0.7/crm1/helpers/versions.py
--rw-r--r--   0        0        0      176 2024-04-01 21:50:09.575339 crm1-0.0.7/crm1/spec/__init__.py
--rw-r--r--   0        0        0     1909 2024-04-01 21:50:09.575339 crm1-0.0.7/crm1/spec/common_modext.py
--rw-r--r--   0        0        0      467 2024-04-01 21:50:09.575339 crm1-0.0.7/crm1/spec/dependency.py
--rw-r--r--   0        0        0      938 2024-04-01 21:50:09.575339 crm1-0.0.7/crm1/spec/mod.py
--rw-r--r--   0        0        0      584 2024-04-01 21:50:09.575339 crm1-0.0.7/crm1/spec/repository.py
--rw-r--r--   0        0        0      153 2024-04-01 21:50:09.575339 crm1-0.0.7/crm1/types/__init__.py
--rw-r--r--   0        0        0     1043 2024-04-01 21:50:09.575339 crm1-0.0.7/crm1/types/dependency.py
--rw-r--r--   0        0        0     1070 2024-04-01 21:50:09.575339 crm1-0.0.7/crm1/types/mod.py
--rw-r--r--   0        0        0     1872 2024-04-01 21:50:09.575339 crm1-0.0.7/crm1/types/repository.py
--rw-r--r--   0        0        0     2619 2024-04-01 21:50:09.575339 crm1-0.0.7/crm1/types/repository_pool.py
--rw-r--r--   0        0        0      574 2024-04-01 21:50:09.575339 crm1-0.0.7/crm1/utils.py
--rw-r--r--   0        0        0      379 2024-04-01 21:50:09.575339 crm1-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     4721 1970-01-01 00:00:00.000000 crm1-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-01 22:01:25.657467 crm1-0.0.8/LICENSE
+-rw-r--r--   0        0        0     4110 2024-04-01 22:01:25.657467 crm1-0.0.8/README.md
+-rw-r--r--   0        0        0      152 2024-04-01 22:01:25.661467 crm1-0.0.8/crm1/__init__.py
+-rw-r--r--   0        0        0      394 2024-04-01 22:01:25.661467 crm1-0.0.8/crm1/autorepotools.py
+-rw-r--r--   0        0        0        0 2024-04-01 22:01:25.661467 crm1-0.0.8/crm1/helpers/__init__.py
+-rw-r--r--   0        0        0     6824 2024-04-01 22:01:25.661467 crm1-0.0.8/crm1/helpers/versions.py
+-rw-r--r--   0        0        0      176 2024-04-01 22:01:25.661467 crm1-0.0.8/crm1/spec/__init__.py
+-rw-r--r--   0        0        0     1922 2024-04-01 22:01:25.661467 crm1-0.0.8/crm1/spec/common_modext.py
+-rw-r--r--   0        0        0      467 2024-04-01 22:01:25.661467 crm1-0.0.8/crm1/spec/dependency.py
+-rw-r--r--   0        0        0      938 2024-04-01 22:01:25.661467 crm1-0.0.8/crm1/spec/mod.py
+-rw-r--r--   0        0        0      584 2024-04-01 22:01:25.661467 crm1-0.0.8/crm1/spec/repository.py
+-rw-r--r--   0        0        0      153 2024-04-01 22:01:25.661467 crm1-0.0.8/crm1/types/__init__.py
+-rw-r--r--   0        0        0     1043 2024-04-01 22:01:25.661467 crm1-0.0.8/crm1/types/dependency.py
+-rw-r--r--   0        0        0     1070 2024-04-01 22:01:25.661467 crm1-0.0.8/crm1/types/mod.py
+-rw-r--r--   0        0        0     1872 2024-04-01 22:01:25.661467 crm1-0.0.8/crm1/types/repository.py
+-rw-r--r--   0        0        0     2619 2024-04-01 22:01:25.661467 crm1-0.0.8/crm1/types/repository_pool.py
+-rw-r--r--   0        0        0      574 2024-04-01 22:01:25.661467 crm1-0.0.8/crm1/utils.py
+-rw-r--r--   0        0        0      379 2024-04-01 22:01:25.661467 crm1-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     4721 1970-01-01 00:00:00.000000 crm1-0.0.8/PKG-INFO
```

### Comparing `crm1-0.0.7/LICENSE` & `crm1-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `crm1-0.0.7/README.md` & `crm1-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `crm1-0.0.7/crm1/helpers/versions.py` & `crm1-0.0.8/crm1/helpers/versions.py`

 * *Files identical despite different names*

### Comparing `crm1-0.0.7/crm1/spec/common_modext.py` & `crm1-0.0.8/crm1/spec/common_modext.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,14 @@
     published_at: Optional[int] = None
     """The time the release was published at, in milliseconds since the Unix epoch."""
     alt_download: Optional[list[list[str, str]]] = None
     """A list of alternative download URLs.
     Each element is a list of two strings: the name and the URL."""
     alt_versions: Optional[list["spec.mod.RMod"]] = None
     """A list of older versions of the mod."""
-    suggests: Optional[list[spec.RDependency]] = None
+    suggests: Optional[list["spec.dependency.RDependency"]] = None
     """A list of suggested mods, that are not required
     but are recommended to be installed with this mod."""
     prerelease: Optional[bool] = None
     """Pre-release status of the mod release. If true, the mod's release is a pre-release."""
     others: CatchAll = field(default_factory=dict)
     """Any other fields that are not defined in this class."""
```

### Comparing `crm1-0.0.7/crm1/spec/mod.py` & `crm1-0.0.8/crm1/spec/mod.py`

 * *Files identical despite different names*

### Comparing `crm1-0.0.7/crm1/spec/repository.py` & `crm1-0.0.8/crm1/spec/repository.py`

 * *Files identical despite different names*

### Comparing `crm1-0.0.7/crm1/types/dependency.py` & `crm1-0.0.8/crm1/types/dependency.py`

 * *Files identical despite different names*

### Comparing `crm1-0.0.7/crm1/types/mod.py` & `crm1-0.0.8/crm1/types/mod.py`

 * *Files identical despite different names*

### Comparing `crm1-0.0.7/crm1/types/repository.py` & `crm1-0.0.8/crm1/types/repository.py`

 * *Files identical despite different names*

### Comparing `crm1-0.0.7/crm1/types/repository_pool.py` & `crm1-0.0.8/crm1/types/repository_pool.py`

 * *Files identical despite different names*

### Comparing `crm1-0.0.7/crm1/utils.py` & `crm1-0.0.8/crm1/utils.py`

 * *Files identical despite different names*

### Comparing `crm1-0.0.7/PKG-INFO` & `crm1-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crm1
-Version: 0.0.7
+Version: 0.0.8
 Summary: A CRM-1 repository exploration package
 License: MIT
 Author: JoJoJux
 Author-email: johannes@jojojux.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

