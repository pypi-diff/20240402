# Comparing `tmp/juicenet_cli-0.9.0.tar.gz` & `tmp/juicenet_cli-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "juicenet_cli-0.9.0.tar", max compression
+gzip compressed data, was "juicenet_cli-0.9.1.tar", max compression
```

## Comparing `juicenet_cli-0.9.0.tar` & `juicenet_cli-0.9.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     4233 2023-10-10 19:15:54.964120 juicenet_cli-0.9.0/README.md
--rw-r--r--   0        0        0    15540 2023-10-10 19:15:54.964120 juicenet_cli-0.9.0/juicenet.py
--rw-r--r--   0        0        0     1053 2023-10-10 19:15:54.964120 juicenet_cli-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     5081 1970-01-01 00:00:00.000000 juicenet_cli-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     4233 2023-10-11 19:56:25.667109 juicenet_cli-0.9.1/README.md
+-rw-r--r--   0        0        0    15450 2023-10-11 19:56:25.667109 juicenet_cli-0.9.1/juicenet.py
+-rw-r--r--   0        0        0     1053 2023-10-11 19:56:25.667109 juicenet_cli-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     5081 1970-01-01 00:00:00.000000 juicenet_cli-0.9.1/PKG-INFO
```

### Comparing `juicenet_cli-0.9.0/README.md` & `juicenet_cli-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `juicenet_cli-0.9.0/juicenet.py` & `juicenet_cli-0.9.1/juicenet.py`

 * *Files 1% similar despite different names*

```diff
@@ -556,11 +556,8 @@
         debug=args.debug,
         move=args.move,
         extensions=args.exts,
     )
 
 
 if __name__ == "__main__":
-    try:
-        CLI()
-    except KeyboardInterrupt:
-        logger.error("Process killed by user")
+    CLI()
```

### Comparing `juicenet_cli-0.9.0/pyproject.toml` & `juicenet_cli-0.9.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "juicenet-cli"
-version = "0.9.0"
+version = "0.9.1"
 description = "Crude CLI tool to upload files to Usenet using Nyuu and ParPar"
 authors = ["Raventric <78981416+Ravencentric@users.noreply.github.com>"]
 license = "Unlicense"
 readme = "README.md"
 packages = [
     { include = "juicenet.py"},
 ]
```

### Comparing `juicenet_cli-0.9.0/PKG-INFO` & `juicenet_cli-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juicenet-cli
-Version: 0.9.0
+Version: 0.9.1
 Summary: Crude CLI tool to upload files to Usenet using Nyuu and ParPar
 Home-page: https://github.com/Ravencentric/juicenet-cli
 License: Unlicense
 Author: Raventric
 Author-email: 78981416+Ravencentric@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: juicenet-cli Version: 0.9.0 Summary: Crude CLI tool
+Metadata-Version: 2.1 Name: juicenet-cli Version: 0.9.1 Summary: Crude CLI tool
 to upload files to Usenet using Nyuu and ParPar Home-page: https://github.com/
 Ravencentric/juicenet-cli License: Unlicense Author: Raventric Author-email:
 78981416+Ravencentric@users.noreply.github.com Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved Classifier: License :: OSI Approved :: The
 Unlicense (Unlicense) Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: PyYAML (>=6.0.1,<7.0.0) Requires-
```

