# Comparing `tmp/geosss-0.1.8.tar.gz` & `tmp/geosss-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geosss-0.1.8.tar", max compression
+gzip compressed data, was "geosss-0.1.9.tar", max compression
```

## Comparing `geosss-0.1.8.tar` & `geosss-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1474 2023-07-24 16:27:27.579099 geosss-0.1.8/LICENSE
--rw-r--r--   0        0        0     4853 2023-08-04 10:47:56.815008 geosss-0.1.8/README.md
--rw-r--r--   0        0        0      793 2023-07-25 18:35:32.784913 geosss-0.1.8/geosss/__init__.py
--rw-r--r--   0        0        0     1981 2023-07-25 18:35:32.784913 geosss-0.1.8/geosss/demo_vis.py
--rw-r--r--   0        0        0     5522 2023-07-25 18:35:32.784913 geosss-0.1.8/geosss/distributions.py
--rw-r--r--   0        0        0    10284 2023-07-25 18:35:32.784913 geosss-0.1.8/geosss/mcmc.py
--rw-r--r--   0        0        0     5091 2023-07-25 18:35:32.784913 geosss-0.1.8/geosss/rand.py
--rw-r--r--   0        0        0     3000 2023-07-25 18:35:32.784913 geosss-0.1.8/geosss/sphere.py
--rw-r--r--   0        0        0     7334 2023-07-25 18:35:32.784913 geosss-0.1.8/geosss/testing.py
--rw-r--r--   0        0        0     5156 2023-07-25 18:35:32.784913 geosss-0.1.8/geosss/utils.py
--rw-r--r--   0        0        0     9249 2023-07-25 18:35:32.784913 geosss-0.1.8/geosss/vMF_diagnostics.py
--rw-r--r--   0        0        0     1068 2023-08-04 10:52:04.367733 geosss-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     5954 1970-01-01 00:00:00.000000 geosss-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1474 2024-01-07 19:37:44.858409 geosss-0.1.9/LICENSE
+-rw-r--r--   0        0        0     5043 2024-01-07 19:37:44.858409 geosss-0.1.9/README.md
+-rw-r--r--   0        0        0      793 2024-01-07 19:37:44.862409 geosss-0.1.9/geosss/__init__.py
+-rw-r--r--   0        0        0     1981 2024-01-07 19:37:44.862409 geosss-0.1.9/geosss/demo_vis.py
+-rw-r--r--   0        0        0     5522 2024-01-07 19:37:44.862409 geosss-0.1.9/geosss/distributions.py
+-rw-r--r--   0        0        0    10284 2024-01-07 19:37:44.862409 geosss-0.1.9/geosss/mcmc.py
+-rw-r--r--   0        0        0     5091 2024-01-07 19:37:44.862409 geosss-0.1.9/geosss/rand.py
+-rw-r--r--   0        0        0     3000 2024-01-07 19:37:44.862409 geosss-0.1.9/geosss/sphere.py
+-rw-r--r--   0        0        0     7334 2024-01-07 19:37:44.862409 geosss-0.1.9/geosss/testing.py
+-rw-r--r--   0        0        0     5156 2024-01-07 19:37:44.862409 geosss-0.1.9/geosss/utils.py
+-rw-r--r--   0        0        0     9249 2024-01-07 19:37:44.862409 geosss-0.1.9/geosss/vMF_diagnostics.py
+-rw-r--r--   0        0        0     1068 2024-04-02 11:37:26.562113 geosss-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     6190 1970-01-01 00:00:00.000000 geosss-0.1.9/PKG-INFO
```

### Comparing `geosss-0.1.8/LICENSE` & `geosss-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `geosss-0.1.8/README.md` & `geosss-0.1.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 </div>
 
 # GeoSSS: Geodesic Slice Sampling on the Sphere
 
 This python package implements two novel tuning-free MCMC algorithms, an **ideal geodesic slice sampler** based on accept/reject strategy and a **shrinkage-based geodesic slice sampler** to sample from spherical distributions on arbitrary dimensions. The package also includes the implementation of random-walk Metropolis-Hastings (RWMH) and Hamiltonian Monte Carlo (HMC) whose step-size parameter is automatically tuned.
 As shown in our [paper](https://doi.org/10.48550/arXiv.2301.08056), our algorithms have outperformed RWMH and HMC for spherical distributions. 
 
-This demo quickly illustrates that. We consider a target that is a mixture of von Mises-Fisher distribution on a 2-sphere with concentration parameter $\kappa=80$. By using $10^3$ samples, our samplers GeoSSS (reject) and GeoSSS (shrink) (top row) explore all modes, whereas RWMH and HMC (bottom row) get stuck in a single mode. 
+This demo quickly illustrates that. We consider a target that is a mixture of von Mises-Fisher distribution on a 2-sphere with concentration parameter $\kappa=80$. By using $10^3$ samples, our samplers geoSSS (reject) and geoSSS (shrink) (top row) explore all modes, whereas RWMH and HMC (bottom row) get stuck in a single mode. 
 
 ![animation_vMF](https://github.com/microscopic-image-analysis/geosss/blob/927ff8c8187b88a1a72725c4e450ae0f0523431b/assets/animation_vMF.gif?raw=true)
 
 ## Installation
 
 GeoSSS is available for installation from [PyPI](https://pypi.org/project/geosss/). Therefore, simply type:
 
@@ -31,14 +31,19 @@
 
 To install dependencies required to run scripts under [`scripts/`](scripts/),
 
 ```bash
 pip install geosss[extras]
 ```
 
+If you want to install with the latest changes including all the dependencies,
+```bash
+pip install geosss[extras]@git+https://github.com/microscopic-image-analysis/geosss.git@main
+```
+
 ## Getting Started
 
 A minimal example to get started as well as reproduce the above demo:
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/microscopic-image-analysis/geosss/blob/main/scripts/demo.ipynb)
 ```python
 import geosss as gs
@@ -66,19 +71,19 @@
 
 # initial state of the samplers
 init_state = np.array([-0.86333052,  0.18685286, -0.46877117])
 
 # sampling with the four samplers
 samples = {}
 
-# GeoSSS (reject): ideal geodesic slice sampler
+# geoSSS (reject): ideal geodesic slice sampler
 rsss = gs.RejectionSphericalSliceSampler(pdf, init_state, seed)
 samples['sss-reject'] = rsss.sample(n_samples, burnin)
 
-# GeoSSS (shrink): shrinkage-based geodesic slice sampler
+# geoSSS (shrink): shrinkage-based geodesic slice sampler
 ssss = gs.ShrinkageSphericalSliceSampler(pdf, init_state, seed)
 samples['sss-shrink'] = ssss.sample(n_samples, burnin)
 
 # RWMH: random-walk Metropolis Hastings
 rwmh = gs.MetropolisHastings(pdf, init_state, seed)
 samples['rwmh'] = rwmh.sample(n_samples, burnin)
```

### Comparing `geosss-0.1.8/geosss/__init__.py` & `geosss-0.1.9/geosss/__init__.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.8/geosss/demo_vis.py` & `geosss-0.1.9/geosss/demo_vis.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.8/geosss/distributions.py` & `geosss-0.1.9/geosss/distributions.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.8/geosss/mcmc.py` & `geosss-0.1.9/geosss/mcmc.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.8/geosss/rand.py` & `geosss-0.1.9/geosss/rand.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.8/geosss/sphere.py` & `geosss-0.1.9/geosss/sphere.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.8/geosss/testing.py` & `geosss-0.1.9/geosss/testing.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.8/geosss/utils.py` & `geosss-0.1.9/geosss/utils.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.8/geosss/vMF_diagnostics.py` & `geosss-0.1.9/geosss/vMF_diagnostics.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.8/pyproject.toml` & `geosss-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geosss"
-version = "0.1.8"
+version = "0.1.9"
 description = "Python package implementing an ideal and shrinkage-based geodesic slice sampling on the sphere."
 authors = ["Michael Habeck <michael.habeck@uni-jena.de>",
            "Shantanu Kodgirwar <shantanu.kodgirwar@uni-jena.de>", 
            "Mareike Hasenpflug <mareike.hasenpflug@uni-passau.de>",
            "Daniel Rudolf <daniel.rudolf@uni-passau.de>"]
 license = "BSD-3-Clause"
 readme = "README.md"
@@ -15,15 +15,15 @@
 scipy = "^1.11.1"
 numpy = "^1.25.1"
 matplotlib = "^3.7.2"
 csb = "^1.2.5"
 arviz = "^0.15.1"
 seaborn = { version = "^0.12.2", optional = true }
 tsp-solver = { version = "^0.1", optional = true }
-black = { version = "^23.7.0", optional = true }
+black = { version = "^24.3.0", optional = true }
 ipykernel = { version = "^6.25.0", optional = true }
 
 [tool.poetry.extras]
 extras = ["seaborn", "tsp-solver"]
 dev = ["seaborn", "tsp-solver", "black", "ipykernel"]
 
 [build-system]
```

### Comparing `geosss-0.1.8/PKG-INFO` & `geosss-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: geosss
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python package implementing an ideal and shrinkage-based geodesic slice sampling on the sphere.
 Home-page: https://github.com/microscopic-image-analysis/geosss
 License: BSD-3-Clause
 Author: Michael Habeck
 Author-email: michael.habeck@uni-jena.de
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: dev
 Provides-Extra: extras
 Requires-Dist: arviz (>=0.15.1,<0.16.0)
-Requires-Dist: black (>=23.7.0,<24.0.0) ; extra == "dev"
+Requires-Dist: black (>=24.3.0,<25.0.0) ; extra == "dev"
 Requires-Dist: csb (>=1.2.5,<2.0.0)
 Requires-Dist: ipykernel (>=6.25.0,<7.0.0) ; extra == "dev"
 Requires-Dist: matplotlib (>=3.7.2,<4.0.0)
 Requires-Dist: numpy (>=1.25.1,<2.0.0)
 Requires-Dist: scipy (>=1.11.1,<2.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0) ; extra == "extras" or extra == "dev"
 Requires-Dist: tsp-solver (>=0.1,<0.2) ; extra == "extras" or extra == "dev"
@@ -41,15 +42,15 @@
 </div>
 
 # GeoSSS: Geodesic Slice Sampling on the Sphere
 
 This python package implements two novel tuning-free MCMC algorithms, an **ideal geodesic slice sampler** based on accept/reject strategy and a **shrinkage-based geodesic slice sampler** to sample from spherical distributions on arbitrary dimensions. The package also includes the implementation of random-walk Metropolis-Hastings (RWMH) and Hamiltonian Monte Carlo (HMC) whose step-size parameter is automatically tuned.
 As shown in our [paper](https://doi.org/10.48550/arXiv.2301.08056), our algorithms have outperformed RWMH and HMC for spherical distributions. 
 
-This demo quickly illustrates that. We consider a target that is a mixture of von Mises-Fisher distribution on a 2-sphere with concentration parameter $\kappa=80$. By using $10^3$ samples, our samplers GeoSSS (reject) and GeoSSS (shrink) (top row) explore all modes, whereas RWMH and HMC (bottom row) get stuck in a single mode. 
+This demo quickly illustrates that. We consider a target that is a mixture of von Mises-Fisher distribution on a 2-sphere with concentration parameter $\kappa=80$. By using $10^3$ samples, our samplers geoSSS (reject) and geoSSS (shrink) (top row) explore all modes, whereas RWMH and HMC (bottom row) get stuck in a single mode. 
 
 ![animation_vMF](https://github.com/microscopic-image-analysis/geosss/blob/927ff8c8187b88a1a72725c4e450ae0f0523431b/assets/animation_vMF.gif?raw=true)
 
 ## Installation
 
 GeoSSS is available for installation from [PyPI](https://pypi.org/project/geosss/). Therefore, simply type:
 
@@ -59,14 +60,19 @@
 
 To install dependencies required to run scripts under [`scripts/`](scripts/),
 
 ```bash
 pip install geosss[extras]
 ```
 
+If you want to install with the latest changes including all the dependencies,
+```bash
+pip install geosss[extras]@git+https://github.com/microscopic-image-analysis/geosss.git@main
+```
+
 ## Getting Started
 
 A minimal example to get started as well as reproduce the above demo:
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/microscopic-image-analysis/geosss/blob/main/scripts/demo.ipynb)
 ```python
 import geosss as gs
@@ -94,19 +100,19 @@
 
 # initial state of the samplers
 init_state = np.array([-0.86333052,  0.18685286, -0.46877117])
 
 # sampling with the four samplers
 samples = {}
 
-# GeoSSS (reject): ideal geodesic slice sampler
+# geoSSS (reject): ideal geodesic slice sampler
 rsss = gs.RejectionSphericalSliceSampler(pdf, init_state, seed)
 samples['sss-reject'] = rsss.sample(n_samples, burnin)
 
-# GeoSSS (shrink): shrinkage-based geodesic slice sampler
+# geoSSS (shrink): shrinkage-based geodesic slice sampler
 ssss = gs.ShrinkageSphericalSliceSampler(pdf, init_state, seed)
 samples['sss-shrink'] = ssss.sample(n_samples, burnin)
 
 # RWMH: random-walk Metropolis Hastings
 rwmh = gs.MetropolisHastings(pdf, init_state, seed)
 samples['rwmh'] = rwmh.sample(n_samples, burnin)
```

