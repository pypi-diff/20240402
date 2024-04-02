# Comparing `tmp/orcalib-0.0.55.tar.gz` & `tmp/orcalib-0.0.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orcalib-0.0.55.tar", max compression
+gzip compressed data, was "orcalib-0.0.56.tar", max compression
```

## Comparing `orcalib-0.0.55.tar` & `orcalib-0.0.56.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      418 2024-03-29 15:16:58.279092 orcalib-0.0.55/README.md
--rw-r--r--   0        0        0    12670 2024-03-29 15:16:58.279092 orcalib-0.0.55/orcalib/__init__.py
--rw-r--r--   0        0        0    43202 2024-03-29 15:16:58.279092 orcalib-0.0.55/orcalib/batched_scan_result.py
--rw-r--r--   0        0        0    58694 2024-03-29 15:16:58.279092 orcalib-0.0.55/orcalib/client.py
--rw-r--r--   0        0        0     1895 2024-03-29 15:16:58.279092 orcalib-0.0.55/orcalib/client_data_model.py
--rw-r--r--   0        0        0      772 2024-03-29 15:16:58.279092 orcalib-0.0.55/orcalib/data_classes.py
--rw-r--r--   0        0        0    23394 2024-03-29 15:16:58.279092 orcalib-0.0.55/orcalib/database.py
--rw-r--r--   0        0        0     1040 2024-03-29 15:16:58.279092 orcalib-0.0.55/orcalib/exceptions.py
--rw-r--r--   0        0        0    10223 2024-03-29 15:16:58.279092 orcalib-0.0.55/orcalib/file_ingestor.py
--rw-r--r--   0        0        0    11355 2024-03-29 15:16:58.279092 orcalib-0.0.55/orcalib/hf_utils.py
--rw-r--r--   0        0        0     3928 2024-03-29 15:16:58.279092 orcalib-0.0.55/orcalib/index_handle.py
--rw-r--r--   0        0        0     7728 2024-03-29 15:16:58.279092 orcalib-0.0.55/orcalib/index_query.py
--rw-r--r--   0        0        0    11563 2024-03-29 15:16:58.279092 orcalib-0.0.55/orcalib/orca_chat.py
--rw-r--r--   0        0        0     5961 2024-03-29 15:16:58.279092 orcalib-0.0.55/orcalib/orca_expr.py
--rw-r--r--   0        0        0   106921 2024-03-29 15:16:58.279092 orcalib-0.0.55/orcalib/orca_torch.py
--rw-r--r--   0        0        0    24204 2024-03-29 15:16:58.279092 orcalib-0.0.55/orcalib/orca_types.py
--rw-r--r--   0        0        0     3183 2024-03-29 15:16:58.279092 orcalib-0.0.55/orcalib/orca_utils.py
--rw-r--r--   0        0        0    13972 2024-03-29 15:16:58.279092 orcalib-0.0.55/orcalib/table.py
--rw-r--r--   0        0        0    10928 2024-03-29 15:16:58.279092 orcalib-0.0.55/orcalib/table_query.py
--rw-r--r--   0        0        0     4489 2024-03-29 15:16:58.279092 orcalib-0.0.55/orcalib/temp_database.py
--rw-r--r--   0        0        0     1313 2024-03-29 15:17:18.675122 orcalib-0.0.55/pyproject.toml
--rw-r--r--   0        0        0     1463 1970-01-01 00:00:00.000000 orcalib-0.0.55/PKG-INFO
+-rw-r--r--   0        0        0      418 2024-04-02 17:50:15.643609 orcalib-0.0.56/README.md
+-rw-r--r--   0        0        0    12670 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/__init__.py
+-rw-r--r--   0        0        0    43202 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/batched_scan_result.py
+-rw-r--r--   0        0        0    58694 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/client.py
+-rw-r--r--   0        0        0     1895 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/client_data_model.py
+-rw-r--r--   0        0        0      772 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/data_classes.py
+-rw-r--r--   0        0        0    23394 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/database.py
+-rw-r--r--   0        0        0     1040 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/exceptions.py
+-rw-r--r--   0        0        0    10223 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/file_ingestor.py
+-rw-r--r--   0        0        0    11355 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/hf_utils.py
+-rw-r--r--   0        0        0     3928 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/index_handle.py
+-rw-r--r--   0        0        0     7728 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/index_query.py
+-rw-r--r--   0        0        0    11737 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/orca_chat.py
+-rw-r--r--   0        0        0     5961 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/orca_expr.py
+-rw-r--r--   0        0        0   106921 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/orca_torch.py
+-rw-r--r--   0        0        0    24204 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/orca_types.py
+-rw-r--r--   0        0        0     3183 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/orca_utils.py
+-rw-r--r--   0        0        0    13972 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/table.py
+-rw-r--r--   0        0        0    10928 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/table_query.py
+-rw-r--r--   0        0        0     4489 2024-04-02 17:50:15.643609 orcalib-0.0.56/orcalib/temp_database.py
+-rw-r--r--   0        0        0     1313 2024-04-02 17:50:37.931760 orcalib-0.0.56/pyproject.toml
+-rw-r--r--   0        0        0     1463 1970-01-01 00:00:00.000000 orcalib-0.0.56/PKG-INFO
```

### Comparing `orcalib-0.0.55/orcalib/__init__.py` & `orcalib-0.0.56/orcalib/__init__.py`

 * *Files identical despite different names*

### Comparing `orcalib-0.0.55/orcalib/batched_scan_result.py` & `orcalib-0.0.56/orcalib/batched_scan_result.py`

 * *Files identical despite different names*

### Comparing `orcalib-0.0.55/orcalib/client.py` & `orcalib-0.0.56/orcalib/client.py`

 * *Files identical despite different names*

### Comparing `orcalib-0.0.55/orcalib/client_data_model.py` & `orcalib-0.0.56/orcalib/client_data_model.py`

 * *Files identical despite different names*

### Comparing `orcalib-0.0.55/orcalib/data_classes.py` & `orcalib-0.0.56/orcalib/data_classes.py`

 * *Files identical despite different names*

### Comparing `orcalib-0.0.55/orcalib/database.py` & `orcalib-0.0.56/orcalib/database.py`

 * *Files identical despite different names*

### Comparing `orcalib-0.0.55/orcalib/exceptions.py` & `orcalib-0.0.56/orcalib/exceptions.py`

 * *Files identical despite different names*

### Comparing `orcalib-0.0.55/orcalib/file_ingestor.py` & `orcalib-0.0.56/orcalib/file_ingestor.py`

 * *Files identical despite different names*

### Comparing `orcalib-0.0.55/orcalib/hf_utils.py` & `orcalib-0.0.56/orcalib/hf_utils.py`

 * *Files identical despite different names*

### Comparing `orcalib-0.0.55/orcalib/index_handle.py` & `orcalib-0.0.56/orcalib/index_handle.py`

 * *Files identical despite different names*

### Comparing `orcalib-0.0.55/orcalib/index_query.py` & `orcalib-0.0.56/orcalib/index_query.py`

 * *Files identical despite different names*

### Comparing `orcalib-0.0.55/orcalib/orca_chat.py` & `orcalib-0.0.56/orcalib/orca_chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,18 @@
         """
         Determine the retrieval query based on the last user input
         and other context.
 
         Currently, this just combines all user inputs into a single query.
         :return: str
         """
-        return " ".join([obj["content"] if obj["role"] == "user" else "" for obj in self.chat_history])
+        if self.mode == "StatelessQA":
+            return " ".join([msgs["content"] if msgs["role"] == "user" else "" for msgs in [self.chat_history[-1]]])
+        else:
+            return " ".join([obj["content"] if obj["role"] == "user" else "" for obj in self.chat_history])
 
     def prep_next_gen(self, last_user_input: str) -> tuple[str, list[list[str]], Optional[list[list[Any]]]]:
         """
         Prepares the next generation by updating the chat history and last user input.
         :param last_user_input: Last user input
         :return: tuple[str, list[list[str]], Optional[list[list[Any]]]]
         """
```

### Comparing `orcalib-0.0.55/orcalib/orca_expr.py` & `orcalib-0.0.56/orcalib/orca_expr.py`

 * *Files identical despite different names*

### Comparing `orcalib-0.0.55/orcalib/orca_torch.py` & `orcalib-0.0.56/orcalib/orca_torch.py`

 * *Files identical despite different names*

### Comparing `orcalib-0.0.55/orcalib/orca_types.py` & `orcalib-0.0.56/orcalib/orca_types.py`

 * *Files identical despite different names*

### Comparing `orcalib-0.0.55/orcalib/orca_utils.py` & `orcalib-0.0.56/orcalib/orca_utils.py`

 * *Files identical despite different names*

### Comparing `orcalib-0.0.55/orcalib/table.py` & `orcalib-0.0.56/orcalib/table.py`

 * *Files identical despite different names*

### Comparing `orcalib-0.0.55/orcalib/table_query.py` & `orcalib-0.0.56/orcalib/table_query.py`

 * *Files identical despite different names*

### Comparing `orcalib-0.0.55/orcalib/temp_database.py` & `orcalib-0.0.56/orcalib/temp_database.py`

 * *Files identical despite different names*

### Comparing `orcalib-0.0.55/pyproject.toml` & `orcalib-0.0.56/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orcalib"
-version = "0.0.55"                              # will be set by CI before building the wheel from the git tag
+version = "0.0.56"                              # will be set by CI before building the wheel from the git tag
 description = "client library for Orca DB"
 license = "Apache-2.0"
 authors = ["Orca DB Inc. <dev-rel@orcadb.ai>"]
 readme = "README.md"
 packages = [{ include = "orcalib" }]
 
 [tool.poetry.dependencies]
```

### Comparing `orcalib-0.0.55/PKG-INFO` & `orcalib-0.0.56/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orcalib
-Version: 0.0.55
+Version: 0.0.56
 Summary: client library for Orca DB
 License: Apache-2.0
 Author: Orca DB Inc.
 Author-email: dev-rel@orcadb.ai
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

