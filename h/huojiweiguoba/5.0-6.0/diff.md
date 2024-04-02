# Comparing `tmp/huojiweiguoba-5.0.tar.gz` & `tmp/huojiweiguoba-6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huojiweiguoba-5.0.tar", last modified: Tue Apr  2 16:35:12 2024, max compression
+gzip compressed data, was "huojiweiguoba-6.0.tar", last modified: Tue Apr  2 16:44:09 2024, max compression
```

## Comparing `huojiweiguoba-5.0.tar` & `huojiweiguoba-6.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 hwj        (501) staff       (20)        0 2024-04-02 16:35:12.070897 huojiweiguoba-5.0/
--rw-r--r--   0 hwj        (501) staff       (20)     1064 2024-04-02 14:33:19.000000 huojiweiguoba-5.0/LICENSE
--rw-r--r--   0 hwj        (501) staff       (20)      224 2024-04-02 16:35:12.070721 huojiweiguoba-5.0/PKG-INFO
--rw-r--r--   0 hwj        (501) staff       (20)       15 2024-04-02 14:33:19.000000 huojiweiguoba-5.0/README.md
-drwxr-xr-x   0 hwj        (501) staff       (20)        0 2024-04-02 16:35:12.069888 huojiweiguoba-5.0/huojiweiguoba/
--rw-r--r--   0 hwj        (501) staff       (20)        0 2024-04-02 14:33:19.000000 huojiweiguoba-5.0/huojiweiguoba/__init__.py
--rw-r--r--   0 hwj        (501) staff       (20)      106 2024-04-02 14:33:19.000000 huojiweiguoba-5.0/huojiweiguoba/lbw.py
--rw-r--r--   0 hwj        (501) staff       (20)      593 2024-04-02 14:33:19.000000 huojiweiguoba-5.0/huojiweiguoba/lbw_datetime.py
--rw-r--r--   0 hwj        (501) staff       (20)      304 2024-04-02 14:33:19.000000 huojiweiguoba-5.0/huojiweiguoba/lbw_excel.py
--rw-r--r--   0 hwj        (501) staff       (20)      307 2024-04-02 14:33:19.000000 huojiweiguoba-5.0/huojiweiguoba/lbw_json.py
--rw-r--r--   0 hwj        (501) staff       (20)      458 2024-04-02 14:33:19.000000 huojiweiguoba-5.0/huojiweiguoba/lbw_math.py
--rw-r--r--   0 hwj        (501) staff       (20)      907 2024-04-02 14:33:19.000000 huojiweiguoba-5.0/huojiweiguoba/lbw_token.py
--rw-r--r--   0 hwj        (501) staff       (20)     3115 2024-04-02 16:34:52.000000 huojiweiguoba-5.0/huojiweiguoba/lbw_xbds.py
--rw-r--r--   0 hwj        (501) staff       (20)      419 2024-04-02 14:33:19.000000 huojiweiguoba-5.0/huojiweiguoba/main.py
-drwxr-xr-x   0 hwj        (501) staff       (20)        0 2024-04-02 16:35:12.070527 huojiweiguoba-5.0/huojiweiguoba.egg-info/
--rw-r--r--   0 hwj        (501) staff       (20)      224 2024-04-02 16:35:12.000000 huojiweiguoba-5.0/huojiweiguoba.egg-info/PKG-INFO
--rw-r--r--   0 hwj        (501) staff       (20)      405 2024-04-02 16:35:12.000000 huojiweiguoba-5.0/huojiweiguoba.egg-info/SOURCES.txt
--rw-r--r--   0 hwj        (501) staff       (20)        1 2024-04-02 16:35:12.000000 huojiweiguoba-5.0/huojiweiguoba.egg-info/dependency_links.txt
--rw-r--r--   0 hwj        (501) staff       (20)       14 2024-04-02 16:35:12.000000 huojiweiguoba-5.0/huojiweiguoba.egg-info/top_level.txt
--rw-r--r--   0 hwj        (501) staff       (20)       38 2024-04-02 16:35:12.070937 huojiweiguoba-5.0/setup.cfg
--rw-r--r--   0 hwj        (501) staff       (20)      990 2024-04-02 16:35:02.000000 huojiweiguoba-5.0/setup.py
+drwxr-xr-x   0 hwj        (501) staff       (20)        0 2024-04-02 16:44:09.243353 huojiweiguoba-6.0/
+-rw-r--r--   0 hwj        (501) staff       (20)     1064 2024-04-02 14:33:19.000000 huojiweiguoba-6.0/LICENSE
+-rw-r--r--   0 hwj        (501) staff       (20)      224 2024-04-02 16:44:09.243168 huojiweiguoba-6.0/PKG-INFO
+-rw-r--r--   0 hwj        (501) staff       (20)       15 2024-04-02 14:33:19.000000 huojiweiguoba-6.0/README.md
+drwxr-xr-x   0 hwj        (501) staff       (20)        0 2024-04-02 16:44:09.242334 huojiweiguoba-6.0/huojiweiguoba/
+-rw-r--r--   0 hwj        (501) staff       (20)        0 2024-04-02 14:33:19.000000 huojiweiguoba-6.0/huojiweiguoba/__init__.py
+-rw-r--r--   0 hwj        (501) staff       (20)      106 2024-04-02 14:33:19.000000 huojiweiguoba-6.0/huojiweiguoba/lbw.py
+-rw-r--r--   0 hwj        (501) staff       (20)      593 2024-04-02 14:33:19.000000 huojiweiguoba-6.0/huojiweiguoba/lbw_datetime.py
+-rw-r--r--   0 hwj        (501) staff       (20)      304 2024-04-02 14:33:19.000000 huojiweiguoba-6.0/huojiweiguoba/lbw_excel.py
+-rw-r--r--   0 hwj        (501) staff       (20)      307 2024-04-02 14:33:19.000000 huojiweiguoba-6.0/huojiweiguoba/lbw_json.py
+-rw-r--r--   0 hwj        (501) staff       (20)      458 2024-04-02 14:33:19.000000 huojiweiguoba-6.0/huojiweiguoba/lbw_math.py
+-rw-r--r--   0 hwj        (501) staff       (20)      907 2024-04-02 14:33:19.000000 huojiweiguoba-6.0/huojiweiguoba/lbw_token.py
+-rw-r--r--   0 hwj        (501) staff       (20)     3135 2024-04-02 16:43:18.000000 huojiweiguoba-6.0/huojiweiguoba/lbw_xbds.py
+-rw-r--r--   0 hwj        (501) staff       (20)      419 2024-04-02 14:33:19.000000 huojiweiguoba-6.0/huojiweiguoba/main.py
+drwxr-xr-x   0 hwj        (501) staff       (20)        0 2024-04-02 16:44:09.242987 huojiweiguoba-6.0/huojiweiguoba.egg-info/
+-rw-r--r--   0 hwj        (501) staff       (20)      224 2024-04-02 16:44:09.000000 huojiweiguoba-6.0/huojiweiguoba.egg-info/PKG-INFO
+-rw-r--r--   0 hwj        (501) staff       (20)      405 2024-04-02 16:44:09.000000 huojiweiguoba-6.0/huojiweiguoba.egg-info/SOURCES.txt
+-rw-r--r--   0 hwj        (501) staff       (20)        1 2024-04-02 16:44:09.000000 huojiweiguoba-6.0/huojiweiguoba.egg-info/dependency_links.txt
+-rw-r--r--   0 hwj        (501) staff       (20)       14 2024-04-02 16:44:09.000000 huojiweiguoba-6.0/huojiweiguoba.egg-info/top_level.txt
+-rw-r--r--   0 hwj        (501) staff       (20)       38 2024-04-02 16:44:09.243399 huojiweiguoba-6.0/setup.cfg
+-rw-r--r--   0 hwj        (501) staff       (20)      990 2024-04-02 16:43:51.000000 huojiweiguoba-6.0/setup.py
```

### Comparing `huojiweiguoba-5.0/LICENSE` & `huojiweiguoba-6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `huojiweiguoba-5.0/huojiweiguoba/lbw_datetime.py` & `huojiweiguoba-6.0/huojiweiguoba/lbw_datetime.py`

 * *Files identical despite different names*

### Comparing `huojiweiguoba-5.0/huojiweiguoba/lbw_token.py` & `huojiweiguoba-6.0/huojiweiguoba/lbw_token.py`

 * *Files identical despite different names*

### Comparing `huojiweiguoba-5.0/huojiweiguoba/lbw_xbds.py` & `huojiweiguoba-6.0/huojiweiguoba/lbw_xbds.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from dotenv import find_dotenv, load_dotenv
 from playhouse.shortcuts import ReconnectMixin
 from playhouse.pool import PooledMySQLDatabase
 
 root_dir = None
 def set_root_dir(path):
     '''设置根目录'''
+    global root_dir
     root_dir = path
 
 
 env_path = find_dotenv()
 assert env_path, "Not found .env file"
 load_dotenv(env_path)
 assert os.getenv('HOST'), "HOST is None"
```

### Comparing `huojiweiguoba-5.0/setup.py` & `huojiweiguoba-6.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="huojiweiguoba",  # 模块名称
-    version="5.0",  # 当前版本
+    version="6.0",  # 当前版本
     author="lbw",  # 作者
     author_email="819577544@qq.com",  # 作者邮箱
     description="人生有梦 各自精彩",  # 模块简介
     long_description=long_description,  # 模块详细介绍
     # long_description_content_type="text/markdown",  # 模块详细介绍格式
     url="https://github.com/ycyxycm/huojiweiguoba",  # 模块github地址
     packages=setuptools.find_packages(),  # 自动找到项目中导入的模块
```

