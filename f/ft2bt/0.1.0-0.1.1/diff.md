# Comparing `tmp/ft2bt-0.1.0.tar.gz` & `tmp/ft2bt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ft2bt-0.1.0.tar", last modified: Mon Apr  1 15:40:35 2024, max compression
+gzip compressed data, was "ft2bt-0.1.1.tar", last modified: Mon Apr  1 16:52:27 2024, max compression
```

## Comparing `ft2bt-0.1.0.tar` & `ft2bt-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-04-01 15:40:35.955469 ft2bt-0.1.0/
--rw-rw-r--   0 tda       (1000) tda       (1000)    35148 2024-04-01 14:58:30.000000 ft2bt-0.1.0/LICENSE
--rw-r--r--   0 tda       (1000) tda       (1000)     4947 2024-04-01 15:40:35.955469 ft2bt-0.1.0/PKG-INFO
--rw-rw-r--   0 tda       (1000) tda       (1000)     4355 2024-04-01 15:02:27.000000 ft2bt-0.1.0/README.md
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-04-01 15:40:35.955469 ft2bt-0.1.0/ft2bt/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-01 14:58:30.000000 ft2bt-0.1.0/ft2bt/__init__.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-04-01 15:40:35.955469 ft2bt-0.1.0/ft2bt/scripts/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-01 14:58:30.000000 ft2bt-0.1.0/ft2bt/scripts/__init__.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-04-01 15:40:35.955469 ft2bt-0.1.0/ft2bt/scripts/behavior_trees/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-01 14:58:30.000000 ft2bt-0.1.0/ft2bt/scripts/behavior_trees/__init__.py
--rw-rw-r--   0 tda       (1000) tda       (1000)    11595 2024-04-01 14:58:30.000000 ft2bt-0.1.0/ft2bt/scripts/behavior_trees/behavior_tree.py
--rw-rw-r--   0 tda       (1000) tda       (1000)      313 2024-04-01 14:58:30.000000 ft2bt-0.1.0/ft2bt/scripts/behavior_trees/behavior_tree_node.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-04-01 15:40:35.955469 ft2bt-0.1.0/ft2bt/scripts/code_generator/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-01 14:58:30.000000 ft2bt-0.1.0/ft2bt/scripts/code_generator/__init__.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     9325 2024-04-01 14:58:30.000000 ft2bt-0.1.0/ft2bt/scripts/code_generator/code_generator.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     2316 2024-04-01 14:58:30.000000 ft2bt-0.1.0/ft2bt/scripts/code_generator/header_file.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     2891 2024-04-01 14:58:30.000000 ft2bt-0.1.0/ft2bt/scripts/code_generator/main_file.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     3417 2024-04-01 14:58:30.000000 ft2bt-0.1.0/ft2bt/scripts/code_generator/source_file.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-04-01 15:40:35.955469 ft2bt-0.1.0/ft2bt/scripts/fault_trees/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-01 14:58:30.000000 ft2bt-0.1.0/ft2bt/scripts/fault_trees/__init__.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     7623 2024-04-01 14:58:30.000000 ft2bt-0.1.0/ft2bt/scripts/fault_trees/xml_fta_parser.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     2201 2024-04-01 14:58:30.000000 ft2bt-0.1.0/ft2bt/scripts/ft2bt.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-04-01 15:40:35.955469 ft2bt-0.1.0/ft2bt.egg-info/
--rw-r--r--   0 tda       (1000) tda       (1000)     4947 2024-04-01 15:40:35.000000 ft2bt-0.1.0/ft2bt.egg-info/PKG-INFO
--rw-rw-r--   0 tda       (1000) tda       (1000)      707 2024-04-01 15:40:35.000000 ft2bt-0.1.0/ft2bt.egg-info/SOURCES.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)        1 2024-04-01 15:40:35.000000 ft2bt-0.1.0/ft2bt.egg-info/dependency_links.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)       51 2024-04-01 15:40:35.000000 ft2bt-0.1.0/ft2bt.egg-info/entry_points.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)       51 2024-04-01 15:40:35.000000 ft2bt-0.1.0/ft2bt.egg-info/requires.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)        6 2024-04-01 15:40:35.000000 ft2bt-0.1.0/ft2bt.egg-info/top_level.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)       38 2024-04-01 15:40:35.955469 ft2bt-0.1.0/setup.cfg
--rw-rw-r--   0 tda       (1000) tda       (1000)      966 2024-04-01 15:40:31.000000 ft2bt-0.1.0/setup.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-04-01 16:52:27.378053 ft2bt-0.1.1/
+-rw-rw-r--   0 tda       (1000) tda       (1000)    35148 2024-04-01 16:49:09.000000 ft2bt-0.1.1/LICENSE
+-rw-r--r--   0 tda       (1000) tda       (1000)     4933 2024-04-01 16:52:27.378053 ft2bt-0.1.1/PKG-INFO
+-rw-rw-r--   0 tda       (1000) tda       (1000)     4341 2024-04-01 16:49:09.000000 ft2bt-0.1.1/README.md
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-04-01 16:52:27.378053 ft2bt-0.1.1/ft2bt/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-01 16:49:09.000000 ft2bt-0.1.1/ft2bt/__init__.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-04-01 16:52:27.378053 ft2bt-0.1.1/ft2bt/scripts/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-01 16:49:09.000000 ft2bt-0.1.1/ft2bt/scripts/__init__.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-04-01 16:52:27.378053 ft2bt-0.1.1/ft2bt/scripts/behavior_trees/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-01 16:49:09.000000 ft2bt-0.1.1/ft2bt/scripts/behavior_trees/__init__.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)    11665 2024-04-01 16:49:58.000000 ft2bt-0.1.1/ft2bt/scripts/behavior_trees/behavior_tree.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)      313 2024-04-01 16:49:09.000000 ft2bt-0.1.1/ft2bt/scripts/behavior_trees/behavior_tree_node.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-04-01 16:52:27.378053 ft2bt-0.1.1/ft2bt/scripts/code_generator/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-01 16:49:09.000000 ft2bt-0.1.1/ft2bt/scripts/code_generator/__init__.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     9283 2024-04-01 16:49:09.000000 ft2bt-0.1.1/ft2bt/scripts/code_generator/code_generator.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     2316 2024-04-01 16:49:09.000000 ft2bt-0.1.1/ft2bt/scripts/code_generator/header_file.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     2891 2024-04-01 16:49:09.000000 ft2bt-0.1.1/ft2bt/scripts/code_generator/main_file.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     3417 2024-04-01 16:49:09.000000 ft2bt-0.1.1/ft2bt/scripts/code_generator/source_file.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-04-01 16:52:27.378053 ft2bt-0.1.1/ft2bt/scripts/fault_trees/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-01 16:49:09.000000 ft2bt-0.1.1/ft2bt/scripts/fault_trees/__init__.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     7623 2024-04-01 16:49:09.000000 ft2bt-0.1.1/ft2bt/scripts/fault_trees/xml_fta_parser.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     2243 2024-04-01 16:49:09.000000 ft2bt-0.1.1/ft2bt/scripts/ft2bt.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-04-01 16:52:27.378053 ft2bt-0.1.1/ft2bt.egg-info/
+-rw-r--r--   0 tda       (1000) tda       (1000)     4933 2024-04-01 16:52:27.000000 ft2bt-0.1.1/ft2bt.egg-info/PKG-INFO
+-rw-rw-r--   0 tda       (1000) tda       (1000)      707 2024-04-01 16:52:27.000000 ft2bt-0.1.1/ft2bt.egg-info/SOURCES.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)        1 2024-04-01 16:52:27.000000 ft2bt-0.1.1/ft2bt.egg-info/dependency_links.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)       51 2024-04-01 16:52:27.000000 ft2bt-0.1.1/ft2bt.egg-info/entry_points.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)       51 2024-04-01 16:52:27.000000 ft2bt-0.1.1/ft2bt.egg-info/requires.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)        6 2024-04-01 16:52:27.000000 ft2bt-0.1.1/ft2bt.egg-info/top_level.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)       38 2024-04-01 16:52:27.378053 ft2bt-0.1.1/setup.cfg
+-rw-rw-r--   0 tda       (1000) tda       (1000)      966 2024-04-01 16:52:20.000000 ft2bt-0.1.1/setup.py
```

### Comparing `ft2bt-0.1.0/LICENSE` & `ft2bt-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ft2bt-0.1.0/PKG-INFO` & `ft2bt-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ft2bt
-Version: 0.1.0
+Version: 0.1.1
 Summary: Automatic conversion from fault trees into behavior trees
 Home-page: https://github.com/cconejob/ft2bt
 Author: Carlos Conejo
 Author-email: carlos.conejo@upc.edu
 License: GNU GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -27,16 +27,16 @@
 1. Clone the repository to your local machine.
 
 2. Ensure you have Python installed.
 
 3. Install the required dependencies by running the following command in the project directory.
 
 ```bash
-git git@github.com:cconejob/ft2bt_converter.git
-cd ft2bt_converter
+git clone git@github.com:cconejob/trees.git
+cd trees
 pip install -r requirements.txt
 ```
 
 ## Usage
 
 The tool is designed to convert fault trees from draw.io diagram XML files into behavior tree XML files compatible with the BehaviorTree.CPP library. Here's how to use it:
```

### Comparing `ft2bt-0.1.0/README.md` & `ft2bt-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 1. Clone the repository to your local machine.
 
 2. Ensure you have Python installed.
 
 3. Install the required dependencies by running the following command in the project directory.
 
 ```bash
-git git@github.com:cconejob/ft2bt_converter.git
-cd ft2bt_converter
+git clone git@github.com:cconejob/trees.git
+cd trees
 pip install -r requirements.txt
 ```
 
 ## Usage
 
 The tool is designed to convert fault trees from draw.io diagram XML files into behavior tree XML files compatible with the BehaviorTree.CPP library. Here's how to use it:
```

### Comparing `ft2bt-0.1.0/ft2bt/scripts/behavior_trees/behavior_tree.py` & `ft2bt-0.1.1/ft2bt/scripts/behavior_trees/behavior_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import graphviz
 import os
 import xml.etree.ElementTree as ET
 import xml.dom.minidom as minidom
 
-from behavior_trees.behavior_tree_node import BehaviorTreeNode
+from .behavior_tree_node import BehaviorTreeNode
 
 
 class BehaviorTree:
     """
     Behavior tree class.
     Each behavior tree has a dictionary of nodes and a list of edges.
     
@@ -276,11 +276,13 @@
         pretty_xml_str = xml_parsed.toprettyxml(indent="  ")
 
         # Write to file
         self.xml_file_path = os.path.join(folder_name, f'BT_{self.name}.xml')
         with open(self.xml_file_path, 'w') as file:
             file.write(pretty_xml_str)
             
+        print(f'Behavior tree XML file saved to {self.xml_file_path}')
+            
         # Render and view the tree graphically using Graphviz if requested
         pdf_file_path = os.path.join(folder_name, 'render', f'BT_{self.name}')
         if view:
             self.render_graphviz_tree(filename=pdf_file_path, view=view)
```

### Comparing `ft2bt-0.1.0/ft2bt/scripts/code_generator/code_generator.py` & `ft2bt-0.1.1/ft2bt/scripts/code_generator/code_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import xml.etree.ElementTree as ET
 from pathlib import Path
 
-from code_generator.header_file import HeaderFile
-from code_generator.source_file import SourceFile
-from code_generator.main_file import MainFile
+from .header_file import HeaderFile
+from .source_file import SourceFile
+from .main_file import MainFile
 
 
 class CodeGenerator:
     def __init__(self, replace=False, filename='fault_tree'):
         """
         Generate the header and source files for the actions and conditions.
```

### Comparing `ft2bt-0.1.0/ft2bt/scripts/code_generator/header_file.py` & `ft2bt-0.1.1/ft2bt/scripts/code_generator/header_file.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.1.0/ft2bt/scripts/code_generator/main_file.py` & `ft2bt-0.1.1/ft2bt/scripts/code_generator/main_file.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.1.0/ft2bt/scripts/code_generator/source_file.py` & `ft2bt-0.1.1/ft2bt/scripts/code_generator/source_file.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.1.0/ft2bt/scripts/fault_trees/xml_fta_parser.py` & `ft2bt-0.1.1/ft2bt/scripts/fault_trees/xml_fta_parser.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.1.0/ft2bt/scripts/ft2bt.py` & `ft2bt-0.1.1/ft2bt/scripts/ft2bt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse
 from pathlib import Path
 
-from fault_trees.xml_fta_parser import XMLFTAParser
-from behavior_trees.behavior_tree import BehaviorTree
-from code_generator.code_generator import CodeGenerator
+from ft2bt.scripts.fault_trees.xml_fta_parser import XMLFTAParser
+from ft2bt.scripts.behavior_trees.behavior_tree import BehaviorTree
+from ft2bt.scripts.code_generator.code_generator import CodeGenerator
 
 
 def main():  
     parser = argparse.ArgumentParser(description='Convert xml file from drawio to behavior tree xml file for Groot.')
     
     # Limit coordinates
     parser.add_argument('-f', '--fta_filepath', type=str, help="*.xml fault tree global path", required=True)
```

### Comparing `ft2bt-0.1.0/ft2bt.egg-info/PKG-INFO` & `ft2bt-0.1.1/ft2bt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ft2bt
-Version: 0.1.0
+Version: 0.1.1
 Summary: Automatic conversion from fault trees into behavior trees
 Home-page: https://github.com/cconejob/ft2bt
 Author: Carlos Conejo
 Author-email: carlos.conejo@upc.edu
 License: GNU GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -27,16 +27,16 @@
 1. Clone the repository to your local machine.
 
 2. Ensure you have Python installed.
 
 3. Install the required dependencies by running the following command in the project directory.
 
 ```bash
-git git@github.com:cconejob/ft2bt_converter.git
-cd ft2bt_converter
+git clone git@github.com:cconejob/trees.git
+cd trees
 pip install -r requirements.txt
 ```
 
 ## Usage
 
 The tool is designed to convert fault trees from draw.io diagram XML files into behavior tree XML files compatible with the BehaviorTree.CPP library. Here's how to use it:
```

### Comparing `ft2bt-0.1.0/ft2bt.egg-info/SOURCES.txt` & `ft2bt-0.1.1/ft2bt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ft2bt-0.1.0/setup.py` & `ft2bt-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your requirements.txt file
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='ft2bt',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
     install_requires=required,  # Use the list from requirements.txt
     entry_points={
         'console_scripts': [
             'ft2bt=ft2bt.scripts.ft2bt:main',
         ],
     },
```

