# Comparing `tmp/fiboa-cli-0.1.1.tar.gz` & `tmp/fiboa-cli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiboa-cli-0.1.1.tar", last modified: Wed Mar 27 12:17:53 2024, max compression
+gzip compressed data, was "fiboa-cli-0.2.0.tar", last modified: Tue Apr  2 12:00:26 2024, max compression
```

## Comparing `fiboa-cli-0.1.1.tar` & `fiboa-cli-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 12:17:53.058531 fiboa-cli-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-27 12:17:26.000000 fiboa-cli-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-03-27 12:17:53.058531 fiboa-cli-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-03-27 12:17:26.000000 fiboa-cli-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 12:17:53.058531 fiboa-cli-0.1.1/fiboa_cli/
--rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-03-27 12:17:26.000000 fiboa-cli-0.1.1/fiboa_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-03-27 12:17:26.000000 fiboa-cli-0.1.1/fiboa_cli/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-03-27 12:17:26.000000 fiboa-cli-0.1.1/fiboa_cli/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-03-27 12:17:26.000000 fiboa-cli-0.1.1/fiboa_cli/describe.py
--rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-03-27 12:17:26.000000 fiboa-cli-0.1.1/fiboa_cli/geopandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-03-27 12:17:26.000000 fiboa-cli-0.1.1/fiboa_cli/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-27 12:17:26.000000 fiboa-cli-0.1.1/fiboa_cli/jsonschema_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-03-27 12:17:26.000000 fiboa-cli-0.1.1/fiboa_cli/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9291 2024-03-27 12:17:26.000000 fiboa-cli-0.1.1/fiboa_cli/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-03-27 12:17:26.000000 fiboa-cli-0.1.1/fiboa_cli/validate_data.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-27 12:17:26.000000 fiboa-cli-0.1.1/fiboa_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 12:17:53.058531 fiboa-cli-0.1.1/fiboa_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-03-27 12:17:53.000000 fiboa-cli-0.1.1/fiboa_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-03-27 12:17:53.000000 fiboa-cli-0.1.1/fiboa_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 12:17:53.000000 fiboa-cli-0.1.1/fiboa_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-27 12:17:53.000000 fiboa-cli-0.1.1/fiboa_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-27 12:17:53.000000 fiboa-cli-0.1.1/fiboa_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-27 12:17:53.000000 fiboa-cli-0.1.1/fiboa_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 12:17:53.058531 fiboa-cli-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-03-27 12:17:26.000000 fiboa-cli-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:00:26.418552 fiboa-cli-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-02 12:00:22.000000 fiboa-cli-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-02 12:00:26.418552 fiboa-cli-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-02 12:00:22.000000 fiboa-cli-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:00:26.414552 fiboa-cli-0.2.0/fiboa_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-04-02 12:00:22.000000 fiboa-cli-0.2.0/fiboa_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-02 12:00:22.000000 fiboa-cli-0.2.0/fiboa_cli/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-02 12:00:22.000000 fiboa-cli-0.2.0/fiboa_cli/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-02 12:00:22.000000 fiboa-cli-0.2.0/fiboa_cli/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-02 12:00:22.000000 fiboa-cli-0.2.0/fiboa_cli/describe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-04-02 12:00:22.000000 fiboa-cli-0.2.0/fiboa_cli/geopandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-04-02 12:00:22.000000 fiboa-cli-0.2.0/fiboa_cli/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-02 12:00:22.000000 fiboa-cli-0.2.0/fiboa_cli/jsonschema_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-04-02 12:00:22.000000 fiboa-cli-0.2.0/fiboa_cli/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-04-02 12:00:22.000000 fiboa-cli-0.2.0/fiboa_cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9578 2024-04-02 12:00:22.000000 fiboa-cli-0.2.0/fiboa_cli/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-02 12:00:22.000000 fiboa-cli-0.2.0/fiboa_cli/validate_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-02 12:00:22.000000 fiboa-cli-0.2.0/fiboa_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:00:26.418552 fiboa-cli-0.2.0/fiboa_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-02 12:00:26.000000 fiboa-cli-0.2.0/fiboa_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-02 12:00:26.000000 fiboa-cli-0.2.0/fiboa_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 12:00:26.000000 fiboa-cli-0.2.0/fiboa_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-02 12:00:26.000000 fiboa-cli-0.2.0/fiboa_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-02 12:00:26.000000 fiboa-cli-0.2.0/fiboa_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-02 12:00:26.000000 fiboa-cli-0.2.0/fiboa_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 12:00:26.418552 fiboa-cli-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-02 12:00:22.000000 fiboa-cli-0.2.0/setup.py
```

### Comparing `fiboa-cli-0.1.1/LICENSE` & `fiboa-cli-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.1.1/PKG-INFO` & `fiboa-cli-0.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiboa-cli
-Version: 0.1.1
+Version: 0.2.0
 Summary: CLI tools such as validation and file format conversion for fiboa.
 Home-page: https://github.com/fiboa/cli
 Author: Matthias Mohr
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -14,29 +14,31 @@
 Requires-Dist: pyarrow>=14.0
 Requires-Dist: fsspec>=2024.0
 Requires-Dist: click>=8.1
 Requires-Dist: geopandas>=0.14
 Requires-Dist: requests>=2.30
 Requires-Dist: aiohttp>=3.9
 Requires-Dist: shapely>=2.0
+Provides-Extra: de-nrw
 
 # fiboa CLI
 
 CLI tools such as validation and file format conversion for fiboa.
 
 ## Installation
 
-You need Python 3.9+ installed. 
+You need **Python 3.9+** installed. 
 Run `pip install fiboa-cli` to install the validator.
 
 ## Validation
 
 To validate a fiboa GeoParquet or GeoJSON file, you can for example run:
 
-`fiboa validate example.json --collection collection.json`
+- GeoJSON: `fiboa validate example.json --collection collection.json`
+- GeoParquet: `fiboa validate example.parquet --data`
 
 Check `fiboa validate --help` for more details.
 
 The validator also supports remote files.
 
 - `http://` or `https://`: no further configuration is needed.
 - `s3://`: `s3fs` needs to be installed (run `pip install .[s3]`) and you may need to set environment variables.
@@ -45,22 +47,47 @@
   By default, `gcsfs` will attempt to use your default gcloud credentials or, attempt to get credentials from the google metadata service, or fall back to anonymous access.
 
 ## Create fiboa GeoParquet from GeoJSON
 
 To create a fiboa-compliant GeoParquet for a fiboa-compliant set of GeoJSON files containing Features or FeatureCollections,
 you can for example run:
 
-`fiboa create geojson/example.json -o test.parquet -c geojson/collection.json`
+- `fiboa create geojson/example.json -o test.parquet -c geojson/collection.json`
 
 Check `fiboa create --help` for more details.
 
+## Inspect fiboa GeoParquet file
+
+To look into a fiboa GeoParquet file to get a rough understanding of the content, the following can be executed:
+
+- `fiboa describe example.parquet`
+
+Check `fiboa describe --help` for more details.
+
 ## Create JSON Schema from fiboa Schema
 
 To create a JSON Schema for a fiboa Schema YAML file, you can for example run:
 
-`fiboa jsonschema example.json --id=https://fiboa.github.io/specification/v0.1.0/geojson/schema.json -o schema.json`
+- `fiboa jsonschema example.json --id=https://fiboa.github.io/specification/v0.1.0/geojson/schema.json -o schema.json`
 
 Check `fiboa jsonschema --help` for more details.
 
+## Converter for existing datasets
+
+To convert an existing dataset to fiboa using the pre-defined converters:
+
+- `fiboa convert de_nrw`
+
+Available converters:
+- `de_nrw` (Germany, NRW from Shapefile)
+
+### Implement a converter
+
+1. Create a new file in `fiboa_cli/datasets` based on the `template.py`
+2. Implement the `convert()` function
+3. Add missing dependencies into a separate dependency group in `setup.py`
+4. Add the converter to the list above
+5. Create a PR to submit your converter for review
+
 ## Development
 
 To install in development mode run `pip install -e .` in this folder.
```

### Comparing `fiboa-cli-0.1.1/README.md` & `fiboa-cli-0.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # fiboa CLI
 
 CLI tools such as validation and file format conversion for fiboa.
 
 ## Installation
 
-You need Python 3.9+ installed. 
+You need **Python 3.9+** installed. 
 Run `pip install fiboa-cli` to install the validator.
 
 ## Validation
 
 To validate a fiboa GeoParquet or GeoJSON file, you can for example run:
 
-`fiboa validate example.json --collection collection.json`
+- GeoJSON: `fiboa validate example.json --collection collection.json`
+- GeoParquet: `fiboa validate example.parquet --data`
 
 Check `fiboa validate --help` for more details.
 
 The validator also supports remote files.
 
 - `http://` or `https://`: no further configuration is needed.
 - `s3://`: `s3fs` needs to be installed (run `pip install .[s3]`) and you may need to set environment variables.
@@ -24,22 +25,47 @@
   By default, `gcsfs` will attempt to use your default gcloud credentials or, attempt to get credentials from the google metadata service, or fall back to anonymous access.
 
 ## Create fiboa GeoParquet from GeoJSON
 
 To create a fiboa-compliant GeoParquet for a fiboa-compliant set of GeoJSON files containing Features or FeatureCollections,
 you can for example run:
 
-`fiboa create geojson/example.json -o test.parquet -c geojson/collection.json`
+- `fiboa create geojson/example.json -o test.parquet -c geojson/collection.json`
 
 Check `fiboa create --help` for more details.
 
+## Inspect fiboa GeoParquet file
+
+To look into a fiboa GeoParquet file to get a rough understanding of the content, the following can be executed:
+
+- `fiboa describe example.parquet`
+
+Check `fiboa describe --help` for more details.
+
 ## Create JSON Schema from fiboa Schema
 
 To create a JSON Schema for a fiboa Schema YAML file, you can for example run:
 
-`fiboa jsonschema example.json --id=https://fiboa.github.io/specification/v0.1.0/geojson/schema.json -o schema.json`
+- `fiboa jsonschema example.json --id=https://fiboa.github.io/specification/v0.1.0/geojson/schema.json -o schema.json`
 
 Check `fiboa jsonschema --help` for more details.
 
+## Converter for existing datasets
+
+To convert an existing dataset to fiboa using the pre-defined converters:
+
+- `fiboa convert de_nrw`
+
+Available converters:
+- `de_nrw` (Germany, NRW from Shapefile)
+
+### Implement a converter
+
+1. Create a new file in `fiboa_cli/datasets` based on the `template.py`
+2. Implement the `convert()` function
+3. Add missing dependencies into a separate dependency group in `setup.py`
+4. Add the converter to the list above
+5. Create a PR to submit your converter for review
+
 ## Development
 
 To install in development mode run `pip install -e .` in this folder.
```

### Comparing `fiboa-cli-0.1.1/fiboa_cli/__init__.py` & `fiboa-cli-0.2.0/fiboa_cli/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import click
 import sys
 
+from .convert import convert as convert_
 from .create import create as create_
 from .describe import describe as describe_
 from .jsonschema import jsonschema as jsonschema_
 from .validate import validate as validate_
-from .version import __version__
+from .version import __version__, fiboa_version
 from .util import log, check_ext_schema_for_cli, valid_file_for_cli, valid_file_for_cli_with_ext, valid_files_folders_for_cli
 
 @click.group()
 @click.version_option(version=__version__)
 def cli():
     """
     The fiboa CLI.
@@ -100,15 +101,15 @@
 
 ## CREATE
 @click.command()
 @click.argument('files', nargs=-1, callback=lambda ctx, param, value: valid_files_folders_for_cli(value, ["json", "geojson"]))
 @click.option(
     '--out', '-o',
     type=click.Path(exists=False),
-    help='File to write the file to. If not provided, prints the file to the STDOUT.',
+    help='File to write the file to.',
     required=True
 )
 @click.option(
     '--collection', '-c',
     callback=valid_file_for_cli,
     help='Points to the STAC collection that defines the fiboa version and extensions.',
     required=True
@@ -156,16 +157,16 @@
     type=click.Path(exists=False),
     help='File to write the file to. If not provided, prints the file to the STDOUT.',
     default=None
 )
 @click.option(
     '--fiboa-version', '-f',
     type=click.STRING,
-    help='The fiboa version to validate against. Defaults to 0.1.0.',
-    default='0.1.0'
+    help=f'The fiboa version to validate against. Defaults to {fiboa_version}.',
+    default=fiboa_version
 )
 @click.option(
     '--id',
     type=click.STRING,
     help='The JSON Schema $id to use for the schema. If not provided, the $id will be omitted.',
 )
 def jsonschema(schema, out, fiboa_version, id):
@@ -182,14 +183,36 @@
     try:
         jsonschema_(config)
     except Exception as e:
         log(e, "error")
         sys.exit(1)
 
 
+## CONVERT
+@click.command()
+@click.argument('dataset', nargs=1)
+@click.option(
+    '--out', '-o',
+    type=click.Path(exists=False),
+    help='File to write the GeoParquet file to.',
+    required=True
+)
+def convert(dataset, out):
+    """
+    Converts existing field boundary datasets to fiboa.
+    """
+    log(f"fiboa CLI {__version__} - Convert {dataset}\n", "success")
+    try:
+        convert_(dataset, out)
+    except Exception as e:
+        log(e, "error")
+        sys.exit(1)
+
+
 cli.add_command(describe)
 cli.add_command(validate)
 cli.add_command(create)
 cli.add_command(jsonschema)
+cli.add_command(convert)
 
 if __name__ == '__main__':
     cli()
```

### Comparing `fiboa-cli-0.1.1/fiboa_cli/const.py` & `fiboa-cli-0.2.0/fiboa_cli/const.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pyarrow as pa
 import pyarrow.types as pat
 import pandas as pd
 
+# fiboa datatypes to geopandas datatypes
 GP_TYPE_MAP = {
     "boolean": "bool",
     "int8": "int8",
     "uint8": "uint8",
     "int16": "int16",
     "uint16": "uint16",
     "int32": "int32",
@@ -21,14 +22,15 @@
     "enum": "category", # todo: check
     "date": "datetime64[D]",
     "date-time": lambda x: pd.to_datetime(x),
     "geometry": None, # not a column, don't convert geometry
     "bounding-box": None # todo
 }
 
+# fiboa datatypes to pyarrow datatypes
 PA_TYPE_MAP = {
     "boolean": pa.bool_(),
     "int8": pa.int8(),
     "uint8": pa.uint8(),
     "int16": pa.int16(),
     "uint16": pa.uint16(),
     "int32": pa.int32(),
@@ -44,14 +46,42 @@
     "enum": pa.string(), # todo: support other data types [ENUM (BYTE_ARRAY)]
     "date": pa.date32(),
     "date-time": pa.timestamp("ms", tz="UTC"),
     "geometry": pa.binary(),
     "bounding-box": None # todo
 }
 
+# geopandas datatypes to pyarrow datatypes
+GP_TO_PA_TYPE_MAP = {
+    "string": pa.string(),
+    "|S0": pa.string(), # todo
+    "<U0": pa.string(), # todo
+    "bool": pa.bool_(),
+    "int8": pa.int8(),
+    "uint8": pa.uint8(),
+    "int16": pa.int16(),
+    "uint16": pa.uint16(),
+    "int32": pa.int32(),
+    "uint32": pa.uint32(),
+    "int64": pa.int64(),
+    "uint64": pa.uint64(),
+    "float16": pa.float16(),
+    "float32": pa.float32(),
+    "float64": pa.float64(),
+    "float128": None, # todo
+    "complex64": None, # todo
+    "complex128": None, # todo
+    "complex256": None, # todo
+    "object": pa.string(),
+    "datetime64": pa.timestamp("ms", tz="UTC"),
+    "record": None, # todo
+    "timedelta64": None # todo
+}
+
+# checks pyarrow datatypes
 PA_TYPE_CHECK = {
     "boolean": pat.is_boolean,
     "int8": pat.is_int8,
     "uint8": pat.is_uint8,
     "int16": pat.is_int16,
     "uint16": pat.is_uint16,
     "int32": pat.is_int32,
```

### Comparing `fiboa-cli-0.1.1/fiboa_cli/create.py` & `fiboa-cli-0.2.0/fiboa_cli/parquet.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,23 @@
 import json
-import os
 import pyarrow as pa
 
-from .const import PA_TYPE_MAP, GP_TYPE_MAP
+from .const import PA_TYPE_MAP, GP_TYPE_MAP, GP_TO_PA_TYPE_MAP
 from .util import log, load_fiboa_schema, load_file
 from .geopandas import to_parquet
 from geopandas import GeoDataFrame
 from shapely.geometry import shape
 
-def create(config):
-    output_file = config.get("out")
-
-    # Add a STAC collection to the fiboa property to the Parquet metadata
-    collection = load_file(config.get("collection"))
-    if "id" not in collection or not collection["id"]:
-        collection["id"] = os.path.basename(output_file)
-    if "fiboa_version" not in collection:
-        raise Exception("No fiboa_version found in collection metadata")
-    else:
-        config["fiboa_version"] = collection["fiboa_version"]
-    # todo: fill with more/better metadata
-
-    # Load all features from the GeoJSON files
-    features = []
-    files = config.get("files")
-    for file in files:
-        geojson = load_file(file)
-        if geojson["type"] == "Feature":
-            features.append(geojson)
-        elif geojson["type"] == "FeatureCollection":
-            features += geojson["features"]
-        else:
-            log(f"{file}: Skipped - Unsupported GeoJSON type, must be Feature or FeatureCollection")
-
-    if len(features) == 0:
-        raise Exception("No valid features provided as input files")
-
-    properties = {}
+def create_parquet(data, columns, collection, output_file, config):
+    columns = list(columns)
+    columns.sort()
 
     # Load the data schema
     fiboa_schema = load_fiboa_schema(config)
+    properties = {}
     properties.update(fiboa_schema["properties"])
 
     # Load all extension schemas
     extensions = {}
     if "fiboa_extensions" in collection and isinstance(collection["fiboa_extensions"], list):
         ext_map = config.get("extension_schemas", [])
         for ext in collection["fiboa_extensions"]:
@@ -54,77 +28,81 @@
                 else:
                     path = ext
                 extensions[ext] = load_file(path)
                 properties.update(extensions[ext]["properties"])
             except Exception as e:
                 log(f"Extension schema for {ext} can't be loaded: {e}", "warning")
 
-    # Get a list of the properties/columns (without duplicates)
-    columns = set(["id", "geometry"])
-    for feature in features:
-        keys = feature["properties"].keys()
-        columns.update(keys)
+    # Create GeoDataFrame from the features
+    if not isinstance(data, GeoDataFrame):
+        data = features_to_dataframe(data, columns)
 
-    columns = list(columns)
-    columns.sort()
+    # Update the GeoDataFrame with the correct types etc.
+    data = update_dataframe(data, columns, properties)
 
     # Define the fields for the schema
     pq_fields = []
     for name in columns:
-        if not name in properties:
-            log(f"{name}: No schema defined", "warning")
-            continue
-        prop_schema = properties[name]
-        pa_type = create_type(prop_schema)
-        nullable = not prop_schema.get("required", False)
-        field = pa.field(name, pa_type, nullable = nullable)
+        if name in properties:
+            prop_schema = properties[name]
+            pa_type = create_type(prop_schema)
+            nullable = not prop_schema.get("required", False)
+            field = pa.field(name, pa_type, nullable = nullable)
+        else:
+            pd_type = str(data[name].dtype) # pandas data type
+            pa_type = GP_TO_PA_TYPE_MAP.get(pd_type, None) # pyarrow data type
+            if pa_type is not None:
+                log(f"{name}: No schema defined, converting {pd_type} to nullable {pa_type}", "warning")
+                field = pa.field(name, pa_type, nullable = True)
+            else:
+                log(f"{name}: No schema defined and converter doesn't support {pd_type}, skipping field", "warning")
+                continue
+
         pq_fields.append(field)
 
     # Define the schema for the Parquet file
     pq_schema = pa.schema(pq_fields)
     pq_schema = pq_schema.with_metadata({"fiboa": json.dumps(collection).encode("utf-8")})
 
-    # Create GeoDataFrame from the features
-    data = create_dataframe(features, columns, fiboa_schema)
-
     # Write the data to the Parquet file
     # Proprietary function exported from geopandas to solve
     # https://github.com/geopandas/geopandas/issues/3182
     to_parquet(
         data,
         output_file,
         schema = pq_schema,
         index = False,
         coerce_timestamps = "ms"
     )
 
-    log(f"Wrote to {output_file}", "success")
 
-def create_dataframe(features, columns, schema):
+def features_to_dataframe(features, columns):
     # Create a list of shapes
     rows = []
     for feature in features:
         id = feature["id"] if "id" in feature else None
         geometry = shape(feature["geometry"]) if "geometry" in feature else None
         row = {
             "id": id,
             "geometry": geometry,
         }
         properties = feature["properties"] if "properties" in feature else {}
         row.update(properties)
         rows.append(row)
 
     # Create the GeoDataFrame
-    data = GeoDataFrame(rows, columns=columns, geometry="geometry", crs="EPSG:4326")
+    return GeoDataFrame(rows, columns=columns, geometry="geometry", crs="EPSG:4326")
+
 
+def update_dataframe(data, columns, schema):
     # Convert the data to the correct types
     for column in columns:
-        if column not in schema["properties"]:
+        if column not in schema:
             continue
-        dtype = schema["properties"][column].get("type", None)
+        dtype = schema[column].get("type", None)
         if dtype == "geometry":
             continue
 
         gp_type = GP_TYPE_MAP.get(dtype, None)
         if gp_type is None:
             log(f"{column}: No type conversion available for {dtype}")
         elif callable(gp_type):
```

### Comparing `fiboa-cli-0.1.1/fiboa_cli/describe.py` & `fiboa-cli-0.2.0/fiboa_cli/describe.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,43 +12,43 @@
         return None
 
 
 def wkb_to_wkt(data):
     return wkb.loads(data)
 
 
-def describe(file, json):
+def describe(file, display_json=False):
     schema = load_parquet_schema(file)
 
     log("== GEOPARQUET ==", "success")
     geo = parse_metadata(schema, b"geo")
     geo_columns = []
     if geo:
         log(f"GeoParquet version: {geo['version']}")
 
         geo_columns = geo.get("columns", {}).keys()
         columns_str = ", ".join(geo_columns)
         log(f"Geometry columns: {columns_str}")
 
-        if (json):
+        if (display_json):
             log(json.dumps(geo, indent=2))
 
     log("\n== COLLECTION ==", "success")
     collection = parse_metadata(schema, b"fiboa")
     if collection:
         log(f"fiboa version: {collection['fiboa_version']}")
         if "fiboa_extensions" in collection and isinstance(collection["fiboa_extensions"], list):
             log("fiboa extensions:")
             for ext in collection["fiboa_extensions"]:
                 log(f"  - {ext}")
 
         if "license" in collection:
             log(f"license: {collection['license']}")
 
-        if (json):
+        if (display_json):
             log(json.dumps(collection, indent=2))
 
     log("\n== SCHEMA ==", "success")
     log(schema.to_string(show_schema_metadata=False))
 
     data = load_parquet_data(file)
     rowcount = len(data)
```

### Comparing `fiboa-cli-0.1.1/fiboa_cli/geopandas.py` & `fiboa-cli-0.2.0/fiboa_cli/geopandas.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.1.1/fiboa_cli/jsonschema.py` & `fiboa-cli-0.2.0/fiboa_cli/jsonschema.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.1.1/fiboa_cli/jsonschema_template.py` & `fiboa-cli-0.2.0/fiboa_cli/jsonschema_template.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.1.1/fiboa_cli/util.py` & `fiboa-cli-0.2.0/fiboa_cli/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,38 +6,66 @@
 import pandas as pd
 
 from urllib.parse import urlparse
 from fsspec import AbstractFileSystem
 from fsspec.implementations.http import HTTPFileSystem
 from fsspec.implementations.local import LocalFileSystem
 from pyarrow.fs import FSSpecHandler, PyFileSystem
+from tempfile import NamedTemporaryFile
 
 from .const import LOG_STATUS_COLOR, SUPPORTED_PROTOCOLS
 
-cache = {}
+small_file_cache = {}
+big_file_cache = {}
 
 def log(text: str, status="info"):
     """Log a message with a severity level (which leads to different colors)"""
     click.echo(click.style(text, fg=LOG_STATUS_COLOR[status]))
 
+
+def download_file(uri):
+    """Download files from various sources"""
+    if uri not in big_file_cache:
+        fs = get_fs(uri)
+        if isinstance(fs, LocalFileSystem):
+            big_file_cache[uri] = uri
+        else:
+            chunk_size = 10 * 1024 * 1024
+            _, extension = os.path.splitext(uri)
+            with NamedTemporaryFile(delete=False, suffix=extension) as tmp_file:
+                with fs.open(uri, mode='rb') as f:
+                    while True:
+                        chunk = f.read(chunk_size)
+                        if not chunk:
+                            break
+                        tmp_file.write(chunk)
+
+            big_file_cache[uri] = tmp_file.name
+
+    path = big_file_cache[uri]
+
+    return path
+
+
 def load_file(uri):
     """Load files from various sources"""
-    if uri in cache:
-        return cache[uri]
+    if uri in small_file_cache:
+        return small_file_cache[uri]
 
     fs = get_fs(uri)
+
     with fs.open(uri) as f:
         data = f.read()
 
     if uri.endswith(".yml") or uri.endswith(".yaml"):
         data = yaml.safe_load(data)
     elif uri.endswith(".json") or uri.endswith(".geojson"):
         data = json.loads(data)
 
-    cache[uri] = data
+    small_file_cache[uri] = data
 
     return data
 
 def get_pyarrow_file(uri):
     fs = get_fs(uri)
     pyarrow_fs = PyFileSystem(FSSpecHandler(fs))
     return pyarrow_fs.open_input_file(uri)
```

### Comparing `fiboa-cli-0.1.1/fiboa_cli/validate.py` & `fiboa-cli-0.2.0/fiboa_cli/validate.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,14 +190,21 @@
             valid = False
 
     # Compile all properties from the schemas
     properties = fiboa_schema["properties"]
     for ext in extensions.values():
         properties.update(ext["properties"])
 
+    # Check that all required fields are present
+    for key, schema in properties.items():
+        required = schema.get("required", False)
+        if required and key not in parquet_schema.names:
+            log(f"{key}: Required field is missing", "error")
+            valid = False
+
     # Validate whether the Parquet schema complies with the property schemas
     for key in parquet_schema.names:
         # Ignore fields without a schema
         if key not in properties:
             log(f"{key}: No schema defined")
             continue
```

### Comparing `fiboa-cli-0.1.1/fiboa_cli/validate_data.py` & `fiboa-cli-0.2.0/fiboa_cli/validate_data.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.1.1/fiboa_cli.egg-info/PKG-INFO` & `fiboa-cli-0.2.0/fiboa_cli.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiboa-cli
-Version: 0.1.1
+Version: 0.2.0
 Summary: CLI tools such as validation and file format conversion for fiboa.
 Home-page: https://github.com/fiboa/cli
 Author: Matthias Mohr
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -14,29 +14,31 @@
 Requires-Dist: pyarrow>=14.0
 Requires-Dist: fsspec>=2024.0
 Requires-Dist: click>=8.1
 Requires-Dist: geopandas>=0.14
 Requires-Dist: requests>=2.30
 Requires-Dist: aiohttp>=3.9
 Requires-Dist: shapely>=2.0
+Provides-Extra: de-nrw
 
 # fiboa CLI
 
 CLI tools such as validation and file format conversion for fiboa.
 
 ## Installation
 
-You need Python 3.9+ installed. 
+You need **Python 3.9+** installed. 
 Run `pip install fiboa-cli` to install the validator.
 
 ## Validation
 
 To validate a fiboa GeoParquet or GeoJSON file, you can for example run:
 
-`fiboa validate example.json --collection collection.json`
+- GeoJSON: `fiboa validate example.json --collection collection.json`
+- GeoParquet: `fiboa validate example.parquet --data`
 
 Check `fiboa validate --help` for more details.
 
 The validator also supports remote files.
 
 - `http://` or `https://`: no further configuration is needed.
 - `s3://`: `s3fs` needs to be installed (run `pip install .[s3]`) and you may need to set environment variables.
@@ -45,22 +47,47 @@
   By default, `gcsfs` will attempt to use your default gcloud credentials or, attempt to get credentials from the google metadata service, or fall back to anonymous access.
 
 ## Create fiboa GeoParquet from GeoJSON
 
 To create a fiboa-compliant GeoParquet for a fiboa-compliant set of GeoJSON files containing Features or FeatureCollections,
 you can for example run:
 
-`fiboa create geojson/example.json -o test.parquet -c geojson/collection.json`
+- `fiboa create geojson/example.json -o test.parquet -c geojson/collection.json`
 
 Check `fiboa create --help` for more details.
 
+## Inspect fiboa GeoParquet file
+
+To look into a fiboa GeoParquet file to get a rough understanding of the content, the following can be executed:
+
+- `fiboa describe example.parquet`
+
+Check `fiboa describe --help` for more details.
+
 ## Create JSON Schema from fiboa Schema
 
 To create a JSON Schema for a fiboa Schema YAML file, you can for example run:
 
-`fiboa jsonschema example.json --id=https://fiboa.github.io/specification/v0.1.0/geojson/schema.json -o schema.json`
+- `fiboa jsonschema example.json --id=https://fiboa.github.io/specification/v0.1.0/geojson/schema.json -o schema.json`
 
 Check `fiboa jsonschema --help` for more details.
 
+## Converter for existing datasets
+
+To convert an existing dataset to fiboa using the pre-defined converters:
+
+- `fiboa convert de_nrw`
+
+Available converters:
+- `de_nrw` (Germany, NRW from Shapefile)
+
+### Implement a converter
+
+1. Create a new file in `fiboa_cli/datasets` based on the `template.py`
+2. Implement the `convert()` function
+3. Add missing dependencies into a separate dependency group in `setup.py`
+4. Add the converter to the list above
+5. Create a PR to submit your converter for review
+
 ## Development
 
 To install in development mode run `pip install -e .` in this folder.
```

