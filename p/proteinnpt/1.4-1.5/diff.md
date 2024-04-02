# Comparing `tmp/proteinnpt-1.4.tar.gz` & `tmp/proteinnpt-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinnpt-1.4.tar", last modified: Wed Mar 27 04:31:10 2024, max compression
+gzip compressed data, was "proteinnpt-1.5.tar", last modified: Tue Apr  2 04:50:17 2024, max compression
```

## Comparing `proteinnpt-1.4.tar` & `proteinnpt-1.5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 pastin   (13415) dphil     (1014)        0 2024-03-27 04:31:10.563041 proteinnpt-1.4/
--rw-r--r--   0 pastin   (13415) dphil     (1014)     1088 2023-12-10 06:55:08.000000 proteinnpt-1.4/LICENSE
--rw-r--r--   0 pastin   (13415) dphil     (1014)     8171 2024-03-27 04:31:10.561042 proteinnpt-1.4/PKG-INFO
--rwxr-xr-x   0 pastin   (13415) dphil     (1014)     7844 2024-03-20 17:26:50.000000 proteinnpt-1.4/README.md
-drwxr-xr-x   0 pastin   (13415) dphil     (1014)        0 2024-03-27 04:31:10.297046 proteinnpt-1.4/proteinnpt/
--rw-r--r--   0 pastin   (13415) dphil     (1014)       40 2024-02-21 20:55:28.000000 proteinnpt-1.4/proteinnpt/__init__.py
-drwxr-xr-x   0 pastin   (13415) dphil     (1014)        0 2024-03-27 04:31:10.325051 proteinnpt-1.4/proteinnpt/baselines/
--rwxrwxr-x   0 pastin   (13415) dphil     (1014)       36 2024-02-10 17:53:31.000000 proteinnpt-1.4/proteinnpt/baselines/__init__.py
--rwxr-xr-x   0 pastin   (13415) dphil     (1014)     7452 2024-03-06 19:06:19.000000 proteinnpt-1.4/proteinnpt/baselines/data_processing.py
--rwxr-xr-x   0 pastin   (13415) dphil     (1014)    15809 2024-03-03 04:14:43.000000 proteinnpt-1.4/proteinnpt/baselines/model.py
-drwxr-xr-x   0 pastin   (13415) dphil     (1014)        0 2024-03-27 04:31:10.346056 proteinnpt-1.4/proteinnpt/proteinnpt/
--rwxrwxr-x   0 pastin   (13415) dphil     (1014)       36 2024-02-10 17:53:31.000000 proteinnpt-1.4/proteinnpt/proteinnpt/__init__.py
--rwxr-xr-x   0 pastin   (13415) dphil     (1014)    15720 2024-03-23 19:36:46.000000 proteinnpt-1.4/proteinnpt/proteinnpt/data_processing.py
--rwxr-xr-x   0 pastin   (13415) dphil     (1014)    24106 2024-03-26 19:46:36.000000 proteinnpt-1.4/proteinnpt/proteinnpt/model.py
-drwxr-xr-x   0 pastin   (13415) dphil     (1014)        0 2024-03-27 04:31:10.385042 proteinnpt-1.4/proteinnpt/utils/
--rwxrwxr-x   0 pastin   (13415) dphil     (1014)       30 2024-02-22 06:23:02.000000 proteinnpt-1.4/proteinnpt/utils/__init__.py
--rw-rw-r--   0 pastin   (13415) dphil     (1014)     7010 2024-03-25 13:33:31.000000 proteinnpt-1.4/proteinnpt/utils/cv_split.py
--rwxr-xr-x   0 pastin   (13415) dphil     (1014)    20614 2024-03-27 03:41:31.000000 proteinnpt-1.4/proteinnpt/utils/data_utils.py
-drwxr-xr-x   0 pastin   (13415) dphil     (1014)        0 2024-03-27 04:31:10.444073 proteinnpt-1.4/proteinnpt/utils/esm/
--rwxrwxr-x   0 pastin   (13415) dphil     (1014)      479 2024-02-18 02:51:04.000000 proteinnpt-1.4/proteinnpt/utils/esm/__init__.py
--rwxrwxr-x   0 pastin   (13415) dphil     (1014)    12149 2024-02-10 17:53:31.000000 proteinnpt-1.4/proteinnpt/utils/esm/axial_attention.py
--rwxrwxr-x   0 pastin   (13415) dphil     (1014)      369 2024-02-10 17:53:31.000000 proteinnpt-1.4/proteinnpt/utils/esm/constants.py
--rwxrwxr-x   0 pastin   (13415) dphil     (1014)    17554 2024-03-08 06:37:38.000000 proteinnpt-1.4/proteinnpt/utils/esm/data.py
-drwxr-xr-x   0 pastin   (13415) dphil     (1014)        0 2024-03-27 04:31:10.485041 proteinnpt-1.4/proteinnpt/utils/esm/model/
--rw-r--r--   0 pastin   (13415) dphil     (1014)        0 2024-02-21 20:55:28.000000 proteinnpt-1.4/proteinnpt/utils/esm/model/__init__.py
--rwxrwxr-x   0 pastin   (13415) dphil     (1014)     7336 2024-02-10 17:53:31.000000 proteinnpt-1.4/proteinnpt/utils/esm/model/esm1.py
--rwxrwxr-x   0 pastin   (13415) dphil     (1014)     5101 2024-02-17 03:11:57.000000 proteinnpt-1.4/proteinnpt/utils/esm/model/esm2.py
--rwxrwxr-x   0 pastin   (13415) dphil     (1014)     8204 2024-02-10 17:53:31.000000 proteinnpt-1.4/proteinnpt/utils/esm/model/msa_transformer.py
--rwxrwxr-x   0 pastin   (13415) dphil     (1014)    14513 2024-02-10 17:53:31.000000 proteinnpt-1.4/proteinnpt/utils/esm/modules.py
--rwxrwxr-x   0 pastin   (13415) dphil     (1014)    20327 2024-02-10 17:53:31.000000 proteinnpt-1.4/proteinnpt/utils/esm/multihead_attention.py
--rwxrwxr-x   0 pastin   (13415) dphil     (1014)    14889 2024-02-17 03:11:57.000000 proteinnpt-1.4/proteinnpt/utils/esm/pretrained.py
--rwxrwxr-x   0 pastin   (13415) dphil     (1014)     2719 2024-02-10 17:53:31.000000 proteinnpt-1.4/proteinnpt/utils/esm/rotary_embedding.py
--rwxrwxr-x   0 pastin   (13415) dphil     (1014)      196 2024-02-10 17:53:31.000000 proteinnpt-1.4/proteinnpt/utils/esm/version.py
--rw-rw-r--   0 pastin   (13415) dphil     (1014)     3222 2024-02-29 20:43:14.000000 proteinnpt-1.4/proteinnpt/utils/merge_zero_shot.py
--rwxrwxr-x   0 pastin   (13415) dphil     (1014)    31840 2024-03-27 03:22:10.000000 proteinnpt-1.4/proteinnpt/utils/model_utils.py
--rwxr-xr-x   0 pastin   (13415) dphil     (1014)    23063 2024-03-26 18:47:41.000000 proteinnpt-1.4/proteinnpt/utils/msa_utils.py
-drwxr-xr-x   0 pastin   (13415) dphil     (1014)        0 2024-03-27 04:31:10.527047 proteinnpt-1.4/proteinnpt/utils/tranception/
--rwxrwxr-x   0 pastin   (13415) dphil     (1014)       52 2024-02-22 06:07:42.000000 proteinnpt-1.4/proteinnpt/utils/tranception/__init__.py
--rwxrwxr-x   0 pastin   (13415) dphil     (1014)     3341 2024-02-10 17:53:31.000000 proteinnpt-1.4/proteinnpt/utils/tranception/activations.py
--rwxrwxr-x   0 pastin   (13415) dphil     (1014)     1260 2024-02-10 17:53:31.000000 proteinnpt-1.4/proteinnpt/utils/tranception/config.py
--rwxr-xr-x   0 pastin   (13415) dphil     (1014)    45989 2024-02-28 02:31:29.000000 proteinnpt-1.4/proteinnpt/utils/tranception/model_pytorch.py
--rwxrwxr-x   0 pastin   (13415) dphil     (1014)     3343 2024-02-10 17:53:31.000000 proteinnpt-1.4/proteinnpt/utils/tranception/outputs.py
-drwxr-xr-x   0 pastin   (13415) dphil     (1014)        0 2024-03-27 04:31:10.555045 proteinnpt-1.4/proteinnpt/utils/tranception/utils/
--rwxrwxr-x   0 pastin   (13415) dphil     (1014)       38 2024-02-10 17:53:31.000000 proteinnpt-1.4/proteinnpt/utils/tranception/utils/__init__.py
--rwxrwxr-x   0 pastin   (13415) dphil     (1014)     1994 2024-02-17 03:11:57.000000 proteinnpt-1.4/proteinnpt/utils/tranception/utils/dms_utils.py
--rwxrwxr-x   0 pastin   (13415) dphil     (1014)    10505 2024-03-15 04:20:31.000000 proteinnpt-1.4/proteinnpt/utils/tranception/utils/msa_utils.py
--rwxrwxr-x   0 pastin   (13415) dphil     (1014)    12892 2024-03-06 22:43:53.000000 proteinnpt-1.4/proteinnpt/utils/tranception/utils/scoring_utils.py
--rw-r--r--   0 pastin   (13415) dphil     (1014)    10325 2024-03-20 17:26:50.000000 proteinnpt-1.4/proteinnpt/utils/weights.py
-drwxr-xr-x   0 pastin   (13415) dphil     (1014)        0 2024-03-27 04:31:10.313042 proteinnpt-1.4/proteinnpt.egg-info/
--rw-r--r--   0 pastin   (13415) dphil     (1014)     8171 2024-03-27 04:31:10.000000 proteinnpt-1.4/proteinnpt.egg-info/PKG-INFO
--rw-r--r--   0 pastin   (13415) dphil     (1014)     1489 2024-03-27 04:31:10.000000 proteinnpt-1.4/proteinnpt.egg-info/SOURCES.txt
--rw-r--r--   0 pastin   (13415) dphil     (1014)        1 2024-03-27 04:31:10.000000 proteinnpt-1.4/proteinnpt.egg-info/dependency_links.txt
--rw-r--r--   0 pastin   (13415) dphil     (1014)       11 2024-03-27 04:31:10.000000 proteinnpt-1.4/proteinnpt.egg-info/top_level.txt
--rw-r--r--   0 pastin   (13415) dphil     (1014)       38 2024-03-27 04:31:10.563053 proteinnpt-1.4/setup.cfg
--rw-r--r--   0 pastin   (13415) dphil     (1014)      493 2024-03-27 04:29:07.000000 proteinnpt-1.4/setup.py
+drwxr-xr-x   0 pastin   (13415) dphil     (1014)        0 2024-04-02 04:50:17.232263 proteinnpt-1.5/
+-rw-r--r--   0 pastin   (13415) dphil     (1014)     1088 2023-12-10 06:55:08.000000 proteinnpt-1.5/LICENSE
+-rw-r--r--   0 pastin   (13415) dphil     (1014)     8171 2024-04-02 04:50:17.231258 proteinnpt-1.5/PKG-INFO
+-rwxr-xr-x   0 pastin   (13415) dphil     (1014)     7844 2024-03-20 17:26:50.000000 proteinnpt-1.5/README.md
+drwxr-xr-x   0 pastin   (13415) dphil     (1014)        0 2024-04-02 04:50:16.967313 proteinnpt-1.5/proteinnpt/
+-rw-r--r--   0 pastin   (13415) dphil     (1014)       40 2024-02-21 20:55:28.000000 proteinnpt-1.5/proteinnpt/__init__.py
+drwxr-xr-x   0 pastin   (13415) dphil     (1014)        0 2024-04-02 04:50:16.999255 proteinnpt-1.5/proteinnpt/baselines/
+-rwxrwxr-x   0 pastin   (13415) dphil     (1014)       36 2024-02-10 17:53:31.000000 proteinnpt-1.5/proteinnpt/baselines/__init__.py
+-rwxr-xr-x   0 pastin   (13415) dphil     (1014)     7452 2024-03-06 19:06:19.000000 proteinnpt-1.5/proteinnpt/baselines/data_processing.py
+-rwxr-xr-x   0 pastin   (13415) dphil     (1014)    16208 2024-04-01 02:15:44.000000 proteinnpt-1.5/proteinnpt/baselines/model.py
+drwxr-xr-x   0 pastin   (13415) dphil     (1014)        0 2024-04-02 04:50:17.013250 proteinnpt-1.5/proteinnpt/proteinnpt/
+-rwxrwxr-x   0 pastin   (13415) dphil     (1014)       36 2024-02-10 17:53:31.000000 proteinnpt-1.5/proteinnpt/proteinnpt/__init__.py
+-rwxr-xr-x   0 pastin   (13415) dphil     (1014)    16385 2024-04-02 04:34:06.000000 proteinnpt-1.5/proteinnpt/proteinnpt/data_processing.py
+-rwxr-xr-x   0 pastin   (13415) dphil     (1014)    24618 2024-04-02 03:34:51.000000 proteinnpt-1.5/proteinnpt/proteinnpt/model.py
+drwxr-xr-x   0 pastin   (13415) dphil     (1014)        0 2024-04-02 04:50:17.054256 proteinnpt-1.5/proteinnpt/utils/
+-rwxrwxr-x   0 pastin   (13415) dphil     (1014)       30 2024-02-22 06:23:02.000000 proteinnpt-1.5/proteinnpt/utils/__init__.py
+-rw-rw-r--   0 pastin   (13415) dphil     (1014)     7010 2024-03-25 13:33:31.000000 proteinnpt-1.5/proteinnpt/utils/cv_split.py
+-rwxr-xr-x   0 pastin   (13415) dphil     (1014)    21806 2024-04-01 22:21:03.000000 proteinnpt-1.5/proteinnpt/utils/data_utils.py
+drwxr-xr-x   0 pastin   (13415) dphil     (1014)        0 2024-04-02 04:50:17.118255 proteinnpt-1.5/proteinnpt/utils/esm/
+-rwxrwxr-x   0 pastin   (13415) dphil     (1014)      479 2024-02-18 02:51:04.000000 proteinnpt-1.5/proteinnpt/utils/esm/__init__.py
+-rwxrwxr-x   0 pastin   (13415) dphil     (1014)    12149 2024-02-10 17:53:31.000000 proteinnpt-1.5/proteinnpt/utils/esm/axial_attention.py
+-rwxrwxr-x   0 pastin   (13415) dphil     (1014)      369 2024-02-10 17:53:31.000000 proteinnpt-1.5/proteinnpt/utils/esm/constants.py
+-rwxrwxr-x   0 pastin   (13415) dphil     (1014)    17554 2024-03-08 06:37:38.000000 proteinnpt-1.5/proteinnpt/utils/esm/data.py
+drwxr-xr-x   0 pastin   (13415) dphil     (1014)        0 2024-04-02 04:50:17.146252 proteinnpt-1.5/proteinnpt/utils/esm/model/
+-rw-r--r--   0 pastin   (13415) dphil     (1014)        0 2024-02-21 20:55:28.000000 proteinnpt-1.5/proteinnpt/utils/esm/model/__init__.py
+-rwxrwxr-x   0 pastin   (13415) dphil     (1014)     7336 2024-02-10 17:53:31.000000 proteinnpt-1.5/proteinnpt/utils/esm/model/esm1.py
+-rwxrwxr-x   0 pastin   (13415) dphil     (1014)     5101 2024-02-17 03:11:57.000000 proteinnpt-1.5/proteinnpt/utils/esm/model/esm2.py
+-rwxrwxr-x   0 pastin   (13415) dphil     (1014)     8204 2024-02-10 17:53:31.000000 proteinnpt-1.5/proteinnpt/utils/esm/model/msa_transformer.py
+-rwxrwxr-x   0 pastin   (13415) dphil     (1014)    14513 2024-02-10 17:53:31.000000 proteinnpt-1.5/proteinnpt/utils/esm/modules.py
+-rwxrwxr-x   0 pastin   (13415) dphil     (1014)    20327 2024-02-10 17:53:31.000000 proteinnpt-1.5/proteinnpt/utils/esm/multihead_attention.py
+-rwxrwxr-x   0 pastin   (13415) dphil     (1014)    14889 2024-02-17 03:11:57.000000 proteinnpt-1.5/proteinnpt/utils/esm/pretrained.py
+-rwxrwxr-x   0 pastin   (13415) dphil     (1014)     2719 2024-02-10 17:53:31.000000 proteinnpt-1.5/proteinnpt/utils/esm/rotary_embedding.py
+-rwxrwxr-x   0 pastin   (13415) dphil     (1014)      196 2024-02-10 17:53:31.000000 proteinnpt-1.5/proteinnpt/utils/esm/version.py
+-rw-rw-r--   0 pastin   (13415) dphil     (1014)     3600 2024-04-02 02:35:07.000000 proteinnpt-1.5/proteinnpt/utils/merge_zero_shot.py
+-rwxrwxr-x   0 pastin   (13415) dphil     (1014)    31840 2024-03-27 03:22:10.000000 proteinnpt-1.5/proteinnpt/utils/model_utils.py
+-rwxr-xr-x   0 pastin   (13415) dphil     (1014)    23091 2024-04-02 02:37:01.000000 proteinnpt-1.5/proteinnpt/utils/msa_utils.py
+drwxr-xr-x   0 pastin   (13415) dphil     (1014)        0 2024-04-02 04:50:17.189260 proteinnpt-1.5/proteinnpt/utils/tranception/
+-rwxrwxr-x   0 pastin   (13415) dphil     (1014)       52 2024-02-22 06:07:42.000000 proteinnpt-1.5/proteinnpt/utils/tranception/__init__.py
+-rwxrwxr-x   0 pastin   (13415) dphil     (1014)     3341 2024-02-10 17:53:31.000000 proteinnpt-1.5/proteinnpt/utils/tranception/activations.py
+-rwxrwxr-x   0 pastin   (13415) dphil     (1014)     1260 2024-02-10 17:53:31.000000 proteinnpt-1.5/proteinnpt/utils/tranception/config.py
+-rwxr-xr-x   0 pastin   (13415) dphil     (1014)    45989 2024-03-29 14:05:38.000000 proteinnpt-1.5/proteinnpt/utils/tranception/model_pytorch.py
+-rwxrwxr-x   0 pastin   (13415) dphil     (1014)     3343 2024-02-10 17:53:31.000000 proteinnpt-1.5/proteinnpt/utils/tranception/outputs.py
+drwxr-xr-x   0 pastin   (13415) dphil     (1014)        0 2024-04-02 04:50:17.226252 proteinnpt-1.5/proteinnpt/utils/tranception/utils/
+-rwxrwxr-x   0 pastin   (13415) dphil     (1014)       38 2024-02-10 17:53:31.000000 proteinnpt-1.5/proteinnpt/utils/tranception/utils/__init__.py
+-rwxrwxr-x   0 pastin   (13415) dphil     (1014)     1994 2024-02-17 03:11:57.000000 proteinnpt-1.5/proteinnpt/utils/tranception/utils/dms_utils.py
+-rwxrwxr-x   0 pastin   (13415) dphil     (1014)    10505 2024-03-15 04:20:31.000000 proteinnpt-1.5/proteinnpt/utils/tranception/utils/msa_utils.py
+-rwxrwxr-x   0 pastin   (13415) dphil     (1014)    12892 2024-03-06 22:43:53.000000 proteinnpt-1.5/proteinnpt/utils/tranception/utils/scoring_utils.py
+-rw-r--r--   0 pastin   (13415) dphil     (1014)    10325 2024-03-20 17:26:50.000000 proteinnpt-1.5/proteinnpt/utils/weights.py
+drwxr-xr-x   0 pastin   (13415) dphil     (1014)        0 2024-04-02 04:50:16.985256 proteinnpt-1.5/proteinnpt.egg-info/
+-rw-r--r--   0 pastin   (13415) dphil     (1014)     8171 2024-04-02 04:50:16.000000 proteinnpt-1.5/proteinnpt.egg-info/PKG-INFO
+-rw-r--r--   0 pastin   (13415) dphil     (1014)     1489 2024-04-02 04:50:16.000000 proteinnpt-1.5/proteinnpt.egg-info/SOURCES.txt
+-rw-r--r--   0 pastin   (13415) dphil     (1014)        1 2024-04-02 04:50:16.000000 proteinnpt-1.5/proteinnpt.egg-info/dependency_links.txt
+-rw-r--r--   0 pastin   (13415) dphil     (1014)       11 2024-04-02 04:50:16.000000 proteinnpt-1.5/proteinnpt.egg-info/top_level.txt
+-rw-r--r--   0 pastin   (13415) dphil     (1014)       38 2024-04-02 04:50:17.233259 proteinnpt-1.5/setup.cfg
+-rw-r--r--   0 pastin   (13415) dphil     (1014)      493 2024-04-02 04:46:03.000000 proteinnpt-1.5/setup.py
```

### Comparing `proteinnpt-1.4/LICENSE` & `proteinnpt-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinnpt-1.4/PKG-INFO` & `proteinnpt-1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteinnpt
-Version: 1.4
+Version: 1.5
 Summary: ProteinNPT: Improving Protein Property Prediction and Design with Non-Parametric Transformers
 Home-page: https://github.com/OATML-Markslab/ProteinNPT
 Author: Pascal Notin and Ruben Weitzman
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `proteinnpt-1.4/README.md` & `proteinnpt-1.5/README.md`

 * *Files identical despite different names*

### Comparing `proteinnpt-1.4/proteinnpt/baselines/data_processing.py` & `proteinnpt-1.5/proteinnpt/baselines/data_processing.py`

 * *Files identical despite different names*

### Comparing `proteinnpt-1.4/proteinnpt/baselines/model.py` & `proteinnpt-1.5/proteinnpt/baselines/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         self.eos_idx = alphabet.eos_idx
         self.prepend_bos = alphabet.prepend_bos
         self.append_eos = alphabet.append_eos
         self.target_names = self.args.target_config.keys() 
         self.MSA_sample_sequences = None 
         self.device = None
         self.model_type = args.model_type 
-        if self.args.aa_embeddings in ["MSA_Transformer","ESM1v"]:
+        if self.args.aa_embeddings == "MSA_Transformer" or self.args.aa_embeddings.startswith("ESM"):
             model, _ = load_model_and_alphabet(args.embedding_model_location)
             self.aa_embedding = model
             if self.args.aa_embeddings == "MSA_Transformer": self.args.seq_len = self.args.MSA_seq_len #If MSA does not cover full sequence length, we adjust seq_len param to be MSA_len (sequences truncated as needed in preprocessing)
         elif self.args.aa_embeddings == "Linear_embedding":
             self.aa_embedding = nn.Sequential(
                 nn.Embedding(
                     self.alphabet_size, self.args.embed_dim, padding_idx=self.padding_idx
@@ -148,16 +148,23 @@
         if sequence_embeddings is not None:
             x = sequence_embeddings.to(self.device)
         else:
             if self.args.aa_embeddings == "MSA_Transformer":
                 output = self.aa_embedding(tokens, repr_layers=[12])
                 x = output["representations"][12][:] # B, N, L, D
                 x = x[:,0,:,:] #In each MSA batch the first sequence is what we care about. The other MSA sequences were just to compute embeddings and logits
-            elif self.args.aa_embeddings == "ESM1v":
-                last_layer_index = 33
+            elif self.args.aa_embeddings.startswith("ESM"):
+                if self.args.aa_embeddings=="ESM1v":
+                    last_layer_index = 33
+                elif self.args.aa_embeddings=="ESM2_15B":
+                    last_layer_index = 48
+                elif self.args.aa_embeddings=="ESM2_3B":
+                    last_layer_index = 36
+                elif self.args.aa_embeddings=="ESM2_650M":
+                    last_layer_index = 33
                 output = self.aa_embedding(tokens, repr_layers=[last_layer_index])
                 x = output["representations"][last_layer_index][:] # N, L, D
             elif self.args.aa_embeddings == "Tranception":
                 processed_batch = {'input_ids': tokens, 'labels': tokens}
                 output = self.aa_embedding(**processed_batch, return_dict=True, output_hidden_states=True)
                 x = output.hidden_states[0]
             elif self.args.aa_embeddings =="Linear_embedding":
```

### Comparing `proteinnpt-1.4/proteinnpt/proteinnpt/data_processing.py` & `proteinnpt-1.5/proteinnpt/proteinnpt/data_processing.py`

 * *Files 4% similar despite different names*

```diff
@@ -176,33 +176,36 @@
         #Re-organize list of sequences to have training_num_assay_sequences_per_batch_per_gpu MSA batches, where in each the sequence to score is the first and the rest are the sampled MSA sequences.
         num_sequences = num_all_mutated_sequences_input + args.num_MSA_sequences_per_training_instance
         assert len(batch['mutant_mutated_seq_pairs']) == num_sequences, "Unexpected number of sequences"
         all_mutated_sequences_input = batch['mutant_mutated_seq_pairs'][:num_all_mutated_sequences_input]
         MSA_sequences = batch['mutant_mutated_seq_pairs'][num_all_mutated_sequences_input:]
         batch['mutant_mutated_seq_pairs'] = [ [sequence] + MSA_sequences for sequence in all_mutated_sequences_input]
 
-    if args.aa_embeddings in ["MSA_Transformer","ESM1v","Linear_embedding"]:
+    if args.aa_embeddings in ["MSA_Transformer", "Linear_embedding"] or args.aa_embeddings.startswith("ESM"):
         token_batch_converter = alphabet.get_batch_converter()
         batch_sequence_names, batch_AA_sequences, batch_token_sequences = token_batch_converter(batch['mutant_mutated_seq_pairs'])
-        if (args.aa_embeddings != "MSA_Transformer") or (args.sequence_embeddings_location is not None): 
+        if args.aa_embeddings=="MSA_Transformer" and args.sequence_embeddings_location is not None: #If loading MSAT embeddings from disk, we drop the MSA dimension (done already if not MSAT via the different tokenizer)
             num_MSAs_in_batch, num_sequences_in_alignments, seqlen = batch_token_sequences.size()
             batch_token_sequences = batch_token_sequences.view(num_sequences_in_alignments, seqlen) #drop the dummy batch dimension from the tokenizer when using ESM1v / LinearEmbedding
     elif args.aa_embeddings == "Tranception":
         _, sequence = zip(*batch['mutant_mutated_seq_pairs'])
-        batch_token_sequences = torch.tensor(model.alphabet(sequence)['input_ids'])
-    
+        batch_token_sequences = torch.tensor(model.alphabet(sequence, add_special_tokens=True, truncation=True, padding=True, max_length=model.aa_embedding.config.n_ctx)['input_ids'])
+        
     # Mask protein sequences
     batch_masked_tokens, batch_token_labels, masked_indices = mask_protein_sequences(
         inputs = batch_token_sequences, 
         alphabet = alphabet, 
         proba_aa_mask = proba_aa_mask if not eval_mode else 0.0, #In eval mode we do not mask any token
         proba_random_mutation = 0.1, 
         proba_unchanged = 0.1
     )
-    if args.sequence_embeddings_location is not None: 
+    if args.sequence_embeddings_location is not None:
+        if sequence_embeddings.shape[1] > masked_indices.shape[1]: # When dealing with sequences of different sizes, and sequences in batch happen to be all smaller than longest sequence in assay for which we computed embeddings
+            extra_padding_in_embeddings = (sequence_embeddings.shape[1] - masked_indices.shape[1])
+            sequence_embeddings = sequence_embeddings[:,:-extra_padding_in_embeddings]
         sequence_embeddings[masked_indices] = 0.0
 
     batch_masked_tokens = batch_masked_tokens.to(device)
     batch_token_labels = batch_token_labels.to(device)
     processed_batch = {
         'masked_tokens': batch_masked_tokens,
         'token_labels': batch_token_labels,
```

### Comparing `proteinnpt-1.4/proteinnpt/proteinnpt/model.py` & `proteinnpt-1.5/proteinnpt/proteinnpt/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         self.model_type = args.model_type
         self.PNPT_ensemble_test_num_seeds = -1
         self.PNPT_no_reconstruction_error = False
         self.deactivate_col_attention = False
         self.tranception_attention = False
         
         assert self.args.embed_dim % self.args.attention_heads ==0, "Embedding size {} needs to be a multiple of number of heads {}".format(self.args.embed_dim, self.args.attention_heads)
-        if self.args.aa_embeddings in ["MSA_Transformer","ESM1v"]:
+        if self.args.aa_embeddings=="MSA_Transformer" or args.aa_embeddings.startswith("ESM"):
             model, _ = load_model_and_alphabet(args.embedding_model_location)
             self.aa_embedding = model
             self.aa_embedding_dim = self.aa_embedding.embed_tokens.weight.shape[-1]
         elif self.args.aa_embeddings == "Tranception":
             self.aa_embedding_dim = 1280
             config = json.load(open(args.embedding_model_location+os.sep+'config.json'))
             config = TranceptionConfig(**config)
@@ -114,15 +114,15 @@
                     )
                     for _ in range(self.args.num_protein_npt_layers)
                 ]
             )
         self.emb_layer_norm_before = ESM1bLayerNorm(self.args.embed_dim)
         self.emb_layer_norm_after = ESM1bLayerNorm(self.args.embed_dim)
         
-        if self.args.aa_embeddings in ["MSA_Transformer","ESM1v"]:
+        if self.args.aa_embeddings=="MSA_Transformer" or args.aa_embeddings.startswith("ESM"):
             weight = self.aa_embedding.embed_tokens.weight
         elif self.args.aa_embeddings == "Tranception":
             weight = self.aa_embedding.lm_head.weight
         else:
             weight = self.aa_embedding.weight
 
         self.lm_head = RobertaLMHead(
@@ -191,31 +191,38 @@
             self.device = next(self.parameters()).device
         print("Model device: {}".format(self.device))
         
     def forward(self, tokens, targets=None, zero_shot_fitness_predictions=None, sequence_embeddings=None, repr_layers=[], need_head_weights=False):
         padding_mask = tokens.eq(self.padding_idx) 
         if not padding_mask.any(): padding_mask = None
         
-        if self.args.aa_embeddings == "MSA_Transformer" and self.args.sequence_embeddings_location is None:
+        if self.args.aa_embeddings == "MSA_Transformer" and self.args.sequence_embeddings_location is None: #If loading MSAT embeddings from disk, we have dropped one dim already
             assert tokens.ndim == 3, "Finding dimension of tokens to be: {}".format(tokens.ndim)
             num_MSAs_in_batch, num_sequences_in_alignments, seqlen = tokens.size() # N, B, L (seqs with labels, seqs in MSA, seq length)
             batch_size = num_MSAs_in_batch
         else:
             assert tokens.ndim == 2, "Finding dimension of tokens to be: {}".format(tokens.ndim)
             batch_size, seqlen = tokens.size() # N, L (seqs with labels, seq length)
         
         if sequence_embeddings is not None:
             x = sequence_embeddings.to(self.device)
         else:
             if self.args.aa_embeddings == "MSA_Transformer":
                 output = self.aa_embedding(tokens, repr_layers=[12])
                 x = output["representations"][12][:] # N, B, L, D
                 x = x[:,0,:,:] # N, L, D. #In each MSA batch the first sequence is what we care about. The other MSA sequences were just to compute embeddings and logits
-            elif self.args.aa_embeddings == "ESM1v":
-                last_layer_index = 33
+            elif self.args.aa_embeddings.startswith("ESM"):
+                if self.args.aa_embeddings=="ESM1v":
+                    last_layer_index = 33
+                elif self.args.aa_embeddings=="ESM2_15B":
+                    last_layer_index = 48
+                elif self.args.aa_embeddings=="ESM2_3B":
+                    last_layer_index = 36
+                elif self.args.aa_embeddings=="ESM2_650M":
+                    last_layer_index = 33
                 output = self.aa_embedding(tokens, repr_layers=[last_layer_index])
                 x = output["representations"][last_layer_index][:] # N, L, D
             elif self.args.aa_embeddings =="Linear_embedding":
                 x = self.aa_embedding(tokens)
                 x = x + self.aa_positions_embedding(tokens.view(batch_size, seqlen)).view(x.size()) # Need position embedding in PNPT since we will apply axial attention
             else:
                 print("AA embeddings not recognized")
@@ -250,18 +257,20 @@
         
         #Concatenate AA tokens and targets
         x = torch.cat((x,y),dim=-2) # 1, N, (L+num_targets), D
         x = self.emb_layer_norm_before(x)
         x = self.dropout_module(x)
 
         if padding_mask is not None:
-            padding_mask_with_targets = torch.zeros(num_MSAs_in_batch, num_sequences_in_alignments, seqlen + self.num_targets_input)
+            B, N, L, D = x.shape
+            padding_mask_with_targets = torch.zeros(B, N, L).to(x.device)
             padding_mask_with_targets[...,:seqlen] = padding_mask
             padding_mask = padding_mask_with_targets
             x = x * (1 - padding_mask.unsqueeze(-1).type_as(x))
+            padding_mask = padding_mask.bool()
         
         repr_layers = set(repr_layers)
         hidden_representations = {}
         if 0 in repr_layers: hidden_representations[0] = x
         if need_head_weights:
             row_attn_weights = []
             col_attn_weights = []
```

### Comparing `proteinnpt-1.4/proteinnpt/utils/cv_split.py` & `proteinnpt-1.5/proteinnpt/utils/cv_split.py`

 * *Files identical despite different names*

### Comparing `proteinnpt-1.4/proteinnpt/utils/data_utils.py` & `proteinnpt-1.5/proteinnpt/utils/data_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os,sys
 import numpy as np
 import pandas as pd
 from scipy.stats import spearmanr
 import torch
 import h5py
 from datasets import Dataset
+from proteinnpt.utils.tranception.utils.scoring_utils import get_mutated_sequence
 
 def standardize(x, epsilon = 1e-10):
     return (x - x.mean()) / (x.std() + epsilon)
 
 def split_data_based_on_test_fold_index(dataframe, fold_variable_name = 'fold_modulo_5', test_fold_index=None, use_validation_set=True):
     unique_folds = np.unique(dataframe[fold_variable_name])
     num_distinct_folds = len(unique_folds)
@@ -32,39 +33,53 @@
             val = None
             test = dataframe[dataframe[fold_variable_name]==test_fold_index]
     del train[fold_variable_name]
     if use_validation_set: del val[fold_variable_name]
     del test[fold_variable_name]
     return train, val, test
 
+def cleanup_ids_assay_data(df, indel_mode=False, target_seq=None):
+    assert 'mutated_sequence' in df.columns or 'mutant' in df.columns, "assay did not reference mutant nor mutated_sequence"
+    if 'mutated_sequence' not in df: 
+        df['mutated_sequence'] = df['mutant'].apply(lambda x: get_mutated_sequence(target_seq, x))
+    if 'mutant' not in df: 
+        if not indel_mode and target_seq is not None: #If substitutions assay, we reconstruct the mutants by comparing the mutated sequences with the target sequence
+            df['mutant'] = df["mutated_sequence"].apply(lambda x: ':'.join([wt + str(i+1) + mut for i, (wt, mut) in enumerate(zip(target_seq, x)) if wt != mut]))
+        else: #If indels we default to dummy mutant names
+            df['mutant'] = df.index.to_series().apply(lambda x: "mutant_" + str(x))
+    return df
+
 def get_train_val_test_data(args, assay_file_names):
     target_names = args.target_config.keys() 
     assay_data={}
     merge = None
     main_target_name = None
     main_target_name_count = 0
     for target in target_names:
         if args.target_config[target]["main_target"]: 
             main_target_name=target
             main_target_name_count+=1
     assert main_target_name is not None, "No main target referenced. Please update config to select a unique main target."
     assert main_target_name_count <= 1, "Several main targets referenced. Please update config to select a unique main target."
     
-    assay_data[main_target_name] = pd.read_csv(args.target_config[main_target_name]["location"] + os.sep + assay_file_names[main_target_name])[['mutant','mutated_sequence',args.target_config[main_target_name]["var_name"],args.fold_variable_name]] 
+    assay_data[main_target_name] = pd.read_csv(args.target_config[main_target_name]["location"] + os.sep + assay_file_names[main_target_name]) 
+    assay_data[main_target_name] = cleanup_ids_assay_data(assay_data[main_target_name])[['mutant','mutated_sequence',args.target_config[main_target_name]["var_name"],args.fold_variable_name]]
     assay_data[main_target_name].columns = ['mutant','mutated_sequence', main_target_name, args.fold_variable_name]
     merge = assay_data[main_target_name]
     
     for target_name in target_names:
         if target_name!=main_target_name:
-            assay_data[target_name] = pd.read_csv(args.target_config[target_name]["location"] + os.sep + assay_file_names[target_name])[['mutant',args.target_config[target_name]["var_name"]]] 
+            assay_data[target_name] = pd.read_csv(args.target_config[target_name]["location"] + os.sep + assay_file_names[target_name]) 
+            assay_data[target_name] = cleanup_ids_assay_data(assay_data[target_name])[['mutant',args.target_config[target_name]["var_name"]]]
             assay_data[target_name].columns = ['mutant',target_name]
             merge = pd.merge(merge, assay_data[target_name], how='outer', on='mutant')
             
     if args.augmentation=="zero_shot_fitness_predictions_covariate":
-        zero_shot_fitness_predictions = pd.read_csv(args.zero_shot_fitness_predictions_location + os.sep + assay_file_names[main_target_name])[['mutant',args.zero_shot_fitness_predictions_var_name]]
+        zero_shot_fitness_predictions = pd.read_csv(args.zero_shot_fitness_predictions_location + os.sep + assay_file_names[main_target_name])
+        zero_shot_fitness_predictions = cleanup_ids_assay_data(zero_shot_fitness_predictions)[['mutant',args.zero_shot_fitness_predictions_var_name]]
         zero_shot_fitness_predictions.columns = ['mutant','zero_shot_fitness_predictions']
         zero_shot_fitness_predictions['zero_shot_fitness_predictions'] = standardize(zero_shot_fitness_predictions['zero_shot_fitness_predictions'])
         merge = pd.merge(merge,zero_shot_fitness_predictions,how='left',on='mutant')
 
     train_val_test_splits = split_data_based_on_test_fold_index(
         dataframe = merge, 
         fold_variable_name = args.fold_variable_name,
```

### Comparing `proteinnpt-1.4/proteinnpt/utils/esm/axial_attention.py` & `proteinnpt-1.5/proteinnpt/utils/esm/axial_attention.py`

 * *Files identical despite different names*

### Comparing `proteinnpt-1.4/proteinnpt/utils/esm/data.py` & `proteinnpt-1.5/proteinnpt/utils/esm/data.py`

 * *Files identical despite different names*

### Comparing `proteinnpt-1.4/proteinnpt/utils/esm/model/esm1.py` & `proteinnpt-1.5/proteinnpt/utils/esm/model/esm1.py`

 * *Files identical despite different names*

### Comparing `proteinnpt-1.4/proteinnpt/utils/esm/model/esm2.py` & `proteinnpt-1.5/proteinnpt/utils/esm/model/esm2.py`

 * *Files identical despite different names*

### Comparing `proteinnpt-1.4/proteinnpt/utils/esm/model/msa_transformer.py` & `proteinnpt-1.5/proteinnpt/utils/esm/model/msa_transformer.py`

 * *Files identical despite different names*

### Comparing `proteinnpt-1.4/proteinnpt/utils/esm/modules.py` & `proteinnpt-1.5/proteinnpt/utils/esm/modules.py`

 * *Files identical despite different names*

### Comparing `proteinnpt-1.4/proteinnpt/utils/esm/multihead_attention.py` & `proteinnpt-1.5/proteinnpt/utils/esm/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `proteinnpt-1.4/proteinnpt/utils/esm/pretrained.py` & `proteinnpt-1.5/proteinnpt/utils/esm/pretrained.py`

 * *Files identical despite different names*

### Comparing `proteinnpt-1.4/proteinnpt/utils/esm/rotary_embedding.py` & `proteinnpt-1.5/proteinnpt/utils/esm/rotary_embedding.py`

 * *Files identical despite different names*

### Comparing `proteinnpt-1.4/proteinnpt/utils/merge_zero_shot.py` & `proteinnpt-1.5/proteinnpt/utils/merge_zero_shot.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,45 @@
 import os
 import argparse
 import pandas as pd
+from proteinnpt.utils.data_utils import cleanup_ids_assay_data
 
 def main(args):
     mapping_protein_seq_DMS = pd.read_csv(args.DMS_reference_file_path)
     DMS_id=mapping_protein_seq_DMS["DMS_id"][args.DMS_index]
     print("Merging all zero-shot scores for DMS: "+str(DMS_id))
     DMS_file_name = mapping_protein_seq_DMS["DMS_filename"][mapping_protein_seq_DMS["DMS_id"]==DMS_id].values[0]
     DMS_data = pd.read_csv(args.DMS_mutants_folder + os.sep + DMS_file_name, low_memory=False)
+    DMS_data = cleanup_ids_assay_data(DMS_data)
     try:
         var_list = ['mutant','mutated_sequence','DMS_score','DMS_score_bin']
+        merge = DMS_data[var_list]
     except:
         var_list = ['mutant','mutated_sequence']
-    merge = DMS_data[var_list]
+        merge = DMS_data[var_list]
     num_mutants = len(merge)
     score_name_mapping_original_names = {
         "Tranception" : "avg_score",
         "ESM1v" : "Ensemble_ESM1v",
         "MSA_Transformer" : "esm_msa1b_t12_100M_UR50S_ensemble",
         "DeepSequence": "evol_indices_ensemble",
-        "TranceptEVE" : "avg_score"
+        "TranceptEVE" : "avg_score",
+        "ESM2_650M" : "esm2_t33_650M_UR50D",
+        "ESM2_3B" : "esm2_t36_3B_UR50D",
+        "ESM2_15B" : "esm2_t48_15B_UR50D"
     }
     score_name_mapping_clean_names = {
         "Tranception" : "Tranception_L",
         "ESM1v" : "ESM1v_ensemble",
         "MSA_Transformer" : "MSA_Transformer_ensemble",
         "DeepSequence": "DeepSequence_ensemble",
-        "TranceptEVE": "TranceptEVE_L"
+        "TranceptEVE": "TranceptEVE_L",
+        "ESM2_650M" : "ESM2_650M",
+        "ESM2_3B" : "ESM2_3B",
+        "ESM2_15B" : "ESM2_15B"
     }
     model_list = ["Tranception", "ESM1v", "MSA_Transformer", "DeepSequence", "TranceptEVE"] if not args.indel_mode else ["Tranception"]
     for model_name in model_list:
         print(model_name)
         model_score_file_path = args.zero_shot_scores_folder + os.sep + model_name + os.sep + DMS_file_name
         if os.path.exists(model_score_file_path):
             scores = pd.read_csv(model_score_file_path,low_memory=False)
```

### Comparing `proteinnpt-1.4/proteinnpt/utils/model_utils.py` & `proteinnpt-1.5/proteinnpt/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `proteinnpt-1.4/proteinnpt/utils/msa_utils.py` & `proteinnpt-1.5/proteinnpt/utils/msa_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,15 +213,15 @@
         If num_cpus == -1, weights are computed in parallel using all available cores.
         Note: This will use multiprocessing.cpu_count() to get the number of available cores, which on clusters may
         return all cores, not just the number of cores available to the user.
         """
         # Refactored into its own function so that we can call it separately
         if self.use_weights:
             if os.path.isfile(self.weights_location):
-                print("Loading sequence weights from disk")
+                print("Loading sequence weights from disk: {}".format(self.weights_location))
                 self.weights = np.load(file=self.weights_location)
             else:
                 print("Computing sequence weights")
                 if num_cpus == -1:
                     num_cpus = get_num_cpus()
 
                 if method == "eve":
@@ -243,15 +243,14 @@
             # If not using weights, use an isotropic weight matrix
             print("Not weighting sequence data")
             self.weights = np.ones(self.one_hot_encoding.shape[0])
 
         self.Neff = np.sum(self.weights)
         print("Neff =", str(self.Neff))
         print("Number of sequences: ", self.num_sequences)
-        
         assert self.weights.shape[0] == self.num_sequences  # == self.one_hot_encoding.shape[0]
         self.seq_name_to_weight={}  # For later, if we want to remove certain sequences and associated weights
         for i,seq_name in enumerate(self.seq_name_to_sequence.keys()):
             self.seq_name_to_weight[seq_name]=self.weights[i]
         
         return self.weights
 
@@ -305,15 +304,15 @@
 def filter_msa(filename, path_to_hhfilter, hhfilter_min_cov=75, hhfilter_max_seq_id=90, hhfilter_min_seq_id=0):
     """
     We use the filtering defaults from the MSA Transformer paper wrt maximum sequence id: hhfilter_max_seq_id = 90; hhfilter_min_cov=75.
     Install hhfilter:
         wget https://github.com/soedinglab/hh-suite/releases/download/v3.3.0/hhsuite-3.3.0-AVX2-Linux.tar.gz; tar xvfz hhsuite-3.3.0-AVX2-Linux.tar.gz; export PATH="$(pwd)/bin:$(pwd)/scripts:$PATH"
     """
     input_folder = '/'.join(filename.split('/')[:-1])
-    msa_name = filename.split('/')[-1].split('.')[0]
+    msa_name = filename.split('/')[-1].split('.a2m')[0]
     preprocessed_filename = input_folder+os.sep+'preprocessed'+os.sep+msa_name
     output_filename = input_folder+os.sep+'hhfiltered'+os.sep+msa_name+'_hhfiltered_cov_'+str(hhfilter_min_cov)+'_maxid_'+str(hhfilter_max_seq_id)+'_minid_'+str(hhfilter_min_seq_id)+'.a2m'
     
     if msa_name=="R1AB_SARS2_02-19-2022_b07": hhfilter_max_seq_id=100 #Otherwise we would only keep 1 sequence.
     if not os.path.isdir(input_folder+os.sep+'preprocessed'):
         os.mkdir(input_folder+os.sep+'preprocessed')
     if not os.path.isdir(input_folder+os.sep+'hhfiltered'):
```

### Comparing `proteinnpt-1.4/proteinnpt/utils/tranception/activations.py` & `proteinnpt-1.5/proteinnpt/utils/tranception/activations.py`

 * *Files identical despite different names*

### Comparing `proteinnpt-1.4/proteinnpt/utils/tranception/config.py` & `proteinnpt-1.5/proteinnpt/utils/tranception/config.py`

 * *Files identical despite different names*

### Comparing `proteinnpt-1.4/proteinnpt/utils/tranception/model_pytorch.py` & `proteinnpt-1.5/proteinnpt/utils/tranception/model_pytorch.py`

 * *Files identical despite different names*

### Comparing `proteinnpt-1.4/proteinnpt/utils/tranception/outputs.py` & `proteinnpt-1.5/proteinnpt/utils/tranception/outputs.py`

 * *Files identical despite different names*

### Comparing `proteinnpt-1.4/proteinnpt/utils/tranception/utils/dms_utils.py` & `proteinnpt-1.5/proteinnpt/utils/tranception/utils/dms_utils.py`

 * *Files identical despite different names*

### Comparing `proteinnpt-1.4/proteinnpt/utils/tranception/utils/msa_utils.py` & `proteinnpt-1.5/proteinnpt/utils/tranception/utils/msa_utils.py`

 * *Files identical despite different names*

### Comparing `proteinnpt-1.4/proteinnpt/utils/tranception/utils/scoring_utils.py` & `proteinnpt-1.5/proteinnpt/utils/tranception/utils/scoring_utils.py`

 * *Files identical despite different names*

### Comparing `proteinnpt-1.4/proteinnpt/utils/weights.py` & `proteinnpt-1.5/proteinnpt/utils/weights.py`

 * *Files identical despite different names*

### Comparing `proteinnpt-1.4/proteinnpt.egg-info/PKG-INFO` & `proteinnpt-1.5/proteinnpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteinnpt
-Version: 1.4
+Version: 1.5
 Summary: ProteinNPT: Improving Protein Property Prediction and Design with Non-Parametric Transformers
 Home-page: https://github.com/OATML-Markslab/ProteinNPT
 Author: Pascal Notin and Ruben Weitzman
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `proteinnpt-1.4/proteinnpt.egg-info/SOURCES.txt` & `proteinnpt-1.5/proteinnpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

