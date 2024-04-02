# Comparing `tmp/margarine-1.2.3.tar.gz` & `tmp/margarine-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "margarine-1.2.3.tar", last modified: Tue Dec 12 12:57:51 2023, max compression
+gzip compressed data, was "margarine-1.2.8.tar", last modified: Tue Apr  2 15:31:12 2024, max compression
```

## Comparing `margarine-1.2.3.tar` & `margarine-1.2.8.tar`

### file list

```diff
@@ -1,22 +1,49 @@
-drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-12-12 12:57:51.189962 margarine-1.2.3/
--rw-r--r--   0 harry      (501) staff       (20)     1082 2022-09-13 13:30:11.000000 margarine-1.2.3/LICENSE
--rw-r--r--   0 harry      (501) staff       (20)     6985 2023-12-12 12:57:51.189793 margarine-1.2.3/PKG-INFO
--rwxr-xr-x   0 harry      (501) staff       (20)     5839 2023-12-12 12:53:25.000000 margarine-1.2.3/README.rst
-drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-12-12 12:57:51.187949 margarine-1.2.3/margarine/
--rwxr-xr-x   0 harry      (501) staff       (20)        0 2022-10-11 07:45:31.000000 margarine-1.2.3/margarine/__init__.py
--rw-r--r--   0 harry      (501) staff       (20)    19203 2023-12-12 12:47:40.000000 margarine-1.2.3/margarine/clustered.py
--rwxr-xr-x   0 harry      (501) staff       (20)    12133 2023-08-30 14:56:59.000000 margarine-1.2.3/margarine/kde.py
--rwxr-xr-x   0 harry      (501) staff       (20)    18944 2023-08-30 15:25:38.000000 margarine-1.2.3/margarine/maf.py
--rwxr-xr-x   0 harry      (501) staff       (20)    10406 2023-12-12 12:47:40.000000 margarine-1.2.3/margarine/marginal_stats.py
--rwxr-xr-x   0 harry      (501) staff       (20)     2437 2023-08-04 12:40:44.000000 margarine-1.2.3/margarine/processing.py
-drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-12-12 12:57:51.189426 margarine-1.2.3/margarine.egg-info/
--rw-r--r--   0 harry      (501) staff       (20)     6985 2023-12-12 12:57:51.000000 margarine-1.2.3/margarine.egg-info/PKG-INFO
--rw-r--r--   0 harry      (501) staff       (20)      365 2023-12-12 12:57:51.000000 margarine-1.2.3/margarine.egg-info/SOURCES.txt
--rw-r--r--   0 harry      (501) staff       (20)        1 2023-12-12 12:57:51.000000 margarine-1.2.3/margarine.egg-info/dependency_links.txt
--rw-r--r--   0 harry      (501) staff       (20)      198 2023-12-12 12:57:51.000000 margarine-1.2.3/margarine.egg-info/requires.txt
--rw-r--r--   0 harry      (501) staff       (20)       10 2023-12-12 12:57:51.000000 margarine-1.2.3/margarine.egg-info/top_level.txt
--rw-r--r--   0 harry      (501) staff       (20)       38 2023-12-12 12:57:51.189996 margarine-1.2.3/setup.cfg
--rwxr-xr-x   0 harry      (501) staff       (20)     1509 2023-12-12 12:53:28.000000 margarine-1.2.3/setup.py
-drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-12-12 12:57:51.189175 margarine-1.2.3/tests/
--rw-r--r--   0 harry      (501) staff       (20)     2517 2023-12-12 12:47:40.000000 margarine-1.2.3/tests/test_clusters.py
--rwxr-xr-x   0 harry      (501) staff       (20)     6264 2023-12-12 12:47:40.000000 margarine-1.2.3/tests/test_stats.py
+drwxr-xr-x   0 harry      (501) staff       (20)        0 2024-04-02 15:31:12.898195 margarine-1.2.8/
+drwxr-xr-x   0 harry      (501) staff       (20)        0 2024-04-02 15:31:12.883231 margarine-1.2.8/.github/
+drwxr-xr-x   0 harry      (501) staff       (20)        0 2024-04-02 15:31:12.886526 margarine-1.2.8/.github/workflows/
+-rw-r--r--   0 harry      (501) staff       (20)     1537 2023-05-16 11:26:37.000000 margarine-1.2.8/.github/workflows/CI.yml
+-rw-r--r--   0 harry      (501) staff       (20)      426 2024-03-11 21:05:45.000000 margarine-1.2.8/.github/workflows/version_checks.yaml
+-rw-r--r--   0 harry      (501) staff       (20)       45 2024-03-21 08:32:39.000000 margarine-1.2.8/.gitignore
+-rw-r--r--   0 harry      (501) staff       (20)      556 2024-03-21 08:32:39.000000 margarine-1.2.8/.readthedocs.yml
+-rw-r--r--   0 harry      (501) staff       (20)     1082 2022-09-13 13:30:11.000000 margarine-1.2.8/LICENSE
+-rw-r--r--   0 harry      (501) staff       (20)     6985 2024-04-02 15:31:12.897908 margarine-1.2.8/PKG-INFO
+-rwxr-xr-x   0 harry      (501) staff       (20)     5839 2024-04-02 15:02:59.000000 margarine-1.2.8/README.rst
+drwxr-xr-x   0 harry      (501) staff       (20)        0 2024-04-02 15:31:12.886834 margarine-1.2.8/bin/
+-rw-r--r--   0 harry      (501) staff       (20)     3908 2024-03-11 21:05:45.000000 margarine-1.2.8/bin/check_version.py
+drwxr-xr-x   0 harry      (501) staff       (20)        0 2024-04-02 15:31:12.887641 margarine-1.2.8/docs/
+-rw-r--r--   0 harry      (501) staff       (20)      637 2024-03-11 21:05:45.000000 margarine-1.2.8/docs/Makefile
+-rw-r--r--   0 harry      (501) staff       (20)      795 2022-09-13 13:30:11.000000 margarine-1.2.8/docs/make.bat
+-rw-r--r--   0 harry      (501) staff       (20)       33 2023-08-05 09:17:51.000000 margarine-1.2.8/docs/requirements.txt
+drwxr-xr-x   0 harry      (501) staff       (20)        0 2024-04-02 15:31:12.892017 margarine-1.2.8/docs/source/
+-rw-r--r--   0 harry      (501) staff       (20)    24566 2022-09-13 15:09:06.000000 margarine-1.2.8/docs/source/Tutorial_15_0.png
+-rw-r--r--   0 harry      (501) staff       (20)    40024 2022-09-13 15:09:06.000000 margarine-1.2.8/docs/source/Tutorial_17_0.png
+-rw-r--r--   0 harry      (501) staff       (20)    37176 2022-09-13 15:09:06.000000 margarine-1.2.8/docs/source/Tutorial_5_0.png
+-rw-r--r--   0 harry      (501) staff       (20)    42371 2022-09-13 15:09:06.000000 margarine-1.2.8/docs/source/Tutorial_9_0.png
+-rw-r--r--   0 harry      (501) staff       (20)     2801 2024-03-11 21:05:45.000000 margarine-1.2.8/docs/source/conf.py
+-rw-r--r--   0 harry      (501) staff       (20)      363 2024-03-11 21:05:45.000000 margarine-1.2.8/docs/source/functions.rst
+-rw-r--r--   0 harry      (501) staff       (20)      226 2022-09-13 13:30:11.000000 margarine-1.2.8/docs/source/index.rst
+-rw-r--r--   0 harry      (501) staff       (20)       86 2022-09-13 13:30:11.000000 margarine-1.2.8/docs/source/intro.rst
+-rw-r--r--   0 harry      (501) staff       (20)      268 2023-08-05 09:17:51.000000 margarine-1.2.8/docs/source/tutorial.rst
+drwxr-xr-x   0 harry      (501) staff       (20)        0 2024-04-02 15:31:12.893818 margarine-1.2.8/margarine/
+-rwxr-xr-x   0 harry      (501) staff       (20)        0 2022-10-11 07:45:31.000000 margarine-1.2.8/margarine/__init__.py
+-rw-r--r--   0 harry      (501) staff       (20)    19625 2024-03-11 21:05:45.000000 margarine-1.2.8/margarine/clustered.py
+-rwxr-xr-x   0 harry      (501) staff       (20)    12134 2024-03-11 21:05:45.000000 margarine-1.2.8/margarine/kde.py
+-rwxr-xr-x   0 harry      (501) staff       (20)    19301 2024-03-21 17:49:34.000000 margarine-1.2.8/margarine/maf.py
+-rwxr-xr-x   0 harry      (501) staff       (20)    10414 2024-03-11 21:05:45.000000 margarine-1.2.8/margarine/marginal_stats.py
+-rwxr-xr-x   0 harry      (501) staff       (20)     2437 2023-08-04 12:40:44.000000 margarine-1.2.8/margarine/processing.py
+drwxr-xr-x   0 harry      (501) staff       (20)        0 2024-04-02 15:31:12.897217 margarine-1.2.8/margarine.egg-info/
+-rw-r--r--   0 harry      (501) staff       (20)     6985 2024-04-02 15:31:12.000000 margarine-1.2.8/margarine.egg-info/PKG-INFO
+-rw-r--r--   0 harry      (501) staff       (20)      856 2024-04-02 15:31:12.000000 margarine-1.2.8/margarine.egg-info/SOURCES.txt
+-rw-r--r--   0 harry      (501) staff       (20)        1 2024-04-02 15:31:12.000000 margarine-1.2.8/margarine.egg-info/dependency_links.txt
+-rw-r--r--   0 harry      (501) staff       (20)      198 2024-04-02 15:31:12.000000 margarine-1.2.8/margarine.egg-info/requires.txt
+-rw-r--r--   0 harry      (501) staff       (20)       10 2024-04-02 15:31:12.000000 margarine-1.2.8/margarine.egg-info/top_level.txt
+drwxr-xr-x   0 harry      (501) staff       (20)        0 2024-04-02 15:31:12.895006 margarine-1.2.8/notebook/
+-rw-r--r--   0 harry      (501) staff       (20)   348569 2023-12-12 12:47:40.000000 margarine-1.2.8/notebook/Tutorial.ipynb
+-rw-r--r--   0 harry      (501) staff       (20)      165 2024-04-02 15:15:44.000000 margarine-1.2.8/requirements.txt
+-rw-r--r--   0 harry      (501) staff       (20)        5 2024-04-02 15:10:35.000000 margarine-1.2.8/requirements_test.txt
+-rw-r--r--   0 harry      (501) staff       (20)       38 2024-04-02 15:31:12.898245 margarine-1.2.8/setup.cfg
+-rwxr-xr-x   0 harry      (501) staff       (20)     1878 2024-03-11 21:05:45.000000 margarine-1.2.8/setup.py
+drwxr-xr-x   0 harry      (501) staff       (20)        0 2024-04-02 15:31:12.896792 margarine-1.2.8/tests/
+-rw-r--r--   0 harry      (501) staff       (20)     2996 2023-05-16 11:26:37.000000 margarine-1.2.8/tests/clustered_distributions.py
+-rw-r--r--   0 harry      (501) staff       (20)     2517 2023-12-12 12:47:40.000000 margarine-1.2.8/tests/test_clusters.py
+-rwxr-xr-x   0 harry      (501) staff       (20)     6264 2024-03-21 08:32:35.000000 margarine-1.2.8/tests/test_stats.py
```

### Comparing `margarine-1.2.3/LICENSE` & `margarine-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `margarine-1.2.3/PKG-INFO` & `margarine-1.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: margarine
-Version: 1.2.3
+Version: 1.2.8
 Summary: margarine: Posterior Sampling and Marginal Bayesian Statistics
 Home-page: https://github.com/htjb/margarine
 Author: Harry T. J. Bevins
 Author-email: htjb2@cam.ac.uk
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
@@ -35,15 +35,15 @@
 ================================================================
 
 Introduction
 ------------
 
 :margarine: Marginal Bayesian Statistics
 :Authors: Harry T.J. Bevins
-:Version: 1.2.3
+:Version: 1.2.8
 :Homepage:  https://github.com/htjb/margarine
 :Documentation: https://margarine.readthedocs.io/
 
 .. image:: https://readthedocs.org/projects/margarine/badge/?version=latest
   :target: https://margarine.readthedocs.io/en/latest/?badge=latest
   :alt: Documentation Status
 .. image:: https://mybinder.org/badge_logo.svg
```

### Comparing `margarine-1.2.3/README.rst` & `margarine-1.2.8/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ================================================================
 
 Introduction
 ------------
 
 :margarine: Marginal Bayesian Statistics
 :Authors: Harry T.J. Bevins
-:Version: 1.2.3
+:Version: 1.2.8
 :Homepage:  https://github.com/htjb/margarine
 :Documentation: https://margarine.readthedocs.io/
 
 .. image:: https://readthedocs.org/projects/margarine/badge/?version=latest
   :target: https://margarine.readthedocs.io/en/latest/?badge=latest
   :alt: Documentation Status
 .. image:: https://mybinder.org/badge_logo.svg
```

### Comparing `margarine-1.2.3/margarine/clustered.py` & `margarine-1.2.8/margarine/clustered.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,19 @@
                 quality of emulation.
 
         hidden_layers: **list / default = [50, 50]**
             | The number of layers and number of nodes in each hidden layer for
                 each neural network. The default is two hidden layers with
                 50 nodes each and each network in the chain has the same hidden
                 layer structure.
+        
+        activation_func: **string / default = 'tanh'**
+            | The choice of activation function. It must be an activation
+                function keyword recognisable by TensorFlow. The default is
+                'tanh', the hyperbolic tangent activation function.
 
         cluster_labels: **list / default = None**
             | If clustering has been performed externally to margarine you can
                 provide a list of labels for the samples theta. The labels
                 should be integers from 0 to k corresponding to the cluster
                 that each sample is in.
 
@@ -73,14 +78,15 @@
         # Unpack kwargs
         self.number_networks = kwargs.pop('number_networks', 6)
         self.learning_rate = kwargs.pop('learning_rate', 1e-3)
         self.hidden_layers = kwargs.pop('hidden_layers', [50, 50])
         self.cluster_labels = kwargs.pop('cluster_labels', None)
         self.cluster_number = kwargs.pop('cluster_number', None)
         self.parameters = kwargs.pop('parameters', None)
+        self.activation_func = kwargs.pop('activation_func', 'tanh')
 
         # Avoid unintended side effects by copying theta
         theta = theta.copy()
 
         if isinstance(theta, 
                       (anesthetic.samples.NestedSamples, 
                        anesthetic.samples.MCMCSamples)):
@@ -228,15 +234,16 @@
         for i in range(len(split_theta)):
             self.flow.append(MAF(split_theta[i], 
                                  weights=split_sample_weights[i],
                                  number_networks=self.number_networks,
                                  learning_rate=self.learning_rate,
                                  hidden_layers=self.hidden_layers,
                                  theta_min=self.theta_min,
-                                 theta_max=self.theta_max))
+                                 theta_max=self.theta_max,
+                                 activation_func=self.activation_func))
 
     def train(self, epochs=100, early_stop=False, loss_type='sum'):
 
         r"""
         This function is called to train the clusterMAF once it has been
         initialised. It calls the `train()` function for each flow.
```

### Comparing `margarine-1.2.3/margarine/kde.py` & `margarine-1.2.8/margarine/kde.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         theta_min: **numpy array**
             | As above but the true lower limits of the priors.
 
         parameters: **list of strings**
             | A list of the relevant parameters to train on. Only needed
                 if theta is an anestehetic samples object. If not provided,
                 all parameters will be used.
+
     **Attributes:**
 
     A list of some key attributes accessible to the user.
 
         kde: **Instance of scipy.stats.gaussian_kde**
             | Once the class has been initalised with a set of samples and
                 their corresponding weights we can generate the kde using
```

### Comparing `margarine-1.2.3/margarine/maf.py` & `margarine-1.2.8/margarine/maf.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,19 @@
 
         hidden_layers: **list / default = [50, 50]**
             | The number of layers and number of nodes in each hidden layer for
                 each neural network. The default is two hidden layers with
                 50 nodes each and each network in the chain has the same hidden
                 layer structure.
 
+        activation_func: **string / default = 'tanh'**
+            | The choice of activation function. It must be an activation
+                function keyword recognisable by TensorFlow. The default is
+                'tanh', the hyperbolic tangent activation function.
+
         theta_max: **numpy array**
             | The true upper limits of the priors used to generate the samples
                 that we want the MAF to learn.
 
         theta_min: **numpy array**
             | As above but the true lower limits of the priors.
             
@@ -81,14 +86,15 @@
     """
 
     def __init__(self, theta, **kwargs):
         self.number_networks = kwargs.pop('number_networks', 6)
         self.learning_rate = kwargs.pop('learning_rate', 1e-3)
         self.hidden_layers = kwargs.pop('hidden_layers', [50, 50])
         self.parameters = kwargs.pop('parameters', None)
+        self.activation_func = kwargs.pop('activation_func', 'tanh')
 
         # Avoids unintended side effects outside the class
         if not isinstance(theta, tf.Tensor):
             theta = theta.copy()
         else:
             theta = tf.identity(theta)
 
@@ -172,15 +178,15 @@
         self.gen_mades()
 
     def gen_mades(self):
 
         """Generating the masked autoregressive flow."""
 
         self.mades = [tfb.AutoregressiveNetwork(params=2,
-                      hidden_units=self.hidden_layers, activation='tanh',
+                      hidden_units=self.hidden_layers, activation=self.activation_func,
                       input_order='random')
                       for _ in range(self.number_networks)]
 
         self.bij = tfb.Chain([
             tfb.MaskedAutoregressiveFlow(made) for made in self.mades])
 
         self.base = tfd.Blockwise(
```

### Comparing `margarine-1.2.3/margarine/marginal_stats.py` & `margarine-1.2.8/margarine/marginal_stats.py`

 * *Files identical despite different names*

```diff
@@ -208,16 +208,16 @@
                 | The number of samples to draw at each iteration.
             sample_size: **int**
                 | The number of samples to draw in total.
             logzero: **float**
                   The definition of zero for the loglikelihood function.
 
         returns:
-        stats: **dict**
-            | Dictionary containing useful statistics
+            stats: **dict**
+                | Dictionary containing useful statistics
 
         """
         xs = np.empty((sample_size, self.de.theta.shape[-1]))
         fs = np.empty(sample_size)
         gs = np.empty(sample_size)
         pis = np.empty(sample_size)
```

### Comparing `margarine-1.2.3/margarine/processing.py` & `margarine-1.2.8/margarine/processing.py`

 * *Files identical despite different names*

### Comparing `margarine-1.2.3/margarine.egg-info/PKG-INFO` & `margarine-1.2.8/margarine.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: margarine
-Version: 1.2.3
+Version: 1.2.8
 Summary: margarine: Posterior Sampling and Marginal Bayesian Statistics
 Home-page: https://github.com/htjb/margarine
 Author: Harry T. J. Bevins
 Author-email: htjb2@cam.ac.uk
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
@@ -35,15 +35,15 @@
 ================================================================
 
 Introduction
 ------------
 
 :margarine: Marginal Bayesian Statistics
 :Authors: Harry T.J. Bevins
-:Version: 1.2.3
+:Version: 1.2.8
 :Homepage:  https://github.com/htjb/margarine
 :Documentation: https://margarine.readthedocs.io/
 
 .. image:: https://readthedocs.org/projects/margarine/badge/?version=latest
   :target: https://margarine.readthedocs.io/en/latest/?badge=latest
   :alt: Documentation Status
 .. image:: https://mybinder.org/badge_logo.svg
```

### Comparing `margarine-1.2.3/setup.py` & `margarine-1.2.8/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,17 +3,26 @@
 def readme(short=False):
     with open('README.rst') as f:
         if short:
             return f.readlines()[1].strip()
         else:
             return f.read()
 
+def get_version_from_readme() -> str:
+    """Get current version of package from README.rst"""
+    readme_text = readme()
+    for line in readme_text.splitlines():
+        if ":Version:" in line:
+            current_version = line.split(":")[-1].strip()
+            return current_version
+    raise ValueError("Could not find version in README.rst")
+
 setup(
     name='margarine',
-    version='1.2.3',
+    version=get_version_from_readme(),
     description='margarine: Posterior Sampling and Marginal Bayesian Statistics',
     long_description=readme(),
     author='Harry T. J. Bevins',
     author_email='htjb2@cam.ac.uk',
     url='https://github.com/htjb/margarine',
     packages=find_packages(),
     install_requires=['numpy',
```

### Comparing `margarine-1.2.3/tests/test_clusters.py` & `margarine-1.2.8/tests/test_clusters.py`

 * *Files identical despite different names*

### Comparing `margarine-1.2.3/tests/test_stats.py` & `margarine-1.2.8/tests/test_stats.py`

 * *Files identical despite different names*

