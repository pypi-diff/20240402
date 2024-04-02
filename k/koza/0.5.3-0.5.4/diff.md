# Comparing `tmp/koza-0.5.3.tar.gz` & `tmp/koza-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koza-0.5.3.tar", max compression
+gzip compressed data, was "koza-0.5.4.tar", max compression
```

## Comparing `koza-0.5.3.tar` & `koza-0.5.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1526 2023-12-13 20:21:35.519684 koza-0.5.3/LICENSE
--rw-r--r--   0        0        0     2809 2023-12-13 20:21:35.519684 koza-0.5.3/README.md
--rw-r--r--   0        0        0     1159 2023-12-13 20:21:35.519684 koza-0.5.3/pyproject.toml
--rw-r--r--   0        0        0       71 2023-12-13 20:21:35.519684 koza-0.5.3/src/koza/__init__.py
--rw-r--r--   0        0        0     8717 2023-12-13 20:21:35.519684 koza-0.5.3/src/koza/app.py
--rw-r--r--   0        0        0     6073 2023-12-13 20:21:35.519684 koza-0.5.3/src/koza/cli_runner.py
--rw-r--r--   0        0        0        0 2023-12-13 20:21:35.519684 koza-0.5.3/src/koza/converter/__init__.py
--rw-r--r--   0        0        0      883 2023-12-13 20:21:35.519684 koza-0.5.3/src/koza/converter/biolink_converter.py
--rw-r--r--   0        0        0     1730 2023-12-13 20:21:35.519684 koza-0.5.3/src/koza/converter/kgx_converter.py
--rw-r--r--   0        0        0      250 2023-12-13 20:21:35.523684 koza-0.5.3/src/koza/io/__init__.py
--rw-r--r--   0        0        0       62 2023-12-13 20:21:35.523684 koza-0.5.3/src/koza/io/reader/__init__.py
--rw-r--r--   0        0        0    10168 2023-12-13 20:21:35.523684 koza-0.5.3/src/koza/io/reader/csv_reader.py
--rw-r--r--   0        0        0     2964 2023-12-13 20:21:35.523684 koza-0.5.3/src/koza/io/reader/json_reader.py
--rw-r--r--   0        0        0     2118 2023-12-13 20:21:35.523684 koza-0.5.3/src/koza/io/reader/jsonl_reader.py
--rw-r--r--   0        0        0     7966 2023-12-13 20:21:35.523684 koza-0.5.3/src/koza/io/utils.py
--rw-r--r--   0        0        0        0 2023-12-13 20:21:35.523684 koza-0.5.3/src/koza/io/writer/__init__.py
--rw-r--r--   0        0        0     1553 2023-12-13 20:21:35.523684 koza-0.5.3/src/koza/io/writer/jsonl_writer.py
--rw-r--r--   0        0        0     4841 2023-12-13 20:21:35.523684 koza-0.5.3/src/koza/io/writer/tsv_writer.py
--rw-r--r--   0        0        0      370 2023-12-13 20:21:35.523684 koza-0.5.3/src/koza/io/writer/writer.py
--rw-r--r--   0        0        0     1572 2023-12-13 20:21:35.523684 koza-0.5.3/src/koza/io/yaml_loader.py
--rwxr-xr-x   0        0        0     2325 2023-12-13 20:21:35.523684 koza-0.5.3/src/koza/main.py
--rw-r--r--   0        0        0       28 2023-12-13 20:21:35.523684 koza-0.5.3/src/koza/model/__init__.py
--rw-r--r--   0        0        0        0 2023-12-13 20:21:35.523684 koza-0.5.3/src/koza/model/config/__init__.py
--rw-r--r--   0        0        0      218 2023-12-13 20:21:35.523684 koza-0.5.3/src/koza/model/config/pydantic_config.py
--rw-r--r--   0        0        0    11357 2023-12-13 20:21:35.523684 koza-0.5.3/src/koza/model/config/source_config.py
--rw-r--r--   0        0        0     6206 2023-12-13 20:21:35.523684 koza-0.5.3/src/koza/model/config/sssom_config.py
--rw-r--r--   0        0        0      396 2023-12-13 20:21:35.523684 koza-0.5.3/src/koza/model/curie_cleaner.py
--rw-r--r--   0        0        0      356 2023-12-13 20:21:35.523684 koza-0.5.3/src/koza/model/map_dict.py
--rw-r--r--   0        0        0     3652 2023-12-13 20:21:35.523684 koza-0.5.3/src/koza/model/source.py
--rw-r--r--   0        0        0     2914 2023-12-13 20:21:35.523684 koza-0.5.3/src/koza/model/translation_table.py
--rw-r--r--   0        0        0        0 2023-12-13 20:21:35.523684 koza-0.5.3/src/koza/utils/__init__
--rw-r--r--   0        0        0      294 2023-12-13 20:21:35.523684 koza-0.5.3/src/koza/utils/exceptions.py
--rw-r--r--   0        0        0      763 2023-12-13 20:21:35.523684 koza-0.5.3/src/koza/utils/log_utils.py
--rw-r--r--   0        0        0     1849 2023-12-13 20:21:35.523684 koza-0.5.3/src/koza/utils/row_filter.py
--rw-r--r--   0        0        0     3695 1970-01-01 00:00:00.000000 koza-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1526 2024-04-02 19:34:36.940962 koza-0.5.4/LICENSE
+-rw-r--r--   0        0        0     2809 2024-04-02 19:34:36.940962 koza-0.5.4/README.md
+-rw-r--r--   0        0        0     1159 2024-04-02 19:34:36.944963 koza-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0       71 2024-04-02 19:34:36.944963 koza-0.5.4/src/koza/__init__.py
+-rw-r--r--   0        0        0     8702 2024-04-02 19:34:36.944963 koza-0.5.4/src/koza/app.py
+-rw-r--r--   0        0        0     6073 2024-04-02 19:34:36.944963 koza-0.5.4/src/koza/cli_runner.py
+-rw-r--r--   0        0        0        0 2024-04-02 19:34:36.944963 koza-0.5.4/src/koza/converter/__init__.py
+-rw-r--r--   0        0        0      883 2024-04-02 19:34:36.944963 koza-0.5.4/src/koza/converter/biolink_converter.py
+-rw-r--r--   0        0        0     1730 2024-04-02 19:34:36.944963 koza-0.5.4/src/koza/converter/kgx_converter.py
+-rw-r--r--   0        0        0      250 2024-04-02 19:34:36.944963 koza-0.5.4/src/koza/io/__init__.py
+-rw-r--r--   0        0        0       62 2024-04-02 19:34:36.944963 koza-0.5.4/src/koza/io/reader/__init__.py
+-rw-r--r--   0        0        0    10168 2024-04-02 19:34:36.944963 koza-0.5.4/src/koza/io/reader/csv_reader.py
+-rw-r--r--   0        0        0     2964 2024-04-02 19:34:36.944963 koza-0.5.4/src/koza/io/reader/json_reader.py
+-rw-r--r--   0        0        0     2118 2024-04-02 19:34:36.944963 koza-0.5.4/src/koza/io/reader/jsonl_reader.py
+-rw-r--r--   0        0        0     7966 2024-04-02 19:34:36.944963 koza-0.5.4/src/koza/io/utils.py
+-rw-r--r--   0        0        0        0 2024-04-02 19:34:36.944963 koza-0.5.4/src/koza/io/writer/__init__.py
+-rw-r--r--   0        0        0     1553 2024-04-02 19:34:36.944963 koza-0.5.4/src/koza/io/writer/jsonl_writer.py
+-rw-r--r--   0        0        0     4841 2024-04-02 19:34:36.944963 koza-0.5.4/src/koza/io/writer/tsv_writer.py
+-rw-r--r--   0        0        0      370 2024-04-02 19:34:36.944963 koza-0.5.4/src/koza/io/writer/writer.py
+-rw-r--r--   0        0        0     1572 2024-04-02 19:34:36.944963 koza-0.5.4/src/koza/io/yaml_loader.py
+-rwxr-xr-x   0        0        0     2325 2024-04-02 19:34:36.944963 koza-0.5.4/src/koza/main.py
+-rw-r--r--   0        0        0       28 2024-04-02 19:34:36.948963 koza-0.5.4/src/koza/model/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 19:34:36.948963 koza-0.5.4/src/koza/model/config/__init__.py
+-rw-r--r--   0        0        0      218 2024-04-02 19:34:36.948963 koza-0.5.4/src/koza/model/config/pydantic_config.py
+-rw-r--r--   0        0        0    11357 2024-04-02 19:34:36.948963 koza-0.5.4/src/koza/model/config/source_config.py
+-rw-r--r--   0        0        0     6206 2024-04-02 19:34:36.948963 koza-0.5.4/src/koza/model/config/sssom_config.py
+-rw-r--r--   0        0        0      396 2024-04-02 19:34:36.948963 koza-0.5.4/src/koza/model/curie_cleaner.py
+-rw-r--r--   0        0        0      356 2024-04-02 19:34:36.948963 koza-0.5.4/src/koza/model/map_dict.py
+-rw-r--r--   0        0        0     3652 2024-04-02 19:34:36.948963 koza-0.5.4/src/koza/model/source.py
+-rw-r--r--   0        0        0     2914 2024-04-02 19:34:36.948963 koza-0.5.4/src/koza/model/translation_table.py
+-rw-r--r--   0        0        0        0 2024-04-02 19:34:36.948963 koza-0.5.4/src/koza/utils/__init__
+-rw-r--r--   0        0        0      294 2024-04-02 19:34:36.948963 koza-0.5.4/src/koza/utils/exceptions.py
+-rw-r--r--   0        0        0      763 2024-04-02 19:34:36.948963 koza-0.5.4/src/koza/utils/log_utils.py
+-rw-r--r--   0        0        0     1849 2024-04-02 19:34:36.948963 koza-0.5.4/src/koza/utils/row_filter.py
+-rw-r--r--   0        0        0     3695 1970-01-01 00:00:00.000000 koza-0.5.4/PKG-INFO
```

### Comparing `koza-0.5.3/LICENSE` & `koza-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `koza-0.5.3/README.md` & `koza-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `koza-0.5.3/pyproject.toml` & `koza-0.5.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "koza"
-version = "0.5.3"
+version = "0.5.4"
 description = "Data transformation framework for LinkML data models"
 authors = [
     "The Monarch Initiative <info@monarchinitiative.org>",
     "Kevin Schaper <kevinschaper@gmail.com>",
     "Glass Elsarboukh <g.elsarboukh@gmail.com>",
     "Kent Shefchek <kent@tislab.org>",
     ]
```

### Comparing `koza-0.5.3/src/koza/app.py` & `koza-0.5.4/src/koza/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import importlib
 import sys
 from pathlib import Path
 from typing import Dict, Union
 import yaml
 
 from linkml.validator import validate
-from pydantic.error_wrappers import ValidationError
+from pydantic import ValidationError
 
 from koza.converter.kgx_converter import KGXConverter
 from koza.utils.exceptions import MapItemException, NextRowException
 from koza.io.writer.jsonl_writer import JSONLWriter
 from koza.io.writer.tsv_writer import TSVWriter
 from koza.io.writer.writer import KozaWriter
 from koza.io.yaml_loader import UniqueIncludeLoader
```

### Comparing `koza-0.5.3/src/koza/cli_runner.py` & `koza-0.5.4/src/koza/cli_runner.py`

 * *Files identical despite different names*

### Comparing `koza-0.5.3/src/koza/converter/biolink_converter.py` & `koza-0.5.4/src/koza/converter/biolink_converter.py`

 * *Files identical despite different names*

### Comparing `koza-0.5.3/src/koza/converter/kgx_converter.py` & `koza-0.5.4/src/koza/converter/kgx_converter.py`

 * *Files identical despite different names*

### Comparing `koza-0.5.3/src/koza/io/reader/csv_reader.py` & `koza-0.5.4/src/koza/io/reader/csv_reader.py`

 * *Files identical despite different names*

### Comparing `koza-0.5.3/src/koza/io/reader/json_reader.py` & `koza-0.5.4/src/koza/io/reader/json_reader.py`

 * *Files identical despite different names*

### Comparing `koza-0.5.3/src/koza/io/reader/jsonl_reader.py` & `koza-0.5.4/src/koza/io/reader/jsonl_reader.py`

 * *Files identical despite different names*

### Comparing `koza-0.5.3/src/koza/io/utils.py` & `koza-0.5.4/src/koza/io/utils.py`

 * *Files identical despite different names*

### Comparing `koza-0.5.3/src/koza/io/writer/jsonl_writer.py` & `koza-0.5.4/src/koza/io/writer/jsonl_writer.py`

 * *Files identical despite different names*

### Comparing `koza-0.5.3/src/koza/io/writer/tsv_writer.py` & `koza-0.5.4/src/koza/io/writer/tsv_writer.py`

 * *Files identical despite different names*

### Comparing `koza-0.5.3/src/koza/io/yaml_loader.py` & `koza-0.5.4/src/koza/io/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `koza-0.5.3/src/koza/main.py` & `koza-0.5.4/src/koza/main.py`

 * *Files identical despite different names*

### Comparing `koza-0.5.3/src/koza/model/config/source_config.py` & `koza-0.5.4/src/koza/model/config/source_config.py`

 * *Files identical despite different names*

### Comparing `koza-0.5.3/src/koza/model/config/sssom_config.py` & `koza-0.5.4/src/koza/model/config/sssom_config.py`

 * *Files identical despite different names*

### Comparing `koza-0.5.3/src/koza/model/source.py` & `koza-0.5.4/src/koza/model/source.py`

 * *Files identical despite different names*

### Comparing `koza-0.5.3/src/koza/model/translation_table.py` & `koza-0.5.4/src/koza/model/translation_table.py`

 * *Files identical despite different names*

### Comparing `koza-0.5.3/src/koza/utils/log_utils.py` & `koza-0.5.4/src/koza/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `koza-0.5.3/src/koza/utils/row_filter.py` & `koza-0.5.4/src/koza/utils/row_filter.py`

 * *Files identical despite different names*

### Comparing `koza-0.5.3/PKG-INFO` & `koza-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koza
-Version: 0.5.3
+Version: 0.5.4
 Summary: Data transformation framework for LinkML data models
 License: BSD License
 Author: The Monarch Initiative
 Author-email: info@monarchinitiative.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

