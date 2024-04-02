# Comparing `tmp/bluepyefe-2.3.8.tar.gz` & `tmp/bluepyefe-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluepyefe-2.3.8.tar", last modified: Tue Jan 16 12:50:13 2024, max compression
+gzip compressed data, was "bluepyefe-2.3.9.tar", last modified: Tue Jan 16 13:31:59 2024, max compression
```

## Comparing `bluepyefe-2.3.8.tar` & `bluepyefe-2.3.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 12:50:13.385535 bluepyefe-2.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-01-16 12:50:07.000000 bluepyefe-2.3.8/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-01-16 12:50:07.000000 bluepyefe-2.3.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-01-16 12:50:07.000000 bluepyefe-2.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-01-16 12:50:13.385535 bluepyefe-2.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-01-16 12:50:07.000000 bluepyefe-2.3.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 12:50:13.385535 bluepyefe-2.3.8/bluepyefe/
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-01-16 12:50:07.000000 bluepyefe-2.3.8/bluepyefe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-01-16 12:50:13.385535 bluepyefe-2.3.8/bluepyefe/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6831 2024-01-16 12:50:07.000000 bluepyefe-2.3.8/bluepyefe/auto_targets.py
--rw-r--r--   0 runner    (1001) docker     (127)     9582 2024-01-16 12:50:07.000000 bluepyefe-2.3.8/bluepyefe/cell.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 12:50:13.385535 bluepyefe-2.3.8/bluepyefe/ecode/
--rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-01-16 12:50:07.000000 bluepyefe-2.3.8/bluepyefe/ecode/DeHyperPol.py
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-01-16 12:50:07.000000 bluepyefe-2.3.8/bluepyefe/ecode/HyperDePol.py
--rw-r--r--   0 runner    (1001) docker     (127)     7184 2024-01-16 12:50:07.000000 bluepyefe-2.3.8/bluepyefe/ecode/SpikeRec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-01-16 12:50:07.000000 bluepyefe-2.3.8/bluepyefe/ecode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6950 2024-01-16 12:50:07.000000 bluepyefe-2.3.8/bluepyefe/ecode/negCheops.py
--rw-r--r--   0 runner    (1001) docker     (127)     6831 2024-01-16 12:50:07.000000 bluepyefe-2.3.8/bluepyefe/ecode/posCheops.py
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-01-16 12:50:07.000000 bluepyefe-2.3.8/bluepyefe/ecode/ramp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9891 2024-01-16 12:50:07.000000 bluepyefe-2.3.8/bluepyefe/ecode/sAHP.py
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-01-16 12:50:07.000000 bluepyefe-2.3.8/bluepyefe/ecode/sineSpec.py
--rw-r--r--   0 runner    (1001) docker     (127)     6573 2024-01-16 12:50:07.000000 bluepyefe-2.3.8/bluepyefe/ecode/step.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-01-16 12:50:07.000000 bluepyefe-2.3.8/bluepyefe/ecode/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    34969 2024-01-16 12:50:07.000000 bluepyefe-2.3.8/bluepyefe/extract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 12:50:13.385535 bluepyefe-2.3.8/bluepyefe/igorpy/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3976 2024-01-16 12:50:07.000000 bluepyefe-2.3.8/bluepyefe/igorpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7279 2024-01-16 12:50:07.000000 bluepyefe-2.3.8/bluepyefe/nwbreader.py
--rw-r--r--   0 runner    (1001) docker     (127)    10073 2024-01-16 12:50:07.000000 bluepyefe-2.3.8/bluepyefe/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-01-16 12:50:07.000000 bluepyefe-2.3.8/bluepyefe/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-01-16 12:50:07.000000 bluepyefe-2.3.8/bluepyefe/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    16246 2024-01-16 12:50:07.000000 bluepyefe-2.3.8/bluepyefe/recording.py
--rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-01-16 12:50:07.000000 bluepyefe-2.3.8/bluepyefe/rheobase.py
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-01-16 12:50:07.000000 bluepyefe-2.3.8/bluepyefe/target.py
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-01-16 12:50:07.000000 bluepyefe-2.3.8/bluepyefe/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-01-16 12:50:07.000000 bluepyefe-2.3.8/bluepyefe/translate_legacy_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 12:50:13.381534 bluepyefe-2.3.8/bluepyefe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-01-16 12:50:13.000000 bluepyefe-2.3.8/bluepyefe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-01-16 12:50:13.000000 bluepyefe-2.3.8/bluepyefe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 12:50:13.000000 bluepyefe-2.3.8/bluepyefe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-01-16 12:50:13.000000 bluepyefe-2.3.8/bluepyefe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-16 12:50:13.000000 bluepyefe-2.3.8/bluepyefe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 12:50:13.385535 bluepyefe-2.3.8/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-01-16 12:50:07.000000 bluepyefe-2.3.8/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-01-16 12:50:13.385535 bluepyefe-2.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-01-16 12:50:07.000000 bluepyefe-2.3.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    69513 2024-01-16 12:50:07.000000 bluepyefe-2.3.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 13:31:59.879604 bluepyefe-2.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-01-16 13:31:54.000000 bluepyefe-2.3.9/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-01-16 13:31:54.000000 bluepyefe-2.3.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-01-16 13:31:54.000000 bluepyefe-2.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-01-16 13:31:59.879604 bluepyefe-2.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-01-16 13:31:54.000000 bluepyefe-2.3.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 13:31:59.879604 bluepyefe-2.3.9/bluepyefe/
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-01-16 13:31:54.000000 bluepyefe-2.3.9/bluepyefe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-01-16 13:31:59.879604 bluepyefe-2.3.9/bluepyefe/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6831 2024-01-16 13:31:54.000000 bluepyefe-2.3.9/bluepyefe/auto_targets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9661 2024-01-16 13:31:54.000000 bluepyefe-2.3.9/bluepyefe/cell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 13:31:59.879604 bluepyefe-2.3.9/bluepyefe/ecode/
+-rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-01-16 13:31:54.000000 bluepyefe-2.3.9/bluepyefe/ecode/DeHyperPol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-01-16 13:31:54.000000 bluepyefe-2.3.9/bluepyefe/ecode/HyperDePol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7184 2024-01-16 13:31:54.000000 bluepyefe-2.3.9/bluepyefe/ecode/SpikeRec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-01-16 13:31:54.000000 bluepyefe-2.3.9/bluepyefe/ecode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6950 2024-01-16 13:31:54.000000 bluepyefe-2.3.9/bluepyefe/ecode/negCheops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6831 2024-01-16 13:31:54.000000 bluepyefe-2.3.9/bluepyefe/ecode/posCheops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-01-16 13:31:54.000000 bluepyefe-2.3.9/bluepyefe/ecode/ramp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9891 2024-01-16 13:31:54.000000 bluepyefe-2.3.9/bluepyefe/ecode/sAHP.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-01-16 13:31:54.000000 bluepyefe-2.3.9/bluepyefe/ecode/sineSpec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-01-16 13:31:54.000000 bluepyefe-2.3.9/bluepyefe/ecode/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-01-16 13:31:54.000000 bluepyefe-2.3.9/bluepyefe/ecode/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34969 2024-01-16 13:31:54.000000 bluepyefe-2.3.9/bluepyefe/extract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 13:31:59.879604 bluepyefe-2.3.9/bluepyefe/igorpy/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3976 2024-01-16 13:31:54.000000 bluepyefe-2.3.9/bluepyefe/igorpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7279 2024-01-16 13:31:54.000000 bluepyefe-2.3.9/bluepyefe/nwbreader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10073 2024-01-16 13:31:54.000000 bluepyefe-2.3.9/bluepyefe/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-01-16 13:31:54.000000 bluepyefe-2.3.9/bluepyefe/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-01-16 13:31:54.000000 bluepyefe-2.3.9/bluepyefe/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16258 2024-01-16 13:31:54.000000 bluepyefe-2.3.9/bluepyefe/recording.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-01-16 13:31:54.000000 bluepyefe-2.3.9/bluepyefe/rheobase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-01-16 13:31:54.000000 bluepyefe-2.3.9/bluepyefe/target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-01-16 13:31:54.000000 bluepyefe-2.3.9/bluepyefe/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-01-16 13:31:54.000000 bluepyefe-2.3.9/bluepyefe/translate_legacy_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 13:31:59.875604 bluepyefe-2.3.9/bluepyefe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-01-16 13:31:59.000000 bluepyefe-2.3.9/bluepyefe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-01-16 13:31:59.000000 bluepyefe-2.3.9/bluepyefe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 13:31:59.000000 bluepyefe-2.3.9/bluepyefe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-01-16 13:31:59.000000 bluepyefe-2.3.9/bluepyefe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-16 13:31:59.000000 bluepyefe-2.3.9/bluepyefe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 13:31:59.879604 bluepyefe-2.3.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-01-16 13:31:54.000000 bluepyefe-2.3.9/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-01-16 13:31:59.879604 bluepyefe-2.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-01-16 13:31:54.000000 bluepyefe-2.3.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69513 2024-01-16 13:31:54.000000 bluepyefe-2.3.9/versioneer.py
```

### Comparing `bluepyefe-2.3.8/LICENSE.txt` & `bluepyefe-2.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.3.8/PKG-INFO` & `bluepyefe-2.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluepyefe
-Version: 2.3.8
+Version: 2.3.9
 Summary: Blue Brain Python E-feature extraction
 Home-page: https://github.com/BlueBrain/BluePyEfe
 Author: BlueBrain Project, EPFL
 License: LGPLv3
 Keywords: neuroscience,BlueBrainProject
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `bluepyefe-2.3.8/README.rst` & `bluepyefe-2.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.3.8/bluepyefe/__init__.py` & `bluepyefe-2.3.9/bluepyefe/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.3.8/bluepyefe/auto_targets.py` & `bluepyefe-2.3.9/bluepyefe/auto_targets.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.3.8/bluepyefe/cell.py` & `bluepyefe-2.3.9/bluepyefe/cell.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,16 @@
             return recording_reader(config_data)
         if ".abf" in filename:
             return axon_reader(config_data)
         if ".ibw" in filename or ".bwav" in filename:
             return igor_reader(config_data)
         if ".nwb" in filename:
             return nwb_reader(config_data)
+        if ".txt" in filename:
+            return csv_lccr_reader(config_data)
 
         raise Exception(
             "The format of the ephys files is unknown and no custom reader"
             "were provided."
         )
 
     def get_protocol_names(self):
```

### Comparing `bluepyefe-2.3.8/bluepyefe/ecode/DeHyperPol.py` & `bluepyefe-2.3.9/bluepyefe/ecode/DeHyperPol.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.3.8/bluepyefe/ecode/HyperDePol.py` & `bluepyefe-2.3.9/bluepyefe/ecode/HyperDePol.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.3.8/bluepyefe/ecode/SpikeRec.py` & `bluepyefe-2.3.9/bluepyefe/ecode/SpikeRec.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.3.8/bluepyefe/ecode/__init__.py` & `bluepyefe-2.3.9/bluepyefe/ecode/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.3.8/bluepyefe/ecode/negCheops.py` & `bluepyefe-2.3.9/bluepyefe/ecode/negCheops.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.3.8/bluepyefe/ecode/posCheops.py` & `bluepyefe-2.3.9/bluepyefe/ecode/posCheops.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.3.8/bluepyefe/ecode/ramp.py` & `bluepyefe-2.3.9/bluepyefe/ecode/ramp.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.3.8/bluepyefe/ecode/sAHP.py` & `bluepyefe-2.3.9/bluepyefe/ecode/sAHP.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.3.8/bluepyefe/ecode/sineSpec.py` & `bluepyefe-2.3.9/bluepyefe/ecode/sineSpec.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.3.8/bluepyefe/ecode/step.py` & `bluepyefe-2.3.9/bluepyefe/ecode/step.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,16 +125,15 @@
         if self.ton is None:
             if self.hypamp is None:
                 self.hypamp = base_current(current)
             if smooth_current is None:
                 smooth_current = scipy_signal2d(current, 85)
             _ = numpy.abs(smooth_current[idx_buffer:] - self.hypamp)
             self.ton = idx_buffer + numpy.argmax(_ > step_threshold)
-
-        else:
+        elif self.hypamp is None:
             # Infer the base current hypamp
             self.hypamp = base_current(current, idx_ton=self.ton)
 
         if self.toff is None:
             if smooth_current is None:
                 smooth_current = scipy_signal2d(current, 85)
             _ = numpy.flip(
```

### Comparing `bluepyefe-2.3.8/bluepyefe/ecode/tools.py` & `bluepyefe-2.3.9/bluepyefe/ecode/tools.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.3.8/bluepyefe/extract.py` & `bluepyefe-2.3.9/bluepyefe/extract.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.3.8/bluepyefe/igorpy/__init__.py` & `bluepyefe-2.3.9/bluepyefe/igorpy/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.3.8/bluepyefe/nwbreader.py` & `bluepyefe-2.3.9/bluepyefe/nwbreader.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.3.8/bluepyefe/plotting.py` & `bluepyefe-2.3.9/bluepyefe/plotting.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.3.8/bluepyefe/protocol.py` & `bluepyefe-2.3.9/bluepyefe/protocol.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.3.8/bluepyefe/reader.py` & `bluepyefe-2.3.9/bluepyefe/reader.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,14 +19,15 @@
  51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 """
 import logging
 import h5py
 import numpy
 import scipy.io
 from neo import io
+import os
 
 from . import igorpy
 from .nwbreader import BBPNWBReader, ScalaNWBReader, AIBSNWBReader
 
 logger = logging.getLogger(__name__)
 
 
@@ -195,7 +196,93 @@
             reader = AIBSNWBReader(content, target_protocols)
         else:
             reader = ScalaNWBReader(content, target_protocols)
 
         data = reader.read()
 
     return data
+
+
+def csv_lccr_reader(in_data):
+    """Reader to read .txt (csv_lccr)
+    Args:
+        in_data (dict): of the format
+        {
+            'filepath': "./XXX.txt",
+            'dt': 0.1,
+            'ton': 2000,
+            'toff': 2500,
+            'ljp': 14.0,
+            'amplitudes': [10 -10 20 -20 30 -30 40 -40 50 -50],
+            'hypamp': -20 # (units should match 'amplitudes'),
+            'remove_last_100ms': True,
+            'v_unit': 'mV',
+            't_unit': 'ms',
+            'i_unit': 'pA' # current unit for 'amplitudes' and 'hypamp'
+        }
+    """
+    _check_metadata(
+        in_data,
+        csv_lccr_reader.__name__,
+        ["filepath", "dt", "amplitudes", "v_unit", "t_unit", "i_unit", "ton", "toff", "hypamp"],
+    )
+
+    data = []
+
+    fln = os.path.join(in_data['filepath'])
+    if not os.path.isfile(fln):
+        raise FileNotFoundError(
+            "Please provide a string with the filename of the txt file; "
+            f"current path not found: {fln}"
+        )
+
+    dt = in_data['dt']
+    ton = in_data['ton']
+    toff = in_data['toff']
+    amplitudes = in_data['amplitudes']
+    hypamp = in_data['hypamp']
+
+    import csv
+    with open(fln, 'rt') as f:
+        reader = csv.reader(f, delimiter='\t')
+        columns = list(zip(*reader))
+        length = numpy.shape(columns)[1]
+
+        voltages = numpy.array([
+            [
+                float(string) if string not in ["-", ""] else 0
+                for string in column
+            ]
+            for column in columns
+        ])
+        t = numpy.arange(length) * dt
+
+    # Remove last 100 ms if needed
+    if in_data.get('remove_last_100ms', False):
+        slice_end = int(-100. / dt)
+        voltages = voltages[:, :slice_end]
+        t = t[:slice_end]
+
+    for amplitude, voltage in zip(amplitudes, voltages):
+        current = numpy.zeros_like(voltage)
+        ion, ioff = int(ton / dt), int(toff / dt)
+        current[:] = hypamp
+        current[ion:ioff] = amplitude + hypamp
+        trace_data = {
+            "filename": os.path.basename(in_data['filepath']),
+            "current": current,
+            "voltage": voltage,
+            "t": t,
+            "dt": numpy.float64(dt),
+            "ton": numpy.float64(ton),
+            "toff": numpy.float64(toff),
+            "amp": numpy.float64(amplitude),
+            "hypamp": numpy.float64(hypamp),
+            "ljp": in_data.get('ljp', 0),
+            "i_unit": in_data['i_unit'],
+            "v_unit": in_data['v_unit'],
+            "t_unit": in_data['t_unit'],
+        }
+
+        data.append(trace_data)
+
+    return data
```

### Comparing `bluepyefe-2.3.8/bluepyefe/recording.py` & `bluepyefe-2.3.9/bluepyefe/recording.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,16 +229,15 @@
                 voltage - numpy.median(voltage[:100]) + config_data["v_corr"]
             )
 
         # Correct for the liquid junction potential
         # WARNING: the ljp is informed as a positive float but we substract it
         # from the voltage
         if "ljp" in config_data and config_data["ljp"] is not None:
-            voltage = voltage - config_data["ljp"]
-
+            voltage = numpy.array(voltage) - config_data["ljp"]
         if "repetition" in reader_data:
             self.repetition = reader_data["repetition"]
 
         return t, current, voltage, amp, hypamp
 
     def call_efel(self, efeatures, efel_settings=None):
         """ Calls efel to compute the wanted efeatures """
```

### Comparing `bluepyefe-2.3.8/bluepyefe/rheobase.py` & `bluepyefe-2.3.9/bluepyefe/rheobase.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.3.8/bluepyefe/target.py` & `bluepyefe-2.3.9/bluepyefe/target.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.3.8/bluepyefe/tools.py` & `bluepyefe-2.3.9/bluepyefe/tools.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.3.8/bluepyefe/translate_legacy_config.py` & `bluepyefe-2.3.9/bluepyefe/translate_legacy_config.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.3.8/bluepyefe.egg-info/PKG-INFO` & `bluepyefe-2.3.9/bluepyefe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluepyefe
-Version: 2.3.8
+Version: 2.3.9
 Summary: Blue Brain Python E-feature extraction
 Home-page: https://github.com/BlueBrain/BluePyEfe
 Author: BlueBrain Project, EPFL
 License: LGPLv3
 Keywords: neuroscience,BlueBrainProject
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `bluepyefe-2.3.8/bluepyefe.egg-info/SOURCES.txt` & `bluepyefe-2.3.9/bluepyefe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.3.8/examples/__init__.py` & `bluepyefe-2.3.9/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.3.8/setup.py` & `bluepyefe-2.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.3.8/versioneer.py` & `bluepyefe-2.3.9/versioneer.py`

 * *Files identical despite different names*

