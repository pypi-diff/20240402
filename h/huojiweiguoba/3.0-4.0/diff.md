# Comparing `tmp/huojiweiguoba-3.0.tar.gz` & `tmp/huojiweiguoba-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huojiweiguoba-3.0.tar", last modified: Wed Dec 27 06:42:12 2023, max compression
+gzip compressed data, was "huojiweiguoba-4.0.tar", last modified: Tue Apr  2 16:18:23 2024, max compression
```

## Comparing `huojiweiguoba-3.0.tar` & `huojiweiguoba-4.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 hwj        (501) staff       (20)        0 2023-12-27 06:42:12.279466 huojiweiguoba-3.0/
--rw-r--r--   0 hwj        (501) staff       (20)     1064 2023-12-27 06:35:34.000000 huojiweiguoba-3.0/LICENSE
--rw-r--r--   0 hwj        (501) staff       (20)      219 2023-12-27 06:42:12.279285 huojiweiguoba-3.0/PKG-INFO
--rw-r--r--   0 hwj        (501) staff       (20)       15 2023-12-27 06:35:34.000000 huojiweiguoba-3.0/README.md
-drwxr-xr-x   0 hwj        (501) staff       (20)        0 2023-12-27 06:42:12.278468 huojiweiguoba-3.0/huojiweiguoba/
--rw-r--r--   0 hwj        (501) staff       (20)        0 2023-12-27 06:35:34.000000 huojiweiguoba-3.0/huojiweiguoba/__init__.py
--rw-r--r--   0 hwj        (501) staff       (20)      106 2023-12-27 06:35:34.000000 huojiweiguoba-3.0/huojiweiguoba/lbw.py
--rw-r--r--   0 hwj        (501) staff       (20)      593 2023-12-27 06:35:34.000000 huojiweiguoba-3.0/huojiweiguoba/lbw_datetime.py
--rw-r--r--   0 hwj        (501) staff       (20)      304 2023-12-27 06:35:34.000000 huojiweiguoba-3.0/huojiweiguoba/lbw_excel.py
--rw-r--r--   0 hwj        (501) staff       (20)      307 2023-12-27 06:35:34.000000 huojiweiguoba-3.0/huojiweiguoba/lbw_json.py
--rw-r--r--   0 hwj        (501) staff       (20)      458 2023-12-27 06:35:34.000000 huojiweiguoba-3.0/huojiweiguoba/lbw_math.py
--rw-r--r--   0 hwj        (501) staff       (20)      907 2023-12-27 06:40:11.000000 huojiweiguoba-3.0/huojiweiguoba/lbw_token.py
--rw-r--r--   0 hwj        (501) staff       (20)      419 2023-12-27 06:35:34.000000 huojiweiguoba-3.0/huojiweiguoba/main.py
-drwxr-xr-x   0 hwj        (501) staff       (20)        0 2023-12-27 06:42:12.279122 huojiweiguoba-3.0/huojiweiguoba.egg-info/
--rw-r--r--   0 hwj        (501) staff       (20)      219 2023-12-27 06:42:12.000000 huojiweiguoba-3.0/huojiweiguoba.egg-info/PKG-INFO
--rw-r--r--   0 hwj        (501) staff       (20)      379 2023-12-27 06:42:12.000000 huojiweiguoba-3.0/huojiweiguoba.egg-info/SOURCES.txt
--rw-r--r--   0 hwj        (501) staff       (20)        1 2023-12-27 06:42:12.000000 huojiweiguoba-3.0/huojiweiguoba.egg-info/dependency_links.txt
--rw-r--r--   0 hwj        (501) staff       (20)       14 2023-12-27 06:42:12.000000 huojiweiguoba-3.0/huojiweiguoba.egg-info/top_level.txt
--rw-r--r--   0 hwj        (501) staff       (20)       38 2023-12-27 06:42:12.279514 huojiweiguoba-3.0/setup.cfg
--rw-r--r--   0 hwj        (501) staff       (20)      985 2023-12-27 06:42:09.000000 huojiweiguoba-3.0/setup.py
+drwxr-xr-x   0 hwj        (501) staff       (20)        0 2024-04-02 16:18:23.317242 huojiweiguoba-4.0/
+-rw-r--r--   0 hwj        (501) staff       (20)     1064 2024-04-02 14:33:19.000000 huojiweiguoba-4.0/LICENSE
+-rw-r--r--   0 hwj        (501) staff       (20)      224 2024-04-02 16:18:23.317070 huojiweiguoba-4.0/PKG-INFO
+-rw-r--r--   0 hwj        (501) staff       (20)       15 2024-04-02 14:33:19.000000 huojiweiguoba-4.0/README.md
+drwxr-xr-x   0 hwj        (501) staff       (20)        0 2024-04-02 16:18:23.316227 huojiweiguoba-4.0/huojiweiguoba/
+-rw-r--r--   0 hwj        (501) staff       (20)        0 2024-04-02 14:33:19.000000 huojiweiguoba-4.0/huojiweiguoba/__init__.py
+-rw-r--r--   0 hwj        (501) staff       (20)      106 2024-04-02 14:33:19.000000 huojiweiguoba-4.0/huojiweiguoba/lbw.py
+-rw-r--r--   0 hwj        (501) staff       (20)      593 2024-04-02 14:33:19.000000 huojiweiguoba-4.0/huojiweiguoba/lbw_datetime.py
+-rw-r--r--   0 hwj        (501) staff       (20)      304 2024-04-02 14:33:19.000000 huojiweiguoba-4.0/huojiweiguoba/lbw_excel.py
+-rw-r--r--   0 hwj        (501) staff       (20)      307 2024-04-02 14:33:19.000000 huojiweiguoba-4.0/huojiweiguoba/lbw_json.py
+-rw-r--r--   0 hwj        (501) staff       (20)      458 2024-04-02 14:33:19.000000 huojiweiguoba-4.0/huojiweiguoba/lbw_math.py
+-rw-r--r--   0 hwj        (501) staff       (20)      907 2024-04-02 14:33:19.000000 huojiweiguoba-4.0/huojiweiguoba/lbw_token.py
+-rw-r--r--   0 hwj        (501) staff       (20)     3066 2024-04-02 16:15:38.000000 huojiweiguoba-4.0/huojiweiguoba/lbw_xbds.py
+-rw-r--r--   0 hwj        (501) staff       (20)      419 2024-04-02 14:33:19.000000 huojiweiguoba-4.0/huojiweiguoba/main.py
+drwxr-xr-x   0 hwj        (501) staff       (20)        0 2024-04-02 16:18:23.316914 huojiweiguoba-4.0/huojiweiguoba.egg-info/
+-rw-r--r--   0 hwj        (501) staff       (20)      224 2024-04-02 16:18:23.000000 huojiweiguoba-4.0/huojiweiguoba.egg-info/PKG-INFO
+-rw-r--r--   0 hwj        (501) staff       (20)      405 2024-04-02 16:18:23.000000 huojiweiguoba-4.0/huojiweiguoba.egg-info/SOURCES.txt
+-rw-r--r--   0 hwj        (501) staff       (20)        1 2024-04-02 16:18:23.000000 huojiweiguoba-4.0/huojiweiguoba.egg-info/dependency_links.txt
+-rw-r--r--   0 hwj        (501) staff       (20)       14 2024-04-02 16:18:23.000000 huojiweiguoba-4.0/huojiweiguoba.egg-info/top_level.txt
+-rw-r--r--   0 hwj        (501) staff       (20)       38 2024-04-02 16:18:23.317280 huojiweiguoba-4.0/setup.cfg
+-rw-r--r--   0 hwj        (501) staff       (20)      990 2024-04-02 16:17:54.000000 huojiweiguoba-4.0/setup.py
```

### Comparing `huojiweiguoba-3.0/LICENSE` & `huojiweiguoba-4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `huojiweiguoba-3.0/huojiweiguoba/lbw_datetime.py` & `huojiweiguoba-4.0/huojiweiguoba/lbw_datetime.py`

 * *Files identical despite different names*

### Comparing `huojiweiguoba-3.0/huojiweiguoba/lbw_token.py` & `huojiweiguoba-4.0/huojiweiguoba/lbw_token.py`

 * *Files identical despite different names*

### Comparing `huojiweiguoba-3.0/setup.py` & `huojiweiguoba-4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="huojiweiguoba",  # 模块名称
-    version="3.0",  # 当前版本
+    version="4.0",  # 当前版本
     author="lbw",  # 作者
     author_email="819577544@qq.com",  # 作者邮箱
-    description="一个非常NB的包",  # 模块简介
+    description="人生有梦 各自精彩",  # 模块简介
     long_description=long_description,  # 模块详细介绍
     # long_description_content_type="text/markdown",  # 模块详细介绍格式
     url="https://github.com/ycyxycm/huojiweiguoba",  # 模块github地址
     packages=setuptools.find_packages(),  # 自动找到项目中导入的模块
     # 模块相关的元数据
     # classifiers=[
     #     "Programming Language :: Python :: 3",
```

