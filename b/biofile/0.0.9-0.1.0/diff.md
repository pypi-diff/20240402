# Comparing `tmp/biofile-0.0.9.tar.gz` & `tmp/biofile-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biofile-0.0.9.tar", last modified: Thu Jan 25 16:53:22 2024, max compression
+gzip compressed data, was "biofile-0.1.0.tar", last modified: Mon Apr  1 22:23:35 2024, max compression
```

## Comparing `biofile-0.0.9.tar` & `biofile-0.1.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxr-x   0 yuan      (1000) yuan      (1000)        0 2024-01-25 16:53:22.230921 biofile-0.0.9/
--rw-r--r--   0 yuan      (1000) yuan      (1000)     1990 2024-01-25 16:53:22.230921 biofile-0.0.9/PKG-INFO
--rw-rw-r--   0 yuan      (1000) yuan      (1000)     1479 2024-01-02 03:18:20.000000 biofile-0.0.9/README.md
--rw-rw-r--   0 yuan      (1000) yuan      (1000)      516 2024-01-25 16:53:04.000000 biofile-0.0.9/pyproject.toml
--rw-rw-r--   0 yuan      (1000) yuan      (1000)       38 2024-01-25 16:53:22.230921 biofile-0.0.9/setup.cfg
-drwxrwxr-x   0 yuan      (1000) yuan      (1000)        0 2024-01-25 16:53:22.222921 biofile-0.0.9/src/
-drwxrwxr-x   0 yuan      (1000) yuan      (1000)        0 2024-01-25 16:53:22.226921 biofile-0.0.9/src/biofile/
--rw-rw-r--   0 yuan      (1000) yuan      (1000)      340 2024-01-23 14:34:33.000000 biofile-0.0.9/src/biofile/__init__.py
--rw-rw-r--   0 yuan      (1000) yuan      (1000)     1136 2024-01-25 16:53:17.000000 biofile-0.0.9/src/biofile/commons.py
--rw-rw-r--   0 yuan      (1000) yuan      (1000)     8979 2023-12-31 03:17:21.000000 biofile-0.0.9/src/biofile/fast5.py
--rw-rw-r--   0 yuan      (1000) yuan      (1000)     3917 2023-12-31 03:17:21.000000 biofile-0.0.9/src/biofile/fasta.py
--rw-rw-r--   0 yuan      (1000) yuan      (1000)     2808 2024-01-25 16:53:17.000000 biofile-0.0.9/src/biofile/fastq.py
-drwxrwxr-x   0 yuan      (1000) yuan      (1000)        0 2024-01-25 16:53:22.226921 biofile-0.0.9/src/biofile/genome/
--rw-rw-r--   0 yuan      (1000) yuan      (1000)     1786 2024-01-24 15:54:53.000000 biofile-0.0.9/src/biofile/genome/annot_file.py
--rw-rw-r--   0 yuan      (1000) yuan      (1000)     2585 2024-01-23 14:34:33.000000 biofile-0.0.9/src/biofile/genome/annot_record.py
--rw-rw-r--   0 yuan      (1000) yuan      (1000)     1028 2024-01-23 14:34:33.000000 biofile-0.0.9/src/biofile/genome/annot_validate.py
--rw-rw-r--   0 yuan      (1000) yuan      (1000)      307 2024-01-23 14:34:33.000000 biofile-0.0.9/src/biofile/genome/base.py
--rw-rw-r--   0 yuan      (1000) yuan      (1000)     3159 2024-01-24 14:48:15.000000 biofile-0.0.9/src/biofile/genome/fasta_dna.py
--rw-rw-r--   0 yuan      (1000) yuan      (1000)     1190 2024-01-23 14:34:33.000000 biofile-0.0.9/src/biofile/genome/gbk.py
--rw-rw-r--   0 yuan      (1000) yuan      (1000)     8090 2024-01-23 14:34:33.000000 biofile-0.0.9/src/biofile/genome/gff.py
--rw-rw-r--   0 yuan      (1000) yuan      (1000)     3150 2024-01-23 14:34:33.000000 biofile-0.0.9/src/biofile/genome/gtf.py
--rw-rw-r--   0 yuan      (1000) yuan      (1000)      994 2024-01-25 16:53:17.000000 biofile-0.0.9/src/biofile/pubmed_xml.py
--rw-rw-r--   0 yuan      (1000) yuan      (1000)     1609 2024-01-25 16:53:17.000000 biofile-0.0.9/src/biofile/sample.py
--rw-rw-r--   0 yuan      (1000) yuan      (1000)     2045 2024-01-25 16:53:17.000000 biofile-0.0.9/src/biofile/wrap.py
-drwxrwxr-x   0 yuan      (1000) yuan      (1000)        0 2024-01-25 16:53:22.230921 biofile-0.0.9/src/biofile.egg-info/
--rw-r--r--   0 yuan      (1000) yuan      (1000)     1990 2024-01-25 16:53:22.000000 biofile-0.0.9/src/biofile.egg-info/PKG-INFO
--rw-rw-r--   0 yuan      (1000) yuan      (1000)      602 2024-01-25 16:53:22.000000 biofile-0.0.9/src/biofile.egg-info/SOURCES.txt
--rw-rw-r--   0 yuan      (1000) yuan      (1000)        1 2024-01-25 16:53:22.000000 biofile-0.0.9/src/biofile.egg-info/dependency_links.txt
--rw-rw-r--   0 yuan      (1000) yuan      (1000)        8 2024-01-25 16:53:22.000000 biofile-0.0.9/src/biofile.egg-info/top_level.txt
-drwxrwxr-x   0 yuan      (1000) yuan      (1000)        0 2024-01-25 16:53:22.226921 biofile-0.0.9/tests/
--rw-rw-r--   0 yuan      (1000) yuan      (1000)      214 2023-12-31 03:17:21.000000 biofile-0.0.9/tests/test_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:23:35.513092 biofile-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-01 22:23:35.509092 biofile-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-01 22:23:23.000000 biofile-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 22:23:35.513092 biofile-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-01 22:23:23.000000 biofile-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:23:35.505092 biofile-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:23:35.509092 biofile-0.1.0/src/biofile/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-01 22:23:23.000000 biofile-0.1.0/src/biofile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-01 22:23:23.000000 biofile-0.1.0/src/biofile/commons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8979 2024-04-01 22:23:23.000000 biofile-0.1.0/src/biofile/fast5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-04-01 22:23:23.000000 biofile-0.1.0/src/biofile/fasta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-01 22:23:23.000000 biofile-0.1.0/src/biofile/fastq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:23:35.509092 biofile-0.1.0/src/biofile/genome/
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-01 22:23:23.000000 biofile-0.1.0/src/biofile/genome/annot_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-01 22:23:23.000000 biofile-0.1.0/src/biofile/genome/annot_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-01 22:23:23.000000 biofile-0.1.0/src/biofile/genome/annot_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-01 22:23:23.000000 biofile-0.1.0/src/biofile/genome/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-01 22:23:23.000000 biofile-0.1.0/src/biofile/genome/fasta_dna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-01 22:23:23.000000 biofile-0.1.0/src/biofile/genome/gbk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8090 2024-04-01 22:23:23.000000 biofile-0.1.0/src/biofile/genome/gff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-01 22:23:23.000000 biofile-0.1.0/src/biofile/genome/gtf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-01 22:23:23.000000 biofile-0.1.0/src/biofile/pubmed_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-01 22:23:23.000000 biofile-0.1.0/src/biofile/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-01 22:23:23.000000 biofile-0.1.0/src/biofile/wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:23:35.509092 biofile-0.1.0/src/biofile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-01 22:23:35.000000 biofile-0.1.0/src/biofile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-01 22:23:35.000000 biofile-0.1.0/src/biofile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 22:23:35.000000 biofile-0.1.0/src/biofile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-01 22:23:35.000000 biofile-0.1.0/src/biofile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-01 22:23:35.000000 biofile-0.1.0/src/biofile.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:23:35.509092 biofile-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-01 22:23:23.000000 biofile-0.1.0/tests/test_env.py
```

### Comparing `biofile-0.0.9/PKG-INFO` & `biofile-0.1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 Metadata-Version: 2.1
 Name: biofile
-Version: 0.0.9
-Summary: Process varous file format for RNA-Seq data analysis
-Author-email: Tiezheng Yuan <tiezhengyuan@hotmail.com>
-Project-URL: Homepage, https://github.com/Tiezhengyuan/bio_file
-Project-URL: Issues, https://github.com/Tiezhengyuan/bio_file/issues
+Version: 0.1.0
+Summary: Process various file format for RNA-Seq data analysis
+Home-page: https://github.com/Tiezhengyuan/bio_file
+Author: Tiezheng Yuan
+Author-email: tiezhengyuan@hotmail.com
+Keywords: pypi,cicd,python
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
+Requires-Dist: Bio
+Requires-Dist: biosequtils
+Requires-Dist: numpy
+Requires-Dist: pandas
 
-# Bioinformatics Tool: bioFile
+\n# Bioinformatics Tool: bioFile
 
 ## Introduction
 Retrieve data from various file formats used in RNA-Seq data analysis. The tool currently support:
 - GTF file: genomic annotations
 - GFF file: genomic annoations
 
 quick installation
```

### Comparing `biofile-0.0.9/README.md` & `biofile-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `biofile-0.0.9/src/biofile/commons.py` & `biofile-0.1.0/src/biofile/commons.py`

 * *Files identical despite different names*

### Comparing `biofile-0.0.9/src/biofile/fast5.py` & `biofile-0.1.0/src/biofile/fast5.py`

 * *Files identical despite different names*

### Comparing `biofile-0.0.9/src/biofile/fasta.py` & `biofile-0.1.0/src/biofile/fasta.py`

 * *Files identical despite different names*

### Comparing `biofile-0.0.9/src/biofile/fastq.py` & `biofile-0.1.0/src/biofile/fastq.py`

 * *Files identical despite different names*

### Comparing `biofile-0.0.9/src/biofile/genome/annot_file.py` & `biofile-0.1.0/src/biofile/genome/annot_file.py`

 * *Files identical despite different names*

### Comparing `biofile-0.0.9/src/biofile/genome/annot_record.py` & `biofile-0.1.0/src/biofile/genome/annot_record.py`

 * *Files identical despite different names*

### Comparing `biofile-0.0.9/src/biofile/genome/annot_validate.py` & `biofile-0.1.0/src/biofile/genome/annot_validate.py`

 * *Files identical despite different names*

### Comparing `biofile-0.0.9/src/biofile/genome/fasta_dna.py` & `biofile-0.1.0/src/biofile/genome/fasta_dna.py`

 * *Files identical despite different names*

### Comparing `biofile-0.0.9/src/biofile/genome/gbk.py` & `biofile-0.1.0/src/biofile/genome/gbk.py`

 * *Files identical despite different names*

### Comparing `biofile-0.0.9/src/biofile/genome/gff.py` & `biofile-0.1.0/src/biofile/genome/gff.py`

 * *Files identical despite different names*

### Comparing `biofile-0.0.9/src/biofile/genome/gtf.py` & `biofile-0.1.0/src/biofile/genome/gtf.py`

 * *Files identical despite different names*

### Comparing `biofile-0.0.9/src/biofile/pubmed_xml.py` & `biofile-0.1.0/src/biofile/pubmed_xml.py`

 * *Files identical despite different names*

### Comparing `biofile-0.0.9/src/biofile/sample.py` & `biofile-0.1.0/src/biofile/sample.py`

 * *Files identical despite different names*

### Comparing `biofile-0.0.9/src/biofile/wrap.py` & `biofile-0.1.0/src/biofile/wrap.py`

 * *Files identical despite different names*

### Comparing `biofile-0.0.9/src/biofile.egg-info/PKG-INFO` & `biofile-0.1.0/src/biofile.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 Metadata-Version: 2.1
 Name: biofile
-Version: 0.0.9
-Summary: Process varous file format for RNA-Seq data analysis
-Author-email: Tiezheng Yuan <tiezhengyuan@hotmail.com>
-Project-URL: Homepage, https://github.com/Tiezhengyuan/bio_file
-Project-URL: Issues, https://github.com/Tiezhengyuan/bio_file/issues
+Version: 0.1.0
+Summary: Process various file format for RNA-Seq data analysis
+Home-page: https://github.com/Tiezhengyuan/bio_file
+Author: Tiezheng Yuan
+Author-email: tiezhengyuan@hotmail.com
+Keywords: pypi,cicd,python
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
+Requires-Dist: Bio
+Requires-Dist: biosequtils
+Requires-Dist: numpy
+Requires-Dist: pandas
 
-# Bioinformatics Tool: bioFile
+\n# Bioinformatics Tool: bioFile
 
 ## Introduction
 Retrieve data from various file formats used in RNA-Seq data analysis. The tool currently support:
 - GTF file: genomic annotations
 - GFF file: genomic annoations
 
 quick installation
```

### Comparing `biofile-0.0.9/src/biofile.egg-info/SOURCES.txt` & `biofile-0.1.0/src/biofile.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 README.md
-pyproject.toml
+setup.py
 src/biofile/__init__.py
 src/biofile/commons.py
 src/biofile/fast5.py
 src/biofile/fasta.py
 src/biofile/fastq.py
 src/biofile/pubmed_xml.py
 src/biofile/sample.py
 src/biofile/wrap.py
 src/biofile.egg-info/PKG-INFO
 src/biofile.egg-info/SOURCES.txt
 src/biofile.egg-info/dependency_links.txt
+src/biofile.egg-info/requires.txt
 src/biofile.egg-info/top_level.txt
 src/biofile/genome/annot_file.py
 src/biofile/genome/annot_record.py
 src/biofile/genome/annot_validate.py
 src/biofile/genome/base.py
 src/biofile/genome/fasta_dna.py
 src/biofile/genome/gbk.py
```

