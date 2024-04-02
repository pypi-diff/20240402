# Comparing `tmp/lightning-whisper-mlx-0.0.2.tar.gz` & `tmp/lightning-whisper-mlx-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-whisper-mlx-0.0.2.tar", last modified: Tue Apr  2 09:34:23 2024, max compression
+gzip compressed data, was "lightning-whisper-mlx-0.0.3.tar", last modified: Tue Apr  2 09:39:36 2024, max compression
```

## Comparing `lightning-whisper-mlx-0.0.2.tar` & `lightning-whisper-mlx-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 mustafaaljadery   (501) staff       (20)        0 2024-04-02 09:34:23.845402 lightning-whisper-mlx-0.0.2/
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)      280 2024-04-02 09:34:23.845200 lightning-whisper-mlx-0.0.2/PKG-INFO
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)     1236 2024-04-02 09:22:13.000000 lightning-whisper-mlx-0.0.2/README.md
-drwxr-xr-x   0 mustafaaljadery   (501) staff       (20)        0 2024-04-02 09:34:23.843904 lightning-whisper-mlx-0.0.2/lightning-whisper-mlx/
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)       73 2024-04-02 06:55:41.000000 lightning-whisper-mlx-0.0.2/lightning-whisper-mlx/__init__.py
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)     5013 2024-04-01 06:18:02.000000 lightning-whisper-mlx-0.0.2/lightning-whisper-mlx/audio.py
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)    28281 2024-04-01 02:41:11.000000 lightning-whisper-mlx-0.0.2/lightning-whisper-mlx/decoding.py
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)     3221 2024-04-02 08:34:26.000000 lightning-whisper-mlx-0.0.2/lightning-whisper-mlx/lightning.py
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)     1035 2024-04-01 02:23:40.000000 lightning-whisper-mlx-0.0.2/lightning-whisper-mlx/load_models.py
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)    10880 2024-04-01 02:23:40.000000 lightning-whisper-mlx-0.0.2/lightning-whisper-mlx/timing.py
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)    12407 2024-04-01 02:23:40.000000 lightning-whisper-mlx-0.0.2/lightning-whisper-mlx/tokenizer.py
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)    10592 2024-04-01 02:23:40.000000 lightning-whisper-mlx-0.0.2/lightning-whisper-mlx/torch_whisper.py
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)    16233 2024-04-02 08:56:32.000000 lightning-whisper-mlx-0.0.2/lightning-whisper-mlx/transcribe.py
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)     8668 2024-04-02 07:03:32.000000 lightning-whisper-mlx-0.0.2/lightning-whisper-mlx/whisper.py
-drwxr-xr-x   0 mustafaaljadery   (501) staff       (20)        0 2024-04-02 09:34:23.844879 lightning-whisper-mlx-0.0.2/lightning_whisper_mlx.egg-info/
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)      280 2024-04-02 09:34:23.000000 lightning-whisper-mlx-0.0.2/lightning_whisper_mlx.egg-info/PKG-INFO
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)      588 2024-04-02 09:34:23.000000 lightning-whisper-mlx-0.0.2/lightning_whisper_mlx.egg-info/SOURCES.txt
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)        1 2024-04-02 09:34:23.000000 lightning-whisper-mlx-0.0.2/lightning_whisper_mlx.egg-info/dependency_links.txt
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)       80 2024-04-02 09:34:23.000000 lightning-whisper-mlx-0.0.2/lightning_whisper_mlx.egg-info/requires.txt
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)       22 2024-04-02 09:34:23.000000 lightning-whisper-mlx-0.0.2/lightning_whisper_mlx.egg-info/top_level.txt
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)       38 2024-04-02 09:34:23.845446 lightning-whisper-mlx-0.0.2/setup.cfg
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)      346 2024-04-02 09:34:20.000000 lightning-whisper-mlx-0.0.2/setup.py
+drwxr-xr-x   0 mustafaaljadery   (501) staff       (20)        0 2024-04-02 09:39:36.299801 lightning-whisper-mlx-0.0.3/
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)      280 2024-04-02 09:39:36.299589 lightning-whisper-mlx-0.0.3/PKG-INFO
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)     1236 2024-04-02 09:22:13.000000 lightning-whisper-mlx-0.0.3/README.md
+drwxr-xr-x   0 mustafaaljadery   (501) staff       (20)        0 2024-04-02 09:39:36.298247 lightning-whisper-mlx-0.0.3/lightning-whisper-mlx/
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)       41 2024-04-02 09:37:33.000000 lightning-whisper-mlx-0.0.3/lightning-whisper-mlx/__init__.py
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)     5013 2024-04-01 06:18:02.000000 lightning-whisper-mlx-0.0.3/lightning-whisper-mlx/audio.py
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)    28281 2024-04-01 02:41:11.000000 lightning-whisper-mlx-0.0.3/lightning-whisper-mlx/decoding.py
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)     3221 2024-04-02 08:34:26.000000 lightning-whisper-mlx-0.0.3/lightning-whisper-mlx/lightning.py
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)     1035 2024-04-01 02:23:40.000000 lightning-whisper-mlx-0.0.3/lightning-whisper-mlx/load_models.py
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)    10880 2024-04-01 02:23:40.000000 lightning-whisper-mlx-0.0.3/lightning-whisper-mlx/timing.py
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)    12407 2024-04-01 02:23:40.000000 lightning-whisper-mlx-0.0.3/lightning-whisper-mlx/tokenizer.py
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)    10592 2024-04-01 02:23:40.000000 lightning-whisper-mlx-0.0.3/lightning-whisper-mlx/torch_whisper.py
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)    16233 2024-04-02 08:56:32.000000 lightning-whisper-mlx-0.0.3/lightning-whisper-mlx/transcribe.py
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)     8668 2024-04-02 07:03:32.000000 lightning-whisper-mlx-0.0.3/lightning-whisper-mlx/whisper.py
+drwxr-xr-x   0 mustafaaljadery   (501) staff       (20)        0 2024-04-02 09:39:36.299286 lightning-whisper-mlx-0.0.3/lightning_whisper_mlx.egg-info/
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)      280 2024-04-02 09:39:36.000000 lightning-whisper-mlx-0.0.3/lightning_whisper_mlx.egg-info/PKG-INFO
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)      636 2024-04-02 09:39:36.000000 lightning-whisper-mlx-0.0.3/lightning_whisper_mlx.egg-info/SOURCES.txt
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)        1 2024-04-02 09:39:36.000000 lightning-whisper-mlx-0.0.3/lightning_whisper_mlx.egg-info/dependency_links.txt
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)       73 2024-04-02 09:39:36.000000 lightning-whisper-mlx-0.0.3/lightning_whisper_mlx.egg-info/entry_points.txt
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)       80 2024-04-02 09:39:36.000000 lightning-whisper-mlx-0.0.3/lightning_whisper_mlx.egg-info/requires.txt
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)       22 2024-04-02 09:39:36.000000 lightning-whisper-mlx-0.0.3/lightning_whisper_mlx.egg-info/top_level.txt
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)       38 2024-04-02 09:39:36.299852 lightning-whisper-mlx-0.0.3/setup.cfg
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)      477 2024-04-02 09:39:33.000000 lightning-whisper-mlx-0.0.3/setup.py
```

### Comparing `lightning-whisper-mlx-0.0.2/README.md` & `lightning-whisper-mlx-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `lightning-whisper-mlx-0.0.2/lightning-whisper-mlx/audio.py` & `lightning-whisper-mlx-0.0.3/lightning-whisper-mlx/audio.py`

 * *Files identical despite different names*

### Comparing `lightning-whisper-mlx-0.0.2/lightning-whisper-mlx/decoding.py` & `lightning-whisper-mlx-0.0.3/lightning-whisper-mlx/decoding.py`

 * *Files identical despite different names*

### Comparing `lightning-whisper-mlx-0.0.2/lightning-whisper-mlx/lightning.py` & `lightning-whisper-mlx-0.0.3/lightning-whisper-mlx/lightning.py`

 * *Files identical despite different names*

### Comparing `lightning-whisper-mlx-0.0.2/lightning-whisper-mlx/load_models.py` & `lightning-whisper-mlx-0.0.3/lightning-whisper-mlx/load_models.py`

 * *Files identical despite different names*

### Comparing `lightning-whisper-mlx-0.0.2/lightning-whisper-mlx/timing.py` & `lightning-whisper-mlx-0.0.3/lightning-whisper-mlx/timing.py`

 * *Files identical despite different names*

### Comparing `lightning-whisper-mlx-0.0.2/lightning-whisper-mlx/tokenizer.py` & `lightning-whisper-mlx-0.0.3/lightning-whisper-mlx/tokenizer.py`

 * *Files identical despite different names*

### Comparing `lightning-whisper-mlx-0.0.2/lightning-whisper-mlx/torch_whisper.py` & `lightning-whisper-mlx-0.0.3/lightning-whisper-mlx/torch_whisper.py`

 * *Files identical despite different names*

### Comparing `lightning-whisper-mlx-0.0.2/lightning-whisper-mlx/transcribe.py` & `lightning-whisper-mlx-0.0.3/lightning-whisper-mlx/transcribe.py`

 * *Files identical despite different names*

### Comparing `lightning-whisper-mlx-0.0.2/lightning-whisper-mlx/whisper.py` & `lightning-whisper-mlx-0.0.3/lightning-whisper-mlx/whisper.py`

 * *Files identical despite different names*

### Comparing `lightning-whisper-mlx-0.0.2/lightning_whisper_mlx.egg-info/SOURCES.txt` & `lightning-whisper-mlx-0.0.3/lightning_whisper_mlx.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -9,9 +9,10 @@
 lightning-whisper-mlx/tokenizer.py
 lightning-whisper-mlx/torch_whisper.py
 lightning-whisper-mlx/transcribe.py
 lightning-whisper-mlx/whisper.py
 lightning_whisper_mlx.egg-info/PKG-INFO
 lightning_whisper_mlx.egg-info/SOURCES.txt
 lightning_whisper_mlx.egg-info/dependency_links.txt
+lightning_whisper_mlx.egg-info/entry_points.txt
 lightning_whisper_mlx.egg-info/requires.txt
 lightning_whisper_mlx.egg-info/top_level.txt
```

