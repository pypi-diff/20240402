# Comparing `tmp/dataconf-3.0.0.tar.gz` & `tmp/dataconf-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataconf-3.0.0.tar", max compression
+gzip compressed data, was "dataconf-3.1.0.tar", max compression
```

## Comparing `dataconf-3.0.0.tar` & `dataconf-3.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    16724 2024-03-08 11:36:34.312762 dataconf-3.0.0/LICENSE
--rw-r--r--   0        0        0     5014 2024-03-08 11:36:34.312762 dataconf-3.0.0/README.md
--rw-r--r--   0        0        0      685 2024-03-08 11:36:34.312762 dataconf-3.0.0/dataconf/__init__.py
--rw-r--r--   0        0        0      871 2024-03-08 11:36:34.312762 dataconf-3.0.0/dataconf/cli.py
--rw-r--r--   0        0        0      691 2024-03-08 11:36:34.312762 dataconf-3.0.0/dataconf/exceptions.py
--rw-r--r--   0        0        0     4412 2024-03-08 11:36:34.312762 dataconf-3.0.0/dataconf/main.py
--rw-r--r--   0        0        0       44 2024-03-08 11:36:34.312762 dataconf-3.0.0/dataconf/py.typed
--rw-r--r--   0        0        0    12418 2024-03-08 11:36:34.312762 dataconf-3.0.0/dataconf/utils.py
--rw-r--r--   0        0        0      111 2024-03-08 11:36:34.312762 dataconf-3.0.0/dataconf/version.py
--rw-r--r--   0        0        0     1444 2024-03-08 11:36:34.316763 dataconf-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     6233 1970-01-01 00:00:00.000000 dataconf-3.0.0/setup.py
--rw-r--r--   0        0        0     6279 1970-01-01 00:00:00.000000 dataconf-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0    16724 2024-04-02 18:16:32.003979 dataconf-3.1.0/LICENSE
+-rw-r--r--   0        0        0     5410 2024-04-02 18:16:32.003979 dataconf-3.1.0/README.md
+-rw-r--r--   0        0        0      685 2024-04-02 18:16:32.003979 dataconf-3.1.0/dataconf/__init__.py
+-rw-r--r--   0        0        0      871 2024-04-02 18:16:32.003979 dataconf-3.1.0/dataconf/cli.py
+-rw-r--r--   0        0        0      691 2024-04-02 18:16:32.003979 dataconf-3.1.0/dataconf/exceptions.py
+-rw-r--r--   0        0        0     4412 2024-04-02 18:16:32.003979 dataconf-3.1.0/dataconf/main.py
+-rw-r--r--   0        0        0       44 2024-04-02 18:16:32.003979 dataconf-3.1.0/dataconf/py.typed
+-rw-r--r--   0        0        0    13391 2024-04-02 18:16:32.003979 dataconf-3.1.0/dataconf/utils.py
+-rw-r--r--   0        0        0      111 2024-04-02 18:16:32.003979 dataconf-3.1.0/dataconf/version.py
+-rw-r--r--   0        0        0     1444 2024-04-02 18:16:32.003979 dataconf-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6646 1970-01-01 00:00:00.000000 dataconf-3.1.0/setup.py
+-rw-r--r--   0        0        0     6675 1970-01-01 00:00:00.000000 dataconf-3.1.0/PKG-INFO
```

### Comparing `dataconf-3.0.0/LICENSE` & `dataconf-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dataconf-3.0.0/README.md` & `dataconf-3.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -25,26 +25,35 @@
 ```
 
 ## Usage
 
 ```python
 import os
 from dataclasses import dataclass, field
-from typing import List, Dict, Text, Union
+from typing import List, Dict, Text, Union, Tuple
 from dateutil.relativedelta import relativedelta
-from datetime import datetime
+from datetime import datetime, timedelta
 import dataconf
 
 conf = """
 str_name = test
 str_name = ${?HOME}
 dash-to-underscore = true
 float_num = 2.2
 iso_datetime = "2000-01-01T20:00:00"
 iso_duration = "P123DT4H5M6S"
+variable_length_tuple_data = [
+    1
+    2
+    3
+]
+tuple_data = [
+    a
+    P1D
+]
 # this is a comment
 list_data = [
     a
     b
 ]
 nested {
     a = test
@@ -85,37 +94,43 @@
 @dataclass
 class Config:
     str_name: Text
     dash_to_underscore: bool
     float_num: float
     iso_datetime: datetime
     iso_duration: timedelta
+    variable_length_tuple_data: Tuple[int, ...]
+    tuple_data: Tuple[Text, timedelta]
     list_data: List[Text]
     nested: Nested
     nested_list: List[Nested]
     duration: relativedelta
     union: Union[Text, int]
     people: AbstractBaseClass
     zone: AbstractBaseClass
     default: Text = 'hello'
     default_factory: Dict[Text, Text] = field(default_factory=dict)
 
 print(dataconf.string(conf, Config))
 # Config(
-#   str_name='/users/root',
+#   str_name='/users/root/',
 #   dash_to_underscore=True,
 #   float_num=2.2,
+#   iso_datetime=datetime.datetime(2000, 1, 1, 20, 0),
+#   iso_duration=datetime.timedelta(days=123, seconds=14706),
+#   variable_length_tuple_data=(1,2,3),
+#   tuple_data=('a', datetime.timedelta(days=1)),
 #   list_data=['a', 'b'],
-#   nested=Nested(a='test'),
+#   nested=Nested(a='test', b=1),
 #   nested_list=[Nested(a='test1', b=2.5)],
-#   duration=relativedelta(seconds=+2), 
-#   union=1, 
-#   people=Person(name='Thailand'), 
+#   duration=relativedelta(seconds=+2),
+#   union=1,
+#   people=Person(name='Thailand'),
 #   zone=Zone(area_code=42),
-#   default='hello', 
+#   default='hello',
 #   default_factory={}
 # )
 
 @dataclass
 class Example:
     hello: str
     world: str
```

### Comparing `dataconf-3.0.0/dataconf/__init__.py` & `dataconf-3.1.0/dataconf/__init__.py`

 * *Files identical despite different names*

### Comparing `dataconf-3.0.0/dataconf/cli.py` & `dataconf-3.1.0/dataconf/cli.py`

 * *Files identical despite different names*

### Comparing `dataconf-3.0.0/dataconf/exceptions.py` & `dataconf-3.1.0/dataconf/exceptions.py`

 * *Files identical despite different names*

### Comparing `dataconf-3.0.0/dataconf/main.py` & `dataconf-3.1.0/dataconf/main.py`

 * *Files identical despite different names*

### Comparing `dataconf-3.0.0/dataconf/utils.py` & `dataconf-3.1.0/dataconf/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,24 +109,49 @@
 
         return clazz(**fs)
 
     origin = get_origin(clazz)
     args = get_args(clazz)
 
     if origin is list:
+        if value is None:
+            raise MalformedConfigException(f"expected list at {path} but received None")
+
         if len(args) != 1:
             raise MissingTypeException("expected list with type information: List[?]")
 
-        if value is not None:
-            parse_candidate = args[0]
-            return [
-                __parse(v, parse_candidate, f"{path}[]", strict, ignore_unexpected)
-                for v in value
-            ]
-        return None
+        parse_candidate = args[0]
+        return [
+            __parse(v, parse_candidate, f"{path}[]", strict, ignore_unexpected)
+            for v in value
+        ]
+
+    if origin is tuple:
+        if value is None:
+            raise MalformedConfigException(
+                f"expected tuple at {path} but received None"
+            )
+
+        if len(args) < 1:
+            raise MissingTypeException("expected tuple with type information: Tuple[?]")
+
+        has_ellipsis = args[-1] == Ellipsis
+        if has_ellipsis and len(args) != 2:
+            raise MissingTypeException(
+                "expected one type since ellipsis is used: Tuple[?, ...]"
+            )
+        _args = args if not has_ellipsis else [args[0]] * len(value)
+        if len(value) > 0 and len(value) != len(_args):
+            raise MalformedConfigException(
+                "number of provided values does not match expected number of values for tuple."
+            )
+        return tuple(
+            __parse(v, arg, f"{path}[]", strict, ignore_unexpected)
+            for v, arg in zip(value, _args)
+        )
 
     if origin is dict:
         if len(args) != 2:
             raise MissingTypeException(
                 "expected dict with type information: Dict[?, ?]"
             )
         if value is not None:
```

### Comparing `dataconf-3.0.0/pyproject.toml` & `dataconf-3.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataconf"
-version = "3.0.0"
+version = "3.1.0"
 description = "Simple dataclasses configuration management for Python with hocon/json/yaml/properties/env-vars/dict support."
 authors = []
 license = "MPL-2.0"
 readme = "README.md"
 repository = "https://github.com/zifeo/dataconf"
 include = [
     "dataconf", "pyproject.toml"
@@ -44,15 +44,15 @@
 pre-commit = ">=2.21,<4.0"
 commitizen = ">=2.42.1,<4.0.0"
 pytest-httpserver = "^1.0.8"
 ruff = ">=0.1.9,<0.4.0"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "3.0.0"
+version = "3.1.0"
 tag_format = "v$major.$minor.$patch$prerelease"
 version_files = [
     "pyproject.toml:version",
     "dataconf/version.py"
 ]
 
 [build-system]
```

### Comparing `dataconf-3.0.0/setup.py` & `dataconf-3.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,17 +15,17 @@
  'python-dateutil>=2.8.2,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['dataconf = dataconf.cli:run']}
 
 setup_kwargs = {
     'name': 'dataconf',
-    'version': '3.0.0',
+    'version': '3.1.0',
     'description': 'Simple dataclasses configuration management for Python with hocon/json/yaml/properties/env-vars/dict support.',
-    'long_description': '# Dataconf\n\n[![Actions Status](https://github.com/zifeo/dataconf/actions/workflows/test-release.yaml/badge.svg)](https://github.com/zifeo/dataconf/actions)\n[![PyPI version](https://badge.fury.io/py/dataconf.svg)](https://badge.fury.io/py/dataconf)\n\nSimple dataclasses configuration management for Python with\nhocon/json/yaml/properties/env-vars/dict/cli support.\n\n## Getting started\n\nRequires at least Python 3.8.\n\n```bash\n# pypi\npip install dataconf\npoetry add dataconf\n\n# remote master\npip install --upgrade git+https://github.com/zifeo/dataconf.git\npoetry add git+https://github.com/zifeo/dataconf.git\n\n# local repo/dev\npoetry install\npre-commit install\n```\n\n## Usage\n\n```python\nimport os\nfrom dataclasses import dataclass, field\nfrom typing import List, Dict, Text, Union\nfrom dateutil.relativedelta import relativedelta\nfrom datetime import datetime\nimport dataconf\n\nconf = """\nstr_name = test\nstr_name = ${?HOME}\ndash-to-underscore = true\nfloat_num = 2.2\niso_datetime = "2000-01-01T20:00:00"\niso_duration = "P123DT4H5M6S"\n# this is a comment\nlist_data = [\n    a\n    b\n]\nnested {\n    a = test\n    b : 1\n}\nnested_list = [\n    {\n        a = test1\n        b : 2.5\n    }\n]\nduration = 2s\nunion = 1\npeople {\n    name = Thailand\n}\nzone {\n    area_code = 42\n}\n"""\n\nclass AbstractBaseClass:\n    pass\n    \n@dataclass\nclass Person(AbstractBaseClass):\n    name: Text\n        \n@dataclass\nclass Zone(AbstractBaseClass):\n    area_code: int\n\n@dataclass\nclass Nested:\n    a: Text\n    b: float\n\n@dataclass\nclass Config:\n    str_name: Text\n    dash_to_underscore: bool\n    float_num: float\n    iso_datetime: datetime\n    iso_duration: timedelta\n    list_data: List[Text]\n    nested: Nested\n    nested_list: List[Nested]\n    duration: relativedelta\n    union: Union[Text, int]\n    people: AbstractBaseClass\n    zone: AbstractBaseClass\n    default: Text = \'hello\'\n    default_factory: Dict[Text, Text] = field(default_factory=dict)\n\nprint(dataconf.string(conf, Config))\n# Config(\n#   str_name=\'/users/root\',\n#   dash_to_underscore=True,\n#   float_num=2.2,\n#   list_data=[\'a\', \'b\'],\n#   nested=Nested(a=\'test\'),\n#   nested_list=[Nested(a=\'test1\', b=2.5)],\n#   duration=relativedelta(seconds=+2), \n#   union=1, \n#   people=Person(name=\'Thailand\'), \n#   zone=Zone(area_code=42),\n#   default=\'hello\', \n#   default_factory={}\n# )\n\n@dataclass\nclass Example:\n    hello: str\n    world: str\n    foo: List[str]\n\nos.environ[\'DC_WORLD\'] = \'monde\'\n\nprint(\n    dataconf\n    .multi\n    .url(\'https://raw.githubusercontent.com/zifeo/dataconf/main/confs/simple.hocon\')\n    .env(\'DC\')\n    .on(Example)\n)\n# Example(hello=\'bonjour\',world=\'monde\')\n```\n\n## API\n\n```python\nimport dataconf\n\nconf = dataconf.string(\'{ name: Test }\', Config)\nconf = dataconf.string(\'name:\\n\\tvalue: Test\', Config, loader=dataconf.YAML)  # dataconf.HOCON by default\nconf = dataconf.env(\'PREFIX_\', Config)\nconf = dataconf.dict({\'name\': \'Test\'}, Config)\nconf = dataconf.url(\'https://raw.githubusercontent.com/zifeo/dataconf/master/confs/test.hocon\', Config)  # hocon, json, yaml, properties\nconf = dataconf.file(\'confs/test.hocon\', Config)  # hocon, json, yaml, properties\nconf = dataconf.cli(sys.argv, Config)\n\n# Aggregation\nconf = dataconf.multi.string(...).env(...).url(...).file(...).dict(...).cli(...).on(Config)\n\n# Same api as Python json/yaml packages (e.g. `load`, `loads`, `dump`, `dumps`)\nconf = dataconf.load(\'confs/test.hocon\', Config)  # hocon, json, yaml, properties\nconf = dataconf.load(\'confs/test.yaml\', Config, loader=dataconf.YAML)  # dataconf.HOCON by default\ndataconf.dump(\'confs/test.hocon\', conf, out=\'hocon\')\ndataconf.dump(\'confs/test.json\', conf, out=\'json\')\ndataconf.dump(\'confs/test.yaml\', conf, out=\'yaml\')\ndataconf.dump(\'confs/test.properties\', conf, out=\'properties\')\n```\n\nFor full HOCON capabilities see\n[here](https://github.com/chimpler/pyhocon/#example-of-hocon-file).\n\n## Parse env vars\n\n```bash\nPREFIX_VAR=a\nPREFIX_VAR_NAME=b\nPREFIX_TEST__NAME=c\nPREFIX_LS_0=d\nPREFIX_LS_1=e\nPREFIX_LSLS_0_0=f\nPREFIX_LSOB_0__NAME=g\nPREFIX_NESTED_="{ name: Test }"\nPREFIX_SUB_="{ value: ${PREFIX_VAR} }"\n```\n\nis equivalent to\n\n```\n{\n    var = a\n    var_name = b\n    test {\n        name = c\n    }\n    ls = [\n        d\n        e\n    ]\n    lsls = [\n        [\n            f\n        ]\n    ]\n    lsob = [\n        {\n            name = g\n        }\n    ]\n    nested {\n        # parse nested config by suffixing env var with `_`\n        name: Test\n    }\n    sub {\n        # will have value "a" at parsing, useful for aliases\n        value = ${PREFIX_VAR}\n    }\n}\n```\n\nNote that when using `.env` source, the strict mode is disabled and value might\nbe casted.\n\n## Parse CLI arguments\n\nSame as env vars parse (dashes are converted to underscore, e.g. `TEST_A` →\n`--test-a`).\n\n## CLI usage\n\nCan be used for validation or converting between supported file formats (`-o`).\n\n```shell\ndataconf -c confs/test.hocon -m tests.configs -d TestConf -o hocon\n# dataconf.exceptions.TypeConfigException: expected type <class \'datetime.timedelta\'> at .duration, got <class \'int\'>\n```\n',
+    'long_description': '# Dataconf\n\n[![Actions Status](https://github.com/zifeo/dataconf/actions/workflows/test-release.yaml/badge.svg)](https://github.com/zifeo/dataconf/actions)\n[![PyPI version](https://badge.fury.io/py/dataconf.svg)](https://badge.fury.io/py/dataconf)\n\nSimple dataclasses configuration management for Python with\nhocon/json/yaml/properties/env-vars/dict/cli support.\n\n## Getting started\n\nRequires at least Python 3.8.\n\n```bash\n# pypi\npip install dataconf\npoetry add dataconf\n\n# remote master\npip install --upgrade git+https://github.com/zifeo/dataconf.git\npoetry add git+https://github.com/zifeo/dataconf.git\n\n# local repo/dev\npoetry install\npre-commit install\n```\n\n## Usage\n\n```python\nimport os\nfrom dataclasses import dataclass, field\nfrom typing import List, Dict, Text, Union, Tuple\nfrom dateutil.relativedelta import relativedelta\nfrom datetime import datetime, timedelta\nimport dataconf\n\nconf = """\nstr_name = test\nstr_name = ${?HOME}\ndash-to-underscore = true\nfloat_num = 2.2\niso_datetime = "2000-01-01T20:00:00"\niso_duration = "P123DT4H5M6S"\nvariable_length_tuple_data = [\n    1\n    2\n    3\n]\ntuple_data = [\n    a\n    P1D\n]\n# this is a comment\nlist_data = [\n    a\n    b\n]\nnested {\n    a = test\n    b : 1\n}\nnested_list = [\n    {\n        a = test1\n        b : 2.5\n    }\n]\nduration = 2s\nunion = 1\npeople {\n    name = Thailand\n}\nzone {\n    area_code = 42\n}\n"""\n\nclass AbstractBaseClass:\n    pass\n    \n@dataclass\nclass Person(AbstractBaseClass):\n    name: Text\n        \n@dataclass\nclass Zone(AbstractBaseClass):\n    area_code: int\n\n@dataclass\nclass Nested:\n    a: Text\n    b: float\n\n@dataclass\nclass Config:\n    str_name: Text\n    dash_to_underscore: bool\n    float_num: float\n    iso_datetime: datetime\n    iso_duration: timedelta\n    variable_length_tuple_data: Tuple[int, ...]\n    tuple_data: Tuple[Text, timedelta]\n    list_data: List[Text]\n    nested: Nested\n    nested_list: List[Nested]\n    duration: relativedelta\n    union: Union[Text, int]\n    people: AbstractBaseClass\n    zone: AbstractBaseClass\n    default: Text = \'hello\'\n    default_factory: Dict[Text, Text] = field(default_factory=dict)\n\nprint(dataconf.string(conf, Config))\n# Config(\n#   str_name=\'/users/root/\',\n#   dash_to_underscore=True,\n#   float_num=2.2,\n#   iso_datetime=datetime.datetime(2000, 1, 1, 20, 0),\n#   iso_duration=datetime.timedelta(days=123, seconds=14706),\n#   variable_length_tuple_data=(1,2,3),\n#   tuple_data=(\'a\', datetime.timedelta(days=1)),\n#   list_data=[\'a\', \'b\'],\n#   nested=Nested(a=\'test\', b=1),\n#   nested_list=[Nested(a=\'test1\', b=2.5)],\n#   duration=relativedelta(seconds=+2),\n#   union=1,\n#   people=Person(name=\'Thailand\'),\n#   zone=Zone(area_code=42),\n#   default=\'hello\',\n#   default_factory={}\n# )\n\n@dataclass\nclass Example:\n    hello: str\n    world: str\n    foo: List[str]\n\nos.environ[\'DC_WORLD\'] = \'monde\'\n\nprint(\n    dataconf\n    .multi\n    .url(\'https://raw.githubusercontent.com/zifeo/dataconf/main/confs/simple.hocon\')\n    .env(\'DC\')\n    .on(Example)\n)\n# Example(hello=\'bonjour\',world=\'monde\')\n```\n\n## API\n\n```python\nimport dataconf\n\nconf = dataconf.string(\'{ name: Test }\', Config)\nconf = dataconf.string(\'name:\\n\\tvalue: Test\', Config, loader=dataconf.YAML)  # dataconf.HOCON by default\nconf = dataconf.env(\'PREFIX_\', Config)\nconf = dataconf.dict({\'name\': \'Test\'}, Config)\nconf = dataconf.url(\'https://raw.githubusercontent.com/zifeo/dataconf/master/confs/test.hocon\', Config)  # hocon, json, yaml, properties\nconf = dataconf.file(\'confs/test.hocon\', Config)  # hocon, json, yaml, properties\nconf = dataconf.cli(sys.argv, Config)\n\n# Aggregation\nconf = dataconf.multi.string(...).env(...).url(...).file(...).dict(...).cli(...).on(Config)\n\n# Same api as Python json/yaml packages (e.g. `load`, `loads`, `dump`, `dumps`)\nconf = dataconf.load(\'confs/test.hocon\', Config)  # hocon, json, yaml, properties\nconf = dataconf.load(\'confs/test.yaml\', Config, loader=dataconf.YAML)  # dataconf.HOCON by default\ndataconf.dump(\'confs/test.hocon\', conf, out=\'hocon\')\ndataconf.dump(\'confs/test.json\', conf, out=\'json\')\ndataconf.dump(\'confs/test.yaml\', conf, out=\'yaml\')\ndataconf.dump(\'confs/test.properties\', conf, out=\'properties\')\n```\n\nFor full HOCON capabilities see\n[here](https://github.com/chimpler/pyhocon/#example-of-hocon-file).\n\n## Parse env vars\n\n```bash\nPREFIX_VAR=a\nPREFIX_VAR_NAME=b\nPREFIX_TEST__NAME=c\nPREFIX_LS_0=d\nPREFIX_LS_1=e\nPREFIX_LSLS_0_0=f\nPREFIX_LSOB_0__NAME=g\nPREFIX_NESTED_="{ name: Test }"\nPREFIX_SUB_="{ value: ${PREFIX_VAR} }"\n```\n\nis equivalent to\n\n```\n{\n    var = a\n    var_name = b\n    test {\n        name = c\n    }\n    ls = [\n        d\n        e\n    ]\n    lsls = [\n        [\n            f\n        ]\n    ]\n    lsob = [\n        {\n            name = g\n        }\n    ]\n    nested {\n        # parse nested config by suffixing env var with `_`\n        name: Test\n    }\n    sub {\n        # will have value "a" at parsing, useful for aliases\n        value = ${PREFIX_VAR}\n    }\n}\n```\n\nNote that when using `.env` source, the strict mode is disabled and value might\nbe casted.\n\n## Parse CLI arguments\n\nSame as env vars parse (dashes are converted to underscore, e.g. `TEST_A` →\n`--test-a`).\n\n## CLI usage\n\nCan be used for validation or converting between supported file formats (`-o`).\n\n```shell\ndataconf -c confs/test.hocon -m tests.configs -d TestConf -o hocon\n# dataconf.exceptions.TypeConfigException: expected type <class \'datetime.timedelta\'> at .duration, got <class \'int\'>\n```\n',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/zifeo/dataconf',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `dataconf-3.0.0/PKG-INFO` & `dataconf-3.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataconf
-Version: 3.0.0
+Version: 3.1.0
 Summary: Simple dataclasses configuration management for Python with hocon/json/yaml/properties/env-vars/dict support.
 Home-page: https://github.com/zifeo/dataconf
 License: MPL-2.0
 Keywords: configuration,dataclasses,yaml,hocon,json,properties,cli,environment variables
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python
@@ -53,26 +53,35 @@
 ```
 
 ## Usage
 
 ```python
 import os
 from dataclasses import dataclass, field
-from typing import List, Dict, Text, Union
+from typing import List, Dict, Text, Union, Tuple
 from dateutil.relativedelta import relativedelta
-from datetime import datetime
+from datetime import datetime, timedelta
 import dataconf
 
 conf = """
 str_name = test
 str_name = ${?HOME}
 dash-to-underscore = true
 float_num = 2.2
 iso_datetime = "2000-01-01T20:00:00"
 iso_duration = "P123DT4H5M6S"
+variable_length_tuple_data = [
+    1
+    2
+    3
+]
+tuple_data = [
+    a
+    P1D
+]
 # this is a comment
 list_data = [
     a
     b
 ]
 nested {
     a = test
@@ -113,37 +122,43 @@
 @dataclass
 class Config:
     str_name: Text
     dash_to_underscore: bool
     float_num: float
     iso_datetime: datetime
     iso_duration: timedelta
+    variable_length_tuple_data: Tuple[int, ...]
+    tuple_data: Tuple[Text, timedelta]
     list_data: List[Text]
     nested: Nested
     nested_list: List[Nested]
     duration: relativedelta
     union: Union[Text, int]
     people: AbstractBaseClass
     zone: AbstractBaseClass
     default: Text = 'hello'
     default_factory: Dict[Text, Text] = field(default_factory=dict)
 
 print(dataconf.string(conf, Config))
 # Config(
-#   str_name='/users/root',
+#   str_name='/users/root/',
 #   dash_to_underscore=True,
 #   float_num=2.2,
+#   iso_datetime=datetime.datetime(2000, 1, 1, 20, 0),
+#   iso_duration=datetime.timedelta(days=123, seconds=14706),
+#   variable_length_tuple_data=(1,2,3),
+#   tuple_data=('a', datetime.timedelta(days=1)),
 #   list_data=['a', 'b'],
-#   nested=Nested(a='test'),
+#   nested=Nested(a='test', b=1),
 #   nested_list=[Nested(a='test1', b=2.5)],
-#   duration=relativedelta(seconds=+2), 
-#   union=1, 
-#   people=Person(name='Thailand'), 
+#   duration=relativedelta(seconds=+2),
+#   union=1,
+#   people=Person(name='Thailand'),
 #   zone=Zone(area_code=42),
-#   default='hello', 
+#   default='hello',
 #   default_factory={}
 # )
 
 @dataclass
 class Example:
     hello: str
     world: str
```

