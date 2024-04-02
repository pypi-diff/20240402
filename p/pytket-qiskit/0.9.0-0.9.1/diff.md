# Comparing `tmp/pytket-qiskit-0.9.0.tar.gz` & `tmp/pytket-qiskit-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytket-qiskit-0.9.0.tar", last modified: Thu Apr  1 10:57:59 2021, max compression
+gzip compressed data, was "pytket-qiskit-0.9.1.tar", last modified: Fri Apr 16 11:45:39 2021, max compression
```

## Comparing `pytket-qiskit-0.9.0.tar` & `pytket-qiskit-0.9.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 10:57:59.916303 pytket-qiskit-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-04-01 10:54:45.000000 pytket-qiskit-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1791 2021-04-01 10:57:59.916303 pytket-qiskit-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      732 2021-04-01 10:54:45.000000 pytket-qiskit-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       69 2021-04-01 10:54:45.000000 pytket-qiskit-0.9.0/_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 10:57:59.908303 pytket-qiskit-0.9.0/pytket/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 10:57:59.908303 pytket-qiskit-0.9.0/pytket/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 10:57:59.912303 pytket-qiskit-0.9.0/pytket/extensions/qiskit/
--rw-r--r--   0 runner    (1001) docker     (121)     1118 2021-04-01 10:54:45.000000 pytket-qiskit-0.9.0/pytket/extensions/qiskit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       69 2021-04-01 10:57:59.000000 pytket-qiskit-0.9.0/pytket/extensions/qiskit/_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 10:57:59.912303 pytket-qiskit-0.9.0/pytket/extensions/qiskit/backends/
--rw-r--r--   0 runner    (1001) docker     (121)      838 2021-04-01 10:54:45.000000 pytket-qiskit-0.9.0/pytket/extensions/qiskit/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    25874 2021-04-01 10:54:45.000000 pytket-qiskit-0.9.0/pytket/extensions/qiskit/backends/aer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1976 2021-04-01 10:54:45.000000 pytket-qiskit-0.9.0/pytket/extensions/qiskit/backends/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    14180 2021-04-01 10:54:45.000000 pytket-qiskit-0.9.0/pytket/extensions/qiskit/backends/ibm.py
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2021-04-01 10:54:45.000000 pytket-qiskit-0.9.0/pytket/extensions/qiskit/backends/ibm_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2376 2021-04-01 10:54:45.000000 pytket-qiskit-0.9.0/pytket/extensions/qiskit/backends/ibmq_emulator.py
--rw-r--r--   0 runner    (1001) docker     (121)    21316 2021-04-01 10:54:45.000000 pytket-qiskit-0.9.0/pytket/extensions/qiskit/qiskit_convert.py
--rw-r--r--   0 runner    (1001) docker     (121)     4113 2021-04-01 10:54:45.000000 pytket-qiskit-0.9.0/pytket/extensions/qiskit/result_convert.py
--rw-r--r--   0 runner    (1001) docker     (121)     5436 2021-04-01 10:54:45.000000 pytket-qiskit-0.9.0/pytket/extensions/qiskit/tket_backend.py
--rw-r--r--   0 runner    (1001) docker     (121)     3470 2021-04-01 10:54:45.000000 pytket-qiskit-0.9.0/pytket/extensions/qiskit/tket_job.py
--rw-r--r--   0 runner    (1001) docker     (121)     4121 2021-04-01 10:54:45.000000 pytket-qiskit-0.9.0/pytket/extensions/qiskit/tket_pass.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 10:57:59.916303 pytket-qiskit-0.9.0/pytket_qiskit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1791 2021-04-01 10:57:59.000000 pytket-qiskit-0.9.0/pytket_qiskit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      810 2021-04-01 10:57:59.000000 pytket-qiskit-0.9.0/pytket_qiskit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-01 10:57:59.000000 pytket-qiskit-0.9.0/pytket_qiskit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-01 10:57:59.000000 pytket-qiskit-0.9.0/pytket_qiskit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       29 2021-04-01 10:57:59.000000 pytket-qiskit-0.9.0/pytket_qiskit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-04-01 10:57:59.000000 pytket-qiskit-0.9.0/pytket_qiskit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-04-01 10:57:59.916303 pytket-qiskit-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2095 2021-04-01 10:54:45.000000 pytket-qiskit-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-16 11:45:39.453254 pytket-qiskit-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2021-04-16 11:45:32.000000 pytket-qiskit-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1791 2021-04-16 11:45:39.453254 pytket-qiskit-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      732 2021-04-16 11:45:32.000000 pytket-qiskit-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2021-04-16 11:45:32.000000 pytket-qiskit-0.9.1/_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-16 11:45:39.449253 pytket-qiskit-0.9.1/pytket/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-16 11:45:39.449253 pytket-qiskit-0.9.1/pytket/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-16 11:45:39.453254 pytket-qiskit-0.9.1/pytket/extensions/qiskit/
+-rw-r--r--   0 runner    (1001) docker     (121)     1118 2021-04-16 11:45:32.000000 pytket-qiskit-0.9.1/pytket/extensions/qiskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2021-04-16 11:45:39.000000 pytket-qiskit-0.9.1/pytket/extensions/qiskit/_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-16 11:45:39.453254 pytket-qiskit-0.9.1/pytket/extensions/qiskit/backends/
+-rw-r--r--   0 runner    (1001) docker     (121)      838 2021-04-16 11:45:32.000000 pytket-qiskit-0.9.1/pytket/extensions/qiskit/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25809 2021-04-16 11:45:32.000000 pytket-qiskit-0.9.1/pytket/extensions/qiskit/backends/aer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1976 2021-04-16 11:45:32.000000 pytket-qiskit-0.9.1/pytket/extensions/qiskit/backends/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14180 2021-04-16 11:45:32.000000 pytket-qiskit-0.9.1/pytket/extensions/qiskit/backends/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1071 2021-04-16 11:45:32.000000 pytket-qiskit-0.9.1/pytket/extensions/qiskit/backends/ibm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2376 2021-04-16 11:45:32.000000 pytket-qiskit-0.9.1/pytket/extensions/qiskit/backends/ibmq_emulator.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21316 2021-04-16 11:45:32.000000 pytket-qiskit-0.9.1/pytket/extensions/qiskit/qiskit_convert.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4113 2021-04-16 11:45:32.000000 pytket-qiskit-0.9.1/pytket/extensions/qiskit/result_convert.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5436 2021-04-16 11:45:32.000000 pytket-qiskit-0.9.1/pytket/extensions/qiskit/tket_backend.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3470 2021-04-16 11:45:32.000000 pytket-qiskit-0.9.1/pytket/extensions/qiskit/tket_job.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4121 2021-04-16 11:45:32.000000 pytket-qiskit-0.9.1/pytket/extensions/qiskit/tket_pass.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-16 11:45:39.453254 pytket-qiskit-0.9.1/pytket_qiskit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1791 2021-04-16 11:45:39.000000 pytket-qiskit-0.9.1/pytket_qiskit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      810 2021-04-16 11:45:39.000000 pytket-qiskit-0.9.1/pytket_qiskit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-16 11:45:39.000000 pytket-qiskit-0.9.1/pytket_qiskit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-16 11:45:39.000000 pytket-qiskit-0.9.1/pytket_qiskit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2021-04-16 11:45:39.000000 pytket-qiskit-0.9.1/pytket_qiskit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-04-16 11:45:39.000000 pytket-qiskit-0.9.1/pytket_qiskit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-04-16 11:45:39.453254 pytket-qiskit-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2095 2021-04-16 11:45:32.000000 pytket-qiskit-0.9.1/setup.py
```

### Comparing `pytket-qiskit-0.9.0/PKG-INFO` & `pytket-qiskit-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytket-qiskit
-Version: 0.9.0
+Version: 0.9.1
 Summary: Extension for pytket, providing translation to and from the Qiskit framework
 Home-page: https://github.com/CQCL/pytket-extensions
 Author: Will Simmons
 Author-email: will.simmons@cambridgequantum.com
 License: Apache 2
 Description: # pytket-qiskit
```

### Comparing `pytket-qiskit-0.9.0/README.md` & `pytket-qiskit-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pytket-qiskit-0.9.0/pytket/extensions/qiskit/__init__.py` & `pytket-qiskit-0.9.1/pytket/extensions/qiskit/__init__.py`

 * *Files identical despite different names*

### Comparing `pytket-qiskit-0.9.0/pytket/extensions/qiskit/backends/__init__.py` & `pytket-qiskit-0.9.1/pytket/extensions/qiskit/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `pytket-qiskit-0.9.0/pytket/extensions/qiskit/backends/aer.py` & `pytket-qiskit-0.9.1/pytket/extensions/qiskit/backends/aer.py`

 * *Files 2% similar despite different names*

```diff
@@ -660,16 +660,14 @@
     characterisation["GenericTwoQubitQErrors"] = generic_2q_qerrors_dict
     characterisation["Architecture"] = Architecture(coupling_map)
 
     return characterisation
 
 
 def _sparse_to_qiskit_pauli(pauli: QubitPauliString, n_qubits: int) -> qk_Pauli:
-    empty = np.zeros(n_qubits)
-    q_pauli = qk_Pauli(empty, empty)
+    x = [False] * n_qubits
+    z = [False] * n_qubits
     for q, p in pauli.to_dict().items():
         i = _default_q_index(q)
-        if p in (Pauli.X, Pauli.Y):
-            q_pauli._x[i] = True
-        if p in (Pauli.Z, Pauli.Y):
-            q_pauli._z[i] = True
-    return q_pauli
+        z[i] = p in (Pauli.Z, Pauli.Y)
+        x[i] = p in (Pauli.X, Pauli.Y)
+    return qk_Pauli((z, x))
```

### Comparing `pytket-qiskit-0.9.0/pytket/extensions/qiskit/backends/config.py` & `pytket-qiskit-0.9.1/pytket/extensions/qiskit/backends/config.py`

 * *Files identical despite different names*

### Comparing `pytket-qiskit-0.9.0/pytket/extensions/qiskit/backends/ibm.py` & `pytket-qiskit-0.9.1/pytket/extensions/qiskit/backends/ibm.py`

 * *Files identical despite different names*

### Comparing `pytket-qiskit-0.9.0/pytket/extensions/qiskit/backends/ibm_utils.py` & `pytket-qiskit-0.9.1/pytket/extensions/qiskit/backends/ibm_utils.py`

 * *Files identical despite different names*

### Comparing `pytket-qiskit-0.9.0/pytket/extensions/qiskit/backends/ibmq_emulator.py` & `pytket-qiskit-0.9.1/pytket/extensions/qiskit/backends/ibmq_emulator.py`

 * *Files identical despite different names*

### Comparing `pytket-qiskit-0.9.0/pytket/extensions/qiskit/qiskit_convert.py` & `pytket-qiskit-0.9.1/pytket/extensions/qiskit/qiskit_convert.py`

 * *Files identical despite different names*

### Comparing `pytket-qiskit-0.9.0/pytket/extensions/qiskit/result_convert.py` & `pytket-qiskit-0.9.1/pytket/extensions/qiskit/result_convert.py`

 * *Files identical despite different names*

### Comparing `pytket-qiskit-0.9.0/pytket/extensions/qiskit/tket_backend.py` & `pytket-qiskit-0.9.1/pytket/extensions/qiskit/tket_backend.py`

 * *Files identical despite different names*

### Comparing `pytket-qiskit-0.9.0/pytket/extensions/qiskit/tket_job.py` & `pytket-qiskit-0.9.1/pytket/extensions/qiskit/tket_job.py`

 * *Files identical despite different names*

### Comparing `pytket-qiskit-0.9.0/pytket/extensions/qiskit/tket_pass.py` & `pytket-qiskit-0.9.1/pytket/extensions/qiskit/tket_pass.py`

 * *Files identical despite different names*

### Comparing `pytket-qiskit-0.9.0/pytket_qiskit.egg-info/PKG-INFO` & `pytket-qiskit-0.9.1/pytket_qiskit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytket-qiskit
-Version: 0.9.0
+Version: 0.9.1
 Summary: Extension for pytket, providing translation to and from the Qiskit framework
 Home-page: https://github.com/CQCL/pytket-extensions
 Author: Will Simmons
 Author-email: will.simmons@cambridgequantum.com
 License: Apache 2
 Description: # pytket-qiskit
```

### Comparing `pytket-qiskit-0.9.0/pytket_qiskit.egg-info/SOURCES.txt` & `pytket-qiskit-0.9.1/pytket_qiskit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytket-qiskit-0.9.0/setup.py` & `pytket-qiskit-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     license="Apache 2",
     packages=find_namespace_packages(include=["pytket.*"]),
     include_package_data=True,
     install_requires=[
         "pytket ~= 0.9.0",
-        "qiskit ~= 0.24.0",
+        "qiskit ~= 0.25.0",
     ],
     classifiers=[
         "Environment :: Console",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "License :: Other/Proprietary License",
```

