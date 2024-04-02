# Comparing `tmp/toolsos-0.2.2.tar.gz` & `tmp/toolsos-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolsos-0.2.2.tar", last modified: Thu Mar 28 13:47:06 2024, max compression
+gzip compressed data, was "toolsos-0.2.3.tar", last modified: Tue Apr  2 13:02:06 2024, max compression
```

## Comparing `toolsos-0.2.2.tar` & `toolsos-0.2.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-03-28 13:47:06.296973 toolsos-0.2.2/
--rw-rw-rw-   0        0        0     2418 2024-03-28 13:47:06.294664 toolsos-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1406 2024-03-28 08:46:48.000000 toolsos-0.2.2/README.md
--rw-rw-rw-   0        0        0     1106 2024-03-28 08:27:37.000000 toolsos-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-28 13:47:06.298108 toolsos-0.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-28 13:47:06.218902 toolsos-0.2.2/src/
-drwxrwxrwx   0        0        0        0 2024-03-28 13:47:06.240797 toolsos-0.2.2/src/toolsos/
--rw-rw-rw-   0        0        0        0 2023-03-09 08:54:45.000000 toolsos-0.2.2/src/toolsos/__init__.py
--rw-rw-rw-   0        0        0     2823 2023-03-03 07:40:20.000000 toolsos-0.2.2/src/toolsos/cbs_tools.py
--rw-rw-rw-   0        0        0      908 2023-10-26 12:51:00.000000 toolsos-0.2.2/src/toolsos/create_tables.py
-drwxrwxrwx   0        0        0        0 2024-03-28 13:47:06.257335 toolsos-0.2.2/src/toolsos/database/
--rw-rw-rw-   0        0        0     3362 2024-03-17 13:47:51.000000 toolsos-0.2.2/src/toolsos/database/database_connection.py
--rw-rw-rw-   0        0        0     1827 2023-10-26 12:54:46.000000 toolsos-0.2.2/src/toolsos/database/database_transfer.py
--rw-rw-rw-   0        0        0     2652 2023-10-26 12:50:51.000000 toolsos-0.2.2/src/toolsos/download.py
--rw-rw-rw-   0        0        0     2412 2023-10-26 12:54:11.000000 toolsos-0.2.2/src/toolsos/geo.py
--rw-rw-rw-   0        0        0      997 2023-10-26 12:54:09.000000 toolsos-0.2.2/src/toolsos/helpers.py
-drwxrwxrwx   0        0        0        0 2024-03-28 13:47:06.261331 toolsos-0.2.2/src/toolsos/huisstijl/
--rw-rw-rw-   0        0        0        0 2024-03-09 19:45:08.000000 toolsos-0.2.2/src/toolsos/huisstijl/__init__.py
--rw-rw-rw-   0        0        0     1484 2024-03-09 07:47:07.000000 toolsos-0.2.2/src/toolsos/huisstijl/colors.py
-drwxrwxrwx   0        0        0        0 2024-03-28 13:47:06.276458 toolsos-0.2.2/src/toolsos/huisstijl/graphs/
--rw-rw-rw-   0        0        0        0 2023-10-20 10:05:27.000000 toolsos-0.2.2/src/toolsos/huisstijl/graphs/__init__.py
--rw-rw-rw-   0        0        0     2582 2023-10-23 07:17:11.000000 toolsos-0.2.2/src/toolsos/huisstijl/graphs/bargraph.py
--rw-rw-rw-   0        0        0      827 2024-03-16 18:43:22.000000 toolsos-0.2.2/src/toolsos/huisstijl/graphs/graph_styles.py
--rw-rw-rw-   0        0        0      527 2024-03-16 18:53:03.000000 toolsos-0.2.2/src/toolsos/huisstijl/graphs/linegraph.py
--rw-rw-rw-   0        0        0      571 2023-10-20 17:25:56.000000 toolsos-0.2.2/src/toolsos/huisstijl/graphs/piegraph.py
--rw-rw-rw-   0        0        0     6626 2024-03-17 10:18:59.000000 toolsos-0.2.2/src/toolsos/huisstijl/graphs/styler.py
-drwxrwxrwx   0        0        0        0 2024-03-28 13:47:06.287647 toolsos-0.2.2/src/toolsos/huisstijl/tables/
--rw-rw-rw-   0        0        0        0 2024-03-09 19:50:14.000000 toolsos-0.2.2/src/toolsos/huisstijl/tables/__init__.py
--rw-rw-rw-   0        0        0     2037 2024-03-28 10:12:33.000000 toolsos-0.2.2/src/toolsos/huisstijl/tables/table_helpers.py
--rw-rw-rw-   0        0        0     1343 2024-03-14 13:23:41.000000 toolsos-0.2.2/src/toolsos/huisstijl/tables/table_styles.py
--rw-rw-rw-   0        0        0    23575 2024-03-28 13:45:46.000000 toolsos-0.2.2/src/toolsos/huisstijl/tables/tables.py
--rw-rw-rw-   0        0        0      770 2023-10-26 12:50:56.000000 toolsos-0.2.2/src/toolsos/polars_helpers.py
-drwxrwxrwx   0        0        0        0 2024-03-28 13:47:06.290663 toolsos-0.2.2/src/toolsos.egg-info/
--rw-rw-rw-   0        0        0     2418 2024-03-28 13:47:06.000000 toolsos-0.2.2/src/toolsos.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      944 2024-03-28 13:47:06.000000 toolsos-0.2.2/src/toolsos.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-28 13:47:06.000000 toolsos-0.2.2/src/toolsos.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      135 2024-03-28 13:47:06.000000 toolsos-0.2.2/src/toolsos.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-28 13:47:06.000000 toolsos-0.2.2/src/toolsos.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 13:02:06.095486 toolsos-0.2.3/
+-rw-rw-rw-   0        0        0     2418 2024-04-02 13:02:06.093658 toolsos-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1406 2024-03-28 08:46:48.000000 toolsos-0.2.3/README.md
+-rw-rw-rw-   0        0        0     1106 2024-04-02 13:01:51.000000 toolsos-0.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-02 13:02:06.095486 toolsos-0.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-02 13:02:06.033057 toolsos-0.2.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-02 13:02:06.049548 toolsos-0.2.3/src/toolsos/
+-rw-rw-rw-   0        0        0        0 2023-03-09 08:54:45.000000 toolsos-0.2.3/src/toolsos/__init__.py
+-rw-rw-rw-   0        0        0     2823 2023-03-03 07:40:20.000000 toolsos-0.2.3/src/toolsos/cbs_tools.py
+-rw-rw-rw-   0        0        0      908 2023-10-26 12:51:00.000000 toolsos-0.2.3/src/toolsos/create_tables.py
+drwxrwxrwx   0        0        0        0 2024-04-02 13:02:06.063713 toolsos-0.2.3/src/toolsos/database/
+-rw-rw-rw-   0        0        0     3362 2024-03-17 13:47:51.000000 toolsos-0.2.3/src/toolsos/database/database_connection.py
+-rw-rw-rw-   0        0        0     1827 2023-10-26 12:54:46.000000 toolsos-0.2.3/src/toolsos/database/database_transfer.py
+-rw-rw-rw-   0        0        0     2652 2023-10-26 12:50:51.000000 toolsos-0.2.3/src/toolsos/download.py
+-rw-rw-rw-   0        0        0     2412 2023-10-26 12:54:11.000000 toolsos-0.2.3/src/toolsos/geo.py
+-rw-rw-rw-   0        0        0      997 2023-10-26 12:54:09.000000 toolsos-0.2.3/src/toolsos/helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-02 13:02:06.067702 toolsos-0.2.3/src/toolsos/huisstijl/
+-rw-rw-rw-   0        0        0        0 2024-03-09 19:45:08.000000 toolsos-0.2.3/src/toolsos/huisstijl/__init__.py
+-rw-rw-rw-   0        0        0     1484 2024-03-09 07:47:07.000000 toolsos-0.2.3/src/toolsos/huisstijl/colors.py
+drwxrwxrwx   0        0        0        0 2024-04-02 13:02:06.080024 toolsos-0.2.3/src/toolsos/huisstijl/graphs/
+-rw-rw-rw-   0        0        0        0 2023-10-20 10:05:27.000000 toolsos-0.2.3/src/toolsos/huisstijl/graphs/__init__.py
+-rw-rw-rw-   0        0        0     2582 2023-10-23 07:17:11.000000 toolsos-0.2.3/src/toolsos/huisstijl/graphs/bargraph.py
+-rw-rw-rw-   0        0        0      827 2024-03-16 18:43:22.000000 toolsos-0.2.3/src/toolsos/huisstijl/graphs/graph_styles.py
+-rw-rw-rw-   0        0        0      659 2024-03-28 14:55:10.000000 toolsos-0.2.3/src/toolsos/huisstijl/graphs/linegraph.py
+-rw-rw-rw-   0        0        0      666 2024-03-28 14:54:10.000000 toolsos-0.2.3/src/toolsos/huisstijl/graphs/piegraph.py
+-rw-rw-rw-   0        0        0     6626 2024-03-17 10:18:59.000000 toolsos-0.2.3/src/toolsos/huisstijl/graphs/styler.py
+drwxrwxrwx   0        0        0        0 2024-04-02 13:02:06.088489 toolsos-0.2.3/src/toolsos/huisstijl/tables/
+-rw-rw-rw-   0        0        0        0 2024-03-09 19:50:14.000000 toolsos-0.2.3/src/toolsos/huisstijl/tables/__init__.py
+-rw-rw-rw-   0        0        0     2037 2024-03-28 10:12:33.000000 toolsos-0.2.3/src/toolsos/huisstijl/tables/table_helpers.py
+-rw-rw-rw-   0        0        0     1343 2024-03-14 13:23:41.000000 toolsos-0.2.3/src/toolsos/huisstijl/tables/table_styles.py
+-rw-rw-rw-   0        0        0    23575 2024-04-02 13:01:28.000000 toolsos-0.2.3/src/toolsos/huisstijl/tables/tables.py
+-rw-rw-rw-   0        0        0      770 2023-10-26 12:50:56.000000 toolsos-0.2.3/src/toolsos/polars_helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-02 13:02:06.090487 toolsos-0.2.3/src/toolsos.egg-info/
+-rw-rw-rw-   0        0        0     2418 2024-04-02 13:02:06.000000 toolsos-0.2.3/src/toolsos.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      944 2024-04-02 13:02:06.000000 toolsos-0.2.3/src/toolsos.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 13:02:06.000000 toolsos-0.2.3/src/toolsos.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      135 2024-04-02 13:02:06.000000 toolsos-0.2.3/src/toolsos.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-02 13:02:06.000000 toolsos-0.2.3/src/toolsos.egg-info/top_level.txt
```

### Comparing `toolsos-0.2.2/PKG-INFO` & `toolsos-0.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: toolsos
-Version: 0.2.2
+Version: 0.2.3
 Summary: OS tools
 Author-email: OS <d.schmitz@amsterdam.nl>
 Keywords: tools,Onderzoek & Statistiek
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
```

### Comparing `toolsos-0.2.2/README.md` & `toolsos-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `toolsos-0.2.2/pyproject.toml` & `toolsos-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "toolsos"
-version = "0.2.2"
+version = "0.2.3"
 description = "OS tools"
 readme = "README.md"
 authors = [{ name = "OS", email = "d.schmitz@amsterdam.nl" }]
 
 # license = { file = "LICENSE" }
 
 classifiers = [
@@ -21,15 +21,15 @@
 
 keywords = ["tools", "Onderzoek & Statistiek"]
 
 # dependencies are kept empty until to be able to install in conda enviroment
 # use pip install "toolsos[all]" to pip install with al dependencies
 
 dependencies = []
-requires-python = ">=3.11"
+requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = [
     "black",
     "bumpver",
     "isort",
     "pip-tools",
```

### Comparing `toolsos-0.2.2/src/toolsos/cbs_tools.py` & `toolsos-0.2.3/src/toolsos/cbs_tools.py`

 * *Files identical despite different names*

### Comparing `toolsos-0.2.2/src/toolsos/create_tables.py` & `toolsos-0.2.3/src/toolsos/create_tables.py`

 * *Files identical despite different names*

### Comparing `toolsos-0.2.2/src/toolsos/database/database_connection.py` & `toolsos-0.2.3/src/toolsos/database/database_connection.py`

 * *Files identical despite different names*

### Comparing `toolsos-0.2.2/src/toolsos/database/database_transfer.py` & `toolsos-0.2.3/src/toolsos/database/database_transfer.py`

 * *Files identical despite different names*

### Comparing `toolsos-0.2.2/src/toolsos/download.py` & `toolsos-0.2.3/src/toolsos/download.py`

 * *Files identical despite different names*

### Comparing `toolsos-0.2.2/src/toolsos/geo.py` & `toolsos-0.2.3/src/toolsos/geo.py`

 * *Files identical despite different names*

### Comparing `toolsos-0.2.2/src/toolsos/helpers.py` & `toolsos-0.2.3/src/toolsos/helpers.py`

 * *Files identical despite different names*

### Comparing `toolsos-0.2.2/src/toolsos/huisstijl/colors.py` & `toolsos-0.2.3/src/toolsos/huisstijl/colors.py`

 * *Files identical despite different names*

### Comparing `toolsos-0.2.2/src/toolsos/huisstijl/graphs/bargraph.py` & `toolsos-0.2.3/src/toolsos/huisstijl/graphs/bargraph.py`

 * *Files identical despite different names*

### Comparing `toolsos-0.2.2/src/toolsos/huisstijl/graphs/graph_styles.py` & `toolsos-0.2.3/src/toolsos/huisstijl/graphs/graph_styles.py`

 * *Files identical despite different names*

### Comparing `toolsos-0.2.2/src/toolsos/huisstijl/graphs/piegraph.py` & `toolsos-0.2.3/src/toolsos/huisstijl/graphs/piegraph.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 import plotly.express as px
+
 from .styler import BaseStyle
 
 basestyle = BaseStyle()
 
 
 def pie(
     data,
     names,
     values,
     hole: float = 0.4,
     width=750,
     height=490,
     text_format: str = None,
+    color_discrete_sequence=None,
     **kwargs,
 ):
     fig = px.pie(
         data_frame=data,
         names=names,
         values=values,
         width=width,
         height=height,
         hole=hole,
         template=BaseStyle().get_base_template(),
+        color_discrete_sequence=color_discrete_sequence,
         **kwargs,
     )
 
     if text_format:
         fig.update_traces(texttemplate=text_format)
 
     return fig
```

### Comparing `toolsos-0.2.2/src/toolsos/huisstijl/graphs/styler.py` & `toolsos-0.2.3/src/toolsos/huisstijl/graphs/styler.py`

 * *Files identical despite different names*

### Comparing `toolsos-0.2.2/src/toolsos/huisstijl/tables/table_helpers.py` & `toolsos-0.2.3/src/toolsos/huisstijl/tables/table_helpers.py`

 * *Files identical despite different names*

### Comparing `toolsos-0.2.2/src/toolsos/huisstijl/tables/table_styles.py` & `toolsos-0.2.3/src/toolsos/huisstijl/tables/table_styles.py`

 * *Files identical despite different names*

### Comparing `toolsos-0.2.2/src/toolsos/huisstijl/tables/tables.py` & `toolsos-0.2.3/src/toolsos/huisstijl/tables/tables.py`

 * *Files identical despite different names*

### Comparing `toolsos-0.2.2/src/toolsos/polars_helpers.py` & `toolsos-0.2.3/src/toolsos/polars_helpers.py`

 * *Files identical despite different names*

### Comparing `toolsos-0.2.2/src/toolsos.egg-info/PKG-INFO` & `toolsos-0.2.3/src/toolsos.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: toolsos
-Version: 0.2.2
+Version: 0.2.3
 Summary: OS tools
 Author-email: OS <d.schmitz@amsterdam.nl>
 Keywords: tools,Onderzoek & Statistiek
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
```

### Comparing `toolsos-0.2.2/src/toolsos.egg-info/SOURCES.txt` & `toolsos-0.2.3/src/toolsos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

