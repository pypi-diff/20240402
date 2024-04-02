# Comparing `tmp/monviso-0.1.0.tar.gz` & `tmp/monviso-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/monviso-0.1.0.tar", last modified: Wed Feb 28 11:03:40 2024, max compression
+gzip compressed data, was "dist/monviso-0.1.1.tar", last modified: Tue Apr  2 13:10:01 2024, max compression
```

## Comparing `monviso-0.1.0.tar` & `monviso-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,49 @@
-drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-02-28 11:03:40.922444 monviso-0.1.0/
--rw-r--r--   0 albani     (502) staff       (20)       89 2024-02-28 10:12:03.000000 monviso-0.1.0/Containerfile
--rw-r--r--   0 albani     (502) staff       (20)      229 2024-02-28 10:12:03.000000 monviso-0.1.0/HISTORY.md
--rw-r--r--   0 albani     (502) staff       (20)     1211 2024-02-28 10:12:03.000000 monviso-0.1.0/LICENSE
--rw-r--r--   0 albani     (502) staff       (20)       92 2024-02-28 10:12:03.000000 monviso-0.1.0/MANIFEST.in
--rw-r--r--   0 albani     (502) staff       (20)     2277 2024-02-28 11:03:40.921729 monviso-0.1.0/PKG-INFO
--rw-r--r--   0 albani     (502) staff       (20)     1302 2024-02-28 10:12:03.000000 monviso-0.1.0/README.md
-drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-02-28 11:03:40.904420 monviso-0.1.0/monviso.egg-info/
--rw-r--r--   0 albani     (502) staff       (20)     2277 2024-02-28 11:03:40.000000 monviso-0.1.0/monviso.egg-info/PKG-INFO
--rw-r--r--   0 albani     (502) staff       (20)      726 2024-02-28 11:03:40.000000 monviso-0.1.0/monviso.egg-info/SOURCES.txt
--rw-r--r--   0 albani     (502) staff       (20)        1 2024-02-28 11:03:40.000000 monviso-0.1.0/monviso.egg-info/dependency_links.txt
--rw-r--r--   0 albani     (502) staff       (20)       69 2024-02-28 11:03:40.000000 monviso-0.1.0/monviso.egg-info/entry_points.txt
--rw-r--r--   0 albani     (502) staff       (20)      125 2024-02-28 11:03:40.000000 monviso-0.1.0/monviso.egg-info/requires.txt
--rw-r--r--   0 albani     (502) staff       (20)       17 2024-02-28 11:03:40.000000 monviso-0.1.0/monviso.egg-info/top_level.txt
-drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-02-28 11:03:40.917982 monviso-0.1.0/monviso_reloaded/
--rw-r--r--   0 albani     (502) staff       (20)     6906 2024-02-28 10:12:03.000000 monviso-0.1.0/monviso_reloaded/PDB_manager.py
--rw-r--r--   0 albani     (502) staff       (20)        6 2024-02-28 10:12:03.000000 monviso-0.1.0/monviso_reloaded/VERSION
--rw-r--r--   0 albani     (502) staff       (20)        0 2024-02-28 10:12:03.000000 monviso-0.1.0/monviso_reloaded/__init__.py
--rw-r--r--   0 albani     (502) staff       (20)      158 2024-02-28 10:12:03.000000 monviso-0.1.0/monviso_reloaded/__main__.py
--rw-r--r--   0 albani     (502) staff       (20)     4103 2024-02-28 10:12:03.000000 monviso-0.1.0/monviso_reloaded/base.py
--rw-r--r--   0 albani     (502) staff       (20)      570 2024-02-28 10:12:03.000000 monviso-0.1.0/monviso_reloaded/cli.py
--rw-r--r--   0 albani     (502) staff       (20)     1739 2024-02-28 10:12:03.000000 monviso-0.1.0/monviso_reloaded/cobalt_wrapper.py
--rw-r--r--   0 albani     (502) staff       (20)     3195 2024-02-28 10:12:03.000000 monviso-0.1.0/monviso_reloaded/database_parser.py
--rw-r--r--   0 albani     (502) staff       (20)     3740 2024-02-28 10:12:03.000000 monviso-0.1.0/monviso_reloaded/file_handler.py
--rw-r--r--   0 albani     (502) staff       (20)    12350 2024-02-28 10:12:03.000000 monviso-0.1.0/monviso_reloaded/gene.py
--rw-r--r--   0 albani     (502) staff       (20)     8723 2024-02-28 10:12:03.000000 monviso-0.1.0/monviso_reloaded/input_parser.py
--rw-r--r--   0 albani     (502) staff       (20)    18946 2024-02-28 10:12:03.000000 monviso-0.1.0/monviso_reloaded/isoform.py
--rw-r--r--   0 albani     (502) staff       (20)     9032 2024-02-28 10:12:03.000000 monviso-0.1.0/monviso_reloaded/modeller_manager.py
--rw-r--r--   0 albani     (502) staff       (20)     5480 2024-02-28 10:12:03.000000 monviso-0.1.0/monviso_reloaded/template.py
--rw-r--r--   0 albani     (502) staff       (20)       38 2024-02-28 11:03:40.922747 monviso-0.1.0/setup.cfg
--rw-r--r--   0 albani     (502) staff       (20)     1581 2024-02-28 11:02:53.000000 monviso-0.1.0/setup.py
-drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-02-28 11:03:40.920581 monviso-0.1.0/tests/
--rw-r--r--   0 albani     (502) staff       (20)        0 2024-02-28 10:12:03.000000 monviso-0.1.0/tests/__init__.py
--rw-r--r--   0 albani     (502) staff       (20)      398 2024-02-28 10:12:03.000000 monviso-0.1.0/tests/conftest.py
--rw-r--r--   0 albani     (502) staff       (20)       96 2024-02-28 10:12:03.000000 monviso-0.1.0/tests/test_base.py
+drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-02 13:10:01.078699 monviso-0.1.1/
+-rw-r--r--   0 albani     (502) staff       (20)       89 2024-02-28 10:12:03.000000 monviso-0.1.1/Containerfile
+-rw-r--r--   0 albani     (502) staff       (20)      388 2024-04-02 13:03:27.000000 monviso-0.1.1/HISTORY.md
+-rw-r--r--   0 albani     (502) staff       (20)     1211 2024-02-28 10:12:03.000000 monviso-0.1.1/LICENSE
+-rw-r--r--   0 albani     (502) staff       (20)       92 2024-02-28 10:12:03.000000 monviso-0.1.1/MANIFEST.in
+-rw-r--r--   0 albani     (502) staff       (20)     2260 2024-04-02 13:10:01.078213 monviso-0.1.1/PKG-INFO
+-rw-r--r--   0 albani     (502) staff       (20)     1302 2024-02-28 10:12:03.000000 monviso-0.1.1/README.md
+drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-02 13:10:01.042437 monviso-0.1.1/monviso.egg-info/
+-rw-r--r--   0 albani     (502) staff       (20)     2260 2024-04-02 13:10:00.000000 monviso-0.1.1/monviso.egg-info/PKG-INFO
+-rw-r--r--   0 albani     (502) staff       (20)     1433 2024-04-02 13:10:00.000000 monviso-0.1.1/monviso.egg-info/SOURCES.txt
+-rw-r--r--   0 albani     (502) staff       (20)        1 2024-04-02 13:10:00.000000 monviso-0.1.1/monviso.egg-info/dependency_links.txt
+-rw-r--r--   0 albani     (502) staff       (20)       69 2024-04-02 13:10:00.000000 monviso-0.1.1/monviso.egg-info/entry_points.txt
+-rw-r--r--   0 albani     (502) staff       (20)      125 2024-04-02 13:10:00.000000 monviso-0.1.1/monviso.egg-info/requires.txt
+-rw-r--r--   0 albani     (502) staff       (20)       17 2024-04-02 13:10:00.000000 monviso-0.1.1/monviso.egg-info/top_level.txt
+drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-02 13:10:01.058065 monviso-0.1.1/monviso_reloaded/
+-rw-r--r--   0 albani     (502) staff       (20)     6906 2024-02-28 10:12:03.000000 monviso-0.1.1/monviso_reloaded/PDB_manager.py
+-rw-r--r--   0 albani     (502) staff       (20)        6 2024-04-02 12:58:34.000000 monviso-0.1.1/monviso_reloaded/VERSION
+-rw-r--r--   0 albani     (502) staff       (20)        0 2024-02-28 10:12:03.000000 monviso-0.1.1/monviso_reloaded/__init__.py
+-rw-r--r--   0 albani     (502) staff       (20)      158 2024-02-28 10:12:03.000000 monviso-0.1.1/monviso_reloaded/__main__.py
+drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-02 13:10:01.074242 monviso-0.1.1/monviso_reloaded/__pycache__/
+-rw-r--r--   0 albani     (502) staff       (20)     5885 2024-03-01 15:37:30.000000 monviso-0.1.1/monviso_reloaded/__pycache__/PDB_manager.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)      172 2024-03-01 15:27:07.000000 monviso-0.1.1/monviso_reloaded/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)      309 2024-03-01 15:27:07.000000 monviso-0.1.1/monviso_reloaded/__pycache__/__main__.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     4774 2024-03-29 12:14:49.000000 monviso-0.1.1/monviso_reloaded/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)      873 2024-03-01 15:27:07.000000 monviso-0.1.1/monviso_reloaded/__pycache__/cli.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     1983 2024-03-01 15:37:30.000000 monviso-0.1.1/monviso_reloaded/__pycache__/cobalt_wrapper.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     4744 2024-03-11 14:35:13.000000 monviso-0.1.1/monviso_reloaded/__pycache__/database_parser.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     4744 2024-03-11 14:31:42.000000 monviso-0.1.1/monviso_reloaded/__pycache__/file_handler.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     8605 2024-03-29 13:43:08.000000 monviso-0.1.1/monviso_reloaded/__pycache__/gene.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     6792 2024-03-01 15:46:41.000000 monviso-0.1.1/monviso_reloaded/__pycache__/input_parser.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)    16845 2024-03-29 09:02:50.000000 monviso-0.1.1/monviso_reloaded/__pycache__/isoform.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)    11425 2024-03-29 16:19:47.000000 monviso-0.1.1/monviso_reloaded/__pycache__/modeller_manager.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     4678 2024-03-01 15:37:30.000000 monviso-0.1.1/monviso_reloaded/__pycache__/template.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     4378 2024-03-29 11:42:41.000000 monviso-0.1.1/monviso_reloaded/base.py
+-rw-r--r--   0 albani     (502) staff       (20)      570 2024-02-28 10:12:03.000000 monviso-0.1.1/monviso_reloaded/cli.py
+-rw-r--r--   0 albani     (502) staff       (20)     1739 2024-02-28 10:12:03.000000 monviso-0.1.1/monviso_reloaded/cobalt_wrapper.py
+-rw-r--r--   0 albani     (502) staff       (20)     4013 2024-03-11 14:35:11.000000 monviso-0.1.1/monviso_reloaded/database_parser.py
+-rw-r--r--   0 albani     (502) staff       (20)     4181 2024-03-11 14:31:34.000000 monviso-0.1.1/monviso_reloaded/file_handler.py
+-rw-r--r--   0 albani     (502) staff       (20)    12827 2024-03-29 13:41:56.000000 monviso-0.1.1/monviso_reloaded/gene.py
+-rw-r--r--   0 albani     (502) staff       (20)     8954 2024-03-01 15:46:37.000000 monviso-0.1.1/monviso_reloaded/input_parser.py
+-rw-r--r--   0 albani     (502) staff       (20)    21299 2024-03-29 09:02:47.000000 monviso-0.1.1/monviso_reloaded/isoform.py
+-rw-r--r--   0 albani     (502) staff       (20)    13309 2024-03-29 16:18:28.000000 monviso-0.1.1/monviso_reloaded/modeller_manager.py
+-rw-r--r--   0 albani     (502) staff       (20)     5480 2024-02-28 10:12:03.000000 monviso-0.1.1/monviso_reloaded/template.py
+-rw-r--r--   0 albani     (502) staff       (20)       38 2024-04-02 13:10:01.078858 monviso-0.1.1/setup.cfg
+-rw-r--r--   0 albani     (502) staff       (20)     1567 2024-02-28 11:07:33.000000 monviso-0.1.1/setup.py
+drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-02 13:10:01.077170 monviso-0.1.1/tests/
+-rw-r--r--   0 albani     (502) staff       (20)        0 2024-02-28 10:12:03.000000 monviso-0.1.1/tests/__init__.py
+-rw-r--r--   0 albani     (502) staff       (20)      398 2024-02-28 10:12:03.000000 monviso-0.1.1/tests/conftest.py
+-rw-r--r--   0 albani     (502) staff       (20)       96 2024-02-28 10:12:03.000000 monviso-0.1.1/tests/test_base.py
```

### Comparing `monviso-0.1.0/LICENSE` & `monviso-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `monviso-0.1.0/PKG-INFO` & `monviso-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: monviso
-Version: 0.1.0
+Version: 0.1.1
 Summary: MoNvIso is a comprehensive software tool designed for the analysis and modeling of protein isoforms. It automates the process of identifying canonical and additional isoforms, assessing their modeling propensity, mapping mutations accurately, and building structural models of proteins.
 Home-page: https://github.com/alisamalb/monviso_reloaded
-Author: ['alisamalb', 'Ciskio']
+Author: Ciskio
 License: UNKNOWN
 Description: # Monviso reloaded
         MoNvIso is a comprehensive software tool designed for the analysis and modeling of protein isoforms. It automates the process of identifying canonical and additional isoforms, assessing their modeling propensity, mapping mutations accurately, and building structural models of proteins. By leveraging data from the Uniprot database, MoNvIso facilitates a deeper understanding of protein function and variation.
         
         [Read the documentation here.](https://alisamalb.github.io/monviso_reloaded/)
         
         ## Quick start
```

### Comparing `monviso-0.1.0/README.md` & `monviso-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `monviso-0.1.0/monviso.egg-info/PKG-INFO` & `monviso-0.1.1/monviso.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: monviso
-Version: 0.1.0
+Version: 0.1.1
 Summary: MoNvIso is a comprehensive software tool designed for the analysis and modeling of protein isoforms. It automates the process of identifying canonical and additional isoforms, assessing their modeling propensity, mapping mutations accurately, and building structural models of proteins.
 Home-page: https://github.com/alisamalb/monviso_reloaded
-Author: ['alisamalb', 'Ciskio']
+Author: Ciskio
 License: UNKNOWN
 Description: # Monviso reloaded
         MoNvIso is a comprehensive software tool designed for the analysis and modeling of protein isoforms. It automates the process of identifying canonical and additional isoforms, assessing their modeling propensity, mapping mutations accurately, and building structural models of proteins. By leveraging data from the Uniprot database, MoNvIso facilitates a deeper understanding of protein function and variation.
         
         [Read the documentation here.](https://alisamalb.github.io/monviso_reloaded/)
         
         ## Quick start
```

### Comparing `monviso-0.1.0/monviso_reloaded/PDB_manager.py` & `monviso-0.1.1/monviso_reloaded/PDB_manager.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.0/monviso_reloaded/base.py` & `monviso-0.1.1/monviso_reloaded/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,24 +90,30 @@
     def select_isoforms(self) -> None:
         for gene in self.genes:
             gene.select_isoforms(
                 float(self.parameters["W_STRUCT"]),
                 float(self.parameters["W_MUT"]),
                 float(self.parameters["SEQID"]),
                 int(self.parameters["MODEL_CUTOFF"]),
+                cobalt_home=self.parameters["COBALT_HOME"],
             )
 
     def start_modeller(self) -> None:
         """Run modeller only for the isoforms to model.
         The method write_modeller() of the isoform accepts the mutation
         as argument.
         """
         for gene in self.genes:
+            gene.report_on_selected_isoforms()
             for isoform, mutation in gene.isoforms_to_model:
                 isoform.run_modeller(
                     mutation, self.parameters["MODELLER_EXEC"],
-                    int(self.parameters["MODEL_CUTOFF"])
-                )
+                    int(self.parameters["MODEL_CUTOFF"]),
+                    int(self.parameters["NUM_OF_MOD_WT"]),
+                    int(self.parameters["NUM_OF_MOD_MUT"]),
+                    self.parameters["COBALT_HOME"])
+
+            
 
     def write_report(self):
         for gene in self.genes:
             gene.write_report()
```

### Comparing `monviso-0.1.0/monviso_reloaded/cli.py` & `monviso-0.1.1/monviso_reloaded/cli.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.0/monviso_reloaded/cobalt_wrapper.py` & `monviso-0.1.1/monviso_reloaded/cobalt_wrapper.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.0/monviso_reloaded/database_parser.py` & `monviso-0.1.1/monviso_reloaded/database_parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,52 @@
 from pathlib import Path
-
+import datetime
+from .file_handler import FileHandler
 
 class DatabaseParser:
     def __init__(self, db_location: str):
         self.db_location = db_location
         self.load_database()
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
-
+    
+    def _check_file_age(self,file_creation_time):
+        """Given a database Path, loads the date of the creation
+        of the file. If it exceeds n_weeks, it raises a warning.
+        
+        The parameter file_creation_time is obtained from FileHandler.get_date()"""
+
+        current_time = datetime.datetime.now()
+        creation_time = datetime.datetime.fromtimestamp(file_creation_time)
+        age = current_time - creation_time
+        
+        if age > datetime.timedelta(weeks=24):
+            print(f"\n\n---WARNING---\n",
+                  "The file database is older than 24 weeks.\nIt should be updated.\n----------")
+    
     def parse_database(self, database_path: Path) -> list[list[str]]:
         """
         Splits the sequences from a database file into a list, where each
         list element corresponds to a single sequence.
         Each sequence is represented as a list of strings, with each string
         being a line from the database that contains
         a part of the sequence. This allows for multi-line sequences in the
         database to be captured fully in each element.
 
         :param database_path: The Path pointing to the Uniprot database
         :return: A list of gene sequences, each split in multiple lines
         """
-        with open(database_path, "r") as f:
-            content = f.read()
+        with FileHandler() as fh:
+            content = fh.read_file(database_path)
+            file_creation_time=fh.get_date(database_path)
+            self._check_file_age(file_creation_time)
         return [
             block.splitlines()
             for block in content.split(">")
             if "sp|" in block
         ]
 
     def load_database(self):
```

### Comparing `monviso-0.1.0/monviso_reloaded/file_handler.py` & `monviso-0.1.1/monviso_reloaded/file_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import os
 import shutil
 from pathlib import Path
 from typing import Union
 
-
 class FileHandler:
     def __init__(self):
         pass
 
     def __enter__(self):
         return self
 
@@ -106,7 +105,21 @@
             raise (FileNotFoundError("The specified file was not found."))
 
         else:
             path = Path(path)
             with path.open("r") as file:
                 content = file.read()
                 return content
+        
+    def get_date(self,path: Union[str,Path]):
+        """ Given a file, returns the creation a last-modified
+            time as a tuple in "seconds since the epoch"
+
+        Args:
+            path (Union[str,Path]): The path of the file
+        """
+        # Both the variables would contain time
+        # elapsed since EPOCH in float
+        ti_c = os.path.getctime(path)
+        ti_m = os.path.getmtime(path)
+
+        return ti_c
```

### Comparing `monviso-0.1.0/monviso_reloaded/gene.py` & `monviso-0.1.1/monviso_reloaded/gene.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from pathlib import Path
+from copy import copy
 
 from Bio.PDB.Polypeptide import index_to_one, three_to_index
 
 from .database_parser import DatabaseParser
 from .file_handler import FileHandler
 from .isoform import Isoform
 
@@ -201,67 +202,64 @@
                     "".join(number),
                     "".join(second_resname),
                 ]
             )
 
         return standard_mutation_list
 
-    def _report_on_selected_isoforms(self):
+    def report_on_selected_isoforms(self):
         """Print on screen a report on the selected isoforms."""
 
         print(
-            f"For the gene {self.name} the following models will be created:"
+            f"For the gene {self.name} the following models will be created,\n"
+            "if the mutation is covered by the strctural templates:"
         )
         for modellable_isoform in self.isoforms_to_model:
             print(
                 f"{modellable_isoform[0].isoform_name} "
                 + "".join(modellable_isoform[1])
             )
 
     def select_isoforms(
         self, w1: float, w2: float, sequence_identity_cutoff: float,
-        model_cutoff: int
+        model_cutoff: int,cobalt_home
     ) -> None:
         """Start the calculation of the scores for all isoforms. The
         templates of each isoform are filtered, based on the sequence
         identity. The isoforms that still have templates
         are ordered by their selection score.
 
         Args:
             w1 (float): weight of the structural function
             w2 (float): weight of the mutation function
             sequence_identity_cutoff (float): templates with a seq. identity
                                               lower than this, are excluded.
         """
         for isoform in self.isoforms:
-
-            isoform.calculate_mutation_score(self.mappable_mutations)
-            isoform.calculate_structural_score(model_cutoff)
-            isoform.filter_templates_by_sequence_identity(
-                sequence_identity_cutoff
-            )
-            isoform.calculate_selection_score(w1, w2)
+            isoform.calculate_score(self.mappable_mutations,model_cutoff,
+                                    sequence_identity_cutoff,w1,w2,
+                                    cobalt_home)
 
         self.isoforms = [
             isoform for isoform in self.isoforms if isoform.modellable
         ]
         if len(self.isoforms) == 0:
             print(f"No modellable isoform for gene {self.name}")
         else:
             self.isoforms.sort(key=lambda x: -x.selection_score)
 
             # Add wild type to list of isoforms to model
-            self.isoforms_to_model.append([self.isoforms[0], "WT"])
+            self.isoforms_to_model.append([copy(self.isoforms[0]), "WT"])
 
             # Take note of mutations to model
             mutations_to_model = self.mutations[:]
 
             # Add mutations of best isoform
             for mutation in self.isoforms[0].mutations:
-                self.isoforms_to_model.append([self.isoforms[0], mutation])
+                self.isoforms_to_model.append([copy(self.isoforms[0]), mutation])
                 mutations_to_model.remove(mutation)
 
             # Try other isoforms to model all mutations
             # if there are other isoforms to select from
             if len(self.isoforms) > 0:
                 for mutation in mutations_to_model:
                     check_across_isoforms = [
@@ -272,15 +270,14 @@
                         isoform_for_mutation = self.isoforms[
                             check_across_isoforms.index(True)
                         ]
                         self.isoforms_to_model.append(
                             [isoform_for_mutation, mutation]
                         )
                         mutations_to_model.remove(mutation)
-            self._report_on_selected_isoforms()
 
             # Print the mutations with that cannot
             # be associated to any isoform
             if len(mutations_to_model) > 0:
                 print(
                     "The following mutations will not be"
                     " modelled for gene " + self.name
@@ -312,14 +309,24 @@
             content+="-- "+isoform.isoform_name+"\n"
             content+="--- Mutation:"
             content+=str(round(isoform.mutation_score,2))+" Structural:"
             content+=str(round(isoform.structural_score,2))+" Selection:"
             content+=str(round(isoform.selection_score,2))+"\n"
             content+="--- Modellable: "+str(isoform.modellable)+"\n"
             
+        #Add a list of mutations excluded due missing structural converage
+        non_covered_isoforms=[]
+        for isoform in self.isoforms_to_model:
+            if isoform[0].modeller_run.mutation_is_modellable==False:
+                non_covered_isoforms.append(isoform)
+        if len(non_covered_isoforms)>0:
+            content+="\nThe following mutations are in a region not covered by templates:\n"
+            for isoform in non_covered_isoforms:
+                content+="".join(isoform[1])+"\n"
+        
         content+="\n## MODELS\n"
         
         for isoform in self.isoforms_to_model:
             #isoform[0] is the object, isoform[1] is the mutation
             content+="- "+isoform[0].isoform_name+" "+"".join(isoform[1])+"\n"
             content+="- Templates: "
```

### Comparing `monviso-0.1.0/monviso_reloaded/input_parser.py` & `monviso-0.1.1/monviso_reloaded/input_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -169,15 +169,23 @@
 
         :param mutation_list: path to the file containing the list
         of mutations and genes
         :return: The list of gene and mutations
         """
         with Path(mutation_file_path).open() as my_file:
             content = my_file.read()
-
+            
+        
+        #Remove useless new lines
+        while content[-1]=="\n":
+            content=content[:-1]
+            
+        while "\n\n\n" in content:
+            content=content.replace('\n\n\n','\n\n')
+        
         blocks = [block.splitlines() for block in content.split("\n\n")]
         return blocks
 
     def get_parameters(
         self,
         parameters_path: argparse.Namespace = "parameters.dat",
     ) -> Dict:
```

### Comparing `monviso-0.1.0/monviso_reloaded/isoform.py` & `monviso-0.1.1/monviso_reloaded/isoform.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,29 +21,30 @@
         out_path: Union[str, Path],
         mutations: list,
     ):
         self.gene_name = gene_name
         self.isoform_index = isoform_index
         self.isoform_name = "isoform" + str(self.isoform_index)
         self.mutations = mutations
+        self.mutations_not_in_structure=[]
         self.first_line = sequence[0]
         self.sequence = sequence[1:]
         self.out_path = Path(out_path, self.isoform_name)
 
         # just for initialization
         self.mutation_score = 0
         self.structural_score = 0
         self.selection_score = 0
         self.templates = []
         self.modellable = True  # False if all templates get excluded
         self.aligned_sequence = ""
         self.clean_aligned_sequence=""
         
         self.modeller_run=None
-
+        
         self.create_directory()
         self.save_fasta_sequence()
 
     def create_directory(self) -> None:
         """Create an empty subdirectory with the isoform index
         at the output path specified by the user, and within
         the gene folder."""
@@ -55,14 +56,20 @@
 
         text_output = "\n".join([">" + self.first_line] + self.sequence)
         with FileHandler() as fh:
             fh.write_file(
                 Path(self.out_path, self.isoform_name + ".fasta"), text_output
             )
 
+    def _check_hmmer_errors(self,possible_templates_string):
+        if "Error" in possible_templates_string:
+            print("The hmmsearch for a template resulted in a server error.")
+            print("Monviso will quit.")
+            quit()
+
     def blastp_search(self) -> None:
         """Use the isoform.fasta file saved in the directory
         to start a Blastp search. If the file already exists,
         nothing is done.
         """
         print(
             f"Looking for homologues of {self.gene_name} {self.isoform_name}"
@@ -178,14 +185,15 @@
                         command,
                         shell=True,
                         universal_newlines=True,
                         capture_output=True,
                         check=True,
                     )
                     output = result.stdout  # Captured output as a string
+                    self._check_hmmer_errors(output)
                     fh.write_file(templates_path, output)
                 except subprocess.CalledProcessError as e:
                     print(f"Error executing curl command: {e}")
             else:
                 print(
                     f"Templates file for {self.gene_name} "
                     f"{self.isoform_name} esists. "
@@ -221,34 +229,35 @@
                 ]
                 templates_list = pdb_list[:max_pdb]
                 fh.write_file(top_templates_path, "\n".join(templates_list))
                 fh.write_file(pdb_list_path, "\n".join(pdb_list))
             templates_list = fh.read_file(top_templates_path).splitlines()
             return templates_list
 
-    def _template_alignment(self, cobalt_home: Union[str, Path]) -> None:
+    def _template_alignment(self, cobalt_home: Union[str, Path],redo=False) -> None:
         """Create a unique file with the templates sequences and
         run a cobalt MSA.
         Args:
             cobalt_home (Union[str,Path]): Home of the Cobalt program,
             where executables are stored.
+            redo: True if part of the scoring cycle. Alignment can be re-written
         """
         content = ">" + self.gene_name + " " + self.isoform_name + "\n"
         content += "".join(self.sequence) + "\n"
         for template in self.templates:
             content += (
                 ">" + template.pdb_name + "_" + template.pdb_chain + "\n"
             )
             content += template.sequence + "\n"
 
         with FileHandler() as fh:
             templates_path = Path(self.out_path, "templates_sequences.fasta")
             fh.write_file(templates_path, content)
             aligned_path = Path(self.out_path, "templates_aligned.fasta")
-            if fh.check_existence(aligned_path):
+            if fh.check_existence(aligned_path) and not redo:
                 print(
                     "Cobalt output file for templates "
                     "already present in folder."
                 )
             else:
                 with Cobalt() as cobalt:
                     cobalt.run(templates_path, aligned_path, cobalt_home)
@@ -471,13 +480,46 @@
             w2 (float): weight of the mutation score
         """
 
         self.selection_score = (
             w1 * self.structural_score + w2 * self.mutation_score
         )
 
-    def run_modeller(self, mutation, modeller_exec: str,model_cutoff:int):
+                    
+    def calculate_score(self,mappable_mutations,model_cutoff,sequence_identity_cutoff,w1,w2,cobalt_home):
+        """Starts a cycle to calculate the mutation, structural and selection scores.
+        The process is repeated in cycle because, after calculating the sequence identity,
+        the number of sequences, and thus the alignments might change. The cycle is repeated
+        untill these values stabilize on a fixed value. After every calculation of the 
+        sequence identy, a new alignment must be created with the filtered sequences.
+        *indirectly: while the list of templates changes, the cycle repeats
+        
+        Args:
+        - mappable mutations: A list of mutations that can be mapped on the sequence. 
+        - model_cutoff: The maximum number of gaps in a region without coverage. Larger
+        gaps are replaced by chain breaks.
+        - sequence_identity_cutoff: Sequences with a lower sequence identity will be skipped.
+        - w1 (float): weight of the structural score
+        - w2 (float): weight of the mutation score
+        """
+        last_template_list=[]
+        
+        while last_template_list!=[t.pdb_name+"_"+t.pdb_chain for t in self.templates]:
+            last_template_list=[t.pdb_name+"_"+t.pdb_chain for t in self.templates]
+            #TO DO
+            #Use of next function in self.load_templates should be avoided
+            self._template_alignment(cobalt_home,redo=True)
+            self.calculate_mutation_score(mappable_mutations)
+            self.calculate_structural_score(model_cutoff)
+            self.filter_templates_by_sequence_identity(
+                    sequence_identity_cutoff
+                )
+            self.calculate_selection_score(w1, w2)
+
+    def run_modeller(self, mutation, modeller_exec: str,model_cutoff:int,number_of_wt:int,number_of_mut:int,cobalt_home:str):
+        """Create the alignment and start the Modeller run."""
         self.modeller_run=Modeller_manager(
-            self, mutation, modeller_exec, model_cutoff)
+            self, mutation, modeller_exec, model_cutoff,number_of_wt,number_of_mut)
+
         
         self.modeller_run.write()
         self.modeller_run.run()
```

### Comparing `monviso-0.1.0/monviso_reloaded/modeller_manager.py` & `monviso-0.1.1/monviso_reloaded/modeller_manager.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,40 +2,66 @@
 import subprocess
 from pathlib import Path
 
 from .file_handler import FileHandler
 
 
 class Modeller_manager:
-    def __init__(self, isoform, mutation: list, modeller_exec: str, model_cutoff: int):
+    def __init__(self, isoform, mutation: list, modeller_exec: str, model_cutoff: int,
+                 number_of_wt:int,number_of_mut:int):
         self.isoform = isoform
         self.mutation = mutation
         self.sequence_to_model = self.isoform.aligned_sequence[:]
         self.modeller_exec = modeller_exec
         self.model_cutoff = model_cutoff
         self.logged_scores=[]
-
-    def __enter__(self):
-        return self
-
-    def __exit__(self, exc_type, exc_value, traceback):
-        pass
-
+        self.num_chains=1
+        self.chain_starts=[]
+        self.mutation_is_modellable=True
+        
+        if "".join(mutation)=="WT":
+            self.num_models=number_of_wt
+        else:
+            self.num_models=number_of_mut
     def write(self):
 
         print(
             f"Modelling {self.isoform.gene_name}"
             f" {self.isoform.isoform_name} "+"".join(self.mutation)
         )
-        if self.mutation != "WT":
-            success_mutation = self._mutate_reside(self.mutation)
-            if not success_mutation:
-                raise (RuntimeError("Could not apply mutation!"))
         self.write_alignment()
         self.write_script()
+    
+    def _check_modellability(self,sequence) -> bool:
+        """Sometimes the mutation can be mapped on the isoform, but it is not
+        in the range of the protein that is covered by the templates. The Gene
+        object that starts the modelling process, should be updated to stop the
+        modelling, and write and informed report.
+        
+        This function checks the mutation residue number in the sequence and returns
+        a boolean representing the presence of the mutated residue. 
+        
+        Args:
+        sequences (list): A list of [residue number, residue], with one element
+        for each residue of the target sequence, after adding chain breaks.
+        
+        Returns:
+        bool: Presence of the mutated residue in the final alignment."""
+        
+        if self.mutation=='WT':
+            return True
+        
+        resnum_to_mutate=int(self.mutation[1])
+        resnumbers=[r[0] for r in sequence]
+        self.mutation_is_modellable = resnum_to_mutate in resnumbers
+        
+        if not self.mutation_is_modellable:
+            self.isoform.mutations_not_in_structure.append(self.mutation)
+        
+        return self.mutation_is_modellable
 
     def write_script(self):
         alignment_name = "../modeller_input_" + "".join(self.mutation) + ".dat"
         output_name = "../modeller_output_" + "".join(self.mutation) + ".dat"
         script_path = Path(
             self.isoform.out_path,
             "run_modeller_" + "".join(self.mutation) + ".py",
@@ -45,31 +71,37 @@
             for t in self.isoform.templates
         ]
         content = (
             """from modeller import *
 from modeller.automodel import *
 from modeller.scripts import complete_pdb
 
+class MyModel(AutoModel):
+    def special_patches(self, aln):
+        # Rename both chains and renumber the residues in each
+        self.rename_segments(segment_ids="""+str(["A" for  i in range(self.num_chains)])+""",
+                             renumber_residues="""+str(self.chain_starts)+""")
+
 log.verbose()
 env = environ()
 env.io.atom_files_directory = '../templates/'
 env.io.hetatm = True
-a = automodel(env,
+a = MyModel(env,
     alnfile =\""""
             + alignment_name
             + """\",
     knowns = ("""
             + str(template_names)
             + """),
     sequence = \""""
             + self.isoform.gene_name
             + """\",
     assess_methods=(assess.DOPE, assess.GA341))
 a.starting_model= 1
-a.ending_model  = 1
+a.ending_model  = """+str(self.num_models)+"""
 a.make()
 ok_models = filter(lambda x: x['failure'] is None, a.outputs)
 toscore = 'DOPE score'
 ok_models = sorted(ok_models, key=lambda k: k[toscore])
 models = [m for m in ok_models[0:10]]
 myout = open(\""""
             + output_name
@@ -84,41 +116,73 @@
             + self.isoform.gene_name
             + """\", normalize_profile=True, smoothing_window=15)"""
         )
 
         with FileHandler() as fh:
             fh.write_file(script_path, content)
 
-    def _mutate_reside(self, mutation) -> bool:
+    def _mutate_reside(self, mutation, sequence:str) -> bool:
         """Take a mutation in the format
         [1 letter amino acid,residue number, 1 lett. amino acid]
         and apply it to the aligned sequence to model,
         taking into account all the "-"'s.
 
-        Returns True, if succesful, else False
+        Returns edited sequence
         """
+ 
+        if mutation=="WT":
+            return sequence
+        
+
         i = int(mutation[1]) - 1
-        while i < len(self.sequence_to_model):
-            actual_residue_index = i - self.sequence_to_model[:i].count("-")
+        while i < len(sequence):
+            actual_residue_index = i - sequence[:i].count("-")
             if (
                 actual_residue_index + 1 == int(mutation[1])
-            ) and self.sequence_to_model[i] == mutation[0]:
-                self.sequence_to_model = (
-                    self.sequence_to_model[:i]
+            ) and sequence[i] == mutation[0]:
+                sequence = (
+                    sequence[:i]
                     + mutation[2]
-                    + self.sequence_to_model[i + 1 :]
+                    + sequence[i + 1 :]
                 )
-                return True
+                return sequence
             i += 1
 
         print(f"Could not apply mutation {mutation}!")
-        return False
+        return sequence
 
+    def _add_number_to_sequence(self,sequence:str)->list:
+        """From a sequence, return a 2D list with [resnum,resiude]"""
+        numbered_seq=[]
+        i=1
+        for char in sequence:
+            if (char=="-"):
+                numbered_seq.append(["-",char])
+            else:
+                numbered_seq.append([i,char])
+                i+=1
+        return numbered_seq
+    
+    def _save_chain_starts(self,sequence_with_resnum:list)->None:
+        """Given a sequence saved as a list [resnum, residue],
+        save all the residue numbers that represent an interruption
+        in the continuity of the protein chain."""
+
+        #lists al resnums without gaps
+        filtered_numbers=[r[0] for r in sequence_with_resnum if r[0]!="-"]
+
+   
+        self.chain_starts.append(filtered_numbers[0])
+
+        for i in range(1,len(filtered_numbers)):
+            if filtered_numbers[i]!=filtered_numbers[i-1]+1:
+                self.chain_starts.append(filtered_numbers[i]-1)
+    
     def _add_chain_breaks(self, sequences: list) -> list:
-        """For alignments inw which there is no coverage for self.model_cutoff+
+        """For alignments in which there is no coverage for self.model_cutoff+
         residues, the section without coverage is replaced by
         chain breaks.
 
         Args:
             sequences (list): A list of [name, sequence] lists,
             one for each sequence to be written in the modeller
             alignment input file.
@@ -127,14 +191,16 @@
             list: Returns the same list, with chain breaks.
         """
 
         # Separate protein names and aligned sequences in two objects
         names = [object[0] for object in sequences]
         aligned_seq = [object[1] for object in sequences]
 
+        #Add object to keep trak of residue number in target seq
+        num_target_seq=self._add_number_to_sequence(aligned_seq[0])
         # Calculate worst case number of residues without coverage
         max_non_covered = max([seq.count("-") for seq in aligned_seq])
 
         # Search for non-covered subsequences with lenght between
         # max_non_covered and model_cutoff
         while max_non_covered >= self.model_cutoff:
 
@@ -158,65 +224,92 @@
                         == "-" * max_non_covered
                         for seq in aligned_seq[1:]
                     ]
                     if sum(check_position) == (len(aligned_seq) - 1):
                         # If that is the case, replace that section in
                         # all sequences (+ target sequences) with a chain
                         # break ("/").
+                        num_target_seq=num_target_seq[:pos]+num_target_seq[pos + max_non_covered :]
                         for i, seq in enumerate(aligned_seq):
                             aligned_seq[i] = (
-                                seq[:pos] + "/" + seq[pos + max_non_covered :]
-                            )
+                                seq[:pos] + "/" + seq[pos + max_non_covered :])
+                            self.num_chains+=1
 
                         max_non_covered += (
                             1  # This repeats the check for the current value
                         )
             max_non_covered -= 1
 
         sequences = [[names[i], aligned_seq[i]] for i in range(len(names))]
+        
+        #Remove "/" at the beginning or end of the sequences:
+        if sequences[0][1][0]=="/":
+            sequences=[[s[0],s[1][1:]] for s in sequences]
+        if sequences[0][1][-1]=="/":
+            sequences=[[s[0],s[1][:-1]] for s in sequences]
+        #Next line is to save resnum at chain breaks as local attributes
+        self._save_chain_starts(num_target_seq)
+        
+        #Next line is to check if mutation can still be mapped
+        _ =self._check_modellability(num_target_seq)
+        
         return sequences
 
     def write_alignment(self):
 
         alignment_name = "modeller_input_" + "".join(self.mutation) + ".dat"
         output_path = Path(self.isoform.out_path, alignment_name)
         # Create an object storing all names and aligned sequences
-        sequences = [[self.isoform.gene_name, self.sequence_to_model]]
-        for template in self.isoform.templates:
-            sequences.append(
-                [
-                    template.pdb_name + "_" + template.pdb_chain,
-                    template.aligned_sequence,
-                ]
-            )
-
+        sequences = []
+        with FileHandler() as fh:
+            file_path=Path(self.isoform.out_path,"templates_aligned.fasta")
+            aligned_sequence_file=fh.read_file(file_path)
+            aligned_sequences=aligned_sequence_file.split(">")[1:]
+            sequences=[[x.split("\n")[0].split()[-1],"".join(x.split('\n')[1:])] for x in aligned_sequences]
+
+        #Add mutation if needed
+        sequences[0][1]=self._mutate_reside(self.mutation,sequences[0][1])
+        
         # Add chain breaks in place of long seqs with no coverage
         sequences = self._add_chain_breaks(sequences)
 
+
         # Start writing the content string to be printed in the file
         content = ""
-        content += ">P1;" + sequences[0][0] + "\n"
-        content += "sequence:" + sequences[0][0] + ":.:.:.:.::::\n"
+        content += ">P1;" + self.isoform.gene_name + "\n"
+        content += "sequence:" + self.isoform.gene_name + ":.:.:.:.::::\n"
         content += sequences[0][1] + "*\n"
 
         # Add templates
         for template_sequence in sequences[1:]:
             content += ">P1;" + template_sequence[0] + "_clean" + "\n"
             content += (
                 "structureX:"
                 + template_sequence[0]
                 + "_clean"
                 + ":.:.:.:.::::\n"
             )
             content += template_sequence[1] + "*\n"
 
-        with FileHandler() as fh:
-            fh.write_file(output_path, content)
+        #After the last alignment it is know if the mutation
+        #Can be certainly applied. Apply last check before
+        #Writing
+        if self.mutation_is_modellable:
+            with FileHandler() as fh:
+                fh.write_file(output_path, content)
 
     def run(self) -> None:
+        
+        if self.mutation_is_modellable==False:
+            print("Modelling of mutation "+"".join(self.mutation)+
+                  " was eexcluded on "+self.isoform.gene_name+" "+
+                  self.isoform.isoform_name+" due to missing coverage.")
+            self.load_log_file()
+            return None
+        
         model_path = Path(
             self.isoform.out_path,
             self.isoform.gene_name + "_" + "".join(self.mutation) + "_model",
         )
         with FileHandler() as fh:
             fh.create_directory(model_path)
         home_working_directory = os.getcwd()
@@ -229,16 +322,22 @@
         os.chdir(home_working_directory)
         self.load_log_file()
 
     def load_log_file(self):
         """ Open the log file after the run of modeller.
         Look for the table with the DOPE scores.
         Save it as attribute (list).
+        
+        But if the mutation is not modellable, due to missing template
+        converage, just save a warning string as attribute.
         """
-        with FileHandler() as fh:
-            log_path = Path(self.isoform.out_path,"run_modeller_" + "".join(self.mutation) + ".log")
-            logs=fh.read_file(log_path).splitlines()
-            
-            table_start_index=logs.index("Filename                          molpdf     DOPE score    GA341 score")
-            table_end_index=table_start_index+logs[table_start_index:].index("")
-            
-            self.logged_scores=logs[table_start_index:table_end_index]
+        if self.mutation_is_modellable:
+            with FileHandler() as fh:
+                log_path = Path(self.isoform.out_path,"run_modeller_" + "".join(self.mutation) + ".log")
+                logs=fh.read_file(log_path).splitlines()
+                
+                table_start_index=logs.index("Filename                          molpdf     DOPE score    GA341 score")
+                table_end_index=table_start_index+logs[table_start_index:].index("")
+                
+                self.logged_scores=logs[table_start_index:table_end_index]
+        else:
+            self.logged_scores=["! The mutation was not modelled, due to missing templates for that region."]
```

### Comparing `monviso-0.1.0/monviso_reloaded/template.py` & `monviso-0.1.1/monviso_reloaded/template.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.0/setup.py` & `monviso-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     name="monviso",
     python_requires='>=3.9',
     version=read("monviso_reloaded", "VERSION"),
     description="MoNvIso is a comprehensive software tool designed for the analysis and modeling of protein isoforms. It automates the process of identifying canonical and additional isoforms, assessing their modeling propensity, mapping mutations accurately, and building structural models of proteins.",
     url="https://github.com/alisamalb/monviso_reloaded",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
-    author=["alisamalb","Ciskio"],
+    author="Ciskio",
     packages=find_packages(exclude=["tests", ".github"]),
     install_requires=read_requirements("requirements.txt"),
     entry_points={
         "console_scripts": ["monviso_reloaded = monviso_reloaded.__main__:main"]
     },
     extras_require={"test": read_requirements("requirements-test.txt")},
 )
```

