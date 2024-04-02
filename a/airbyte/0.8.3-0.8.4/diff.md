# Comparing `tmp/airbyte-0.8.3.tar.gz` & `tmp/airbyte-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-0.8.3.tar", max compression
+gzip compressed data, was "airbyte-0.8.4.tar", max compression
```

## Comparing `airbyte-0.8.3.tar` & `airbyte-0.8.4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     3804 2024-04-02 00:35:03.698301 airbyte-0.8.3/LICENSE.md
--rw-r--r--   0        0        0     6176 2024-04-02 00:35:03.698301 airbyte-0.8.3/README.md
--rw-r--r--   0        0        0     1154 2024-04-02 00:35:03.698301 airbyte-0.8.3/airbyte/__init__.py
--rw-r--r--   0        0        0     2262 2024-04-02 00:35:03.698301 airbyte-0.8.3/airbyte/_batch_handles.py
--rw-r--r--   0        0        0    16354 2024-04-02 00:35:03.698301 airbyte-0.8.3/airbyte/_executor.py
--rw-r--r--   0        0        0        0 2024-04-02 00:35:03.698301 airbyte-0.8.3/airbyte/_processors/__init__.py
--rw-r--r--   0        0        0     9095 2024-04-02 00:35:03.698301 airbyte-0.8.3/airbyte/_processors/base.py
--rw-r--r--   0        0        0      352 2024-04-02 00:35:03.698301 airbyte-0.8.3/airbyte/_processors/file/__init__.py
--rw-r--r--   0        0        0     7496 2024-04-02 00:35:03.698301 airbyte-0.8.3/airbyte/_processors/file/base.py
--rw-r--r--   0        0        0      928 2024-04-02 00:35:03.698301 airbyte-0.8.3/airbyte/_processors/file/jsonl.py
--rw-r--r--   0        0        0       79 2024-04-02 00:35:03.698301 airbyte-0.8.3/airbyte/_processors/sql/__init__.py
--rw-r--r--   0        0        0    32880 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/_processors/sql/base.py
--rw-r--r--   0        0        0     8397 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/_processors/sql/bigquery.py
--rw-r--r--   0        0        0     3949 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/_processors/sql/duckdb.py
--rw-r--r--   0        0        0     1235 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/_processors/sql/motherduck.py
--rw-r--r--   0        0        0      837 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/_processors/sql/postgres.py
--rw-r--r--   0        0        0     3762 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/_processors/sql/snowflake.py
--rw-r--r--   0        0        0      420 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/_util/__init__.py
--rw-r--r--   0        0        0     3855 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/_util/document_rendering.py
--rw-r--r--   0        0        0     1854 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/_util/google_secrets.py
--rw-r--r--   0        0        0     3355 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/_util/meta.py
--rw-r--r--   0        0        0     6988 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/_util/name_normalizers.py
--rw-r--r--   0        0        0     1683 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/_util/pip_util.py
--rw-r--r--   0        0        0    10605 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/_util/telemetry.py
--rw-r--r--   0        0        0      903 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/caches/__init__.py
--rw-r--r--   0        0        0    10139 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/caches/_catalog_manager.py
--rw-r--r--   0        0        0     3775 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/caches/base.py
--rw-r--r--   0        0        0     1882 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/caches/bigquery.py
--rw-r--r--   0        0        0     1947 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/caches/duckdb.py
--rw-r--r--   0        0        0      471 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/caches/generic.py
--rw-r--r--   0        0        0     1169 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/caches/motherduck.py
--rw-r--r--   0        0        0     1213 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/caches/postgres.py
--rw-r--r--   0        0        0     1627 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/caches/snowflake.py
--rw-r--r--   0        0        0     1998 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/caches/util.py
--rw-r--r--   0        0        0      346 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/datasets/__init__.py
--rw-r--r--   0        0        0     2212 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/datasets/_base.py
--rw-r--r--   0        0        0      917 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/datasets/_lazy.py
--rw-r--r--   0        0        0      819 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/datasets/_map.py
--rw-r--r--   0        0        0     5481 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/datasets/_sql.py
--rw-r--r--   0        0        0     1861 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/documents.py
--rw-r--r--   0        0        0     9245 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/exceptions.py
--rw-r--r--   0        0        0    13834 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/progress.py
--rw-r--r--   0        0        0        0 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/py.typed
--rw-r--r--   0        0        0     1580 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/results.py
--rw-r--r--   0        0        0     3519 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/secrets.py
--rw-r--r--   0        0        0      517 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/sources/__init__.py
--rw-r--r--   0        0        0    28443 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/sources/base.py
--rw-r--r--   0        0        0     3718 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/sources/registry.py
--rw-r--r--   0        0        0     5516 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/sources/util.py
--rw-r--r--   0        0        0      987 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/strategies.py
--rw-r--r--   0        0        0     4733 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/types.py
--rw-r--r--   0        0        0     5423 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/validate.py
--rw-r--r--   0        0        0      232 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/version.py
--rw-r--r--   0        0        0      369 2024-04-02 00:35:03.702301 airbyte-0.8.3/airbyte/warnings.py
--rw-r--r--   0        0        0     8366 2024-04-02 00:35:15.246369 airbyte-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     7567 1970-01-01 00:00:00.000000 airbyte-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     3804 2024-04-02 06:23:28.499375 airbyte-0.8.4/LICENSE.md
+-rw-r--r--   0        0        0     6176 2024-04-02 06:23:28.499375 airbyte-0.8.4/README.md
+-rw-r--r--   0        0        0     1154 2024-04-02 06:23:28.499375 airbyte-0.8.4/airbyte/__init__.py
+-rw-r--r--   0        0        0     2262 2024-04-02 06:23:28.499375 airbyte-0.8.4/airbyte/_batch_handles.py
+-rw-r--r--   0        0        0    16354 2024-04-02 06:23:28.499375 airbyte-0.8.4/airbyte/_executor.py
+-rw-r--r--   0        0        0        0 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_processors/__init__.py
+-rw-r--r--   0        0        0     9095 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_processors/base.py
+-rw-r--r--   0        0        0      352 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_processors/file/__init__.py
+-rw-r--r--   0        0        0     7496 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_processors/file/base.py
+-rw-r--r--   0        0        0      928 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_processors/file/jsonl.py
+-rw-r--r--   0        0        0       79 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_processors/sql/__init__.py
+-rw-r--r--   0        0        0    32880 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_processors/sql/base.py
+-rw-r--r--   0        0        0     8568 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_processors/sql/bigquery.py
+-rw-r--r--   0        0        0     3949 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_processors/sql/duckdb.py
+-rw-r--r--   0        0        0     1235 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_processors/sql/motherduck.py
+-rw-r--r--   0        0        0      837 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_processors/sql/postgres.py
+-rw-r--r--   0        0        0     3762 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_processors/sql/snowflake.py
+-rw-r--r--   0        0        0      420 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_util/__init__.py
+-rw-r--r--   0        0        0     3855 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_util/document_rendering.py
+-rw-r--r--   0        0        0     1854 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_util/google_secrets.py
+-rw-r--r--   0        0        0     3355 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_util/meta.py
+-rw-r--r--   0        0        0     6988 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_util/name_normalizers.py
+-rw-r--r--   0        0        0     1683 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_util/pip_util.py
+-rw-r--r--   0        0        0    10605 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_util/telemetry.py
+-rw-r--r--   0        0        0      903 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/caches/__init__.py
+-rw-r--r--   0        0        0    10139 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/caches/_catalog_manager.py
+-rw-r--r--   0        0        0     3775 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/caches/base.py
+-rw-r--r--   0        0        0     2124 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/caches/bigquery.py
+-rw-r--r--   0        0        0     1947 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/caches/duckdb.py
+-rw-r--r--   0        0        0      471 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/caches/generic.py
+-rw-r--r--   0        0        0     1169 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/caches/motherduck.py
+-rw-r--r--   0        0        0     1213 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/caches/postgres.py
+-rw-r--r--   0        0        0     1627 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/caches/snowflake.py
+-rw-r--r--   0        0        0     1998 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/caches/util.py
+-rw-r--r--   0        0        0      346 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/datasets/__init__.py
+-rw-r--r--   0        0        0     2212 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/datasets/_base.py
+-rw-r--r--   0        0        0      917 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/datasets/_lazy.py
+-rw-r--r--   0        0        0      819 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/datasets/_map.py
+-rw-r--r--   0        0        0     5481 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/datasets/_sql.py
+-rw-r--r--   0        0        0     1861 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/documents.py
+-rw-r--r--   0        0        0     9245 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/exceptions.py
+-rw-r--r--   0        0        0    13834 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/progress.py
+-rw-r--r--   0        0        0        0 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/py.typed
+-rw-r--r--   0        0        0     1580 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/results.py
+-rw-r--r--   0        0        0     3519 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/secrets.py
+-rw-r--r--   0        0        0      517 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/sources/__init__.py
+-rw-r--r--   0        0        0    28443 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/sources/base.py
+-rw-r--r--   0        0        0     3718 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/sources/registry.py
+-rw-r--r--   0        0        0     5516 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/sources/util.py
+-rw-r--r--   0        0        0      987 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/strategies.py
+-rw-r--r--   0        0        0     4733 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/types.py
+-rw-r--r--   0        0        0     5423 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/validate.py
+-rw-r--r--   0        0        0      232 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/version.py
+-rw-r--r--   0        0        0      369 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/warnings.py
+-rw-r--r--   0        0        0     8366 2024-04-02 06:23:42.691383 airbyte-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0     7567 1970-01-01 00:00:00.000000 airbyte-0.8.4/PKG-INFO
```

### Comparing `airbyte-0.8.3/LICENSE.md` & `airbyte-0.8.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/README.md` & `airbyte-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/__init__.py` & `airbyte-0.8.4/airbyte/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/_batch_handles.py` & `airbyte-0.8.4/airbyte/_batch_handles.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/_executor.py` & `airbyte-0.8.4/airbyte/_executor.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/_processors/base.py` & `airbyte-0.8.4/airbyte/_processors/base.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/_processors/file/base.py` & `airbyte-0.8.4/airbyte/_processors/file/base.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/_processors/file/jsonl.py` & `airbyte-0.8.4/airbyte/_processors/file/jsonl.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/_processors/sql/base.py` & `airbyte-0.8.4/airbyte/_processors/sql/base.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/_processors/sql/bigquery.py` & `airbyte-0.8.4/airbyte/_processors/sql/bigquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 """A BigQuery implementation of the cache."""
 
 from __future__ import annotations
 
 from pathlib import Path
 from typing import TYPE_CHECKING, final
 
+import google.oauth2
 import sqlalchemy
 from google.api_core.exceptions import NotFound
 from google.cloud import bigquery
 from google.oauth2 import service_account
 from overrides import overrides
 
 from airbyte import exceptions as exc
@@ -55,15 +56,15 @@
     file_writer_class = JsonlWriter
     type_converter_class = BigQueryTypeConverter
     supports_merge_insert = True
 
     cache: BigQueryCache
 
     def __init__(self, cache: CacheBase, file_writer: FileWriterBase | None = None) -> None:
-        self._credentials: service_account.Credentials | None = None
+        self._credentials: google.auth.credentials.Credentials | None = None
         self._schema_exists: bool | None = None
         super().__init__(cache, file_writer)
 
     @final
     @overrides
     def _fully_qualified(
         self,
@@ -138,21 +139,23 @@
         except Exception as ex:
             # Ignore schema exists errors.
             if "already exists" not in str(ex):
                 raise
 
         self._schema_exists = True
 
-    def _get_credentials(self) -> service_account.Credentials:
+    def _get_credentials(self) -> google.auth.credentials.Credentials:
         """Return the GCP credentials."""
         if self._credentials is None:
-            self._credentials = service_account.Credentials.from_service_account_file(
-                self.cache.credentials_path
-            )
-
+            if self.cache.credentials_path:
+                self._credentials = service_account.Credentials.from_service_account_file(
+                    self.cache.credentials_path
+                )
+            else:
+                self._credentials, _ = google.auth.default()
         return self._credentials
 
     def _table_exists(
         self,
         table_name: str,
     ) -> bool:
         """Return true if the given table exists.
```

### Comparing `airbyte-0.8.3/airbyte/_processors/sql/duckdb.py` & `airbyte-0.8.4/airbyte/_processors/sql/duckdb.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/_processors/sql/motherduck.py` & `airbyte-0.8.4/airbyte/_processors/sql/motherduck.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/_processors/sql/postgres.py` & `airbyte-0.8.4/airbyte/_processors/sql/postgres.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/_processors/sql/snowflake.py` & `airbyte-0.8.4/airbyte/_processors/sql/snowflake.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/_util/document_rendering.py` & `airbyte-0.8.4/airbyte/_util/document_rendering.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/_util/google_secrets.py` & `airbyte-0.8.4/airbyte/_util/google_secrets.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/_util/meta.py` & `airbyte-0.8.4/airbyte/_util/meta.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/_util/name_normalizers.py` & `airbyte-0.8.4/airbyte/_util/name_normalizers.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/_util/pip_util.py` & `airbyte-0.8.4/airbyte/_util/pip_util.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/_util/telemetry.py` & `airbyte-0.8.4/airbyte/_util/telemetry.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/caches/__init__.py` & `airbyte-0.8.4/airbyte/caches/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/caches/_catalog_manager.py` & `airbyte-0.8.4/airbyte/caches/_catalog_manager.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/caches/base.py` & `airbyte-0.8.4/airbyte/caches/base.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/caches/bigquery.py` & `airbyte-0.8.4/airbyte/caches/bigquery.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,37 +13,42 @@
     credentials_path="path/to/credentials.json",
 )
 ```
 """
 
 from __future__ import annotations
 
-import urllib
-from typing import Any
+from typing import TYPE_CHECKING, Any, Optional
 
 from overrides import overrides
 from pydantic import root_validator
+from sqlalchemy.engine import make_url
 
 from airbyte._processors.sql.bigquery import BigQuerySqlProcessor
 from airbyte.caches.base import (
     CacheBase,
 )
 
 
+if TYPE_CHECKING:
+    from sqlalchemy.engine.url import URL
+
+
 class BigQueryCache(CacheBase):
     """The BigQuery cache implementation."""
 
     project_name: str
     """The name of the project to use. In BigQuery, this is equivalent to the database name."""
 
     dataset_name: str = "airbyte_raw"
     """The name of the dataset to use. In BigQuery, this is equivalent to the schema name."""
 
-    credentials_path: str
-    """The path to the credentials file to use."""
+    credentials_path: Optional[str] = None
+    """The path to the credentials file to use.
+    If not passed, falls back to the default inferred from the environment."""
 
     _sql_processor_class: type[BigQuerySqlProcessor] = BigQuerySqlProcessor
 
     @root_validator(pre=True)
     @classmethod
     def set_schema_name(cls, values: dict[str, Any]) -> dict[str, Any]:
         dataset_name = values.get("dataset_name")
@@ -56,9 +61,12 @@
     def get_database_name(self) -> str:
         """Return the name of the database. For BigQuery, this is the project name."""
         return self.project_name
 
     @overrides
     def get_sql_alchemy_url(self) -> str:
         """Return the SQLAlchemy URL to use."""
-        credentials_path_encoded = urllib.parse.quote(self.credentials_path)
-        return f"bigquery://{self.project_name!s}?credentials_path={credentials_path_encoded}"
+        url: URL = make_url(f"bigquery://{self.project_name!s}")
+        if self.credentials_path:
+            url = url.update_query_dict({"credentials_path": self.credentials_path})
+
+        return str(url)
```

### Comparing `airbyte-0.8.3/airbyte/caches/duckdb.py` & `airbyte-0.8.4/airbyte/caches/duckdb.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/caches/motherduck.py` & `airbyte-0.8.4/airbyte/caches/motherduck.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/caches/postgres.py` & `airbyte-0.8.4/airbyte/caches/postgres.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/caches/snowflake.py` & `airbyte-0.8.4/airbyte/caches/snowflake.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/caches/util.py` & `airbyte-0.8.4/airbyte/caches/util.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/datasets/_base.py` & `airbyte-0.8.4/airbyte/datasets/_base.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/datasets/_lazy.py` & `airbyte-0.8.4/airbyte/datasets/_lazy.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/datasets/_map.py` & `airbyte-0.8.4/airbyte/datasets/_map.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/datasets/_sql.py` & `airbyte-0.8.4/airbyte/datasets/_sql.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/documents.py` & `airbyte-0.8.4/airbyte/documents.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/exceptions.py` & `airbyte-0.8.4/airbyte/exceptions.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/progress.py` & `airbyte-0.8.4/airbyte/progress.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/results.py` & `airbyte-0.8.4/airbyte/results.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/secrets.py` & `airbyte-0.8.4/airbyte/secrets.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/sources/__init__.py` & `airbyte-0.8.4/airbyte/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/sources/base.py` & `airbyte-0.8.4/airbyte/sources/base.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/sources/registry.py` & `airbyte-0.8.4/airbyte/sources/registry.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/sources/util.py` & `airbyte-0.8.4/airbyte/sources/util.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/strategies.py` & `airbyte-0.8.4/airbyte/strategies.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/types.py` & `airbyte-0.8.4/airbyte/types.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/airbyte/validate.py` & `airbyte-0.8.4/airbyte/validate.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.3/pyproject.toml` & `airbyte-0.8.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = "PyAirbyte"
 authors = ["Airbyte <contact@airbyte.io>"]
 readme = "README.md"
 packages = [{include = "airbyte"}]
 
 # This project uses dynamic versioning
 # https://github.com/mtkennerly/poetry-dynamic-versioning
-version = "0.8.3"
+version = "0.8.4"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
```

### Comparing `airbyte-0.8.3/PKG-INFO` & `airbyte-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte
-Version: 0.8.3
+Version: 0.8.4
 Summary: PyAirbyte
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

