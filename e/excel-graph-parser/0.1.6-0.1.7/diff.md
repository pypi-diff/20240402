# Comparing `tmp/excel_graph_parser-0.1.6.tar.gz` & `tmp/excel_graph_parser-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "excel_graph_parser-0.1.6.tar", last modified: Thu Mar 14 14:49:25 2024, max compression
+gzip compressed data, was "excel_graph_parser-0.1.7.tar", last modified: Tue Apr  2 14:25:24 2024, max compression
```

## Comparing `excel_graph_parser-0.1.6.tar` & `excel_graph_parser-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 dsommers  (1000) dsommers  (1000)        0 2024-03-14 14:49:24.997469 excel_graph_parser-0.1.6/
--rw-r--r--   0 dsommers  (1000) dsommers  (1000)     1063 2024-02-13 13:30:58.000000 excel_graph_parser-0.1.6/LICENSE
--rw-r--r--   0 dsommers  (1000) dsommers  (1000)     2655 2024-03-14 14:49:24.997469 excel_graph_parser-0.1.6/PKG-INFO
--rw-r--r--   0 dsommers  (1000) dsommers  (1000)      759 2024-02-14 06:51:33.000000 excel_graph_parser-0.1.6/README.md
-drwxr-xr-x   0 dsommers  (1000) dsommers  (1000)        0 2024-03-14 14:49:24.997469 excel_graph_parser-0.1.6/excel_graph_parser/
--rw-r--r--   0 dsommers  (1000) dsommers  (1000)      140 2024-02-13 14:42:52.000000 excel_graph_parser-0.1.6/excel_graph_parser/__init__.py
--rw-r--r--   0 dsommers  (1000) dsommers  (1000)    13459 2024-03-14 14:32:27.000000 excel_graph_parser-0.1.6/excel_graph_parser/graph_parser.py
-drwxr-xr-x   0 dsommers  (1000) dsommers  (1000)        0 2024-03-14 14:49:24.997469 excel_graph_parser-0.1.6/excel_graph_parser.egg-info/
--rw-r--r--   0 dsommers  (1000) dsommers  (1000)     2655 2024-03-14 14:49:24.000000 excel_graph_parser-0.1.6/excel_graph_parser.egg-info/PKG-INFO
--rw-r--r--   0 dsommers  (1000) dsommers  (1000)      307 2024-03-14 14:49:24.000000 excel_graph_parser-0.1.6/excel_graph_parser.egg-info/SOURCES.txt
--rw-r--r--   0 dsommers  (1000) dsommers  (1000)        1 2024-03-14 14:49:24.000000 excel_graph_parser-0.1.6/excel_graph_parser.egg-info/dependency_links.txt
--rw-r--r--   0 dsommers  (1000) dsommers  (1000)       49 2024-03-14 14:49:24.000000 excel_graph_parser-0.1.6/excel_graph_parser.egg-info/requires.txt
--rw-r--r--   0 dsommers  (1000) dsommers  (1000)       19 2024-03-14 14:49:24.000000 excel_graph_parser-0.1.6/excel_graph_parser.egg-info/top_level.txt
--rw-r--r--   0 dsommers  (1000) dsommers  (1000)     1209 2024-03-14 14:47:57.000000 excel_graph_parser-0.1.6/pyproject.toml
--rw-r--r--   0 dsommers  (1000) dsommers  (1000)       38 2024-03-14 14:49:24.997469 excel_graph_parser-0.1.6/setup.cfg
+drwxr-xr-x   0 dsommers  (1000) dsommers  (1000)        0 2024-04-02 14:25:24.869022 excel_graph_parser-0.1.7/
+-rw-r--r--   0 dsommers  (1000) dsommers  (1000)     1063 2024-02-13 13:30:58.000000 excel_graph_parser-0.1.7/LICENSE
+-rw-r--r--   0 dsommers  (1000) dsommers  (1000)     2655 2024-04-02 14:25:24.869022 excel_graph_parser-0.1.7/PKG-INFO
+-rw-r--r--   0 dsommers  (1000) dsommers  (1000)      759 2024-02-14 06:51:33.000000 excel_graph_parser-0.1.7/README.md
+drwxr-xr-x   0 dsommers  (1000) dsommers  (1000)        0 2024-04-02 14:25:24.859020 excel_graph_parser-0.1.7/excel_graph_parser/
+-rw-r--r--   0 dsommers  (1000) dsommers  (1000)      140 2024-02-13 14:42:52.000000 excel_graph_parser-0.1.7/excel_graph_parser/__init__.py
+-rw-r--r--   0 dsommers  (1000) dsommers  (1000)    13582 2024-04-02 14:24:07.000000 excel_graph_parser-0.1.7/excel_graph_parser/graph_parser.py
+drwxr-xr-x   0 dsommers  (1000) dsommers  (1000)        0 2024-04-02 14:25:24.869022 excel_graph_parser-0.1.7/excel_graph_parser.egg-info/
+-rw-r--r--   0 dsommers  (1000) dsommers  (1000)     2655 2024-04-02 14:25:24.000000 excel_graph_parser-0.1.7/excel_graph_parser.egg-info/PKG-INFO
+-rw-r--r--   0 dsommers  (1000) dsommers  (1000)      307 2024-04-02 14:25:24.000000 excel_graph_parser-0.1.7/excel_graph_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 dsommers  (1000) dsommers  (1000)        1 2024-04-02 14:25:24.000000 excel_graph_parser-0.1.7/excel_graph_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 dsommers  (1000) dsommers  (1000)       49 2024-04-02 14:25:24.000000 excel_graph_parser-0.1.7/excel_graph_parser.egg-info/requires.txt
+-rw-r--r--   0 dsommers  (1000) dsommers  (1000)       19 2024-04-02 14:25:24.000000 excel_graph_parser-0.1.7/excel_graph_parser.egg-info/top_level.txt
+-rw-r--r--   0 dsommers  (1000) dsommers  (1000)     1209 2024-04-02 14:24:07.000000 excel_graph_parser-0.1.7/pyproject.toml
+-rw-r--r--   0 dsommers  (1000) dsommers  (1000)       38 2024-04-02 14:25:24.869022 excel_graph_parser-0.1.7/setup.cfg
```

### Comparing `excel_graph_parser-0.1.6/LICENSE` & `excel_graph_parser-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `excel_graph_parser-0.1.6/PKG-INFO` & `excel_graph_parser-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excel_graph_parser
-Version: 0.1.6
+Version: 0.1.7
 Summary: Parser to translate excel graphs to Plotly figures
 Author-email: "D. Sommers" <dsommers@viktor.ai>
 Maintainer-email: "D. Sommers" <dsommers@viktor.ai>
 License: MIT License
         
         Copyright (c) 2024 VIKTOR
```

### Comparing `excel_graph_parser-0.1.6/README.md` & `excel_graph_parser-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `excel_graph_parser-0.1.6/excel_graph_parser/graph_parser.py` & `excel_graph_parser-0.1.7/excel_graph_parser/graph_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         for index, row in enumerate(ws_output.iter_rows(min_row=2, max_col=4)):
             name = row[0].value
             unit = row[1].value if row[1].value else ""
             description = row[2].value
             if name:
                 outputs.append(
                     {"name": name, "unit": unit, "description": description, "key": f"output_{index}",
-                     "value": values[row[0].value]}
+                     "value": values[row[0].value], "type": str(type(values[row[0].value]))}
                 )
         return outputs
 
     def get_figures_from_excel_file(self) -> list:
         """Gets figures from the excel file as a list"""
 
         wb, _ = self.get_evaluated_spreadsheet()
@@ -235,18 +235,20 @@
             # Get the chart titles
             if chart.title:
                 chart_title = ''.join([title_element.t for title_element in chart.title.tx.rich.p[0].r])
             else:
                 chart_title = f"Untitled Chart {i}"
             clean_name = [s.lower() for s in chart_title.replace(" ", "_") if s.isalnum() or s == "_"]
             figure_name = "".join(clean_name)
+            figure_type = chart.tagname
             figure_list.append(
                 {
                     "name": chart_title,
-                    "concat_name": figure_name
+                    "concat_name": figure_name,
+                    "type": figure_type,
                 }
             )
 
         return figure_list
 
     @staticmethod
     def create_ploty_figure(chart_data: dict):
@@ -286,8 +288,8 @@
                 xaxis_title=chart_data["x_axis_title"],
                 yaxis_title=chart_data["y_axis_title"],
                 yaxis_tickformat=chart_data["series"][0]["values_value_format"],
                 xaxis_tickformat=chart_data["series"][0]["category_value_format"],
             )
 
         chart_data["fig"] = fig
-        return chart_data
+        return chart_data
```

### Comparing `excel_graph_parser-0.1.6/excel_graph_parser.egg-info/PKG-INFO` & `excel_graph_parser-0.1.7/excel_graph_parser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excel_graph_parser
-Version: 0.1.6
+Version: 0.1.7
 Summary: Parser to translate excel graphs to Plotly figures
 Author-email: "D. Sommers" <dsommers@viktor.ai>
 Maintainer-email: "D. Sommers" <dsommers@viktor.ai>
 License: MIT License
         
         Copyright (c) 2024 VIKTOR
```

### Comparing `excel_graph_parser-0.1.6/pyproject.toml` & `excel_graph_parser-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "excel_graph_parser"
-version = "0.1.6"
+version = "0.1.7"
 description = "Parser to translate excel graphs to Plotly figures"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 authors = [
     {name = "D. Sommers", email = "dsommers@viktor.ai" }
 ]
```

