# Comparing `tmp/tidydata-0.1.8.tar.gz` & `tmp/tidydata-0.1.9.tar.gz`

## Comparing `tidydata-0.1.8.tar` & `tidydata-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 tidydata-0.1.8/.python-version
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 tidydata-0.1.8/requirements-dev.lock
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 tidydata-0.1.8/requirements.lock
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 tidydata-0.1.8/src/tidydata/__init__.py
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 tidydata-0.1.8/src/tidydata/command.py
--rw-r--r--   0        0        0    13946 2020-02-02 00:00:00.000000 tidydata-0.1.8/src/tidydata/config.py
--rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 tidydata-0.1.8/src/tidydata/io.py
--rw-r--r--   0        0        0    21441 2020-02-02 00:00:00.000000 tidydata-0.1.8/src/tidydata/table.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tidydata-0.1.8/.gitignore
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 tidydata-0.1.8/README.md
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 tidydata-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 tidydata-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 tidydata-0.1.9/.python-version
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 tidydata-0.1.9/requirements-dev.lock
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 tidydata-0.1.9/requirements.lock
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 tidydata-0.1.9/src/tidydata/__init__.py
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 tidydata-0.1.9/src/tidydata/command.py
+-rw-r--r--   0        0        0    13946 2020-02-02 00:00:00.000000 tidydata-0.1.9/src/tidydata/config.py
+-rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 tidydata-0.1.9/src/tidydata/io.py
+-rw-r--r--   0        0        0    21441 2020-02-02 00:00:00.000000 tidydata-0.1.9/src/tidydata/table.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tidydata-0.1.9/.gitignore
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 tidydata-0.1.9/README.md
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 tidydata-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 tidydata-0.1.9/PKG-INFO
```

### Comparing `tidydata-0.1.8/requirements-dev.lock` & `tidydata-0.1.9/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `tidydata-0.1.8/requirements.lock` & `tidydata-0.1.9/requirements.lock`

 * *Files identical despite different names*

### Comparing `tidydata-0.1.8/src/tidydata/command.py` & `tidydata-0.1.9/src/tidydata/command.py`

 * *Files identical despite different names*

### Comparing `tidydata-0.1.8/src/tidydata/config.py` & `tidydata-0.1.9/src/tidydata/config.py`

 * *Files identical despite different names*

### Comparing `tidydata-0.1.8/src/tidydata/io.py` & `tidydata-0.1.9/src/tidydata/io.py`

 * *Files identical despite different names*

### Comparing `tidydata-0.1.8/src/tidydata/table.py` & `tidydata-0.1.9/src/tidydata/table.py`

 * *Files identical despite different names*

### Comparing `tidydata-0.1.8/pyproject.toml` & `tidydata-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tidydata"
-version = "0.1.8"
+version = "0.1.9"
 description = "Data cleaner for economic research"
 authors = [
     { name = "kyrie1218", email = "kyrie1218@163.com" }
 ]
 dependencies = [
     "pandas[performance,computation, plot,output-formatting,html, xml,hdf5, parquet, feather, spss, excel]==2.1.1",
     "ipykernel==6.25.2",
@@ -16,15 +16,15 @@
     "loguru==0.7.2",
     "strictyaml==1.7.3",
     "click==8.1.7",
     "seedir==0.4.2",
     "emoji==2.8.0",
 ]
 readme = "README.md"
-requires-python = "== 3.11.5"
+requires-python = "==3.11.5"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.rye]
 managed = true
```

