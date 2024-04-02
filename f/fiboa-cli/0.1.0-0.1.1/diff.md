# Comparing `tmp/fiboa-cli-0.1.0.tar.gz` & `tmp/fiboa-cli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiboa-cli-0.1.0.tar", last modified: Wed Mar 27 10:43:35 2024, max compression
+gzip compressed data, was "fiboa-cli-0.1.1.tar", last modified: Wed Mar 27 12:17:53 2024, max compression
```

## Comparing `fiboa-cli-0.1.0.tar` & `fiboa-cli-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:43:35.824633 fiboa-cli-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-27 10:43:31.000000 fiboa-cli-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-03-27 10:43:35.824633 fiboa-cli-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-03-27 10:43:31.000000 fiboa-cli-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:43:35.820633 fiboa-cli-0.1.0/fiboa_cli/
--rw-r--r--   0 runner    (1001) docker     (127)     5964 2024-03-27 10:43:31.000000 fiboa-cli-0.1.0/fiboa_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-03-27 10:43:31.000000 fiboa-cli-0.1.0/fiboa_cli/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-03-27 10:43:31.000000 fiboa-cli-0.1.0/fiboa_cli/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-03-27 10:43:31.000000 fiboa-cli-0.1.0/fiboa_cli/describe.py
--rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-03-27 10:43:31.000000 fiboa-cli-0.1.0/fiboa_cli/geopandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-03-27 10:43:31.000000 fiboa-cli-0.1.0/fiboa_cli/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-27 10:43:31.000000 fiboa-cli-0.1.0/fiboa_cli/jsonschema_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-03-27 10:43:31.000000 fiboa-cli-0.1.0/fiboa_cli/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-03-27 10:43:31.000000 fiboa-cli-0.1.0/fiboa_cli/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-27 10:43:31.000000 fiboa-cli-0.1.0/fiboa_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:43:35.824633 fiboa-cli-0.1.0/fiboa_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-03-27 10:43:35.000000 fiboa-cli-0.1.0/fiboa_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-27 10:43:35.000000 fiboa-cli-0.1.0/fiboa_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 10:43:35.000000 fiboa-cli-0.1.0/fiboa_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-27 10:43:35.000000 fiboa-cli-0.1.0/fiboa_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-27 10:43:35.000000 fiboa-cli-0.1.0/fiboa_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-27 10:43:35.000000 fiboa-cli-0.1.0/fiboa_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 10:43:35.824633 fiboa-cli-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-03-27 10:43:31.000000 fiboa-cli-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 12:17:53.058531 fiboa-cli-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-27 12:17:26.000000 fiboa-cli-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-03-27 12:17:53.058531 fiboa-cli-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-03-27 12:17:26.000000 fiboa-cli-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 12:17:53.058531 fiboa-cli-0.1.1/fiboa_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-03-27 12:17:26.000000 fiboa-cli-0.1.1/fiboa_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-03-27 12:17:26.000000 fiboa-cli-0.1.1/fiboa_cli/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-03-27 12:17:26.000000 fiboa-cli-0.1.1/fiboa_cli/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-03-27 12:17:26.000000 fiboa-cli-0.1.1/fiboa_cli/describe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-03-27 12:17:26.000000 fiboa-cli-0.1.1/fiboa_cli/geopandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-03-27 12:17:26.000000 fiboa-cli-0.1.1/fiboa_cli/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-27 12:17:26.000000 fiboa-cli-0.1.1/fiboa_cli/jsonschema_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-03-27 12:17:26.000000 fiboa-cli-0.1.1/fiboa_cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9291 2024-03-27 12:17:26.000000 fiboa-cli-0.1.1/fiboa_cli/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-03-27 12:17:26.000000 fiboa-cli-0.1.1/fiboa_cli/validate_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-27 12:17:26.000000 fiboa-cli-0.1.1/fiboa_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 12:17:53.058531 fiboa-cli-0.1.1/fiboa_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-03-27 12:17:53.000000 fiboa-cli-0.1.1/fiboa_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-03-27 12:17:53.000000 fiboa-cli-0.1.1/fiboa_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 12:17:53.000000 fiboa-cli-0.1.1/fiboa_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-27 12:17:53.000000 fiboa-cli-0.1.1/fiboa_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-27 12:17:53.000000 fiboa-cli-0.1.1/fiboa_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-27 12:17:53.000000 fiboa-cli-0.1.1/fiboa_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 12:17:53.058531 fiboa-cli-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-03-27 12:17:26.000000 fiboa-cli-0.1.1/setup.py
```

### Comparing `fiboa-cli-0.1.0/LICENSE` & `fiboa-cli-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.1.0/PKG-INFO` & `fiboa-cli-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiboa-cli
-Version: 0.1.0
+Version: 0.1.1
 Summary: CLI tools such as validation and file format conversion for fiboa.
 Home-page: https://github.com/fiboa/cli
 Author: Matthias Mohr
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `fiboa-cli-0.1.0/README.md` & `fiboa-cli-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.1.0/fiboa_cli/__init__.py` & `fiboa-cli-0.1.1/fiboa_cli/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     help='Points to the STAC collection that defines the fiboa version and extensions.',
     default=None
 )
 @click.option(
     '--data', '-d',
     is_flag=True,
     type=click.BOOL,
-    help='Validate the data in the GeoParquet file. Enabling this might be slow. Default is False.',
+    help='EXPERIMENTAL: Validate the data in the GeoParquet file. Enabling this might be slow or exceed memory. Default is False.',
     default=False
 )
 def validate(files, schema, ext_schema, fiboa_version, collection, data):
     """
     Validates a fiboa GeoParquet or GeoJSON file.
     """
     log(f"fiboa CLI {__version__} - Validator\n", "success")
```

### Comparing `fiboa-cli-0.1.0/fiboa_cli/const.py` & `fiboa-cli-0.1.1/fiboa_cli/const.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.1.0/fiboa_cli/create.py` & `fiboa-cli-0.1.1/fiboa_cli/create.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.1.0/fiboa_cli/describe.py` & `fiboa-cli-0.1.1/fiboa_cli/describe.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.1.0/fiboa_cli/geopandas.py` & `fiboa-cli-0.1.1/fiboa_cli/geopandas.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.1.0/fiboa_cli/jsonschema.py` & `fiboa-cli-0.1.1/fiboa_cli/jsonschema.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.1.0/fiboa_cli/jsonschema_template.py` & `fiboa-cli-0.1.1/fiboa_cli/jsonschema_template.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.1.0/fiboa_cli/util.py` & `fiboa-cli-0.1.1/fiboa_cli/util.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.1.0/fiboa_cli/validate.py` & `fiboa-cli-0.1.1/fiboa_cli/validate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import json
 import pyarrow.types as pat
 import geopandas as gpd
 
 from jsonschema.validators import Draft7Validator
 from .const import PA_TYPE_CHECK
 from .jsonschema import create_jsonschema
-from .util import log as log_, load_datatypes, load_file, load_fiboa_schema, load_parquet_schema
+from .util import log as log_, load_datatypes, load_file, load_fiboa_schema, load_parquet_data, load_parquet_schema
+from .validate_data import validate_column
 
 STAC_COLLECTION_SCHEMA = "http://schemas.stacspec.org/v1.0.0/collection-spec/json-schema/collection.json"
 
 def log(text: str, status="info"):
     # Indent logs
     log_("  - " + text, status)
 
@@ -175,14 +176,23 @@
 
     # Validate Collection
     valid, extensions = validate_collection(collection, config)
 
     # load the actual fiboa schema
     fiboa_schema = load_fiboa_schema(config)
 
+    # Load data if needed
+    df = None
+    if config.get("data"):
+        try:
+            df = load_parquet_data(file)
+        except Exception as e:
+            log(f"Data could not be read: {e}", "error")
+            valid = False
+
     # Compile all properties from the schemas
     properties = fiboa_schema["properties"]
     for ext in extensions.values():
         properties.update(ext["properties"])
 
     # Validate whether the Parquet schema complies with the property schemas
     for key in parquet_schema.names:
@@ -225,34 +235,29 @@
                 log(f"{key}: Timestamp timezone invalid, must be UTC", "error")
                 valid = False
         elif dtype == "object":
             if not pat.is_string(pq_field.key_type):
                 log(f"{key}: Map key datatype is not string", "error")
                 valid = False
 
-    if config.get("data"):
-        if not validate_data(file, config):
-            valid = False
-    else:
+        # Validate data of the column
+        if df is not None:
+            issues = validate_column(df[key], prop_schema)
+            if len(issues) > 0:
+                for issue in issues:
+                    log(f"{key}: {issue}")
+                valid = False
+
+    # Show a note once if data was not validated
+    if not config.get("data"):
         log("Data was not validated as the --data parameter was not provided", "info")
 
     return valid
 
 
-def validate_data(file, config):
-    # todo: validate data
-    try:
-        df = gpd.read_parquet(file)
-    except Exception as e:
-        log(f"Data could not be read: {e}", "error")
-        return False
-
-    log("Reading the file succeeded, but detailed data validation is not implemented yet", "warning")
-
-
 # todo: use stac_validator instead of our own validation routine
 def validate_colletion_schema(obj):
     schema = load_file(STAC_COLLECTION_SCHEMA)
     errors = validate_json_schema(obj, schema)
     for error in errors:
         log(f"Collection: {error.path}: {error.message}", "error")
```

### Comparing `fiboa-cli-0.1.0/fiboa_cli.egg-info/PKG-INFO` & `fiboa-cli-0.1.1/fiboa_cli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiboa-cli
-Version: 0.1.0
+Version: 0.1.1
 Summary: CLI tools such as validation and file format conversion for fiboa.
 Home-page: https://github.com/fiboa/cli
 Author: Matthias Mohr
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `fiboa-cli-0.1.0/setup.py` & `fiboa-cli-0.1.1/setup.py`

 * *Files identical despite different names*

