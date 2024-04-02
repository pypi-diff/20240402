# Comparing `tmp/tangermeme-0.1.0.tar.gz` & `tmp/tangermeme-0.1.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tangermeme-0.1.0.tar", last modified: Tue Apr  2 05:52:48 2024, max compression
+gzip compressed data, was "tangermeme-0.1.0rc0.tar", last modified: Thu Mar 28 15:12:47 2024, max compression
```

## Comparing `tangermeme-0.1.0.tar` & `tangermeme-0.1.0rc0.tar`

### file list

```diff
@@ -1,45 +1,40 @@
-drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2024-04-02 05:52:50.022307 tangermeme-0.1.0/
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     1072 2024-02-04 20:42:51.000000 tangermeme-0.1.0/LICENSE
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)      556 2024-04-02 05:52:50.018307 tangermeme-0.1.0/PKG-INFO
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    11659 2024-04-01 05:36:53.000000 tangermeme-0.1.0/README.md
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)       38 2024-04-02 05:52:50.022307 tangermeme-0.1.0/setup.cfg
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)      662 2024-04-02 05:51:48.000000 tangermeme-0.1.0/setup.py
-drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2024-04-02 05:52:49.862307 tangermeme-0.1.0/tangermeme/
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)      111 2024-04-02 05:51:36.000000 tangermeme-0.1.0/tangermeme/__init__.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     4617 2024-04-02 00:33:14.000000 tangermeme-0.1.0/tangermeme/ablate.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     6383 2024-04-02 01:35:58.000000 tangermeme-0.1.0/tangermeme/design.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    22259 2024-03-28 04:48:35.000000 tangermeme-0.1.0/tangermeme/ersatz.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    14430 2024-03-28 04:48:35.000000 tangermeme-0.1.0/tangermeme/io.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     3707 2024-03-28 04:48:35.000000 tangermeme-0.1.0/tangermeme/ism.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     6550 2024-02-18 21:52:53.000000 tangermeme-0.1.0/tangermeme/kmers.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     4231 2024-04-01 23:34:29.000000 tangermeme-0.1.0/tangermeme/marginalize.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    12384 2024-02-16 06:07:44.000000 tangermeme-0.1.0/tangermeme/match.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     5031 2024-04-02 05:50:43.000000 tangermeme-0.1.0/tangermeme/plot.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     3409 2024-04-01 23:34:04.000000 tangermeme-0.1.0/tangermeme/predict.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     4424 2024-04-01 23:49:41.000000 tangermeme-0.1.0/tangermeme/product.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     3825 2024-04-02 00:33:29.000000 tangermeme-0.1.0/tangermeme/space.py
-drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2024-04-02 05:52:49.890307 tangermeme-0.1.0/tangermeme/tools/
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)        0 2024-02-12 20:33:38.000000 tangermeme-0.1.0/tangermeme/tools/__init__.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    13248 2024-02-19 18:37:49.000000 tangermeme-0.1.0/tangermeme/tools/fimo.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     2445 2024-02-25 18:18:37.000000 tangermeme-0.1.0/tangermeme/tools/tomtom.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     9101 2024-02-16 06:07:44.000000 tangermeme-0.1.0/tangermeme/utils.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     5454 2024-03-28 04:48:35.000000 tangermeme-0.1.0/tangermeme/variant_effect.py
-drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2024-04-02 05:52:50.014307 tangermeme-0.1.0/tangermeme.egg-info/
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)      556 2024-04-02 05:52:49.000000 tangermeme-0.1.0/tangermeme.egg-info/PKG-INFO
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)      851 2024-04-02 05:52:49.000000 tangermeme-0.1.0/tangermeme.egg-info/SOURCES.txt
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)        1 2024-04-02 05:52:49.000000 tangermeme-0.1.0/tangermeme.egg-info/dependency_links.txt
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)      139 2024-04-02 05:52:49.000000 tangermeme-0.1.0/tangermeme.egg-info/requires.txt
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)       28 2024-04-02 05:52:49.000000 tangermeme-0.1.0/tangermeme.egg-info/top_level.txt
-drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2024-04-02 05:52:50.010307 tangermeme-0.1.0/tests/
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    16973 2024-04-02 00:32:57.000000 tangermeme-0.1.0/tests/test_ablate.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    25611 2024-03-28 04:48:35.000000 tangermeme-0.1.0/tests/test_ersatz.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    22795 2024-03-28 04:48:35.000000 tangermeme-0.1.0/tests/test_io.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     5107 2024-03-28 05:30:44.000000 tangermeme-0.1.0/tests/test_ism.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     1536 2024-02-19 00:37:13.000000 tangermeme-0.1.0/tests/test_kmers.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    11000 2024-04-02 00:59:56.000000 tangermeme-0.1.0/tests/test_marginalize.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    13448 2024-02-16 07:04:10.000000 tangermeme-0.1.0/tests/test_match.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     6951 2024-04-02 00:59:49.000000 tangermeme-0.1.0/tests/test_predict.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    23100 2024-04-02 01:08:34.000000 tangermeme-0.1.0/tests/test_product.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    11548 2024-04-02 01:00:03.000000 tangermeme-0.1.0/tests/test_space.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     6841 2024-02-16 07:04:33.000000 tangermeme-0.1.0/tests/test_utils.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     7610 2024-03-28 04:48:35.000000 tangermeme-0.1.0/tests/test_variant_effect.py
+drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2024-03-28 15:12:46.243402 tangermeme-0.1.0rc0/
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     1072 2024-02-04 20:42:51.000000 tangermeme-0.1.0rc0/LICENSE
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)      559 2024-03-28 15:12:46.235402 tangermeme-0.1.0rc0/PKG-INFO
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     3251 2024-03-28 05:30:44.000000 tangermeme-0.1.0rc0/README.md
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)       38 2024-03-28 15:12:46.243402 tangermeme-0.1.0rc0/setup.cfg
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)      665 2024-03-28 15:11:06.000000 tangermeme-0.1.0rc0/setup.py
+drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2024-03-28 15:12:46.111402 tangermeme-0.1.0rc0/tangermeme/
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)      114 2024-03-28 15:11:24.000000 tangermeme-0.1.0rc0/tangermeme/__init__.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    22259 2024-03-28 04:48:35.000000 tangermeme-0.1.0rc0/tangermeme/ersatz.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    14430 2024-03-28 04:48:35.000000 tangermeme-0.1.0rc0/tangermeme/io.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     3707 2024-03-28 04:48:35.000000 tangermeme-0.1.0rc0/tangermeme/ism.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     6550 2024-02-18 21:52:53.000000 tangermeme-0.1.0rc0/tangermeme/kmers.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     6991 2024-03-12 01:37:58.000000 tangermeme-0.1.0rc0/tangermeme/marginalize.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    12384 2024-02-16 06:07:44.000000 tangermeme-0.1.0rc0/tangermeme/match.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     5018 2024-02-16 06:07:44.000000 tangermeme-0.1.0rc0/tangermeme/plot.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     6062 2024-03-28 04:48:35.000000 tangermeme-0.1.0rc0/tangermeme/predict.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     7703 2024-03-28 04:48:35.000000 tangermeme-0.1.0rc0/tangermeme/space.py
+drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2024-03-28 15:12:46.167402 tangermeme-0.1.0rc0/tangermeme/tools/
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)        0 2024-02-12 20:33:38.000000 tangermeme-0.1.0rc0/tangermeme/tools/__init__.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    13248 2024-02-19 18:37:49.000000 tangermeme-0.1.0rc0/tangermeme/tools/fimo.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     2445 2024-02-25 18:18:37.000000 tangermeme-0.1.0rc0/tangermeme/tools/tomtom.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     9101 2024-02-16 06:07:44.000000 tangermeme-0.1.0rc0/tangermeme/utils.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     5454 2024-03-28 04:48:35.000000 tangermeme-0.1.0rc0/tangermeme/variant_effect.py
+drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2024-03-28 15:12:46.227402 tangermeme-0.1.0rc0/tangermeme.egg-info/
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)      559 2024-03-28 15:12:45.000000 tangermeme-0.1.0rc0/tangermeme.egg-info/PKG-INFO
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)      744 2024-03-28 15:12:46.000000 tangermeme-0.1.0rc0/tangermeme.egg-info/SOURCES.txt
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)        1 2024-03-28 15:12:45.000000 tangermeme-0.1.0rc0/tangermeme.egg-info/dependency_links.txt
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)      139 2024-03-28 15:12:45.000000 tangermeme-0.1.0rc0/tangermeme.egg-info/requires.txt
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)       28 2024-03-28 15:12:45.000000 tangermeme-0.1.0rc0/tangermeme.egg-info/top_level.txt
+drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2024-03-28 15:12:46.223402 tangermeme-0.1.0rc0/tests/
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    25611 2024-03-28 04:48:35.000000 tangermeme-0.1.0rc0/tests/test_ersatz.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    22795 2024-03-28 04:48:35.000000 tangermeme-0.1.0rc0/tests/test_io.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     5107 2024-03-28 05:30:44.000000 tangermeme-0.1.0rc0/tests/test_ism.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     1536 2024-02-19 00:37:13.000000 tangermeme-0.1.0rc0/tests/test_kmers.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    18843 2024-03-28 04:48:35.000000 tangermeme-0.1.0rc0/tests/test_marginalize.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    13448 2024-02-16 07:04:10.000000 tangermeme-0.1.0rc0/tests/test_match.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    12913 2024-02-16 07:04:20.000000 tangermeme-0.1.0rc0/tests/test_predict.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    19522 2024-03-28 04:48:35.000000 tangermeme-0.1.0rc0/tests/test_space.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     6841 2024-02-16 07:04:33.000000 tangermeme-0.1.0rc0/tests/test_utils.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     7610 2024-03-28 04:48:35.000000 tangermeme-0.1.0rc0/tests/test_variant_effect.py
```

### Comparing `tangermeme-0.1.0/LICENSE` & `tangermeme-0.1.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `tangermeme-0.1.0/PKG-INFO` & `tangermeme-0.1.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tangermeme
-Version: 0.1.0
+Version: 0.1.0rc0
 Summary: Biological sequence analysis for the modern age.
 Home-page: https://github.com/jmschrei/tangermeme
 Author: Jacob Schreiber
 Author-email: jmschreiber91@gmail.com
 License: LICENSE.txt
 License-File: LICENSE
 Requires-Dist: numpy>=1.14.2
```

### Comparing `tangermeme-0.1.0/setup.py` & `tangermeme-0.1.0rc0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='tangermeme',
-    version='0.1.0',
+    version='0.1.0-rc',
     author='Jacob Schreiber',
     author_email='jmschreiber91@gmail.com',
     packages=['tangermeme', 'tangermeme/tools'],
     scripts=[],
     url='https://github.com/jmschrei/tangermeme',
     license='LICENSE.txt',
     description='Biological sequence analysis for the modern age.',
```

### Comparing `tangermeme-0.1.0/tangermeme/ersatz.py` & `tangermeme-0.1.0rc0/tangermeme/ersatz.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.1.0/tangermeme/io.py` & `tangermeme-0.1.0rc0/tangermeme/io.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.1.0/tangermeme/ism.py` & `tangermeme-0.1.0rc0/tangermeme/ism.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.1.0/tangermeme/kmers.py` & `tangermeme-0.1.0rc0/tangermeme/kmers.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.1.0/tangermeme/match.py` & `tangermeme-0.1.0rc0/tangermeme/match.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.1.0/tangermeme/plot.py` & `tangermeme-0.1.0rc0/tangermeme/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,14 @@
 	if annotations is not None:
 		annotations_ = annotations[annotations['start'] > start]
 		annotations_ = annotations_[annotations_['end'] < end]
 		annotations_ = annotations_.sort_values(["score"], ascending=False)
 
 		ylim = ylim or max(abs(X_attr.min()), abs(X_attr.max()))
 		plt.ylim(-ylim, ylim)
-		r = ylim*2
 
 		motifs = numpy.zeros((end-start, annotations_.shape[0]))
 		for _, row in annotations_.iterrows():
 			(motif, motif_start, motif_end, _, score, _, _) = row
 			motif_start -= start
 			motif_end -= start
 			
@@ -127,17 +126,17 @@
 						text = "{}: ({:3.3})".format(motif, score)
 						motifs[motif_start:motif_end, i] = 1
 						y_offset += 0.2*i
 						
 						xp = [motif_start, motif_end]
 						yp = [-ylim*y_offset, -ylim*y_offset]
 
-						plt.plot(xp, yp, color='0.3', linewidth=2)        
+						plt.plot(xp, yp, color='0.7', linewidth=2)        
 						plt.text(xp[0], -ylim*(y_offset+0.1), text, 
-							color='0.3', fontsize=9)
+							color='0.7', fontsize=9)
 						
 					elif show_extra:
 						s = motif_start
 
 						motifs[motif_start:motif_start+len(motif)*2, i] = 1
 						y_offset += -0.1 + 0.2*(n_tracks) + 0.1*(i-n_tracks)
```

### Comparing `tangermeme-0.1.0/tangermeme/space.py` & `tangermeme-0.1.0rc0/tangermeme/space.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 
 import numpy
 import torch
 
 from .utils import one_hot_encode
 from .ersatz import multisubstitute
 from .predict import predict
+from .predict import predict_cross
 
 
-def space(model, X, motifs, spacing, start=None, alphabet=['A', 'C', 'G', 'T'], 
-	args=None, batch_size=32, device='cuda', verbose=False):
+def space(model, X, motifs, spacing, args=None, start=None, 
+	alphabet=['A', 'C', 'G', 'T'], batch_size=32, device='cuda', 
+	verbose=False):
 	"""Runs a single spacing experiment and returns predictions.
 
 	Given a predictive model, a set of motifs to insert and the spacings
 	between them, and a set of background sequences, return the predictions 
 	from the model when using the background sequences and after inserting 
 	the motifs into the sequences.
 
@@ -35,34 +37,34 @@
 
 	spacing: list or int
 		An integer specifying a constant spacing between all motifs or a list
 		of spacings of length equal to n-1 where n is the number of motifs. If
 		a list is provided, the $i$-th entry should be interpreted as the
 		distance after the $i$-th motif that the $i+1$-th motif begins.
 
+	args: tuple or list or None
+		An optional set of additional arguments to pass into the model. If
+		provided, each element in the tuple or list is one input to the model
+		and the element must be formatted to be the same batch size as `X`. If
+		None, no additional arguments are passed into the forward function.
+		Default is None.
+
 	start: int or None, optional
 		The starting position of where to insert the motif. If None, insert the
 		motif into the middle of the sequence such that the middle of the motif
 		occurs at the middle of the sequence. Default is None.
 
 	alphabet : set or tuple or list, optional
 		A pre-defined alphabet where the ordering of the symbols is the same
 		as the index into the returned tensor, i.e., for the alphabet ['A', 'B']
 		the returned tensor will have a 1 at index 0 if the character was 'A'.
 		Characters outside the alphabet are ignored and none of the indexes are
 		set to 1. This is not necessary or used if a one-hot encoded tensor is
 		provided for the motif. Default is ['A', 'C', 'G', 'T'].
 
-	args: tuple or list or None
-		An optional set of additional arguments to pass into the model. If
-		provided, each element in the tuple or list is one input to the model
-		and the element must be formatted to be the same batch size as `X`. If
-		None, no additional arguments are passed into the forward function.
-		Default is None.
-
 	batch_size: int, optional
 		The number of examples to make predictions for at a time. Default is 32.
 
 	device: str or torch.device
 		The device to move the model and batches to when making predictions. If
 		set to 'cuda' without a GPU, this function will crash and must be set
 		to 'cpu'. Default is 'cuda'. 
@@ -89,7 +91,98 @@
 		alphabet=alphabet)
 	y_before = predict(model, X, args=args, batch_size=batch_size, 
 		device=device, verbose=verbose)
 	y_after = predict(model, X_perturb, args=args, batch_size=batch_size, 
 		device=device, verbose=verbose)
 
 	return y_before, y_after
+
+
+def space_cross(model, X, motifs, spacing, args, start=None, 
+	alphabet=['A', 'C', 'G', 'T'], batch_size=32, device='cuda', 
+	verbose=False):
+	"""Runs spacings on X for each element in `args`.
+
+	This function will return a spacing on X for each index in the elements of
+	`args`. Specifically, the tensors provided in args must all have the same 
+	first dimension (the batch size) and one marginalization is performed on X 
+	for each element in those tensors. 
+
+	More concretely, if a model's forward function takes in X and some other
+	inputs W and Z with shapes (5, 10) and (5, 3, 8) respectively, 5
+	marginalizations will be done, the first with W[0] and Z[0] passed in, the
+	second with W[1] and Z[1] passed in, etc..
+
+
+	Parameters
+	----------
+	model: torch.nn.Module
+		A PyTorch model to use for making predictions. These models can take in
+		any number of inputs and make any number of outputs. The additional
+		inputs must be specified in the `args` parameter.
+
+	X: torch.tensor, shape=(-1, len(alphabet), length)
+		A one-hot encoded set of sequences to have a motif inserted into.
+
+	motifs: list of torch.tensor, shape=(-1, len(alphabet), motif_length)
+		A list of strings or of one-hot encoded version of a short motif to 
+		substitute into the set of sequences.
+
+	spacing: list or int
+		An integer specifying a constant spacing between all motifs or a list
+		of spacings of length equal to n-1 where n is the number of motifs. If
+		a list is provided, the $i$-th entry should be interpreted as the
+		distance after the $i$-th motif that the $i+1$-th motif begins.
+
+	args: tuple or list
+		A set of additional arguments to pass into the model. Each element in 
+		the tuple or list is one input to the model and each tensor in the list
+		must have the same first dimension. Does not have to have the same
+		batch size as `X`.
+
+	start: int or None, optional
+		The starting position of where to insert the motif. If None, insert the
+		motif into the middle of the sequence such that the middle of the motif
+		occurs at the middle of the sequence. Default is None.
+
+	alphabet : set or tuple or list, optional
+		A pre-defined alphabet where the ordering of the symbols is the same
+		as the index into the returned tensor, i.e., for the alphabet ['A', 'B']
+		the returned tensor will have a 1 at index 0 if the character was 'A'.
+		Characters outside the alphabet are ignored and none of the indexes are
+		set to 1. This is not necessary or used if a one-hot encoded tensor is
+		provided for the motif. Default is ['A', 'C', 'G', 'T'].
+
+	batch_size: int, optional
+		The number of examples to make predictions for at a time. Default is 32.
+
+	device: str or torch.device
+		The device to move the model and batches to when making predictions. If
+		set to 'cuda' without a GPU, this function will crash and must be set
+		to 'cpu'. Default is 'cuda'. 
+
+	verbose: bool, optional
+		Whether to display a progress bar during predictions. Default is False.
+
+	Returns
+	-------
+	y_before: torch.Tensor or list of torch.Tensors
+		The predictions from the model before inserting the motif in. If the
+		output from the model's forward function is a single tensor, it will
+		return that. If the model outputs a list of tensors, it will return
+		those.
+
+	y_after: torch.Tensor or list of torch.Tensors
+		The predictions from the model after inserting the motif in. If the
+		output from the model's forward function is a single tensor, it will
+		return that. If the model outputs a list of tensors, it will return
+		those.
+	"""
+
+	X_perturb = multisubstitute(X, motifs, spacing, start=start, 
+		alphabet=alphabet)
+	y_before = predict_cross(model, X, args=args, batch_size=batch_size,
+		device=device, verbose=verbose)
+	y_after = predict_cross(model, X_perturb, args=args, batch_size=batch_size, 
+		device=device, verbose=verbose)
+
+	return y_before, y_after
```

### Comparing `tangermeme-0.1.0/tangermeme/tools/fimo.py` & `tangermeme-0.1.0rc0/tangermeme/tools/fimo.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.1.0/tangermeme/tools/tomtom.py` & `tangermeme-0.1.0rc0/tangermeme/tools/tomtom.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.1.0/tangermeme/utils.py` & `tangermeme-0.1.0rc0/tangermeme/utils.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.1.0/tangermeme/variant_effect.py` & `tangermeme-0.1.0rc0/tangermeme/variant_effect.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.1.0/tangermeme.egg-info/PKG-INFO` & `tangermeme-0.1.0rc0/tangermeme.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tangermeme
-Version: 0.1.0
+Version: 0.1.0rc0
 Summary: Biological sequence analysis for the modern age.
 Home-page: https://github.com/jmschrei/tangermeme
 Author: Jacob Schreiber
 Author-email: jmschreiber91@gmail.com
 License: LICENSE.txt
 License-File: LICENSE
 Requires-Dist: numpy>=1.14.2
```

### Comparing `tangermeme-0.1.0/tangermeme.egg-info/SOURCES.txt` & `tangermeme-0.1.0rc0/tangermeme.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,33 @@
 LICENSE
 README.md
 setup.py
 tangermeme/__init__.py
-tangermeme/ablate.py
-tangermeme/design.py
 tangermeme/ersatz.py
 tangermeme/io.py
 tangermeme/ism.py
 tangermeme/kmers.py
 tangermeme/marginalize.py
 tangermeme/match.py
 tangermeme/plot.py
 tangermeme/predict.py
-tangermeme/product.py
 tangermeme/space.py
 tangermeme/utils.py
 tangermeme/variant_effect.py
 tangermeme.egg-info/PKG-INFO
 tangermeme.egg-info/SOURCES.txt
 tangermeme.egg-info/dependency_links.txt
 tangermeme.egg-info/requires.txt
 tangermeme.egg-info/top_level.txt
 tangermeme/tools/__init__.py
 tangermeme/tools/fimo.py
 tangermeme/tools/tomtom.py
-tests/test_ablate.py
 tests/test_ersatz.py
 tests/test_io.py
 tests/test_ism.py
 tests/test_kmers.py
 tests/test_marginalize.py
 tests/test_match.py
 tests/test_predict.py
-tests/test_product.py
 tests/test_space.py
 tests/test_utils.py
 tests/test_variant_effect.py
```

### Comparing `tangermeme-0.1.0/tests/test_ablate.py` & `tangermeme-0.1.0rc0/tests/test_space.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-# test_ablate.py
+# test_marginalize.py
 # Contact: Jacob Schreiber <jmschreiber91@gmail.com>
 
 import numpy
 import torch
 import pytest
 
 from tangermeme.utils import one_hot_encode
 from tangermeme.utils import random_one_hot
 
-from tangermeme.ablate import ablate
-from tangermeme.ersatz import substitute
+from tangermeme.space import space
+from tangermeme.space import space_cross
+
+from tangermeme.marginalize import marginalize
+from tangermeme.marginalize import marginalize_cross
 
 from .toy_models import SumModel
 from .toy_models import FlattenDense
 from .toy_models import Conv
 from .toy_models import Scatter
 from .toy_models import ConvDense
 
@@ -23,17 +26,15 @@
 
 torch.manual_seed(0)
 torch.use_deterministic_algorithms(True)
 
 
 @pytest.fixture
 def X():
-	X_ = random_one_hot((64, 4, 100), random_state=0).type(torch.float32)
-	X_ = substitute(X_, "ACGTACGT")
-	return X_
+	return random_one_hot((64, 4, 100), random_state=0).type(torch.float32)
 
 
 @pytest.fixture
 def alpha():
 	r = numpy.random.RandomState(0)
 	return torch.from_numpy(r.randn(64, 1)).type(torch.float32)
 
@@ -41,190 +42,147 @@
 def beta():
 	r = numpy.random.RandomState(1)
 	return torch.from_numpy(r.randn(64, 1)).type(torch.float32)
 
 
 ##
 
-def test_ablate_summodel(X):
+def test_space_summodel(X):
 	torch.manual_seed(0)
 	model = SumModel()
-	y_before, y_after = ablate(model, X, 46, 54, batch_size=5, device='cpu')
+	y_before, y_after = space(model, X, ["ACGTC", "GAGA"], 1, 
+		batch_size=5, device='cpu')
 
 	assert y_before.shape == (64, 4)
 	assert y_before.dtype == torch.float32
 	assert y_before.sum() == X.sum()
-
 	assert_array_almost_equal(y_before[:8], [
-		[26., 23., 20., 31.],
-        [27., 18., 29., 26.],
-        [27., 25., 22., 26.],
-        [21., 33., 18., 28.],
-        [26., 22., 24., 28.],
-        [28., 28., 22., 22.],
-        [28., 16., 23., 33.],
-        [20., 29., 31., 20.]])
+		[25., 24., 19., 32.],
+        [26., 18., 29., 27.],
+        [28., 25., 21., 26.],
+        [21., 33., 19., 27.],
+        [27., 22., 23., 28.],
+        [31., 27., 21., 21.],
+        [26., 20., 21., 33.],
+        [21., 28., 31., 20.]])
 
-	assert y_after.shape == (64, 20, 4)
+	assert y_after.shape == (64, 4)
 	assert y_after.dtype == torch.float32
-	assert y_after[:, 0].sum() == X.sum()
-	assert_array_almost_equal(y_after[:8, 0], [
-		[26., 23., 20., 31.],
-        [27., 18., 29., 26.],
-        [27., 25., 22., 26.],
-        [21., 33., 18., 28.],
-        [26., 22., 24., 28.],
-        [28., 28., 22., 22.],
-        [28., 16., 23., 33.],
-        [20., 29., 31., 20.]])
-
-	for i in range(8):
-		assert_array_almost_equal(y_after[:, 0], y_after[:, i])
-		assert_array_almost_equal(y_before, y_after[:, 0])
+	assert y_after.sum() == X.sum()
+	assert_array_almost_equal(y_after[:8], [
+		[28., 22., 21., 29.],
+        [28., 18., 29., 25.],
+        [28., 24., 23., 25.],
+        [21., 34., 19., 26.],
+        [27., 22., 25., 26.],
+        [28., 29., 22., 21.],
+        [28., 17., 23., 32.],
+        [22., 28., 32., 18.]])
 
-	y_before2, y_after2 = ablate(model, X, 0, -1, batch_size=1, 
-		device='cpu')
+	y_before2, y_after2 = space(model, X, ["ACGTC", "GAGA"], 1, 
+		batch_size=64, device='cpu')
 	assert_array_almost_equal(y_before, y_before2)
 	assert_array_almost_equal(y_after, y_after2)	
 
 
-def test_ablate_flattendense(X):
+def test_space_flattendense(X):
 	torch.manual_seed(0)
 	model = FlattenDense()
-	y_before, y_after = ablate(model, X, 46, 54, random_state=0, batch_size=8, 
-		device='cpu')
+	y_before, y_after = space(model, X, ["ACGTC", "GAGA"], 1, 
+		batch_size=5, device='cpu')
 
 	assert y_before.shape == (64, 3)
 	assert y_before.dtype == torch.float32
 	assert_array_almost_equal(y_before[:8], [
-		[ 0.2161,  0.3207,  0.0147],
-        [-0.0664, -0.0846, -0.2305],
-        [-0.0801,  0.1022, -0.0152],
-        [-0.0967,  0.0734, -0.0764],
-        [ 0.0647, -0.1418, -0.1951],
-        [-0.3011, -0.0956, -0.3683],
-        [-0.2201, -0.0099, -0.2535],
-        [-0.3861,  0.6259, -0.3530]], 4)
+		[ 0.1928,  0.2788, -0.1000],
+        [-0.0505,  0.0174, -0.1751],
+        [-0.1408,  0.0105,  0.0673],
+        [-0.2375, -0.0069,  0.0835],
+        [ 0.0442, -0.0692, -0.1565],
+        [-0.3489, -0.0876, -0.2994],
+        [-0.3894, -0.1332, -0.3717],
+        [-0.3682,  0.5173, -0.4089]], 4)
 
-	assert y_after.shape == (64, 20, 3)
+	assert y_after.shape == (64, 3)
 	assert y_after.dtype == torch.float32
-	assert_array_almost_equal(y_after[:8, :2], [
-		[[ 0.1324,  0.3553,  0.1465],
-         [ 0.2455,  0.3811,  0.1003]],
-
-        [[-0.1501, -0.0500, -0.0986],
-         [-0.0370, -0.0243, -0.1448]],
-
-        [[-0.1639,  0.1369,  0.1167],
-         [-0.0508,  0.1626,  0.0705]],
-
-        [[-0.1805,  0.1081,  0.0555],
-         [-0.0674,  0.1338,  0.0092]],
-
-        [[-0.0191, -0.1072, -0.0632],
-         [ 0.0940, -0.0814, -0.1094]],
-
-        [[-0.3848, -0.0610, -0.2364],
-         [-0.2718, -0.0352, -0.2826]],
-
-        [[-0.3039,  0.0247, -0.1216],
-         [-0.1908,  0.0504, -0.1678]],
-
-        [[-0.4698,  0.6605, -0.2211],
-         [-0.3568,  0.6863, -0.2673]]], 4)
-
-	y_before2, y_after2 = ablate(model, X, 0, -1, batch_size=1, 
-		device='cpu')
-	assert_array_almost_equal(y_before, y_before2, 4)
-	assert_raises(AssertionError, assert_array_almost_equal, y_after, y_after2)
-
+	assert_array_almost_equal(y_after[:8], [
+		[ 0.1087,  0.3662,  0.0668],
+        [-0.1331,  0.0071, -0.0907],
+        [-0.3239,  0.0593,  0.1154],
+        [-0.3762,  0.0659,  0.0011],
+        [-0.1361, -0.0605, -0.0853],
+        [-0.4873, -0.1080, -0.3462],
+        [-0.3656, -0.0071, -0.1459],
+        [-0.4935,  0.6714, -0.3008]], 4)
 
-def test_ablate_flattendense_alpha_beta(X, alpha, beta):
-	torch.manual_seed(0)
-	model = FlattenDense()
-
-	y_before, y_after = ablate(model, X, 46, 54, random_state=0, batch_size=8,
-		args=(alpha, beta), device='cpu')
-	y_before0, y_after0 = ablate(model, X, 46, 54, random_state=0, batch_size=8,
-		device='cpu')
-
-	assert y_before.shape == (64, 3)
-	assert y_before.dtype == torch.float32
-	assert_array_almost_equal(y_before, y_before0 * beta + alpha)
-	assert_array_almost_equal(y_after, y_after0 * beta[:, None] + alpha[:, None])
-
-	assert_array_almost_equal(y_before[:2], [
-		[2.1151, 2.2849, 1.7879],
-        [0.4407, 0.4519, 0.5412]], 4)
-
-	assert y_after.shape == (64, 20, 3)
-	assert y_after.dtype == torch.float32
-	assert_array_almost_equal(y_after[:2, :2], [
-		[[1.9791, 2.3412, 2.0021],
-         [2.1628, 2.3830, 1.9270]],
-
-        [[0.4920, 0.4307, 0.4605],
-         [0.4228, 0.4150, 0.4888]]], 4)
+	y_before2, y_after2 = space(model, X, ["ACGTC", "GAGA"], 1, 
+		batch_size=64, device='cpu')
+	assert_array_almost_equal(y_before, y_before2)
+	assert_array_almost_equal(y_after, y_after2)
 
 
-def test_ablate_conv(X):
+def test_space_conv(X):
 	torch.manual_seed(0)
 	model = Conv()
-	y_before, y_after = ablate(model, X, 46, 54, random_state=0, batch_size=8, 
-		device='cpu')
+	y_before, y_after = space(model, X, ["ACGTC", "GAGA"], 1, 
+		start=0, batch_size=5, device='cpu')
 
 	assert y_before.shape == (64, 12, 98)
 	assert y_before.dtype == torch.float32
-	assert_array_almost_equal(y_before[:2, :4, :6], [
-		[[-0.2713, -0.5317, -0.3737, -0.4055, -0.3269, -0.3269],
-         [-0.2988,  0.0980, -0.1013, -0.2560,  0.2595,  0.2595],
-         [-0.1247,  0.1433, -0.3111, -0.3220, -0.4084, -0.4084],
-         [-0.1362, -0.0067,  0.5554,  0.1810,  0.2007,  0.2007]],
-
-        [[-0.4805, -0.1669, -0.5863, -0.0537, -0.2702, -0.1669],
-         [-0.3709, -0.3077, -0.5910,  0.0165, -0.6573, -0.3077],
-         [ 0.4396, -0.1558,  0.2097, -0.0929,  0.6608, -0.1558],
-         [-0.0027,  0.4644,  0.1406, -0.1111, -0.3111,  0.4644]]], 4)
+	assert_array_almost_equal(y_before[:2, :4, :10], [
+		[[-0.2713, -0.5317, -0.3737, -0.4055, -0.3269, -0.3269, -0.1928,
+          -0.3509, -0.4816, -0.3197],
+         [-0.2988,  0.0980, -0.1013, -0.2560,  0.2595,  0.2595,  0.2167,
+           0.4330, -0.0124,  0.3218],
+         [-0.1247,  0.1433, -0.3111, -0.3220, -0.4084, -0.4084, -0.2111,
+          -0.3884, -0.3460, -0.3052],
+         [-0.1362, -0.0067,  0.5554,  0.1810,  0.2007,  0.2007, -0.1166,
+           0.0337,  0.1722, -0.3441]],
+
+        [[-0.4805, -0.1669, -0.5863, -0.0537, -0.2702, -0.1669, -0.4055,
+          -0.5078, -0.0848, -0.5863],
+         [-0.3709, -0.3077, -0.5910,  0.0165, -0.6573, -0.3077, -0.2560,
+          -0.0755,  0.1277, -0.5910],
+         [ 0.4396, -0.1558,  0.2097, -0.0929,  0.6608, -0.1558, -0.3220,
+           0.1234, -0.1761,  0.2097],
+         [-0.0027,  0.4644,  0.1406, -0.1111, -0.3111,  0.4644,  0.1810,
+           0.1603,  0.2667,  0.1406]]], 4)
 
-	assert y_after.shape == (64, 20, 12, 98)
+	assert y_after.shape == (64, 12, 98)
 	assert y_after.dtype == torch.float32
-	assert_array_almost_equal(y_after[:2, :2, :4, :6], [
-		[[[-0.2713, -0.5317, -0.3737, -0.4055, -0.3269, -0.3269],
-          [-0.2988,  0.0980, -0.1013, -0.2560,  0.2595,  0.2595],
-          [-0.1247,  0.1433, -0.3111, -0.3220, -0.4084, -0.4084],
-          [-0.1362, -0.0067,  0.5554,  0.1810,  0.2007,  0.2007]],
-
-         [[-0.2713, -0.5317, -0.3737, -0.4055, -0.3269, -0.3269],
-          [-0.2988,  0.0980, -0.1013, -0.2560,  0.2595,  0.2595],
-          [-0.1247,  0.1433, -0.3111, -0.3220, -0.4084, -0.4084],
-          [-0.1362, -0.0067,  0.5554,  0.1810,  0.2007,  0.2007]]],
-
-
-        [[[-0.4805, -0.1669, -0.5863, -0.0537, -0.2702, -0.1669],
-          [-0.3709, -0.3077, -0.5910,  0.0165, -0.6573, -0.3077],
-          [ 0.4396, -0.1558,  0.2097, -0.0929,  0.6608, -0.1558],
-          [-0.0027,  0.4644,  0.1406, -0.1111, -0.3111,  0.4644]],
-
-         [[-0.4805, -0.1669, -0.5863, -0.0537, -0.2702, -0.1669],
-          [-0.3709, -0.3077, -0.5910,  0.0165, -0.6573, -0.3077],
-          [ 0.4396, -0.1558,  0.2097, -0.0929,  0.6608, -0.1558],
-          [-0.0027,  0.4644,  0.1406, -0.1111, -0.3111,  0.4644]]]], 4)
-
-	for i in range(20):
-		assert_array_almost_equal(y_before[:, :, :35], y_after[:, i, :, :35])
-		assert_array_almost_equal(y_before[:, :, 60:], y_after[:, i, :, 60:])
-		assert_raises(AssertionError, assert_array_almost_equal, 
-			y_before[:, :, 35:60], y_after[:, i, :, 35:60])
+	assert_array_almost_equal(y_after[:2, :4, :10], [
+		[[-0.3983, -0.2996, -0.2749, -0.3509, -0.5846, -0.1916, -0.1358,
+          -0.2702, -0.0328, -0.3983],
+         [-0.1937, -0.0358, -0.2188,  0.4330, -0.0807, -0.1418, -0.4189,
+          -0.6573, -0.3505, -0.1937],
+         [-0.2188, -0.0922, -0.1907, -0.3884, -0.4600,  0.5745, -0.0725,
+           0.6608,  0.0415, -0.2188],
+         [-0.3638,  0.0378,  0.0811,  0.0337,  0.1116, -0.2914,  0.0865,
+          -0.3111,  0.1471, -0.3638]],
+
+        [[-0.3983, -0.2996, -0.2749, -0.3197, -0.2685, -0.2737, -0.1358,
+          -0.2702, -0.1669, -0.5863],
+         [-0.1937, -0.0358, -0.2188,  0.3218, -0.1470, -0.5773, -0.4189,
+          -0.6573, -0.3077, -0.5910],
+         [-0.2188, -0.0922, -0.1907, -0.3052, -0.0089,  0.5948, -0.0725,
+           0.6608, -0.1558,  0.2097],
+         [-0.3638,  0.0378,  0.0811, -0.3441, -0.3401, -0.0938,  0.0865,
+          -0.3111,  0.4644,  0.1406]]], 4)
+
+	y_before2, y_after2 = space(model, X, ["ACGTC", "GAGA"], 1, 
+		start=0, batch_size=64, device='cpu')
+	assert_array_almost_equal(y_before, y_before2)
+	assert_array_almost_equal(y_after, y_after2)
 
 
-def test_ablate_scatter(X):
+def test_space_scatter(X):
 	torch.manual_seed(0)
 	model = Scatter()
-	y_before, y_after = ablate(model, X, 46, 54, random_state=0, batch_size=8, 
-		device='cpu')
+	y_before, y_after = space(model, X, ["ACGTC", "GAGA"], 1, 
+		start=0, batch_size=8, device='cpu')
 
 	assert y_before.shape == (64, 100, 4)
 	assert y_before.dtype == torch.float32
 	assert y_before.sum() == X.sum()
 	assert (y_before.sum(axis=-1) == X.sum(axis=1)).all()
 	assert (y_before.sum(axis=1) == X.sum(axis=-1)).all()
 	assert_array_almost_equal(y_before[:4, :5], [
@@ -248,283 +206,395 @@
 
         [[0., 1., 0., 0.],
          [1., 0., 0., 0.],
          [0., 0., 0., 1.],
          [1., 0., 0., 0.],
          [0., 0., 1., 0.]]], 4)
 
-	assert y_after.shape == (64, 20, 100, 4)
+	assert y_after.shape == (64, 100, 4)
 	assert y_after.dtype == torch.float32
-	assert y_after[:, 0].sum() == X.sum()
-	assert_array_almost_equal(y_after[:4, :2, :5], [
-		[[[1., 0., 0., 0.],
-          [0., 0., 0., 1.],
-          [0., 1., 0., 0.],
-          [1., 0., 0., 0.],
-          [0., 0., 0., 1.]],
-
-         [[1., 0., 0., 0.],
-          [0., 0., 0., 1.],
-          [0., 1., 0., 0.],
-          [1., 0., 0., 0.],
-          [0., 0., 0., 1.]]],
-
-
-        [[[0., 1., 0., 0.],
-          [0., 0., 1., 0.],
-          [1., 0., 0., 0.],
-          [0., 0., 0., 1.],
-          [1., 0., 0., 0.]],
-
-         [[0., 1., 0., 0.],
-          [0., 0., 1., 0.],
-          [1., 0., 0., 0.],
-          [0., 0., 0., 1.],
-          [1., 0., 0., 0.]]],
-
-
-        [[[0., 1., 0., 0.],
-          [0., 0., 1., 0.],
-          [0., 0., 0., 1.],
-          [0., 0., 1., 0.],
-          [0., 0., 1., 0.]],
-
-         [[0., 1., 0., 0.],
-          [0., 0., 1., 0.],
-          [0., 0., 0., 1.],
-          [0., 0., 1., 0.],
-          [0., 0., 1., 0.]]],
-
-
-        [[[0., 1., 0., 0.],
-          [1., 0., 0., 0.],
-          [0., 0., 0., 1.],
-          [1., 0., 0., 0.],
-          [0., 0., 1., 0.]],
-
-         [[0., 1., 0., 0.],
-          [1., 0., 0., 0.],
-          [0., 0., 0., 1.],
-          [1., 0., 0., 0.],
-          [0., 0., 1., 0.]]]], 4)
+	assert y_after.sum() == X.sum()
+	assert_array_almost_equal(y_after[:4, :5], [
+		[[1., 0., 0., 0.],
+         [0., 1., 0., 0.],
+         [0., 0., 1., 0.],
+         [0., 0., 0., 1.],
+         [0., 1., 0., 0.]],
 
+        [[1., 0., 0., 0.],
+         [0., 1., 0., 0.],
+         [0., 0., 1., 0.],
+         [0., 0., 0., 1.],
+         [0., 1., 0., 0.]],
 
-def test_ablate_convdense(X):
+        [[1., 0., 0., 0.],
+         [0., 1., 0., 0.],
+         [0., 0., 1., 0.],
+         [0., 0., 0., 1.],
+         [0., 1., 0., 0.]],
+
+        [[1., 0., 0., 0.],
+         [0., 1., 0., 0.],
+         [0., 0., 1., 0.],
+         [0., 0., 0., 1.],
+         [0., 1., 0., 0.]]], 4)
+
+	y_before2, y_after2 = space(model, X, ["ACGTC", "GAGA"], 1, 
+		start=0, batch_size=64, device='cpu')
+	assert_array_almost_equal(y_before, y_before2)
+	assert_array_almost_equal(y_after, y_after2)
+
+
+def test_space_convdense(X):
 	torch.manual_seed(0)
 	model = ConvDense()
-	y_before, y_after = ablate(model, X, 46, 54, random_state=0, batch_size=2, 
-		device='cpu')
+	y_before, y_after = space(model, X, ["ACGTC", "GAGA"], 1, 
+		start=0, batch_size=2, device='cpu')
 
 	assert len(y_before) == 2
 	assert y_before[0].shape == (64, 12, 98)
 	assert y_before[1].shape == (64, 3)
 
 	assert y_before[0].dtype == torch.float32
 	assert y_before[1].dtype == torch.float32
 
-	assert_array_almost_equal(y_before[0][:2, :4, 42:46], [
-		[[-0.4906, -0.6971,  0.0397, -0.6363],
-         [-0.3881,  0.2000,  0.2042,  0.1789],
-         [ 0.8900,  0.4674,  0.5009,  0.5628],
-         [-0.4831, -0.2439, -0.0296, -0.4263]],
-
-        [[-0.5812, -0.2696, -0.7301, -0.7149],
-         [ 0.2148,  0.2771,  0.1086,  0.0737],
-         [ 0.2273,  0.3059,  0.5017,  0.4734],
-         [-0.7614, -0.5326, -0.1356, -0.7810]]], 4)
+	assert_array_almost_equal(y_before[0][:2, :4, :4], [
+		[[-0.7757,  0.0397, -0.8799, -1.0194],
+         [ 0.0947,  0.2042, -0.2302, -0.3144],
+         [ 0.3781,  0.5009,  0.8585,  0.6738],
+         [-0.5986, -0.0296, -0.0995, -0.2718]],
+
+        [[-0.6676, -0.8873, -0.8696, -0.4684],
+         [-0.0768, -0.0089,  0.0244,  0.1355],
+         [ 0.4828,  0.5419,  0.3170,  0.3288],
+         [-0.1026, -0.4676, -0.3080, -0.2606]]], 4)
 
 	assert_array_almost_equal(y_before[1][:4], [
-		[ 0.2161,  0.3207,  0.0147],
-        [-0.0664, -0.0846, -0.2305],
-        [-0.0801,  0.1022, -0.0152],
-        [-0.0967,  0.0734, -0.0764]], 4)
-
+		[ 0.1928,  0.2788, -0.1000],
+        [-0.0505,  0.0174, -0.1751],
+        [-0.1408,  0.0105,  0.0673],
+        [-0.2375, -0.0069,  0.0835]], 4)
 
 	assert len(y_after) == 2
-	assert y_after[0].shape == (64, 20, 12, 98)
-	assert y_after[1].shape == (64, 20, 3)
+	assert y_after[0].shape == (64, 12, 98)
+	assert y_after[1].shape == (64, 3)
 
 	assert y_after[0].dtype == torch.float32
 	assert y_after[1].dtype == torch.float32
 
-	assert_array_almost_equal(y_after[0][:2, :2, :4, 42:46], [
-		[[[-4.9062e-01, -6.9711e-01, -4.2652e-04, -7.0773e-01],
-          [-3.8814e-01,  2.0001e-01,  8.2816e-02, -1.9818e-01],
-          [ 8.9002e-01,  4.6741e-01,  4.4968e-01,  4.3157e-01],
-          [-4.8307e-01, -2.4389e-01, -2.8948e-01, -3.6251e-01]],
-
-         [[-4.9062e-01, -6.9711e-01,  1.3353e-01, -3.0229e-01],
-          [-3.8814e-01,  2.0001e-01,  2.7458e-01, -6.5521e-02],
-          [ 8.9002e-01,  4.6741e-01,  5.6203e-01,  5.7124e-01],
-          [-4.8307e-01, -2.4389e-01, -3.2021e-01, -4.2439e-01]]],
-
-
-        [[[-5.8118e-01, -2.6960e-01, -7.7023e-01, -7.8636e-01],
-          [ 2.1482e-01,  2.7712e-01, -1.2824e-02, -3.0346e-01],
-          [ 2.2734e-01,  3.0591e-01,  4.5041e-01,  3.4224e-01],
-          [-7.6136e-01, -5.3260e-01, -3.9553e-01, -7.1724e-01]],
-
-         [[-5.8118e-01, -2.6960e-01, -6.3627e-01, -3.8092e-01],
-          [ 2.1482e-01,  2.7712e-01,  1.7894e-01, -1.7080e-01],
-          [ 2.2734e-01,  3.0591e-01,  5.6276e-01,  4.8191e-01],
-          [-7.6136e-01, -5.3260e-01, -4.2626e-01, -7.7912e-01]]]], 4)
-
-	assert_array_almost_equal(y_after[1][:2, :4], [
-		[[ 0.1324,  0.3553,  0.1465],
-         [ 0.2455,  0.3811,  0.1003],
-         [ 0.1798,  0.2700,  0.1818],
-         [ 0.1989,  0.2952,  0.0110]],
-
-        [[-0.1501, -0.0500, -0.0986],
-         [-0.0370, -0.0243, -0.1448],
-         [-0.1027, -0.1353, -0.0634],
-         [-0.0835, -0.1101, -0.2342]]], 4)
+	assert_array_almost_equal(y_after[0][:2, :4, :4], [
+		[[-3.8092e-01, -8.1744e-01, -7.0452e-01, -1.1013e-01],
+         [-1.7080e-01, -4.1553e-01,  4.2124e-01, -1.3453e-01],
+         [ 4.8191e-01,  8.3968e-01,  1.5083e-01,  8.5779e-01],
+         [-7.7912e-01, -6.6461e-02, -6.1201e-01,  6.5689e-03]],
+
+        [[-3.8092e-01, -8.1744e-01, -7.0452e-01, -4.2652e-04],
+         [-1.7080e-01, -4.1553e-01,  4.2124e-01,  8.2816e-02],
+         [ 4.8191e-01,  8.3968e-01,  1.5083e-01,  4.4968e-01],
+         [-7.7912e-01, -6.6461e-02, -6.1201e-01, -2.8948e-01]]], 4)
+
+	assert_array_almost_equal(y_after[1][:4], [
+		[ 0.2248,  0.2780,  0.0710],
+        [-0.1218,  0.1338, -0.2101],
+        [-0.1292,  0.1851,  0.2033],
+        [-0.2042,  0.1904,  0.2121]], 4)
 
 
-def test_ablate_convdense_alpha(X, alpha):
+def test_space_convdense_batch_size(X):
 	torch.manual_seed(0)
 	model = ConvDense()
-
-	y_before, y_after = ablate(model, X, 46, 54, random_state=0, 
-		args=(alpha[:, :, None],), batch_size=2, device='cpu')
+	y_before, y_after = space(model, X, ["ACGTC", "GAGA"], 1, 
+		batch_size=68, device='cpu')
 
 	assert len(y_before) == 2
 	assert y_before[0].shape == (64, 12, 98)
 	assert y_before[1].shape == (64, 3)
 
-	assert y_before[0].dtype == torch.float32
-	assert y_before[1].dtype == torch.float32
+	assert len(y_after) == 2
+	assert y_after[0].shape == (64, 12, 98)
+	assert y_after[1].shape == (64, 3)
 
-	assert_array_almost_equal(y_before[0][:2, :4, 42:46], [
-		[[ 1.2734,  1.0669,  1.8037,  1.1278],
-         [ 1.3759,  1.9641,  1.9683,  1.9430],
-         [ 2.6541,  2.2315,  2.2650,  2.3268],
-         [ 1.2810,  1.5202,  1.7345,  1.3378]],
-
-        [[-0.1810,  0.1306, -0.3300, -0.3147],
-         [ 0.6150,  0.6773,  0.5087,  0.4738],
-         [ 0.6275,  0.7061,  0.9018,  0.8736],
-         [-0.3612, -0.1324,  0.2645, -0.3808]]], 4)
 
-	assert_array_almost_equal(y_before[1][:4], [
-		[ 0.2161,  0.3207,  0.0147],
-        [-0.0664, -0.0846, -0.2305],
-        [-0.0801,  0.1022, -0.0152],
-        [-0.0967,  0.0734, -0.0764]], 4)
+def test_space_scatter_batch_size(X):
+	torch.manual_seed(0)
+	model = Scatter()
+	y_before, y_after = space(model, X, ["ACGTC", "GAGA"], 1, 
+		batch_size=68, device='cpu')
 
+	assert y_before.shape == (64, 100, 4)
+	assert y_after.shape == (64, 100, 4)
 
-	assert len(y_after) == 2
-	assert y_after[0].shape == (64, 20, 12, 98)
-	assert y_after[1].shape == (64, 20, 3)
 
-	assert y_after[0].dtype == torch.float32
-	assert y_after[1].dtype == torch.float32
+def test_space_raises_shape(X):
+	torch.manual_seed(0)
+	model = Scatter()
+	assert_raises(ValueError, space, model, X[0], ["ACGTC", "ACC"], 0, 
+		device='cpu')
+	assert_raises(ValueError, space, model, X[:, 0], ["ACGTC", "ACC"], 0,
+		device='cpu')
+	assert_raises(ValueError, space, model, X.unsqueeze(0), ["ACGTC", "ACC"], 
+		0, device='cpu')
 
-	assert_array_almost_equal(y_after[0][:2, :2, :4, 42:46], [
-		[[[ 1.2734,  1.0669,  1.7636,  1.0563],
-          [ 1.3759,  1.9641,  1.8469,  1.5659],
-          [ 2.6541,  2.2315,  2.2137,  2.1956],
-          [ 1.2810,  1.5202,  1.4746,  1.4015]],
-
-         [[ 1.2734,  1.0669,  1.8976,  1.4618],
-          [ 1.3759,  1.9641,  2.0386,  1.6985],
-          [ 2.6541,  2.2315,  2.3261,  2.3353],
-          [ 1.2810,  1.5202,  1.4438,  1.3397]]],
-
-
-        [[[-0.1810,  0.1306, -0.3701, -0.3862],
-          [ 0.6150,  0.6773,  0.3873,  0.0967],
-          [ 0.6275,  0.7061,  0.8506,  0.7424],
-          [-0.3612, -0.1324,  0.0046, -0.3171]],
-
-         [[-0.1810,  0.1306, -0.2361,  0.0192],
-          [ 0.6150,  0.6773,  0.5791,  0.2294],
-          [ 0.6275,  0.7061,  0.9629,  0.8821],
-          [-0.3612, -0.1324, -0.0261, -0.3790]]]], 4)
-
-	assert_array_almost_equal(y_after[1][:2, :4], [
-		[[ 0.1324,  0.3553,  0.1465],
-         [ 0.2455,  0.3811,  0.1003],
-         [ 0.1798,  0.2700,  0.1818],
-         [ 0.1989,  0.2952,  0.0110]],
-
-        [[-0.1501, -0.0500, -0.0986],
-         [-0.0370, -0.0243, -0.1448],
-         [-0.1027, -0.1353, -0.0634],
-         [-0.0835, -0.1101, -0.2342]]], 4)
 
+def test_space_raises_args(X, alpha, beta):
+	torch.manual_seed(0)
+	model = FlattenDense()
+	assert_raises(ValueError, space, model, X, ["ACGTC", "ACC"], [0, 1], 
+		batch_size=2, device='cpu')
+	assert_raises(ValueError, space, model, X, ["ACGTC", "ACC"], [-5], 
+		batch_size=2, device='cpu')
+	assert_raises(ValueError, space, model, X, ["ACGTC", "ACC"], -3, 
+		batch_size=2, device='cpu')
+	assert_raises(ValueError, space, model, X, ["ACGTC", "ACC"], [], 
+		batch_size=2, device='cpu')
+	assert_raises(ValueError, space, model, X, ["ACGTC", "ACC"], [1500], 
+		batch_size=2, device='cpu')
+
+	assert_raises(TypeError, space, model, X, ["ACGTC", "ACC"], 0, 
+		batch_size=2, args=5, device='cpu')
+	assert_raises(TypeError, space, model, X, ["ACGTC", "ACC"], 0, 
+		batch_size=2, args=(5,), device='cpu')
+	assert_raises(TypeError, space, model, X, ["ACGTC", "ACC"], 0, 
+		batch_size=2, args=alpha, device='cpu')
+	assert_raises(RuntimeError, space, model, X, ["ACGTC", "ACC"], 0,
+		batch_size=2, args=(alpha[:5],), device='cpu')
+	assert_raises(RuntimeError, space, model, X, ["ACGTC", "ACC"], 0, 
+		batch_size=2, args=(alpha, beta[:5]), device='cpu')
 
-def test_ablate_convdense_batch_size(X, alpha):
+
+###
+
+
+def test_space_cross_flattendense_alpha(X, alpha, beta):
 	torch.manual_seed(0)
-	model = ConvDense()
-	y_before0, y_after0 = ablate(model, X, 46, 54, random_state=0, 
-		args=(alpha[:, :, None],), batch_size=1, device='cpu')
+	model = FlattenDense()
+	y0_before, y0_after = space(model, X, ['ACGTGC', 'TGTT'], 3, 
+		device='cpu')
+	y_before, y_after = space_cross(model, X, ['ACGTGC', 'TGTT'], 3, 
+		(alpha[:5],), device='cpu')
 
-	y_before1, y_after1 = ablate(model, X, 46, 54, random_state=0, 
-		args=(alpha[:, :, None],), batch_size=5, device='cpu')
+	assert y_before.shape == (64, 5, 3)
+	assert y_before.dtype == torch.float32
+	assert_array_almost_equal(y_before, y0_before[:, None] + alpha[:5][None, :])
+	assert_array_almost_equal(y_before[:2], [
+		[[1.9569, 2.0429, 1.6640],
+         [0.5930, 0.6790, 0.3001],
+         [1.1715, 1.2575, 0.8787],
+         [2.4337, 2.5197, 2.1409],
+         [2.0604, 2.1464, 1.7675]],
+
+        [[1.7136, 1.7814, 1.5889],
+         [0.3497, 0.4175, 0.2250],
+         [0.9283, 0.9961, 0.8036],
+         [2.1904, 2.2583, 2.0658],
+         [1.8171, 1.8849, 1.6924]]], 4)
 
-	y_before2, y_after2 = ablate(model, X, 46, 54, random_state=0, 
-		args=(alpha[:, :, None],), batch_size=68, device='cpu')
 
-	assert len(y_before0) == len(y_before1) == len(y_before2) == 2
-	assert len(y_after0) == len(y_after1) == len(y_after2) == 2
-	
-	assert y_before0[0].shape == (64, 12, 98)
-	assert y_before0[1].shape == (64, 3)
+	assert y_after.shape == (64, 5, 3)
+	assert y_after.dtype == torch.float32
+	assert_array_almost_equal(y_after, y0_after[:, None] + alpha[:5][None, :])
+	assert_array_almost_equal(y_after[:2], [
+		[[1.9143, 1.9713, 1.6641],
+         [0.5504, 0.6074, 0.3002],
+         [1.1290, 1.1860, 0.8788],
+         [2.3912, 2.4481, 2.1409],
+         [2.0178, 2.0748, 1.7676]],
+
+        [[1.7369, 1.6794, 1.6200],
+         [0.3730, 0.3156, 0.2561],
+         [0.9516, 0.8941, 0.8347],
+         [2.2137, 2.1563, 2.0968],
+         [1.8404, 1.7830, 1.7235]]], 4)
 
-	assert y_before1[0].shape == (64, 12, 98)
-	assert y_before1[1].shape == (64, 3)
 
-	assert y_before2[0].shape == (64, 12, 98)
-	assert y_before2[1].shape == (64, 3)
 
-	assert y_after0[0].shape == (64, 20, 12, 98)
-	assert y_after0[1].shape == (64, 20, 3)
+def test_space_cross_flattendense_beta(X, alpha, beta):
+	torch.manual_seed(0)
+	model = FlattenDense()
+	alpha = torch.zeros(X.shape[0], 1)
 
-	assert y_after1[0].shape == (64, 20, 12, 98)
-	assert y_after1[1].shape == (64, 20, 3)
+	y0_before, y0_after = space(model, X, ['ACGTGC', 'TGTT'], 3, 
+		device='cpu')
+	y_before, y_after = space_cross(model, X, ['ACGTGC', 'TGTT'], 3, 
+		(alpha[:5], beta[:5]), device='cpu')
 
-	assert y_after2[0].shape == (64, 20, 12, 98)
-	assert y_after2[1].shape == (64, 20, 3)
+	assert y_before.shape == (64, 5, 3)
+	assert y_before.dtype == torch.float32
+	assert_array_almost_equal(y_before, y0_before[:, None] * beta[:5][None, :])
+	assert_array_almost_equal(y_before[:2], [
+		[[ 0.3132,  0.4529, -0.1624],
+         [-0.1179, -0.1706,  0.0612],
+         [-0.1018, -0.1473,  0.0528],
+         [-0.2069, -0.2991,  0.1073],
+         [ 0.1669,  0.2413, -0.0865]],
+
+        [[-0.0820,  0.0282, -0.2845],
+         [ 0.0309, -0.0106,  0.1071],
+         [ 0.0267, -0.0092,  0.0925],
+         [ 0.0542, -0.0186,  0.1879],
+         [-0.0437,  0.0150, -0.1516]]], 4)
 
-	assert_array_almost_equal(y_before0[0], y_before1[0])
-	assert_array_almost_equal(y_before0[0], y_before2[0])
+	assert y_after.shape == (64, 5, 3)
+	assert y_after.dtype == torch.float32
+	assert_array_almost_equal(y_after, y0_after[:, None] * beta[:5][None, :])
+	assert_array_almost_equal(y_after[:2], [
+		[[ 0.2441,  0.3366, -0.1624],
+         [-0.0919, -0.1268,  0.0612],
+         [-0.0794, -0.1095,  0.0528],
+         [-0.1613, -0.2224,  0.1073],
+         [ 0.1301,  0.1793, -0.0865]],
+
+        [[-0.0441, -0.1374, -0.2340],
+         [ 0.0166,  0.0518,  0.0881],
+         [ 0.0143,  0.0447,  0.0761],
+         [ 0.0291,  0.0908,  0.1546],
+         [-0.0235, -0.0732, -0.1247]]], 4)
 
-	assert_array_almost_equal(y_before0[1], y_before1[1])
-	assert_array_almost_equal(y_before0[1], y_before2[1])
 
-	assert_array_almost_equal(y_after0[0], y_after1[0])
-	assert_array_almost_equal(y_after0[0], y_after2[0])
+def test_space_cross_flattendense_alpha_beta(X, alpha, beta):
+	torch.manual_seed(0)
+	model = FlattenDense()
+	y0_before, y0_after = space(model, X, ['ACGTGC', 'TGTT'], 3, 
+		device='cpu')
+	y_before, y_after = space_cross(model, X, ['ACGTGC', 'TGTT'], 3, 
+		(alpha[:5], beta[:5]), device='cpu')
 
-	assert_array_almost_equal(y_after0[1], y_after1[1])
-	assert_array_almost_equal(y_after0[1], y_after2[1])
+	assert y_before.shape == (64, 5, 3)
+	assert y_before.dtype == torch.float32
+	assert_array_almost_equal(y_before, y0_before[:, None] * beta[:5][None, :]
+		+ alpha[:5][None, :])
+	assert_array_almost_equal(y_before[:2], [
+		[[2.0772, 2.2169, 1.6016],
+         [0.2822, 0.2296, 0.4613],
+         [0.8769, 0.8315, 1.0316],
+         [2.0340, 1.9417, 2.3482],
+         [2.0344, 2.1088, 1.7810]],
+
+        [[1.6821, 1.7923, 1.4796],
+         [0.4310, 0.3895, 0.5073],
+         [1.0054, 0.9696, 1.0712],
+         [2.2951, 2.2223, 2.4288],
+         [1.8239, 1.8826, 1.7160]]], 4)
+
+	assert y_after.shape == (64, 5, 3)
+	assert y_after.dtype == torch.float32
+	assert_array_almost_equal(y_after, y0_after[:, None] * beta[:5][None, :]
+		+ alpha[:5][None, :])
+	assert_array_almost_equal(y_after[:2], [
+		[[2.0082, 2.1007, 1.6017],
+         [0.3082, 0.2734, 0.4613],
+         [0.8994, 0.8693, 1.0315],
+         [2.0796, 2.0185, 2.3482],
+         [1.9976, 2.0469, 1.7810]],
+
+        [[1.7199, 1.6266, 1.5301],
+         [0.4168, 0.4519, 0.4883],
+         [0.9931, 1.0234, 1.0548],
+         [2.2700, 2.3317, 2.3955],
+         [1.8441, 1.7943, 1.7429]]], 4)
 
 
-def test_ablate_raises_shape(X, alpha):
+def test_space_cross_convdense_alpha(X, alpha):
 	torch.manual_seed(0)
 	model = ConvDense()
+	y_before, y_after = space_cross(model, X, ["ACGTGC", "TGGTT"], 3, 
+		start=0, args=(alpha[:5, :, None],), batch_size=2, device='cpu')
 
-	assert_raises(ValueError, ablate, model, X[0], 46, 54, device='cpu')
-	assert_raises(ValueError, ablate, model, X[:, 0], 46, 54, device='cpu')
-	assert_raises(ValueError, ablate, model, X.unsqueeze(0), 46, 54, 
-		device='cpu')
+	assert len(y_before) == 2
+	assert y_before[0].shape == (64, 5, 12, 98)
+	assert y_before[1].shape == (64, 5, 3)
 
-	assert_raises(ValueError, ablate, model, X, 46, 54, args=(alpha[:2],), 
-		device='cpu')
-	assert_raises(ValueError, ablate, model, X, 46, 54, args=alpha, 
-		device='cpu')
-	assert_raises(ValueError, ablate, model, X, 46, 54, args=(alpha[:2, None],),
-		device='cpu')
+	assert y_before[0].dtype == torch.float32
+	assert y_before[1].dtype == torch.float32
 
+	assert_array_almost_equal(y_before[0][:2, :2, :3, :4], [
+		[[[ 0.9883,  1.8037,  0.8841,  0.7446],
+          [ 1.8588,  1.9683,  1.5339,  1.4497],
+          [ 2.1421,  2.2650,  2.6226,  2.4379]],
+
+         [[-0.3756,  0.4398, -0.4798, -0.6192],
+          [ 0.4949,  0.6044,  0.1700,  0.0858],
+          [ 0.7782,  0.9011,  1.2587,  1.0740]]],
+
+
+        [[[ 1.0964,  0.8767,  0.8945,  1.2957],
+          [ 1.6873,  1.7551,  1.7884,  1.8996],
+          [ 2.2469,  2.3060,  2.0810,  2.0929]],
+
+         [[-0.2675, -0.4872, -0.4694, -0.0682],
+          [ 0.3234,  0.3912,  0.4245,  0.5357],
+          [ 0.8830,  0.9421,  0.7171,  0.7290]]]], 4)
 
-def test_ablate_raises_args(X, alpha, beta):
-	torch.manual_seed(0)
-	model = FlattenDense()
+	assert_array_almost_equal(y_before[1][:4], [
+		[[ 0.1928,  0.2788, -0.1000],
+         [ 0.1928,  0.2788, -0.1000],
+         [ 0.1928,  0.2788, -0.1000],
+         [ 0.1928,  0.2788, -0.1000],
+         [ 0.1928,  0.2788, -0.1000]],
+
+        [[-0.0505,  0.0174, -0.1751],
+         [-0.0505,  0.0174, -0.1751],
+         [-0.0505,  0.0174, -0.1751],
+         [-0.0505,  0.0174, -0.1751],
+         [-0.0505,  0.0174, -0.1751]],
+
+        [[-0.1408,  0.0105,  0.0673],
+         [-0.1408,  0.0105,  0.0673],
+         [-0.1408,  0.0105,  0.0673],
+         [-0.1408,  0.0105,  0.0673],
+         [-0.1408,  0.0105,  0.0673]],
+
+        [[-0.2375, -0.0069,  0.0835],
+         [-0.2375, -0.0069,  0.0835],
+         [-0.2375, -0.0069,  0.0835],
+         [-0.2375, -0.0069,  0.0835],
+         [-0.2375, -0.0069,  0.0835]]], 4)
 
-	assert_raises(ValueError, ablate, model, X, -6, 5, device='cpu')
-	assert_raises(ValueError, ablate, model, X, 7, 5, device='cpu')
-	assert_raises(ValueError, ablate, model, X, 7, 5000, device='cpu')
-	assert_raises(ValueError, ablate, model, X, 5, 10, args=alpha, device='cpu')
-	assert_raises(ValueError, ablate, model, X, 5, 10, args=(alpha[:5],), 
-		device='cpu')
-	assert_raises(ValueError, ablate, model, X, 5, 10, args=(alpha, beta[:5]), 
-		device='cpu')
+	assert len(y_after) == 2
+	assert y_after[0].shape == (64, 5, 12, 98)
+	assert y_after[1].shape == (64, 5, 3)
+
+	assert y_after[0].dtype == torch.float32
+	assert y_after[1].dtype == torch.float32
+
+	assert_array_almost_equal(y_after[0][:2, :2, :3, :4], [
+		[[[ 1.3831,  0.9466,  0.9256,  1.4921],
+          [ 1.5933,  1.3485,  1.9935,  1.9060],
+          [ 2.2460,  2.6037,  1.8025,  2.1864]],
+
+         [[ 0.0192, -0.4173, -0.4383,  0.1282],
+          [ 0.2294, -0.0154,  0.6296,  0.5421],
+          [ 0.8821,  1.2398,  0.4386,  0.8225]]],
+
+
+        [[[ 1.3831,  0.9466,  0.9256,  1.4921],
+          [ 1.5933,  1.3485,  1.9935,  1.9060],
+          [ 2.2460,  2.6037,  1.8025,  2.1864]],
+
+         [[ 0.0192, -0.4173, -0.4383,  0.1282],
+          [ 0.2294, -0.0154,  0.6296,  0.5421],
+          [ 0.8821,  1.2398,  0.4386,  0.8225]]]], 4)
+
+	assert_array_almost_equal(y_after[1][:4], [
+		[[ 0.3324,  0.1149, -0.0712],
+         [ 0.3324,  0.1149, -0.0712],
+         [ 0.3324,  0.1149, -0.0712],
+         [ 0.3324,  0.1149, -0.0712],
+         [ 0.3324,  0.1149, -0.0712]],
+
+        [[-0.0377, -0.0666, -0.1223],
+         [-0.0377, -0.0666, -0.1223],
+         [-0.0377, -0.0666, -0.1223],
+         [-0.0377, -0.0666, -0.1223],
+         [-0.0377, -0.0666, -0.1223]],
+
+        [[-0.0393, -0.0238,  0.2462],
+         [-0.0393, -0.0238,  0.2462],
+         [-0.0393, -0.0238,  0.2462],
+         [-0.0393, -0.0238,  0.2462],
+         [-0.0393, -0.0238,  0.2462]],
+
+        [[-0.1770, -0.0393,  0.1683],
+         [-0.1770, -0.0393,  0.1683],
+         [-0.1770, -0.0393,  0.1683],
+         [-0.1770, -0.0393,  0.1683],
+         [-0.1770, -0.0393,  0.1683]]], 4)
```

### Comparing `tangermeme-0.1.0/tests/test_ersatz.py` & `tangermeme-0.1.0rc0/tests/test_ersatz.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.1.0/tests/test_io.py` & `tangermeme-0.1.0rc0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.1.0/tests/test_ism.py` & `tangermeme-0.1.0rc0/tests/test_ism.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.1.0/tests/test_kmers.py` & `tangermeme-0.1.0rc0/tests/test_kmers.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.1.0/tests/test_marginalize.py` & `tangermeme-0.1.0rc0/tests/test_marginalize.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import torch
 import pytest
 
 from tangermeme.utils import one_hot_encode
 from tangermeme.utils import random_one_hot
 
 from tangermeme.marginalize import marginalize
+from tangermeme.marginalize import marginalize_cross
 
 from .toy_models import SumModel
 from .toy_models import FlattenDense
 from .toy_models import Conv
 from .toy_models import Scatter
 from .toy_models import ConvDense
 
@@ -332,15 +333,250 @@
 
 
 def test_marginalize_raises_args(X, alpha, beta):
 	torch.manual_seed(0)
 	model = FlattenDense()
 	assert_raises(TypeError, marginalize, model, X, "ACGTC", batch_size=2, 
 		args=5, device='cpu')
-	assert_raises(AttributeError, marginalize, model, X, "ACGTC",  batch_size=2, 
+	assert_raises(TypeError, marginalize, model, X, "ACGTC",  batch_size=2, 
 		args=(5,), device='cpu')
-	assert_raises(ValueError, marginalize, model, X, "ACGTC", batch_size=2, 
+	assert_raises(TypeError, marginalize, model, X, "ACGTC", batch_size=2, 
 		args=alpha, device='cpu')
-	assert_raises(ValueError, marginalize, model, X, "ACGTC", batch_size=2, 
+	assert_raises(RuntimeError, marginalize, model, X, "ACGTC", batch_size=2, 
 		args=(alpha[:5],), device='cpu')
-	assert_raises(ValueError, marginalize, model, X, "ACGTC", batch_size=2, 
+	assert_raises(RuntimeError, marginalize, model, X, "ACGTC", batch_size=2, 
 		args=(alpha, beta[:5]), device='cpu')
+
+
+###
+
+
+def test_marginalize_cross_flattendense_alpha(X, alpha, beta):
+	torch.manual_seed(0)
+	model = FlattenDense()
+	y0_before, y0_after = marginalize(model, X, 'ACGTGC', device='cpu')
+	y_before, y_after = marginalize_cross(model, X, 'ACGTGC', (alpha[:5],), 
+		device='cpu')
+
+	assert y_before.shape == (64, 5, 3)
+	assert y_before.dtype == torch.float32
+	assert_array_almost_equal(y_before, y0_before[:, None] + alpha[:5][None, :])
+	assert_array_almost_equal(y_before[:2], [
+		[[1.9569, 2.0429, 1.6640],
+         [0.5930, 0.6790, 0.3001],
+         [1.1715, 1.2575, 0.8787],
+         [2.4337, 2.5197, 2.1409],
+         [2.0604, 2.1464, 1.7675]],
+
+        [[1.7136, 1.7814, 1.5889],
+         [0.3497, 0.4175, 0.2250],
+         [0.9283, 0.9961, 0.8036],
+         [2.1904, 2.2583, 2.0658],
+         [1.8171, 1.8849, 1.6924]]], 4)
+
+	assert y_after.shape == (64, 5, 3)
+	assert y_after.dtype == torch.float32
+	assert_array_almost_equal(y_after, y0_after[:, None] + alpha[:5][None, :])
+	assert_array_almost_equal(y_after[:2], [
+		[[1.9098, 2.0546, 1.9081],
+         [0.5459, 0.6907, 0.5442],
+         [1.1245, 1.2693, 1.1228],
+         [2.3867, 2.5314, 2.3850],
+         [2.0133, 2.1581, 2.0116]],
+
+        [[1.6194, 1.7230, 1.7036],
+         [0.2555, 0.3591, 0.3397],
+         [0.8341, 0.9377, 0.9183],
+         [2.0962, 2.1999, 2.1805],
+         [1.7229, 1.8265, 1.8071]]], 4)
+
+
+
+def test_marginalize_cross_flattendense_beta(X, alpha, beta):
+	torch.manual_seed(0)
+	model = FlattenDense()
+	alpha = torch.zeros(X.shape[0], 1)
+
+	y0_before, y0_after = marginalize(model, X, 'ACGTGC', device='cpu')
+	y_before, y_after = marginalize_cross(model, X, 'ACGTGC', (alpha[:5], 
+		beta[:5]), device='cpu')
+
+	assert y_before.shape == (64, 5, 3)
+	assert y_before.dtype == torch.float32
+	assert_array_almost_equal(y_before, y0_before[:, None] * beta[:5][None, :])
+	assert_array_almost_equal(y_before[:2], [
+		[[ 0.3132,  0.4529, -0.1624],
+         [-0.1179, -0.1706,  0.0612],
+         [-0.1018, -0.1473,  0.0528],
+         [-0.2069, -0.2991,  0.1073],
+         [ 0.1669,  0.2413, -0.0865]],
+
+        [[-0.0820,  0.0282, -0.2845],
+         [ 0.0309, -0.0106,  0.1071],
+         [ 0.0267, -0.0092,  0.0925],
+         [ 0.0542, -0.0186,  0.1879],
+         [-0.0437,  0.0150, -0.1516]]], 4)
+
+	assert y_after.shape == (64, 5, 3)
+	assert y_after.dtype == torch.float32
+	assert_array_almost_equal(y_after, y0_after[:, None] * beta[:5][None, :])
+	assert_array_almost_equal(y_after[:2], [
+		[[ 0.2368,  0.4720,  0.2340],
+         [-0.0892, -0.1777, -0.0881],
+         [-0.0770, -0.1535, -0.0761],
+         [-0.1564, -0.3118, -0.1546],
+         [ 0.1262,  0.2514,  0.1247]],
+
+        [[-0.2350, -0.0666, -0.0981],
+         [ 0.0885,  0.0251,  0.0370],
+         [ 0.0764,  0.0217,  0.0319],
+         [ 0.1552,  0.0440,  0.0648],
+         [-0.1252, -0.0355, -0.0523]]], 4)
+
+
+def test_marginalize_cross_flattendense_alpha_beta(X, alpha, beta):
+	torch.manual_seed(0)
+	model = FlattenDense()
+	y0_before, y0_after = marginalize(model, X, 'ACGTGC', device='cpu')
+	y_before, y_after = marginalize_cross(model, X, 'ACGTGC', (alpha[:5], 
+		beta[:5]), device='cpu')
+
+	assert y_before.shape == (64, 5, 3)
+	assert y_before.dtype == torch.float32
+	assert_array_almost_equal(y_before, y0_before[:, None] * beta[:5][None, :]
+		+ alpha[:5][None, :])
+	assert_array_almost_equal(y_before[:2], [
+		[[2.0772, 2.2169, 1.6016],
+         [0.2822, 0.2296, 0.4613],
+         [0.8769, 0.8315, 1.0316],
+         [2.0340, 1.9417, 2.3482],
+         [2.0344, 2.1088, 1.7810]],
+
+        [[1.6821, 1.7923, 1.4796],
+         [0.4310, 0.3895, 0.5073],
+         [1.0054, 0.9696, 1.0712],
+         [2.2951, 2.2223, 2.4288],
+         [1.8239, 1.8826, 1.7160]]], 4)
+
+	assert y_after.shape == (64, 5, 3)
+	assert y_after.dtype == torch.float32
+	assert_array_almost_equal(y_after, y0_after[:, None] * beta[:5][None, :]
+		+ alpha[:5][None, :])
+	assert_array_almost_equal(y_after[:2], [
+		[[2.0008, 2.2360, 1.9981],
+         [0.3110, 0.2224, 0.3120],
+         [0.9017, 0.8253, 0.9026],
+         [2.0845, 1.9291, 2.0863],
+         [1.9937, 2.1190, 1.9922]],
+
+        [[1.5291, 1.6974, 1.6659],
+         [0.4887, 0.4252, 0.4371],
+         [1.0552, 1.0004, 1.0106],
+         [2.3961, 2.2849, 2.3057],
+         [1.7424, 1.8321, 1.8153]]], 4)
+
+
+def test_marginalize_cross_convdense_alpha(X, alpha):
+	torch.manual_seed(0)
+	model = ConvDense()
+	y_before, y_after = marginalize_cross(model, X, "ACGTGC", start=0, 
+		args=(alpha[:5, :, None],), batch_size=2, device='cpu')
+
+	assert len(y_before) == 2
+	assert y_before[0].shape == (64, 5, 12, 98)
+	assert y_before[1].shape == (64, 5, 3)
+
+	assert y_before[0].dtype == torch.float32
+	assert y_before[1].dtype == torch.float32
+
+	assert_array_almost_equal(y_before[0][:2, :2, :3, :4], [
+		[[[ 0.9883,  1.8037,  0.8841,  0.7446],
+          [ 1.8588,  1.9683,  1.5339,  1.4497],
+          [ 2.1421,  2.2650,  2.6226,  2.4379]],
+
+         [[-0.3756,  0.4398, -0.4798, -0.6192],
+          [ 0.4949,  0.6044,  0.1700,  0.0858],
+          [ 0.7782,  0.9011,  1.2587,  1.0740]]],
+
+
+        [[[ 1.0964,  0.8767,  0.8945,  1.2957],
+          [ 1.6873,  1.7551,  1.7884,  1.8996],
+          [ 2.2469,  2.3060,  2.0810,  2.0929]],
+
+         [[-0.2675, -0.4872, -0.4694, -0.0682],
+          [ 0.3234,  0.3912,  0.4245,  0.5357],
+          [ 0.8830,  0.9421,  0.7171,  0.7290]]]], 4)
+
+	assert_array_almost_equal(y_before[1][:4], [
+		[[ 0.1928,  0.2788, -0.1000],
+         [ 0.1928,  0.2788, -0.1000],
+         [ 0.1928,  0.2788, -0.1000],
+         [ 0.1928,  0.2788, -0.1000],
+         [ 0.1928,  0.2788, -0.1000]],
+
+        [[-0.0505,  0.0174, -0.1751],
+         [-0.0505,  0.0174, -0.1751],
+         [-0.0505,  0.0174, -0.1751],
+         [-0.0505,  0.0174, -0.1751],
+         [-0.0505,  0.0174, -0.1751]],
+
+        [[-0.1408,  0.0105,  0.0673],
+         [-0.1408,  0.0105,  0.0673],
+         [-0.1408,  0.0105,  0.0673],
+         [-0.1408,  0.0105,  0.0673],
+         [-0.1408,  0.0105,  0.0673]],
+
+        [[-0.2375, -0.0069,  0.0835],
+         [-0.2375, -0.0069,  0.0835],
+         [-0.2375, -0.0069,  0.0835],
+         [-0.2375, -0.0069,  0.0835],
+         [-0.2375, -0.0069,  0.0835]]], 4)
+
+	assert len(y_after) == 2
+	assert y_after[0].shape == (64, 5, 12, 98)
+	assert y_after[1].shape == (64, 5, 3)
+
+	assert y_after[0].dtype == torch.float32
+	assert y_after[1].dtype == torch.float32
+
+	assert_array_almost_equal(y_after[0][:2, :2, :3, :4], [
+		[[[ 1.3831,  0.9466,  0.9256,  1.4921],
+          [ 1.5933,  1.3485,  1.9935,  1.9060],
+          [ 2.2460,  2.6037,  1.8025,  2.1864]],
+
+         [[ 0.0192, -0.4173, -0.4383,  0.1282],
+          [ 0.2294, -0.0154,  0.6296,  0.5421],
+          [ 0.8821,  1.2398,  0.4386,  0.8225]]],
+
+
+        [[[ 1.3831,  0.9466,  0.9256,  1.4921],
+          [ 1.5933,  1.3485,  1.9935,  1.9060],
+          [ 2.2460,  2.6037,  1.8025,  2.1864]],
+
+         [[ 0.0192, -0.4173, -0.4383,  0.1282],
+          [ 0.2294, -0.0154,  0.6296,  0.5421],
+          [ 0.8821,  1.2398,  0.4386,  0.8225]]]], 4)
+
+	assert_array_almost_equal(y_after[1][:4], [
+		[[ 0.2472,  0.1913, -0.0212],
+         [ 0.2472,  0.1913, -0.0212],
+         [ 0.2472,  0.1913, -0.0212],
+         [ 0.2472,  0.1913, -0.0212],
+         [ 0.2472,  0.1913, -0.0212]],
+
+        [[-0.1387,  0.0929, -0.1931],
+         [-0.1387,  0.0929, -0.1931],
+         [-0.1387,  0.0929, -0.1931],
+         [-0.1387,  0.0929, -0.1931],
+         [-0.1387,  0.0929, -0.1931]],
+
+        [[-0.1165,  0.0957,  0.1448],
+         [-0.1165,  0.0957,  0.1448],
+         [-0.1165,  0.0957,  0.1448],
+         [-0.1165,  0.0957,  0.1448],
+         [-0.1165,  0.0957,  0.1448]],
+
+        [[-0.2053,  0.0571,  0.1370],
+         [-0.2053,  0.0571,  0.1370],
+         [-0.2053,  0.0571,  0.1370],
+         [-0.2053,  0.0571,  0.1370],
+         [-0.2053,  0.0571,  0.1370]]], 4)
```

### Comparing `tangermeme-0.1.0/tests/test_match.py` & `tangermeme-0.1.0rc0/tests/test_match.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.1.0/tests/test_utils.py` & `tangermeme-0.1.0rc0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.1.0/tests/test_variant_effect.py` & `tangermeme-0.1.0rc0/tests/test_variant_effect.py`

 * *Files identical despite different names*

