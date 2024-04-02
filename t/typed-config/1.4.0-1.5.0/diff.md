# Comparing `tmp/typed-config-1.4.0.tar.gz` & `tmp/typed-config-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typed-config-1.4.0.tar", last modified: Thu Mar 28 16:57:36 2024, max compression
+gzip compressed data, was "typed-config-1.5.0.tar", last modified: Tue Apr  2 10:50:01 2024, max compression
```

## Comparing `typed-config-1.4.0.tar` & `typed-config-1.5.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-03-28 16:57:36.476440 typed-config-1.4.0/
--rw-rw-rw-   0        0        0     1089 2019-03-11 17:34:14.000000 typed-config-1.4.0/LICENSE
--rw-rw-rw-   0        0        0    27760 2024-03-28 16:57:36.475441 typed-config-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0    26760 2024-03-28 16:19:50.000000 typed-config-1.4.0/README.md
--rw-rw-rw-   0        0        0       33 2022-11-28 09:33:43.000000 typed-config-1.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-28 16:57:36.476440 typed-config-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1461 2022-11-14 18:44:22.000000 typed-config-1.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-28 16:57:36.416868 typed-config-1.4.0/test/
--rw-rw-rw-   0        0        0     3032 2024-03-28 16:14:10.000000 typed-config-1.4.0/test/test_casts.py
--rw-rw-rw-   0        0        0     2488 2022-11-28 09:33:43.000000 typed-config-1.4.0/test/test_config_source.py
--rw-rw-rw-   0        0        0    16510 2022-12-01 14:30:40.000000 typed-config-1.4.0/test/test_configuration.py
--rw-rw-rw-   0        0        0      395 2021-11-03 10:30:42.000000 typed-config-1.4.0/test/test_version.py
-drwxrwxrwx   0        0        0        0 2024-03-28 16:57:36.437867 typed-config-1.4.0/typed_config.egg-info/
--rw-rw-rw-   0        0        0    27760 2024-03-28 16:57:36.000000 typed-config-1.4.0/typed_config.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      475 2024-03-28 16:57:36.000000 typed-config-1.4.0/typed_config.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-28 16:57:36.000000 typed-config-1.4.0/typed_config.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-03-28 16:57:36.000000 typed-config-1.4.0/typed_config.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-28 16:57:36.000000 typed-config-1.4.0/typed_config.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-28 16:57:36.470875 typed-config-1.4.0/typedconfig/
--rw-rw-rw-   0        0        0       52 2019-03-11 17:20:46.000000 typed-config-1.4.0/typedconfig/__init__.py
--rw-rw-rw-   0        0        0       66 2024-03-28 16:20:44.000000 typed-config-1.4.0/typedconfig/__version__.py
--rw-rw-rw-   0        0        0     4971 2024-03-28 16:08:15.000000 typed-config-1.4.0/typedconfig/casts.py
--rw-rw-rw-   0        0        0    15717 2022-11-28 09:33:43.000000 typed-config-1.4.0/typedconfig/config.py
--rw-rw-rw-   0        0        0     2951 2022-11-28 09:33:43.000000 typed-config-1.4.0/typedconfig/provider.py
--rw-rw-rw-   0        0        0        0 2021-11-03 10:59:05.000000 typed-config-1.4.0/typedconfig/py.typed
--rw-rw-rw-   0        0        0     3311 2024-03-28 16:45:04.000000 typed-config-1.4.0/typedconfig/source.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:50:01.658566 typed-config-1.5.0/
+-rw-rw-rw-   0        0        0     1089 2019-03-11 17:34:14.000000 typed-config-1.5.0/LICENSE
+-rw-rw-rw-   0        0        0    28620 2024-04-02 10:50:01.655460 typed-config-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0    27620 2024-04-02 10:48:08.000000 typed-config-1.5.0/README.md
+-rw-rw-rw-   0        0        0       33 2022-11-28 09:33:43.000000 typed-config-1.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-02 10:50:01.658566 typed-config-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1461 2022-11-14 18:44:22.000000 typed-config-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:50:01.593168 typed-config-1.5.0/test/
+-rw-rw-rw-   0        0        0     3032 2024-03-28 16:14:10.000000 typed-config-1.5.0/test/test_casts.py
+-rw-rw-rw-   0        0        0     2994 2024-04-02 10:42:42.000000 typed-config-1.5.0/test/test_config_source.py
+-rw-rw-rw-   0        0        0    16510 2022-12-01 14:30:40.000000 typed-config-1.5.0/test/test_configuration.py
+-rw-rw-rw-   0        0        0      395 2021-11-03 10:30:42.000000 typed-config-1.5.0/test/test_version.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:50:01.621997 typed-config-1.5.0/typed_config.egg-info/
+-rw-rw-rw-   0        0        0    28620 2024-04-02 10:50:01.000000 typed-config-1.5.0/typed_config.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      475 2024-04-02 10:50:01.000000 typed-config-1.5.0/typed_config.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 10:50:01.000000 typed-config-1.5.0/typed_config.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-02 10:50:01.000000 typed-config-1.5.0/typed_config.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-02 10:50:01.000000 typed-config-1.5.0/typed_config.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 10:50:01.652938 typed-config-1.5.0/typedconfig/
+-rw-rw-rw-   0        0        0       52 2019-03-11 17:20:46.000000 typed-config-1.5.0/typedconfig/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-04-02 10:48:32.000000 typed-config-1.5.0/typedconfig/__version__.py
+-rw-rw-rw-   0        0        0     4971 2024-03-28 16:08:15.000000 typed-config-1.5.0/typedconfig/casts.py
+-rw-rw-rw-   0        0        0    15717 2022-11-28 09:33:43.000000 typed-config-1.5.0/typedconfig/config.py
+-rw-rw-rw-   0        0        0     2951 2022-11-28 09:33:43.000000 typed-config-1.5.0/typedconfig/provider.py
+-rw-rw-rw-   0        0        0        0 2021-11-03 10:59:05.000000 typed-config-1.5.0/typedconfig/py.typed
+-rw-rw-rw-   0        0        0     3860 2024-04-02 10:39:55.000000 typed-config-1.5.0/typedconfig/source.py
```

### Comparing `typed-config-1.4.0/LICENSE` & `typed-config-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `typed-config-1.4.0/PKG-INFO` & `typed-config-1.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: typed-config
-Version: 1.4.0
-Summary: Typed, extensible, dependency free configuration reader for Python projects for multiple config sources and working well in IDEs for great autocomplete performance.
-Home-page: https://github.com/bwindsor/typed-config
-Author: Ben Windsor
-Author-email: 
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Software Development
-Classifier: Typing :: Typed
-Requires-Python: >=3.6.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Build Status](https://travis-ci.org/bwindsor/typed-config.svg?branch=master)](https://travis-ci.org/bwindsor/typed-config)
 [![codecov](https://codecov.io/gh/bwindsor/typed-config/branch/master/graph/badge.svg)](https://codecov.io/gh/bwindsor/typed-config)
 
 # typed-config
 Typed, extensible, dependency free configuration reader for Python projects for multiple config sources and working well in IDEs for great autocomplete performance.
 
 `pip install typed-config`
@@ -443,14 +419,30 @@
 })
 ```
 
 It expects data type `Dict[str, Dict[str, str]]`, i.e. such that `string_value = d['section_name']['key_name']`. Everything should be provided as string data so that it can be parsed in the same way as if data was coming from a file or elsewhere.
 
 This is an alternative way of supplying default values instead of using the `default` option when defining your `key`s. Just provide a `DictConfigSource` as the lowest priority source, containing your defaults.
 
+#### `CmdConfigSource`
+This reads configuration from command line arguments
+```python
+from typedconfig.source import CmdConfigSource
+source = CmdConfigSource(prefix="XYZ")
+# OR just
+source = CmdConfigSource()
+```
+
+It will use Python's `argparse` library to extract the relevant command line arguments. It takes an optional input argument, the `prefix`. This can be useful if you also accept other command line arguments and wish to avoid clashes with your own arguments.
+
+* Arguments will be expected in the format `--{PREFIX}_{SECTION}_{KEY} {VALUE}`, for example `--xyz_database_port 2000`
+* If no `prefix` is provided, arguments will be expected in the format `--{SECTION}_{KEY} {VALUE}`, for example `--database_port 2000`
+
+The names are case insensitive so, for example, `--DATABASE_PORT` and `--database_port` would be treated the same.
+
 ### Writing your own `ConfigSource`s
 An abstract base class `ConfigSource` is supplied. You should extend it and implement the method `get_config_value` as demonstrated below, which takes a section name and key name, and returns either a `str` config value, or `None` if the value could not be found. It should not error if the value cannot be found, `Config` will throw an error later if it still can't find the value in any of its other available sources. To make it easier for the user try to make your source case insensitive.
 
 Here's an outline of how you might implement a source to read your config from a JSON file, for example. Use the `__init__` method to provide any information your source needs to fetch the data, such as filename, api details, etc. You can do sanity checks in the `__init__` method and throw an error if something is wrong.
 ```python
 import json
 from typing import Optional
```

### Comparing `typed-config-1.4.0/README.md` & `typed-config-1.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: typed-config
+Version: 1.5.0
+Summary: Typed, extensible, dependency free configuration reader for Python projects for multiple config sources and working well in IDEs for great autocomplete performance.
+Home-page: https://github.com/bwindsor/typed-config
+Author: Ben Windsor
+Author-email: 
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Software Development
+Classifier: Typing :: Typed
+Requires-Python: >=3.6.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![Build Status](https://travis-ci.org/bwindsor/typed-config.svg?branch=master)](https://travis-ci.org/bwindsor/typed-config)
 [![codecov](https://codecov.io/gh/bwindsor/typed-config/branch/master/graph/badge.svg)](https://codecov.io/gh/bwindsor/typed-config)
 
 # typed-config
 Typed, extensible, dependency free configuration reader for Python projects for multiple config sources and working well in IDEs for great autocomplete performance.
 
 `pip install typed-config`
@@ -419,14 +443,30 @@
 })
 ```
 
 It expects data type `Dict[str, Dict[str, str]]`, i.e. such that `string_value = d['section_name']['key_name']`. Everything should be provided as string data so that it can be parsed in the same way as if data was coming from a file or elsewhere.
 
 This is an alternative way of supplying default values instead of using the `default` option when defining your `key`s. Just provide a `DictConfigSource` as the lowest priority source, containing your defaults.
 
+#### `CmdConfigSource`
+This reads configuration from command line arguments
+```python
+from typedconfig.source import CmdConfigSource
+source = CmdConfigSource(prefix="XYZ")
+# OR just
+source = CmdConfigSource()
+```
+
+It will use Python's `argparse` library to extract the relevant command line arguments. It takes an optional input argument, the `prefix`. This can be useful if you also accept other command line arguments and wish to avoid clashes with your own arguments.
+
+* Arguments will be expected in the format `--{PREFIX}_{SECTION}_{KEY} {VALUE}`, for example `--xyz_database_port 2000`
+* If no `prefix` is provided, arguments will be expected in the format `--{SECTION}_{KEY} {VALUE}`, for example `--database_port 2000`
+
+The names are case insensitive so, for example, `--DATABASE_PORT` and `--database_port` would be treated the same.
+
 ### Writing your own `ConfigSource`s
 An abstract base class `ConfigSource` is supplied. You should extend it and implement the method `get_config_value` as demonstrated below, which takes a section name and key name, and returns either a `str` config value, or `None` if the value could not be found. It should not error if the value cannot be found, `Config` will throw an error later if it still can't find the value in any of its other available sources. To make it easier for the user try to make your source case insensitive.
 
 Here's an outline of how you might implement a source to read your config from a JSON file, for example. Use the `__init__` method to provide any information your source needs to fetch the data, such as filename, api details, etc. You can do sanity checks in the `__init__` method and throw an error if something is wrong.
 ```python
 import json
 from typing import Optional
```

### Comparing `typed-config-1.4.0/setup.py` & `typed-config-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `typed-config-1.4.0/test/test_casts.py` & `typed-config-1.5.0/test/test_casts.py`

 * *Files identical despite different names*

### Comparing `typed-config-1.4.0/test/test_config_source.py` & `typed-config-1.5.0/test/test_config_source.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import pytest
 import tempfile
 import os
+import sys
 from unittest.mock import patch
 from typedconfig.source import (
     ConfigSource,
     IniFileConfigSource,
     IniStringConfigSource,
     DictConfigSource,
     EnvironmentConfigSource,
+    CmdConfigSource,
 )
 
 
 def do_assertions(source: ConfigSource, expected_repr: str):
     v = source.get_config_value("s", "A")
     assert "1" == v
 
@@ -89,7 +91,19 @@
     do_assertions(source, "<EnvironmentConfigSource(prefix='PREFIX')>")
 
 
 @patch.dict(os.environ, {"S_A": "1", "S_B": "2"})
 def test_environment_config_source():
     source = EnvironmentConfigSource()
     do_assertions(source, "<EnvironmentConfigSource(prefix='')>")
+
+
+@patch('sys.argv', ["name.py", "--S_A", "1", "another_thing", "--S_B", "2", "--extra", "hello", "--no_value"])
+def test_cmd_config_source():
+    source = CmdConfigSource()
+    do_assertions(source, "<CmdConfigSource(prefix='')>")
+
+
+@patch('sys.argv', ["name.py", "--prefix_S_A", "1", "--PREFiX_S_B", "2"])
+def test_cmd_config_source_with_prefix():
+    source = CmdConfigSource(prefix="PREFIX")
+    do_assertions(source, "<CmdConfigSource(prefix='PREFIX')>")
```

### Comparing `typed-config-1.4.0/test/test_configuration.py` & `typed-config-1.5.0/test/test_configuration.py`

 * *Files identical despite different names*

### Comparing `typed-config-1.4.0/typed_config.egg-info/PKG-INFO` & `typed-config-1.5.0/typed_config.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typed-config
-Version: 1.4.0
+Version: 1.5.0
 Summary: Typed, extensible, dependency free configuration reader for Python projects for multiple config sources and working well in IDEs for great autocomplete performance.
 Home-page: https://github.com/bwindsor/typed-config
 Author: Ben Windsor
 Author-email: 
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -443,14 +443,30 @@
 })
 ```
 
 It expects data type `Dict[str, Dict[str, str]]`, i.e. such that `string_value = d['section_name']['key_name']`. Everything should be provided as string data so that it can be parsed in the same way as if data was coming from a file or elsewhere.
 
 This is an alternative way of supplying default values instead of using the `default` option when defining your `key`s. Just provide a `DictConfigSource` as the lowest priority source, containing your defaults.
 
+#### `CmdConfigSource`
+This reads configuration from command line arguments
+```python
+from typedconfig.source import CmdConfigSource
+source = CmdConfigSource(prefix="XYZ")
+# OR just
+source = CmdConfigSource()
+```
+
+It will use Python's `argparse` library to extract the relevant command line arguments. It takes an optional input argument, the `prefix`. This can be useful if you also accept other command line arguments and wish to avoid clashes with your own arguments.
+
+* Arguments will be expected in the format `--{PREFIX}_{SECTION}_{KEY} {VALUE}`, for example `--xyz_database_port 2000`
+* If no `prefix` is provided, arguments will be expected in the format `--{SECTION}_{KEY} {VALUE}`, for example `--database_port 2000`
+
+The names are case insensitive so, for example, `--DATABASE_PORT` and `--database_port` would be treated the same.
+
 ### Writing your own `ConfigSource`s
 An abstract base class `ConfigSource` is supplied. You should extend it and implement the method `get_config_value` as demonstrated below, which takes a section name and key name, and returns either a `str` config value, or `None` if the value could not be found. It should not error if the value cannot be found, `Config` will throw an error later if it still can't find the value in any of its other available sources. To make it easier for the user try to make your source case insensitive.
 
 Here's an outline of how you might implement a source to read your config from a JSON file, for example. Use the `__init__` method to provide any information your source needs to fetch the data, such as filename, api details, etc. You can do sanity checks in the `__init__` method and throw an error if something is wrong.
 ```python
 import json
 from typing import Optional
```

### Comparing `typed-config-1.4.0/typedconfig/casts.py` & `typed-config-1.5.0/typedconfig/casts.py`

 * *Files identical despite different names*

### Comparing `typed-config-1.4.0/typedconfig/config.py` & `typed-config-1.5.0/typedconfig/config.py`

 * *Files identical despite different names*

### Comparing `typed-config-1.4.0/typedconfig/provider.py` & `typed-config-1.5.0/typedconfig/provider.py`

 * *Files identical despite different names*

### Comparing `typed-config-1.4.0/typedconfig/source.py` & `typed-config-1.5.0/typedconfig/source.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import sys
+import argparse
 from abc import ABC, abstractmethod
 from typing import Optional, Dict
 from configparser import ConfigParser
 
 
 class ConfigSource(ABC):
     @abstractmethod
@@ -75,18 +76,29 @@
         section = self._config.get(section_name.lower(), None)
         if section is None:
             return None
         return section.get(key_name.lower(), None)
 
 
 class CmdConfigSource(ConfigSource):
-    def __init__(self):
-        pass
+    def __init__(self, prefix: str = ""):
+        self._init_prefix = prefix
+
+        self._prefix = prefix.lower()
+        if len(self._prefix) > 0:
+            self._prefix += "_"
+
+    @property
+    def prefix(self) -> str:
+        return self._init_prefix
 
     def get_config_value(self, section_name: str, key_name: str) -> Optional[str]:
         sys_argv_lower = [x.lower() for x in sys.argv]
-        try:
-            idx = sys_argv_lower.index(f"--{section_name.lower()}_{key_name.lower()}")
-        except ValueError:
-            # Command line argument not found
-            return None
-        return sys.argv[idx+1]
+        arg_name = f"{self._prefix}{section_name.lower()}_{key_name.lower()}"
+        parser = argparse.ArgumentParser(allow_abbrev=False, exit_on_error=False)
+        parser.add_argument("--" + arg_name, type=str)
+        parsed_args, rest = parser.parse_known_args(sys_argv_lower)
+        # Attribute should always exist, but will be None if the argument was not found
+        return getattr(parsed_args, arg_name)
+
+    def __repr__(self) -> str:
+        return f"<{self.__class__.__qualname__}(prefix={repr(self.prefix)})>"
```

