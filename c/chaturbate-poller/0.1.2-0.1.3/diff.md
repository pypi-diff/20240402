# Comparing `tmp/chaturbate_poller-0.1.2.tar.gz` & `tmp/chaturbate_poller-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chaturbate_poller-0.1.2.tar", max compression
+gzip compressed data, was "chaturbate_poller-0.1.3.tar", max compression
```

## Comparing `chaturbate_poller-0.1.2.tar` & `chaturbate_poller-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0     1071 2024-04-01 02:43:57.075882 chaturbate_poller-0.1.2/LICENSE
--rw-r--r--   0        0        0     2251 2024-04-01 02:43:57.075882 chaturbate_poller-0.1.2/README.md
--rw-r--r--   0        0        0     3062 2024-04-01 02:44:10.064041 chaturbate_poller-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      818 2024-04-01 02:43:57.075882 chaturbate_poller-0.1.2/src/chaturbate_poller/__init__.py
--rw-r--r--   0        0        0     1572 2024-04-01 02:43:57.075882 chaturbate_poller-0.1.2/src/chaturbate_poller/__main__.py
--rw-r--r--   0        0        0     4272 2024-04-01 02:43:57.075882 chaturbate_poller-0.1.2/src/chaturbate_poller/chaturbate_poller.py
--rw-r--r--   0        0        0      724 2024-04-01 02:43:57.075882 chaturbate_poller-0.1.2/src/chaturbate_poller/constants.py
--rw-r--r--   0        0        0     1429 2024-04-01 02:43:57.075882 chaturbate_poller-0.1.2/src/chaturbate_poller/logging_config.py
--rw-r--r--   0        0        0     3480 2024-04-01 02:43:57.075882 chaturbate_poller-0.1.2/src/chaturbate_poller/models.py
--rw-r--r--   0        0        0     3144 1970-01-01 00:00:00.000000 chaturbate_poller-0.1.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1071 2024-04-02 01:25:52.435591 chaturbate_poller-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2251 2024-04-02 01:25:52.435591 chaturbate_poller-0.1.3/README.md
+-rw-r--r--   0        0        0     3080 2024-04-02 01:26:05.459641 chaturbate_poller-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      818 2024-04-02 01:25:52.439591 chaturbate_poller-0.1.3/src/chaturbate_poller/__init__.py
+-rw-r--r--   0        0        0     1572 2024-04-02 01:25:52.439591 chaturbate_poller-0.1.3/src/chaturbate_poller/__main__.py
+-rw-r--r--   0        0        0     4272 2024-04-02 01:25:52.439591 chaturbate_poller-0.1.3/src/chaturbate_poller/chaturbate_poller.py
+-rw-r--r--   0        0        0      724 2024-04-02 01:25:52.439591 chaturbate_poller-0.1.3/src/chaturbate_poller/constants.py
+-rw-r--r--   0        0        0     1429 2024-04-02 01:25:52.439591 chaturbate_poller-0.1.3/src/chaturbate_poller/logging_config.py
+-rw-r--r--   0        0        0     3480 2024-04-02 01:25:52.439591 chaturbate_poller-0.1.3/src/chaturbate_poller/models.py
+-rw-r--r--   0        0        0     3144 1970-01-01 00:00:00.000000 chaturbate_poller-0.1.3/PKG-INFO
```

### Comparing `chaturbate_poller-0.1.2/LICENSE` & `chaturbate_poller-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.1.2/README.md` & `chaturbate_poller-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.1.2/pyproject.toml` & `chaturbate_poller-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chaturbate-poller"
-version = "0.1.2"
+version = "0.1.3"
 description = "Poller for the Chaturbate events API."
 authors = ["MountainGod2"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/MountainGod2/chaturbate_poller"
 documentation = "https://mountaingod2.github.io/chaturbate_poller/"
 
@@ -27,14 +27,15 @@
 pytest-mock = "^3.14.0"
 pytest-cov = "^5.0.0"
 myst-nb = {version = "^1.0.0", python = "^3.9"}
 sphinx-autoapi = "^3.0.0"
 sphinx-rtd-theme = "^2.0.0"
 python-semantic-release = "^9.4.0"
 ruff = "^0.3.4"
+poetry = "^1.8.2"
 
 [tool.semantic_release]
 version_variable = "pyproject.toml:version"
 version_toml = [
     "pyproject.toml:tool.poetry.version",
 ]                                                    # version location
 branch = "main"                                      # branch to make releases of
```

### Comparing `chaturbate_poller-0.1.2/src/chaturbate_poller/__init__.py` & `chaturbate_poller-0.1.3/src/chaturbate_poller/__init__.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.1.2/src/chaturbate_poller/__main__.py` & `chaturbate_poller-0.1.3/src/chaturbate_poller/__main__.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.1.2/src/chaturbate_poller/chaturbate_poller.py` & `chaturbate_poller-0.1.3/src/chaturbate_poller/chaturbate_poller.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.1.2/src/chaturbate_poller/constants.py` & `chaturbate_poller-0.1.3/src/chaturbate_poller/constants.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.1.2/src/chaturbate_poller/logging_config.py` & `chaturbate_poller-0.1.3/src/chaturbate_poller/logging_config.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.1.2/src/chaturbate_poller/models.py` & `chaturbate_poller-0.1.3/src/chaturbate_poller/models.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.1.2/PKG-INFO` & `chaturbate_poller-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaturbate-poller
-Version: 0.1.2
+Version: 0.1.3
 Summary: Poller for the Chaturbate events API.
 Home-page: https://github.com/MountainGod2/chaturbate_poller
 License: MIT
 Author: MountainGod2
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

