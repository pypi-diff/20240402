# Comparing `tmp/minto-0.8.3.tar.gz` & `tmp/minto-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minto-0.8.3.tar", max compression
+gzip compressed data, was "minto-0.8.4.tar", max compression
```

## Comparing `minto-0.8.3.tar` & `minto-0.8.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1060 2024-03-07 23:02:40.648580 minto-0.8.3/LICENSE
--rw-r--r--   0        0        0     1749 2024-03-07 23:02:40.648580 minto-0.8.3/README.md
--rw-r--r--   0        0        0      261 2024-03-07 23:02:40.660580 minto-0.8.3/minto/__init__.py
--rw-r--r--   0        0        0        0 2024-03-07 23:02:40.660580 minto-0.8.3/minto/consts/__init__.py
--rw-r--r--   0        0        0      233 2024-03-07 23:02:40.660580 minto-0.8.3/minto/consts/default.py
--rw-r--r--   0        0        0      229 2024-03-07 23:02:40.660580 minto-0.8.3/minto/exceptions/__init__.py
--rw-r--r--   0        0        0       76 2024-03-07 23:02:40.660580 minto-0.8.3/minto/exceptions/exceptions.py
--rw-r--r--   0        0        0       83 2024-03-07 23:02:40.660580 minto-0.8.3/minto/experiment/__init__.py
--rw-r--r--   0        0        0    14811 2024-03-07 23:02:40.660580 minto-0.8.3/minto/experiment/experiment.py
--rw-r--r--   0        0        0      176 2024-03-07 23:02:40.660580 minto-0.8.3/minto/io/__init__.py
--rw-r--r--   0        0        0     5603 2024-03-07 23:02:40.660580 minto-0.8.3/minto/io/load.py
--rw-r--r--   0        0        0     5454 2024-03-07 23:02:40.660580 minto-0.8.3/minto/io/save.py
--rw-r--r--   0        0        0        0 2024-03-07 23:02:40.660580 minto-0.8.3/minto/records/__init__.py
--rw-r--r--   0        0        0     3860 2024-03-07 23:02:40.660580 minto-0.8.3/minto/records/records.py
--rw-r--r--   0        0        0     3142 2024-03-07 23:02:40.660580 minto-0.8.3/minto/records/sampleset_expansion.py
--rw-r--r--   0        0        0        0 2024-03-07 23:02:40.660580 minto-0.8.3/minto/table/__init__.py
--rw-r--r--   0        0        0     3298 2024-03-07 23:02:40.660580 minto-0.8.3/minto/table/table.py
--rw-r--r--   0        0        0      163 2024-03-07 23:02:40.660580 minto-0.8.3/minto/typing.py
--rw-r--r--   0        0        0     2177 2024-03-07 23:03:06.985263 minto-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     2922 1970-01-01 00:00:00.000000 minto-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-04-02 09:37:16.247682 minto-0.8.4/LICENSE
+-rw-r--r--   0        0        0     1749 2024-04-02 09:37:16.247682 minto-0.8.4/README.md
+-rw-r--r--   0        0        0      261 2024-04-02 09:37:16.255682 minto-0.8.4/minto/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 09:37:16.255682 minto-0.8.4/minto/consts/__init__.py
+-rw-r--r--   0        0        0      233 2024-04-02 09:37:16.255682 minto-0.8.4/minto/consts/default.py
+-rw-r--r--   0        0        0      229 2024-04-02 09:37:16.255682 minto-0.8.4/minto/exceptions/__init__.py
+-rw-r--r--   0        0        0       76 2024-04-02 09:37:16.255682 minto-0.8.4/minto/exceptions/exceptions.py
+-rw-r--r--   0        0        0       83 2024-04-02 09:37:16.255682 minto-0.8.4/minto/experiment/__init__.py
+-rw-r--r--   0        0        0    14811 2024-04-02 09:37:16.259683 minto-0.8.4/minto/experiment/experiment.py
+-rw-r--r--   0        0        0      176 2024-04-02 09:37:16.259683 minto-0.8.4/minto/io/__init__.py
+-rw-r--r--   0        0        0     5603 2024-04-02 09:37:16.259683 minto-0.8.4/minto/io/load.py
+-rw-r--r--   0        0        0     5423 2024-04-02 09:37:16.259683 minto-0.8.4/minto/io/save.py
+-rw-r--r--   0        0        0        0 2024-04-02 09:37:16.259683 minto-0.8.4/minto/records/__init__.py
+-rw-r--r--   0        0        0     3860 2024-04-02 09:37:16.259683 minto-0.8.4/minto/records/records.py
+-rw-r--r--   0        0        0     3142 2024-04-02 09:37:16.259683 minto-0.8.4/minto/records/sampleset_expansion.py
+-rw-r--r--   0        0        0        0 2024-04-02 09:37:16.259683 minto-0.8.4/minto/table/__init__.py
+-rw-r--r--   0        0        0     3298 2024-04-02 09:37:16.259683 minto-0.8.4/minto/table/table.py
+-rw-r--r--   0        0        0      163 2024-04-02 09:37:16.259683 minto-0.8.4/minto/typing.py
+-rw-r--r--   0        0        0     2197 2024-04-02 09:37:35.079978 minto-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 minto-0.8.4/PKG-INFO
```

### Comparing `minto-0.8.3/LICENSE` & `minto-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `minto-0.8.3/README.md` & `minto-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `minto-0.8.3/minto/experiment/experiment.py` & `minto-0.8.4/minto/experiment/experiment.py`

 * *Files identical despite different names*

### Comparing `minto-0.8.3/minto/io/load.py` & `minto-0.8.4/minto/io/load.py`

 * *Files identical despite different names*

### Comparing `minto-0.8.3/minto/io/save.py` & `minto-0.8.4/minto/io/save.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         # save problem
         if isinstance(content, jm.Problem):
             with open(base_dir / f"{key}" / "problems" / f"{content_id}.pb", "wb") as f:
                 f.write(jm.to_protobuf(content))
 
         # save jijzept JijModelingResponse
         elif isinstance(content, JijModelingResponse):
-            sampleset = jm.experimental.from_old_sampleset(content.sample_set)
+            sampleset = content.get_sampleset()
             with open(
                 base_dir / f"{key}" / "samplesets" / f"{content_id}.json", "w"
             ) as f:
                 json.dump(sampleset.to_dict(), f, cls=_NumpyEncoder)
 
         # save jijmodeling SampleSet
         elif isinstance(content, jm.SampleSet):
```

### Comparing `minto-0.8.3/minto/records/records.py` & `minto-0.8.4/minto/records/records.py`

 * *Files identical despite different names*

### Comparing `minto-0.8.3/minto/records/sampleset_expansion.py` & `minto-0.8.4/minto/records/sampleset_expansion.py`

 * *Files identical despite different names*

### Comparing `minto-0.8.3/minto/table/table.py` & `minto-0.8.4/minto/table/table.py`

 * *Files identical despite different names*

### Comparing `minto-0.8.3/pyproject.toml` & `minto-0.8.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -29,22 +29,23 @@
 documentation = "https://jij-inc.github.io/minto" 
 homepage = "https://www.j-ij.com/" 
 include = ["minto/*.py"] 
 license = "MIT" 
 name = "minto" 
 readme = "README.md" 
 repository = "https://github.com/Jij-Inc/MINTO-Public" 
-version = "0.8.3" # using poetry-dynamic-versioning
+version = "0.8.4" # using poetry-dynamic-versioning
 
 [tool.poetry.dependencies]
-jijmodeling = "^1.0.0"
+jijmodeling = "^1.3.3"
 jijzept = "^1.16.9"
 numpy = "^1.24.2"
 pandas = ">=1.5.3,<3.0.0"
 protobuf = "^4.24.0"
+pyarrow = "^15.0.2"
 pydantic = "^2.0.0"
 python = ">=3.9,<3.12"
 
 [tool.poetry.group.tests.dependencies]
 coverage = "^7.2.2"
 jijmodeling-transpiler = "^0.6.13"
 openjij = ">=0.7.3,<0.10.0"
```

### Comparing `minto-0.8.3/PKG-INFO` & `minto-0.8.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minto
-Version: 0.8.3
+Version: 0.8.4
 Summary: Experiment management and benchmark tools for mathematical optimization
 Home-page: https://www.j-ij.com/
 License: MIT
 Author: Jij Inc.
 Author-email: info@j-ij.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -14,19 +14,20 @@
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Dist: jijmodeling (>=1.0.0,<2.0.0)
+Requires-Dist: jijmodeling (>=1.3.3,<2.0.0)
 Requires-Dist: jijzept (>=1.16.9,<2.0.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<3.0.0)
 Requires-Dist: protobuf (>=4.24.0,<5.0.0)
+Requires-Dist: pyarrow (>=15.0.2,<16.0.0)
 Requires-Dist: pydantic (>=2.0.0,<3.0.0)
 Project-URL: Documentation, https://jij-inc.github.io/minto
 Project-URL: Repository, https://github.com/Jij-Inc/MINTO-Public
 Description-Content-Type: text/markdown
 
 
 # MINTO: Jij Management and Insight tool for Optimization
```

