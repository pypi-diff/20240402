# Comparing `tmp/bluequbit-0.6.0b1.tar.gz` & `tmp/bluequbit-0.7.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluequbit-0.6.0b1.tar", last modified: Thu Oct 19 16:09:41 2023, max compression
+gzip compressed data, was "bluequbit-0.7.0b1.tar", last modified: Tue Apr  2 09:21:16 2024, max compression
```

## Comparing `bluequbit-0.6.0b1.tar` & `bluequbit-0.7.0b1.tar`

### file list

```diff
@@ -1,59 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 16:09:41.541600 bluequbit-0.6.0b1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2023-10-19 16:09:41.541600 bluequbit-0.6.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 16:09:41.537600 bluequbit-0.6.0b1/bluequbit/
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/bluequbit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 16:09:41.537600 bluequbit-0.6.0b1/bluequbit/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/bluequbit/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/bluequbit/api/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4381 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/bluequbit/backend_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    11692 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/bluequbit/bluequbit_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/bluequbit/check_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/bluequbit/circuit_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/bluequbit/estimate_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/bluequbit/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/bluequbit/http_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/bluequbit/job_metadata_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7361 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/bluequbit/job_result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 16:09:41.537600 bluequbit-0.6.0b1/bluequbit/library/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/bluequbit/library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 16:09:41.537600 bluequbit-0.6.0b1/bluequbit/library/circuits/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/bluequbit/library/circuits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/bluequbit/library/circuits/bell_pair.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/bluequbit/library/circuits/coin_toss.py
--rw-r--r--   0 runner    (1001) docker     (127)     7484 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/bluequbit/library/circuits/draper_adder.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/bluequbit/library/circuits/ghz.py
--rw-r--r--   0 runner    (1001) docker     (127)     3900 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/bluequbit/library/circuits/multi_adder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/bluequbit/library/circuits/qft.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/bluequbit/library/circuits/random_circuit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/bluequbit/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/bluequbit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 16:09:41.537600 bluequbit-0.6.0b1/bluequbit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2023-10-19 16:09:41.000000 bluequbit-0.6.0b1/bluequbit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2023-10-19 16:09:41.000000 bluequbit-0.6.0b1/bluequbit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-19 16:09:41.000000 bluequbit-0.6.0b1/bluequbit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-10-19 16:09:41.000000 bluequbit-0.6.0b1/bluequbit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-10-19 16:09:41.000000 bluequbit-0.6.0b1/bluequbit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-19 16:09:41.541600 bluequbit-0.6.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      837 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 16:09:41.541600 bluequbit-0.6.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      838 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/tests/test_basic_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/tests/test_basic_large_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4882 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/tests/test_batch_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/tests/test_cancel_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/tests/test_circuit_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4782 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/tests/test_complex_circuits.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/tests/test_count_wrong.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/tests/test_get_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4470 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/tests/test_gpu_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/tests/test_job_estimate.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/tests/test_ok.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/tests/test_pauli_sum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/tests/test_quantum_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/tests/test_stress_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2023-10-19 16:09:29.000000 bluequbit-0.6.0b1/tests/test_very_large_job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:16.556703 bluequbit-0.7.0b1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-02 09:21:12.000000 bluequbit-0.7.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-02 09:21:12.000000 bluequbit-0.7.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-02 09:21:16.556703 bluequbit-0.7.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-02 09:21:12.000000 bluequbit-0.7.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:16.552703 bluequbit-0.7.0b1/bluequbit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-02 09:21:12.000000 bluequbit-0.7.0b1/bluequbit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:16.552703 bluequbit-0.7.0b1/bluequbit/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:12.000000 bluequbit-0.7.0b1/bluequbit/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-02 09:21:12.000000 bluequbit-0.7.0b1/bluequbit/api/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-04-02 09:21:12.000000 bluequbit-0.7.0b1/bluequbit/backend_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13154 2024-04-02 09:21:12.000000 bluequbit-0.7.0b1/bluequbit/bluequbit_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-02 09:21:12.000000 bluequbit-0.7.0b1/bluequbit/check_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-04-02 09:21:12.000000 bluequbit-0.7.0b1/bluequbit/circuit_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-04-02 09:21:12.000000 bluequbit-0.7.0b1/bluequbit/computation_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-02 09:21:12.000000 bluequbit-0.7.0b1/bluequbit/estimate_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-02 09:21:12.000000 bluequbit-0.7.0b1/bluequbit/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-02 09:21:12.000000 bluequbit-0.7.0b1/bluequbit/http_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-02 09:21:12.000000 bluequbit-0.7.0b1/bluequbit/job_metadata_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-04-02 09:21:12.000000 bluequbit-0.7.0b1/bluequbit/job_result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:16.552703 bluequbit-0.7.0b1/bluequbit/library/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-02 09:21:12.000000 bluequbit-0.7.0b1/bluequbit/library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:16.556703 bluequbit-0.7.0b1/bluequbit/library/circuits/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-02 09:21:12.000000 bluequbit-0.7.0b1/bluequbit/library/circuits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-02 09:21:12.000000 bluequbit-0.7.0b1/bluequbit/library/circuits/bell_pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-02 09:21:12.000000 bluequbit-0.7.0b1/bluequbit/library/circuits/coin_toss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7484 2024-04-02 09:21:12.000000 bluequbit-0.7.0b1/bluequbit/library/circuits/draper_adder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-02 09:21:12.000000 bluequbit-0.7.0b1/bluequbit/library/circuits/ghz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-04-02 09:21:12.000000 bluequbit-0.7.0b1/bluequbit/library/circuits/multi_adder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-02 09:21:12.000000 bluequbit-0.7.0b1/bluequbit/library/circuits/qft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-02 09:21:12.000000 bluequbit-0.7.0b1/bluequbit/library/circuits/random_circuit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:16.556703 bluequbit-0.7.0b1/bluequbit/library/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-02 09:21:12.000000 bluequbit-0.7.0b1/bluequbit/library/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-04-02 09:21:12.000000 bluequbit-0.7.0b1/bluequbit/library/helpers/data_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:16.556703 bluequbit-0.7.0b1/bluequbit/pennylane_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-02 09:21:12.000000 bluequbit-0.7.0b1/bluequbit/pennylane_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-02 09:21:12.000000 bluequbit-0.7.0b1/bluequbit/pennylane_plugin/bluequbit_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9817 2024-04-02 09:21:12.000000 bluequbit-0.7.0b1/bluequbit/pennylane_plugin/bluequbit_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-02 09:21:12.000000 bluequbit-0.7.0b1/bluequbit/pennylane_plugin/bluequbit_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-02 09:21:12.000000 bluequbit-0.7.0b1/bluequbit/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-02 09:21:12.000000 bluequbit-0.7.0b1/bluequbit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:16.556703 bluequbit-0.7.0b1/bluequbit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-02 09:21:16.000000 bluequbit-0.7.0b1/bluequbit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-02 09:21:16.000000 bluequbit-0.7.0b1/bluequbit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 09:21:16.000000 bluequbit-0.7.0b1/bluequbit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-02 09:21:16.000000 bluequbit-0.7.0b1/bluequbit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-02 09:21:16.000000 bluequbit-0.7.0b1/bluequbit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-02 09:21:16.000000 bluequbit-0.7.0b1/bluequbit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-02 09:21:12.000000 bluequbit-0.7.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-02 09:21:12.000000 bluequbit-0.7.0b1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 09:21:16.556703 bluequbit-0.7.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-02 09:21:12.000000 bluequbit-0.7.0b1/setup.py
```

### Comparing `bluequbit-0.6.0b1/LICENSE` & `bluequbit-0.7.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `bluequbit-0.6.0b1/PKG-INFO` & `bluequbit-0.7.0b1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: bluequbit
-Version: 0.6.0b1
+Version: 0.7.0b1
 Summary: Python SDK to BlueQubit app
 Author: BlueQubit
 Author-email: hovnatan@bluequbit.io
 License: Apache 2.0
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests~=2.28
 Requires-Dist: python-dateutil~=2.8
 Requires-Dist: numpy~=1.21
 Requires-Dist: packaging
 
@@ -38,15 +38,35 @@
 
     job_result = bq_client.run(qc_qiskit, job_name="testing_1")
 
     state_vector = job_result.get_statevector() 
     # returns a NumPy array of [0. +0.j 0. +0.j 0.70710677+0.j 0.70710677+0.j]
 ```
 
-The packages is tested extensively on Python 3.8.
+4. An example of how to run a Pennylane circuit using the SDK:
+
+To use the Pennylane plugin, you must have pennylane~=0.35.1 version installed. It requires
+Python 3.9, but we recommend using Python 3.10 . Make sure your Python version is not older
+```
+    import pennylane as qml
+    from pennylane import numpy as np
+    
+    dev = qml.device('bluequbit.cpu', wires=1, token="<token>")
+    
+    @qml.qnode(dev)
+    def circuit(angle):
+        qml.RY(angle, wires=0)
+        return qml.probs(wires=0)
+    
+    
+    probabilities = circuit(np.pi / 4)
+    # returns a NumPy array of [0.85355339 0.14644661]
+```
+
+The packages is tested extensively on Python 3.10.
 
 ## Full reference
 
 Please find detailed reference at https://app.bluequbit.io/sdk-docs.
 
 ## Questions and Issues
```

### Comparing `bluequbit-0.6.0b1/README.md` & `bluequbit-0.7.0b1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -25,15 +25,35 @@
 
     job_result = bq_client.run(qc_qiskit, job_name="testing_1")
 
     state_vector = job_result.get_statevector() 
     # returns a NumPy array of [0. +0.j 0. +0.j 0.70710677+0.j 0.70710677+0.j]
 ```
 
-The packages is tested extensively on Python 3.8.
+4. An example of how to run a Pennylane circuit using the SDK:
+
+To use the Pennylane plugin, you must have pennylane~=0.35.1 version installed. It requires
+Python 3.9, but we recommend using Python 3.10 . Make sure your Python version is not older
+```
+    import pennylane as qml
+    from pennylane import numpy as np
+    
+    dev = qml.device('bluequbit.cpu', wires=1, token="<token>")
+    
+    @qml.qnode(dev)
+    def circuit(angle):
+        qml.RY(angle, wires=0)
+        return qml.probs(wires=0)
+    
+    
+    probabilities = circuit(np.pi / 4)
+    # returns a NumPy array of [0.85355339 0.14644661]
+```
+
+The packages is tested extensively on Python 3.10.
 
 ## Full reference
 
 Please find detailed reference at https://app.bluequbit.io/sdk-docs.
 
 ## Questions and Issues
```

### Comparing `bluequbit-0.6.0b1/bluequbit/__init__.py` & `bluequbit-0.7.0b1/bluequbit/__init__.py`

 * *Files identical despite different names*

### Comparing `bluequbit-0.6.0b1/bluequbit/api/jobs.py` & `bluequbit-0.7.0b1/bluequbit/api/jobs.py`

 * *Files identical despite different names*

### Comparing `bluequbit-0.6.0b1/bluequbit/backend_connection.py` & `bluequbit-0.7.0b1/bluequbit/backend_connection.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,114 +1,100 @@
 import json
 import logging
 import os
 from pathlib import Path
 
-from .exceptions import BQAPIError, BQError, BQUnauthorizedAccessError
+from .exceptions import AUTH_ERROR_MESSAGE, BQAPIError, BQUnauthorizedAccessError
 from .http_utils import request_retriable
 from .version import __version__
 
 logger = logging.getLogger("bluequbit-python-sdk")
 
 
 class BackendConnection:
     def __init__(self, api_token=None):
+        super().__init__()
         config_dir = Path.home() / ".config" / "bluequbit"
         config_location = config_dir / "config.json"
 
         main_endpoint_from_config_file = None
         ssl_verify_from_config_file = None
         token_from_env_variable = os.environ.get("BLUEQUBIT_API_TOKEN")
 
         if config_location.is_file():
             with config_location.open(encoding="utf-8") as f:
                 config = json.load(f)
             main_endpoint_from_config_file = config.get("main_endpoint")
             ssl_verify_from_config_file = config.get("ssl_verify")
-
+        self._authenticated = None
         if api_token is None:
             if token_from_env_variable is None:
-                raise BQError(
-                    "Please specify an API token to init(<your-api-token>) or have API"
-                    " token set in BLUEQUBIT_API_TOKEN environment variable. You can"
-                    " find your API token once you log in to https://app.bluequbit.io",
-                )
+                logger.warning(AUTH_ERROR_MESSAGE)
+                self._authenticated = False
             api_token = token_from_env_variable
 
-        self._api_config = {
+        api_config = {
             "token": api_token,
             "main_endpoint": (
                 "https://app.bluequbit.io/api/v1"
                 if main_endpoint_from_config_file is None
                 else main_endpoint_from_config_file
             ),
             "ssl_verify": (
                 True
                 if ssl_verify_from_config_file is None
                 else ssl_verify_from_config_file
             ),
         }
 
-        try:
-            self._token = self._api_config["token"]
-        except KeyError:
-            raise BQError(
-                "Incorrect config file: 'token' key is not present in the config"
-                f" file {config_location}.",
-            ) from None
+        self._token = api_token
 
         self._default_headers = {
             "Authorization": f"SDK {self._token}",
             "Connection": "close",
             "User-Agent": f"BlueQubit SDK {__version__}",
         }
 
         self._main_endpoint = "https://app.bluequbit.io/api/v1"
-        if (
-            "main_endpoint" in self._api_config
-            and self._main_endpoint != self._api_config["main_endpoint"]
-        ):
-            self._main_endpoint = self._api_config["main_endpoint"]
+        if self._main_endpoint != api_config["main_endpoint"]:
+            self._main_endpoint = api_config["main_endpoint"]
             logger.warning("Using custom endpoint %s", self._main_endpoint)
         self._verify = True
-        if "ssl_verify" in self._api_config:
-            self._verify = self._api_config["ssl_verify"]
+        if "ssl_verify" in api_config:
+            self._verify = api_config["ssl_verify"]
         self._session = None
-        self._authenticated = False
-        response = self.send_request(
-            req_type="GET",
-            path="/jobs",
-            params={"limit": 1},
-            authentication_request=True,
-        )
-
-        if response.ok:
-            self._authenticated = True
-        elif response.status_code == 401:
-            raise BQUnauthorizedAccessError
-        else:
-            raise BQAPIError(
-                response.status_code, f"Couldn't reach BlueQubit {response.text}."
-            )
+        if self._authenticated is not False:
+            try:
+                response = self.send_request(
+                    req_type="GET",
+                    path="/jobs",
+                    params={"limit": 1},
+                )
+                if response.ok:
+                    self._authenticated = True
+                else:
+                    self._authenticated = False
+                    raise BQAPIError(
+                        response.status_code,
+                        f"Couldn't reach BlueQubit {response.text}.",
+                    )
+            except BQUnauthorizedAccessError:
+                self._authenticated = False
+                logger.warning(AUTH_ERROR_MESSAGE)
+                return
 
     def send_request(
         self,
         req_type,
         path,
         params=None,
         data=None,
         json_req=None,
         headers=None,
-        authentication_request=False,
     ):
-        if not authentication_request and not self._authenticated:
-            raise BQError(
-                "BQClient was not initialized. Please provide correct API token to"
-                " BQClient(<token>).",
-            )
         url = self._main_endpoint + path
 
         if params is not None:
             for key, value in params.items():
                 if isinstance(value, str):
                     params[key] = value.replace("\\", "\\\\")
                 if isinstance(value, list):
```

### Comparing `bluequbit-0.6.0b1/bluequbit/bluequbit_client.py` & `bluequbit-0.7.0b1/bluequbit/bluequbit_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,20 +8,23 @@
 import time
 from typing import TYPE_CHECKING, Any, List, Tuple, Union
 
 from . import job_metadata_constants
 from .api import jobs
 from .backend_connection import BackendConnection
 from .check_version import check_version
+from .circuit_serialization import isa_qiskit_circuit
+from .computation_local import run_circuit_cirq, run_circuit_qiskit
 from .estimate_result import EstimateResult
 from .exceptions import (
     BQBatchJobsLimitExceededError,
     BQJobCouldNotCancelError,
     BQJobInvalidDeviceTypeError,
     BQJobNotCompleteError,
+    BQSDKUsageError,
 )
 from .job_result import JobResult
 from .version import __version__
 
 if TYPE_CHECKING:
     import datetime
 
@@ -33,22 +36,54 @@
 
 logger = logging.getLogger("bluequbit-python-sdk")
 
 
 _SHOTS_LIMIT_NON_QPU = 131072
 
 
+def _run_circuits_local(circuits, shots):
+    first_circuit = circuits[0] if isinstance(circuits, list) else circuits
+    try:
+        from deqart_internal.computation import run_circuit_object
+
+        try:
+            import cuquantum  # noqa: F401
+
+            device_type = "gpu"
+        except ImportError:
+            # Not in a cuQuantum Appliance
+            device_type = "cpu"
+        print(f"Using cuQuantum cuStateVec with device type {device_type}")
+        if isinstance(circuits, list):
+            return [run_circuit_object(c, device_type, shots=shots) for c in circuits]
+        return run_circuit_object(circuits, device_type, shots=shots)
+    except (ImportError, ModuleNotFoundError):
+        if isa_qiskit_circuit(first_circuit):
+            fn = run_circuit_qiskit
+        elif str(type(first_circuit)) == "<class 'cirq.circuits.circuit.Circuit'>":
+            fn = run_circuit_cirq
+        else:
+            raise BQSDKUsageError(
+                f"Circuit type not yet supported for {first_circuit}"
+            ) from None
+
+        if isinstance(circuits, list):
+            return [fn(c, shots=shots) for c in circuits]
+        return fn(circuits, shots=shots)
+
+
 class BQClient:
     """Client for managing jobs on BlueQubit platform.
 
     :param api_token: API token of the user. If ``None``, the token will be looked
                       in the environment variable BLUEQUBIT_API_TOKEN.
     """
 
     def __init__(self, api_token: str | None = None):
+        super().__init__()
         if os.environ.get("BLUEQUBIT_TESTING") is None:
             with contextlib.suppress(Exception):
                 check_version(__version__)
 
         self._backend_connection = BackendConnection(api_token)
 
     def name(self):
@@ -101,15 +136,15 @@
         pauli_sum: PauliSumT | list[PauliSumT] | None = None,
     ) -> JobResult | list[JobResult]:
         """Submit a job to run on BlueQubit platform
 
         :param circuits: quantum circuit or list of circuits
         :type circuits: Cirq, Qiskit, list
         :param device: device on which to run the circuit. Can be one of
-                       ``"cpu"`` | ``"gpu"`` | ``"quantum"``
+                       ``"cpu"`` | ``"gpu"`` | ``"quantum"`` | ``"local"``
         :param asynchronous: if set to ``False``, wait for job completion before
                              returning. If set to ``True``, return immediately
         :param job_name: customizable job name
         :param shots: number of shots to run. If device is quantum and shots is None then
                       it is set to 1000. For non quantum devices, if None, full
                       probability distribution will be returned. For non quantum
                       devices it is limited to 131072
@@ -122,14 +157,16 @@
         if device == "quantum" and shots is None:
             shots = 1000
         elif device != "quantum" and shots is not None and shots > _SHOTS_LIMIT_NON_QPU:
             logger.warning(
                 "Number of shots is set to %s, because of limit.",
                 _SHOTS_LIMIT_NON_QPU,
             )
+        elif device == "local":
+            return _run_circuits_local(circuits, shots)
         response = jobs.submit_jobs(
             self._backend_connection,
             circuits,
             device,
             job_name,
             shots=shots,
             asynchronous=asynchronous,
```

### Comparing `bluequbit-0.6.0b1/bluequbit/check_version.py` & `bluequbit-0.7.0b1/bluequbit/check_version.py`

 * *Files identical despite different names*

### Comparing `bluequbit-0.6.0b1/bluequbit/circuit_serialization.py` & `bluequbit-0.7.0b1/bluequbit/circuit_serialization.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,25 @@
 import base64
 import io
+import pickle
+import zlib
+
+
+def isa_qiskit_circuit(qc):
+    return any(
+        str(cls) == "<class 'qiskit.circuit.quantumcircuit.QuantumCircuit'>"
+        for cls in type(qc).mro()
+    )
+
+
+def isa_pennylane_circuit(qc):
+    return str(type(qc)) == "<class 'dict'>" and any(
+        str(cls) == "<class 'pennylane.tape.qscript.QuantumScript'>"
+        for cls in type(qc.get("pennylane_circuit")).mro()
+    )
 
 
 def cirq_to_qasm2(circuit):
     import cirq
     from cirq import ops
 
     qubit_order = ops.QubitOrder.DEFAULT
@@ -42,31 +58,35 @@
         serialized = cirq.to_json(qc)
         return {"circuit_type": "Cirq", "circuit": serialized}
     elif circuit_type == "<class 'braket.circuits.circuit.Circuit'>":
         from braket.circuits.serialization import IRType
 
         serialized = qc.to_ir(IRType.OPENQASM).source
         return {"circuit_type": "Braket", "circuit": serialized}
-    elif any(
-        str(cls) == "<class 'qiskit.circuit.quantumcircuit.QuantumCircuit'>"
-        for cls in type(qc).mro()
-    ):
+    elif isa_qiskit_circuit(qc):
         from qiskit import qpy
 
         # https://qiskit.org/documentation/apidoc/qpy.html
         with io.BytesIO() as f:
             qpy.dump(qc, f)
             # Rewind back to the beginning of the "file".
             f.seek(0)
             serialized = f.read()
             # Convert to base64
             serialized = base64.b64encode(serialized)
             # Convert bytes to str
             serialized = serialized.decode("utf-8")
         return {"circuit_type": "Qiskit", "circuit": serialized}
+    elif isa_pennylane_circuit(qc):
+        return {
+            "circuit_type": "Pennylane",
+            "circuit": base64.b64encode(zlib.compress(pickle.dumps(qc))).decode(
+                "utf-8"
+            ),
+        }
     else:
         raise Exception("Unsupported circuit type", qc)
 
 
 def encode_circuit_with_fallback(qc):
     # Temporary workaround: see https://trello.com/c/0SMvJuLV/266-productofsums-issue
     encoded = encode_circuit(qc)
@@ -100,11 +120,22 @@
         with io.BytesIO(_bytes) as f:
             circuits = qpy.load(f)
             if len(circuits) != 1:
                 raise Exception(
                     f"Unexpected number of circuits: {len(circuits)}. Must be 1."
                 )
             return circuits[0]
+    elif circuit_type == "Pennylane":
+        encoded_circuit = data["circuit"]
+        decoded_bytes = base64.b64decode(encoded_circuit)
+        circuit = pickle.loads(zlib.decompress(decoded_bytes))  # noqa: S301
+        if isinstance(circuit, dict):
+            pennylane_circuit = circuit.get("pennylane_circuit")
+        else:
+            raise TypeError(
+                "the circuit must be dictionary containing pennylane_circuit"
+            )
+        return pennylane_circuit
     elif circuit_type == "Braket":
         raise Exception("Braket decoding is not yet supported.")
     else:
         raise Exception("Unsupported circuit type", circuit_type)
```

### Comparing `bluequbit-0.6.0b1/bluequbit/estimate_result.py` & `bluequbit-0.7.0b1/bluequbit/estimate_result.py`

 * *Files identical despite different names*

### Comparing `bluequbit-0.6.0b1/bluequbit/exceptions.py` & `bluequbit-0.7.0b1/bluequbit/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from . import job_metadata_constants
 
+AUTH_ERROR_MESSAGE = (
+    "BlueQubit client was not authorized. For full functionality please specify an API token to init(<your-api-token>) or have API"
+    " token set in BLUEQUBIT_API_TOKEN environment variable. You can"
+    " find your API token once you log in to https://app.bluequbit.io"
+)
+
 
 class BQError(Exception):
     def __init__(self, message="Unknown Error Message"):
         super().__init__(message)
         self.message = message
 
 
 class BQSDKUsageError(BQError):
     def __init__(self, message):
         super().__init__(message)
 
 
 class BQUnauthorizedAccessError(BQError):
     def __init__(self):
-        super().__init__(
-            "Wrong API key. You can find your API key once you log in to"
-            " https://app.bluequbit.io."
-        )
+        super().__init__(AUTH_ERROR_MESSAGE)
 
 
 class BQJobStatevectorNotAvailableError(BQError):
     def __init__(self, job_id, num_qubits, shots, pauli_sum):
         message = "Statevector is not available."
         if shots is not None and shots != 0:
             message += " Job run with shots > 0. Please use .get_counts() instead."
```

### Comparing `bluequbit-0.6.0b1/bluequbit/http_utils.py` & `bluequbit-0.7.0b1/bluequbit/http_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import logging
 import time
 
 import requests
 
+from .exceptions import BQUnauthorizedAccessError
+
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.WARNING)
 logger.addHandler(logging.StreamHandler())
 
 DEFAULT_TIMEOUT = (15.0, 300.0)
 NUMBER_OF_RETRIES = 5
 
@@ -37,14 +39,16 @@
             ]:
                 logger.warning(
                     "Retrying. Num retries: %s. HTTP status code: %s.",
                     retry_num,
                     resp.status_code,
                 )
                 return _send()
+            elif resp.status_code == 401:
+                raise BQUnauthorizedAccessError
             else:
                 resp.raise_for_status()
         except requests.ConnectTimeout as e:
             if retry_num <= NUMBER_OF_RETRIES:
                 logger.warning(
                     "Retrying. Num retries %s. ConnectTimeout: %s", retry_num, e
                 )
```

### Comparing `bluequbit-0.6.0b1/bluequbit/job_result.py` & `bluequbit-0.7.0b1/bluequbit/job_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,17 @@
 
         #: dict: top 131072 (2^17) results
         self.top_100k_results = data.get("top_100k")
 
         #: dict: top 128 results
         self.top_128_results = data.get("top_128")
 
+        #: string: pickled string of pennylane result
+        self.pennylane_result = data.get("pennylane_result")
+
         #: int: number of qubits
         self.num_qubits = data.get("num_qubits")
         self.tags = data.get("tags")
 
         #: list[tuple[str, float]]: expectation value
         self.pauli_sum = data.get("pauli_sum")
```

### Comparing `bluequbit-0.6.0b1/bluequbit/library/circuits/bell_pair.py` & `bluequbit-0.7.0b1/bluequbit/library/circuits/bell_pair.py`

 * *Files identical despite different names*

### Comparing `bluequbit-0.6.0b1/bluequbit/library/circuits/coin_toss.py` & `bluequbit-0.7.0b1/bluequbit/library/circuits/coin_toss.py`

 * *Files identical despite different names*

### Comparing `bluequbit-0.6.0b1/bluequbit/library/circuits/draper_adder.py` & `bluequbit-0.7.0b1/bluequbit/library/circuits/draper_adder.py`

 * *Files identical despite different names*

### Comparing `bluequbit-0.6.0b1/bluequbit/library/circuits/ghz.py` & `bluequbit-0.7.0b1/bluequbit/library/circuits/ghz.py`

 * *Files identical despite different names*

### Comparing `bluequbit-0.6.0b1/bluequbit/library/circuits/multi_adder.py` & `bluequbit-0.7.0b1/bluequbit/library/circuits/multi_adder.py`

 * *Files identical despite different names*

### Comparing `bluequbit-0.6.0b1/bluequbit/library/circuits/qft.py` & `bluequbit-0.7.0b1/bluequbit/library/circuits/qft.py`

 * *Files identical despite different names*

### Comparing `bluequbit-0.6.0b1/bluequbit/library/circuits/random_circuit.py` & `bluequbit-0.7.0b1/bluequbit/library/circuits/random_circuit.py`

 * *Files identical despite different names*

### Comparing `bluequbit-0.6.0b1/bluequbit/tools.py` & `bluequbit-0.7.0b1/bluequbit/tools.py`

 * *Files identical despite different names*

### Comparing `bluequbit-0.6.0b1/bluequbit.egg-info/PKG-INFO` & `bluequbit-0.7.0b1/bluequbit.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: bluequbit
-Version: 0.6.0b1
+Version: 0.7.0b1
 Summary: Python SDK to BlueQubit app
 Author: BlueQubit
 Author-email: hovnatan@bluequbit.io
 License: Apache 2.0
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests~=2.28
 Requires-Dist: python-dateutil~=2.8
 Requires-Dist: numpy~=1.21
 Requires-Dist: packaging
 
@@ -38,15 +38,35 @@
 
     job_result = bq_client.run(qc_qiskit, job_name="testing_1")
 
     state_vector = job_result.get_statevector() 
     # returns a NumPy array of [0. +0.j 0. +0.j 0.70710677+0.j 0.70710677+0.j]
 ```
 
-The packages is tested extensively on Python 3.8.
+4. An example of how to run a Pennylane circuit using the SDK:
+
+To use the Pennylane plugin, you must have pennylane~=0.35.1 version installed. It requires
+Python 3.9, but we recommend using Python 3.10 . Make sure your Python version is not older
+```
+    import pennylane as qml
+    from pennylane import numpy as np
+    
+    dev = qml.device('bluequbit.cpu', wires=1, token="<token>")
+    
+    @qml.qnode(dev)
+    def circuit(angle):
+        qml.RY(angle, wires=0)
+        return qml.probs(wires=0)
+    
+    
+    probabilities = circuit(np.pi / 4)
+    # returns a NumPy array of [0.85355339 0.14644661]
+```
+
+The packages is tested extensively on Python 3.10.
 
 ## Full reference
 
 Please find detailed reference at https://app.bluequbit.io/sdk-docs.
 
 ## Questions and Issues
```

### Comparing `bluequbit-0.6.0b1/pyproject.toml` & `bluequbit-0.7.0b1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tool.pyright]
-pythonVersion = "3.8"
+pythonVersion = "3.10"
 typeCheckingMode = "off"
 reportImportCycles = true
 reportConstantRedefinition = true
 reportMissingImport = true
 reportUnusedClass = true
 reportUnusedFunction = true
 reportUnusedVariable = true
@@ -19,32 +19,33 @@
 reportUninitializedInstanceVariable = true
 reportInvalidStringEscapeSequence = true
 
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [tool.black]
-preview = true
+preview = false
 
 [tool.codespell]
-ignore-words-list = 'Braket,braket'
+ignore-words-list = 'Braket,braket,ket'
 skip="jquery*.js,.git,./docs/build/html,./.venv,./.venv2,./.gitignore"
 check-filenames = true
 
 [tool.isort]
 profile = "black"
 skip = [".venv", ".venv2"]
 
 [tool.pytest.ini_options]
 timeout = "900"
 timeout_method = "thread"
 
 [tool.ruff]
+preview = false
 # See https://github.com/charliermarsh/ruff#rules for error code definitions.
-select = [
+lint.select = [
     "C40", # comprehensions
     "DTZ", # naive datetime
     "F", # flakes
     "E", # style errors
     "W", # style warnings
     #"I", # isort
     "ISC", # string concatenation
@@ -54,21 +55,21 @@
     "PLE", # pylint error
     "PLR", # pylint refactor
     "PLW", # pylint warning
     "Q", # quotes
     "RUF", # Ruff
     "S", # security
     "SIM", # simplify
-    # "UP", # pyupgrade
+    "UP", # pyupgrade
     "W", # style warnings
     "YTT", # sys.version
     "B", # bugbear
     "PTH", # use Path
 ]
-extend-ignore = [
+lint.extend-ignore = [
     "E501",
     "S101", # use of assert
     "PLR0912", # Too many branches
     "PLR2004", # Magic value used in comparison, consider replacing 2 with a constant variable
     "PLW0602", # Using global, but no assignment is done
     "PLR0913", # too many function arguments
 ]
```

### Comparing `bluequbit-0.6.0b1/setup.py` & `bluequbit-0.7.0b1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,16 +6,14 @@
     requirements = f.read()
 requirements = requirements.splitlines()
 
 with Path("README.md").open(encoding="utf-8") as f:
     readme = f.read()
 readme = "\n".join(readme.split("\n")[2:])
 
-packages = find_packages()
-
 with Path("bluequbit/version.py").open() as f:
     Version = f.read()
 
 Version = Version.rstrip()
 Version = Version[15:-1]
 
 setup(
@@ -25,9 +23,15 @@
     license="Apache 2.0",
     author="BlueQubit",
     author_email="hovnatan@bluequbit.io",
     long_description=readme,
     long_description_content_type="text/markdown",
     install_requires=requirements,
     packages=find_packages(exclude=("tests",)),
-    python_requires=">=3.7",
+    python_requires=">=3.8",
+    entry_points={
+        "pennylane.plugins": [
+            "bluequbit.cpu = bluequbit.pennylane_plugin:BluequbitCPU",
+        ]
+    },
+    include_package_data=False,
 )
```

