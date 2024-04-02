# Comparing `tmp/klay-beam-0.13.4.tar.gz` & `tmp/klay-beam-0.13.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klay-beam-0.13.4.tar", last modified: Wed Mar 27 14:49:54 2024, max compression
+gzip compressed data, was "klay-beam-0.13.5.tar", last modified: Tue Apr  2 20:34:53 2024, max compression
```

## Comparing `klay-beam-0.13.4.tar` & `klay-beam-0.13.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:49:54.318782 klay-beam-0.13.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-03-27 14:49:47.000000 klay-beam-0.13.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    18593 2024-03-27 14:49:54.318782 klay-beam-0.13.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16547 2024-03-27 14:49:47.000000 klay-beam-0.13.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-03-27 14:49:47.000000 klay-beam-0.13.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-27 14:49:54.318782 klay-beam-0.13.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-27 14:49:47.000000 klay-beam-0.13.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:49:54.310782 klay-beam-0.13.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:49:54.314782 klay-beam-0.13.4/src/klay_beam/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-27 14:49:47.000000 klay-beam-0.13.4/src/klay_beam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-03-27 14:49:47.000000 klay-beam-0.13.4/src/klay_beam/path.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 14:49:47.000000 klay-beam-0.13.4/src/klay_beam/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-03-27 14:49:47.000000 klay-beam-0.13.4/src/klay_beam/run_cuda_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-03-27 14:49:47.000000 klay-beam-0.13.4/src/klay_beam/run_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-03-27 14:49:47.000000 klay-beam-0.13.4/src/klay_beam/torch_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-03-27 14:49:47.000000 klay-beam-0.13.4/src/klay_beam/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-03-27 14:49:47.000000 klay-beam-0.13.4/src/klay_beam/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-03-27 14:49:47.000000 klay-beam-0.13.4/src/klay_beam/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:49:54.314782 klay-beam-0.13.4/src/klay_beam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18593 2024-03-27 14:49:54.000000 klay-beam-0.13.4/src/klay_beam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-27 14:49:54.000000 klay-beam-0.13.4/src/klay_beam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 14:49:54.000000 klay-beam-0.13.4/src/klay_beam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-03-27 14:49:54.000000 klay-beam-0.13.4/src/klay_beam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-27 14:49:54.000000 klay-beam-0.13.4/src/klay_beam.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:49:54.314782 klay-beam-0.13.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3886 2024-03-27 14:49:47.000000 klay-beam-0.13.4/tests/test_audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-03-27 14:49:47.000000 klay-beam-0.13.4/tests/test_audio_file_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-03-27 14:49:47.000000 klay-beam-0.13.4/tests/test_audio_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-03-27 14:49:47.000000 klay-beam-0.13.4/tests/test_multi_match_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-03-27 14:49:47.000000 klay-beam-0.13.4/tests/test_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-03-27 14:49:47.000000 klay-beam-0.13.4/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:34:53.412318 klay-beam-0.13.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-02 20:34:45.000000 klay-beam-0.13.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    18593 2024-04-02 20:34:53.412318 klay-beam-0.13.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16547 2024-04-02 20:34:45.000000 klay-beam-0.13.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-02 20:34:45.000000 klay-beam-0.13.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-02 20:34:53.412318 klay-beam-0.13.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-02 20:34:45.000000 klay-beam-0.13.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:34:53.412318 klay-beam-0.13.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:34:53.412318 klay-beam-0.13.5/src/klay_beam/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 20:34:45.000000 klay-beam-0.13.5/src/klay_beam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-02 20:34:45.000000 klay-beam-0.13.5/src/klay_beam/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:34:45.000000 klay-beam-0.13.5/src/klay_beam/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-04-02 20:34:45.000000 klay-beam-0.13.5/src/klay_beam/run_cuda_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-04-02 20:34:45.000000 klay-beam-0.13.5/src/klay_beam/run_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-04-02 20:34:45.000000 klay-beam-0.13.5/src/klay_beam/torch_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-02 20:34:45.000000 klay-beam-0.13.5/src/klay_beam/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-04-02 20:34:45.000000 klay-beam-0.13.5/src/klay_beam/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-02 20:34:45.000000 klay-beam-0.13.5/src/klay_beam/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:34:53.412318 klay-beam-0.13.5/src/klay_beam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18593 2024-04-02 20:34:53.000000 klay-beam-0.13.5/src/klay_beam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-02 20:34:53.000000 klay-beam-0.13.5/src/klay_beam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 20:34:53.000000 klay-beam-0.13.5/src/klay_beam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-02 20:34:53.000000 klay-beam-0.13.5/src/klay_beam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-02 20:34:53.000000 klay-beam-0.13.5/src/klay_beam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:34:53.412318 klay-beam-0.13.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3886 2024-04-02 20:34:45.000000 klay-beam-0.13.5/tests/test_audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-04-02 20:34:45.000000 klay-beam-0.13.5/tests/test_audio_file_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-02 20:34:45.000000 klay-beam-0.13.5/tests/test_audio_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-02 20:34:45.000000 klay-beam-0.13.5/tests/test_multi_match_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-02 20:34:45.000000 klay-beam-0.13.5/tests/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-02 20:34:45.000000 klay-beam-0.13.5/tests/test_transforms.py
```

### Comparing `klay-beam-0.13.4/LICENSE` & `klay-beam-0.13.5/LICENSE`

 * *Files identical despite different names*

### Comparing `klay-beam-0.13.4/PKG-INFO` & `klay-beam-0.13.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klay-beam
-Version: 0.13.4
+Version: 0.13.5
 Summary: Toolkit for massively parallel audio processing via Apache Beam
 License:  The MIT License (MIT)
         
         Copyright © 2023 Klay Vision INC.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `klay-beam-0.13.4/README.md` & `klay-beam-0.13.5/README.md`

 * *Files identical despite different names*

### Comparing `klay-beam-0.13.4/pyproject.toml` & `klay-beam-0.13.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `klay-beam-0.13.4/src/klay_beam/path.py` & `klay-beam-0.13.5/src/klay_beam/path.py`

 * *Files identical despite different names*

### Comparing `klay-beam-0.13.4/src/klay_beam/run_cuda_test.py` & `klay-beam-0.13.5/src/klay_beam/run_cuda_test.py`

 * *Files identical despite different names*

### Comparing `klay-beam-0.13.4/src/klay_beam/run_example.py` & `klay-beam-0.13.5/src/klay_beam/run_example.py`

 * *Files identical despite different names*

### Comparing `klay-beam-0.13.4/src/klay_beam/torch_transforms.py` & `klay-beam-0.13.5/src/klay_beam/torch_transforms.py`

 * *Files identical despite different names*

### Comparing `klay-beam-0.13.4/src/klay_beam/torch_utils.py` & `klay-beam-0.13.5/src/klay_beam/torch_utils.py`

 * *Files identical despite different names*

### Comparing `klay-beam-0.13.4/src/klay_beam/transforms.py` & `klay-beam-0.13.5/src/klay_beam/transforms.py`

 * *Files identical despite different names*

### Comparing `klay-beam-0.13.4/src/klay_beam/utils.py` & `klay-beam-0.13.5/src/klay_beam/utils.py`

 * *Files identical despite different names*

### Comparing `klay-beam-0.13.4/src/klay_beam.egg-info/PKG-INFO` & `klay-beam-0.13.5/src/klay_beam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klay-beam
-Version: 0.13.4
+Version: 0.13.5
 Summary: Toolkit for massively parallel audio processing via Apache Beam
 License:  The MIT License (MIT)
         
         Copyright © 2023 Klay Vision INC.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `klay-beam-0.13.4/src/klay_beam.egg-info/SOURCES.txt` & `klay-beam-0.13.5/src/klay_beam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `klay-beam-0.13.4/tests/test_audio.py` & `klay-beam-0.13.5/tests/test_audio.py`

 * *Files identical despite different names*

### Comparing `klay-beam-0.13.4/tests/test_audio_file_io.py` & `klay-beam-0.13.5/tests/test_audio_file_io.py`

 * *Files identical despite different names*

### Comparing `klay-beam-0.13.4/tests/test_audio_loaders.py` & `klay-beam-0.13.5/tests/test_audio_loaders.py`

 * *Files identical despite different names*

### Comparing `klay-beam-0.13.4/tests/test_multi_match_files.py` & `klay-beam-0.13.5/tests/test_multi_match_files.py`

 * *Files identical despite different names*

### Comparing `klay-beam-0.13.4/tests/test_path.py` & `klay-beam-0.13.5/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `klay-beam-0.13.4/tests/test_transforms.py` & `klay-beam-0.13.5/tests/test_transforms.py`

 * *Files identical despite different names*

