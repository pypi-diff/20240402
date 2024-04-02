# Comparing `tmp/apscale-1.6.3.tar.gz` & `tmp/apscale-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apscale-1.6.3.tar", last modified: Tue Feb 21 10:46:00 2023, max compression
+gzip compressed data, was "apscale-1.7.0.tar", last modified: Tue Apr  2 12:06:08 2024, max compression
```

## Comparing `apscale-1.6.3.tar` & `apscale-1.7.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-02-21 10:46:00.385763 apscale-1.6.3/
--rw-rw-rw-   0        0        0     1093 2022-01-25 10:07:17.000000 apscale-1.6.3/LICENSE
--rw-rw-rw-   0        0        0       17 2022-04-05 12:21:44.000000 apscale-1.6.3/MANIFEST.in
--rw-rw-rw-   0        0        0     8528 2023-02-21 10:46:00.385763 apscale-1.6.3/PKG-INFO
--rw-rw-rw-   0        0        0     7496 2023-01-06 15:12:01.000000 apscale-1.6.3/README.md
-drwxrwxrwx   0        0        0        0 2023-02-21 10:46:00.372760 apscale-1.6.3/apscale/
--rw-rw-rw-   0        0        0        0 2022-01-25 10:07:17.000000 apscale-1.6.3/apscale/__init__.py
--rw-rw-rw-   0        0        0     6466 2023-01-06 09:50:21.000000 apscale-1.6.3/apscale/__main__.py
--rw-rw-rw-   0        0        0     3547 2023-01-06 10:01:45.000000 apscale-1.6.3/apscale/a_create_project.py
--rw-rw-rw-   0        0        0     7023 2023-01-06 12:04:43.000000 apscale-1.6.3/apscale/b_pe_merging.py
--rw-rw-rw-   0        0        0     6732 2023-01-06 15:29:00.000000 apscale-1.6.3/apscale/c_primer_trimming.py
--rw-rw-rw-   0        0        0     7059 2023-01-06 15:28:42.000000 apscale-1.6.3/apscale/d_quality_filtering.py
--rw-rw-rw-   0        0        0    11383 2023-01-10 16:10:43.000000 apscale-1.6.3/apscale/e_dereplication_pooling.py
--rw-rw-rw-   0        0        0    14065 2023-01-06 14:39:50.000000 apscale-1.6.3/apscale/f_otu_clustering.py
--rw-rw-rw-   0        0        0    13937 2023-01-06 14:49:41.000000 apscale-1.6.3/apscale/g_denoising.py
--rw-rw-rw-   0        0        0    20487 2023-01-06 15:03:43.000000 apscale-1.6.3/apscale/h_lulu_filtering.py
-drwxrwxrwx   0        0        0        0 2023-02-21 10:46:00.384762 apscale-1.6.3/apscale.egg-info/
--rw-rw-rw-   0        0        0     8528 2023-02-21 10:46:00.000000 apscale-1.6.3/apscale.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      492 2023-02-21 10:46:00.000000 apscale-1.6.3/apscale.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-21 10:46:00.000000 apscale-1.6.3/apscale.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-02-21 10:46:00.000000 apscale-1.6.3/apscale.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      157 2023-02-21 10:46:00.000000 apscale-1.6.3/apscale.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-02-21 10:46:00.000000 apscale-1.6.3/apscale.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-21 10:46:00.385763 apscale-1.6.3/setup.cfg
--rw-rw-rw-   0        0        0     1235 2023-02-21 10:45:44.000000 apscale-1.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:06:08.016601 apscale-1.7.0/
+-rw-rw-rw-   0        0        0     1093 2022-01-25 10:07:17.000000 apscale-1.7.0/LICENSE
+-rw-rw-rw-   0        0        0       17 2022-04-05 12:21:44.000000 apscale-1.7.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     8845 2024-04-02 12:06:08.015601 apscale-1.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7496 2023-01-06 15:12:01.000000 apscale-1.7.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 12:06:07.995064 apscale-1.7.0/apscale/
+-rw-rw-rw-   0        0        0        0 2022-01-25 10:07:17.000000 apscale-1.7.0/apscale/__init__.py
+-rw-rw-rw-   0        0        0     6466 2023-01-06 09:50:21.000000 apscale-1.7.0/apscale/__main__.py
+-rw-rw-rw-   0        0        0     3547 2023-01-06 10:01:45.000000 apscale-1.7.0/apscale/a_create_project.py
+-rw-rw-rw-   0        0        0     7023 2023-01-06 12:04:43.000000 apscale-1.7.0/apscale/b_pe_merging.py
+-rw-rw-rw-   0        0        0     6732 2023-01-06 15:29:00.000000 apscale-1.7.0/apscale/c_primer_trimming.py
+-rw-rw-rw-   0        0        0     7059 2023-01-06 15:28:42.000000 apscale-1.7.0/apscale/d_quality_filtering.py
+-rw-rw-rw-   0        0        0    11383 2023-01-10 16:10:43.000000 apscale-1.7.0/apscale/e_dereplication_pooling.py
+-rw-rw-rw-   0        0        0    14320 2024-04-02 11:56:54.000000 apscale-1.7.0/apscale/f_otu_clustering.py
+-rw-rw-rw-   0        0        0    14192 2024-04-02 11:55:44.000000 apscale-1.7.0/apscale/g_denoising.py
+-rw-rw-rw-   0        0        0    20487 2023-01-06 15:03:43.000000 apscale-1.7.0/apscale/h_lulu_filtering.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:06:08.014602 apscale-1.7.0/apscale.egg-info/
+-rw-rw-rw-   0        0        0     8845 2024-04-02 12:06:07.000000 apscale-1.7.0/apscale.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      492 2024-04-02 12:06:07.000000 apscale-1.7.0/apscale.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 12:06:07.000000 apscale-1.7.0/apscale.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-02 12:06:07.000000 apscale-1.7.0/apscale.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      157 2024-04-02 12:06:07.000000 apscale-1.7.0/apscale.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-02 12:06:07.000000 apscale-1.7.0/apscale.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 12:06:08.016601 apscale-1.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     1235 2024-04-02 12:05:24.000000 apscale-1.7.0/setup.py
```

### Comparing `apscale-1.6.3/LICENSE` & `apscale-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `apscale-1.6.3/PKG-INFO` & `apscale-1.7.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,31 @@
 Metadata-Version: 2.1
 Name: apscale
-Version: 1.6.3
+Version: 1.7.0
 Summary: Advanced Pipeline for Simple yet Comprehensive AnaLysEs of DNA metabarcoding data
 Home-page: https://github.com/DominikBuchner/apscale
 Author: Dominik Buchner
 Author-email: dominik.buchner524@googlemail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: openpyxl>=3.0.10
+Requires-Dist: psutil>=5.8.0
+Requires-Dist: pandas>=1.5.0
+Requires-Dist: demultiplexer>=1.1.0
+Requires-Dist: joblib>=1.0.0
+Requires-Dist: biopython>=1.78
+Requires-Dist: cutadapt>=3.5
+Requires-Dist: tqdm>=4.56.0
+Requires-Dist: fastparquet>=0.8.0
+Requires-Dist: pyarrow>=7.0.0
 
 # apscale
 Advanced Pipeline for Simple yet Comprehensive AnaLysEs of DNA metabarcoding data
 
 ## Introduction
 Apscale is a metabarcoding pipeline that handles the most common tasks in metabarcoding
 pipelines like paired-end merging, primer trimming, quality filtering, otu clustering and
```

### Comparing `apscale-1.6.3/README.md` & `apscale-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `apscale-1.6.3/apscale/__main__.py` & `apscale-1.7.0/apscale/__main__.py`

 * *Files identical despite different names*

### Comparing `apscale-1.6.3/apscale/a_create_project.py` & `apscale-1.7.0/apscale/a_create_project.py`

 * *Files identical despite different names*

### Comparing `apscale-1.6.3/apscale/b_pe_merging.py` & `apscale-1.7.0/apscale/b_pe_merging.py`

 * *Files identical despite different names*

### Comparing `apscale-1.6.3/apscale/c_primer_trimming.py` & `apscale-1.7.0/apscale/c_primer_trimming.py`

 * *Files identical despite different names*

### Comparing `apscale-1.6.3/apscale/d_quality_filtering.py` & `apscale-1.7.0/apscale/d_quality_filtering.py`

 * *Files identical despite different names*

### Comparing `apscale-1.6.3/apscale/e_dereplication_pooling.py` & `apscale-1.7.0/apscale/e_dereplication_pooling.py`

 * *Files identical despite different names*

### Comparing `apscale-1.6.3/apscale/f_otu_clustering.py` & `apscale-1.7.0/apscale/f_otu_clustering.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from joblib import Parallel, delayed
 from pathlib import Path
 from Bio.SeqIO.FastaIO import SimpleFastaParser
 from io import StringIO
 from tqdm import tqdm
 from openpyxl.utils.dataframe import dataframe_to_rows
 
+
 ## clustering function to cluster all sequences in input fasta with given pct_id
 def otu_clustering(project=None, comp_lvl=None, cores=None, pct_id=None):
     """Function to apply OTU clustering to a given gzipped file. Outputs a fasta file
     with all centroid sequences."""
 
     ## define the name for the output fasta
     ## create an output path to write to
@@ -310,15 +311,15 @@
                 Path(project).joinpath(
                     "7_otu_clustering", "{}_OTUs.fasta".format(Path(project).stem)
                 )
             )
         )
     )
     otu_table = pd.DataFrame(otu_list, columns=["ID", "Seq"])
-    seq_col = otu_table.pop("Seq")
+    seq_dict = dict(zip(otu_table["ID"], otu_table.pop("Seq")))
 
     ## extract individual OTU tabs from the clustering output, rename columns correctly, merge all individual tabs with the otu table frame
     otu_tabs = glob.glob(
         str(Path(project).joinpath("7_otu_clustering", "temp", "*_otu_tab.pkl"))
     )
     otu_tabs = [pickle.load(open(tab_file, "rb")) for tab_file in otu_tabs]
     otu_tabs = [tab.rename(columns={tab.columns[0]: "ID"}) for tab in otu_tabs]
@@ -336,15 +337,20 @@
             otu_table[otu_table.columns.difference(["ID"])].sort_index(axis=1),
         ],
         ignore_index=False,
         axis=1,
     )
 
     ## move sequences to the end of the dataframe
-    otu_table.insert(len(otu_table.columns), "Seq", seq_col)
+    otu_table["Seq"] = otu_table["ID"].map(seq_dict)
+
+    ## sort the OTU table by OTU nr
+    otu_table["sort"] = otu_table["ID"].str.split("_").str[-1].astype("int")
+    otu_table = otu_table.sort_values(by="sort", axis=0)
+    otu_table = otu_table.drop(labels=["sort"], axis=1)
 
     ## save the final OTU table if option is selected
     if to_excel:
         wb = openpyxl.Workbook(write_only=True)
         ws = wb.create_sheet("OTU table")
 
         ## save the output line by line for optimized memory usage
```

### Comparing `apscale-1.6.3/apscale/g_denoising.py` & `apscale-1.7.0/apscale/g_denoising.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from joblib import Parallel, delayed
 from pathlib import Path
 from Bio.SeqIO.FastaIO import SimpleFastaParser
 from io import StringIO
 from tqdm import tqdm
 from openpyxl.utils.dataframe import dataframe_to_rows
 
+
 ## denoising function to denoise all sequences the input fasta with a given alpha and minsize
 def denoise(project=None, comp_lvl=None, cores=None, alpha=None, minsize=None):
     """Function to apply denoisind to a given gzipped file. Outputs a fasta file with all
     centroid sequences."""
 
     ## define the name for the output fasta
     ## create an output path to write to
@@ -319,15 +320,15 @@
                 Path(project).joinpath(
                     "8_denoising", "{}_ESVs.fasta".format(Path(project).stem)
                 )
             )
         )
     )
     esv_table = pd.DataFrame(esv_list, columns=["ID", "Seq"])
-    seq_col = esv_table.pop("Seq")
+    seq_dict = dict(zip(esv_table["ID"], esv_table.pop("Seq")))
 
     ## extract individual ESV tabs from the clustering output, rename columns correctly, merge individual tabs
     esv_tabs = glob.glob(
         str(Path(project).joinpath("8_denoising", "temp", "*_esv_tab.pkl"))
     )
     esv_tabs = [pickle.load(open(tab_file, "rb")) for tab_file in esv_tabs]
     esv_tabs = [tab.rename(columns={tab.columns[0]: "ID"}) for tab in esv_tabs]
@@ -345,15 +346,20 @@
             esv_table[esv_table.columns.difference(["ID"])].sort_index(axis=1),
         ],
         ignore_index=False,
         axis=1,
     )
 
     ## move sequences to the end of the dataframe
-    esv_table.insert(len(esv_table.columns), "Seq", seq_col)
+    esv_table["Seq"] = esv_table["ID"].map(seq_dict)
+
+    ## sort the ESV table by OTU nr
+    esv_table["sort"] = esv_table["ID"].str.split("_").str[-1].astype("int")
+    esv_table = esv_table.sort_values(by="sort", axis=0)
+    esv_table = esv_table.drop(labels=["sort"], axis=1)
 
     ## save the final OTU table if selected
     if to_excel:
         wb = openpyxl.Workbook(write_only=True)
         ws = wb.create_sheet("ESV table")
 
         ## save the output line by line for optimized memory usage
```

### Comparing `apscale-1.6.3/apscale/h_lulu_filtering.py` & `apscale-1.7.0/apscale/h_lulu_filtering.py`

 * *Files identical despite different names*

### Comparing `apscale-1.6.3/apscale.egg-info/PKG-INFO` & `apscale-1.7.0/apscale.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,31 @@
 Metadata-Version: 2.1
 Name: apscale
-Version: 1.6.3
+Version: 1.7.0
 Summary: Advanced Pipeline for Simple yet Comprehensive AnaLysEs of DNA metabarcoding data
 Home-page: https://github.com/DominikBuchner/apscale
 Author: Dominik Buchner
 Author-email: dominik.buchner524@googlemail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: openpyxl>=3.0.10
+Requires-Dist: psutil>=5.8.0
+Requires-Dist: pandas>=1.5.0
+Requires-Dist: demultiplexer>=1.1.0
+Requires-Dist: joblib>=1.0.0
+Requires-Dist: biopython>=1.78
+Requires-Dist: cutadapt>=3.5
+Requires-Dist: tqdm>=4.56.0
+Requires-Dist: fastparquet>=0.8.0
+Requires-Dist: pyarrow>=7.0.0
 
 # apscale
 Advanced Pipeline for Simple yet Comprehensive AnaLysEs of DNA metabarcoding data
 
 ## Introduction
 Apscale is a metabarcoding pipeline that handles the most common tasks in metabarcoding
 pipelines like paired-end merging, primer trimming, quality filtering, otu clustering and
```

### Comparing `apscale-1.6.3/setup.py` & `apscale-1.7.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="apscale",
-    version="1.6.3",
+    version="1.7.0",
     author="Dominik Buchner",
     author_email="dominik.buchner524@googlemail.com",
     description="Advanced Pipeline for Simple yet Comprehensive AnaLysEs of DNA metabarcoding data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/DominikBuchner/apscale",
     packages=setuptools.find_packages(),
```

