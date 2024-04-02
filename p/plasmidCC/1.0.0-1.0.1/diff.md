# Comparing `tmp/plasmidCC-1.0.0.tar.gz` & `tmp/plasmidCC-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plasmidCC-1.0.0.tar", last modified: Mon Mar 25 12:39:35 2024, max compression
+gzip compressed data, was "plasmidCC-1.0.1.tar", last modified: Tue Apr  2 10:40:57 2024, max compression
```

## Comparing `plasmidCC-1.0.0.tar` & `plasmidCC-1.0.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0 oscar     (1000) oscar     (1000)        0 2024-03-25 12:39:35.185843 plasmidCC-1.0.0/
--rwxrwxrwx   0 oscar     (1000) oscar     (1000)     1624 2024-03-25 12:20:36.000000 plasmidCC-1.0.0/.gitignore
--rwxrwxrwx   0 oscar     (1000) oscar     (1000)     1072 2024-03-25 12:20:36.000000 plasmidCC-1.0.0/LICENSE
--rwxrwxrwx   0 oscar     (1000) oscar     (1000)     8396 2024-03-25 12:39:35.184247 plasmidCC-1.0.0/PKG-INFO
--rwxrwxrwx   0 oscar     (1000) oscar     (1000)     8081 2024-03-25 12:20:36.000000 plasmidCC-1.0.0/README.md
-drwxrwxrwx   0 oscar     (1000) oscar     (1000)        0 2024-03-25 12:39:35.088064 plasmidCC-1.0.0/plasmidCC/
--rwxrwxrwx   0 oscar     (1000) oscar     (1000)        0 2024-03-25 12:20:36.000000 plasmidCC-1.0.0/plasmidCC/__init__.py
-drwxrwxrwx   0 oscar     (1000) oscar     (1000)        0 2024-03-25 12:39:35.130745 plasmidCC-1.0.0/plasmidCC/databases/
--rwxrwxrwx   0 oscar     (1000) oscar     (1000)        0 2024-03-25 12:20:36.000000 plasmidCC-1.0.0/plasmidCC/databases/.gitkeep
--rwxrwxrwx   0 oscar     (1000) oscar     (1000)     8085 2024-03-25 12:20:36.000000 plasmidCC-1.0.0/plasmidCC/plasmid_CC.py
-drwxrwxrwx   0 oscar     (1000) oscar     (1000)        0 2024-03-25 12:39:35.158007 plasmidCC-1.0.0/plasmidCC/scripts/
--rwxrwxrwx   0 oscar     (1000) oscar     (1000)       16 2024-03-25 12:20:36.000000 plasmidCC-1.0.0/plasmidCC/scripts/__init__.py
--rwxrwxrwx   0 oscar     (1000) oscar     (1000)     2146 2024-03-25 12:20:36.000000 plasmidCC-1.0.0/plasmidCC/scripts/download_centrifuge_db.py
--rwxrwxrwx   0 oscar     (1000) oscar     (1000)     2048 2024-03-25 12:20:36.000000 plasmidCC-1.0.0/plasmidCC/scripts/extract_nodes.py
--rwxrwxrwx   0 oscar     (1000) oscar     (1000)     4360 2024-03-25 12:20:36.000000 plasmidCC-1.0.0/plasmidCC/scripts/process_centrifuge.py
--rwxrwxrwx   0 oscar     (1000) oscar     (1000)     1045 2024-03-25 12:20:36.000000 plasmidCC-1.0.0/plasmidCC/scripts/run_centrifuge.py
--rwxrwxrwx   0 oscar     (1000) oscar     (1000)     3570 2024-03-25 12:20:36.000000 plasmidCC-1.0.0/plasmidCC/scripts/utils.py
--rwxrwxrwx   0 oscar     (1000) oscar     (1000)      411 2024-03-25 12:39:34.000000 plasmidCC-1.0.0/plasmidCC/version.py
-drwxrwxrwx   0 oscar     (1000) oscar     (1000)        0 2024-03-25 12:39:35.181392 plasmidCC-1.0.0/plasmidCC.egg-info/
--rwxrwxrwx   0 oscar     (1000) oscar     (1000)     8396 2024-03-25 12:39:34.000000 plasmidCC-1.0.0/plasmidCC.egg-info/PKG-INFO
--rwxrwxrwx   0 oscar     (1000) oscar     (1000)      582 2024-03-25 12:39:34.000000 plasmidCC-1.0.0/plasmidCC.egg-info/SOURCES.txt
--rwxrwxrwx   0 oscar     (1000) oscar     (1000)        1 2024-03-25 12:39:34.000000 plasmidCC-1.0.0/plasmidCC.egg-info/dependency_links.txt
--rwxrwxrwx   0 oscar     (1000) oscar     (1000)       56 2024-03-25 12:39:34.000000 plasmidCC-1.0.0/plasmidCC.egg-info/entry_points.txt
--rwxrwxrwx   0 oscar     (1000) oscar     (1000)       72 2024-03-25 12:39:34.000000 plasmidCC-1.0.0/plasmidCC.egg-info/requires.txt
--rwxrwxrwx   0 oscar     (1000) oscar     (1000)       10 2024-03-25 12:39:34.000000 plasmidCC-1.0.0/plasmidCC.egg-info/top_level.txt
--rwxrwxrwx   0 oscar     (1000) oscar     (1000)       72 2024-03-25 12:20:36.000000 plasmidCC-1.0.0/requirements.txt
--rwxrwxrwx   0 oscar     (1000) oscar     (1000)       38 2024-03-25 12:39:35.189548 plasmidCC-1.0.0/setup.cfg
--rwxrwxrwx   0 oscar     (1000) oscar     (1000)      861 2024-03-25 12:20:36.000000 plasmidCC-1.0.0/setup.py
-drwxrwxrwx   0 oscar     (1000) oscar     (1000)        0 2024-03-25 12:39:35.160514 plasmidCC-1.0.0/test/
--rwxrwxrwx   0 oscar     (1000) oscar     (1000)  5033578 2024-03-25 12:20:36.000000 plasmidCC-1.0.0/test/test_ecoli.gfa
+drwxrwxr-x   0 aschuerch  (1001) aschuerch  (1001)        0 2024-04-02 10:40:57.413804 plasmidCC-1.0.1/
+-rw-rw-r--   0 aschuerch  (1001) aschuerch  (1001)     1624 2024-04-02 10:37:26.000000 plasmidCC-1.0.1/.gitignore
+-rw-rw-r--   0 aschuerch  (1001) aschuerch  (1001)     1072 2024-04-02 10:37:26.000000 plasmidCC-1.0.1/LICENSE
+-rw-r--r--   0 aschuerch  (1001) aschuerch  (1001)     8490 2024-04-02 10:40:57.413804 plasmidCC-1.0.1/PKG-INFO
+-rw-rw-r--   0 aschuerch  (1001) aschuerch  (1001)     8175 2024-04-02 10:37:26.000000 plasmidCC-1.0.1/README.md
+drwxrwxr-x   0 aschuerch  (1001) aschuerch  (1001)        0 2024-04-02 10:40:57.397804 plasmidCC-1.0.1/plasmidCC/
+-rw-rw-r--   0 aschuerch  (1001) aschuerch  (1001)        0 2023-12-19 12:57:13.000000 plasmidCC-1.0.1/plasmidCC/__init__.py
+drwxrwxr-x   0 aschuerch  (1001) aschuerch  (1001)        0 2024-04-02 10:40:57.397804 plasmidCC-1.0.1/plasmidCC/databases/
+-rw-rw-r--   0 aschuerch  (1001) aschuerch  (1001)        0 2024-04-02 10:37:26.000000 plasmidCC-1.0.1/plasmidCC/databases/.gitkeep
+-rw-rw-r--   0 aschuerch  (1001) aschuerch  (1001)     8174 2024-04-02 10:37:26.000000 plasmidCC-1.0.1/plasmidCC/plasmid_CC.py
+drwxrwxr-x   0 aschuerch  (1001) aschuerch  (1001)        0 2024-04-02 10:40:57.401804 plasmidCC-1.0.1/plasmidCC/scripts/
+-rw-rw-r--   0 aschuerch  (1001) aschuerch  (1001)       16 2024-04-02 10:37:26.000000 plasmidCC-1.0.1/plasmidCC/scripts/__init__.py
+-rw-rw-r--   0 aschuerch  (1001) aschuerch  (1001)     2146 2024-04-02 10:37:26.000000 plasmidCC-1.0.1/plasmidCC/scripts/download_centrifuge_db.py
+-rw-rw-r--   0 aschuerch  (1001) aschuerch  (1001)     2048 2024-04-02 10:37:26.000000 plasmidCC-1.0.1/plasmidCC/scripts/extract_nodes.py
+-rw-rw-r--   0 aschuerch  (1001) aschuerch  (1001)     4360 2024-04-02 10:37:26.000000 plasmidCC-1.0.1/plasmidCC/scripts/process_centrifuge.py
+-rw-rw-r--   0 aschuerch  (1001) aschuerch  (1001)     1045 2024-04-02 10:37:26.000000 plasmidCC-1.0.1/plasmidCC/scripts/run_centrifuge.py
+-rw-rw-r--   0 aschuerch  (1001) aschuerch  (1001)     3570 2024-04-02 10:37:26.000000 plasmidCC-1.0.1/plasmidCC/scripts/utils.py
+-rw-rw-r--   0 aschuerch  (1001) aschuerch  (1001)      411 2024-04-02 10:40:57.000000 plasmidCC-1.0.1/plasmidCC/version.py
+drwxrwxr-x   0 aschuerch  (1001) aschuerch  (1001)        0 2024-04-02 10:40:57.413804 plasmidCC-1.0.1/plasmidCC.egg-info/
+-rw-r--r--   0 aschuerch  (1001) aschuerch  (1001)     8490 2024-04-02 10:40:57.000000 plasmidCC-1.0.1/plasmidCC.egg-info/PKG-INFO
+-rw-rw-r--   0 aschuerch  (1001) aschuerch  (1001)      582 2024-04-02 10:40:57.000000 plasmidCC-1.0.1/plasmidCC.egg-info/SOURCES.txt
+-rw-rw-r--   0 aschuerch  (1001) aschuerch  (1001)        1 2024-04-02 10:40:57.000000 plasmidCC-1.0.1/plasmidCC.egg-info/dependency_links.txt
+-rw-rw-r--   0 aschuerch  (1001) aschuerch  (1001)       56 2024-04-02 10:40:57.000000 plasmidCC-1.0.1/plasmidCC.egg-info/entry_points.txt
+-rw-rw-r--   0 aschuerch  (1001) aschuerch  (1001)       72 2024-04-02 10:40:57.000000 plasmidCC-1.0.1/plasmidCC.egg-info/requires.txt
+-rw-rw-r--   0 aschuerch  (1001) aschuerch  (1001)       10 2024-04-02 10:40:57.000000 plasmidCC-1.0.1/plasmidCC.egg-info/top_level.txt
+-rw-rw-r--   0 aschuerch  (1001) aschuerch  (1001)       72 2024-04-02 10:37:26.000000 plasmidCC-1.0.1/requirements.txt
+-rw-rw-r--   0 aschuerch  (1001) aschuerch  (1001)       38 2024-04-02 10:40:57.413804 plasmidCC-1.0.1/setup.cfg
+-rw-rw-r--   0 aschuerch  (1001) aschuerch  (1001)      861 2024-04-02 10:37:26.000000 plasmidCC-1.0.1/setup.py
+drwxrwxr-x   0 aschuerch  (1001) aschuerch  (1001)        0 2024-04-02 10:40:57.401804 plasmidCC-1.0.1/test/
+-rw-rw-r--   0 aschuerch  (1001) aschuerch  (1001)  5033578 2024-04-02 10:37:26.000000 plasmidCC-1.0.1/test/test_ecoli.gfa
```

### Comparing `plasmidCC-1.0.0/.gitignore` & `plasmidCC-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `plasmidCC-1.0.0/LICENSE` & `plasmidCC-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `plasmidCC-1.0.0/PKG-INFO` & `plasmidCC-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plasmidCC
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Centrifuge based plasmid prediction tool
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: biopython>=1.83
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: pandas>=2.2.0
 Requires-Dist: rich>=13.7.0
@@ -110,15 +110,16 @@
 Parameters:
   -l LENGTH             Minimum sequence length filter (default: 1000)
   -t THREADS            Number of alignment threads to launch (default: 8)
   -P PLASMID_CUTOFF     Threshold of plasmid fraction to predict contig as plasmid (default: 0.7)
   -C CHROMOSOME_CUTOFF  Threshold of plasmid fraction to predict contig as chromosome (default: 0.3)
 
 Other:
-  -D, --download        Download embedded database if not yet downloaded
+  -D, --download        Download embedded database if not yet downloaded.
+                        Embedded databases are stored within the plasmidCC package directory
   -g, --gplas           Write an extra output file that is compatible for use with gplas
   -f, --force           Overwrite existing output if the same name is already used
   -k, --keep            Keep intermediary files
 
 Info:
   --speciesopts         Prints a list of all supported species for the -s flag
   -v, --version         Prints plasmidCC version
```

### Comparing `plasmidCC-1.0.0/README.md` & `plasmidCC-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,16 @@
 Parameters:
   -l LENGTH             Minimum sequence length filter (default: 1000)
   -t THREADS            Number of alignment threads to launch (default: 8)
   -P PLASMID_CUTOFF     Threshold of plasmid fraction to predict contig as plasmid (default: 0.7)
   -C CHROMOSOME_CUTOFF  Threshold of plasmid fraction to predict contig as chromosome (default: 0.3)
 
 Other:
-  -D, --download        Download embedded database if not yet downloaded
+  -D, --download        Download embedded database if not yet downloaded.
+                        Embedded databases are stored within the plasmidCC package directory
   -g, --gplas           Write an extra output file that is compatible for use with gplas
   -f, --force           Overwrite existing output if the same name is already used
   -k, --keep            Keep intermediary files
 
 Info:
   --speciesopts         Prints a list of all supported species for the -s flag
   -v, --version         Prints plasmidCC version
```

### Comparing `plasmidCC-1.0.0/plasmidCC/plasmid_CC.py` & `plasmidCC-1.0.1/plasmidCC/plasmid_CC.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     paramgroup.add_argument('-l', dest='length', type=int, default=1000, help="Minimum sequence length filter (default: %(default)s)")
     paramgroup.add_argument('-t', dest='threads', type=int, default=8, help="Number of alignment threads to launch (default: %(default)s)")
     paramgroup.add_argument('-P', dest='plasmid_cutoff', type=float, default=0.7, help="Threshold of plasmid fraction to predict contig as plasmid (default: %(default)s)")
     paramgroup.add_argument('-C', dest='chromosome_cutoff', type=float, default=0.3, help="Threshold of plasmid fraction to predict contig as chromosome (default: %(default)s)")
 
     # Utility options
     othergroup = parser.add_argument_group('Other')
-    othergroup.add_argument('-D', '--download', action='store_true', help="Download embedded database if not yet downloaded")
+    othergroup.add_argument('-D', '--download', action='store_true', help=f"Download embedded database if not yet downloaded. Embedded databases are stored within the plasmidCC package directory: {default_db_dir}")
     othergroup.add_argument('-g', '--gplas', action='store_true', help="Write an extra output file that is compatible for use with gplas")
     othergroup.add_argument('-f', '--force', action='store_true', help="Overwrite existing output if the same name is already used")
     othergroup.add_argument('-k', '--keep', action='store_true', help="Keep intermediary files")
 
     # plasmidCC version and usage info
     infogroup = parser.add_argument_group('Info')
     infogroup.add_argument('--speciesopts', action='printing', nargs=0, help="Prints a list of all supported species for the -s flag")
```

### Comparing `plasmidCC-1.0.0/plasmidCC/scripts/download_centrifuge_db.py` & `plasmidCC-1.0.1/plasmidCC/scripts/download_centrifuge_db.py`

 * *Files identical despite different names*

### Comparing `plasmidCC-1.0.0/plasmidCC/scripts/extract_nodes.py` & `plasmidCC-1.0.1/plasmidCC/scripts/extract_nodes.py`

 * *Files identical despite different names*

### Comparing `plasmidCC-1.0.0/plasmidCC/scripts/process_centrifuge.py` & `plasmidCC-1.0.1/plasmidCC/scripts/process_centrifuge.py`

 * *Files identical despite different names*

### Comparing `plasmidCC-1.0.0/plasmidCC/scripts/run_centrifuge.py` & `plasmidCC-1.0.1/plasmidCC/scripts/run_centrifuge.py`

 * *Files identical despite different names*

### Comparing `plasmidCC-1.0.0/plasmidCC/scripts/utils.py` & `plasmidCC-1.0.1/plasmidCC/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `plasmidCC-1.0.0/plasmidCC.egg-info/PKG-INFO` & `plasmidCC-1.0.1/plasmidCC.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plasmidCC
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Centrifuge based plasmid prediction tool
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: biopython>=1.83
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: pandas>=2.2.0
 Requires-Dist: rich>=13.7.0
@@ -110,15 +110,16 @@
 Parameters:
   -l LENGTH             Minimum sequence length filter (default: 1000)
   -t THREADS            Number of alignment threads to launch (default: 8)
   -P PLASMID_CUTOFF     Threshold of plasmid fraction to predict contig as plasmid (default: 0.7)
   -C CHROMOSOME_CUTOFF  Threshold of plasmid fraction to predict contig as chromosome (default: 0.3)
 
 Other:
-  -D, --download        Download embedded database if not yet downloaded
+  -D, --download        Download embedded database if not yet downloaded.
+                        Embedded databases are stored within the plasmidCC package directory
   -g, --gplas           Write an extra output file that is compatible for use with gplas
   -f, --force           Overwrite existing output if the same name is already used
   -k, --keep            Keep intermediary files
 
 Info:
   --speciesopts         Prints a list of all supported species for the -s flag
   -v, --version         Prints plasmidCC version
```

### Comparing `plasmidCC-1.0.0/plasmidCC.egg-info/SOURCES.txt` & `plasmidCC-1.0.1/plasmidCC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plasmidCC-1.0.0/setup.py` & `plasmidCC-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `plasmidCC-1.0.0/test/test_ecoli.gfa` & `plasmidCC-1.0.1/test/test_ecoli.gfa`

 * *Files identical despite different names*

