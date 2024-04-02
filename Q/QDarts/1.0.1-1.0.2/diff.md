# Comparing `tmp/QDarts-1.0.1.tar.gz` & `tmp/QDarts-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QDarts-1.0.1.tar", last modified: Tue Apr  2 08:34:24 2024, max compression
+gzip compressed data, was "QDarts-1.0.2.tar", last modified: Tue Apr  2 14:33:58 2024, max compression
```

## Comparing `QDarts-1.0.1.tar` & `QDarts-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 evert      (501) staff       (20)        0 2024-04-02 08:34:24.939702 QDarts-1.0.1/
--rw-r--r--   0 evert      (501) staff       (20)     1073 2024-03-29 08:16:26.000000 QDarts-1.0.1/LICENCE.md
--rw-r--r--   0 evert      (501) staff       (20)     2983 2024-04-02 08:34:24.939523 QDarts-1.0.1/PKG-INFO
-drwxr-xr-x   0 evert      (501) staff       (20)        0 2024-04-02 08:34:24.939333 QDarts-1.0.1/QDarts.egg-info/
--rw-r--r--   0 evert      (501) staff       (20)     2983 2024-04-02 08:34:24.000000 QDarts-1.0.1/QDarts.egg-info/PKG-INFO
--rw-r--r--   0 evert      (501) staff       (20)      350 2024-04-02 08:34:24.000000 QDarts-1.0.1/QDarts.egg-info/SOURCES.txt
--rw-r--r--   0 evert      (501) staff       (20)        1 2024-04-02 08:34:24.000000 QDarts-1.0.1/QDarts.egg-info/dependency_links.txt
--rw-r--r--   0 evert      (501) staff       (20)        7 2024-04-02 08:34:24.000000 QDarts-1.0.1/QDarts.egg-info/top_level.txt
--rw-r--r--   0 evert      (501) staff       (20)     2319 2024-04-02 08:30:14.000000 QDarts-1.0.1/README.md
--rw-r--r--   0 evert      (501) staff       (20)      769 2024-04-02 08:32:05.000000 QDarts-1.0.1/pyproject.toml
-drwxr-xr-x   0 evert      (501) staff       (20)        0 2024-04-02 08:34:24.938723 QDarts-1.0.1/qdarts/
--rw-r--r--   0 evert      (501) staff       (20)        0 2024-03-29 08:16:26.000000 QDarts-1.0.1/qdarts/__init__.py
--rw-r--r--   0 evert      (501) staff       (20)    18216 2024-04-02 08:13:36.000000 QDarts-1.0.1/qdarts/experiment.py
--rw-r--r--   0 evert      (501) staff       (20)    10462 2024-03-29 08:16:26.000000 QDarts-1.0.1/qdarts/model.py
--rw-r--r--   0 evert      (501) staff       (20)      673 2024-03-29 08:16:26.000000 QDarts-1.0.1/qdarts/noise_processes.py
--rw-r--r--   0 evert      (501) staff       (20)     9073 2024-03-29 08:16:26.000000 QDarts-1.0.1/qdarts/plotting.py
--rw-r--r--   0 evert      (501) staff       (20)     2034 2024-03-29 08:16:26.000000 QDarts-1.0.1/qdarts/polytope.py
--rw-r--r--   0 evert      (501) staff       (20)    13713 2024-03-29 08:16:26.000000 QDarts-1.0.1/qdarts/simulator.py
--rw-r--r--   0 evert      (501) staff       (20)    12536 2024-03-29 08:16:26.000000 QDarts-1.0.1/qdarts/tunneling_simulator.py
--rw-r--r--   0 evert      (501) staff       (20)     9989 2024-03-29 08:16:26.000000 QDarts-1.0.1/qdarts/util_functions.py
--rw-r--r--   0 evert      (501) staff       (20)       38 2024-04-02 08:34:24.939747 QDarts-1.0.1/setup.cfg
+drwxr-xr-x   0 evert      (501) staff       (20)        0 2024-04-02 14:33:58.066310 QDarts-1.0.2/
+-rw-r--r--   0 evert      (501) staff       (20)     1073 2024-03-29 08:16:26.000000 QDarts-1.0.2/LICENCE.md
+-rw-r--r--   0 evert      (501) staff       (20)     2981 2024-04-02 14:33:58.066119 QDarts-1.0.2/PKG-INFO
+drwxr-xr-x   0 evert      (501) staff       (20)        0 2024-04-02 14:33:58.065902 QDarts-1.0.2/QDarts.egg-info/
+-rw-r--r--   0 evert      (501) staff       (20)     2981 2024-04-02 14:33:58.000000 QDarts-1.0.2/QDarts.egg-info/PKG-INFO
+-rw-r--r--   0 evert      (501) staff       (20)      350 2024-04-02 14:33:58.000000 QDarts-1.0.2/QDarts.egg-info/SOURCES.txt
+-rw-r--r--   0 evert      (501) staff       (20)        1 2024-04-02 14:33:58.000000 QDarts-1.0.2/QDarts.egg-info/dependency_links.txt
+-rw-r--r--   0 evert      (501) staff       (20)        7 2024-04-02 14:33:58.000000 QDarts-1.0.2/QDarts.egg-info/top_level.txt
+-rw-r--r--   0 evert      (501) staff       (20)     2317 2024-04-02 14:33:14.000000 QDarts-1.0.2/README.md
+-rw-r--r--   0 evert      (501) staff       (20)      769 2024-04-02 14:33:35.000000 QDarts-1.0.2/pyproject.toml
+drwxr-xr-x   0 evert      (501) staff       (20)        0 2024-04-02 14:33:58.065476 QDarts-1.0.2/qdarts/
+-rw-r--r--   0 evert      (501) staff       (20)        0 2024-03-29 08:16:26.000000 QDarts-1.0.2/qdarts/__init__.py
+-rw-r--r--   0 evert      (501) staff       (20)    18216 2024-04-02 08:13:36.000000 QDarts-1.0.2/qdarts/experiment.py
+-rw-r--r--   0 evert      (501) staff       (20)    10462 2024-03-29 08:16:26.000000 QDarts-1.0.2/qdarts/model.py
+-rw-r--r--   0 evert      (501) staff       (20)      673 2024-03-29 08:16:26.000000 QDarts-1.0.2/qdarts/noise_processes.py
+-rw-r--r--   0 evert      (501) staff       (20)     9073 2024-03-29 08:16:26.000000 QDarts-1.0.2/qdarts/plotting.py
+-rw-r--r--   0 evert      (501) staff       (20)     2034 2024-03-29 08:16:26.000000 QDarts-1.0.2/qdarts/polytope.py
+-rw-r--r--   0 evert      (501) staff       (20)    13713 2024-03-29 08:16:26.000000 QDarts-1.0.2/qdarts/simulator.py
+-rw-r--r--   0 evert      (501) staff       (20)    12536 2024-03-29 08:16:26.000000 QDarts-1.0.2/qdarts/tunneling_simulator.py
+-rw-r--r--   0 evert      (501) staff       (20)     9989 2024-03-29 08:16:26.000000 QDarts-1.0.2/qdarts/util_functions.py
+-rw-r--r--   0 evert      (501) staff       (20)       38 2024-04-02 14:33:58.066352 QDarts-1.0.2/setup.cfg
```

### Comparing `QDarts-1.0.1/LICENCE.md` & `QDarts-1.0.2/LICENCE.md`

 * *Files identical despite different names*

### Comparing `QDarts-1.0.1/PKG-INFO` & `QDarts-1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QDarts
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package for simulating realistic quantum dot arrays and their charge transitions.
 Author-email: Jan Krzywda <j.a.krzywda@liacs.leidenuniv.nl>, Evert van Nieuwenburg <e.p.l.van.nieuwenburg@liacs.leidenuniv.nl>, Oswin Krause <oswin.krause@di.ku.dk>
 Project-URL: Homepage, https://github.com/condensedAI/QDarts
 Project-URL: Issues, https://github.com/condensedAI/QDarts
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,28 +27,25 @@
 
 ## Installation
 The package supports Python 3.6 and later. To install the package, run the following command:
 
     pip install qdarts
 
 ## Manuscript
-The package is based on the manuscript by [Krause et al., QDarts: Efficient Quantum Dot array transition simulator; The transition finding in presence of finite tunnel couplings, non-constant charging energies and sensor dots](). The manuscript has been submitted to the SciPost Physics Codebases.
+The package is based on the manuscript by [Krzywda et al., QDarts: A Quantum Dot Array Transition Simulator for finding charge transitions in the presence of finite tunnel couplings, non-constant charging energies and sensor dots](). The manuscript has been submitted to the SciPost Physics Codebases.
 
 ## Examples
 The package provides a simple example to demonstrate the usage of the package. The example is available in the examples qatpack/examples folder. The example demonstrates the simulation of a quantum dot array with sensor dots, tunnel couplings, and non-constant charging energy. 
 
-As a proof of principle, in the example we reconstruct the figure from the paper [Neyens et al.](https://journals.aps.org/prapplied/abstract/10.1103/PhysRevApplied.12.064049z), which shows the measured charge conductance signal from two sensor dots, which detect simultanous four-dot transition in the quantum dot array. The figure, visible below, has been computed in about a minute on tabletop computer.
+As a proof of principle, in the example we reconstruct the figure from the paper [Neyens et al.](https://journals.aps.org/prapplied/abstract/10.1103/PhysRevApplied.12.064049z), which shows the measured charge conductance signal from two sensor dots, which detect simultanous four-dot transition in the quantum dot array. The figure, visible below, has been computed in about a minute on a standard laptop.
 
 <p align="center">
-  <img src="qdarts/figures/neyens.png" />
+  <img src="examples/figures/neyens.png" />
 <p/>
-using several line prompt:
     
-    
-
 ## Files in this repository
     qdarts
         |-- qdarts
             |-- model.py
             |-- noise_processes.py
             |-- experiment.py
             |-- plotting.py
@@ -56,7 +53,8 @@
             |-- simulator.py
             |-- tunneling_simulator.py
             |-- util_functions.py
         |-- examples
             |-- examples_scipost.ipynb # notebook to reproduce figures from paper
         |-- README.md
         |-- LICENCE.md
+        |-- CITATION.cff
```

### Comparing `QDarts-1.0.1/QDarts.egg-info/PKG-INFO` & `QDarts-1.0.2/QDarts.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QDarts
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package for simulating realistic quantum dot arrays and their charge transitions.
 Author-email: Jan Krzywda <j.a.krzywda@liacs.leidenuniv.nl>, Evert van Nieuwenburg <e.p.l.van.nieuwenburg@liacs.leidenuniv.nl>, Oswin Krause <oswin.krause@di.ku.dk>
 Project-URL: Homepage, https://github.com/condensedAI/QDarts
 Project-URL: Issues, https://github.com/condensedAI/QDarts
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,28 +27,25 @@
 
 ## Installation
 The package supports Python 3.6 and later. To install the package, run the following command:
 
     pip install qdarts
 
 ## Manuscript
-The package is based on the manuscript by [Krause et al., QDarts: Efficient Quantum Dot array transition simulator; The transition finding in presence of finite tunnel couplings, non-constant charging energies and sensor dots](). The manuscript has been submitted to the SciPost Physics Codebases.
+The package is based on the manuscript by [Krzywda et al., QDarts: A Quantum Dot Array Transition Simulator for finding charge transitions in the presence of finite tunnel couplings, non-constant charging energies and sensor dots](). The manuscript has been submitted to the SciPost Physics Codebases.
 
 ## Examples
 The package provides a simple example to demonstrate the usage of the package. The example is available in the examples qatpack/examples folder. The example demonstrates the simulation of a quantum dot array with sensor dots, tunnel couplings, and non-constant charging energy. 
 
-As a proof of principle, in the example we reconstruct the figure from the paper [Neyens et al.](https://journals.aps.org/prapplied/abstract/10.1103/PhysRevApplied.12.064049z), which shows the measured charge conductance signal from two sensor dots, which detect simultanous four-dot transition in the quantum dot array. The figure, visible below, has been computed in about a minute on tabletop computer.
+As a proof of principle, in the example we reconstruct the figure from the paper [Neyens et al.](https://journals.aps.org/prapplied/abstract/10.1103/PhysRevApplied.12.064049z), which shows the measured charge conductance signal from two sensor dots, which detect simultanous four-dot transition in the quantum dot array. The figure, visible below, has been computed in about a minute on a standard laptop.
 
 <p align="center">
-  <img src="qdarts/figures/neyens.png" />
+  <img src="examples/figures/neyens.png" />
 <p/>
-using several line prompt:
     
-    
-
 ## Files in this repository
     qdarts
         |-- qdarts
             |-- model.py
             |-- noise_processes.py
             |-- experiment.py
             |-- plotting.py
@@ -56,7 +53,8 @@
             |-- simulator.py
             |-- tunneling_simulator.py
             |-- util_functions.py
         |-- examples
             |-- examples_scipost.ipynb # notebook to reproduce figures from paper
         |-- README.md
         |-- LICENCE.md
+        |-- CITATION.cff
```

### Comparing `QDarts-1.0.1/README.md` & `QDarts-1.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -13,36 +13,34 @@
 
 ## Installation
 The package supports Python 3.6 and later. To install the package, run the following command:
 
     pip install qdarts
 
 ## Manuscript
-The package is based on the manuscript by [Krause et al., QDarts: Efficient Quantum Dot array transition simulator; The transition finding in presence of finite tunnel couplings, non-constant charging energies and sensor dots](). The manuscript has been submitted to the SciPost Physics Codebases.
+The package is based on the manuscript by [Krzywda et al., QDarts: A Quantum Dot Array Transition Simulator for finding charge transitions in the presence of finite tunnel couplings, non-constant charging energies and sensor dots](). The manuscript has been submitted to the SciPost Physics Codebases.
 
 ## Examples
 The package provides a simple example to demonstrate the usage of the package. The example is available in the examples qatpack/examples folder. The example demonstrates the simulation of a quantum dot array with sensor dots, tunnel couplings, and non-constant charging energy. 
 
-As a proof of principle, in the example we reconstruct the figure from the paper [Neyens et al.](https://journals.aps.org/prapplied/abstract/10.1103/PhysRevApplied.12.064049z), which shows the measured charge conductance signal from two sensor dots, which detect simultanous four-dot transition in the quantum dot array. The figure, visible below, has been computed in about a minute on tabletop computer.
+As a proof of principle, in the example we reconstruct the figure from the paper [Neyens et al.](https://journals.aps.org/prapplied/abstract/10.1103/PhysRevApplied.12.064049z), which shows the measured charge conductance signal from two sensor dots, which detect simultanous four-dot transition in the quantum dot array. The figure, visible below, has been computed in about a minute on a standard laptop.
 
 <p align="center">
-  <img src="qdarts/figures/neyens.png" />
+  <img src="examples/figures/neyens.png" />
 <p/>
-using several line prompt:
     
-    
-
 ## Files in this repository
     qdarts
         |-- qdarts
             |-- model.py
             |-- noise_processes.py
             |-- experiment.py
             |-- plotting.py
             |-- polytope.py 
             |-- simulator.py
             |-- tunneling_simulator.py
             |-- util_functions.py
         |-- examples
             |-- examples_scipost.ipynb # notebook to reproduce figures from paper
         |-- README.md
-        |-- LICENCE.md
+        |-- LICENCE.md
+        |-- CITATION.cff
```

### Comparing `QDarts-1.0.1/pyproject.toml` & `QDarts-1.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "QDarts"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Jan Krzywda", email="j.a.krzywda@liacs.leidenuniv.nl" },
   { name="Evert van Nieuwenburg", email="e.p.l.van.nieuwenburg@liacs.leidenuniv.nl" },
   { name="Oswin Krause", email="oswin.krause@di.ku.dk" },
 ]
 description = "A package for simulating realistic quantum dot arrays and their charge transitions."
 readme = "README.md"
```

### Comparing `QDarts-1.0.1/qdarts/experiment.py` & `QDarts-1.0.2/qdarts/experiment.py`

 * *Files identical despite different names*

### Comparing `QDarts-1.0.1/qdarts/model.py` & `QDarts-1.0.2/qdarts/model.py`

 * *Files identical despite different names*

### Comparing `QDarts-1.0.1/qdarts/noise_processes.py` & `QDarts-1.0.2/qdarts/noise_processes.py`

 * *Files identical despite different names*

### Comparing `QDarts-1.0.1/qdarts/plotting.py` & `QDarts-1.0.2/qdarts/plotting.py`

 * *Files identical despite different names*

### Comparing `QDarts-1.0.1/qdarts/polytope.py` & `QDarts-1.0.2/qdarts/polytope.py`

 * *Files identical despite different names*

### Comparing `QDarts-1.0.1/qdarts/simulator.py` & `QDarts-1.0.2/qdarts/simulator.py`

 * *Files identical despite different names*

### Comparing `QDarts-1.0.1/qdarts/tunneling_simulator.py` & `QDarts-1.0.2/qdarts/tunneling_simulator.py`

 * *Files identical despite different names*

### Comparing `QDarts-1.0.1/qdarts/util_functions.py` & `QDarts-1.0.2/qdarts/util_functions.py`

 * *Files identical despite different names*

