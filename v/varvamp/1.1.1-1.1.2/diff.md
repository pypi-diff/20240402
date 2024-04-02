# Comparing `tmp/varvamp-1.1.1.tar.gz` & `tmp/varvamp-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varvamp-1.1.1.tar", last modified: Fri Jan 26 14:03:47 2024, max compression
+gzip compressed data, was "varvamp-1.1.2.tar", last modified: Tue Apr  2 12:29:03 2024, max compression
```

## Comparing `varvamp-1.1.1.tar` & `varvamp-1.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 14:03:47.156256 varvamp-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-01-26 14:03:47.156256 varvamp-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-01-26 14:03:32.000000 varvamp-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-26 14:03:47.156256 varvamp-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-01-26 14:03:32.000000 varvamp-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 14:03:47.152256 varvamp-1.1.1/varvamp/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-01-26 14:03:32.000000 varvamp-1.1.1/varvamp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-01-26 14:03:32.000000 varvamp-1.1.1/varvamp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18445 2024-01-26 14:03:32.000000 varvamp-1.1.1/varvamp/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 14:03:47.152256 varvamp-1.1.1/varvamp/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-01-26 14:03:32.000000 varvamp-1.1.1/varvamp/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7317 2024-01-26 14:03:32.000000 varvamp-1.1.1/varvamp/scripts/alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     9705 2024-01-26 14:03:32.000000 varvamp-1.1.1/varvamp/scripts/blast.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-01-26 14:03:32.000000 varvamp-1.1.1/varvamp/scripts/consensus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-01-26 14:03:32.000000 varvamp-1.1.1/varvamp/scripts/default_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-01-26 14:03:32.000000 varvamp-1.1.1/varvamp/scripts/get_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    20528 2024-01-26 14:03:32.000000 varvamp-1.1.1/varvamp/scripts/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-01-26 14:03:32.000000 varvamp-1.1.1/varvamp/scripts/param_estimation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13428 2024-01-26 14:03:32.000000 varvamp-1.1.1/varvamp/scripts/primers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14483 2024-01-26 14:03:32.000000 varvamp-1.1.1/varvamp/scripts/qpcr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-01-26 14:03:32.000000 varvamp-1.1.1/varvamp/scripts/regions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21338 2024-01-26 14:03:32.000000 varvamp-1.1.1/varvamp/scripts/reporting.py
--rw-r--r--   0 runner    (1001) docker     (127)    15229 2024-01-26 14:03:32.000000 varvamp-1.1.1/varvamp/scripts/scheme.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 14:03:47.156256 varvamp-1.1.1/varvamp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-01-26 14:03:47.000000 varvamp-1.1.1/varvamp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-01-26 14:03:47.000000 varvamp-1.1.1/varvamp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 14:03:47.000000 varvamp-1.1.1/varvamp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-26 14:03:47.000000 varvamp-1.1.1/varvamp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 14:03:47.000000 varvamp-1.1.1/varvamp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-26 14:03:47.000000 varvamp-1.1.1/varvamp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-26 14:03:47.000000 varvamp-1.1.1/varvamp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:29:03.807459 varvamp-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-04-02 12:29:03.807459 varvamp-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-04-02 12:28:55.000000 varvamp-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 12:29:03.807459 varvamp-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-02 12:28:55.000000 varvamp-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:29:03.803459 varvamp-1.1.2/varvamp/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-02 12:28:55.000000 varvamp-1.1.2/varvamp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-02 12:28:55.000000 varvamp-1.1.2/varvamp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18516 2024-04-02 12:28:55.000000 varvamp-1.1.2/varvamp/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:29:03.807459 varvamp-1.1.2/varvamp/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-02 12:28:55.000000 varvamp-1.1.2/varvamp/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7317 2024-04-02 12:28:55.000000 varvamp-1.1.2/varvamp/scripts/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9705 2024-04-02 12:28:55.000000 varvamp-1.1.2/varvamp/scripts/blast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-02 12:28:55.000000 varvamp-1.1.2/varvamp/scripts/consensus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-02 12:28:55.000000 varvamp-1.1.2/varvamp/scripts/default_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-02 12:28:55.000000 varvamp-1.1.2/varvamp/scripts/get_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20624 2024-04-02 12:28:55.000000 varvamp-1.1.2/varvamp/scripts/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-02 12:28:55.000000 varvamp-1.1.2/varvamp/scripts/param_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13428 2024-04-02 12:28:55.000000 varvamp-1.1.2/varvamp/scripts/primers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14483 2024-04-02 12:28:55.000000 varvamp-1.1.2/varvamp/scripts/qpcr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-02 12:28:55.000000 varvamp-1.1.2/varvamp/scripts/regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21338 2024-04-02 12:28:55.000000 varvamp-1.1.2/varvamp/scripts/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15229 2024-04-02 12:28:55.000000 varvamp-1.1.2/varvamp/scripts/scheme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:29:03.807459 varvamp-1.1.2/varvamp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-04-02 12:29:03.000000 varvamp-1.1.2/varvamp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-02 12:29:03.000000 varvamp-1.1.2/varvamp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 12:29:03.000000 varvamp-1.1.2/varvamp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-02 12:29:03.000000 varvamp-1.1.2/varvamp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 12:29:03.000000 varvamp-1.1.2/varvamp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-02 12:29:03.000000 varvamp-1.1.2/varvamp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 12:29:03.000000 varvamp-1.1.2/varvamp.egg-info/top_level.txt
```

### Comparing `varvamp-1.1.1/PKG-INFO` & `varvamp-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varvamp
-Version: 1.1.1
+Version: 1.1.2
 Summary: Variable VirusAMPlicons (varVAMP) is a tool to design primers for highly diverse viruses
 Home-page: https://github.com/jonas-fuchs/varVAMP
 Author: Dr. Jonas Fuchs
 Author-email: jonas.fuchs@uniklinik-freiburg.de
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.9
```

### Comparing `varvamp-1.1.1/README.md` & `varvamp-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `varvamp-1.1.1/setup.py` & `varvamp-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `varvamp-1.1.1/varvamp/command.py` & `varvamp-1.1.2/varvamp/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,16 +176,19 @@
     preprocessed_alignment = alignment.preprocess(args.input[0])
     # check alignment length distribution
     logging.check_alignment_length(preprocessed_alignment, log_file)
 
     # estimate threshold or number of ambiguous bases if args were not supplied
     if args.threshold is None or args.n_ambig is None:
         args.threshold, args.n_ambig = param_estimation.get_parameters(preprocessed_alignment, args, log_file)
-    if args.mode == "qpcr" and args.n_ambig >= 1 and args.pn_ambig is None:
-        args.pn_ambig = args.n_ambig - 1
+    if args.mode == "qpcr" and args.pn_ambig is None:
+        if args.n_ambig == 0:
+            args.pn_ambig = 0
+        if args.n_ambig > 0:
+            args.pn_ambig = args.n_ambig - 1
         with open(log_file, "a") as f:
             print(f"Automatic parameter selection set -pa {args.pn_ambig}.", file=f)
 
     # check arguments
     logging.raise_arg_errors(args, log_file)
 
     # config check
```

### Comparing `varvamp-1.1.1/varvamp/scripts/alignment.py` & `varvamp-1.1.2/varvamp/scripts/alignment.py`

 * *Files identical despite different names*

### Comparing `varvamp-1.1.1/varvamp/scripts/blast.py` & `varvamp-1.1.2/varvamp/scripts/blast.py`

 * *Files identical despite different names*

### Comparing `varvamp-1.1.1/varvamp/scripts/consensus.py` & `varvamp-1.1.2/varvamp/scripts/consensus.py`

 * *Files identical despite different names*

### Comparing `varvamp-1.1.1/varvamp/scripts/default_config.py` & `varvamp-1.1.2/varvamp/scripts/default_config.py`

 * *Files identical despite different names*

### Comparing `varvamp-1.1.1/varvamp/scripts/get_config.py` & `varvamp-1.1.2/varvamp/scripts/get_config.py`

 * *Files identical despite different names*

### Comparing `varvamp-1.1.1/varvamp/scripts/logging.py` & `varvamp-1.1.2/varvamp/scripts/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,15 +169,15 @@
                 "your intended overlap is higher than half of your optimal length. This reduces how well varvamps will find overlapping amplicons. Consider decreasing.",
                 log_file
             )
     # QPCR specific warnings
     if args.mode == "qpcr":
         if args.pn_ambig < 0:
             raise_error(
-                "number of ambiguous characters in the qPCR probe cannot be 0.",
+                "number of ambiguous characters in the qPCR probe cannot be negative.",
                 log_file,
                 exit=True
             )
         if args.pn_ambig > args.n_ambig:
             raise_error(
                 "the degeneracy of qPCR probes should not be higher than that of qPCR primers to retain specificity",
                 log_file,
@@ -279,14 +279,15 @@
             "QPROBE_TMP",
             "QPROBE_SIZES",
             "QPROBE_GC_RANGE",
             "QPROBE_GC_END",
             "QPRIMER_DIFF",
             "QPROBE_TEMP_DIFF",
             "QPROBE_DISTANCE",
+            "END_OVERLAP",
             "QAMPLICON_LENGTH",
             "QAMPLICON_GC",
             "QAMPLICON_DEL_CUTOFF"
         ),
         (
             "BLAST_MAX_DIFF",
             "BLAST_SIZE_MULTI",
@@ -375,14 +376,15 @@
         ("dNTP concentration", config.PCR_DNTP_CONC),
         ("primer temperature penalty", config.PRIMER_TM_PENALTY),
         ("primer gc penalty", config.PRIMER_GC_PENALTY),
         ("primer size penalty", config.PRIMER_SIZE_PENALTY),
         ("max base penalty", config.PRIMER_MAX_BASE_PENALTY),
         ("primer permutation penalty", config.PRIMER_PERMUTATION_PENALTY),
         ("qpcr flanking primer difference", config.QPRIMER_DIFF),
+        ("probe and primer end overlap", config.END_OVERLAP),
         ("qpcr deletion size still considered for deltaG calculation", config.QAMPLICON_DEL_CUTOFF),
         ("maximum difference between primer and blast db", config.BLAST_MAX_DIFF),
         ("multiplier of the maximum length for non-specific amplicons", config.BLAST_SIZE_MULTI),
         ("blast penalty for off targets", config.BLAST_PENALTY)
     ]
     for var_type, var in non_negative_var:
         if var < 0:
```

### Comparing `varvamp-1.1.1/varvamp/scripts/param_estimation.py` & `varvamp-1.1.2/varvamp/scripts/param_estimation.py`

 * *Files identical despite different names*

### Comparing `varvamp-1.1.1/varvamp/scripts/primers.py` & `varvamp-1.1.2/varvamp/scripts/primers.py`

 * *Files identical despite different names*

### Comparing `varvamp-1.1.1/varvamp/scripts/qpcr.py` & `varvamp-1.1.2/varvamp/scripts/qpcr.py`

 * *Files identical despite different names*

### Comparing `varvamp-1.1.1/varvamp/scripts/regions.py` & `varvamp-1.1.2/varvamp/scripts/regions.py`

 * *Files identical despite different names*

### Comparing `varvamp-1.1.1/varvamp/scripts/reporting.py` & `varvamp-1.1.2/varvamp/scripts/reporting.py`

 * *Files identical despite different names*

### Comparing `varvamp-1.1.1/varvamp/scripts/scheme.py` & `varvamp-1.1.2/varvamp/scripts/scheme.py`

 * *Files identical despite different names*

### Comparing `varvamp-1.1.1/varvamp.egg-info/PKG-INFO` & `varvamp-1.1.2/varvamp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varvamp
-Version: 1.1.1
+Version: 1.1.2
 Summary: Variable VirusAMPlicons (varVAMP) is a tool to design primers for highly diverse viruses
 Home-page: https://github.com/jonas-fuchs/varVAMP
 Author: Dr. Jonas Fuchs
 Author-email: jonas.fuchs@uniklinik-freiburg.de
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.9
```

### Comparing `varvamp-1.1.1/varvamp.egg-info/SOURCES.txt` & `varvamp-1.1.2/varvamp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

