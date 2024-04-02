# Comparing `tmp/sanctify-1.3.0.tar.gz` & `tmp/sanctify-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sanctify-1.3.0.tar", last modified: Tue Mar 12 16:32:02 2024, max compression
+gzip compressed data, was "sanctify-1.4.0.tar", last modified: Tue Apr  2 09:27:27 2024, max compression
```

## Comparing `sanctify-1.3.0.tar` & `sanctify-1.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2024-03-12 16:32:02.843199 sanctify-1.3.0/
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    11349 2023-07-24 05:34:49.000000 sanctify-1.3.0/LICENSE
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    19181 2024-03-12 16:32:02.842915 sanctify-1.3.0/PKG-INFO
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    18062 2023-09-20 08:58:16.000000 sanctify-1.3.0/README.md
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1814 2024-03-12 11:16:48.000000 sanctify-1.3.0/pyproject.toml
-drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2024-03-12 16:32:02.840131 sanctify-1.3.0/sanctify/
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1286 2024-03-12 12:14:52.000000 sanctify-1.3.0/sanctify/__init__.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    17286 2024-03-12 11:16:48.000000 sanctify-1.3.0/sanctify/cleanser.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     2805 2024-03-08 13:21:10.000000 sanctify-1.3.0/sanctify/constants.py
-drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2024-03-12 16:32:02.842055 sanctify-1.3.0/sanctify/examples/
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      329 2024-03-12 12:14:52.000000 sanctify-1.3.0/sanctify/examples/__init__.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     2155 2024-03-09 16:56:05.000000 sanctify-1.3.0/sanctify/examples/column_mapping_schema.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     3238 2023-10-16 06:12:09.000000 sanctify-1.3.0/sanctify/examples/data_type_schema.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      332 2023-08-07 05:30:23.000000 sanctify-1.3.0/sanctify/exception.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    14964 2024-03-12 12:14:52.000000 sanctify-1.3.0/sanctify/processor.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     4145 2023-08-07 05:30:23.000000 sanctify-1.3.0/sanctify/serializer.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    13067 2024-03-12 12:14:52.000000 sanctify-1.3.0/sanctify/transformer.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     4922 2024-03-12 11:16:48.000000 sanctify-1.3.0/sanctify/utils.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    13172 2024-03-12 12:14:52.000000 sanctify-1.3.0/sanctify/validator.py
-drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2024-03-12 16:32:02.842632 sanctify-1.3.0/sanctify.egg-info/
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    19181 2024-03-12 16:32:02.000000 sanctify-1.3.0/sanctify.egg-info/PKG-INFO
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      497 2024-03-12 16:32:02.000000 sanctify-1.3.0/sanctify.egg-info/SOURCES.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        1 2024-03-12 16:32:02.000000 sanctify-1.3.0/sanctify.egg-info/dependency_links.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      256 2024-03-12 16:32:02.000000 sanctify-1.3.0/sanctify.egg-info/requires.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        9 2024-03-12 16:32:02.000000 sanctify-1.3.0/sanctify.egg-info/top_level.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)       38 2024-03-12 16:32:02.843240 sanctify-1.3.0/setup.cfg
+drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2024-04-02 09:27:27.301941 sanctify-1.4.0/
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    11349 2023-07-24 05:34:49.000000 sanctify-1.4.0/LICENSE
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    19181 2024-04-02 09:27:27.301638 sanctify-1.4.0/PKG-INFO
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    18062 2023-09-20 08:58:16.000000 sanctify-1.4.0/README.md
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1814 2024-04-02 09:27:08.000000 sanctify-1.4.0/pyproject.toml
+drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2024-04-02 09:27:27.299127 sanctify-1.4.0/sanctify/
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1286 2024-04-02 09:24:44.000000 sanctify-1.4.0/sanctify/__init__.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    18219 2024-04-02 09:27:08.000000 sanctify-1.4.0/sanctify/cleanser.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     2805 2024-03-08 13:21:10.000000 sanctify-1.4.0/sanctify/constants.py
+drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2024-04-02 09:27:27.300948 sanctify-1.4.0/sanctify/examples/
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      329 2024-04-02 09:24:44.000000 sanctify-1.4.0/sanctify/examples/__init__.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     2155 2024-03-09 16:56:05.000000 sanctify-1.4.0/sanctify/examples/column_mapping_schema.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     3238 2023-10-16 06:12:09.000000 sanctify-1.4.0/sanctify/examples/data_type_schema.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      332 2023-08-07 05:30:23.000000 sanctify-1.4.0/sanctify/exception.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    14964 2024-04-02 09:24:45.000000 sanctify-1.4.0/sanctify/processor.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     4145 2023-08-07 05:30:23.000000 sanctify-1.4.0/sanctify/serializer.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    13067 2024-04-02 09:24:45.000000 sanctify-1.4.0/sanctify/transformer.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     4922 2024-03-12 11:16:48.000000 sanctify-1.4.0/sanctify/utils.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    13172 2024-04-02 09:24:45.000000 sanctify-1.4.0/sanctify/validator.py
+drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2024-04-02 09:27:27.301270 sanctify-1.4.0/sanctify.egg-info/
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    19181 2024-04-02 09:27:27.000000 sanctify-1.4.0/sanctify.egg-info/PKG-INFO
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      497 2024-04-02 09:27:27.000000 sanctify-1.4.0/sanctify.egg-info/SOURCES.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        1 2024-04-02 09:27:27.000000 sanctify-1.4.0/sanctify.egg-info/dependency_links.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      256 2024-04-02 09:27:27.000000 sanctify-1.4.0/sanctify.egg-info/requires.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        9 2024-04-02 09:27:27.000000 sanctify-1.4.0/sanctify.egg-info/top_level.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)       38 2024-04-02 09:27:27.301980 sanctify-1.4.0/setup.cfg
```

### Comparing `sanctify-1.3.0/LICENSE` & `sanctify-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sanctify-1.3.0/PKG-INFO` & `sanctify-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sanctify
-Version: 1.3.0
+Version: 1.4.0
 Summary: Column Mapping based cleansing and validations for a given pandas dataframe
 Author-email: Avijeet Diwaker <avijeetdiwaker@gmail.com>
 Project-URL: Homepage, https://github.com/skit-ai/sanctify
 Project-URL: Bug Tracker, https://github.com/skit-ai/sanctify/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `sanctify-1.3.0/README.md` & `sanctify-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `sanctify-1.3.0/pyproject.toml` & `sanctify-1.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 [tool.pytest.ini_options]
 log_cli=true
 log_cli_level='DEBUG'
 
 [project]
 name = "sanctify"
-version = "1.3.0"
+version = "1.4.0"
 authors = [{name = "Avijeet Diwaker", email = "avijeetdiwaker@gmail.com"}]
 description = "Column Mapping based cleansing and validations for a given pandas dataframe"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers=[
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
```

### Comparing `sanctify-1.3.0/sanctify/__init__.py` & `sanctify-1.4.0/sanctify/__init__.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.3.0/sanctify/cleanser.py` & `sanctify-1.4.0/sanctify/cleanser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # External Imports
 from typing import Iterable
 
 import pandas as pd
 from frozendict import frozendict
 
 # Internal Imports
-from sanctify.constants import Constants, DefaultColumns
+from sanctify.constants import Constants, DefaultColumns, PrimitiveDataTypes
 from sanctify.utils import convert_stringified_list_to_list, replace_dict_keys
 
 
 class Cleanser:
     """
     The Cleanser class is responsible for validating and checking if a column is present and should be used.
     """
@@ -289,15 +289,16 @@
 
             # Get the optional column names in their raw form
             optional_columns_raw = cleanser.get_optional_column_names_from_column_mapping(return_standard_column_names=False)
         """
         optional_column_names = set()
         for raw_column_name, column_config in self.column_mapping_schema.items():
             if column_config.get(Constants.IS_OPTIONAL.value, False) is True:
-                if return_standard_column_names is True:
+                standard_column = column_config.get(Constants.STANDARD_COLUMN.value)
+                if return_standard_column_names is True and standard_column is not None:
                     optional_column_names.add(column_config.get(Constants.STANDARD_COLUMN.value))
                 else:
                     optional_column_names.add(raw_column_name)
         return optional_column_names
 
     def merge_data_type_schema_into_column_mapping_schema(self) -> frozendict:
         """
@@ -306,15 +307,15 @@
         Updates the column configuration in the column mapping schema with the corresponding data type configuration from the data type schema.
 
         Returns:
             A frozendict representing the merged column mapping schema, where the keys are the raw column names and the values are the updated column configurations.
         """
         merged_column_mapping_schema: dict[str:dict] = dict(self.column_mapping_schema)
         for _, column_config in merged_column_mapping_schema.items():
-            data_type = column_config.pop(Constants.DATA_TYPE.value, {})
+            data_type = column_config.get(Constants.DATA_TYPE.value, {})
             column_config |= self.data_type_schema.get(data_type, {})
         return frozendict(merged_column_mapping_schema)
 
     def coalesce_rows(self, merge_on: str, agg_col_modifier: str = "Child ") -> None:
         """
         ### Modifies Dataframe in place!
 
@@ -394,7 +395,24 @@
             self.df.loc[non_empty_mask, col] = self.df.loc[non_empty_mask, subcol]
 
         # Remove aggregated columns
         if remove_agg_cols is True:
             self.df = self.df.drop(columns=list(agg_cols_map.keys()), inplace=False)
 
         return self.df
+
+    def merge_same_data_type_column(self, merge_column_name: str) -> pd.DataFrame:
+        cell_phone_columns = [
+            key
+            for key, value in self.column_mapping_schema.items()
+            if merge_column_name == value.get(Constants.STANDARD_COLUMN.value)
+        ]
+
+        for col in cell_phone_columns[1:]:
+            self.df[cell_phone_columns[0]] = (
+                self.df[cell_phone_columns[0]].replace("", pd.NA).combine_first(self.df[col])
+            )
+            self.column_mapping_schema[col][Constants.DATA_TYPE.value] = PrimitiveDataTypes.STRING.value
+            self.column_mapping_schema[col].pop(Constants.STANDARD_COLUMN.value, None)
+        self.input_vs_standard_column_mapping = self.extract_input_vs_standard_column_mapping()
+
+        return self.df
```

### Comparing `sanctify-1.3.0/sanctify/constants.py` & `sanctify-1.4.0/sanctify/constants.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.3.0/sanctify/examples/column_mapping_schema.py` & `sanctify-1.4.0/sanctify/examples/column_mapping_schema.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.3.0/sanctify/examples/data_type_schema.py` & `sanctify-1.4.0/sanctify/examples/data_type_schema.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.3.0/sanctify/processor.py` & `sanctify-1.4.0/sanctify/processor.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.3.0/sanctify/serializer.py` & `sanctify-1.4.0/sanctify/serializer.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.3.0/sanctify/transformer.py` & `sanctify-1.4.0/sanctify/transformer.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.3.0/sanctify/utils.py` & `sanctify-1.4.0/sanctify/utils.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.3.0/sanctify/validator.py` & `sanctify-1.4.0/sanctify/validator.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.3.0/sanctify.egg-info/PKG-INFO` & `sanctify-1.4.0/sanctify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sanctify
-Version: 1.3.0
+Version: 1.4.0
 Summary: Column Mapping based cleansing and validations for a given pandas dataframe
 Author-email: Avijeet Diwaker <avijeetdiwaker@gmail.com>
 Project-URL: Homepage, https://github.com/skit-ai/sanctify
 Project-URL: Bug Tracker, https://github.com/skit-ai/sanctify/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

