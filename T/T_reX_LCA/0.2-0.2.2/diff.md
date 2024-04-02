# Comparing `tmp/t_rex_lca-0.2.tar.gz` & `tmp/t_rex_lca-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t_rex_lca-0.2.tar", max compression
+gzip compressed data, was "t_rex_lca-0.2.2.tar", max compression
```

## Comparing `t_rex_lca-0.2.tar` & `t_rex_lca-0.2.2.tar`

### file list

```diff
@@ -1,58 +1,27 @@
--rw-r--r--   0        0        0     7047 2023-12-26 13:36:23.904641 t_rex_lca-0.2/LICENSE
--rw-r--r--   0        0        0    11821 2024-03-08 07:51:08.819236 t_rex_lca-0.2/README.md
--rw-r--r--   0        0        0    95085 2017-10-06 19:52:45.000000 t_rex_lca-0.2/misc/moo.mp3
--rw-r--r--   0        0        0    65828 2023-12-08 17:34:23.457275 t_rex_lca-0.2/misc/success.mp3
--rw-r--r--   0        0        0     2145 2024-03-08 08:45:15.139456 t_rex_lca-0.2/pyproject.toml
--rw-r--r--   0        0        0     2795 2024-03-07 17:14:33.667170 t_rex_lca-0.2/src/T-reX/CustomConfig.py
--rw-r--r--   0        0        0     6890 2024-03-08 08:36:55.964150 t_rex_lca-0.2/src/T-reX/ExchangeEditor.py
--rw-r--r--   0        0        0     3245 2023-12-30 09:53:28.908751 t_rex_lca-0.2/src/T-reX/ExplodeDatabase.py
--rw-r--r--   0        0        0     9780 2024-01-16 14:42:03.165105 t_rex_lca-0.2/src/T-reX/FutureScenarios.py
--rw-r--r--   0        0        0     6043 2024-03-07 17:38:18.229072 t_rex_lca-0.2/src/T-reX/MakeCustomDatabase.py
--rw-r--r--   0        0        0     3719 2024-03-07 17:38:19.677094 t_rex_lca-0.2/src/T-reX/MethodEditor.py
--rw-r--r--   0        0        0     7604 2024-03-07 17:34:57.886005 t_rex_lca-0.2/src/T-reX/SearchMaterial.py
--rw-r--r--   0        0        0     5209 2024-03-07 17:38:21.973129 t_rex_lca-0.2/src/T-reX/SearchWaste.py
--rw-r--r--   0        0        0     4766 2024-03-07 17:29:17.076697 t_rex_lca-0.2/src/T-reX/VerifyDatabase.py
--rw-r--r--   0        0        0     1046 2024-03-07 17:14:33.671170 t_rex_lca-0.2/src/T-reX/__init__.py
--rw-r--r--   0        0        0     2195 2023-12-29 17:18:32.806404 t_rex_lca-0.2/src/T-reX/__pycache__/CustomConfig.cpython-310.pyc
--rw-r--r--   0        0        0     1865 2023-12-28 09:13:03.483995 t_rex_lca-0.2/src/T-reX/__pycache__/CustomConfig.cpython-311.pyc
--rw-r--r--   0        0        0     4907 2024-03-07 20:15:39.536342 t_rex_lca-0.2/src/T-reX/__pycache__/ExchangeEditor.cpython-310.pyc
--rw-r--r--   0        0        0     8855 2023-12-30 09:54:01.421244 t_rex_lca-0.2/src/T-reX/__pycache__/ExchangeEditor.cpython-311.pyc
--rw-r--r--   0        0        0     2742 2024-01-15 22:00:24.452644 t_rex_lca-0.2/src/T-reX/__pycache__/ExplodeDatabase.cpython-310.pyc
--rw-r--r--   0        0        0     4643 2023-12-30 09:54:01.421244 t_rex_lca-0.2/src/T-reX/__pycache__/ExplodeDatabase.cpython-311.pyc
--rw-r--r--   0        0        0     7146 2024-01-16 14:42:43.061703 t_rex_lca-0.2/src/T-reX/__pycache__/FutureScenarios.cpython-310.pyc
--rw-r--r--   0        0        0    12585 2024-01-16 18:33:24.505581 t_rex_lca-0.2/src/T-reX/__pycache__/FutureScenarios.cpython-311.pyc
--rw-r--r--   0        0        0     4898 2024-03-07 20:15:50.432504 t_rex_lca-0.2/src/T-reX/__pycache__/MakeCustomDatabase.cpython-310.pyc
--rw-r--r--   0        0        0     8336 2023-12-30 10:00:28.947113 t_rex_lca-0.2/src/T-reX/__pycache__/MakeCustomDatabase.cpython-311.pyc
--rw-r--r--   0        0        0     3473 2024-03-07 20:15:50.432504 t_rex_lca-0.2/src/T-reX/__pycache__/MethodEditor.cpython-310.pyc
--rw-r--r--   0        0        0     5775 2024-01-16 14:22:21.567313 t_rex_lca-0.2/src/T-reX/__pycache__/MethodEditor.cpython-311.pyc
--rw-r--r--   0        0        0     5853 2024-03-07 20:15:50.436504 t_rex_lca-0.2/src/T-reX/__pycache__/SearchMaterial.cpython-310.pyc
--rw-r--r--   0        0        0     9974 2024-01-16 06:45:52.044383 t_rex_lca-0.2/src/T-reX/__pycache__/SearchMaterial.cpython-311.pyc
--rw-r--r--   0        0        0     4602 2024-03-07 20:15:50.436504 t_rex_lca-0.2/src/T-reX/__pycache__/SearchWaste.cpython-310.pyc
--rw-r--r--   0        0        0     7996 2024-01-16 14:22:21.567313 t_rex_lca-0.2/src/T-reX/__pycache__/SearchWaste.cpython-311.pyc
--rw-r--r--   0        0        0     3676 2024-03-07 20:15:50.436504 t_rex_lca-0.2/src/T-reX/__pycache__/VerifyDatabase.cpython-310.pyc
--rw-r--r--   0        0        0     6221 2023-12-30 10:00:28.947113 t_rex_lca-0.2/src/T-reX/__pycache__/VerifyDatabase.cpython-311.pyc
--rw-r--r--   0        0        0      933 2023-12-29 17:13:53.830174 t_rex_lca-0.2/src/T-reX/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1308 2023-12-26 17:32:55.986996 t_rex_lca-0.2/src/T-reX/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    10654 2023-12-29 17:07:22.148265 t_rex_lca-0.2/src/T-reX/__pycache__/main.cpython-310.pyc
--rw-r--r--   0        0        0    18312 2023-12-29 13:18:33.619561 t_rex_lca-0.2/src/T-reX/__pycache__/main.cpython-311.pyc
--rw-r--r--   0        0        0      833 2024-03-07 17:34:57.898005 t_rex_lca-0.2/src/T-reX/config/__init__.py
--rw-r--r--   0        0        0      736 2024-03-07 20:15:50.404503 t_rex_lca-0.2/src/T-reX/config/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1007 2023-12-30 09:54:01.429244 t_rex_lca-0.2/src/T-reX/config/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3333 2024-03-07 20:15:50.432504 t_rex_lca-0.2/src/T-reX/config/__pycache__/queries_materials.cpython-310.pyc
--rw-r--r--   0        0        0     3308 2024-01-16 12:52:40.318002 t_rex_lca-0.2/src/T-reX/config/__pycache__/queries_materials.cpython-311.pyc
--rw-r--r--   0        0        0     2526 2024-03-07 20:15:50.432504 t_rex_lca-0.2/src/T-reX/config/__pycache__/queries_waste.cpython-310.pyc
--rw-r--r--   0        0        0     3756 2024-01-16 18:33:24.509581 t_rex_lca-0.2/src/T-reX/config/__pycache__/queries_waste.cpython-311.pyc
--rw-r--r--   0        0        0     3610 2024-03-07 20:15:50.404503 t_rex_lca-0.2/src/T-reX/config/__pycache__/user_settings.cpython-310.pyc
--rw-r--r--   0        0        0     5105 2024-01-16 18:33:24.509581 t_rex_lca-0.2/src/T-reX/config/__pycache__/user_settings.cpython-311.pyc
--rw-r--r--   0        0        0     3653 2024-03-07 17:14:33.691170 t_rex_lca-0.2/src/T-reX/config/queries_materials.py
--rw-r--r--   0        0        0     4116 2024-03-07 17:34:57.890005 t_rex_lca-0.2/src/T-reX/config/queries_waste.py
--rw-r--r--   0        0        0     7409 2024-03-07 20:14:27.839280 t_rex_lca-0.2/src/T-reX/config/user_settings.py
--rw-r--r--   0        0        0    12783 2024-03-07 17:34:57.886005 t_rex_lca-0.2/src/T-reX/main.py
--rw-r--r--   0        0        0      833 2024-03-07 17:34:57.870005 t_rex_lca-0.2/src/config_backup/__init__.py
--rw-r--r--   0        0        0     3565 2024-03-07 17:14:33.651170 t_rex_lca-0.2/src/config_backup/queries_materials.py
--rw-r--r--   0        0        0     4141 2024-03-07 17:34:57.862005 t_rex_lca-0.2/src/config_backup/queries_waste.py
--rw-r--r--   0        0        0        0 2023-12-29 17:12:50.917220 t_rex_lca-0.2/src/config_backup/test
--rw-r--r--   0        0        0     7472 2024-03-07 17:38:15.145025 t_rex_lca-0.2/src/config_backup/user_settings.py
--rw-r--r--   0        0        0      836 2024-03-07 17:34:57.898005 t_rex_lca-0.2/tests/test-import.py
--rw-r--r--   0        0        0      247 2024-03-08 08:39:53.678748 t_rex_lca-0.2/tests/test-verify.py
--rw-r--r--   0        0        0    13052 1970-01-01 00:00:00.000000 t_rex_lca-0.2/PKG-INFO
+-rw-r--r--   0        0        0     7047 2024-04-01 17:38:22.144387 t_rex_lca-0.2.2/LICENSE
+-rw-r--r--   0        0        0    12629 2024-04-01 17:38:22.144387 t_rex_lca-0.2.2/README.md
+-rw-r--r--   0        0        0    95085 2024-04-01 17:38:25.216488 t_rex_lca-0.2.2/misc/moo.mp3
+-rw-r--r--   0        0        0    65828 2024-04-01 17:38:25.216488 t_rex_lca-0.2.2/misc/success.mp3
+-rw-r--r--   0        0        0     1277 2024-04-02 10:21:25.741120 t_rex_lca-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2795 2024-04-01 17:38:25.216488 t_rex_lca-0.2.2/src/T-reX/CustomConfig.py
+-rw-r--r--   0        0        0     6889 2024-04-02 10:35:20.765592 t_rex_lca-0.2.2/src/T-reX/ExchangeEditor.py
+-rw-r--r--   0        0        0     3245 2024-04-01 17:38:25.216488 t_rex_lca-0.2.2/src/T-reX/ExplodeDatabase.py
+-rw-r--r--   0        0        0    10187 2024-04-01 17:38:25.216488 t_rex_lca-0.2.2/src/T-reX/FutureScenarios.py
+-rw-r--r--   0        0        0     6043 2024-04-01 17:38:25.216488 t_rex_lca-0.2.2/src/T-reX/MakeCustomDatabase.py
+-rw-r--r--   0        0        0     3719 2024-04-01 17:38:25.216488 t_rex_lca-0.2.2/src/T-reX/MethodEditor.py
+-rw-r--r--   0        0        0     7604 2024-04-01 17:38:25.216488 t_rex_lca-0.2.2/src/T-reX/SearchMaterial.py
+-rw-r--r--   0        0        0     5209 2024-04-01 17:38:25.216488 t_rex_lca-0.2.2/src/T-reX/SearchWaste.py
+-rw-r--r--   0        0        0     4766 2024-04-01 17:38:25.216488 t_rex_lca-0.2.2/src/T-reX/VerifyDatabase.py
+-rw-r--r--   0        0        0     1046 2024-04-01 17:38:25.216488 t_rex_lca-0.2.2/src/T-reX/__init__.py
+-rw-r--r--   0        0        0      833 2024-04-01 17:38:25.216488 t_rex_lca-0.2.2/src/T-reX/config/__init__.py
+-rw-r--r--   0        0        0     3653 2024-04-01 17:38:25.216488 t_rex_lca-0.2.2/src/T-reX/config/queries_materials.py
+-rw-r--r--   0        0        0     4125 2024-04-01 17:38:25.216488 t_rex_lca-0.2.2/src/T-reX/config/queries_waste.py
+-rw-r--r--   0        0        0     7412 2024-04-01 17:38:25.216488 t_rex_lca-0.2.2/src/T-reX/config/user_settings.py
+-rw-r--r--   0        0        0      833 2024-04-01 17:38:25.216488 t_rex_lca-0.2.2/src/T-reX/config_backup/__init__.py
+-rw-r--r--   0        0        0     3653 2024-04-01 17:38:25.216488 t_rex_lca-0.2.2/src/T-reX/config_backup/queries_materials.py
+-rw-r--r--   0        0        0     4125 2024-04-01 17:38:25.216488 t_rex_lca-0.2.2/src/T-reX/config_backup/queries_waste.py
+-rw-r--r--   0        0        0     7411 2024-04-01 17:38:25.216488 t_rex_lca-0.2.2/src/T-reX/config_backup/user_settings.py
+-rw-r--r--   0        0        0    13287 2024-04-01 17:38:25.216488 t_rex_lca-0.2.2/src/T-reX/main.py
+-rw-r--r--   0        0        0      836 2024-04-01 17:38:25.216488 t_rex_lca-0.2.2/tests/test-import.py
+-rw-r--r--   0        0        0      247 2024-04-01 17:38:25.216488 t_rex_lca-0.2.2/tests/test-verify.py
+-rw-r--r--   0        0        0    13710 1970-01-01 00:00:00.000000 t_rex_lca-0.2.2/PKG-INFO
```

### Comparing `t_rex_lca-0.2/LICENSE` & `t_rex_lca-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `t_rex_lca-0.2/README.md` & `t_rex_lca-0.2.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,40 @@
-# T-reX (formerly "WasteAndMaterialFootprint)
+# T-reX: waste and material footprinting in LCA
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10431181.svg)](https://doi.org/10.5281/zenodo.10431180)
 
-A program for Life Cycle Assessment (LCA) calculations of supply chain waste and material footprints.
+Formerly known as "WasteAndMaterialFootprint"
 
-Soon to be a paper, hopefully. The manuscript has its own github repo [here](https://github.com/Stew-McD/T-reX_publication)
+**T** stands for *tool* and **reX** for *the circular economy strategies reduce, reuse, recycle, etc.* 
+
+A python program for Life Cycle Assessment (LCA) calculations of supply chain waste and material footprints in current and prospective databases.
+
+Built as an extension to the [brightway LCA ecosystem](https://brightway.dev/), using [premise](https://github.com/polca/premise) for the generation of future scenario databases and [wurst](https://github.com/polca/wurst) for database expansion. 
+
+Soon to be a paper, hopefully. The manuscript has its own github repo [here](https://github.com/Stew-McD/T-reX_Publication). Reviews and comments are very welcome.
+
+Email: T-reX@scmcd.ch
 
 ## Documentation
 
 The documentation is available as a [website](https://T-reX.readthedocs.io/en/latest/). Also, as a  [pdf](https://T-reX.readthedocs.io/_/downloads/en/latest/pdf/).
 
-The documentation is still under development, but the code is well documented and there is a full API reference.
+The documentation is still under development, but the code is well commented and there is a full API reference.
 
 The following readme provides a brief introduction to the program, how to install it, and how to use it.
 
 See the example output [here](examples/package_test/example-output.pdf)
 
 ## Contents
 
-- [T-reX (formerly "WasteAndMaterialFootprint)](#t-rex-formerly-wasteandmaterialfootprint)
+- [T-reX: waste and material footprinting in LCA](#t-rex-waste-and-material-footprinting-in-lca)
   - [Documentation](#documentation)
   - [Contents](#contents)
+  - [Visual overview](#visual-overview)
+    - [Generalised and computational flowcharts](#generalised-and-computational-flowcharts)
   - [Installation](#installation)
     - [Dependencies](#dependencies)
     - [Installation instructions](#installation-instructions)
   - [Usage](#usage)
     - [Command line](#command-line)
     - [Python module](#python-module)
   - [Configuration](#configuration)
@@ -41,14 +51,20 @@
       - [Usage Considerations](#usage-considerations)
         - [Example Tuples](#example-tuples)
     - [Examples](#examples)
     - [Contributing](#contributing)
     - [License](#license)
     - [Citation](#citation)
 
+## Visual overview
+
+### Generalised and computational flowcharts
+
+<img src="docs/source/_static/T-reX_flowchart_combined.png" alt="T-reX flowcharts" width="500">
+
 ## Installation
 
 ### Dependencies
 
 The program is written in Python and the required packages are listed in the `requirements.txt` file. These should be installed automatically when installing the program.
 
 The main dependencies are:
@@ -95,15 +111,15 @@
   ```bash
   pip install -r requirements.txt
   ```
 
 Another option: the program can be installed using pip:
 
   ```bash
-  pip install T-reX
+  pip install T_reX_LCA
   ```
 
 Or, if you want to install the latest version from GitHub:
 
   ```bash
   pip install git+https://github.com/Stew-McD/T-reX.git
   ```
@@ -129,43 +145,43 @@
   ```
 
 ### Python module
 
 The program can be imported as a Python module:
 
   ```python
-      import T-reX as T-reX
-      T-reX.run()
+      import T_reX_LCA as TreX
+      TreX.run()
   ```
 
 ## Configuration
 
 You can find the configuration files in the `config` folder (`src/T-reX/config`). Or if you install it with pip, you can find the config folder in the `site-packages/T-reX/config` folder of your Python venv installation.
 
 If you have installed via pip, or want to have things separate, you can create a new folder somewhere and then run some built-in functions to create and reload the config files.
 
   ```python
-      import T-reX as T-reX
-      T-reX.create_config()
+      import T_reX_LCA as TreX
+      TreX.create_config()
   ```
 
 This will create a folder `config` in the current working directory containing the default configuration files (see below).
 
 You can then edit these files with some kind of text editor, and run:
 
   ```python
-      T-reX.reload_config()
+      TreX.reload_config()
   ```
 
 Note that you will need to close the Python session and start a new one to reload the config files.
 
 If you want to revert to the default config files, you can run:
 
   ```python
-      T-reX.reset_config()
+      TreX.reset_config()
   ```
 
 And then close and restart the Python session.
 
 If you are running the program as an editable package, you can edit the config files directly in the `src/T-reX/config` folder.
 
 Details of the configuration files are given below.
@@ -187,15 +203,15 @@
       # Choose whether to use T-reX to edit the databases (you could also turn this off and just use the package as an easy way to make a set of future scenario databases)
       use_T_reX = True
 
       # Choose the names of the projects to use
       project_premise_base = "default"
       project_premise = "SSP-cutoff"
       project_base = project_premise
-      project_T_reX = f"T_reXootprint-{project_base}"
+      project_T_reX = f"T-reX-{project_base}"
 
       # Choose the name of the database to use (needed for premise only, the T-reX tool will run all databases except the biospheres)
       database_name = "ecoinvent-3.9.1-cutoff"
 
       # if you want to use a fresh project
       delete_existing_premise_project = False
       delete_existing_T_reX_project = False
@@ -292,14 +308,14 @@
 
 Contributions are very welcome! Test the code, report bugs, suggest features, etc. If you want to contribute code, please fork the repo and make a pull request.
 
 See the [CONTRIBUTING.md](CONTRIBUTING.md) file for more details.
 
 ### License
 
-T-reX by Stewart Charles McDowall is marked with CC0 1.0 Universal, do whatever you want with it - see the [LICENSE](LICENSE) file for details
+T-reX by Stewart Charles McDowall is marked with CC0 1.0 Universal, do whatever you want with it. - see the [LICENSE](LICENSE) file for details
 
 ### Citation
 
 If you use this code, please cite it as described in the [CITATION.cff](CITATION.cff) file (see the sidebar on the right).
 
 When the paper is published, a citation for that will be added to the CITATION file.
```

### Comparing `t_rex_lca-0.2/misc/moo.mp3` & `t_rex_lca-0.2.2/misc/moo.mp3`

 * *Files identical despite different names*

### Comparing `t_rex_lca-0.2/misc/success.mp3` & `t_rex_lca-0.2.2/misc/success.mp3`

 * *Files identical despite different names*

### Comparing `t_rex_lca-0.2/src/T-reX/CustomConfig.py` & `t_rex_lca-0.2.2/src/T-reX/CustomConfig.py`

 * *Files identical despite different names*

### Comparing `t_rex_lca-0.2/src/T-reX/ExchangeEditor.py` & `t_rex_lca-0.2.2/src/T-reX/ExchangeEditor.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 Each appended exchange replicates the same amount and unit as the original technosphere waste and material exchange.
 
 """
 
 # Imports
 import os
 from datetime import datetime
-
 import bw2data as bd
 import pandas as pd
 from tqdm import tqdm
 
 
 def ExchangeEditor(project_T_reX, db_name, db_T_reX_name):
     """
```

### Comparing `t_rex_lca-0.2/src/T-reX/ExplodeDatabase.py` & `t_rex_lca-0.2.2/src/T-reX/ExplodeDatabase.py`

 * *Files identical despite different names*

### Comparing `t_rex_lca-0.2/src/T-reX/FutureScenarios.py` & `t_rex_lca-0.2.2/src/T-reX/FutureScenarios.py`

 * *Files 14% similar despite different names*

```diff
@@ -229,28 +229,41 @@
             key=premise_key,
             use_multiprocessing=use_mp,
             system_args=model_args,
             quiet=premise_quiet,
             keep_uncertainty_data=True,
         )
 
-        try:
-            ndb.update_all()
-            ndb.update_cars()
-            ndb.update_buses()
-            ndb.update_emissions()
-            ndb.update_dac()
-            ndb.update_trucks()
-            ndb.update_two_wheelers()
-            ndb.update_electricity()
-            ndb.update_cement()
-            ndb.update_steel()
-            ndb.update_fuels()
-        except Exception as e:
-            print(f"Error: {e}")
+        # List of update functions to try
+        sectors = [
+            "cars",
+            "buses",
+            "two_wheelers",
+            # "dac",
+            # "emissions",
+            # "trucks",
+            # "electricity",
+            # "cement",
+            # "steel",
+            # "fuels",
+        ]
+        
+        # CHANGED UPDATE SYNTAX TO MATCH UPDATES IN PREMISE V2.0.0
+        print("\n***** Updating sectors... *****\n")
+        
+        ndb.update()
+
+        for sector in sectors:
+            try:
+                ndb.update([sector])
+                print(f"Successfully updated {sector}\n")
+                print("*****************************************")
+            except Exception as e:
+                print(f"Error updating {sector}: {e}")
+                print("+++++++++++++++++++++++++++++++++++++++++")
 
         # Write the new database to brightway
         ndb.write_db_to_brightway()
 
     # Add GWP factors to the project
     add_premise_gwp()
     print("***** Done! *****")
```

### Comparing `t_rex_lca-0.2/src/T-reX/MakeCustomDatabase.py` & `t_rex_lca-0.2.2/src/T-reX/MakeCustomDatabase.py`

 * *Files identical despite different names*

### Comparing `t_rex_lca-0.2/src/T-reX/MethodEditor.py` & `t_rex_lca-0.2.2/src/T-reX/MethodEditor.py`

 * *Files identical despite different names*

### Comparing `t_rex_lca-0.2/src/T-reX/SearchMaterial.py` & `t_rex_lca-0.2.2/src/T-reX/SearchMaterial.py`

 * *Files identical despite different names*

### Comparing `t_rex_lca-0.2/src/T-reX/SearchWaste.py` & `t_rex_lca-0.2.2/src/T-reX/SearchWaste.py`

 * *Files identical despite different names*

### Comparing `t_rex_lca-0.2/src/T-reX/VerifyDatabase.py` & `t_rex_lca-0.2.2/src/T-reX/VerifyDatabase.py`

 * *Files identical despite different names*

### Comparing `t_rex_lca-0.2/src/T-reX/__init__.py` & `t_rex_lca-0.2.2/src/T-reX/__init__.py`

 * *Files identical despite different names*

### Comparing `t_rex_lca-0.2/src/T-reX/config/__init__.py` & `t_rex_lca-0.2.2/src/T-reX/config/__init__.py`

 * *Files identical despite different names*

### Comparing `t_rex_lca-0.2/src/T-reX/config/queries_materials.py` & `t_rex_lca-0.2.2/src/T-reX/config/queries_materials.py`

 * *Files identical despite different names*

### Comparing `t_rex_lca-0.2/src/T-reX/config/queries_waste.py` & `t_rex_lca-0.2.2/src/T-reX/config/queries_waste.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
                         "carbon dioxide storage",
                         "carbon dioxide, captured",
                     ]
                 }
             )
             query.update({"NOT": ["methane"]})
             query.update({"AND": [""]})
+        
 
         # add the query to the list of queries
         queries_kg.append(query)
 
     # add same queries defined above, now for liquid waste and material
     queries_m3 = []
     for q in queries_kg:
```

### Comparing `t_rex_lca-0.2/src/T-reX/config/user_settings.py` & `t_rex_lca-0.2.2/src/T-reX/config/user_settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,23 +35,23 @@
 import bw2data as bd
 
 # ------------------------------------------------------------
 ## SETTINGS FOR PROJECTS
 # set project name and other things here
 
 project_premise_base = "default"
-project_premise = "SSP2LT-cutoff"
+project_premise = "premise-SSP2-cutoff"
 project_base = project_premise
 # if you want to use the same project for the T-reX tool, change this to project_base, otherwise, it will create a new project
-project_T_reX = f"T_reX-{project_base}"
+project_T_reX = f"TreX-{project_base}"
 
 # ------------------------------------------------------------
 ## SETTINGS FOR THE WASTEANDMATERIAL FOOTPRINT TOOL
 use_T_reX = True
-db_T_reX_name = "T-reX"  # name of the database that will be created (pseudobiosphere)
+db_T_reX_name = "biosphere_T-reX"  # name of the database that will be created (pseudobiosphere)
 
 # if you only want to run one database, set single to True and choose the database name here
 single = False
 single_database = "ecoinvent_cutoff_3.9_remind_SSP2-Base_2065"
 
 # if you want to use a fresh project
 delete_T_reX_project = True
@@ -62,33 +62,33 @@
 do_search = True
 do_methods = True
 do_edit = True
 
 # ------------------------------------------------------------
 ## PREMISE SETTINGS -  to construct future LCA databases with premise
 
-use_premise = False
+use_premise = True
 
 # this will be the database that premise will use to construct the future databases
 database_name = "ecoinvent-3.9.1-cutoff"
 
 # if you want to use a fresh project
 delete_existing_premise_project = False
 
 # if you want to use multiprocessing in premise (some people have reported problems with this)
 use_mp = True
 
-# if you want to give premise multiple databases at once, increase this number, otherwise, leave it at 1. From my experience, it is better to give it one database at a time, otherwise memory issues can occur.
-batch_size = 1
+# if you want to give premise multiple databases at once, increase this number, otherwise, leave it at 1. Memory issues can occur if the batch size is too large.
+batch_size = 3
 
 # This seems not to have much effect, because most of the print statemenents are in `wurst`, not in `premise`
 premise_quiet = True
 
 if use_premise and project_base != project_premise:
-    project_T_reX = f"T_reX-{project_premise}"
+    project_T_reX = f"T-reX-{project_premise}"
 
 # Get the premise key (at the moment, it is stored in the code to make it easier for people, but it would be better to have it in a file)
 premise_key = "tUePmX_S5B8ieZkkM7WUU2CnO8SmShwmAeWK9x2rTFo="
 if premise_key is None:
     key_path = Path(__file__).parents[1] / ".secrets" / "premise_key.txt"
     with open(key_path, "r") as f:
         premise_key = f.read()
@@ -129,25 +129,30 @@
     # "PkBudg1150",
 ]
 
 # If the years you put here are inside the range of the scenario, it will interpolate the data, otherwise, probably it fails. Most of the scenarios are between 2020 and 2100, I think. 5 year intervals until 2050, then 10 year intervals until 2100.
 
 years = [
     2020,
-    #2030,
-    # 2035,
-    #2040,
-    # 2045,
-    #2050,
-    #2060,
-    # 2065,
-    #2070,
-    #2080,
-    #2090,
-    #2100,
+    2025,
+    2030,
+    2035,
+    2040,
+    2045,
+    2050,
+    2055,
+    2060,
+    2065,
+    2070,
+    2075,
+    2080,
+    2085,
+    2090,
+    2095,
+    2100,
 ]
 
 # this part makes all the possible combinations of the scenarios you want to use, the will be filtered out later if they are not possible
 
 desired_scenarios = []
 for model, ssp, rcp in product(models, ssps, rcps):
     desired_scenarios.append({"model": model, "pathway": ssp + "-" + rcp})
```

### Comparing `t_rex_lca-0.2/src/T-reX/main.py` & `t_rex_lca-0.2.2/src/T-reX/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,14 +117,33 @@
     {80*'='}
     {80*'~'}
     {'** Starting the T-reX tool **'.center(80, ' ')}
     {80*'~'}
     {80*'='}
     """
     )
+    
+    sleep(1)
+
+    try:
+
+        def animate_cowsay(message, delay=0.2):
+            cow = cowsay.get_output_string("stegosaurus", message)
+            for line in cow.split("\n"):
+                print(line.center(80, " "))
+                sleep(delay)
+
+        message = "\nArrrgh!!! a T-reX!!!\n Run away!!!\n"
+        animate_cowsay(message)
+        print("\n\n")
+        print(f'\n{"-"*60}\n')
+    except:
+        pass
+    
+    
     # create future scenario databases
     if use_premise:
         MakeFutureScenarios()
 
     assert use_T_reX, "use_T_reX is False, so T-reX will not run"
 
     start_time = datetime.now()
@@ -403,10 +422,13 @@
             + db_name
             + "\n"
         )
 
     return None
 
 
-# 2. RUN MAIN FUNCTION
 if __name__ == "__main__":
     run()
+    
+    # clean up tmp files
+    for file in dir_tmp.glob("*"):
+        os.remove(file)
```

### Comparing `t_rex_lca-0.2/src/config_backup/__init__.py` & `t_rex_lca-0.2.2/src/T-reX/config_backup/__init__.py`

 * *Files identical despite different names*

### Comparing `t_rex_lca-0.2/src/config_backup/queries_materials.py` & `t_rex_lca-0.2.2/src/T-reX/config_backup/queries_materials.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,34 +21,36 @@
     ("market for beryllium", "beryllium"),
     ("market for bismuth", "bismuth"),
     ("market for cadmium", "cadmium"),
     ("market for calcium borates", "borates"),
     ("market for cement", "cement"),
     ("market for cerium", "cerium"),
     ("market for chromium", "chromium"),
-    ("market for coal", "coal"),
     ("market for cobalt", "cobalt"),
     ("market for coke", "coke"),
     ("market for copper", "copper"),
     ("market for dysprosium", "dysprosium"),
     ("market for erbium", "erbium"),
     ("market for europium", "europium"),
     ("market for electricity,", "electricity"),
     ("market for ferroniobium,", "niobium"),
     ("market for fluorspar,", "fluorspar"),
     ("market for gadolinium", "gadolinium"),
     ("market for gallium", "gallium"),
     ("market for gold", "gold"),
     ("market for graphite", "graphite"),
     ("market for hafnium", "hafnium"),
+    ("market for hard coal", "coal(black)"),
     ("market for helium", "helium"),
     ("market for holmium", "holmium"),
     ("market for hydrogen,", "hydrogen"),
     ("market for indium", "indium"),
     ("market for latex", "latex"),
+    ("market for lead", "lead"),
+    ("market for lignite", "coal(brown)"),
     ("market for lithium", "lithium"),
     ("market for magnesium", "magnesium"),
     ("market for natural gas,", "natural gas"),
     ("market for nickel", "nickel"),
     ("market for palladium", "palladium"),
     ("market for petroleum", "petroleum"),
     ("market for phosphate", "phosphate rock"),
```

### Comparing `t_rex_lca-0.2/src/config_backup/queries_waste.py` & `t_rex_lca-0.2.2/src/T-reX/config_backup/queries_waste.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         "digestion",
         "composting",
         "open burning",
         "incineration",
         "recycling",
         "landfill",
         "hazardous",
+        "radioactive",
         # "non-hazardous", # not really needed, as it is just "total" - "hazardous", and it makes the process slower (20k+ more exchanges)
         "carbon dioxide",  # in prospective databases, carbon capture and storage is included
         "total",
     ]
 
     # QUERY FORMAT
     # setup the dictionary of search terms for
@@ -81,21 +82,21 @@
         if "radioactive" in name:
             query["AND"] += ["radioactive"]
         if "carbon dioxide" in name:
             query.update(
                 {
                     "OR": [
                         "carbon dioxide storage",
-                        "carbon dioxide capture",
                         "carbon dioxide, captured",
                     ]
                 }
             )
             query.update({"NOT": ["methane"]})
-            query.update({"AND": ""})
+            query.update({"AND": [""]})
+        
 
         # add the query to the list of queries
         queries_kg.append(query)
 
     # add same queries defined above, now for liquid waste and material
     queries_m3 = []
     for q in queries_kg:
```

### Comparing `t_rex_lca-0.2/src/config_backup/user_settings.py` & `t_rex_lca-0.2.2/src/T-reX/config_backup/user_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 user_settings Module
 ====================
 
-Configure Project and Database Settings for T-reX tool.
+Configure Project and Database Settings for T-reX.
 
 This script is used to configure the project and database settings, as well as set up the essential paths for the data, config, and result directories.
 
 The script allows for two modes of operation:
     1. Single Mode (`single` is True): Set the project and database names to a single specified value.
     2. Multiple projects/databases mode (`single` is False): Facilitates batch processing of multiple projects and databases.
 
@@ -35,60 +35,60 @@
 import bw2data as bd
 
 # ------------------------------------------------------------
 ## SETTINGS FOR PROJECTS
 # set project name and other things here
 
 project_premise_base = "default"
-project_premise = "SSP-cutoff"
+project_premise = "premise-SSP2-cutoff"
 project_base = project_premise
 # if you want to use the same project for the T-reX tool, change this to project_base, otherwise, it will create a new project
-project_T_reX = f"T_reX-{project_base}"
+project_T_reX = f"TreX-{project_base}"
 
 # ------------------------------------------------------------
 ## SETTINGS FOR THE WASTEANDMATERIAL FOOTPRINT TOOL
-use_T_reX = False
-db_T_reX_name = "T-reX"  # name of the database that will be created (pseudobiosphere)
+use_T_reX = True
+db_T_reX_name = "biosphere_T-reX"  # name of the database that will be created (pseudobiosphere)
 
 # if you only want to run one database, set single to True and choose the database name here
 single = False
-single_database = "ecoinvent_cutoff_3.9_remind_SSP5-Base_2050"
+single_database = "ecoinvent_cutoff_3.9_remind_SSP2-Base_2065"
 
 # if you want to use a fresh project
-delete_T_reX_project = False
+delete_T_reX_project = True
 use_multiprocessing = False
 verbose = False
 
 # set these to True if you want to run the different parts of the tool separately
 do_search = True
 do_methods = True
 do_edit = True
 
 # ------------------------------------------------------------
 ## PREMISE SETTINGS -  to construct future LCA databases with premise
 
-use_premise = False
+use_premise = True
 
 # this will be the database that premise will use to construct the future databases
 database_name = "ecoinvent-3.9.1-cutoff"
 
 # if you want to use a fresh project
-delete_existing_premise_project = False
+delete_existing_premise_project = True
 
-# if you want to use multiprocessing (some people have reported problems with this)
+# if you want to use multiprocessing in premise (some people have reported problems with this)
 use_mp = True
 
-# if you want to give premise multiple databases at once, increase this number, otherwise, leave it at 1. From my experience, it is better to give it one database at a time, otherwise memory issues can occur.
-batch_size = 1
+# if you want to give premise multiple databases at once, increase this number, otherwise, leave it at 1. Memory issues can occur if the batch size is too large.
+batch_size = 9
 
 # This seems not to have much effect, because most of the print statemenents are in `wurst`, not in `premise`
 premise_quiet = True
 
 if use_premise and project_base != project_premise:
-    project_T_reX = f"T_reX-{project_premise}"
+    project_T_reX = f"T-reX-{project_premise}"
 
 # Get the premise key (at the moment, it is stored in the code to make it easier for people, but it would be better to have it in a file)
 premise_key = "tUePmX_S5B8ieZkkM7WUU2CnO8SmShwmAeWK9x2rTFo="
 if premise_key is None:
     key_path = Path(__file__).parents[1] / ".secrets" / "premise_key.txt"
     with open(key_path, "r") as f:
         premise_key = f.read()
@@ -128,26 +128,30 @@
     "PkBudg500",
     # "PkBudg1150",
 ]
 
 # If the years you put here are inside the range of the scenario, it will interpolate the data, otherwise, probably it fails. Most of the scenarios are between 2020 and 2100, I think. 5 year intervals until 2050, then 10 year intervals until 2100.
 
 years = [
-    # 2020,
-    # 2025,
+    2020,
+    2025,
     2030,
-    # 2035,
-    # 2040,
-    # 2045,
-    # 2050,
-    # 2060,
+    2035,
+    2040,
+    2045,
+    2050,
+    2055,
+    2060,
     2065,
-    # 2070,
-    # 2080,
-    # 2090,
+    2070,
+    2075,
+    2080,
+    2085,
+    2090,
+    2095,
     2100,
 ]
 
 # this part makes all the possible combinations of the scenarios you want to use, the will be filtered out later if they are not possible
 
 desired_scenarios = []
 for model, ssp, rcp in product(models, ssps, rcps):
@@ -196,19 +200,15 @@
 # By default, the program will create new directories in the working directory
 
 
 # Get the directory of the main script
 cwd = Path.cwd()
 # Set the paths
 dir_config = cwd / "config"
-
-list_materials = dir_config / "list_materials.txt"
-
 dir_data = cwd / "data"
-
 dir_tmp = dir_data / "tmp"
 dir_logs = dir_data / "logs"
 
 dir_searchwaste_results = dir_data / "SearchWasteResults"
 dir_searchmaterial_results = dir_data / "SearchMaterialResults"
 dir_databases_T_reX = dir_data / "DatabasesWasteAndMaterial"
```

### Comparing `t_rex_lca-0.2/tests/test-import.py` & `t_rex_lca-0.2.2/tests/test-import.py`

 * *Files identical despite different names*

### Comparing `t_rex_lca-0.2/PKG-INFO` & `t_rex_lca-0.2.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,64 @@
 Metadata-Version: 2.1
 Name: T_reX_LCA
-Version: 0.2
+Version: 0.2.2
 Summary: A tool for analysing waste and material footprints in Life Cycle Assessment (LCA) databases
 License: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Author: Stewart Charles McDowall
 Author-email: s.c.mcdowall@cml.leidenuniv.nl
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Dist: bw2calc (>=1.8.2,<2.0.0)
-Requires-Dist: bw2data (>=3.6.6,<4.0.0)
-Requires-Dist: bw2io (>=0.8.12,<0.9.0)
+Requires-Dist: brightway2 (>=2.4.6,<3.0.0)
 Requires-Dist: cowsay (>=6.1,<7.0)
-Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
-Requires-Dist: pandas (>=2.1.4,<3.0.0)
-Requires-Dist: premise (>=1.8.2dev3,<2.0.0)
-Requires-Dist: premise-gwp (>=0.9.6,<0.10.0)
-Requires-Dist: tqdm (>=4.66.1,<5.0.0)
-Requires-Dist: wurst (>=0.4,<0.5)
+Requires-Dist: premise (>=2.0.2,<3.0.0)
+Project-URL: documentation, https://T-reX.readthedocs.io/en/latest/
+Project-URL: homepage, https://github.com/Stew-McD/T-reX
 Description-Content-Type: text/markdown
 
-# T-reX (formerly "WasteAndMaterialFootprint)
+# T-reX: waste and material footprinting in LCA
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10431181.svg)](https://doi.org/10.5281/zenodo.10431180)
 
-A program for Life Cycle Assessment (LCA) calculations of supply chain waste and material footprints.
+Formerly known as "WasteAndMaterialFootprint"
 
-Soon to be a paper, hopefully. The manuscript has its own github repo [here](https://github.com/Stew-McD/T-reX_publication)
+**T** stands for *tool* and **reX** for *the circular economy strategies reduce, reuse, recycle, etc.* 
+
+A python program for Life Cycle Assessment (LCA) calculations of supply chain waste and material footprints in current and prospective databases.
+
+Built as an extension to the [brightway LCA ecosystem](https://brightway.dev/), using [premise](https://github.com/polca/premise) for the generation of future scenario databases and [wurst](https://github.com/polca/wurst) for database expansion. 
+
+Soon to be a paper, hopefully. The manuscript has its own github repo [here](https://github.com/Stew-McD/T-reX_Publication). Reviews and comments are very welcome.
+
+Email: T-reX@scmcd.ch
 
 ## Documentation
 
 The documentation is available as a [website](https://T-reX.readthedocs.io/en/latest/). Also, as a  [pdf](https://T-reX.readthedocs.io/_/downloads/en/latest/pdf/).
 
-The documentation is still under development, but the code is well documented and there is a full API reference.
+The documentation is still under development, but the code is well commented and there is a full API reference.
 
 The following readme provides a brief introduction to the program, how to install it, and how to use it.
 
 See the example output [here](examples/package_test/example-output.pdf)
 
 ## Contents
 
-- [T-reX (formerly "WasteAndMaterialFootprint)](#t-rex-formerly-wasteandmaterialfootprint)
+- [T-reX: waste and material footprinting in LCA](#t-rex-waste-and-material-footprinting-in-lca)
   - [Documentation](#documentation)
   - [Contents](#contents)
+  - [Visual overview](#visual-overview)
+    - [Generalised and computational flowcharts](#generalised-and-computational-flowcharts)
   - [Installation](#installation)
     - [Dependencies](#dependencies)
     - [Installation instructions](#installation-instructions)
   - [Usage](#usage)
     - [Command line](#command-line)
     - [Python module](#python-module)
   - [Configuration](#configuration)
@@ -70,14 +75,20 @@
       - [Usage Considerations](#usage-considerations)
         - [Example Tuples](#example-tuples)
     - [Examples](#examples)
     - [Contributing](#contributing)
     - [License](#license)
     - [Citation](#citation)
 
+## Visual overview
+
+### Generalised and computational flowcharts
+
+<img src="docs/source/_static/T-reX_flowchart_combined.png" alt="T-reX flowcharts" width="500">
+
 ## Installation
 
 ### Dependencies
 
 The program is written in Python and the required packages are listed in the `requirements.txt` file. These should be installed automatically when installing the program.
 
 The main dependencies are:
@@ -124,15 +135,15 @@
   ```bash
   pip install -r requirements.txt
   ```
 
 Another option: the program can be installed using pip:
 
   ```bash
-  pip install T-reX
+  pip install T_reX_LCA
   ```
 
 Or, if you want to install the latest version from GitHub:
 
   ```bash
   pip install git+https://github.com/Stew-McD/T-reX.git
   ```
@@ -158,43 +169,43 @@
   ```
 
 ### Python module
 
 The program can be imported as a Python module:
 
   ```python
-      import T-reX as T-reX
-      T-reX.run()
+      import T_reX_LCA as TreX
+      TreX.run()
   ```
 
 ## Configuration
 
 You can find the configuration files in the `config` folder (`src/T-reX/config`). Or if you install it with pip, you can find the config folder in the `site-packages/T-reX/config` folder of your Python venv installation.
 
 If you have installed via pip, or want to have things separate, you can create a new folder somewhere and then run some built-in functions to create and reload the config files.
 
   ```python
-      import T-reX as T-reX
-      T-reX.create_config()
+      import T_reX_LCA as TreX
+      TreX.create_config()
   ```
 
 This will create a folder `config` in the current working directory containing the default configuration files (see below).
 
 You can then edit these files with some kind of text editor, and run:
 
   ```python
-      T-reX.reload_config()
+      TreX.reload_config()
   ```
 
 Note that you will need to close the Python session and start a new one to reload the config files.
 
 If you want to revert to the default config files, you can run:
 
   ```python
-      T-reX.reset_config()
+      TreX.reset_config()
   ```
 
 And then close and restart the Python session.
 
 If you are running the program as an editable package, you can edit the config files directly in the `src/T-reX/config` folder.
 
 Details of the configuration files are given below.
@@ -216,15 +227,15 @@
       # Choose whether to use T-reX to edit the databases (you could also turn this off and just use the package as an easy way to make a set of future scenario databases)
       use_T_reX = True
 
       # Choose the names of the projects to use
       project_premise_base = "default"
       project_premise = "SSP-cutoff"
       project_base = project_premise
-      project_T_reX = f"T_reXootprint-{project_base}"
+      project_T_reX = f"T-reX-{project_base}"
 
       # Choose the name of the database to use (needed for premise only, the T-reX tool will run all databases except the biospheres)
       database_name = "ecoinvent-3.9.1-cutoff"
 
       # if you want to use a fresh project
       delete_existing_premise_project = False
       delete_existing_T_reX_project = False
@@ -321,15 +332,15 @@
 
 Contributions are very welcome! Test the code, report bugs, suggest features, etc. If you want to contribute code, please fork the repo and make a pull request.
 
 See the [CONTRIBUTING.md](CONTRIBUTING.md) file for more details.
 
 ### License
 
-T-reX by Stewart Charles McDowall is marked with CC0 1.0 Universal, do whatever you want with it - see the [LICENSE](LICENSE) file for details
+T-reX by Stewart Charles McDowall is marked with CC0 1.0 Universal, do whatever you want with it. - see the [LICENSE](LICENSE) file for details
 
 ### Citation
 
 If you use this code, please cite it as described in the [CITATION.cff](CITATION.cff) file (see the sidebar on the right).
 
 When the paper is published, a citation for that will be added to the CITATION file.
```

