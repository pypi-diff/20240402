# Comparing `tmp/muti.numer-0.0.1.tar.gz` & `tmp/muti.numer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muti.numer-0.0.1.tar", last modified: Tue Apr  2 06:24:02 2024, max compression
+gzip compressed data, was "muti.numer-0.0.2.tar", last modified: Tue Apr  2 06:36:22 2024, max compression
```

## Comparing `muti.numer-0.0.1.tar` & `muti.numer-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 06:24:02.458356 muti.numer-0.0.1/
--rw-rw-rw-   0        0        0     1089 2024-03-22 08:37:41.000000 muti.numer-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      767 2024-04-02 06:24:02.457357 muti.numer-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      346 2024-03-29 10:24:16.000000 muti.numer-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 06:24:02.457357 muti.numer-0.0.1/muti.numer.egg-info/
--rw-rw-rw-   0        0        0      767 2024-04-02 06:24:02.000000 muti.numer-0.0.1/muti.numer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2024-04-02 06:24:02.000000 muti.numer-0.0.1/muti.numer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 06:24:02.000000 muti.numer-0.0.1/muti.numer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-02 06:24:02.000000 muti.numer-0.0.1/muti.numer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-02 06:24:02.456356 muti.numer-0.0.1/numer/
--rw-rw-rw-   0        0        0     1301 2024-04-02 03:02:54.000000 muti.numer-0.0.1/numer/__deps__.py
--rw-rw-rw-   0        0        0      537 2024-04-01 01:49:04.000000 muti.numer-0.0.1/numer/__init__.py
--rw-rw-rw-   0        0        0        0 2024-03-29 07:33:09.000000 muti.numer-0.0.1/numer/conLam.py
--rw-rw-rw-   0        0        0     2325 2024-04-02 06:23:15.000000 muti.numer-0.0.1/numer/depLam.py
--rw-rw-rw-   0        0        0      902 2024-04-01 09:32:26.000000 muti.numer-0.0.1/numer/iniLam.py
--rw-rw-rw-   0        0        0     1746 2024-04-02 06:10:40.000000 muti.numer-0.0.1/numer/modLas.py
--rw-rw-rw-   0        0        0    11573 2024-04-02 05:31:41.000000 muti.numer-0.0.1/numer/shfLam.py
--rw-rw-rw-   0        0        0        0 2024-03-29 07:33:52.000000 muti.numer-0.0.1/numer/updLam.py
--rw-rw-rw-   0        0        0       42 2024-04-02 06:24:02.458356 muti.numer-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      653 2024-04-02 06:24:00.000000 muti.numer-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 06:36:22.213399 muti.numer-0.0.2/
+-rw-rw-rw-   0        0        0     1089 2024-03-22 08:37:41.000000 muti.numer-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      767 2024-04-02 06:36:22.213399 muti.numer-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2024-03-29 10:24:16.000000 muti.numer-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 06:36:22.212399 muti.numer-0.0.2/muti.numer.egg-info/
+-rw-rw-rw-   0        0        0      767 2024-04-02 06:36:22.000000 muti.numer-0.0.2/muti.numer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2024-04-02 06:36:22.000000 muti.numer-0.0.2/muti.numer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 06:36:22.000000 muti.numer-0.0.2/muti.numer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-02 06:36:22.000000 muti.numer-0.0.2/muti.numer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 06:36:22.212399 muti.numer-0.0.2/numer/
+-rw-rw-rw-   0        0        0     1301 2024-04-02 03:02:54.000000 muti.numer-0.0.2/numer/__deps__.py
+-rw-rw-rw-   0        0        0      560 2024-04-02 06:34:31.000000 muti.numer-0.0.2/numer/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-03-29 07:33:09.000000 muti.numer-0.0.2/numer/conLam.py
+-rw-rw-rw-   0        0        0     2325 2024-04-02 06:23:15.000000 muti.numer-0.0.2/numer/depLam.py
+-rw-rw-rw-   0        0        0      902 2024-04-01 09:32:26.000000 muti.numer-0.0.2/numer/iniLam.py
+-rw-rw-rw-   0        0        0     1746 2024-04-02 06:10:40.000000 muti.numer-0.0.2/numer/modLas.py
+-rw-rw-rw-   0        0        0    11573 2024-04-02 05:31:41.000000 muti.numer-0.0.2/numer/shfLam.py
+-rw-rw-rw-   0        0        0        0 2024-03-29 07:33:52.000000 muti.numer-0.0.2/numer/updLam.py
+-rw-rw-rw-   0        0        0       42 2024-04-02 06:36:22.213399 muti.numer-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      653 2024-04-02 06:35:01.000000 muti.numer-0.0.2/setup.py
```

### Comparing `muti.numer-0.0.1/LICENSE` & `muti.numer-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `muti.numer-0.0.1/PKG-INFO` & `muti.numer-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muti.numer
-Version: 0.0.1
+Version: 0.0.2
 Summary: utils for math-numer
 Home-page: https://github.com/E-C-Ares/
 Author: E.C.Ares
 Author-email: E.C.Ares@outlook.com
 License: MIT DIVIƷON
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `muti.numer-0.0.1/muti.numer.egg-info/PKG-INFO` & `muti.numer-0.0.2/muti.numer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muti.numer
-Version: 0.0.1
+Version: 0.0.2
 Summary: utils for math-numer
 Home-page: https://github.com/E-C-Ares/
 Author: E.C.Ares
 Author-email: E.C.Ares@outlook.com
 License: MIT DIVIƷON
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `muti.numer-0.0.1/numer/__deps__.py` & `muti.numer-0.0.2/numer/__deps__.py`

 * *Files identical despite different names*

### Comparing `muti.numer-0.0.1/numer/__init__.py` & `muti.numer-0.0.2/numer/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 _JC_NYM = "muti.torch"
 
 
 
 # core.numer
+from .depLam import *
 # 形式转换: mod\dat 放置到 MEM\CPU\GPU\.. ; .tensor .ndarrray 等类转换
 from .iniLam import *
 # 更新 pln or BW\OPT| loss.backward() 网络反向传播, 优化器更新
 from .shfLam import *
 # 初化 for model\optimizer : Model(arg_model)\Optimizer(arg_opt, model.parameters())
 from .updLam import *
 # 算路              | y = mod.forward(x) : mod = ModLas(cfg)
```

### Comparing `muti.numer-0.0.1/numer/depLam.py` & `muti.numer-0.0.2/numer/depLam.py`

 * *Files identical despite different names*

### Comparing `muti.numer-0.0.1/numer/iniLam.py` & `muti.numer-0.0.2/numer/iniLam.py`

 * *Files identical despite different names*

### Comparing `muti.numer-0.0.1/numer/modLas.py` & `muti.numer-0.0.2/numer/modLas.py`

 * *Files identical despite different names*

### Comparing `muti.numer-0.0.1/numer/shfLam.py` & `muti.numer-0.0.2/numer/shfLam.py`

 * *Files identical despite different names*

### Comparing `muti.numer-0.0.1/setup.py` & `muti.numer-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   url          = "https://github.com/E-C-Ares/",
   name         = "muti.numer",
-  version      = "0.0.1",
+  version      = "0.0.2",
   author       = "E.C.Ares",
   author_email = "E.C.Ares@outlook.com",
   license      = 'MIT DIVIƷON',
   description  = "utils for math-numer",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages     = setuptools.find_packages(),
```

