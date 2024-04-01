# Comparing `tmp/mDeepFRI-1.1.4.tar.gz` & `tmp/mDeepFRI-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mDeepFRI-1.1.4.tar", last modified: Sat Mar 23 19:02:23 2024, max compression
+gzip compressed data, was "mDeepFRI-1.1.5.tar", last modified: Mon Apr  1 22:16:58 2024, max compression
```

## Comparing `mDeepFRI-1.1.4.tar` & `mDeepFRI-1.1.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:02:23.979736 mDeepFRI-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-03-23 19:02:14.000000 mDeepFRI-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10459 2024-03-23 19:02:23.979736 mDeepFRI-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9482 2024-03-23 19:02:14.000000 mDeepFRI-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:02:23.975736 mDeepFRI-1.1.4/mDeepFRI/
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-03-23 19:02:14.000000 mDeepFRI-1.1.4/mDeepFRI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-03-23 19:02:14.000000 mDeepFRI-1.1.4/mDeepFRI/alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-03-23 19:02:14.000000 mDeepFRI-1.1.4/mDeepFRI/alignment_utils.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    16248 2024-03-23 19:02:14.000000 mDeepFRI-1.1.4/mDeepFRI/bio_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-03-23 19:02:14.000000 mDeepFRI-1.1.4/mDeepFRI/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-03-23 19:02:14.000000 mDeepFRI-1.1.4/mDeepFRI/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     6776 2024-03-23 19:02:14.000000 mDeepFRI-1.1.4/mDeepFRI/mmseqs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-03-23 19:02:14.000000 mDeepFRI-1.1.4/mDeepFRI/pdb.py
--rw-r--r--   0 runner    (1001) docker     (127)    10448 2024-03-23 19:02:14.000000 mDeepFRI-1.1.4/mDeepFRI/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-03-23 19:02:14.000000 mDeepFRI-1.1.4/mDeepFRI/predict.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:02:23.979736 mDeepFRI-1.1.4/mDeepFRI/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 19:02:14.000000 mDeepFRI-1.1.4/mDeepFRI/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-03-23 19:02:14.000000 mDeepFRI-1.1.4/mDeepFRI/tests/test_alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-03-23 19:02:14.000000 mDeepFRI-1.1.4/mDeepFRI/tests/test_bio_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 19:02:14.000000 mDeepFRI-1.1.4/mDeepFRI/tests/test_build_database.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-03-23 19:02:14.000000 mDeepFRI-1.1.4/mDeepFRI/tests/test_install.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-23 19:02:14.000000 mDeepFRI-1.1.4/mDeepFRI/tests/test_pdb.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-23 19:02:14.000000 mDeepFRI-1.1.4/mDeepFRI/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7475 2024-03-23 19:02:14.000000 mDeepFRI-1.1.4/mDeepFRI/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:02:23.979736 mDeepFRI-1.1.4/mDeepFRI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10459 2024-03-23 19:02:23.000000 mDeepFRI-1.1.4/mDeepFRI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-23 19:02:23.000000 mDeepFRI-1.1.4/mDeepFRI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 19:02:23.000000 mDeepFRI-1.1.4/mDeepFRI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-23 19:02:23.000000 mDeepFRI-1.1.4/mDeepFRI.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 19:02:23.000000 mDeepFRI-1.1.4/mDeepFRI.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-23 19:02:23.000000 mDeepFRI-1.1.4/mDeepFRI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-23 19:02:23.000000 mDeepFRI-1.1.4/mDeepFRI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-03-23 19:02:14.000000 mDeepFRI-1.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-03-23 19:02:23.979736 mDeepFRI-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6502 2024-03-23 19:02:14.000000 mDeepFRI-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:16:58.931135 mDeepFRI-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-01 22:16:51.000000 mDeepFRI-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12564 2024-04-01 22:16:58.931135 mDeepFRI-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-04-01 22:16:51.000000 mDeepFRI-1.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:16:58.927135 mDeepFRI-1.1.5/mDeepFRI/
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-04-01 22:16:51.000000 mDeepFRI-1.1.5/mDeepFRI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-04-01 22:16:51.000000 mDeepFRI-1.1.5/mDeepFRI/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7398 2024-04-01 22:16:51.000000 mDeepFRI-1.1.5/mDeepFRI/alignment_utils.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    10029 2024-04-01 22:16:51.000000 mDeepFRI-1.1.5/mDeepFRI/bio_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7705 2024-04-01 22:16:51.000000 mDeepFRI-1.1.5/mDeepFRI/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-04-01 22:16:51.000000 mDeepFRI-1.1.5/mDeepFRI/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7379 2024-04-01 22:16:51.000000 mDeepFRI-1.1.5/mDeepFRI/mmseqs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-04-01 22:16:51.000000 mDeepFRI-1.1.5/mDeepFRI/pdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12900 2024-04-01 22:16:51.000000 mDeepFRI-1.1.5/mDeepFRI/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-04-01 22:16:51.000000 mDeepFRI-1.1.5/mDeepFRI/predict.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:16:58.931135 mDeepFRI-1.1.5/mDeepFRI/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:16:51.000000 mDeepFRI-1.1.5/mDeepFRI/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-01 22:16:51.000000 mDeepFRI-1.1.5/mDeepFRI/tests/test_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-01 22:16:51.000000 mDeepFRI-1.1.5/mDeepFRI/tests/test_bio_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-01 22:16:51.000000 mDeepFRI-1.1.5/mDeepFRI/tests/test_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-01 22:16:51.000000 mDeepFRI-1.1.5/mDeepFRI/tests/test_pdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-01 22:16:51.000000 mDeepFRI-1.1.5/mDeepFRI/tests/test_predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-01 22:16:51.000000 mDeepFRI-1.1.5/mDeepFRI/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-04-01 22:16:51.000000 mDeepFRI-1.1.5/mDeepFRI/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:16:58.927135 mDeepFRI-1.1.5/mDeepFRI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12564 2024-04-01 22:16:58.000000 mDeepFRI-1.1.5/mDeepFRI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-01 22:16:58.000000 mDeepFRI-1.1.5/mDeepFRI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 22:16:58.000000 mDeepFRI-1.1.5/mDeepFRI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-01 22:16:58.000000 mDeepFRI-1.1.5/mDeepFRI.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 22:16:58.000000 mDeepFRI-1.1.5/mDeepFRI.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-01 22:16:58.000000 mDeepFRI-1.1.5/mDeepFRI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 22:16:58.000000 mDeepFRI-1.1.5/mDeepFRI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-01 22:16:51.000000 mDeepFRI-1.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-01 22:16:58.931135 mDeepFRI-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-04-01 22:16:51.000000 mDeepFRI-1.1.5/setup.py
```

### Comparing `mDeepFRI-1.1.4/LICENSE` & `mDeepFRI-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mDeepFRI-1.1.4/PKG-INFO` & `mDeepFRI-1.1.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,13 @@
-Metadata-Version: 2.1
-Name: mDeepFRI
-Version: 1.1.4
-Summary: Pipeline for searching and aligning contact maps for proteins, then running DeepFri's GCN.
-Home-page: https://github.com/bioinf-mcb/Metagenomic-DeepFRI
-Download-URL: https://github.com/bioinf-mcb/Metagenomic-DeepFRI
-Author:  Valentyn Bezshapkin, Piotr Kucharski
-Author-email: valentyn.bezshapkin@micro.biol.ethz.ch, soliareofastorauj@gmail.com
-License: BSD-3-Clause
-Keywords: protein function metagenomics deep neural network
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # 🍳 Metagenomic-DeepFRI [![Stars](https://img.shields.io/github/stars/bioinf-MCB/Metagenomic-DeepFRI.svg?style=social&maxAge=3600&label=Star)](https://github.com/bioinf-MCB/Metagenomic-DeepFRI/stargazers)
 *A pipeline for annotation of genes with [DeepFRI](https://github.com/flatironinstitute/DeepFRI), a deep learning model for functional protein annotation with [Gene Ontology (GO) terms](https://geneontology.org/docs/go-annotations/). It incorporates [FoldComp](https://github.com/steineggerlab/foldcomp) databases of predicted protein structures for fast annotation of metagenomic gene catalogues.*
 
 ## 🔍 Overview
 Proteins perform most of the work of living cells. Amino acid sequence and structural features of proteins determine a wide range of functions: from binding specificity and conferring mechanical stability, to catalysis of biochemical reactions, transport, and signal transduction.
-DeepFRI is a neural network designed to predict protein function within the framework of the Gene Ontology (GO). The exponential growth in the number of available protein sequences, driven by advancements in low-cost sequencing technologies and computational methods (e.g., gene prediction), has resulted in a pressing need for efficient software to facilitate the annotation of protein databases.
+DeepFRI is a neural network designed to predict protein function within the framework of the Gene Ontology (GO). The exponential growth in the number of available protein sequences, driven by advancements in low-cost sequencing technologies and computational methods (e.g. gene prediction), has resulted in a pressing need for efficient software to facilitate the annotation of protein databases.
 Metagenomic-DeepFRI addresses such need, building upon efficient libraries. It incorporates novel databases of predicted structures (AlphaFold, ESMFold, MIP, etc.) and improves runtimes of DeepFRI by [2-12 times](https://github.com/bioinf-mcb/Metagenomic-DeepFRI/blob/main/weight_convert/onnx_vs_tf2.png)!
 
 ### 📋 Pipeline stages
 
 1. Search proteins similar to query in PDB and supplied `FoldComp` databases with `MMSeqs2`.
 2. Find the best alignment among `MMSeqs2` hits using `PyOpal`.
 3. Align target protein contact map to query protein with unknown structure.
@@ -41,36 +19,63 @@
 * [pyOpal](https://github.com/althonos/pyOpal)
 * [DeepFRI](https://github.com/flatironinstitute/DeepFRI)
 * [FoldComp](https://github.com/steineggerlab/foldcomp)
 * [ONNX](https://github.com/onnx/onnx)
 
 ## 🔧 Installation
 
-1. Clone repo locally
+1. Download environment YAML.
 ```{code-block} bash
-git clone https://github.com/bioinf-mcb/Metagenomic-DeepFRI
-cd Metagenomic-DeepFRI
+wget https://raw.githubusercontent.com/bioinf-mcb/Metagenomic-DeepFRI/main/environment.yml
 ```
-2. Setup conda environment
+2. Setup conda environment and actiate it.
 ```{code-block} bash
 conda env create --name deepfri --file environment.yml
 conda activate deepfri
+# Optional cleanup
+rm environment.yml
 ```
-3. Show help message
+3. Run and view the help message.
 ```{code-block} bash
 mDeepFRI --help
 ```
 
 ## 💡 Usage
 ### 1. Prepare structural database
-The PDB database will be automatically downloaded and installed during first run of `mDeepFRI`. You can download additional databases from [website](https://foldcomp.steineggerlab.workers.dev/). The app was tested with `afdb_swissprot_v4`. You can use different databases, but be mindful that computation time might increase exponentially with the size of the database.
+#### 1.1 Existing `FoldComp` databases
+The PDB database will be automatically downloaded and installed during first run of `mDeepFRI`. The PDB suffers from formatting inconsistencies, therefore during PDB alignment around 10% will fail and will be reported via `WARNING`. We suggest coupling PDB search with predicted databaes.
+
+You can download additional databases from [website](https://foldcomp.steineggerlab.workers.dev/). During a first run, FASTA sequences will be extracted from `FoldComp` database and `MMseqs2` database will be create and indexed. You can use different databases, but be mindful that computation time might increase exponentially with the size of the database.
+
+Tested databases:
+- `afdb_swissprot`
+- `afdb_swissprot_v4`
+- `afdb_rep_v4`
+- `afdb_rep_dark_v4`
+- `afdb_uniprot_v4`
+- `esmatlas`
+- `esmatlas_v2023_02`
+- `highquality_clust30`
+
+
+`ATTENTION:` Please, do not rename downloaded databases. `FoldComp` has certain inconsistencies in the way FASTA sequences are extracted ([example](https://github.com/steineggerlab/foldcomp/issues/51)), therefore pipeline was tweaked for each database. If database you need does not work, please report in [issues](https://github.com/bioinf-mcb/Metagenomic-DeepFRI/issues) and we will add it as soon as possible. Sorry for the inconvenience.
+
+`ATTENTION:` database creation is a very sensitive step which relies on external software. If pipeline is interrupted during this step, the databases might be corrupted. If you are not sure about your database, rerun the pipeline with `--overwrite` flag - it will rerun database creation process.
+
+#### 1.2. Custom `FoldComp` database
+In order to use personal database of structures, you will have to create a custom FoldComp database. For that, download a `FoldComp` executable and run  the following command:
+```
+foldcomp compress [-t number] <dir|tar(.gz)> [<dir|tar|db>]
+```
+
 ### 2. Download models
 Two versions of models available:
 - `v1.0` - is the original version from DeepFRI publication.
-- `v1.1` - is a version finetuned on AlphaFold models and Gene Ontology Uniprot annotations.
+- `v1.1` - is a version finetuned on AlphaFold models and machine-generated Gene Ontology Uniprot annotations. You can read details about `v1.1` in [ISMB 2023 presentation by Pawel Szczerbiak](https://docs.google.com/presentation/d/1Pzn_gQH5-dDImpApSoWFQNu3WByFZYWqfesplANK9hI/edit?usp=sharing)
+
 To download models run command:
 ```
 mDeepFRI get-models --output path/to/weights/folder -v {1.0 or 1.1}
 ```
 
 ### 3. Predict protein function & capture log
 ```
@@ -94,22 +99,25 @@
 | unaligned | 3.2.1.-          | 0.215 | 3.2.1.-                        | cnn        | ec           | nan | nan | nan
 
 This is an example of protein annotation with the AlphaFold database.
 - Protein - the name of the protein from the FASTA file.
 - GO_term/EC_numer - predicted GO term or EC number (dependent on mode)
 - Score - DeepFRI score, translates to model confidence in prediction. Details in [publication](https://www.nature.com/articles/s41467-021-23303-9).
 - Annotation - annotation from ontology
-- Neural_net - type of neural network used for prediction (gcn = Graph Convolutional Network; cnn = Convolutional Neural Network). GCN (Graph Convolutional Network) is employed when structural information is available in the database, allowing for generally more confident predictions.
+- Neural_net - type of neural network used for prediction (gcn = Graph Convolutional Network; cnn = Convolutional Neural Network). GCN (Graph Convolutional Network) is used when structural information is available in the database, allowing for generally more confident predictions. When there are no proteins above similarity cut-off (50% identity by default), CNN is used.
 - DeepFRI_mode:
    ```
    mf = molecular_function
    bp = biological_process
    cc = cellular_component
    ec = enzyme_commission
    ```
+- DB_hit - name of the hit in the database. Empty if no hit was found.
+- DB_name - name of the database. Empty if no hit was found.
+- Identity - sequence identity between query and hit. Empty if no hit was found.
 
 ## ⚙️Features
 ### 1. Prediction modes
 The GO ontology contains three subontologies, defined by their root nodes:
 - Molecular Function (MF)
 - Biological Process (BP)
 - Cellular Component (CC)
```

### Comparing `mDeepFRI-1.1.4/mDeepFRI/__init__.py` & `mDeepFRI-1.1.5/mDeepFRI/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 import os
 
-__version__ = "1.1.4"
+__version__ = "1.1.5"
 
 repo_url = "https://huggingface.co/valentynbez/mDeepFRI/resolve/main/"
 
+DEEPFRI_MODES = {
+    "bp": "GO Biological Process",
+    "cc": "GO Cellular Component",
+    "mf": "GO Molecular Function",
+    "ec": "Enzyme Commission"
+}
+
 cnn_model_links = {
     "bp": {
         "model": os.path.join(repo_url, "DeepCNN-MERGED_bp.onnx"),
         "config": os.path.join(repo_url, "DeepCNN-MERGED_bp_model_params.json")
     },
     "cc": {
         "model": os.path.join(repo_url, "DeepCNN-MERGED_cc.onnx"),
```

### Comparing `mDeepFRI-1.1.4/mDeepFRI/alignment.py` & `mDeepFRI-1.1.5/mDeepFRI/alignment.py`

 * *Files identical despite different names*

### Comparing `mDeepFRI-1.1.4/mDeepFRI/cli.py` & `mDeepFRI-1.1.5/mDeepFRI/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     required=True,
     type=click.Path(exists=True),
     help="Path to an input protein sequences (FASTA file, may be gzipped).",
 )
 @click.option(
     "-d",
     "--db-path",
-    required=True,
+    required=False,
     type=click.Path(exists=True),
     multiple=True,
     help="Path to a structures database compessed with FoldComp.",
 )
 @click.option(
     "-w",
     "--weights",
@@ -201,14 +201,36 @@
                      remove_intermediate, overwrite, threads, skip_pdb,
                      min_length, max_length):
     """Predict protein function from sequence."""
     logger.info("Starting Metagenomic-DeepFRI.")
 
     output_path = Path(output)
     output_path.mkdir(parents=True, exist_ok=True)
+    # write command parameters to log
+    logger.info("Command parameters:")
+    logger.info("Input:                         %s", input)
+    logger.info("Database:                      %s", db_path)
+    logger.info("Weights:                       %s", weights)
+    logger.info("Output:                        %s", output)
+    logger.info("Processing modes:              %s", processing_modes)
+    logger.info("Angstrom contact threshold:    %s", angstrom_contact_thresh)
+    logger.info("Generate contacts:             %s", generate_contacts)
+    logger.info("MMSeqs2 minimum bitscore:      %s", mmseqs_min_bitscore)
+    logger.info("MMSeqs2 maximum e-value:       %s", mmseqs_max_evalue)
+    logger.info("MMSeqs2 minimum identity:      %s", mmseqs_min_identity)
+    logger.info("Top k results:                 %s", top_k)
+    logger.info("Alignment gap open:            %s", alignment_gap_open)
+    logger.info("Alignment gap extend:          %s", alignment_gap_extend)
+    logger.info("Alignment minimum identity:    %s", alignment_min_identity)
+    logger.info("Remove intermediate:           %s", remove_intermediate)
+    logger.info("Overwrite:                     %s", overwrite)
+    logger.info("Threads:                       %s", threads)
+    logger.info("Skip PDB:                      %s", skip_pdb)
+    logger.info("Minimum length:                %s", min_length)
+    logger.info("Maximum length:                %s", max_length)
 
     predict_protein_function(
         query_file=input,
         databases=db_path,
         weights=weights,
         output_path=output_path,
         deepfri_processing_modes=processing_modes,
```

### Comparing `mDeepFRI-1.1.4/mDeepFRI/database.py` & `mDeepFRI-1.1.5/mDeepFRI/database.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# Create logger
 import logging
 from dataclasses import dataclass
 from pathlib import Path
 
 import numpy as np
 
 from mDeepFRI.mmseqs import (create_target_database, extract_fasta_foldcomp,
@@ -80,19 +79,19 @@
         logger.info("FASTA file extracted to %s", output_sequences)
         needs_new_mmseqs = True
 
     # create mmseqs db
     mmseqs_path = output_path / Path(input_path.stem + ".mmseqsDB")
     mmseqs_valid = validate_mmseqs_database(mmseqs_path)
     if not mmseqs_valid:
-        logger.info("Creating MMSeqs2 database.")
-        create_target_database(output_sequences, mmseqs_path)
+        logger.info("Creating and indexing MMSeqs2 database.")
+        create_target_database(output_sequences, mmseqs_path, threads)
     elif overwrite or needs_new_mmseqs:
-        logger.info("Creating MMSeqs2 database.")
-        create_target_database(output_sequences, mmseqs_path)
+        logger.info("Creating and indexing MMSeqs2 database.")
+        create_target_database(output_sequences, mmseqs_path, threads)
     else:
         logger.info("Database created at %s", output_path)
         logger.info("Found %s in %s", mmseqs_path, output_path)
         logger.info("Skipping creation of MMSeqs2 database.")
 
     database = Database(foldcomp_db=input_path,
                         sequence_db=output_sequences,
```

### Comparing `mDeepFRI-1.1.4/mDeepFRI/mmseqs.py` & `mDeepFRI-1.1.5/mDeepFRI/mmseqs.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 
 MMSEQS_COLUMN_NAMES = [
     "query", "target", "identity", "alignment_length", "mismatches",
     "gap_openings", "query_start", "query_end", "target_start", "target_end",
     "e_value", "bit_score"
 ]
 
+ESM_DATABASES = ["highquality_clust30", "esmatlas", "esmatlas_v2023_02"]
+
 logging.basicConfig(
     level=logging.DEBUG,
     format='[%(asctime)s] %(module)s.%(funcName)s %(levelname)s: %(message)s',
     datefmt='%Y-%m-%d %H:%M:%S')
 
 logger = logging.getLogger(__name__)
 
@@ -37,17 +39,18 @@
 
     Returns:
         None
     """
     run_command(f"mmseqs createdb {sequences_file} {db_path} --dbtype 1")
 
 
-def createindex(db_path):
+def createindex(db_path: str, threads: int = 1):
     with tempfile.TemporaryDirectory() as tmp_path:
-        run_command(f"mmseqs createindex {db_path} {tmp_path}")
+        run_command(
+            f"mmseqs createindex {db_path} {tmp_path} --threads {threads}")
 
 
 def search(query_db: str, target_db: str, result_db: str, threads: int = 1):
     with tempfile.TemporaryDirectory() as tmp_path:
         run_command(
             f"mmseqs search --threads {threads} {query_db} {target_db} {result_db} {tmp_path}"
         )
@@ -62,41 +65,56 @@
 def extract_fasta_foldcomp(foldcomp_db: str,
                            output_file: str,
                            threads: int = 1):
     """
     Extracts FASTA from database
     """
     foldcomp_bin = Path(mDeepFRI.__path__[0]).parent / "foldcomp_bin"
+    database_name = Path(foldcomp_db).stem
 
     # run command
     run_command(
         f"{foldcomp_bin} extract --fasta -t {threads} {foldcomp_db} {output_file}"
     )
+
+    if database_name in ESM_DATABASES:
+        # use sed to correct the headers
+        os.system(
+            fr"sed -i 's/^>\(ESMFOLD V0 PREDICTION FOR \)\(.*\)/>\2/' {output_file}"
+        )
+
     # gzip fasta file
     tabix_compress(output_file, str(output_file) + ".gz", force=True)
     # remove unzipped file
     os.remove(output_file)
+    # remove possible previous index, might lead to errror
+    try:
+        os.remove(str(output_file) + ".gz.fai")
+        os.remove(str(output_file) + ".gz.gzi")
+    except FileNotFoundError:
+        pass
+
     return Path(str(output_file) + ".gz")
 
 
 def create_target_database(foldcomp_fasta_path: str,
-                           mmseqs_db_path: str) -> None:
+                           mmseqs_db_path: str,
+                           threads: int = 1) -> None:
     """
     Extracts sequences from compressed FoldComp database.
 
     Args:
         foldcomp_db_path (str): Path to FoldComp database.
         new_db_path (str): Path to new MMSeqs database.
 
     Returns:
         None
     """
     createdb(foldcomp_fasta_path, mmseqs_db_path)
-    logger.info("Indexing new target mmseqs2 database %s", mmseqs_db_path)
-    createindex(mmseqs_db_path)
+    createindex(mmseqs_db_path, threads)
 
 
 def validate_mmseqs_database(database: str):
     """
     Check if MMSeqs2 database is intact.
 
     Args:
@@ -113,15 +131,15 @@
         ".idx.index", ".idx.dbtype", ".lookup", ".source"
     ]
 
     target_db = Path(database)
     is_valid = True
     for ext in mmseqs2_ext:
         if not os.path.isfile(f"{target_db}{ext}"):
-            logging.debug(f"{target_db}{ext} is missing.")
+            logger.debug(f"{target_db}{ext} is missing.")
             is_valid = False
             break
 
     return is_valid
 
 
 def run_mmseqs_search(query_file: str,
@@ -206,11 +224,12 @@
         output.sort(order=["query", "identity", "e_value"], kind="quciksort")
         top_k_db = partial(select_top_k, db=output[::-1], k=k_best_hits)
         with ThreadPool(threads) as pool:
             top_k_chunks = pool.map(top_k_db, np.unique(output["query"]))
 
         final_database = np.concatenate(top_k_chunks)
 
+        ## TODO: move logging module a level up
         logger.info("%i pairs after filtering with k=%i best hits.",
                     final_database.shape[0], k_best_hits)
 
     return final_database
```

### Comparing `mDeepFRI-1.1.4/mDeepFRI/pipeline.py` & `mDeepFRI-1.1.5/mDeepFRI/pipeline.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 import csv
 import logging
 import pathlib
 from functools import partial
 from multiprocessing import Pool
 from typing import List, Tuple
 
+import foldcomp
 import numpy as np
+from tqdm import tqdm
 
+from mDeepFRI import DEEPFRI_MODES
 from mDeepFRI.alignment import run_alignment
-from mDeepFRI.bio_utils import load_fasta_as_dict, retrieve_align_contact_map
+from mDeepFRI.bio_utils import (build_align_contact_map,
+                                extract_residues_coordinates,
+                                foldcomp_sniff_suffix, load_fasta_as_dict)
 from mDeepFRI.database import build_database
-from mDeepFRI.pdb import create_pdb_mmseqs
+from mDeepFRI.pdb import create_pdb_mmseqs, get_pdb_seq_coords
 from mDeepFRI.predict import Predictor
 from mDeepFRI.utils import load_deepfri_config, remove_intermediate_files
 
 logging.basicConfig(
     level=logging.DEBUG,
     format='[%(asctime)s] %(module)s.%(funcName)s %(levelname)s: %(message)s',
     datefmt='%Y-%m-%d %H:%M:%S')
 
 logger = logging.getLogger(__name__)
+BAR_FORMAT = "{l_bar}{bar}| {n_fmt}/{total_fmt} [{elapsed}], {rate_fmt}{postfix}"
 
 
 def predict_protein_function(
         query_file: str,
         databases: Tuple[str],
         weights: str,
         output_path: str,
@@ -42,16 +48,14 @@
         threads: int = 1,
         skip_pdb: bool = False,
         min_length: int = 60,
         max_length: int = 1000):
 
     MIN_SEQ_LEN = min_length
     MAX_SEQ_LEN = max_length
-    logger.info("DeepFRI protein sequence limit: %i-%i aa.", MIN_SEQ_LEN,
-                MAX_SEQ_LEN)
 
     query_file = pathlib.Path(query_file)
     weights = pathlib.Path(weights)
     output_path = pathlib.Path(output_path)
     output_path.mkdir(parents=True, exist_ok=True)
 
     deepfri_models_config = load_deepfri_config(weights)
@@ -87,20 +91,37 @@
             output_path=database.parent,
             overwrite=overwrite,
             threads=threads,
         )
         deepfri_dbs.append(db)
 
     query_seqs = load_fasta_as_dict(query_file)
+    # sort dictionary by length
+    query_seqs = dict(sorted(query_seqs.items(), key=lambda x: len(x[1])))
+
+    # filter query seqs and log their sizes
+    to_remove = []
+    for seq in query_seqs:
+        if len(query_seqs[seq]) < MIN_SEQ_LEN:
+            logger.info("Skipping %s; sequence too short %i aa", seq,
+                        len(query_seqs[seq]))
+            to_remove.append(seq)
+        elif len(query_seqs[seq]) > MAX_SEQ_LEN:
+            logger.info("Skipping %s; sequence too long %i aa", seq,
+                        len(query_seqs[seq]))
+            to_remove.append(seq)
+
+    for seq in to_remove:
+        del query_seqs[seq]
+
     aligned_cmaps = []
 
     for db in deepfri_dbs:
         # SEQUENCE ALIGNMENT
         # calculate already aligned sequences
-        aligned = len(aligned_cmaps)
         logger.info("Aligning %s sequences against %s.", len(query_seqs),
                     db.name)
 
         # align new sequences agains db
         alignments = run_alignment(query_file, db.mmseqs_db, db.sequence_db,
                                    output_path, mmseqs_min_bitscore,
                                    mmseqs_max_eval, mmseqs_min_identity, top_k,
@@ -125,41 +146,80 @@
         for aln in alignments:
             aln.db_name = db.name
 
         aligned_queries = [aln[0].query_name for aln in aligned_cmaps]
         new_alignments = {
             aln.query_name: aln
             for aln in alignments if aln.query_name not in aligned_queries
+            and aln.query_name in query_seqs
         }
 
         # CONTACT MAP ALIGNMENT
         # initially designed as a separate step
         # some protein structures in PDB are not formatted correctly
         # so contact map alignment fails for them
         # for this cases we replace closest experimental structure with
         # closest predicted structure if available
         # if no alignments were found - report
-        logger.info("Aligning contact maps for %i proteins against %s.",
-                    len(new_alignments), db.name)
 
-        partial_align = partial(retrieve_align_contact_map,
-                                database=db.foldcomp_db,
+        query_ids = [aln.query_name for aln in new_alignments.values()]
+        target_ids = [
+            aln.target_name.rsplit(".", 1)[0]
+            for aln in new_alignments.values()
+        ]
+
+        # extract structural information
+        # in form of C-alpha coordinates
+        if "pdb100" in db.name:
+            with Pool(threads) as p:
+                iterable = zip(target_ids, query_ids)
+                _, coords = zip(*p.starmap(get_pdb_seq_coords, iterable))
+
+        else:
+            suffix = foldcomp_sniff_suffix(target_ids[0], db.foldcomp_db)
+            if suffix:
+                target_ids = [f"{t}{suffix}" for t in target_ids]
+
+            # extracting coordinates from FoldComp
+            with foldcomp.open(db.foldcomp_db, ids=target_ids) as struct_db:
+                coords = [
+                    extract_residues_coordinates(struct, filetype="pdb")[1]
+                    for _, struct in struct_db
+                ]
+
+        for aln, coord in zip(new_alignments.values(), coords):
+            aln.coords = coord
+
+        partial_align = partial(build_align_contact_map,
                                 threshold=angstrom_contact_threshold,
                                 generated_contacts=generate_contacts)
 
         with Pool(threads) as p:
-            partial_cmaps = p.map(partial_align, new_alignments.values())
+            # align with progress bar
+            partial_cmaps = list(
+                tqdm(
+                    p.imap(partial_align, new_alignments.values()),
+                    total=len(new_alignments),
+                    miniters=len(new_alignments) // 10,
+                    desc=f"Aligning contact maps against {db.name}",
+                    bar_format=BAR_FORMAT,
+                ))
 
         # filter errored contact maps
         # returned as Tuple[AlignmentResult, None] from `retrieve_align_contact_map`
         partial_cmaps = [cmap for cmap in partial_cmaps if cmap[1] is not None]
         aligned_cmaps.extend(partial_cmaps)
-
-    # report alignments for each database
-    logger.info("Aligned %i sequences.", len(aligned_queries) - aligned)
+        aligned_database = round(len(partial_cmaps) / len(query_seqs) * 100, 2)
+        aligned_total = round(len(aligned_cmaps) / len(query_seqs) * 100, 2)
+        logger.info(
+            f"Aligned {len(partial_cmaps)}/{len(query_seqs)} ({aligned_database}% of total) proteins against {db.name}."
+        )
+        logger.info(
+            f"Aligned {len(aligned_cmaps)}/{len(query_seqs)} ({aligned_total}%) proteins in total."
+        )
 
     aligned_queries = [aln.query_name for aln in alignments]
     unaligned_queries = {
         k: v
         for k, v in query_seqs.items() if k not in aligned_queries
     }
 
@@ -168,14 +228,17 @@
     # bp = biological_process
     # cc = cellular_component
     # ec = enzyme_commission
 
     # sort cmaps by length of query sequence
     aligned_cmaps = sorted(aligned_cmaps,
                            key=lambda x: len(x[0].query_sequence))
+    # sort unaligned queries by length
+    unaligned_queries = dict(
+        sorted(unaligned_queries.items(), key=lambda x: len(x[1])))
 
     output_file_name = output_path / "results.tsv"
     output_buffer = open(output_file_name, "w", encoding="utf-8")
     csv_writer = csv.writer(output_buffer, delimiter="\t")
     csv_writer.writerow([
         'Protein',
         'GO_term/EC_number',
@@ -190,37 +253,41 @@
 
     # FUNCTION PREDICTION
     for i, mode in enumerate(deepfri_processing_modes):
         # GCN
         gcn_prots = len(aligned_cmaps)
         if gcn_prots > 0:
             net_type = "gcn"
-            logger.info("Processing mode: %s; %i/%i", mode, i + 1,
-                        len(deepfri_processing_modes))
+            logger.info("Processing mode: %s; %i/%i", DEEPFRI_MODES[mode],
+                        i + 1, len(deepfri_processing_modes))
             # GCN for queries with aligned contact map
-            logger.info("Predicting with GCN: %i proteins", gcn_prots)
             gcn_path = deepfri_models_config[net_type][mode]
 
             gcn = Predictor(gcn_path, threads=threads)
 
-            for i, (aln, aligned_cmap) in enumerate(aligned_cmaps):
+            for i, (aln, aligned_cmap) in tqdm(
+                    enumerate(aligned_cmaps),
+                    total=gcn_prots,
+                    miniters=len(aligned_cmaps) // 10,
+                    desc=f"Predicting with GCN ({DEEPFRI_MODES[mode]})",
+                    bar_format=BAR_FORMAT):
 
                 ### PROTEIN LENGTH CHECKS
                 if len(aln.query_sequence) < MIN_SEQ_LEN:
                     logger.info("Skipping %s; sequence too short %i aa",
                                 aln.query_name, len(aln.query_sequence))
                     continue
 
                 elif len(aln.query_sequence) > MAX_SEQ_LEN:
                     logger.info("Skipping %s; sequence too long - %i aa",
                                 aln.query_name, len(aln.query_sequence))
                     continue
 
-                logger.info("Predicting %s; %i/%i", aln.query_name, i + 1,
-                            gcn_prots)
+                logger.debug("Predicting %s; %i/%i", aln.query_name, i + 1,
+                             gcn_prots)
                 # running the actual prediction
                 prediction_rows = gcn.predict_function(
                     seqres=aln.query_sequence,
                     cmap=aligned_cmap,
                     chain=str(aln.query_name))
                 # writing the results to the output file
                 for row in prediction_rows:
@@ -237,49 +304,43 @@
         # CNN for queries without satisfying alignments
         cnn_prots = len(unaligned_queries)
         if cnn_prots > 0:
             net_type = "cnn"
             logger.info("Predicting with CNN: %i proteins", cnn_prots)
             cnn_path = deepfri_models_config[net_type][mode]
             cnn = Predictor(cnn_path, threads=threads)
-            for i, query_id in enumerate(unaligned_queries):
+            for i, query_id in tqdm(
+                    enumerate(unaligned_queries),
+                    total=cnn_prots,
+                    miniters=len(unaligned_queries) // 10,
+                    desc=f"Predicting with CNN ({DEEPFRI_MODES[mode]})",
+                    bar_format=BAR_FORMAT):
+
                 seq = query_seqs[query_id]
                 if len(seq) > MAX_SEQ_LEN:
-                    logger.info("Skipping %s; sequence too long %i", query_id,
-                                len(seq))
+                    logger.info("Skipping %s; sequence too long %i aa.",
+                                query_id, len(seq))
                     continue
 
                 elif len(seq) < MIN_SEQ_LEN:
-                    logger.info("Skipping %s; sequence too short %i", query_id,
-                                len(seq))
+                    logger.info("Skipping %s; sequence too short %i aa.",
+                                query_id, len(seq))
                     continue
 
-                logger.info("Predicting %s; %i/%i", query_id, i + 1, cnn_prots)
+                logger.debug("Predicting %s; %i/%i", query_id, i + 1,
+                             cnn_prots)
                 prediction_rows = cnn.predict_function(
                     seqres=query_seqs[query_id], chain=str(query_id))
                 for row in prediction_rows:
                     row.extend([net_type, mode])
                     row.extend([np.nan, np.nan, np.nan])
                     csv_writer.writerow(row)
 
             del cnn
 
     output_buffer.close()
 
-    # sort predictions by protein name and score
-    with open(output_file_name, "r", encoding="utf-8") as f:
-        reader = csv.reader(f, delimiter="\t")
-        header = next(reader)
-        # row[0] - protein name
-        # row[2] - DeepFRI score
-        rows = sorted(reader, key=lambda row: (str(row[0]), -float(row[2])))
-
-    with open(output_file_name, "w", encoding="utf-8") as f:
-        writer = csv.writer(f, delimiter="\t")
-        writer.writerow(header)
-        writer.writerows(rows)
-
     if remove_intermediate:
         for db in deepfri_dbs:
             remove_intermediate_files([db.sequence_db, db.mmseqs_db])
 
     logger.info("meta-DeepFRI finished successfully.")
```

### Comparing `mDeepFRI-1.1.4/mDeepFRI/predict.pyx` & `mDeepFRI-1.1.5/mDeepFRI/predict.pyx`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,68 @@
-import csv
 import json
 
 import numpy as np
 
 cimport numpy as np
 
 np.import_array()
 
+import operator
+
+import cython
 import onnxruntime as rt
 
-from mDeepFRI.bio_utils import seq2onehot
+
+@cython.boundscheck(False)
+@cython.wraparound(False)
+@cython.cdivision(True)
+@cython.initializedcheck(False)
+cpdef np.ndarray[float, ndim=2] seq2onehot(str seq):
+    """
+    Converts a protein sequence to 26-dim one-hot encoding.
+
+    Args:
+        seq (str): protein sequence
+
+    Returns:
+        np.ndarray: one-hot encoding of the protein sequence
+    """
+    cdef bytes seq_bytes = seq.encode()
+
+    cdef bytes chars = b"-DGULNTKHYWCPVSOIEFXQABZRM"
+    cdef int vocab_size = len(chars)
+    cdef int seq_len = len(seq)
+    cdef int i, j
+    cdef int[:, ::1] onehot_view = np.zeros((seq_len, vocab_size), dtype=np.int32)
+
+    for i in range(seq_len):
+        j = chars.find(seq_bytes[i])
+        if j != -1:
+            onehot_view[i, j] = 1
+        else:
+            raise ValueError(f"Invalid character in sequence: {seq[i]}")
+
+    return np.asarray(onehot_view, dtype=np.float32)
 
 
-## TODO: do not accumulate predictions, write them out to csv asap to avoid unneccessary RAM usage
 cdef class Predictor(object):
     """
     Class for loading trained models and computing GO/EC predictions and class activation maps (CAMs).
     """
 
-    cdef public bint gcn
     cdef public str model_path
     cdef public int threads
     cdef public dict prot2goterms
     cdef public dict goidx2chains
     cdef public np.ndarray gonames
     cdef public np.ndarray goterms
     cdef public np.ndarray thresh
     cdef public session
     cdef public np.ndarray Y_hat
     cdef public dict data
-    cdef public list test_prot_list
 
     def __init__(self, model_path: str, threads: int = 0):
         self.model_path = model_path
         self.threads = threads
 
         self._load_model()
 
@@ -52,65 +81,80 @@
         with open(self.model_path.rsplit(".", 1)[0] + "_model_params.json") as json_file:
             metadata = json.load(json_file)
 
         self.gonames = np.asarray(metadata['gonames'])
         self.goterms = np.asarray(metadata['goterms'])
         self.thresh = 0.1 * np.ones(len(self.goterms))
 
-    def predict_function(
-        self,
-        seqres: str,
-        cmap = None,
-        chain: str = "",
-    ):
-        """
-        Computes GO/EC predictions for a single protein chain from sequence and contact map.
-
-        Args:
-            seqres (str): protein sequence
-            cmap (np.array): contact map
-            chain (str): chain ID
-
-        Returns:
-            None
-        """
+    def forward_pass(self, seqres: str, cmap = None):
 
         cdef np.ndarray A
         cdef np.ndarray prediction
         cdef np.ndarray y
-        cdef list output_rows = []
-        cdef str go_term
-        cdef float score
-        cdef str annotation
 
-        self.Y_hat = np.zeros((1, len(self.goterms)), dtype=float)
-        self.data = {}
-        self.test_prot_list = [chain]
+        # self.data = {}
         S = seq2onehot(seqres)
         S = S.reshape(1, *S.shape)
         inputDetails = self.session.get_inputs()
         # if cmap present use GCN with 2 inputs - sequence + cmap
         if cmap is not None:
             A = cmap.reshape(1, *cmap.shape)
             prediction = self.session.run(
                 None, {
                     inputDetails[0].name: A.astype(np.float32),
                     inputDetails[1].name: S.astype(np.float32)
                 })[0]
-            self.data[chain] = [[A, S], seqres]
+            # self.data[chain] = [[A, S], seqres]
 
         # if no cmap use CNN with 1 input
         else:
             prediction = self.session.run(
                 None, {inputDetails[0].name: S.astype(np.float32)})[0]
-            self.data[chain] = [[S], seqres]
+            # self.data[chain] = [[S], seqres]
 
         y = prediction[:, :, 0].reshape(-1)
-        self.Y_hat[0] = y
+
+        return y
+
+    def format_predictions(self, y, chain: str = ""):
+
+        cdef list output_rows = []
+        cdef str go_term
+        cdef float score
+        cdef str annotation
+
         go_idx = np.where(y >= self.thresh)[0]
         for idx in go_idx:
             go_term = self.goterms[idx].item()
             score = float(y[idx])
             annotation = self.gonames[idx].item()
             output_rows.append([chain, go_term, score, annotation])
 
+        # Sort output_rows based on score in descending order
+        output_rows.sort(key=operator.itemgetter(2), reverse=True)
+
+        return output_rows
+
+
+    def predict_function(
+        self,
+        seqres: str,
+        cmap = None,
+        chain: str = ""
+    ):
+        """
+        Computes GO/EC predictions for a single protein chain from sequence and contact map.
+
+        Args:
+            seqres (str): protein sequence.
+            cmap (np.array): contact map.
+            chain (str): protein ID.
+
+        Returns:
+            list: list of GO/EC predictions.
+
+        """
+
+        y = self.forward_pass(seqres, cmap)
+        output_rows = self.format_predictions(y, chain)
+
         return output_rows
```

### Comparing `mDeepFRI-1.1.4/mDeepFRI/tests/test_alignment.py` & `mDeepFRI-1.1.5/mDeepFRI/tests/test_alignment.py`

 * *Files identical despite different names*

### Comparing `mDeepFRI-1.1.4/mDeepFRI/utils.py` & `mDeepFRI-1.1.5/mDeepFRI/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -153,60 +153,14 @@
         del config["gcn"]["ec"]
 
     config_name = "model_config.json"
     with open(weights_path / config_name, "w") as f:
         json.dump(config, f, indent=4, sort_keys=True)
 
 
-# def merge_files_binary(file_paths: list, output_path: pathlib.Path) -> None:
-#     """
-#     Merges files in binary format.
-
-#     Args:
-#         file_paths (list): List of paths to merge.
-#         output_path (str): Path to save the merged file.
-
-#     Returns:
-#         None
-#     """
-
-#     with open(output_path, 'wb') as writer:
-#         for input_file in file_paths:
-#             with open(input_file, 'rb') as reader:
-#                 shutil.copyfileobj(reader, writer)
-
-# def search_files_in_paths(paths: list, pattern: str):
-#     """
-#     Searches for files in paths.
-
-#     Args:
-#         paths (list): List of paths to search.
-#         pattern (str): Pattern to search for.
-
-#     Returns:
-#         list: List of files found.
-#     """
-
-#     files = []
-#     for path in paths:
-#         if not path.exists():
-#             print(f"Unable to locate {path}.")
-#             continue
-#         if path.is_dir():
-#             files.extend(list(path.glob("**/*" + pattern)))
-#         else:
-#             if not path.name.endswith(pattern):
-#                 print(
-#                     f"{path} is not an {pattern} file which is excepted format."
-#                 )
-#             else:
-#                 files.append(path)
-#     return files
-
-
 def shutdown(message):
     """
     Terminates program execution with a reason.
 
     Args:
         message (str): Reason for termination.
     """
```

### Comparing `mDeepFRI-1.1.4/mDeepFRI.egg-info/PKG-INFO` & `mDeepFRI-1.1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mDeepFRI
-Version: 1.1.4
+Version: 1.1.5
 Summary: Pipeline for searching and aligning contact maps for proteins, then running DeepFri's GCN.
 Home-page: https://github.com/bioinf-mcb/Metagenomic-DeepFRI
 Download-URL: https://github.com/bioinf-mcb/Metagenomic-DeepFRI
 Author:  Valentyn Bezshapkin, Piotr Kucharski
 Author-email: valentyn.bezshapkin@micro.biol.ethz.ch, soliareofastorauj@gmail.com
 License: BSD-3-Clause
 Keywords: protein function metagenomics deep neural network
@@ -21,15 +21,15 @@
 License-File: LICENSE
 
 # 🍳 Metagenomic-DeepFRI [![Stars](https://img.shields.io/github/stars/bioinf-MCB/Metagenomic-DeepFRI.svg?style=social&maxAge=3600&label=Star)](https://github.com/bioinf-MCB/Metagenomic-DeepFRI/stargazers)
 *A pipeline for annotation of genes with [DeepFRI](https://github.com/flatironinstitute/DeepFRI), a deep learning model for functional protein annotation with [Gene Ontology (GO) terms](https://geneontology.org/docs/go-annotations/). It incorporates [FoldComp](https://github.com/steineggerlab/foldcomp) databases of predicted protein structures for fast annotation of metagenomic gene catalogues.*
 
 ## 🔍 Overview
 Proteins perform most of the work of living cells. Amino acid sequence and structural features of proteins determine a wide range of functions: from binding specificity and conferring mechanical stability, to catalysis of biochemical reactions, transport, and signal transduction.
-DeepFRI is a neural network designed to predict protein function within the framework of the Gene Ontology (GO). The exponential growth in the number of available protein sequences, driven by advancements in low-cost sequencing technologies and computational methods (e.g., gene prediction), has resulted in a pressing need for efficient software to facilitate the annotation of protein databases.
+DeepFRI is a neural network designed to predict protein function within the framework of the Gene Ontology (GO). The exponential growth in the number of available protein sequences, driven by advancements in low-cost sequencing technologies and computational methods (e.g. gene prediction), has resulted in a pressing need for efficient software to facilitate the annotation of protein databases.
 Metagenomic-DeepFRI addresses such need, building upon efficient libraries. It incorporates novel databases of predicted structures (AlphaFold, ESMFold, MIP, etc.) and improves runtimes of DeepFRI by [2-12 times](https://github.com/bioinf-mcb/Metagenomic-DeepFRI/blob/main/weight_convert/onnx_vs_tf2.png)!
 
 ### 📋 Pipeline stages
 
 1. Search proteins similar to query in PDB and supplied `FoldComp` databases with `MMSeqs2`.
 2. Find the best alignment among `MMSeqs2` hits using `PyOpal`.
 3. Align target protein contact map to query protein with unknown structure.
@@ -41,36 +41,63 @@
 * [pyOpal](https://github.com/althonos/pyOpal)
 * [DeepFRI](https://github.com/flatironinstitute/DeepFRI)
 * [FoldComp](https://github.com/steineggerlab/foldcomp)
 * [ONNX](https://github.com/onnx/onnx)
 
 ## 🔧 Installation
 
-1. Clone repo locally
+1. Download environment YAML.
 ```{code-block} bash
-git clone https://github.com/bioinf-mcb/Metagenomic-DeepFRI
-cd Metagenomic-DeepFRI
+wget https://raw.githubusercontent.com/bioinf-mcb/Metagenomic-DeepFRI/main/environment.yml
 ```
-2. Setup conda environment
+2. Setup conda environment and actiate it.
 ```{code-block} bash
 conda env create --name deepfri --file environment.yml
 conda activate deepfri
+# Optional cleanup
+rm environment.yml
 ```
-3. Show help message
+3. Run and view the help message.
 ```{code-block} bash
 mDeepFRI --help
 ```
 
 ## 💡 Usage
 ### 1. Prepare structural database
-The PDB database will be automatically downloaded and installed during first run of `mDeepFRI`. You can download additional databases from [website](https://foldcomp.steineggerlab.workers.dev/). The app was tested with `afdb_swissprot_v4`. You can use different databases, but be mindful that computation time might increase exponentially with the size of the database.
+#### 1.1 Existing `FoldComp` databases
+The PDB database will be automatically downloaded and installed during first run of `mDeepFRI`. The PDB suffers from formatting inconsistencies, therefore during PDB alignment around 10% will fail and will be reported via `WARNING`. We suggest coupling PDB search with predicted databaes.
+
+You can download additional databases from [website](https://foldcomp.steineggerlab.workers.dev/). During a first run, FASTA sequences will be extracted from `FoldComp` database and `MMseqs2` database will be create and indexed. You can use different databases, but be mindful that computation time might increase exponentially with the size of the database.
+
+Tested databases:
+- `afdb_swissprot`
+- `afdb_swissprot_v4`
+- `afdb_rep_v4`
+- `afdb_rep_dark_v4`
+- `afdb_uniprot_v4`
+- `esmatlas`
+- `esmatlas_v2023_02`
+- `highquality_clust30`
+
+
+`ATTENTION:` Please, do not rename downloaded databases. `FoldComp` has certain inconsistencies in the way FASTA sequences are extracted ([example](https://github.com/steineggerlab/foldcomp/issues/51)), therefore pipeline was tweaked for each database. If database you need does not work, please report in [issues](https://github.com/bioinf-mcb/Metagenomic-DeepFRI/issues) and we will add it as soon as possible. Sorry for the inconvenience.
+
+`ATTENTION:` database creation is a very sensitive step which relies on external software. If pipeline is interrupted during this step, the databases might be corrupted. If you are not sure about your database, rerun the pipeline with `--overwrite` flag - it will rerun database creation process.
+
+#### 1.2. Custom `FoldComp` database
+In order to use personal database of structures, you will have to create a custom FoldComp database. For that, download a `FoldComp` executable and run  the following command:
+```
+foldcomp compress [-t number] <dir|tar(.gz)> [<dir|tar|db>]
+```
+
 ### 2. Download models
 Two versions of models available:
 - `v1.0` - is the original version from DeepFRI publication.
-- `v1.1` - is a version finetuned on AlphaFold models and Gene Ontology Uniprot annotations.
+- `v1.1` - is a version finetuned on AlphaFold models and machine-generated Gene Ontology Uniprot annotations. You can read details about `v1.1` in [ISMB 2023 presentation by Pawel Szczerbiak](https://docs.google.com/presentation/d/1Pzn_gQH5-dDImpApSoWFQNu3WByFZYWqfesplANK9hI/edit?usp=sharing)
+
 To download models run command:
 ```
 mDeepFRI get-models --output path/to/weights/folder -v {1.0 or 1.1}
 ```
 
 ### 3. Predict protein function & capture log
 ```
@@ -94,22 +121,25 @@
 | unaligned | 3.2.1.-          | 0.215 | 3.2.1.-                        | cnn        | ec           | nan | nan | nan
 
 This is an example of protein annotation with the AlphaFold database.
 - Protein - the name of the protein from the FASTA file.
 - GO_term/EC_numer - predicted GO term or EC number (dependent on mode)
 - Score - DeepFRI score, translates to model confidence in prediction. Details in [publication](https://www.nature.com/articles/s41467-021-23303-9).
 - Annotation - annotation from ontology
-- Neural_net - type of neural network used for prediction (gcn = Graph Convolutional Network; cnn = Convolutional Neural Network). GCN (Graph Convolutional Network) is employed when structural information is available in the database, allowing for generally more confident predictions.
+- Neural_net - type of neural network used for prediction (gcn = Graph Convolutional Network; cnn = Convolutional Neural Network). GCN (Graph Convolutional Network) is used when structural information is available in the database, allowing for generally more confident predictions. When there are no proteins above similarity cut-off (50% identity by default), CNN is used.
 - DeepFRI_mode:
    ```
    mf = molecular_function
    bp = biological_process
    cc = cellular_component
    ec = enzyme_commission
    ```
+- DB_hit - name of the hit in the database. Empty if no hit was found.
+- DB_name - name of the database. Empty if no hit was found.
+- Identity - sequence identity between query and hit. Empty if no hit was found.
 
 ## ⚙️Features
 ### 1. Prediction modes
 The GO ontology contains three subontologies, defined by their root nodes:
 - Molecular Function (MF)
 - Biological Process (BP)
 - Cellular Component (CC)
```

### Comparing `mDeepFRI-1.1.4/mDeepFRI.egg-info/SOURCES.txt` & `mDeepFRI-1.1.5/mDeepFRI.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,11 +20,11 @@
 mDeepFRI.egg-info/entry_points.txt
 mDeepFRI.egg-info/not-zip-safe
 mDeepFRI.egg-info/requires.txt
 mDeepFRI.egg-info/top_level.txt
 mDeepFRI/tests/__init__.py
 mDeepFRI/tests/test_alignment.py
 mDeepFRI/tests/test_bio_utils.py
-mDeepFRI/tests/test_build_database.py
 mDeepFRI/tests/test_install.py
 mDeepFRI/tests/test_pdb.py
+mDeepFRI/tests/test_predict.py
 mDeepFRI/tests/test_utils.py
```

### Comparing `mDeepFRI-1.1.4/pyproject.toml` & `mDeepFRI-1.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mDeepFRI-1.1.4/setup.cfg` & `mDeepFRI-1.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `mDeepFRI-1.1.4/setup.py` & `mDeepFRI-1.1.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -151,20 +151,24 @@
 extra_compile_args = ["-std=c++14", "-O3"]
 
 EXTENSIONS = [
     Extension("mDeepFRI.predict",
               sources=[SRC_DIR + "/predict.pyx"],
               language="c++",
               libraries=["stdc++"],
-              extra_compile_args=extra_compile_args),
+              extra_compile_args=extra_compile_args,
+              define_macros=[("NPY_NO_DEPRECATED_API", "NPY_1_7_API_VERSION")
+                             ]),
     Extension("mDeepFRI.alignment_utils",
               sources=[SRC_DIR + "/alignment_utils.pyx"],
               language="c++",
               libraries=["stdc++"],
-              extra_compile_args=extra_compile_args),
+              extra_compile_args=extra_compile_args,
+              define_macros=[("NPY_NO_DEPRECATED_API", "NPY_1_7_API_VERSION")
+                             ]),
 ]
 
 extras = {}
 extras["dev"] = ["pre-commit"]
 
 setup(
     name="mDeepFRI",
```

