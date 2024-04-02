# Comparing `tmp/covjson_pydantic-0.2.1.tar.gz` & `tmp/covjson_pydantic-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covjson_pydantic-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "covjson_pydantic-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `covjson_pydantic-0.2.1.tar` & `covjson_pydantic-0.3.0.tar`

### file list

```diff
@@ -1,45 +1,48 @@
--rw-r--r--   0        0        0      273 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/.gitignore
--rw-r--r--   0        0        0     2598 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11383 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/LICENSE
--rw-r--r--   0        0        0     4299 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/README.md
--rw-r--r--   0        0        0      811 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/example.py
--rw-r--r--   0        0        0     1196 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      208 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/setup.py
--rw-r--r--   0        0        0        0 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/src/covjson_pydantic/__init__.py
--rw-r--r--   0        0        0      337 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/src/covjson_pydantic/base_models.py
--rw-r--r--   0        0        0     1194 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/src/covjson_pydantic/coverage.py
--rw-r--r--   0        0        0     6652 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/src/covjson_pydantic/domain.py
--rw-r--r--   0        0        0      585 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/src/covjson_pydantic/i18n.py
--rw-r--r--   0        0        0     1965 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/src/covjson_pydantic/ndarray.py
--rw-r--r--   0        0        0      397 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/src/covjson_pydantic/observed_property.py
--rw-r--r--   0        0        0     1751 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/src/covjson_pydantic/parameter.py
--rw-r--r--   0        0        0        0 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/src/covjson_pydantic/py.typed
--rw-r--r--   0        0        0     1919 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/src/covjson_pydantic/reference_system.py
--rw-r--r--   0        0        0      591 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/src/covjson_pydantic/unit.py
--rw-r--r--   0        0        0        0 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0     2882 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/tests/test_coverage.py
--rw-r--r--   0        0        0     1003 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/tests/test_data/categorical-data-parameter.json
--rw-r--r--   0        0        0      685 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/tests/test_data/continuous-data-parameter.json
--rw-r--r--   0        0        0     3007 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/tests/test_data/coverage-json.json
--rw-r--r--   0        0        0     4306 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/tests/test_data/doc-example-coverage-collection.json
--rw-r--r--   0        0        0     1890 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/tests/test_data/doc-example-coverage.json
--rw-r--r--   0        0        0      866 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/tests/test_data/grid-domain-no-y.json
--rw-r--r--   0        0        0     1074 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/tests/test_data/grid-domain.json
--rw-r--r--   0        0        0      275 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/tests/test_data/ndarray-float.json
--rw-r--r--   0        0        0      938 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/tests/test_data/point-series-domain-custom.json
--rw-r--r--   0        0        0     1000 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/tests/test_data/point-series-domain-more-z.json
--rw-r--r--   0        0        0      528 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/tests/test_data/point-series-domain-no-t.json
--rw-r--r--   0        0        0      769 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/tests/test_data/spec-axes.json
--rw-r--r--   0        0        0      491 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/tests/test_data/spec-domain-grid.json
--rw-r--r--   0        0        0      648 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/tests/test_data/spec-domain-multipoint-series.json
--rw-r--r--   0        0        0      614 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/tests/test_data/spec-domain-multipoint.json
--rw-r--r--   0        0        0      471 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/tests/test_data/spec-domain-point-compact.json
--rw-r--r--   0        0        0      474 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/tests/test_data/spec-domain-point-series.json
--rw-r--r--   0        0        0      428 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/tests/test_data/spec-domain-point.json
--rw-r--r--   0        0        0      481 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/tests/test_data/spec-domain-vertical-profile.json
--rw-r--r--   0        0        0      278 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/tests/test_data/spec-ndarray.json
--rw-r--r--   0        0        0      381 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/tests/test_data/spec-parametergroup.json
--rw-r--r--   0        0        0      754 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/tests/test_data/spec-reference-system-identifierrs.json
--rw-r--r--   0        0        0      764 2024-01-18 11:43:29.619603 covjson_pydantic-0.2.1/tests/test_data/spec-tiled-ndarray.json
--rw-r--r--   0        0        0     4938 2024-01-18 11:43:29.623603 covjson_pydantic-0.2.1/tests/test_data/spec-vertical-profile-coverage.json
--rw-r--r--   0        0        0     5266 1970-01-01 00:00:00.000000 covjson_pydantic-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      273 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/.gitignore
+-rw-r--r--   0        0        0     2598 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11383 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4299 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/README.md
+-rw-r--r--   0        0        0      811 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/example.py
+-rw-r--r--   0        0        0     1196 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      208 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/setup.py
+-rw-r--r--   0        0        0        0 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/src/covjson_pydantic/__init__.py
+-rw-r--r--   0        0        0      337 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/src/covjson_pydantic/base_models.py
+-rw-r--r--   0        0        0     1194 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/src/covjson_pydantic/coverage.py
+-rw-r--r--   0        0        0     6703 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/src/covjson_pydantic/domain.py
+-rw-r--r--   0        0        0      585 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/src/covjson_pydantic/i18n.py
+-rw-r--r--   0        0        0     1965 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/src/covjson_pydantic/ndarray.py
+-rw-r--r--   0        0        0      397 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/src/covjson_pydantic/observed_property.py
+-rw-r--r--   0        0        0     1751 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/src/covjson_pydantic/parameter.py
+-rw-r--r--   0        0        0        0 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/src/covjson_pydantic/py.typed
+-rw-r--r--   0        0        0     1919 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/src/covjson_pydantic/reference_system.py
+-rw-r--r--   0        0        0      591 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/src/covjson_pydantic/unit.py
+-rw-r--r--   0        0        0        0 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     3055 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/tests/test_coverage.py
+-rw-r--r--   0        0        0     1003 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/tests/test_data/categorical-data-parameter.json
+-rw-r--r--   0        0        0      685 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/tests/test_data/continuous-data-parameter.json
+-rw-r--r--   0        0        0     3007 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/tests/test_data/coverage-json.json
+-rw-r--r--   0        0        0     4306 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/tests/test_data/doc-example-coverage-collection.json
+-rw-r--r--   0        0        0     1890 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/tests/test_data/doc-example-coverage.json
+-rw-r--r--   0        0        0      866 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/tests/test_data/grid-domain-no-y.json
+-rw-r--r--   0        0        0     1074 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/tests/test_data/grid-domain.json
+-rw-r--r--   0        0        0       87 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/tests/test_data/mixed-type-axes-2.json
+-rw-r--r--   0        0        0       87 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/tests/test_data/mixed-type-axes.json
+-rw-r--r--   0        0        0      275 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/tests/test_data/ndarray-float.json
+-rw-r--r--   0        0        0      938 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/tests/test_data/point-series-domain-custom.json
+-rw-r--r--   0        0        0     1000 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/tests/test_data/point-series-domain-more-z.json
+-rw-r--r--   0        0        0      528 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/tests/test_data/point-series-domain-no-t.json
+-rw-r--r--   0        0        0      769 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/tests/test_data/spec-axes.json
+-rw-r--r--   0        0        0      491 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/tests/test_data/spec-domain-grid.json
+-rw-r--r--   0        0        0      648 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/tests/test_data/spec-domain-multipoint-series.json
+-rw-r--r--   0        0        0      614 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/tests/test_data/spec-domain-multipoint.json
+-rw-r--r--   0        0        0      471 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/tests/test_data/spec-domain-point-compact.json
+-rw-r--r--   0        0        0      474 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/tests/test_data/spec-domain-point-series.json
+-rw-r--r--   0        0        0      428 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/tests/test_data/spec-domain-point.json
+-rw-r--r--   0        0        0      481 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/tests/test_data/spec-domain-vertical-profile.json
+-rw-r--r--   0        0        0      278 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/tests/test_data/spec-ndarray.json
+-rw-r--r--   0        0        0      381 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/tests/test_data/spec-parametergroup.json
+-rw-r--r--   0        0        0      754 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/tests/test_data/spec-reference-system-identifierrs.json
+-rw-r--r--   0        0        0      764 2024-04-02 09:18:51.297978 covjson_pydantic-0.3.0/tests/test_data/spec-tiled-ndarray.json
+-rw-r--r--   0        0        0     4938 2024-04-02 09:18:51.301977 covjson_pydantic-0.3.0/tests/test_data/spec-vertical-profile-coverage.json
+-rw-r--r--   0        0        0       88 2024-04-02 09:18:51.301977 covjson_pydantic-0.3.0/tests/test_data/str-axes.json
+-rw-r--r--   0        0        0     5266 1970-01-01 00:00:00.000000 covjson_pydantic-0.3.0/PKG-INFO
```

### Comparing `covjson_pydantic-0.2.1/.pre-commit-config.yaml` & `covjson_pydantic-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `covjson_pydantic-0.2.1/LICENSE` & `covjson_pydantic-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `covjson_pydantic-0.2.1/README.md` & `covjson_pydantic-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `covjson_pydantic-0.2.1/example.py` & `covjson_pydantic-0.3.0/example.py`

 * *Files identical despite different names*

### Comparing `covjson_pydantic-0.2.1/pyproject.toml` & `covjson_pydantic-0.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: GIS",
     "Typing :: Typed",
 ]
-version = "0.2.1"
+version = "0.3.0"
 dependencies = ["pydantic>=2.3,<3"]
 
 [project.optional-dependencies]
 test = ["pytest", "pytest-cov"]
 dev = ["pre-commit"]
 
 [project.urls]
```

### Comparing `covjson_pydantic-0.2.1/src/covjson_pydantic/coverage.py` & `covjson_pydantic-0.3.0/src/covjson_pydantic/coverage.py`

 * *Files identical despite different names*

### Comparing `covjson_pydantic-0.2.1/src/covjson_pydantic/domain.py` & `covjson_pydantic-0.3.0/src/covjson_pydantic/domain.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,17 +52,17 @@
     point_series = "PointSeries"
     point = "Point"
     multi_point_series = "MultiPointSeries"
     multi_point = "MultiPoint"
 
 
 class Axes(CovJsonBaseModel):
-    x: Optional[Union[ValuesAxis[float], CompactAxis]] = None
-    y: Optional[Union[ValuesAxis[float], CompactAxis]] = None
-    z: Optional[Union[ValuesAxis[float], CompactAxis]] = None
+    x: Optional[Union[ValuesAxis[float], ValuesAxis[str], CompactAxis]] = None
+    y: Optional[Union[ValuesAxis[float], ValuesAxis[str], CompactAxis]] = None
+    z: Optional[Union[ValuesAxis[float], ValuesAxis[str], CompactAxis]] = None
     t: Optional[ValuesAxis[AwareDatetime]] = None
     composite: Optional[ValuesAxis[Tuple]] = None
 
     @model_validator(mode="after")
     def at_least_one_axes(self):
         if self.x is None and self.y is None and self.z is None and self.t is None and self.composite is None:
             raise ValueError("At least one axis of x,y,z,t or composite must be given.")
```

### Comparing `covjson_pydantic-0.2.1/src/covjson_pydantic/i18n.py` & `covjson_pydantic-0.3.0/src/covjson_pydantic/i18n.py`

 * *Files identical despite different names*

### Comparing `covjson_pydantic-0.2.1/src/covjson_pydantic/ndarray.py` & `covjson_pydantic-0.3.0/src/covjson_pydantic/ndarray.py`

 * *Files identical despite different names*

### Comparing `covjson_pydantic-0.2.1/src/covjson_pydantic/parameter.py` & `covjson_pydantic-0.3.0/src/covjson_pydantic/parameter.py`

 * *Files identical despite different names*

### Comparing `covjson_pydantic-0.2.1/src/covjson_pydantic/reference_system.py` & `covjson_pydantic-0.3.0/src/covjson_pydantic/reference_system.py`

 * *Files identical despite different names*

### Comparing `covjson_pydantic-0.2.1/src/covjson_pydantic/unit.py` & `covjson_pydantic-0.3.0/src/covjson_pydantic/unit.py`

 * *Files identical despite different names*

### Comparing `covjson_pydantic-0.2.1/tests/test_coverage.py` & `covjson_pydantic-0.3.0/tests/test_coverage.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from covjson_pydantic.parameter import ParameterGroup
 from covjson_pydantic.reference_system import ReferenceSystem
 from pydantic import ValidationError
 
 
 happy_cases = [
     ("spec-axes.json", Axes),
+    ("str-axes.json", Axes),
     ("coverage-json.json", Coverage),
     ("doc-example-coverage.json", Coverage),
     ("spec-vertical-profile-coverage.json", Coverage),
     ("doc-example-coverage-collection.json", CoverageCollection),
     ("grid-domain.json", Domain),
     ("point-series-domain-custom.json", Domain),
     ("spec-domain-grid.json", Domain),
@@ -56,14 +57,16 @@
     (
         "point-series-domain-more-z.json",
         Domain,
         r"If provided, the 'values' field of the ValuesAxis 'z'-axis of a 'PointSeries' "
         + "domain must contain a single value.",
     ),
     ("point-series-domain-no-t.json", Domain, r"A 'PointSeries' must have a 't'-axis."),
+    ("mixed-type-axes.json", Axes, r"Input should be a valid number"),
+    ("mixed-type-axes-2.json", Axes, r"Input should be a valid string"),
 ]
 
 
 @pytest.mark.parametrize("file_name, object_type, error_message", error_cases)
 def test_error_cases(file_name, object_type, error_message):
     file = Path(__file__).parent.resolve() / "test_data" / file_name
     # Put JSON in default unindented format
```

### Comparing `covjson_pydantic-0.2.1/tests/test_data/categorical-data-parameter.json` & `covjson_pydantic-0.3.0/tests/test_data/categorical-data-parameter.json`

 * *Files identical despite different names*

### Comparing `covjson_pydantic-0.2.1/tests/test_data/continuous-data-parameter.json` & `covjson_pydantic-0.3.0/tests/test_data/continuous-data-parameter.json`

 * *Files identical despite different names*

### Comparing `covjson_pydantic-0.2.1/tests/test_data/coverage-json.json` & `covjson_pydantic-0.3.0/tests/test_data/coverage-json.json`

 * *Files identical despite different names*

### Comparing `covjson_pydantic-0.2.1/tests/test_data/doc-example-coverage-collection.json` & `covjson_pydantic-0.3.0/tests/test_data/doc-example-coverage-collection.json`

 * *Files identical despite different names*

### Comparing `covjson_pydantic-0.2.1/tests/test_data/doc-example-coverage.json` & `covjson_pydantic-0.3.0/tests/test_data/doc-example-coverage.json`

 * *Files identical despite different names*

### Comparing `covjson_pydantic-0.2.1/tests/test_data/grid-domain-no-y.json` & `covjson_pydantic-0.3.0/tests/test_data/grid-domain-no-y.json`

 * *Files identical despite different names*

### Comparing `covjson_pydantic-0.2.1/tests/test_data/grid-domain.json` & `covjson_pydantic-0.3.0/tests/test_data/grid-domain.json`

 * *Files identical despite different names*

### Comparing `covjson_pydantic-0.2.1/tests/test_data/point-series-domain-custom.json` & `covjson_pydantic-0.3.0/tests/test_data/point-series-domain-custom.json`

 * *Files identical despite different names*

### Comparing `covjson_pydantic-0.2.1/tests/test_data/point-series-domain-more-z.json` & `covjson_pydantic-0.3.0/tests/test_data/point-series-domain-more-z.json`

 * *Files identical despite different names*

### Comparing `covjson_pydantic-0.2.1/tests/test_data/point-series-domain-no-t.json` & `covjson_pydantic-0.3.0/tests/test_data/point-series-domain-no-t.json`

 * *Files identical despite different names*

### Comparing `covjson_pydantic-0.2.1/tests/test_data/spec-axes.json` & `covjson_pydantic-0.3.0/tests/test_data/spec-axes.json`

 * *Files identical despite different names*

### Comparing `covjson_pydantic-0.2.1/tests/test_data/spec-domain-multipoint-series.json` & `covjson_pydantic-0.3.0/tests/test_data/spec-domain-multipoint-series.json`

 * *Files identical despite different names*

### Comparing `covjson_pydantic-0.2.1/tests/test_data/spec-domain-multipoint.json` & `covjson_pydantic-0.3.0/tests/test_data/spec-domain-multipoint.json`

 * *Files identical despite different names*

### Comparing `covjson_pydantic-0.2.1/tests/test_data/spec-reference-system-identifierrs.json` & `covjson_pydantic-0.3.0/tests/test_data/spec-reference-system-identifierrs.json`

 * *Files identical despite different names*

### Comparing `covjson_pydantic-0.2.1/tests/test_data/spec-tiled-ndarray.json` & `covjson_pydantic-0.3.0/tests/test_data/spec-tiled-ndarray.json`

 * *Files identical despite different names*

### Comparing `covjson_pydantic-0.2.1/tests/test_data/spec-vertical-profile-coverage.json` & `covjson_pydantic-0.3.0/tests/test_data/spec-vertical-profile-coverage.json`

 * *Files identical despite different names*

### Comparing `covjson_pydantic-0.2.1/PKG-INFO` & `covjson_pydantic-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covjson-pydantic
-Version: 0.2.1
+Version: 0.3.0
 Summary: The Pydantic models for CoverageJSON
 Keywords: covjson,Pydantic
 Author-email: KNMI Data Platform Team <opendata@knmi.nl>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: covjson-pydantic Version: 0.2.1 Summary: The
+Metadata-Version: 2.1 Name: covjson-pydantic Version: 0.3.0 Summary: The
 Pydantic models for CoverageJSON Keywords: covjson,Pydantic Author-email: KNMI
 Data Platform Team
 knmi.nl> Requires-Python: >=3.8 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

