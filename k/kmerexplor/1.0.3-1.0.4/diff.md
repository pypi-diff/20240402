# Comparing `tmp/kmerexplor-1.0.3.tar.gz` & `tmp/kmerexplor-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmerexplor-1.0.3.tar", last modified: Tue Mar 26 10:56:40 2024, max compression
+gzip compressed data, was "kmerexplor-1.0.4.tar", last modified: Tue Apr  2 07:01:43 2024, max compression
```

## Comparing `kmerexplor-1.0.3.tar` & `kmerexplor-1.0.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2024-03-26 10:56:40.829586 kmerexplor-1.0.3/
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)      212 2023-07-19 12:51:29.000000 kmerexplor-1.0.3/MANIFEST.in
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)    14032 2024-03-26 10:56:40.825218 kmerexplor-1.0.3/PKG-INFO
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)    11137 2024-03-25 08:29:20.000000 kmerexplor-1.0.3/README.md
-drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2024-03-26 10:56:40.598492 kmerexplor-1.0.3/kmerexplor/
--rwxrwxr-x   0 benoit    (1017) bio2m     (1010)      115 2023-07-19 12:51:29.000000 kmerexplor-1.0.3/kmerexplor/__init__.py
--rwxrwxr-x   0 benoit    (1017) bio2m     (1010)     2478 2023-07-19 12:51:29.000000 kmerexplor-1.0.3/kmerexplor/checkFile.py
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)     1088 2024-03-25 08:29:20.000000 kmerexplor-1.0.3/kmerexplor/common.py
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)    11533 2024-03-13 11:14:24.000000 kmerexplor-1.0.3/kmerexplor/config.yaml
--rwxrwxr-x   0 benoit    (1017) bio2m     (1010)     6768 2024-03-25 08:29:20.000000 kmerexplor-1.0.3/kmerexplor/core.py
--rwxrwxr-x   0 benoit    (1017) bio2m     (1010)    89080 2023-07-19 12:51:29.000000 kmerexplor-1.0.3/kmerexplor/countTags
--rwxrwxr-x   0 benoit    (1017) bio2m     (1010)    14740 2024-03-25 08:29:20.000000 kmerexplor-1.0.3/kmerexplor/counts.py
--rwxrwxr-x   0 benoit    (1017) bio2m     (1010)      209 2024-03-26 10:56:24.000000 kmerexplor-1.0.3/kmerexplor/info.py
--rwxrwxr-x   0 benoit    (1017) bio2m     (1010)   658096 2024-03-25 08:29:21.000000 kmerexplor-1.0.3/kmerexplor/mk_results.py
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)    10475 2024-03-25 08:29:21.000000 kmerexplor-1.0.3/kmerexplor/options.py
--rwxrwxr-x   0 benoit    (1017) bio2m     (1010)     2659 2023-07-19 12:51:30.000000 kmerexplor-1.0.3/kmerexplor/samples.py
-drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2024-03-26 10:56:40.808542 kmerexplor-1.0.3/kmerexplor/tagsets/
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)     1198 2024-03-25 08:29:21.000000 kmerexplor-1.0.3/kmerexplor/tagsets/human-quality.md
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)  4116851 2024-03-25 17:03:22.000000 kmerexplor-1.0.3/kmerexplor/tagsets/human-quality.tsv.gz
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)    11533 2024-03-25 08:29:21.000000 kmerexplor-1.0.3/kmerexplor/tagsets/human-quality.yaml
-drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2024-03-26 10:56:40.683918 kmerexplor-1.0.3/kmerexplor.egg-info/
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)    14032 2024-03-26 10:56:40.000000 kmerexplor-1.0.3/kmerexplor.egg-info/PKG-INFO
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)      590 2024-03-26 10:56:40.000000 kmerexplor-1.0.3/kmerexplor.egg-info/SOURCES.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)        1 2024-03-26 10:56:40.000000 kmerexplor-1.0.3/kmerexplor.egg-info/dependency_links.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)       53 2024-03-26 10:56:40.000000 kmerexplor-1.0.3/kmerexplor.egg-info/entry_points.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)       16 2024-03-26 10:56:40.000000 kmerexplor-1.0.3/kmerexplor.egg-info/requires.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)       11 2024-03-26 10:56:40.000000 kmerexplor-1.0.3/kmerexplor.egg-info/top_level.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)       38 2024-03-26 10:56:40.832118 kmerexplor-1.0.3/setup.cfg
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)     1032 2023-10-20 07:36:54.000000 kmerexplor-1.0.3/setup.py
+drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2024-04-02 07:01:43.807968 kmerexplor-1.0.4/
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)      212 2023-07-19 12:51:29.000000 kmerexplor-1.0.4/MANIFEST.in
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)    14032 2024-04-02 07:01:43.803335 kmerexplor-1.0.4/PKG-INFO
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)    11137 2024-03-25 08:29:20.000000 kmerexplor-1.0.4/README.md
+drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2024-04-02 07:01:43.602276 kmerexplor-1.0.4/kmerexplor/
+-rwxrwxr-x   0 benoit    (1017) bio2m     (1010)      115 2023-07-19 12:51:29.000000 kmerexplor-1.0.4/kmerexplor/__init__.py
+-rwxrwxr-x   0 benoit    (1017) bio2m     (1010)     2478 2023-07-19 12:51:29.000000 kmerexplor-1.0.4/kmerexplor/checkFile.py
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)     1088 2024-03-25 08:29:20.000000 kmerexplor-1.0.4/kmerexplor/common.py
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)    11533 2024-03-13 11:14:24.000000 kmerexplor-1.0.4/kmerexplor/config.yaml
+-rwxrwxr-x   0 benoit    (1017) bio2m     (1010)     6768 2024-03-25 08:29:20.000000 kmerexplor-1.0.4/kmerexplor/core.py
+-rwxrwxr-x   0 benoit    (1017) bio2m     (1010)    89080 2023-07-19 12:51:29.000000 kmerexplor-1.0.4/kmerexplor/countTags
+-rwxrwxr-x   0 benoit    (1017) bio2m     (1010)    14740 2024-03-25 08:29:20.000000 kmerexplor-1.0.4/kmerexplor/counts.py
+-rwxrwxr-x   0 benoit    (1017) bio2m     (1010)      209 2024-04-02 07:01:23.000000 kmerexplor-1.0.4/kmerexplor/info.py
+-rwxrwxr-x   0 benoit    (1017) bio2m     (1010)   658096 2024-03-25 08:29:21.000000 kmerexplor-1.0.4/kmerexplor/mk_results.py
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)    10495 2024-04-02 06:52:17.000000 kmerexplor-1.0.4/kmerexplor/options.py
+-rwxrwxr-x   0 benoit    (1017) bio2m     (1010)     2659 2023-07-19 12:51:30.000000 kmerexplor-1.0.4/kmerexplor/samples.py
+drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2024-04-02 07:01:43.786089 kmerexplor-1.0.4/kmerexplor/tagsets/
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)     1198 2024-03-25 08:29:21.000000 kmerexplor-1.0.4/kmerexplor/tagsets/human-quality.md
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)  4116851 2024-03-25 17:03:22.000000 kmerexplor-1.0.4/kmerexplor/tagsets/human-quality.tsv.gz
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)    11533 2024-03-25 08:29:21.000000 kmerexplor-1.0.4/kmerexplor/tagsets/human-quality.yaml
+drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2024-04-02 07:01:43.692458 kmerexplor-1.0.4/kmerexplor.egg-info/
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)    14032 2024-04-02 07:01:43.000000 kmerexplor-1.0.4/kmerexplor.egg-info/PKG-INFO
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)      590 2024-04-02 07:01:43.000000 kmerexplor-1.0.4/kmerexplor.egg-info/SOURCES.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)        1 2024-04-02 07:01:43.000000 kmerexplor-1.0.4/kmerexplor.egg-info/dependency_links.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)       53 2024-04-02 07:01:43.000000 kmerexplor-1.0.4/kmerexplor.egg-info/entry_points.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)       16 2024-04-02 07:01:43.000000 kmerexplor-1.0.4/kmerexplor.egg-info/requires.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)       11 2024-04-02 07:01:43.000000 kmerexplor-1.0.4/kmerexplor.egg-info/top_level.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)       38 2024-04-02 07:01:43.810448 kmerexplor-1.0.4/setup.cfg
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)     1032 2023-10-20 07:36:54.000000 kmerexplor-1.0.4/setup.py
```

### Comparing `kmerexplor-1.0.3/PKG-INFO` & `kmerexplor-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmerexplor
-Version: 1.0.3
+Version: 1.0.4
 Summary: KmerExploR provides information on RNA-sequencing datasets.
 Home-page: https://github.com/Transipedia/KmerExploR
 Author: Benoit Guibert
 Author-email: benoit.guibert@free.fr
 License: GPLv3
 Description: # KmerExploR
```

### Comparing `kmerexplor-1.0.3/README.md` & `kmerexplor-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `kmerexplor-1.0.3/kmerexplor/checkFile.py` & `kmerexplor-1.0.4/kmerexplor/checkFile.py`

 * *Files identical despite different names*

### Comparing `kmerexplor-1.0.3/kmerexplor/common.py` & `kmerexplor-1.0.4/kmerexplor/common.py`

 * *Files identical despite different names*

### Comparing `kmerexplor-1.0.3/kmerexplor/config.yaml` & `kmerexplor-1.0.4/kmerexplor/config.yaml`

 * *Files identical despite different names*

### Comparing `kmerexplor-1.0.3/kmerexplor/core.py` & `kmerexplor-1.0.4/kmerexplor/core.py`

 * *Files identical despite different names*

### Comparing `kmerexplor-1.0.3/kmerexplor/countTags` & `kmerexplor-1.0.4/kmerexplor/countTags`

 * *Files identical despite different names*

### Comparing `kmerexplor-1.0.3/kmerexplor/counts.py` & `kmerexplor-1.0.4/kmerexplor/counts.py`

 * *Files identical despite different names*

### Comparing `kmerexplor-1.0.3/kmerexplor/mk_results.py` & `kmerexplor-1.0.4/kmerexplor/mk_results.py`

 * *Files identical despite different names*

### Comparing `kmerexplor-1.0.3/kmerexplor/options.py` & `kmerexplor-1.0.4/kmerexplor/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,30 +2,20 @@
 import os
 import argparse
 from shutil import copyfile
 import gzip
 
 
 import info
-# from opt_actions import DumpAction, ShowTagsAction, ListTagsetsAction
 from common import *
 
 APPPATH = os.path.dirname(os.path.realpath(__file__))
 DEFAULT_TAGSET = "human-quality"
 
 
-"""
-ajouter les def :
- - dump_config()
- - show_tags()
- - list_tagsets
-contrôler que
- - qu'il y a '-s' OU '-p'
-"""
-
 def handle_args(args):
     ### check some args
     check_args(args)
     ### check special options
     if args.dump_config: _dump_config(args)
     if args.show_tags: _show_tags(args)
     if args.list_tagsets: _list_tagsets(args)
@@ -36,14 +26,17 @@
     ### --paired OR --single
     if not special_option:
         if len([True for i in (args.paired, args.single) if i]) != 1:
             sys.exit("Syntax error: one of the arguments -s/--single -p/--paired is required")
         ### At least one fastq must be define
         if not args.files:
             sys.exit("Syntax error: the following arguments are required: <files1>")
+    ### output directory must be writable
+    if not os.access(os.path.dirname(os.path.abspath(args.output)), os.W_OK):
+        sys.exit(f"Permission denied: {os.path.dirname(os.path.abspath(args.output))}")
     ### Define user tagset tsv, config yaml, desc md and put them in args
     user_args_len = len([_ for _ in (args.config, args.tags) if _])
     if user_args_len == 2:
         ### check file presences
         if not os.path.isfile(args.tags):
             sys.exit(f"File error: {args.tags!r} not found")
         ### Is user has define a markdown description file ?
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `kmerexplor-1.0.3/kmerexplor/samples.py` & `kmerexplor-1.0.4/kmerexplor/samples.py`

 * *Files identical despite different names*

### Comparing `kmerexplor-1.0.3/kmerexplor/tagsets/human-quality.md` & `kmerexplor-1.0.4/kmerexplor/tagsets/human-quality.md`

 * *Files identical despite different names*

### Comparing `kmerexplor-1.0.3/kmerexplor/tagsets/human-quality.tsv.gz` & `kmerexplor-1.0.4/kmerexplor/tagsets/human-quality.tsv.gz`

 * *Files identical despite different names*

### Comparing `kmerexplor-1.0.3/kmerexplor/tagsets/human-quality.yaml` & `kmerexplor-1.0.4/kmerexplor/tagsets/human-quality.yaml`

 * *Files identical despite different names*

### Comparing `kmerexplor-1.0.3/kmerexplor.egg-info/PKG-INFO` & `kmerexplor-1.0.4/kmerexplor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmerexplor
-Version: 1.0.3
+Version: 1.0.4
 Summary: KmerExploR provides information on RNA-sequencing datasets.
 Home-page: https://github.com/Transipedia/KmerExploR
 Author: Benoit Guibert
 Author-email: benoit.guibert@free.fr
 License: GPLv3
 Description: # KmerExploR
```

### Comparing `kmerexplor-1.0.3/kmerexplor.egg-info/SOURCES.txt` & `kmerexplor-1.0.4/kmerexplor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kmerexplor-1.0.3/setup.py` & `kmerexplor-1.0.4/setup.py`

 * *Files identical despite different names*

