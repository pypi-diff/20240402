# Comparing `tmp/czo-0.1.5.tar.gz` & `tmp/czo-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "czo-0.1.5.tar", last modified: Sun Mar 31 08:13:33 2024, max compression
+gzip compressed data, was "czo-0.1.6.tar", last modified: Tue Apr  2 05:37:19 2024, max compression
```

## Comparing `czo-0.1.5.tar` & `czo-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 sfwwslm   (1000) sfwwslm   (1000)        0 2024-03-31 08:13:33.638610 czo-0.1.5/
--rw-r--r--   0 sfwwslm   (1000) sfwwslm   (1000)      315 2024-03-31 08:13:33.638610 czo-0.1.5/PKG-INFO
--rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)       83 2024-03-27 06:33:55.000000 czo-0.1.5/README.md
--rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)       38 2024-03-31 08:13:33.638610 czo-0.1.5/setup.cfg
--rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)      478 2024-03-31 08:13:31.000000 czo-0.1.5/setup.py
-drwxrwxr-x   0 sfwwslm   (1000) sfwwslm   (1000)        0 2024-03-31 08:13:33.634610 czo-0.1.5/src/
-drwxrwxr-x   0 sfwwslm   (1000) sfwwslm   (1000)        0 2024-03-31 08:13:33.634610 czo-0.1.5/src/czo/
--rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)      232 2024-03-31 07:44:26.000000 czo-0.1.5/src/czo/__init__.py
--rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)     8557 2024-03-27 06:33:55.000000 czo-0.1.5/src/czo/_date.py
--rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)    12017 2024-03-27 06:33:55.000000 czo-0.1.5/src/czo/_faker.py
--rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)     5940 2024-03-31 08:09:18.000000 czo-0.1.5/src/czo/_path.py
--rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)     4781 2024-03-27 06:33:55.000000 czo-0.1.5/src/czo/_rand.py
-drwxrwxr-x   0 sfwwslm   (1000) sfwwslm   (1000)        0 2024-03-31 08:13:33.638610 czo-0.1.5/src/czo/data/
--rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)        0 2024-03-27 06:33:55.000000 czo-0.1.5/src/czo/data/__init__.py
--rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)    14519 2024-03-27 06:33:55.000000 czo-0.1.5/src/czo/data/_country.py
--rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)    16493 2024-03-27 06:33:55.000000 czo-0.1.5/src/czo/data/_housing.py
--rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)   154755 2024-03-27 06:33:55.000000 czo-0.1.5/src/czo/data/_internal_utils.py
-drwxrwxr-x   0 sfwwslm   (1000) sfwwslm   (1000)        0 2024-03-31 08:13:33.638610 czo-0.1.5/src/czo.egg-info/
--rw-r--r--   0 sfwwslm   (1000) sfwwslm   (1000)      315 2024-03-31 08:13:33.000000 czo-0.1.5/src/czo.egg-info/PKG-INFO
--rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)      368 2024-03-31 08:13:33.000000 czo-0.1.5/src/czo.egg-info/SOURCES.txt
--rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)        1 2024-03-31 08:13:33.000000 czo-0.1.5/src/czo.egg-info/dependency_links.txt
--rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)       25 2024-03-31 08:13:33.000000 czo-0.1.5/src/czo.egg-info/requires.txt
--rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)        4 2024-03-31 08:13:33.000000 czo-0.1.5/src/czo.egg-info/top_level.txt
+drwxrwxr-x   0 sfwwslm   (1000) sfwwslm   (1000)        0 2024-04-02 05:37:19.767175 czo-0.1.6/
+-rw-r--r--   0 sfwwslm   (1000) sfwwslm   (1000)      237 2024-04-02 05:37:19.767175 czo-0.1.6/PKG-INFO
+-rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)       83 2024-03-27 06:33:55.000000 czo-0.1.6/README.md
+-rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)       38 2024-04-02 05:37:19.767175 czo-0.1.6/setup.cfg
+-rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)      394 2024-04-02 05:36:47.000000 czo-0.1.6/setup.py
+drwxrwxr-x   0 sfwwslm   (1000) sfwwslm   (1000)        0 2024-04-02 05:37:19.763174 czo-0.1.6/src/
+drwxrwxr-x   0 sfwwslm   (1000) sfwwslm   (1000)        0 2024-04-02 05:37:19.763174 czo-0.1.6/src/czo/
+-rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)      232 2024-03-31 07:44:26.000000 czo-0.1.6/src/czo/__init__.py
+-rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)     8557 2024-03-27 06:33:55.000000 czo-0.1.6/src/czo/_date.py
+-rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)    12017 2024-03-27 06:33:55.000000 czo-0.1.6/src/czo/_faker.py
+-rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)     5943 2024-04-02 05:36:58.000000 czo-0.1.6/src/czo/_path.py
+-rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)     4781 2024-03-27 06:33:55.000000 czo-0.1.6/src/czo/_rand.py
+drwxrwxr-x   0 sfwwslm   (1000) sfwwslm   (1000)        0 2024-04-02 05:37:19.763174 czo-0.1.6/src/czo/data/
+-rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)        0 2024-03-27 06:33:55.000000 czo-0.1.6/src/czo/data/__init__.py
+-rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)    14519 2024-03-27 06:33:55.000000 czo-0.1.6/src/czo/data/_country.py
+-rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)    16493 2024-03-27 06:33:55.000000 czo-0.1.6/src/czo/data/_housing.py
+-rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)   154755 2024-03-27 06:33:55.000000 czo-0.1.6/src/czo/data/_internal_utils.py
+drwxrwxr-x   0 sfwwslm   (1000) sfwwslm   (1000)        0 2024-04-02 05:37:19.767175 czo-0.1.6/src/czo.egg-info/
+-rw-r--r--   0 sfwwslm   (1000) sfwwslm   (1000)      237 2024-04-02 05:37:19.000000 czo-0.1.6/src/czo.egg-info/PKG-INFO
+-rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)      368 2024-04-02 05:37:19.000000 czo-0.1.6/src/czo.egg-info/SOURCES.txt
+-rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)        1 2024-04-02 05:37:19.000000 czo-0.1.6/src/czo.egg-info/dependency_links.txt
+-rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)       25 2024-04-02 05:37:19.000000 czo-0.1.6/src/czo.egg-info/requires.txt
+-rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)        4 2024-04-02 05:37:19.000000 czo-0.1.6/src/czo.egg-info/top_level.txt
```

### Comparing `czo-0.1.5/src/czo/_date.py` & `czo-0.1.6/src/czo/_date.py`

 * *Files identical despite different names*

### Comparing `czo-0.1.5/src/czo/_faker.py` & `czo-0.1.6/src/czo/_faker.py`

 * *Files identical despite different names*

### Comparing `czo-0.1.5/src/czo/_path.py` & `czo-0.1.6/src/czo/_path.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,15 @@
 
                 if new_path is None:
                     # 如果未指定新路径，则在原路径下重命名
                     new_directory_path = self.directory.parent / new_directory_name
                 else:
                     # 如果指定了新路径，则在新路径下重命名
                     new_path = Path(new_path)
-                    Path.is_none_then_mkdir(new_path)  # 确保新路径存在
+                    PathLib.is_none_then_mkdir(new_path)  # 确保新路径存在
                     new_directory_path: Path = new_path / new_directory_name
 
                 if new_directory_path.exists():
                     serial_number += 1  # 如果新名称已存在，则递增序列号并重试
                     continue
                 else:
                     break  # 找到可用的新名称，退出循环
```

### Comparing `czo-0.1.5/src/czo/_rand.py` & `czo-0.1.6/src/czo/_rand.py`

 * *Files identical despite different names*

### Comparing `czo-0.1.5/src/czo/data/_country.py` & `czo-0.1.6/src/czo/data/_country.py`

 * *Files identical despite different names*

### Comparing `czo-0.1.5/src/czo/data/_housing.py` & `czo-0.1.6/src/czo/data/_housing.py`

 * *Files identical despite different names*

### Comparing `czo-0.1.5/src/czo/data/_internal_utils.py` & `czo-0.1.6/src/czo/data/_internal_utils.py`

 * *Files identical despite different names*

