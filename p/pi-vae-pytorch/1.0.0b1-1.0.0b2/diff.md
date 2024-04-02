# Comparing `tmp/pi-vae-pytorch-1.0.0b1.tar.gz` & `tmp/pi-vae-pytorch-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pi-vae-pytorch-1.0.0b1.tar", last modified: Tue Apr  2 04:42:04 2024, max compression
+gzip compressed data, was "pi-vae-pytorch-1.0.0b2.tar", last modified: Tue Apr  2 07:25:47 2024, max compression
```

## Comparing `pi-vae-pytorch-1.0.0b1.tar` & `pi-vae-pytorch-1.0.0b2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:42:04.173883 pi-vae-pytorch-1.0.0b1/
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-02 04:41:54.000000 pi-vae-pytorch-1.0.0b1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-02 04:41:54.000000 pi-vae-pytorch-1.0.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-02 04:41:54.000000 pi-vae-pytorch-1.0.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-04-02 04:42:04.173883 pi-vae-pytorch-1.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-04-02 04:41:54.000000 pi-vae-pytorch-1.0.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:42:04.173883 pi-vae-pytorch-1.0.0b1/pi_vae_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-02 04:41:54.000000 pi-vae-pytorch-1.0.0b1/pi_vae_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-02 04:41:54.000000 pi-vae-pytorch-1.0.0b1/pi_vae_pytorch/decoders.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1296 2024-04-02 04:41:54.000000 pi-vae-pytorch-1.0.0b1/pi_vae_pytorch/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)    10690 2024-04-02 04:41:54.000000 pi-vae-pytorch-1.0.0b1/pi_vae_pytorch/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-04-02 04:41:54.000000 pi-vae-pytorch-1.0.0b1/pi_vae_pytorch/pivae.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5270 2024-04-02 04:41:54.000000 pi-vae-pytorch-1.0.0b1/pi_vae_pytorch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:42:04.173883 pi-vae-pytorch-1.0.0b1/pi_vae_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-04-02 04:42:04.000000 pi-vae-pytorch-1.0.0b1/pi_vae_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-02 04:42:04.000000 pi-vae-pytorch-1.0.0b1/pi_vae_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 04:42:04.000000 pi-vae-pytorch-1.0.0b1/pi_vae_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 04:42:04.000000 pi-vae-pytorch-1.0.0b1/pi_vae_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-02 04:42:04.000000 pi-vae-pytorch-1.0.0b1/pi_vae_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-02 04:41:54.000000 pi-vae-pytorch-1.0.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 04:42:04.173883 pi-vae-pytorch-1.0.0b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:25:47.764736 pi-vae-pytorch-1.0.0b2/
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-02 07:25:43.000000 pi-vae-pytorch-1.0.0b2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-02 07:25:43.000000 pi-vae-pytorch-1.0.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-02 07:25:43.000000 pi-vae-pytorch-1.0.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-04-02 07:25:47.764736 pi-vae-pytorch-1.0.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-04-02 07:25:43.000000 pi-vae-pytorch-1.0.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:25:47.760736 pi-vae-pytorch-1.0.0b2/pi_vae_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-02 07:25:43.000000 pi-vae-pytorch-1.0.0b2/pi_vae_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-02 07:25:43.000000 pi-vae-pytorch-1.0.0b2/pi_vae_pytorch/decoders.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1296 2024-04-02 07:25:43.000000 pi-vae-pytorch-1.0.0b2/pi_vae_pytorch/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10690 2024-04-02 07:25:43.000000 pi-vae-pytorch-1.0.0b2/pi_vae_pytorch/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-04-02 07:25:43.000000 pi-vae-pytorch-1.0.0b2/pi_vae_pytorch/pivae.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5270 2024-04-02 07:25:43.000000 pi-vae-pytorch-1.0.0b2/pi_vae_pytorch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:25:47.764736 pi-vae-pytorch-1.0.0b2/pi_vae_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-04-02 07:25:47.000000 pi-vae-pytorch-1.0.0b2/pi_vae_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-02 07:25:47.000000 pi-vae-pytorch-1.0.0b2/pi_vae_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 07:25:47.000000 pi-vae-pytorch-1.0.0b2/pi_vae_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 07:25:47.000000 pi-vae-pytorch-1.0.0b2/pi_vae_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-02 07:25:47.000000 pi-vae-pytorch-1.0.0b2/pi_vae_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-02 07:25:43.000000 pi-vae-pytorch-1.0.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 07:25:47.764736 pi-vae-pytorch-1.0.0b2/setup.cfg
```

### Comparing `pi-vae-pytorch-1.0.0b1/.gitignore` & `pi-vae-pytorch-1.0.0b2/.gitignore`

 * *Files identical despite different names*

### Comparing `pi-vae-pytorch-1.0.0b1/PKG-INFO` & `pi-vae-pytorch-1.0.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pi-vae-pytorch
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: A Pytorch implementation of Poisson Identifiable VAE (pi-VAE), a variational auto encoder used to construct latent variable models of neural activity while simultaneously modeling the relation between the latent and task variables.
 Author-email: Marlan McInnes-Taylor <mmcinnestaylor@gmail.com>
-Maintainer-email: Marlan McInnes-Taylor <mmcinnestaylor@gmail.com>
-Project-URL: Homepage, https://mmcinnestaylor.github.io/pi-vae-pytorch/
-Project-URL: Repository, https://github.com/mmcinnestaylor/pi-vae-pytorch
+Maintainer-email: B-B-C Lab <weixx@utexas.edu>
+Project-URL: Homepage, https://wei-bbc-lab.github.io/pi-vae-pytorch/
+Project-URL: Repository, https://github.com/wei-bbc-lab/pi-vae-pytorch
 Keywords: vae,pi-vae,poisson identifiable vae,poisson identifiable variational autoencoder,identifiable vae,identifiable variational autoencoder
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.9
```

### Comparing `pi-vae-pytorch-1.0.0b1/README.md` & `pi-vae-pytorch-1.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `pi-vae-pytorch-1.0.0b1/pi_vae_pytorch/decoders.py` & `pi-vae-pytorch-1.0.0b2/pi_vae_pytorch/decoders.py`

 * *Files identical despite different names*

### Comparing `pi-vae-pytorch-1.0.0b1/pi_vae_pytorch/encoders.py` & `pi-vae-pytorch-1.0.0b2/pi_vae_pytorch/encoders.py`

 * *Files identical despite different names*

### Comparing `pi-vae-pytorch-1.0.0b1/pi_vae_pytorch/layers.py` & `pi-vae-pytorch-1.0.0b2/pi_vae_pytorch/layers.py`

 * *Files identical despite different names*

### Comparing `pi-vae-pytorch-1.0.0b1/pi_vae_pytorch/pivae.py` & `pi-vae-pytorch-1.0.0b2/pi_vae_pytorch/pivae.py`

 * *Files identical despite different names*

### Comparing `pi-vae-pytorch-1.0.0b1/pi_vae_pytorch/utils.py` & `pi-vae-pytorch-1.0.0b2/pi_vae_pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `pi-vae-pytorch-1.0.0b1/pi_vae_pytorch.egg-info/PKG-INFO` & `pi-vae-pytorch-1.0.0b2/pi_vae_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pi-vae-pytorch
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: A Pytorch implementation of Poisson Identifiable VAE (pi-VAE), a variational auto encoder used to construct latent variable models of neural activity while simultaneously modeling the relation between the latent and task variables.
 Author-email: Marlan McInnes-Taylor <mmcinnestaylor@gmail.com>
-Maintainer-email: Marlan McInnes-Taylor <mmcinnestaylor@gmail.com>
-Project-URL: Homepage, https://mmcinnestaylor.github.io/pi-vae-pytorch/
-Project-URL: Repository, https://github.com/mmcinnestaylor/pi-vae-pytorch
+Maintainer-email: B-B-C Lab <weixx@utexas.edu>
+Project-URL: Homepage, https://wei-bbc-lab.github.io/pi-vae-pytorch/
+Project-URL: Repository, https://github.com/wei-bbc-lab/pi-vae-pytorch
 Keywords: vae,pi-vae,poisson identifiable vae,poisson identifiable variational autoencoder,identifiable vae,identifiable variational autoencoder
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.9
```

### Comparing `pi-vae-pytorch-1.0.0b1/pyproject.toml` & `pi-vae-pytorch-1.0.0b2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -6,37 +6,37 @@
 name = "pi-vae-pytorch"
 dependencies = ["pytorch"]
 requires-python = ">= 3.9"
 authors = [
     {name = "Marlan McInnes-Taylor", email = "mmcinnestaylor@gmail.com"}
 ]
 maintainers = [
-    {name = "Marlan McInnes-Taylor", email = "mmcinnestaylor@gmail.com"}
+    {name = "B-B-C Lab", email = "weixx@utexas.edu"}
 ]
 description = "A Pytorch implementation of Poisson Identifiable VAE (pi-VAE), a variational auto encoder used to construct latent variable models of neural activity while simultaneously modeling the relation between the latent and task variables."
 readme = "README.md"
 keywords = [
     "vae",
     "pi-vae",
     "poisson identifiable vae",
     "poisson identifiable variational autoencoder",
     "identifiable vae",
     "identifiable variational autoencoder"
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Science/Research",
-    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+    "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dynamic = ["version"]
 
 [project.urls]
-Homepage = "https://mmcinnestaylor.github.io/pi-vae-pytorch/"
-Repository = "https://github.com/mmcinnestaylor/pi-vae-pytorch"
+Homepage = "https://wei-bbc-lab.github.io/pi-vae-pytorch/"
+Repository = "https://github.com/wei-bbc-lab/pi-vae-pytorch"
 
 [tool.setuptools_scm]
```

