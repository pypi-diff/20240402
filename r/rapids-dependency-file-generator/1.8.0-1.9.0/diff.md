# Comparing `tmp/rapids-dependency-file-generator-1.8.0.tar.gz` & `tmp/rapids-dependency-file-generator-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapids-dependency-file-generator-1.8.0.tar", last modified: Thu Dec 14 06:15:00 2023, max compression
+gzip compressed data, was "rapids-dependency-file-generator-1.9.0.tar", last modified: Thu Feb 22 17:55:46 2024, max compression
```

## Comparing `rapids-dependency-file-generator-1.8.0.tar` & `rapids-dependency-file-generator-1.9.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 06:15:00.311737 rapids-dependency-file-generator-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11348 2023-12-14 06:14:43.000000 rapids-dependency-file-generator-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-12-14 06:14:43.000000 rapids-dependency-file-generator-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    28419 2023-12-14 06:15:00.311737 rapids-dependency-file-generator-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14923 2023-12-14 06:14:43.000000 rapids-dependency-file-generator-1.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      984 2023-12-14 06:14:43.000000 rapids-dependency-file-generator-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-14 06:15:00.311737 rapids-dependency-file-generator-1.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 06:15:00.303737 rapids-dependency-file-generator-1.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 06:15:00.307737 rapids-dependency-file-generator-1.8.0/src/rapids_dependency_file_generator/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-12-14 06:14:43.000000 rapids-dependency-file-generator-1.8.0/src/rapids_dependency_file_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-14 06:14:52.000000 rapids-dependency-file-generator-1.8.0/src/rapids_dependency_file_generator/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3237 2023-12-14 06:14:43.000000 rapids-dependency-file-generator-1.8.0/src/rapids_dependency_file_generator/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2023-12-14 06:14:43.000000 rapids-dependency-file-generator-1.8.0/src/rapids_dependency_file_generator/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    17515 2023-12-14 06:14:43.000000 rapids-dependency-file-generator-1.8.0/src/rapids_dependency_file_generator/rapids_dependency_file_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-12-14 06:14:43.000000 rapids-dependency-file-generator-1.8.0/src/rapids_dependency_file_generator/rapids_dependency_file_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6294 2023-12-14 06:14:52.000000 rapids-dependency-file-generator-1.8.0/src/rapids_dependency_file_generator/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 06:15:00.311737 rapids-dependency-file-generator-1.8.0/src/rapids_dependency_file_generator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    28419 2023-12-14 06:15:00.000000 rapids-dependency-file-generator-1.8.0/src/rapids_dependency_file_generator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      902 2023-12-14 06:15:00.000000 rapids-dependency-file-generator-1.8.0/src/rapids_dependency_file_generator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-14 06:15:00.000000 rapids-dependency-file-generator-1.8.0/src/rapids_dependency_file_generator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2023-12-14 06:15:00.000000 rapids-dependency-file-generator-1.8.0/src/rapids_dependency_file_generator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-14 06:15:00.000000 rapids-dependency-file-generator-1.8.0/src/rapids_dependency_file_generator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-14 06:15:00.000000 rapids-dependency-file-generator-1.8.0/src/rapids_dependency_file_generator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 06:15:00.311737 rapids-dependency-file-generator-1.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      938 2023-12-14 06:14:43.000000 rapids-dependency-file-generator-1.8.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3706 2023-12-14 06:14:43.000000 rapids-dependency-file-generator-1.8.0/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     3546 2023-12-14 06:14:43.000000 rapids-dependency-file-generator-1.8.0/tests/test_rapids_dependency_file_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2023-12-14 06:14:43.000000 rapids-dependency-file-generator-1.8.0/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 17:55:46.938926 rapids-dependency-file-generator-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-02-22 17:55:28.000000 rapids-dependency-file-generator-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-02-22 17:55:28.000000 rapids-dependency-file-generator-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    28806 2024-02-22 17:55:46.938926 rapids-dependency-file-generator-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15310 2024-02-22 17:55:28.000000 rapids-dependency-file-generator-1.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-02-22 17:55:28.000000 rapids-dependency-file-generator-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 17:55:46.938926 rapids-dependency-file-generator-1.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 17:55:46.934926 rapids-dependency-file-generator-1.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 17:55:46.934926 rapids-dependency-file-generator-1.9.0/src/rapids_dependency_file_generator/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-22 17:55:28.000000 rapids-dependency-file-generator-1.9.0/src/rapids_dependency_file_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-22 17:55:39.000000 rapids-dependency-file-generator-1.9.0/src/rapids_dependency_file_generator/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-02-22 17:55:28.000000 rapids-dependency-file-generator-1.9.0/src/rapids_dependency_file_generator/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-02-22 17:55:28.000000 rapids-dependency-file-generator-1.9.0/src/rapids_dependency_file_generator/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17618 2024-02-22 17:55:28.000000 rapids-dependency-file-generator-1.9.0/src/rapids_dependency_file_generator/rapids_dependency_file_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-02-22 17:55:28.000000 rapids-dependency-file-generator-1.9.0/src/rapids_dependency_file_generator/rapids_dependency_file_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-02-22 17:55:39.000000 rapids-dependency-file-generator-1.9.0/src/rapids_dependency_file_generator/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 17:55:46.938926 rapids-dependency-file-generator-1.9.0/src/rapids_dependency_file_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28806 2024-02-22 17:55:46.000000 rapids-dependency-file-generator-1.9.0/src/rapids_dependency_file_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-02-22 17:55:46.000000 rapids-dependency-file-generator-1.9.0/src/rapids_dependency_file_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 17:55:46.000000 rapids-dependency-file-generator-1.9.0/src/rapids_dependency_file_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-22 17:55:46.000000 rapids-dependency-file-generator-1.9.0/src/rapids_dependency_file_generator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-22 17:55:46.000000 rapids-dependency-file-generator-1.9.0/src/rapids_dependency_file_generator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-22 17:55:46.000000 rapids-dependency-file-generator-1.9.0/src/rapids_dependency_file_generator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 17:55:46.938926 rapids-dependency-file-generator-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-02-22 17:55:28.000000 rapids-dependency-file-generator-1.9.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-02-22 17:55:28.000000 rapids-dependency-file-generator-1.9.0/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-02-22 17:55:28.000000 rapids-dependency-file-generator-1.9.0/tests/test_rapids_dependency_file_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-22 17:55:28.000000 rapids-dependency-file-generator-1.9.0/tests/test_schema.py
```

### Comparing `rapids-dependency-file-generator-1.8.0/LICENSE` & `rapids-dependency-file-generator-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rapids-dependency-file-generator-1.8.0/PKG-INFO` & `rapids-dependency-file-generator-1.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapids-dependency-file-generator
-Version: 1.8.0
+Version: 1.9.0
 Summary: Tool for generating RAPIDS environment files
 Author-email: RAPIDS Development Team <pypi@rapids.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -546,14 +546,18 @@
 # install cudf packages built in CI and test them in newly created environment...
 ```
 
 The `--file_key` argument is passed the `test` key name from the `files` configuration. Additional flags are used to generate a single dependency file. When the CLI is used in this fashion, it will print to `stdout` instead of writing the resulting contents to the filesystem.
 
 The `--file_key`, `--output`, and `--matrix` flags must be used together. `--matrix` may be an empty string if the file that should be generated does not depend on any specific matrix variations.
 
+The `--prepend-channels` argument accepts a semi-colon separated list of additional channels to use, like `rapids-dependency-file-generator --prepend-channels "my_channel;my_other_channel"`.
+If both `--output` and `--prepend-channels` are provided, the output format must be conda.
+Prepending channels can be useful for adding local channels with packages to be tested in CI workflows.
+
 Running `rapids-dependency-file-generator -h` will show the most up-to-date CLI arguments.
 
 ## Examples
 
 The [tests/examples](./tests/examples/) directory has example `dependencies.yaml` files along with their corresponding output files.
 
 To create new `example` tests do the following:
```

### Comparing `rapids-dependency-file-generator-1.8.0/README.md` & `rapids-dependency-file-generator-1.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -329,14 +329,18 @@
 # install cudf packages built in CI and test them in newly created environment...
 ```
 
 The `--file_key` argument is passed the `test` key name from the `files` configuration. Additional flags are used to generate a single dependency file. When the CLI is used in this fashion, it will print to `stdout` instead of writing the resulting contents to the filesystem.
 
 The `--file_key`, `--output`, and `--matrix` flags must be used together. `--matrix` may be an empty string if the file that should be generated does not depend on any specific matrix variations.
 
+The `--prepend-channels` argument accepts a semi-colon separated list of additional channels to use, like `rapids-dependency-file-generator --prepend-channels "my_channel;my_other_channel"`.
+If both `--output` and `--prepend-channels` are provided, the output format must be conda.
+Prepending channels can be useful for adding local channels with packages to be tested in CI workflows.
+
 Running `rapids-dependency-file-generator -h` will show the most up-to-date CLI arguments.
 
 ## Examples
 
 The [tests/examples](./tests/examples/) directory has example `dependencies.yaml` files along with their corresponding output files.
 
 To create new `example` tests do the following:
```

### Comparing `rapids-dependency-file-generator-1.8.0/pyproject.toml` & `rapids-dependency-file-generator-1.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rapids-dependency-file-generator-1.8.0/src/rapids_dependency_file_generator/constants.py` & `rapids-dependency-file-generator-1.9.0/src/rapids_dependency_file_generator/constants.py`

 * *Files identical despite different names*

### Comparing `rapids-dependency-file-generator-1.8.0/src/rapids_dependency_file_generator/rapids_dependency_file_generator.py` & `rapids-dependency-file-generator-1.9.0/src/rapids_dependency_file_generator/rapids_dependency_file_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,24 +17,24 @@
 )
 
 OUTPUT_ENUM_VALUES = [str(x) for x in OutputTypes]
 NON_NONE_OUTPUT_ENUM_VALUES = [str(x) for x in OutputTypes if not x == OutputTypes.NONE]
 HEADER = f"# This file is generated by `{cli_name}`."
 
 
-def delete_existing_files(root="."):
+def delete_existing_files(root: str) -> None:
     """Delete any files generated by this generator.
 
     This function can be used to clean up a directory tree before generating a new set
     of files from scratch.
 
     Parameters
     ----------
     root : str
-        The path to the root of the directory tree to search for files to delete.
+        The path (relative or absolute) to the root of the directory tree to search for files to delete.
     """
     for dirpath, _, filenames in os.walk(root):
         for fn in filter(
             lambda fn: fn.endswith(".txt") or fn.endswith(".yaml"), filenames
         ):
             with open(file_path := os.path.join(dirpath, fn)) as f:
                 try:
@@ -89,15 +89,15 @@
         combinations of parameter values from `gridspec`.
     """
     for values in itertools.product(*gridspec.values()):
         yield dict(zip(gridspec.keys(), values))
 
 
 def make_dependency_file(
-    file_type, name, config_file, output_dir, conda_channels, dependencies, extras=None
+    *, file_type, name, config_file, output_dir, conda_channels, dependencies, extras
 ):
     """Generate the contents of the dependency file.
 
     Parameters
     ----------
     file_type : str
         A string corresponding to the value of a member of constants.OutputTypes.
@@ -436,21 +436,21 @@
 
                 output_dir = (
                     "."
                     if to_stdout
                     else get_output_dir(file_type, config_file_path, file_config)
                 )
                 contents = make_dependency_file(
-                    file_type,
-                    full_file_name,
-                    config_file_path,
-                    output_dir,
-                    channels,
-                    deduped_deps,
-                    extras,
+                    file_type=file_type,
+                    name=full_file_name,
+                    config_file=config_file_path,
+                    output_dir=output_dir,
+                    conda_channels=channels,
+                    dependencies=deduped_deps,
+                    extras=extras,
                 )
 
                 if to_stdout:
                     print(contents)
                 else:
                     os.makedirs(output_dir, exist_ok=True)
                     file_path = os.path.join(output_dir, full_file_name)
```

### Comparing `rapids-dependency-file-generator-1.8.0/src/rapids_dependency_file_generator/rapids_dependency_file_validator.py` & `rapids-dependency-file-generator-1.9.0/src/rapids_dependency_file_generator/rapids_dependency_file_validator.py`

 * *Files identical despite different names*

### Comparing `rapids-dependency-file-generator-1.8.0/src/rapids_dependency_file_generator/schema.json` & `rapids-dependency-file-generator-1.9.0/src/rapids_dependency_file_generator/schema.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'$id'": "'https://raw.githubusercontent.com/rapidsai/dependency-file-generator/v1.9.0/src/rapids_dependency_file_generator/schema.json'"}*

```diff
@@ -166,15 +166,15 @@
             "items": {
                 "$ref": "#/$defs/requirement"
             },
             "minItems": 1,
             "type": "array"
         }
     },
-    "$id": "https://raw.githubusercontent.com/rapidsai/dependency-file-generator/v1.8.0/src/rapids_dependency_file_generator/schema.json",
+    "$id": "https://raw.githubusercontent.com/rapidsai/dependency-file-generator/v1.9.0/src/rapids_dependency_file_generator/schema.json",
     "$schema": "http://json-schema.org/draft-07/schema#",
     "additionalProperties": false,
     "description": "Consolidated specification of RAPIDS project dependencies",
     "properties": {
         "channels": {
             "$ref": "#/$defs/channels"
         },
```

### Comparing `rapids-dependency-file-generator-1.8.0/src/rapids_dependency_file_generator.egg-info/PKG-INFO` & `rapids-dependency-file-generator-1.9.0/src/rapids_dependency_file_generator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapids-dependency-file-generator
-Version: 1.8.0
+Version: 1.9.0
 Summary: Tool for generating RAPIDS environment files
 Author-email: RAPIDS Development Team <pypi@rapids.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -546,14 +546,18 @@
 # install cudf packages built in CI and test them in newly created environment...
 ```
 
 The `--file_key` argument is passed the `test` key name from the `files` configuration. Additional flags are used to generate a single dependency file. When the CLI is used in this fashion, it will print to `stdout` instead of writing the resulting contents to the filesystem.
 
 The `--file_key`, `--output`, and `--matrix` flags must be used together. `--matrix` may be an empty string if the file that should be generated does not depend on any specific matrix variations.
 
+The `--prepend-channels` argument accepts a semi-colon separated list of additional channels to use, like `rapids-dependency-file-generator --prepend-channels "my_channel;my_other_channel"`.
+If both `--output` and `--prepend-channels` are provided, the output format must be conda.
+Prepending channels can be useful for adding local channels with packages to be tested in CI workflows.
+
 Running `rapids-dependency-file-generator -h` will show the most up-to-date CLI arguments.
 
 ## Examples
 
 The [tests/examples](./tests/examples/) directory has example `dependencies.yaml` files along with their corresponding output files.
 
 To create new `example` tests do the following:
```

### Comparing `rapids-dependency-file-generator-1.8.0/src/rapids_dependency_file_generator.egg-info/SOURCES.txt` & `rapids-dependency-file-generator-1.9.0/src/rapids_dependency_file_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rapids-dependency-file-generator-1.8.0/tests/test_examples.py` & `rapids-dependency-file-generator-1.9.0/tests/test_examples.py`

 * *Files 18% similar despite different names*

```diff
@@ -59,22 +59,26 @@
             if filename == "pyproject.toml":
                 full_path = pathlib.Path(dirpath) / filename
                 relative_path = full_path.relative_to(expected_dir)
                 new_path = actual_dir / relative_path
                 new_path.parent.mkdir(parents=True, exist_ok=True)
                 shutil.copyfile(full_path, new_path)
 
-    main(
-        [
-            "--config",
-            str(dep_file_path),
-            "--clean",
-            str(example_dir.joinpath("output", "actual")),
-        ]
-    )
+    cli_args = [
+        "--config",
+        str(dep_file_path),
+        "--clean",
+        str(example_dir.joinpath("output", "actual")),
+    ]
+
+    # Prepend channels for the prepend_channels tests
+    if example_dir.name in ("prepend-channels"):
+        cli_args = ["--prepend-channels", "my_channel;my_other_channel"] + cli_args
+
+    main(cli_args)
 
     expected_file_set = make_file_set(expected_dir)
     actual_file_set = make_file_set(actual_dir)
 
     assert expected_file_set == actual_file_set
 
     for file in actual_file_set:
```

### Comparing `rapids-dependency-file-generator-1.8.0/tests/test_rapids_dependency_file_generator.py` & `rapids-dependency-file-generator-1.9.0/tests/test_rapids_dependency_file_generator.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,36 +36,38 @@
     relpath = "../../config_file.yaml"
     mock_relpath.return_value = relpath
     header = f"""\
 # This file is generated by `{cli_name}`.
 # To make changes, edit {relpath} and run `{cli_name}`.
 """
     env = make_dependency_file(
-        "conda",
-        "tmp_env.yaml",
-        "config_file",
-        "output_path",
-        ["rapidsai", "nvidia"],
-        ["dep1", "dep2"],
+        file_type="conda",
+        name="tmp_env.yaml",
+        config_file="config_file",
+        output_dir="output_path",
+        conda_channels=["rapidsai", "nvidia"],
+        dependencies=["dep1", "dep2"],
+        extras=None,
     )
     assert env == header + yaml.dump(
         {
             "name": "tmp_env",
             "channels": ["rapidsai", "nvidia"],
             "dependencies": ["dep1", "dep2"],
         }
     )
 
     env = make_dependency_file(
-        "requirements",
-        "tmp_env.txt",
-        "config_file",
-        "output_path",
-        ["rapidsai", "nvidia"],
-        ["dep1", "dep2"],
+        file_type="requirements",
+        name="tmp_env.txt",
+        config_file="config_file",
+        output_dir="output_path",
+        conda_channels=["rapidsai", "nvidia"],
+        dependencies=["dep1", "dep2"],
+        extras=None,
     )
     assert env == header + "dep1\ndep2\n"
 
 
 def test_should_use_specific_entry():
     # no match
     matrix_combo = {"cuda": "11.5", "arch": "x86_64"}
```

