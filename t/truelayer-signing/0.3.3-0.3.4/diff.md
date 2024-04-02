# Comparing `tmp/truelayer_signing-0.3.3.tar.gz` & `tmp/truelayer_signing-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truelayer_signing-0.3.3.tar", max compression
+gzip compressed data, was "truelayer_signing-0.3.4.tar", max compression
```

## Comparing `truelayer_signing-0.3.3.tar` & `truelayer_signing-0.3.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     9723 2024-02-23 15:22:31.940379 truelayer_signing-0.3.3/LICENSE-APACHE
--rw-r--r--   0        0        0     1066 2024-02-23 15:22:31.940379 truelayer_signing-0.3.3/LICENSE-MIT
--rw-r--r--   0        0        0     1075 2024-02-23 15:22:31.940379 truelayer_signing-0.3.3/README.md
--rw-r--r--   0        0        0      826 2024-02-23 15:22:31.944379 truelayer_signing-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     1203 2024-02-23 15:22:31.944379 truelayer_signing-0.3.3/truelayer_signing/__init__.py
--rw-r--r--   0        0        0     6193 2024-02-23 15:22:31.944379 truelayer_signing-0.3.3/truelayer_signing/crypto.py
--rw-r--r--   0        0        0      198 2024-02-23 15:22:31.944379 truelayer_signing-0.3.3/truelayer_signing/errors.py
--rw-r--r--   0        0        0     2686 2024-02-23 15:22:31.944379 truelayer_signing-0.3.3/truelayer_signing/sign.py
--rw-r--r--   0        0        0     5273 2024-02-23 15:22:31.944379 truelayer_signing-0.3.3/truelayer_signing/utils.py
--rw-r--r--   0        0        0     5798 2024-02-23 15:22:31.944379 truelayer_signing-0.3.3/truelayer_signing/verify.py
--rw-r--r--   0        0        0     1872 1970-01-01 00:00:00.000000 truelayer_signing-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     9723 2024-04-02 15:17:24.056306 truelayer_signing-0.3.4/LICENSE-APACHE
+-rw-r--r--   0        0        0     1066 2024-04-02 15:17:24.056306 truelayer_signing-0.3.4/LICENSE-MIT
+-rw-r--r--   0        0        0     1075 2024-04-02 15:17:24.056306 truelayer_signing-0.3.4/README.md
+-rw-r--r--   0        0        0      831 2024-04-02 15:17:24.056306 truelayer_signing-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     1203 2024-04-02 15:17:24.056306 truelayer_signing-0.3.4/truelayer_signing/__init__.py
+-rw-r--r--   0        0        0     6193 2024-04-02 15:17:24.056306 truelayer_signing-0.3.4/truelayer_signing/crypto.py
+-rw-r--r--   0        0        0      198 2024-04-02 15:17:24.056306 truelayer_signing-0.3.4/truelayer_signing/errors.py
+-rw-r--r--   0        0        0     2686 2024-04-02 15:17:24.056306 truelayer_signing-0.3.4/truelayer_signing/sign.py
+-rw-r--r--   0        0        0     5273 2024-04-02 15:17:24.056306 truelayer_signing-0.3.4/truelayer_signing/utils.py
+-rw-r--r--   0        0        0     5798 2024-04-02 15:17:24.060306 truelayer_signing-0.3.4/truelayer_signing/verify.py
+-rw-r--r--   0        0        0     1872 1970-01-01 00:00:00.000000 truelayer_signing-0.3.4/PKG-INFO
```

### Comparing `truelayer_signing-0.3.3/LICENSE-APACHE` & `truelayer_signing-0.3.4/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `truelayer_signing-0.3.3/LICENSE-MIT` & `truelayer_signing-0.3.4/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `truelayer_signing-0.3.3/README.md` & `truelayer_signing-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `truelayer_signing-0.3.3/pyproject.toml` & `truelayer_signing-0.3.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "truelayer-signing"
-version = "0.3.3"
+version = "0.3.4"
 description = "Produce & verify TrueLayer API requests signatures"
 authors = ["tl-flavio-barinas <flavio.barinas@truelayer.com>"]
 license = "Apache-2.0 or MIT"
 readme = "README.md"
 homepage = "https://github.com/TrueLayer/truelayer-signing/tree/main/python"
 repository = "https://github.com/TrueLayer/truelayer-signing"
 keywords = ["truelayer"]
 include = ["LICENSE-APACHE", "LICENSE-MIT"]
 
 [tool.poetry.dependencies]
 cryptography = ">=39,<43"
 python = "^3.8.1"
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.12.0"
+black = ">=22.12,<25.0"
 coverage = "^7.0.2"
 flake8 = "^6.0.0"
 mypy = "^0.991"
 pre-commit = "^2.21.0"
 pylint = "^2.15.9"
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
```

### Comparing `truelayer_signing-0.3.3/truelayer_signing/__init__.py` & `truelayer_signing-0.3.4/truelayer_signing/__init__.py`

 * *Files identical despite different names*

### Comparing `truelayer_signing-0.3.3/truelayer_signing/crypto.py` & `truelayer_signing-0.3.4/truelayer_signing/crypto.py`

 * *Files identical despite different names*

### Comparing `truelayer_signing-0.3.3/truelayer_signing/sign.py` & `truelayer_signing-0.3.4/truelayer_signing/sign.py`

 * *Files identical despite different names*

### Comparing `truelayer_signing-0.3.3/truelayer_signing/utils.py` & `truelayer_signing-0.3.4/truelayer_signing/utils.py`

 * *Files identical despite different names*

### Comparing `truelayer_signing-0.3.3/truelayer_signing/verify.py` & `truelayer_signing-0.3.4/truelayer_signing/verify.py`

 * *Files identical despite different names*

### Comparing `truelayer_signing-0.3.3/PKG-INFO` & `truelayer_signing-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truelayer-signing
-Version: 0.3.3
+Version: 0.3.4
 Summary: Produce & verify TrueLayer API requests signatures
 Home-page: https://github.com/TrueLayer/truelayer-signing/tree/main/python
 License: Apache-2.0 or MIT
 Keywords: truelayer
 Author: tl-flavio-barinas
 Author-email: flavio.barinas@truelayer.com
 Requires-Python: >=3.8.1,<4.0.0
```

