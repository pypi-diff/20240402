# Comparing `tmp/gemsembler-0.5.6.tar.gz` & `tmp/gemsembler-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemsembler-0.5.6.tar", last modified: Wed Mar 27 12:59:34 2024, max compression
+gzip compressed data, was "gemsembler-0.6.1.tar", last modified: Tue Apr  2 11:15:57 2024, max compression
```

## Comparing `gemsembler-0.5.6.tar` & `gemsembler-0.6.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 12:59:34.110224 gemsembler-0.5.6/
--rw-rw-rw-   0 root         (0) root         (0)     1083 2024-03-27 12:59:20.000000 gemsembler-0.5.6/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       72 2024-03-27 12:59:20.000000 gemsembler-0.5.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4174 2024-03-27 12:59:34.109224 gemsembler-0.5.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1867 2024-03-27 12:59:20.000000 gemsembler-0.5.6/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1846 2024-03-27 12:59:20.000000 gemsembler-0.5.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-27 12:59:34.110224 gemsembler-0.5.6/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 12:59:34.101224 gemsembler-0.5.6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 12:59:34.104224 gemsembler-0.5.6/src/gemsembler/
--rw-rw-rw-   0 root         (0) root         (0)     1785 2024-03-27 12:59:20.000000 gemsembler-0.5.6/src/gemsembler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      896 2024-03-27 12:59:20.000000 gemsembler-0.5.6/src/gemsembler/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     7898 2024-03-27 12:59:20.000000 gemsembler-0.5.6/src/gemsembler/anticreation.py
--rw-rw-rw-   0 root         (0) root         (0)    19906 2024-03-27 12:59:20.000000 gemsembler-0.5.6/src/gemsembler/comparison.py
--rw-rw-rw-   0 root         (0) root         (0)    13666 2024-03-27 12:59:20.000000 gemsembler-0.5.6/src/gemsembler/conversion.py
--rw-rw-rw-   0 root         (0) root         (0)    52270 2024-03-27 12:59:20.000000 gemsembler-0.5.6/src/gemsembler/creation.py
--rw-rw-rw-   0 root         (0) root         (0)     4300 2024-03-27 12:59:20.000000 gemsembler-0.5.6/src/gemsembler/curation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 12:59:34.104224 gemsembler-0.5.6/src/gemsembler/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 12:59:34.106224 gemsembler-0.5.6/src/gemsembler/data/BU/
--rw-rw-rw-   0 root         (0) root         (0)   180894 2024-03-27 12:59:20.000000 gemsembler-0.5.6/src/gemsembler/data/BU/BU_agora.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)   303843 2024-03-27 12:59:20.000000 gemsembler-0.5.6/src/gemsembler/data/BU/BU_carveme_hom.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)   381510 2024-03-27 12:59:20.000000 gemsembler-0.5.6/src/gemsembler/data/BU/BU_gapseq.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)    83221 2024-03-27 12:59:20.000000 gemsembler-0.5.6/src/gemsembler/data/BU/BU_modelSEED.sbml.gz
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-27 12:59:20.000000 gemsembler-0.5.6/src/gemsembler/data/BU/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 12:59:34.109224 gemsembler-0.5.6/src/gemsembler/data/LP/
--rw-rw-rw-   0 root         (0) root         (0)   153653 2024-03-27 12:59:20.000000 gemsembler-0.5.6/src/gemsembler/data/LP/LP_CA1.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)   157673 2024-03-27 12:59:20.000000 gemsembler-0.5.6/src/gemsembler/data/LP/LP_CA2.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)    82710 2024-03-27 12:59:20.000000 gemsembler-0.5.6/src/gemsembler/data/LP/LP_MS2.sbml.gz
--rw-rw-rw-   0 root         (0) root         (0)   885760 2024-03-27 12:59:20.000000 gemsembler-0.5.6/src/gemsembler/data/LP/LP_WCFS1.fasta.gz
--rw-rw-rw-   0 root         (0) root         (0)   151435 2024-03-27 12:59:20.000000 gemsembler-0.5.6/src/gemsembler/data/LP/LP_WCFS1_agora.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)   124883 2024-03-27 12:59:20.000000 gemsembler-0.5.6/src/gemsembler/data/LP/LP_iLP728_revision_data_met_C_c.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)   547669 2024-03-27 12:59:20.000000 gemsembler-0.5.6/src/gemsembler/data/LP/LP_protein_fasta.faa.gz
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-27 12:59:20.000000 gemsembler-0.5.6/src/gemsembler/data/LP/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-27 12:59:20.000000 gemsembler-0.5.6/src/gemsembler/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9181 2024-03-27 12:59:20.000000 gemsembler-0.5.6/src/gemsembler/dbs.py
--rw-rw-rw-   0 root         (0) root         (0)    18986 2024-03-27 12:59:20.000000 gemsembler-0.5.6/src/gemsembler/downstream.py
--rw-rw-rw-   0 root         (0) root         (0)    50045 2024-03-27 12:59:20.000000 gemsembler-0.5.6/src/gemsembler/drawing.py
--rw-rw-rw-   0 root         (0) root         (0)    23995 2024-03-27 12:59:20.000000 gemsembler-0.5.6/src/gemsembler/gathering.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2024-03-27 12:59:20.000000 gemsembler-0.5.6/src/gemsembler/general.py
--rw-rw-rw-   0 root         (0) root         (0)    13330 2024-03-27 12:59:20.000000 gemsembler-0.5.6/src/gemsembler/genes.py
--rw-rw-rw-   0 root         (0) root         (0)    22859 2024-03-27 12:59:20.000000 gemsembler-0.5.6/src/gemsembler/pathsfinding.py
--rw-rw-rw-   0 root         (0) root         (0)     4557 2024-03-27 12:59:20.000000 gemsembler-0.5.6/src/gemsembler/periplasmic.py
--rw-rw-rw-   0 root         (0) root         (0)    10165 2024-03-27 12:59:20.000000 gemsembler-0.5.6/src/gemsembler/selection.py
--rw-rw-rw-   0 root         (0) root         (0)    31443 2024-03-27 12:59:20.000000 gemsembler-0.5.6/src/gemsembler/structural.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 12:59:34.109224 gemsembler-0.5.6/src/gemsembler.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4174 2024-03-27 12:59:34.000000 gemsembler-0.5.6/src/gemsembler.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1435 2024-03-27 12:59:34.000000 gemsembler-0.5.6/src/gemsembler.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-27 12:59:34.000000 gemsembler-0.5.6/src/gemsembler.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2024-03-27 12:59:34.000000 gemsembler-0.5.6/src/gemsembler.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      121 2024-03-27 12:59:34.000000 gemsembler-0.5.6/src/gemsembler.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-03-27 12:59:34.000000 gemsembler-0.5.6/src/gemsembler.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 12:59:34.109224 gemsembler-0.5.6/tests/
--rw-rw-rw-   0 root         (0) root         (0)    12691 2024-03-27 12:59:20.000000 gemsembler-0.5.6/tests/test_conversion.py
--rw-rw-rw-   0 root         (0) root         (0)     2191 2024-03-27 12:59:20.000000 gemsembler-0.5.6/tests/test_curation.py
--rw-rw-rw-   0 root         (0) root         (0)     4293 2024-03-27 12:59:20.000000 gemsembler-0.5.6/tests/test_dbs.py
--rw-rw-rw-   0 root         (0) root         (0)     4021 2024-03-27 12:59:20.000000 gemsembler-0.5.6/tests/test_gathering.py
--rw-rw-rw-   0 root         (0) root         (0)     2357 2024-03-27 12:59:20.000000 gemsembler-0.5.6/tests/test_selection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:15:57.105188 gemsembler-0.6.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1083 2024-04-02 11:15:45.000000 gemsembler-0.6.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       72 2024-04-02 11:15:45.000000 gemsembler-0.6.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4174 2024-04-02 11:15:57.105188 gemsembler-0.6.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2024-04-02 11:15:45.000000 gemsembler-0.6.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1846 2024-04-02 11:15:45.000000 gemsembler-0.6.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 11:15:57.105188 gemsembler-0.6.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:15:57.097188 gemsembler-0.6.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:15:57.099188 gemsembler-0.6.1/src/gemsembler/
+-rw-rw-rw-   0 root         (0) root         (0)     1785 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      896 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7898 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/anticreation.py
+-rw-rw-rw-   0 root         (0) root         (0)    19906 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/comparison.py
+-rw-rw-rw-   0 root         (0) root         (0)    14845 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)    52270 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/creation.py
+-rw-rw-rw-   0 root         (0) root         (0)     4300 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/curation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:15:57.100188 gemsembler-0.6.1/src/gemsembler/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:15:57.101188 gemsembler-0.6.1/src/gemsembler/data/BU/
+-rw-rw-rw-   0 root         (0) root         (0)   180894 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/data/BU/BU_agora.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)   303843 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/data/BU/BU_carveme_hom.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)   381510 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/data/BU/BU_gapseq.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)    83221 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/data/BU/BU_modelSEED.sbml.gz
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/data/BU/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:15:57.104188 gemsembler-0.6.1/src/gemsembler/data/LP/
+-rw-rw-rw-   0 root         (0) root         (0)   153653 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/data/LP/LP_CA1.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)   157673 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/data/LP/LP_CA2.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)    82710 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/data/LP/LP_MS2.sbml.gz
+-rw-rw-rw-   0 root         (0) root         (0)   885760 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/data/LP/LP_WCFS1.fasta.gz
+-rw-rw-rw-   0 root         (0) root         (0)   151435 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/data/LP/LP_WCFS1_agora.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)   124883 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/data/LP/LP_iLP728_revision_data_met_C_c.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)   547669 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/data/LP/LP_protein_fasta.faa.gz
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/data/LP/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10388 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/dbs.py
+-rw-rw-rw-   0 root         (0) root         (0)    18986 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/downstream.py
+-rw-rw-rw-   0 root         (0) root         (0)    50045 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/drawing.py
+-rw-rw-rw-   0 root         (0) root         (0)    24355 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/gathering.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/general.py
+-rw-rw-rw-   0 root         (0) root         (0)    13330 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/genes.py
+-rw-rw-rw-   0 root         (0) root         (0)    22859 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/pathsfinding.py
+-rw-rw-rw-   0 root         (0) root         (0)     4557 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/periplasmic.py
+-rw-rw-rw-   0 root         (0) root         (0)    10165 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/selection.py
+-rw-rw-rw-   0 root         (0) root         (0)    31443 2024-04-02 11:15:45.000000 gemsembler-0.6.1/src/gemsembler/structural.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:15:57.105188 gemsembler-0.6.1/src/gemsembler.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4174 2024-04-02 11:15:57.000000 gemsembler-0.6.1/src/gemsembler.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1435 2024-04-02 11:15:57.000000 gemsembler-0.6.1/src/gemsembler.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 11:15:57.000000 gemsembler-0.6.1/src/gemsembler.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2024-04-02 11:15:57.000000 gemsembler-0.6.1/src/gemsembler.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      121 2024-04-02 11:15:57.000000 gemsembler-0.6.1/src/gemsembler.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-02 11:15:57.000000 gemsembler-0.6.1/src/gemsembler.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:15:57.105188 gemsembler-0.6.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    12691 2024-04-02 11:15:45.000000 gemsembler-0.6.1/tests/test_conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2024-04-02 11:15:45.000000 gemsembler-0.6.1/tests/test_curation.py
+-rw-rw-rw-   0 root         (0) root         (0)     4293 2024-04-02 11:15:45.000000 gemsembler-0.6.1/tests/test_dbs.py
+-rw-rw-rw-   0 root         (0) root         (0)     4021 2024-04-02 11:15:45.000000 gemsembler-0.6.1/tests/test_gathering.py
+-rw-rw-rw-   0 root         (0) root         (0)     2357 2024-04-02 11:15:45.000000 gemsembler-0.6.1/tests/test_selection.py
```

### Comparing `gemsembler-0.5.6/LICENSE` & `gemsembler-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gemsembler-0.5.6/PKG-INFO` & `gemsembler-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemsembler
-Version: 0.5.6
+Version: 0.6.1
 Summary: A tool for assembling and comparing several types of Genome-Scale Metabolic Models.
 Author-email: Elena Matveishina <elena.matveishina@embl.de>, Bartosz Bartmanski <bartosz.bartmanski@embl.de>
 License: MIT License
         
         Copyright (c) 2024 Zimmermann-Kogadeeva Group
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `gemsembler-0.5.6/README.md` & `gemsembler-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `gemsembler-0.5.6/pyproject.toml` & `gemsembler-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gemsembler"
-version = "0.5.6"
+version = "0.6.1"
 description = "A tool for assembling and comparing several types of Genome-Scale Metabolic Models."
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [
     { name = "Elena Matveishina", email = "elena.matveishina@embl.de" },
     { name = "Bartosz Bartmanski", email = "bartosz.bartmanski@embl.de" }
 ]
@@ -47,15 +47,15 @@
 include-package-data = true
 
 [tool.setuptools.packages.find]
 namespaces = true
 where = ["src"]
 
 [tool.bumpver]
-current_version = "0.5.6"
+current_version = "0.6.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `gemsembler-0.5.6/src/gemsembler/__init__.py` & `gemsembler-0.6.1/src/gemsembler/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from importlib.resources import files
 
 from .anticreation import get_model_of_interest
 from .creation import read_supermodel_from_pkl
 from .data import BU, LP
 from .gathering import GatheredModels, load_sbml_model
 
-__version__ = "0.5.6"
+__version__ = "0.6.1"
 
 lp_example = [
     dict(
         model_id="curated_LP",
         path_to_model=files(LP) / "LP_iLP728_revision_data_met_C_c.xml.gz",
         model_type="carveme",
         path_to_genome=files(LP) / "LP_protein_fasta.faa.gz",
```

### Comparing `gemsembler-0.5.6/src/gemsembler/__main__.py` & `gemsembler-0.6.1/src/gemsembler/__main__.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.5.6/src/gemsembler/anticreation.py` & `gemsembler-0.6.1/src/gemsembler/anticreation.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.5.6/src/gemsembler/comparison.py` & `gemsembler-0.6.1/src/gemsembler/comparison.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.5.6/src/gemsembler/conversion.py` & `gemsembler-0.6.1/src/gemsembler/conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import re
 from abc import ABC, abstractmethod
 
 from .dbs import (
     get_BiGG_lists,
     get_kegg_m,
     get_kegg_r,
+    get_mnx_m,
+    get_mnx_r,
     get_old_bigg_m,
     get_old_bigg_r,
     get_seed_addit_m,
     get_seed_addit_r,
     get_seed_orig_m,
     get_seed_orig_r,
 )
@@ -214,14 +216,52 @@
             compartment=[x.removesuffix("0") for x in reaction.compartments],
             main=conv_main,
             addit=conv_addit,
             metabolite=False,
         )
 
 
+class ConvMetanetx(ConvBase):
+    def __init__(
+        self,
+        main_map_m=None,
+        main_map_r=None,
+        bigg_m=None,
+        bigg_r=None,
+    ):
+        super().__init__(bigg_m, bigg_r)
+
+        # TODO: checks that tables, if given, are of the appropriate format
+        self.__main_map_m__ = main_map_m or get_mnx_m()
+        self.__main_map_r__ = main_map_r or get_mnx_r()
+        self.__comp_regex__ = re.compile("[c@].*$")
+
+    def convert_metabolite(self, metabolite):
+        id_wo_comp = self.__comp_regex__.sub("", metabolite.id)
+        conv_main = self.__main_map_m__.get(id_wo_comp, [])
+
+        return Converted(
+            check_db=self.__bigg_m__,
+            compartment=[metabolite.compartment],
+            main=conv_main,
+            metabolite=True,
+        )
+
+    def convert_reaction(self, reaction):
+        id_wo_comp = self.__comp_regex__.sub("", reaction.id)
+        conv_main = self.__main_map_r__.get(id_wo_comp, [])
+
+        return Converted(
+            check_db=self.__bigg_r__,
+            compartment=list(reaction.compartments),
+            main=conv_main,
+            metabolite=False,
+        )
+
+
 class ConvAgora(ConvBase):
     def __init__(
         self,
         main_map_m=None,
         additional_table_m=None,
         main_map_r=None,
         additional_table_r=None,
```

### Comparing `gemsembler-0.5.6/src/gemsembler/creation.py` & `gemsembler-0.6.1/src/gemsembler/creation.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.5.6/src/gemsembler/curation.py` & `gemsembler-0.6.1/src/gemsembler/curation.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.5.6/src/gemsembler/data/BU/BU_agora.xml.gz` & `gemsembler-0.6.1/src/gemsembler/data/BU/BU_agora.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.5.6/src/gemsembler/data/BU/BU_carveme_hom.xml.gz` & `gemsembler-0.6.1/src/gemsembler/data/BU/BU_carveme_hom.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.5.6/src/gemsembler/data/BU/BU_gapseq.xml.gz` & `gemsembler-0.6.1/src/gemsembler/data/BU/BU_gapseq.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.5.6/src/gemsembler/data/BU/BU_modelSEED.sbml.gz` & `gemsembler-0.6.1/src/gemsembler/data/BU/BU_modelSEED.sbml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.5.6/src/gemsembler/data/LP/LP_CA1.xml.gz` & `gemsembler-0.6.1/src/gemsembler/data/LP/LP_CA1.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.5.6/src/gemsembler/data/LP/LP_CA2.xml.gz` & `gemsembler-0.6.1/src/gemsembler/data/LP/LP_CA2.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.5.6/src/gemsembler/data/LP/LP_MS2.sbml.gz` & `gemsembler-0.6.1/src/gemsembler/data/LP/LP_MS2.sbml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.5.6/src/gemsembler/data/LP/LP_WCFS1.fasta.gz` & `gemsembler-0.6.1/src/gemsembler/data/LP/LP_WCFS1.fasta.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.5.6/src/gemsembler/data/LP/LP_WCFS1_agora.xml.gz` & `gemsembler-0.6.1/src/gemsembler/data/LP/LP_WCFS1_agora.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.5.6/src/gemsembler/data/LP/LP_iLP728_revision_data_met_C_c.xml.gz` & `gemsembler-0.6.1/src/gemsembler/data/LP/LP_iLP728_revision_data_met_C_c.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.5.6/src/gemsembler/data/LP/LP_protein_fasta.faa.gz` & `gemsembler-0.6.1/src/gemsembler/data/LP/LP_protein_fasta.faa.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.5.6/src/gemsembler/dbs.py` & `gemsembler-0.6.1/src/gemsembler/dbs.py`

 * *Files 6% similar despite different names*

```diff
@@ -127,15 +127,16 @@
     df_modelseed_r = download_db(
         "https://github.com/ModelSEED/ModelSEEDDatabase/raw/master/Biochemistry/reactions.tsv",
         "reactions.tsv.gz",
     )
     return df_modelseed_r.pipe(process_modelseed)
 
 
-def process_metanetx(data, db_name, repl_regex):
+def process_with_metanetx(data, db_name, repl_regex):
+    """Get a mapping between `db_name` and bigg using metanetx db."""
     return (
         data.query("source.str.startswith(@db_name) or source.str.startswith('bigg')")
         .copy()
         .reset_index(drop=True)
         .assign(source=lambda x: x.source.str.replace(repl_regex, ":", regex=True))
         .pipe(separate, "source", sep=":", into=["db", "db_id"], expand=True)
         .drop_duplicates(subset=["db", "db_id"])
@@ -156,53 +157,89 @@
     df_metanetx_m = download_db(
         "https://www.metanetx.org/cgi-bin/mnxget/mnxref/chem_xref.tsv",
         "chem_xref.tsv.gz",
         comment="#",
         names=["source", "ID", "description"],
     )
     return df_metanetx_m.pipe(
-        process_metanetx, "seed", "(\.compound|M|\.metabolite):(M_)?"
+        process_with_metanetx, "seed", "(\.compound|M|\.metabolite):(M_)?"
     )
 
 
 @cache_file
 def get_seed_addit_r():
     df_metanetx_r = download_db(
         "https://www.metanetx.org/cgi-bin/mnxget/mnxref/reac_xref.tsv",
         "reac_xref.tsv.gz",
         comment="#",
         names=["source", "ID", "description"],
     )
-    return df_metanetx_r.pipe(process_metanetx, "seed", "(\.reaction|R|):(R_)?")
+    return df_metanetx_r.pipe(process_with_metanetx, "seed", "(\.reaction|R|):(R_)?")
+
+
+def process_metanetx(data, repl_regex):
+    """Get a mapping between metanetx and bigg"""
+    return (
+        data.query("source.str.startswith('bigg') and ID != 'EMPTY'")
+        .assign(source=lambda x: x.source.str.replace(repl_regex, "", regex=True))
+        .rename(columns={"source": "bigg", "ID": "mnx"})
+        .drop_duplicates(subset="bigg")
+        .drop(columns="description")
+        .groupby("mnx")["bigg"]
+        .apply(list)
+        .to_dict()
+    )
+
+
+@cache_file
+def get_mnx_m():
+    df_metanetx_m = download_db(
+        "https://www.metanetx.org/cgi-bin/mnxget/mnxref/chem_xref.tsv",
+        "chem_xref.tsv.gz",
+        comment="#",
+        names=["source", "ID", "description"],
+    )
+    return df_metanetx_m.pipe(process_metanetx, "bigg(\.compound|M|\.metabolite):(M_)?")
+
+
+@cache_file
+def get_mnx_r():
+    df_metanetx_r = download_db(
+        "https://www.metanetx.org/cgi-bin/mnxget/mnxref/reac_xref.tsv",
+        "reac_xref.tsv.gz",
+        comment="#",
+        names=["source", "ID", "description"],
+    )
+    return df_metanetx_r.pipe(process_metanetx, "bigg(\.reaction|R|):(R_)?")
 
 
 @cache_file
 def get_kegg_m():
     df_metanetx_m = download_db(
         "https://www.metanetx.org/cgi-bin/mnxget/mnxref/chem_xref.tsv",
         "chem_xref.tsv.gz",
         comment="#",
         names=["source", "ID", "description"],
     )
     return df_metanetx_m.pipe(
-        process_metanetx,
+        process_with_metanetx,
         "kegg",
         "(\.compound|\.drug|\.metabolite|\.glycan|[CDGM]):(M_)?",
     )
 
 
 @cache_file
 def get_kegg_r():
     df_metanetx_r = download_db(
         "https://www.metanetx.org/cgi-bin/mnxget/mnxref/reac_xref.tsv",
         "reac_xref.tsv.gz",
         comment="#",
         names=["source", "ID", "description"],
     )
-    return df_metanetx_r.pipe(process_metanetx, "kegg", "(\.reaction|R|):(R_)?")
+    return df_metanetx_r.pipe(process_with_metanetx, "kegg", "(\.reaction|R|):(R_)?")
 
 
 def get_BiGG_lists(metabolites: bool):
     if metabolites:
         bigg_data = download_db(
             "http://bigg.ucsd.edu/static/namespace/bigg_models_metabolites.txt",
             "bigg_models_metabolites.txt.gz",
```

### Comparing `gemsembler-0.5.6/src/gemsembler/downstream.py` & `gemsembler-0.6.1/src/gemsembler/downstream.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.5.6/src/gemsembler/drawing.py` & `gemsembler-0.6.1/src/gemsembler/drawing.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.5.6/src/gemsembler/gathering.py` & `gemsembler-0.6.1/src/gemsembler/gathering.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from .conversion import (
     ConvAgora,
     ConvBase,
     ConvBigg,
     ConvCarveme,
     ConvGapseq,
     ConvModelseed,
+    ConvMetanetx,
     no_changes_for_notconv,
     remove_zero_for_notconv,
     replace_square_brackets,
 )
 from .creation import SetofNewElements, SetofNewGenes, SuperModel
 from .curation import get_duplicated_reactions, remove_b_type_exchange
 from .dbs import download_db, get_bigg_network
@@ -140,14 +141,22 @@
                 "db_name": "bigg",
                 "wo_periplasmic": False,
                 "conv_strategy": ConvBigg(),
                 "genome_model_strategy": get_genes_not_gapseq,
                 "alter_notconv_m": no_changes_for_notconv,
                 "alter_notconv_r": no_changes_for_notconv,
             },
+            "metanetx": {
+                "remove_b": False,
+                "db_name": "bigg",
+                "wo_periplasmic": ConvMetanetx(),
+                "genome_model_strategy": get_genes_not_gapseq,
+                "alter_notconv_m": no_changes_for_notconv,
+                "alter_notconv_r": no_changes_for_notconv,
+            },
             "gapseq": {
                 "remove_b": False,
                 "db_name": "modelseed",
                 "wo_periplasmic": False,
                 "conv_strategy": ConvGapseq(),
                 "genome_model_strategy": get_genes_gapseq,
                 "alter_notconv_m": remove_zero_for_notconv,
```

### Comparing `gemsembler-0.5.6/src/gemsembler/genes.py` & `gemsembler-0.6.1/src/gemsembler/genes.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.5.6/src/gemsembler/pathsfinding.py` & `gemsembler-0.6.1/src/gemsembler/pathsfinding.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.5.6/src/gemsembler/periplasmic.py` & `gemsembler-0.6.1/src/gemsembler/periplasmic.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.5.6/src/gemsembler/selection.py` & `gemsembler-0.6.1/src/gemsembler/selection.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.5.6/src/gemsembler/structural.py` & `gemsembler-0.6.1/src/gemsembler/structural.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.5.6/src/gemsembler.egg-info/PKG-INFO` & `gemsembler-0.6.1/src/gemsembler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemsembler
-Version: 0.5.6
+Version: 0.6.1
 Summary: A tool for assembling and comparing several types of Genome-Scale Metabolic Models.
 Author-email: Elena Matveishina <elena.matveishina@embl.de>, Bartosz Bartmanski <bartosz.bartmanski@embl.de>
 License: MIT License
         
         Copyright (c) 2024 Zimmermann-Kogadeeva Group
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `gemsembler-0.5.6/src/gemsembler.egg-info/SOURCES.txt` & `gemsembler-0.6.1/src/gemsembler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gemsembler-0.5.6/tests/test_conversion.py` & `gemsembler-0.6.1/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.5.6/tests/test_curation.py` & `gemsembler-0.6.1/tests/test_curation.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.5.6/tests/test_dbs.py` & `gemsembler-0.6.1/tests/test_dbs.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.5.6/tests/test_gathering.py` & `gemsembler-0.6.1/tests/test_gathering.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.5.6/tests/test_selection.py` & `gemsembler-0.6.1/tests/test_selection.py`

 * *Files identical despite different names*

