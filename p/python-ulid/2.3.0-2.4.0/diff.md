# Comparing `tmp/python_ulid-2.3.0.tar.gz` & `tmp/python_ulid-2.4.0.tar.gz`

## Comparing `python_ulid-2.3.0.tar` & `python_ulid-2.4.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 python_ulid-2.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 python_ulid-2.3.0/.readthedocs.yml
--rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 python_ulid-2.3.0/CHANGELOG.rst
--rw-r--r--   0        0        0     5677 2020-02-02 00:00:00.000000 python_ulid-2.3.0/README.rst
--rw-r--r--   0        0        0     6010 2020-02-02 00:00:00.000000 python_ulid-2.3.0/logo.png
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 python_ulid-2.3.0/.github/workflows/lint-and-test.yml
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 python_ulid-2.3.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 python_ulid-2.3.0/docs/Makefile
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_ulid-2.3.0/docs/requirements.txt
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 python_ulid-2.3.0/docs/source/api.rst
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 python_ulid-2.3.0/docs/source/changelog.rst
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 python_ulid-2.3.0/docs/source/conf.py
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 python_ulid-2.3.0/docs/source/index.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_ulid-2.3.0/tests/__init__.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 python_ulid-2.3.0/tests/test_base32.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 python_ulid-2.3.0/tests/test_cli.py
--rw-r--r--   0        0        0     4715 2020-02-02 00:00:00.000000 python_ulid-2.3.0/tests/test_ulid.py
--rw-r--r--   0        0        0     9114 2020-02-02 00:00:00.000000 python_ulid-2.3.0/ulid/__init__.py
--rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 python_ulid-2.3.0/ulid/__main__.py
--rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 python_ulid-2.3.0/ulid/base32.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 python_ulid-2.3.0/ulid/constants.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_ulid-2.3.0/ulid/py.typed
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 python_ulid-2.3.0/.gitignore
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 python_ulid-2.3.0/LICENSE
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 python_ulid-2.3.0/hatch.toml
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 python_ulid-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 python_ulid-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 python_ulid-2.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 python_ulid-2.4.0/.readthedocs.yml
+-rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 python_ulid-2.4.0/CHANGELOG.rst
+-rw-r--r--   0        0        0     5677 2020-02-02 00:00:00.000000 python_ulid-2.4.0/README.rst
+-rw-r--r--   0        0        0     6010 2020-02-02 00:00:00.000000 python_ulid-2.4.0/logo.png
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 python_ulid-2.4.0/.github/workflows/lint-and-test.yml
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 python_ulid-2.4.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 python_ulid-2.4.0/docs/Makefile
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_ulid-2.4.0/docs/requirements.txt
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 python_ulid-2.4.0/docs/source/api.rst
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 python_ulid-2.4.0/docs/source/changelog.rst
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 python_ulid-2.4.0/docs/source/conf.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 python_ulid-2.4.0/docs/source/index.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_ulid-2.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 python_ulid-2.4.0/tests/test_base32.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 python_ulid-2.4.0/tests/test_cli.py
+-rw-r--r--   0        0        0     5081 2020-02-02 00:00:00.000000 python_ulid-2.4.0/tests/test_ulid.py
+-rw-r--r--   0        0        0     9235 2020-02-02 00:00:00.000000 python_ulid-2.4.0/ulid/__init__.py
+-rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 python_ulid-2.4.0/ulid/__main__.py
+-rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 python_ulid-2.4.0/ulid/base32.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 python_ulid-2.4.0/ulid/constants.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_ulid-2.4.0/ulid/py.typed
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 python_ulid-2.4.0/.gitignore
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 python_ulid-2.4.0/LICENSE
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 python_ulid-2.4.0/hatch.toml
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 python_ulid-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5570 2020-02-02 00:00:00.000000 python_ulid-2.4.0/PKG-INFO
```

### Comparing `python_ulid-2.3.0/CHANGELOG.rst` & `python_ulid-2.4.0/CHANGELOG.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 .. _changelog:
 
 Changelog
 =========
 
 Versions follow `Semantic Versioning <http://www.semver.org>`_
 
-`2.3.0`_ - 2023-09-21
+`2.4.0`_ - 2024-04-02
+---------------------
+
+Added
+~~~~~
+* :class:`.ULID` objects are now properly serialized when used as Pydantic types `@Avihais12344 <https://github.com/Avihais12344>`_.
+
+
+`2.3.0`_ - 2024-03-21
 ---------------------
 
 Added
 ~~~~~
 * :class:`.ULID` objects can now be converted to bytes with ``bytes(ulid)``.
 * The Pydantic v2 protocol is now supported, so that the :class:`.ULID` class can be directly used
   as type annotations in `Pydantic models <https://docs.pydantic.dev/latest/concepts/models/#basic-model-usage>`_
@@ -139,14 +147,15 @@
     >>> ULID().hex
     '0171caa5459a8631a6894d072c8550a8'
 
 * Equality checks and ordering now also work with ``str``-instances.
 * The package now has no external dependencies.
 * The test-coverage has been raised to 100%.
 
+.. _2.4.0: https://github.com/mdomke/python-ulid/compare/2.3.0...2.4.0
 .. _2.3.0: https://github.com/mdomke/python-ulid/compare/2.2.0...2.3.0
 .. _2.2.0: https://github.com/mdomke/python-ulid/compare/2.1.0...2.2.0
 .. _2.1.0: https://github.com/mdomke/python-ulid/compare/2.0.0...2.1.0
 .. _2.0.0: https://github.com/mdomke/python-ulid/compare/1.1.0...2.0.0
 .. _1.1.0: https://github.com/mdomke/python-ulid/compare/1.0.3...1.1.0
 .. _1.0.3: https://github.com/mdomke/python-ulid/compare/1.0.2...1.0.3
 .. _1.0.0: https://github.com/mdomke/python-ulid/compare/0.2.0...1.0.0
```

### Comparing `python_ulid-2.3.0/README.rst` & `python_ulid-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `python_ulid-2.3.0/logo.png` & `python_ulid-2.4.0/logo.png`

 * *Files identical despite different names*

### Comparing `python_ulid-2.3.0/.github/workflows/lint-and-test.yml` & `python_ulid-2.4.0/.github/workflows/lint-and-test.yml`

 * *Files identical despite different names*

### Comparing `python_ulid-2.3.0/.github/workflows/publish.yml` & `python_ulid-2.4.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `python_ulid-2.3.0/docs/Makefile` & `python_ulid-2.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python_ulid-2.3.0/docs/source/conf.py` & `python_ulid-2.4.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `python_ulid-2.3.0/docs/source/index.rst` & `python_ulid-2.4.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `python_ulid-2.3.0/tests/test_base32.py` & `python_ulid-2.4.0/tests/test_base32.py`

 * *Files identical despite different names*

### Comparing `python_ulid-2.3.0/tests/test_cli.py` & `python_ulid-2.4.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `python_ulid-2.3.0/tests/test_ulid.py` & `python_ulid-2.4.0/tests/test_ulid.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import time
 import uuid
 from collections.abc import Callable
 from datetime import datetime
 from datetime import timedelta
 from datetime import timezone
 from typing import Union
@@ -173,7 +174,17 @@
         model = Model(ulid=value)
         assert isinstance(model.ulid, ULID)
         assert model.ulid == ulid
 
     for value in [b"not-enough", "not-enough"]:
         with pytest.raises(ValidationError):
             Model(ulid=value)
+
+    model_dict = model.model_dump()
+    ulid_from_dict = model_dict["ulid"]
+    assert ulid_from_dict == ulid
+    assert isinstance(ulid_from_dict, ULID)
+    assert Model(**model_dict) == model
+
+    model_json = model.model_dump_json()
+    assert isinstance(json.loads(model_json)["ulid"], str)
+    assert Model.model_validate_json(model_json) == model
```

### Comparing `python_ulid-2.3.0/ulid/__init__.py` & `python_ulid-2.4.0/ulid/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,14 +257,17 @@
             cls._pydantic_validate,
             core_schema.union_schema(
                 [
                     core_schema.is_instance_schema(ULID),
                     core_schema.no_info_plain_validator_function(ULID),
                 ]
             ),
+            serialization=core_schema.to_string_ser_schema(
+                when_used="json-unless-none",
+            ),
         )
 
     @classmethod
     def _pydantic_validate(cls, value: Any, handler: ValidatorFunctionWrapHandler) -> Any:
         from pydantic_core import PydanticCustomError
 
         try:
```

### Comparing `python_ulid-2.3.0/ulid/__main__.py` & `python_ulid-2.4.0/ulid/__main__.py`

 * *Files identical despite different names*

### Comparing `python_ulid-2.3.0/ulid/base32.py` & `python_ulid-2.4.0/ulid/base32.py`

 * *Files identical despite different names*

### Comparing `python_ulid-2.3.0/LICENSE` & `python_ulid-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_ulid-2.3.0/hatch.toml` & `python_ulid-2.4.0/hatch.toml`

 * *Files identical despite different names*

### Comparing `python_ulid-2.3.0/pyproject.toml` & `python_ulid-2.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,19 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Software Development :: Libraries",
 ]
 
+[project.urls]
+Homepage = "https://github.com/mdomke/python-ulid"
+Repository = "https://github.com/mdomke/python-ulid"
+Documentation = "https://python-ulid.readthedocs.io/"
+
 [project.optional-dependencies]
 pydantic = [
     "pydantic>=2.0"
 ]
 
 [project.scripts]
 ulid = "ulid.__main__:entrypoint"
```

### Comparing `python_ulid-2.3.0/PKG-INFO` & `python_ulid-2.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 Metadata-Version: 2.3
 Name: python-ulid
-Version: 2.3.0
+Version: 2.4.0
 Summary: Universally unique lexicographically sortable identifier
+Project-URL: Homepage, https://github.com/mdomke/python-ulid
+Project-URL: Repository, https://github.com/mdomke/python-ulid
+Project-URL: Documentation, https://python-ulid.readthedocs.io/
 Author-email: Martin Domke <mail@martindomke.net>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

