# Comparing `tmp/ft2bt-0.1.1.tar.gz` & `tmp/ft2bt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ft2bt-0.1.1.tar", last modified: Mon Apr  1 16:52:27 2024, max compression
+gzip compressed data, was "ft2bt-0.1.2.tar", last modified: Tue Apr  2 07:01:20 2024, max compression
```

## Comparing `ft2bt-0.1.1.tar` & `ft2bt-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-04-01 16:52:27.378053 ft2bt-0.1.1/
--rw-rw-r--   0 tda       (1000) tda       (1000)    35148 2024-04-01 16:49:09.000000 ft2bt-0.1.1/LICENSE
--rw-r--r--   0 tda       (1000) tda       (1000)     4933 2024-04-01 16:52:27.378053 ft2bt-0.1.1/PKG-INFO
--rw-rw-r--   0 tda       (1000) tda       (1000)     4341 2024-04-01 16:49:09.000000 ft2bt-0.1.1/README.md
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-04-01 16:52:27.378053 ft2bt-0.1.1/ft2bt/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-01 16:49:09.000000 ft2bt-0.1.1/ft2bt/__init__.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-04-01 16:52:27.378053 ft2bt-0.1.1/ft2bt/scripts/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-01 16:49:09.000000 ft2bt-0.1.1/ft2bt/scripts/__init__.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-04-01 16:52:27.378053 ft2bt-0.1.1/ft2bt/scripts/behavior_trees/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-01 16:49:09.000000 ft2bt-0.1.1/ft2bt/scripts/behavior_trees/__init__.py
--rw-rw-r--   0 tda       (1000) tda       (1000)    11665 2024-04-01 16:49:58.000000 ft2bt-0.1.1/ft2bt/scripts/behavior_trees/behavior_tree.py
--rw-rw-r--   0 tda       (1000) tda       (1000)      313 2024-04-01 16:49:09.000000 ft2bt-0.1.1/ft2bt/scripts/behavior_trees/behavior_tree_node.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-04-01 16:52:27.378053 ft2bt-0.1.1/ft2bt/scripts/code_generator/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-01 16:49:09.000000 ft2bt-0.1.1/ft2bt/scripts/code_generator/__init__.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     9283 2024-04-01 16:49:09.000000 ft2bt-0.1.1/ft2bt/scripts/code_generator/code_generator.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     2316 2024-04-01 16:49:09.000000 ft2bt-0.1.1/ft2bt/scripts/code_generator/header_file.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     2891 2024-04-01 16:49:09.000000 ft2bt-0.1.1/ft2bt/scripts/code_generator/main_file.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     3417 2024-04-01 16:49:09.000000 ft2bt-0.1.1/ft2bt/scripts/code_generator/source_file.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-04-01 16:52:27.378053 ft2bt-0.1.1/ft2bt/scripts/fault_trees/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-01 16:49:09.000000 ft2bt-0.1.1/ft2bt/scripts/fault_trees/__init__.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     7623 2024-04-01 16:49:09.000000 ft2bt-0.1.1/ft2bt/scripts/fault_trees/xml_fta_parser.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     2243 2024-04-01 16:49:09.000000 ft2bt-0.1.1/ft2bt/scripts/ft2bt.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-04-01 16:52:27.378053 ft2bt-0.1.1/ft2bt.egg-info/
--rw-r--r--   0 tda       (1000) tda       (1000)     4933 2024-04-01 16:52:27.000000 ft2bt-0.1.1/ft2bt.egg-info/PKG-INFO
--rw-rw-r--   0 tda       (1000) tda       (1000)      707 2024-04-01 16:52:27.000000 ft2bt-0.1.1/ft2bt.egg-info/SOURCES.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)        1 2024-04-01 16:52:27.000000 ft2bt-0.1.1/ft2bt.egg-info/dependency_links.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)       51 2024-04-01 16:52:27.000000 ft2bt-0.1.1/ft2bt.egg-info/entry_points.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)       51 2024-04-01 16:52:27.000000 ft2bt-0.1.1/ft2bt.egg-info/requires.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)        6 2024-04-01 16:52:27.000000 ft2bt-0.1.1/ft2bt.egg-info/top_level.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)       38 2024-04-01 16:52:27.378053 ft2bt-0.1.1/setup.cfg
--rw-rw-r--   0 tda       (1000) tda       (1000)      966 2024-04-01 16:52:20.000000 ft2bt-0.1.1/setup.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-04-02 07:01:20.939796 ft2bt-0.1.2/
+-rw-rw-r--   0 tda       (1000) tda       (1000)    35148 2024-04-02 06:58:33.000000 ft2bt-0.1.2/LICENSE
+-rw-r--r--   0 tda       (1000) tda       (1000)     4604 2024-04-02 07:01:20.939796 ft2bt-0.1.2/PKG-INFO
+-rw-rw-r--   0 tda       (1000) tda       (1000)     4012 2024-04-02 06:58:33.000000 ft2bt-0.1.2/README.md
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-04-02 07:01:20.935799 ft2bt-0.1.2/ft2bt/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-02 06:58:33.000000 ft2bt-0.1.2/ft2bt/__init__.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-04-02 07:01:20.935799 ft2bt-0.1.2/ft2bt/scripts/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-02 06:58:33.000000 ft2bt-0.1.2/ft2bt/scripts/__init__.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-04-02 07:01:20.935799 ft2bt-0.1.2/ft2bt/scripts/behavior_trees/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-02 06:58:33.000000 ft2bt-0.1.2/ft2bt/scripts/behavior_trees/__init__.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)    11665 2024-04-02 06:58:33.000000 ft2bt-0.1.2/ft2bt/scripts/behavior_trees/behavior_tree.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)      313 2024-04-02 06:58:33.000000 ft2bt-0.1.2/ft2bt/scripts/behavior_trees/behavior_tree_node.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-04-02 07:01:20.939796 ft2bt-0.1.2/ft2bt/scripts/code_generator/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-02 06:58:33.000000 ft2bt-0.1.2/ft2bt/scripts/code_generator/__init__.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     9283 2024-04-02 06:58:33.000000 ft2bt-0.1.2/ft2bt/scripts/code_generator/code_generator.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     2316 2024-04-02 06:58:33.000000 ft2bt-0.1.2/ft2bt/scripts/code_generator/header_file.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     2891 2024-04-02 06:58:33.000000 ft2bt-0.1.2/ft2bt/scripts/code_generator/main_file.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     3417 2024-04-02 06:58:33.000000 ft2bt-0.1.2/ft2bt/scripts/code_generator/source_file.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-04-02 07:01:20.939796 ft2bt-0.1.2/ft2bt/scripts/fault_trees/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-02 06:58:33.000000 ft2bt-0.1.2/ft2bt/scripts/fault_trees/__init__.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     7623 2024-04-02 06:58:33.000000 ft2bt-0.1.2/ft2bt/scripts/fault_trees/xml_fta_parser.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     2553 2024-04-02 06:58:33.000000 ft2bt-0.1.2/ft2bt/scripts/ft2bt.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-04-02 07:01:20.939796 ft2bt-0.1.2/ft2bt.egg-info/
+-rw-r--r--   0 tda       (1000) tda       (1000)     4604 2024-04-02 07:01:20.000000 ft2bt-0.1.2/ft2bt.egg-info/PKG-INFO
+-rw-rw-r--   0 tda       (1000) tda       (1000)      707 2024-04-02 07:01:20.000000 ft2bt-0.1.2/ft2bt.egg-info/SOURCES.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)        1 2024-04-02 07:01:20.000000 ft2bt-0.1.2/ft2bt.egg-info/dependency_links.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)       51 2024-04-02 07:01:20.000000 ft2bt-0.1.2/ft2bt.egg-info/entry_points.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)       51 2024-04-02 07:01:20.000000 ft2bt-0.1.2/ft2bt.egg-info/requires.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)        6 2024-04-02 07:01:20.000000 ft2bt-0.1.2/ft2bt.egg-info/top_level.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)       38 2024-04-02 07:01:20.939796 ft2bt-0.1.2/setup.cfg
+-rw-rw-r--   0 tda       (1000) tda       (1000)      966 2024-04-02 07:01:05.000000 ft2bt-0.1.2/setup.py
```

### Comparing `ft2bt-0.1.1/LICENSE` & `ft2bt-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ft2bt-0.1.1/PKG-INFO` & `ft2bt-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ft2bt
-Version: 0.1.1
+Version: 0.1.2
 Summary: Automatic conversion from fault trees into behavior trees
 Home-page: https://github.com/cconejob/ft2bt
 Author: Carlos Conejo
 Author-email: carlos.conejo@upc.edu
 License: GNU GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -20,24 +20,18 @@
 
 ## Overview
 
 This project focuses on the conversion of fault trees, represented in draw.io diagram XML files, into behavior tree XML files compatible with the BehaviorTree.CPP library. It enables users to transform their fault tree diagrams into actionable behavior trees, facilitating integration with systems that utilize the BehaviorTree.CPP framework for managing complex behaviors.
 
 ## Installation
 
-1. Clone the repository to your local machine.
-
-2. Ensure you have Python installed.
-
-3. Install the required dependencies by running the following command in the project directory.
+Install with PyPI:
 
 ```bash
-git clone git@github.com:cconejob/trees.git
-cd trees
-pip install -r requirements.txt
+pip install ft2bt
 ```
 
 ## Usage
 
 The tool is designed to convert fault trees from draw.io diagram XML files into behavior tree XML files compatible with the BehaviorTree.CPP library. Here's how to use it:
 
 ### Preparing Your Fault Tree Diagram
@@ -62,29 +56,27 @@
 
 <p align="center">
   <img src="fault_trees/fta_example.png" alt="Fault Tree Example">
 </p>
 
 ### Running the Conversion Tool
 
-1. Ensure you have the required XML file from draw.io in the /fault_trees folder.
-2. Open a terminal or command prompt and navigate to the project directory.
-3. Run the conversion command:
-
-    ```bash
-    cd ft2bt/scripts
-    python3 ft2bt.py [-h] -f FTA_FILENAME [-v] [-c] [-r]
-    ```
+Run the conversion command:
+
+```bash
+ft2bt [-h] -f FTA_FILENAME [-v] [-c] [-r] [-o]
+```
 
 Where:
 
 * **-f**: (Required) Specifies the XML global filepath name of the draw.io diagram.
 * **-v**: (Optional) Automatically shows and saves the renders. Defaults to false.
 * **-c**: (Optional) Generate a cpp ROS node template for the behavior tree. Defaults to false.
 * **-r**: (Optional) Replaces current code if previously generated and -c is set to True.
+* **-o**: (Optional) Specifies the global folder path, where the behavior tree XML diagram is saved.
 
 ### Output Example: Behavior Tree Diagram
 
 Below is an example of the behavior tree diagrams generated from the fault tree. The XML file is loaded using [Groot](https://github.com/BehaviorTree/Groot):
 
 The order of the events is randomly selected in this version of the software. Future versions will sort the events by probability of occurrence.
```

### Comparing `ft2bt-0.1.1/README.md` & `ft2bt-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,24 +2,18 @@
 
 ## Overview
 
 This project focuses on the conversion of fault trees, represented in draw.io diagram XML files, into behavior tree XML files compatible with the BehaviorTree.CPP library. It enables users to transform their fault tree diagrams into actionable behavior trees, facilitating integration with systems that utilize the BehaviorTree.CPP framework for managing complex behaviors.
 
 ## Installation
 
-1. Clone the repository to your local machine.
-
-2. Ensure you have Python installed.
-
-3. Install the required dependencies by running the following command in the project directory.
+Install with PyPI:
 
 ```bash
-git clone git@github.com:cconejob/trees.git
-cd trees
-pip install -r requirements.txt
+pip install ft2bt
 ```
 
 ## Usage
 
 The tool is designed to convert fault trees from draw.io diagram XML files into behavior tree XML files compatible with the BehaviorTree.CPP library. Here's how to use it:
 
 ### Preparing Your Fault Tree Diagram
@@ -44,29 +38,27 @@
 
 <p align="center">
   <img src="fault_trees/fta_example.png" alt="Fault Tree Example">
 </p>
 
 ### Running the Conversion Tool
 
-1. Ensure you have the required XML file from draw.io in the /fault_trees folder.
-2. Open a terminal or command prompt and navigate to the project directory.
-3. Run the conversion command:
-
-    ```bash
-    cd ft2bt/scripts
-    python3 ft2bt.py [-h] -f FTA_FILENAME [-v] [-c] [-r]
-    ```
+Run the conversion command:
+
+```bash
+ft2bt [-h] -f FTA_FILENAME [-v] [-c] [-r] [-o]
+```
 
 Where:
 
 * **-f**: (Required) Specifies the XML global filepath name of the draw.io diagram.
 * **-v**: (Optional) Automatically shows and saves the renders. Defaults to false.
 * **-c**: (Optional) Generate a cpp ROS node template for the behavior tree. Defaults to false.
 * **-r**: (Optional) Replaces current code if previously generated and -c is set to True.
+* **-o**: (Optional) Specifies the global folder path, where the behavior tree XML diagram is saved.
 
 ### Output Example: Behavior Tree Diagram
 
 Below is an example of the behavior tree diagrams generated from the fault tree. The XML file is loaded using [Groot](https://github.com/BehaviorTree/Groot):
 
 The order of the events is randomly selected in this version of the software. Future versions will sort the events by probability of occurrence.
```

### Comparing `ft2bt-0.1.1/ft2bt/scripts/behavior_trees/behavior_tree.py` & `ft2bt-0.1.2/ft2bt/scripts/behavior_trees/behavior_tree.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.1.1/ft2bt/scripts/code_generator/code_generator.py` & `ft2bt-0.1.2/ft2bt/scripts/code_generator/code_generator.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.1.1/ft2bt/scripts/code_generator/header_file.py` & `ft2bt-0.1.2/ft2bt/scripts/code_generator/header_file.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.1.1/ft2bt/scripts/code_generator/main_file.py` & `ft2bt-0.1.2/ft2bt/scripts/code_generator/main_file.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.1.1/ft2bt/scripts/code_generator/source_file.py` & `ft2bt-0.1.2/ft2bt/scripts/code_generator/source_file.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.1.1/ft2bt/scripts/fault_trees/xml_fta_parser.py` & `ft2bt-0.1.2/ft2bt/scripts/fault_trees/xml_fta_parser.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.1.1/ft2bt/scripts/ft2bt.py` & `ft2bt-0.1.2/ft2bt/scripts/ft2bt.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     parser = argparse.ArgumentParser(description='Convert xml file from drawio to behavior tree xml file for Groot.')
     
     # Limit coordinates
     parser.add_argument('-f', '--fta_filepath', type=str, help="*.xml fault tree global path", required=True)
     parser.add_argument('-v', '--view', action='store_true', help="View the behavior tree renders?")
     parser.add_argument('-c', '--generate_cpp', action='store_true', help="Generate C++ code template?")
     parser.add_argument('-r', '--replace', action='store_true', help="Replace existing files?")
+    parser.add_argument('-o', '--output_folder', type=str, help="Output folder for the behavior trees.")
     args = parser.parse_args()
     
     # Get the path to the package
     module_path = Path(__file__).resolve()
     package_path = module_path.parent.parent.parent
     
     # Add the .xml extension if it is not present
@@ -27,19 +28,25 @@
         print(f'Added .xml extension to the file path: {args.fta_filepath}')
     
     # Generate the fault tree diagram from the XML file
     fta_filename = Path(args.fta_filepath).stem
     fta_parser = XMLFTAParser(xml_file=args.fta_filepath)
     fta_list = fta_parser.generate_fault_trees(plot=args.view)
 
-    # Generate the behavior tree diagram from every fault tree diagram
-    behavior_tree_folder = package_path / 'behavior_trees'
+    # Initialize the behavior tree and code generator objects
     prev_bt = BehaviorTree(name='prev')
     code_generator = CodeGenerator(replace=args.replace, filename=fta_filename.lower())
     
+    # Create the folder for the behavior trees
+    if args.output_folder:
+        behavior_tree_folder = args.output_folder
+    else:
+        behavior_tree_folder = package_path / 'behavior_trees'
+    
+    # Generate the behavior tree diagram from every fault tree diagram
     for fta in fta_list:
         bt = BehaviorTree(name=fta.name)
         bt.event_number = prev_bt.event_number
         bt.action_number = prev_bt.action_number
         bt.generate_from_fault_tree(fta)
         bt.generate_xml_file(folder_name=behavior_tree_folder, view=args.view)
```

### Comparing `ft2bt-0.1.1/ft2bt.egg-info/PKG-INFO` & `ft2bt-0.1.2/ft2bt.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ft2bt
-Version: 0.1.1
+Version: 0.1.2
 Summary: Automatic conversion from fault trees into behavior trees
 Home-page: https://github.com/cconejob/ft2bt
 Author: Carlos Conejo
 Author-email: carlos.conejo@upc.edu
 License: GNU GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -20,24 +20,18 @@
 
 ## Overview
 
 This project focuses on the conversion of fault trees, represented in draw.io diagram XML files, into behavior tree XML files compatible with the BehaviorTree.CPP library. It enables users to transform their fault tree diagrams into actionable behavior trees, facilitating integration with systems that utilize the BehaviorTree.CPP framework for managing complex behaviors.
 
 ## Installation
 
-1. Clone the repository to your local machine.
-
-2. Ensure you have Python installed.
-
-3. Install the required dependencies by running the following command in the project directory.
+Install with PyPI:
 
 ```bash
-git clone git@github.com:cconejob/trees.git
-cd trees
-pip install -r requirements.txt
+pip install ft2bt
 ```
 
 ## Usage
 
 The tool is designed to convert fault trees from draw.io diagram XML files into behavior tree XML files compatible with the BehaviorTree.CPP library. Here's how to use it:
 
 ### Preparing Your Fault Tree Diagram
@@ -62,29 +56,27 @@
 
 <p align="center">
   <img src="fault_trees/fta_example.png" alt="Fault Tree Example">
 </p>
 
 ### Running the Conversion Tool
 
-1. Ensure you have the required XML file from draw.io in the /fault_trees folder.
-2. Open a terminal or command prompt and navigate to the project directory.
-3. Run the conversion command:
-
-    ```bash
-    cd ft2bt/scripts
-    python3 ft2bt.py [-h] -f FTA_FILENAME [-v] [-c] [-r]
-    ```
+Run the conversion command:
+
+```bash
+ft2bt [-h] -f FTA_FILENAME [-v] [-c] [-r] [-o]
+```
 
 Where:
 
 * **-f**: (Required) Specifies the XML global filepath name of the draw.io diagram.
 * **-v**: (Optional) Automatically shows and saves the renders. Defaults to false.
 * **-c**: (Optional) Generate a cpp ROS node template for the behavior tree. Defaults to false.
 * **-r**: (Optional) Replaces current code if previously generated and -c is set to True.
+* **-o**: (Optional) Specifies the global folder path, where the behavior tree XML diagram is saved.
 
 ### Output Example: Behavior Tree Diagram
 
 Below is an example of the behavior tree diagrams generated from the fault tree. The XML file is loaded using [Groot](https://github.com/BehaviorTree/Groot):
 
 The order of the events is randomly selected in this version of the software. Future versions will sort the events by probability of occurrence.
```

### Comparing `ft2bt-0.1.1/ft2bt.egg-info/SOURCES.txt` & `ft2bt-0.1.2/ft2bt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ft2bt-0.1.1/setup.py` & `ft2bt-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your requirements.txt file
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='ft2bt',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     install_requires=required,  # Use the list from requirements.txt
     entry_points={
         'console_scripts': [
             'ft2bt=ft2bt.scripts.ft2bt:main',
         ],
     },
```

