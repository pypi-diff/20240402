# Comparing `tmp/Oasys.gRPC-21.0.0b8.tar.gz` & `tmp/Oasys.gRPC-21.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Oasys.gRPC-21.0.0b8.tar", last modified: Fri Mar  8 14:48:07 2024, max compression
+gzip compressed data, was "Oasys.gRPC-21.0.0b9.tar", last modified: Wed Mar 13 15:56:01 2024, max compression
```

## Comparing `Oasys.gRPC-21.0.0b8.tar` & `Oasys.gRPC-21.0.0b9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-03-08 14:48:07.715161 Oasys.gRPC-21.0.0b8/
--rw-rw-rw-   0        0        0     1086 2024-01-18 09:17:20.000000 Oasys.gRPC-21.0.0b8/LICENSE
--rw-rw-rw-   0        0        0     3065 2024-03-08 14:48:07.714171 Oasys.gRPC-21.0.0b8/PKG-INFO
--rw-rw-rw-   0        0        0     1379 2023-10-04 15:07:25.000000 Oasys.gRPC-21.0.0b8/README.rst
--rw-rw-rw-   0        0        0      564 2024-03-07 13:26:15.000000 Oasys.gRPC-21.0.0b8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-08 14:48:07.715161 Oasys.gRPC-21.0.0b8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-08 14:48:07.655161 Oasys.gRPC-21.0.0b8/src/
-drwxrwxrwx   0        0        0        0 2024-03-08 14:48:07.655161 Oasys.gRPC-21.0.0b8/src/Oasys/
-drwxrwxrwx   0        0        0        0 2024-03-08 14:48:07.712168 Oasys.gRPC-21.0.0b8/src/Oasys/gRPC/
--rw-rw-rw-   0        0        0      158 2023-06-16 10:22:29.000000 Oasys.gRPC-21.0.0b8/src/Oasys/gRPC/__init__.py
--rw-rw-rw-   0        0        0      487 2023-06-20 12:04:49.000000 Oasys.gRPC-21.0.0b8/src/Oasys/gRPC/classes.py
--rw-rw-rw-   0        0        0    20568 2024-03-07 11:30:32.000000 Oasys.gRPC-21.0.0b8/src/Oasys/gRPC/connection.py
--rw-rw-rw-   0        0        0     6696 2023-07-07 07:24:38.000000 Oasys.gRPC-21.0.0b8/src/Oasys/gRPC/oasys_pb2.py
--rw-rw-rw-   0        0        0    19597 2023-05-23 16:18:29.000000 Oasys.gRPC-21.0.0b8/src/Oasys/gRPC/oasys_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2024-03-08 14:48:07.713160 Oasys.gRPC-21.0.0b8/src/Oasys.gRPC.egg-info/
--rw-rw-rw-   0        0        0     3065 2024-03-08 14:48:07.000000 Oasys.gRPC-21.0.0b8/src/Oasys.gRPC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      365 2024-03-08 14:48:07.000000 Oasys.gRPC-21.0.0b8/src/Oasys.gRPC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-08 14:48:07.000000 Oasys.gRPC-21.0.0b8/src/Oasys.gRPC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-03-08 14:48:07.000000 Oasys.gRPC-21.0.0b8/src/Oasys.gRPC.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-03-08 14:48:07.000000 Oasys.gRPC-21.0.0b8/src/Oasys.gRPC.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-13 15:56:01.263708 Oasys.gRPC-21.0.0b9/
+-rw-rw-rw-   0        0        0     1086 2024-01-18 09:17:20.000000 Oasys.gRPC-21.0.0b9/LICENSE
+-rw-rw-rw-   0        0        0     3065 2024-03-13 15:56:01.262695 Oasys.gRPC-21.0.0b9/PKG-INFO
+-rw-rw-rw-   0        0        0     1379 2023-10-04 15:07:25.000000 Oasys.gRPC-21.0.0b9/README.rst
+-rw-rw-rw-   0        0        0      564 2024-03-13 15:53:09.000000 Oasys.gRPC-21.0.0b9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-03-13 15:56:01.264777 Oasys.gRPC-21.0.0b9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-03-13 15:56:01.197276 Oasys.gRPC-21.0.0b9/src/
+drwxrwxrwx   0        0        0        0 2024-03-13 15:56:01.198275 Oasys.gRPC-21.0.0b9/src/Oasys/
+drwxrwxrwx   0        0        0        0 2024-03-13 15:56:01.258695 Oasys.gRPC-21.0.0b9/src/Oasys/gRPC/
+-rw-rw-rw-   0        0        0      158 2023-06-16 10:22:29.000000 Oasys.gRPC-21.0.0b9/src/Oasys/gRPC/__init__.py
+-rw-rw-rw-   0        0        0      487 2023-06-20 12:04:49.000000 Oasys.gRPC-21.0.0b9/src/Oasys/gRPC/classes.py
+-rw-rw-rw-   0        0        0    20652 2024-03-13 15:18:15.000000 Oasys.gRPC-21.0.0b9/src/Oasys/gRPC/connection.py
+-rw-rw-rw-   0        0        0     6696 2023-07-07 07:24:38.000000 Oasys.gRPC-21.0.0b9/src/Oasys/gRPC/oasys_pb2.py
+-rw-rw-rw-   0        0        0    19597 2023-05-23 16:18:29.000000 Oasys.gRPC-21.0.0b9/src/Oasys/gRPC/oasys_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2024-03-13 15:56:01.260730 Oasys.gRPC-21.0.0b9/src/Oasys.gRPC.egg-info/
+-rw-rw-rw-   0        0        0     3065 2024-03-13 15:56:01.000000 Oasys.gRPC-21.0.0b9/src/Oasys.gRPC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      365 2024-03-13 15:56:01.000000 Oasys.gRPC-21.0.0b9/src/Oasys.gRPC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-13 15:56:01.000000 Oasys.gRPC-21.0.0b9/src/Oasys.gRPC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-03-13 15:56:01.000000 Oasys.gRPC-21.0.0b9/src/Oasys.gRPC.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-03-13 15:56:01.000000 Oasys.gRPC-21.0.0b9/src/Oasys.gRPC.egg-info/top_level.txt
```

### Comparing `Oasys.gRPC-21.0.0b8/LICENSE` & `Oasys.gRPC-21.0.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `Oasys.gRPC-21.0.0b8/PKG-INFO` & `Oasys.gRPC-21.0.0b9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Oasys.gRPC
-Version: 21.0.0b8
+Version: 21.0.0b9
 Summary: gRPC functions for Oasys D3PLOT, PRIMER, REPORTER and T/HIS
 Author: Miles Thornton
 Maintainer-email: dyna.support@arup.com
 License: MIT License
         
         Copyright (c) 2024 Oasys Ltd
```

### Comparing `Oasys.gRPC-21.0.0b8/README.rst` & `Oasys.gRPC-21.0.0b9/README.rst`

 * *Files identical despite different names*

### Comparing `Oasys.gRPC-21.0.0b8/pyproject.toml` & `Oasys.gRPC-21.0.0b9/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "Oasys.gRPC"
-version = "21.0.0b8"
+version = "21.0.0b9"
 license = {file = "LICENSE"}
 requires-python = ">=3.8"
 keywords = ["Oasys", "gRPC"]
 dependencies = [
   "grpcio >= 1.54.0",
   "protobuf"
 ]
```

### Comparing `Oasys.gRPC-21.0.0b8/src/Oasys/gRPC/connection.py` & `Oasys.gRPC-21.0.0b9/src/Oasys/gRPC/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 # Initialise
         request = Oasys.gRPC.oasys_pb2.Memory()
         request.size = memory
         self.dbg("Calling Initialise")
         response = self.stub.Initialise(request)
 
         self.dbg("Returned {} '{}'".format(response.status, response.message))
+        assert response.status == Oasys.gRPC.oasys_pb2.STATUS_OK, response.message
 
         if response.value.HasField("dictarg"):
             dict = self.decode_dictarg(response.value.dictarg)
             self.version = dict.get('version')
             self.build   = dict.get('build')
 
         self.dbg("Connected to {} version {} build {}".format(self.program, self.version, self.build))
```

### Comparing `Oasys.gRPC-21.0.0b8/src/Oasys/gRPC/oasys_pb2.py` & `Oasys.gRPC-21.0.0b9/src/Oasys/gRPC/oasys_pb2.py`

 * *Files identical despite different names*

### Comparing `Oasys.gRPC-21.0.0b8/src/Oasys/gRPC/oasys_pb2_grpc.py` & `Oasys.gRPC-21.0.0b9/src/Oasys/gRPC/oasys_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Oasys.gRPC-21.0.0b8/src/Oasys.gRPC.egg-info/PKG-INFO` & `Oasys.gRPC-21.0.0b9/src/Oasys.gRPC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Oasys.gRPC
-Version: 21.0.0b8
+Version: 21.0.0b9
 Summary: gRPC functions for Oasys D3PLOT, PRIMER, REPORTER and T/HIS
 Author: Miles Thornton
 Maintainer-email: dyna.support@arup.com
 License: MIT License
         
         Copyright (c) 2024 Oasys Ltd
```

