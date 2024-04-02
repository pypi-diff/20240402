# Comparing `tmp/lightning-whisper-mlx-0.0.6.tar.gz` & `tmp/lightning-whisper-mlx-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-whisper-mlx-0.0.6.tar", last modified: Tue Apr  2 09:44:17 2024, max compression
+gzip compressed data, was "lightning-whisper-mlx-0.0.7.tar", last modified: Tue Apr  2 09:45:50 2024, max compression
```

## Comparing `lightning-whisper-mlx-0.0.6.tar` & `lightning-whisper-mlx-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 mustafaaljadery   (501) staff       (20)        0 2024-04-02 09:44:17.227828 lightning-whisper-mlx-0.0.6/
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)      280 2024-04-02 09:44:17.227133 lightning-whisper-mlx-0.0.6/PKG-INFO
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)     1236 2024-04-02 09:22:13.000000 lightning-whisper-mlx-0.0.6/README.md
-drwxr-xr-x   0 mustafaaljadery   (501) staff       (20)        0 2024-04-02 09:44:17.225866 lightning-whisper-mlx-0.0.6/lighting_whisper_mlx/
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)       41 2024-04-02 09:37:33.000000 lightning-whisper-mlx-0.0.6/lighting_whisper_mlx/__init__.py
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)     5013 2024-04-01 06:18:02.000000 lightning-whisper-mlx-0.0.6/lighting_whisper_mlx/audio.py
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)    28281 2024-04-01 02:41:11.000000 lightning-whisper-mlx-0.0.6/lighting_whisper_mlx/decoding.py
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)     3221 2024-04-02 08:34:26.000000 lightning-whisper-mlx-0.0.6/lighting_whisper_mlx/lightning.py
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)     1035 2024-04-01 02:23:40.000000 lightning-whisper-mlx-0.0.6/lighting_whisper_mlx/load_models.py
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)    10880 2024-04-01 02:23:40.000000 lightning-whisper-mlx-0.0.6/lighting_whisper_mlx/timing.py
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)    12407 2024-04-01 02:23:40.000000 lightning-whisper-mlx-0.0.6/lighting_whisper_mlx/tokenizer.py
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)    10592 2024-04-01 02:23:40.000000 lightning-whisper-mlx-0.0.6/lighting_whisper_mlx/torch_whisper.py
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)    16233 2024-04-02 08:56:32.000000 lightning-whisper-mlx-0.0.6/lighting_whisper_mlx/transcribe.py
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)     8668 2024-04-02 07:03:32.000000 lightning-whisper-mlx-0.0.6/lighting_whisper_mlx/whisper.py
-drwxr-xr-x   0 mustafaaljadery   (501) staff       (20)        0 2024-04-02 09:44:17.226831 lightning-whisper-mlx-0.0.6/lightning_whisper_mlx.egg-info/
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)      280 2024-04-02 09:44:17.000000 lightning-whisper-mlx-0.0.6/lightning_whisper_mlx.egg-info/PKG-INFO
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)      626 2024-04-02 09:44:17.000000 lightning-whisper-mlx-0.0.6/lightning_whisper_mlx.egg-info/SOURCES.txt
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)        1 2024-04-02 09:44:17.000000 lightning-whisper-mlx-0.0.6/lightning_whisper_mlx.egg-info/dependency_links.txt
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)       68 2024-04-02 09:44:17.000000 lightning-whisper-mlx-0.0.6/lightning_whisper_mlx.egg-info/entry_points.txt
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)       80 2024-04-02 09:44:17.000000 lightning-whisper-mlx-0.0.6/lightning_whisper_mlx.egg-info/requires.txt
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)       21 2024-04-02 09:44:17.000000 lightning-whisper-mlx-0.0.6/lightning_whisper_mlx.egg-info/top_level.txt
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)       38 2024-04-02 09:44:17.227919 lightning-whisper-mlx-0.0.6/setup.cfg
--rw-r--r--   0 mustafaaljadery   (501) staff       (20)      472 2024-04-02 09:44:14.000000 lightning-whisper-mlx-0.0.6/setup.py
+drwxr-xr-x   0 mustafaaljadery   (501) staff       (20)        0 2024-04-02 09:45:50.785087 lightning-whisper-mlx-0.0.7/
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)      280 2024-04-02 09:45:50.784876 lightning-whisper-mlx-0.0.7/PKG-INFO
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)     1236 2024-04-02 09:22:13.000000 lightning-whisper-mlx-0.0.7/README.md
+drwxr-xr-x   0 mustafaaljadery   (501) staff       (20)        0 2024-04-02 09:45:50.783700 lightning-whisper-mlx-0.0.7/lighting_whisper_mlx/
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)       41 2024-04-02 09:37:33.000000 lightning-whisper-mlx-0.0.7/lighting_whisper_mlx/__init__.py
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)     5013 2024-04-01 06:18:02.000000 lightning-whisper-mlx-0.0.7/lighting_whisper_mlx/audio.py
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)    28281 2024-04-01 02:41:11.000000 lightning-whisper-mlx-0.0.7/lighting_whisper_mlx/decoding.py
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)     3221 2024-04-02 08:34:26.000000 lightning-whisper-mlx-0.0.7/lighting_whisper_mlx/lightning.py
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)     1035 2024-04-01 02:23:40.000000 lightning-whisper-mlx-0.0.7/lighting_whisper_mlx/load_models.py
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)    10880 2024-04-01 02:23:40.000000 lightning-whisper-mlx-0.0.7/lighting_whisper_mlx/timing.py
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)    12407 2024-04-01 02:23:40.000000 lightning-whisper-mlx-0.0.7/lighting_whisper_mlx/tokenizer.py
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)    10592 2024-04-01 02:23:40.000000 lightning-whisper-mlx-0.0.7/lighting_whisper_mlx/torch_whisper.py
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)    16233 2024-04-02 08:56:32.000000 lightning-whisper-mlx-0.0.7/lighting_whisper_mlx/transcribe.py
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)     8668 2024-04-02 07:03:32.000000 lightning-whisper-mlx-0.0.7/lighting_whisper_mlx/whisper.py
+drwxr-xr-x   0 mustafaaljadery   (501) staff       (20)        0 2024-04-02 09:45:50.784605 lightning-whisper-mlx-0.0.7/lightning_whisper_mlx.egg-info/
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)      280 2024-04-02 09:45:50.000000 lightning-whisper-mlx-0.0.7/lightning_whisper_mlx.egg-info/PKG-INFO
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)      626 2024-04-02 09:45:50.000000 lightning-whisper-mlx-0.0.7/lightning_whisper_mlx.egg-info/SOURCES.txt
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)        1 2024-04-02 09:45:50.000000 lightning-whisper-mlx-0.0.7/lightning_whisper_mlx.egg-info/dependency_links.txt
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)       68 2024-04-02 09:45:50.000000 lightning-whisper-mlx-0.0.7/lightning_whisper_mlx.egg-info/entry_points.txt
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)       80 2024-04-02 09:45:50.000000 lightning-whisper-mlx-0.0.7/lightning_whisper_mlx.egg-info/requires.txt
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)       21 2024-04-02 09:45:50.000000 lightning-whisper-mlx-0.0.7/lightning_whisper_mlx.egg-info/top_level.txt
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)       38 2024-04-02 09:45:50.785129 lightning-whisper-mlx-0.0.7/setup.cfg
+-rw-r--r--   0 mustafaaljadery   (501) staff       (20)      472 2024-04-02 09:45:47.000000 lightning-whisper-mlx-0.0.7/setup.py
```

### Comparing `lightning-whisper-mlx-0.0.6/README.md` & `lightning-whisper-mlx-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `lightning-whisper-mlx-0.0.6/lighting_whisper_mlx/audio.py` & `lightning-whisper-mlx-0.0.7/lighting_whisper_mlx/audio.py`

 * *Files identical despite different names*

### Comparing `lightning-whisper-mlx-0.0.6/lighting_whisper_mlx/decoding.py` & `lightning-whisper-mlx-0.0.7/lighting_whisper_mlx/decoding.py`

 * *Files identical despite different names*

### Comparing `lightning-whisper-mlx-0.0.6/lighting_whisper_mlx/lightning.py` & `lightning-whisper-mlx-0.0.7/lighting_whisper_mlx/lightning.py`

 * *Files identical despite different names*

### Comparing `lightning-whisper-mlx-0.0.6/lighting_whisper_mlx/load_models.py` & `lightning-whisper-mlx-0.0.7/lighting_whisper_mlx/load_models.py`

 * *Files identical despite different names*

### Comparing `lightning-whisper-mlx-0.0.6/lighting_whisper_mlx/timing.py` & `lightning-whisper-mlx-0.0.7/lighting_whisper_mlx/timing.py`

 * *Files identical despite different names*

### Comparing `lightning-whisper-mlx-0.0.6/lighting_whisper_mlx/tokenizer.py` & `lightning-whisper-mlx-0.0.7/lighting_whisper_mlx/tokenizer.py`

 * *Files identical despite different names*

### Comparing `lightning-whisper-mlx-0.0.6/lighting_whisper_mlx/torch_whisper.py` & `lightning-whisper-mlx-0.0.7/lighting_whisper_mlx/torch_whisper.py`

 * *Files identical despite different names*

### Comparing `lightning-whisper-mlx-0.0.6/lighting_whisper_mlx/transcribe.py` & `lightning-whisper-mlx-0.0.7/lighting_whisper_mlx/transcribe.py`

 * *Files identical despite different names*

### Comparing `lightning-whisper-mlx-0.0.6/lighting_whisper_mlx/whisper.py` & `lightning-whisper-mlx-0.0.7/lighting_whisper_mlx/whisper.py`

 * *Files identical despite different names*

### Comparing `lightning-whisper-mlx-0.0.6/lightning_whisper_mlx.egg-info/SOURCES.txt` & `lightning-whisper-mlx-0.0.7/lightning_whisper_mlx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

