# Comparing `tmp/muti.numer-0.0.2.tar.gz` & `tmp/muti.numer-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muti.numer-0.0.2.tar", last modified: Tue Apr  2 06:36:22 2024, max compression
+gzip compressed data, was "muti.numer-0.0.3.tar", last modified: Tue Apr  2 06:50:10 2024, max compression
```

## Comparing `muti.numer-0.0.2.tar` & `muti.numer-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 06:36:22.213399 muti.numer-0.0.2/
--rw-rw-rw-   0        0        0     1089 2024-03-22 08:37:41.000000 muti.numer-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      767 2024-04-02 06:36:22.213399 muti.numer-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      346 2024-03-29 10:24:16.000000 muti.numer-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 06:36:22.212399 muti.numer-0.0.2/muti.numer.egg-info/
--rw-rw-rw-   0        0        0      767 2024-04-02 06:36:22.000000 muti.numer-0.0.2/muti.numer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2024-04-02 06:36:22.000000 muti.numer-0.0.2/muti.numer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 06:36:22.000000 muti.numer-0.0.2/muti.numer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-02 06:36:22.000000 muti.numer-0.0.2/muti.numer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-02 06:36:22.212399 muti.numer-0.0.2/numer/
--rw-rw-rw-   0        0        0     1301 2024-04-02 03:02:54.000000 muti.numer-0.0.2/numer/__deps__.py
--rw-rw-rw-   0        0        0      560 2024-04-02 06:34:31.000000 muti.numer-0.0.2/numer/__init__.py
--rw-rw-rw-   0        0        0        0 2024-03-29 07:33:09.000000 muti.numer-0.0.2/numer/conLam.py
--rw-rw-rw-   0        0        0     2325 2024-04-02 06:23:15.000000 muti.numer-0.0.2/numer/depLam.py
--rw-rw-rw-   0        0        0      902 2024-04-01 09:32:26.000000 muti.numer-0.0.2/numer/iniLam.py
--rw-rw-rw-   0        0        0     1746 2024-04-02 06:10:40.000000 muti.numer-0.0.2/numer/modLas.py
--rw-rw-rw-   0        0        0    11573 2024-04-02 05:31:41.000000 muti.numer-0.0.2/numer/shfLam.py
--rw-rw-rw-   0        0        0        0 2024-03-29 07:33:52.000000 muti.numer-0.0.2/numer/updLam.py
--rw-rw-rw-   0        0        0       42 2024-04-02 06:36:22.213399 muti.numer-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      653 2024-04-02 06:35:01.000000 muti.numer-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 06:50:10.013462 muti.numer-0.0.3/
+-rw-rw-rw-   0        0        0     1089 2024-03-22 08:37:41.000000 muti.numer-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      767 2024-04-02 06:50:10.012216 muti.numer-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2024-03-29 10:24:16.000000 muti.numer-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 06:50:10.012216 muti.numer-0.0.3/muti.numer.egg-info/
+-rw-rw-rw-   0        0        0      767 2024-04-02 06:50:09.000000 muti.numer-0.0.3/muti.numer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2024-04-02 06:50:09.000000 muti.numer-0.0.3/muti.numer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 06:50:09.000000 muti.numer-0.0.3/muti.numer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-02 06:50:09.000000 muti.numer-0.0.3/muti.numer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 06:50:10.011218 muti.numer-0.0.3/numer/
+-rw-rw-rw-   0        0        0     1300 2024-04-02 06:48:06.000000 muti.numer-0.0.3/numer/__deps__.py
+-rw-rw-rw-   0        0        0      562 2024-04-02 06:49:33.000000 muti.numer-0.0.3/numer/__init__.py
+-rw-rw-rw-   0        0        0     2326 2024-04-02 06:48:19.000000 muti.numer-0.0.3/numer/depLam.py
+-rw-rw-rw-   0        0        0      903 2024-04-02 06:49:59.000000 muti.numer-0.0.3/numer/iniLam.py
+-rw-rw-rw-   0        0        0     1748 2024-04-02 06:49:13.000000 muti.numer-0.0.3/numer/modLas.py
+-rw-rw-rw-   0        0        0    11574 2024-04-02 06:48:45.000000 muti.numer-0.0.3/numer/shfLam.py
+-rw-rw-rw-   0        0        0       42 2024-04-02 06:50:10.013462 muti.numer-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      653 2024-04-02 06:49:58.000000 muti.numer-0.0.3/setup.py
```

### Comparing `muti.numer-0.0.2/LICENSE` & `muti.numer-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `muti.numer-0.0.2/PKG-INFO` & `muti.numer-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muti.numer
-Version: 0.0.2
+Version: 0.0.3
 Summary: utils for math-numer
 Home-page: https://github.com/E-C-Ares/
 Author: E.C.Ares
 Author-email: E.C.Ares@outlook.com
 License: MIT DIVIƷON
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `muti.numer-0.0.2/muti.numer.egg-info/PKG-INFO` & `muti.numer-0.0.3/muti.numer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muti.numer
-Version: 0.0.2
+Version: 0.0.3
 Summary: utils for math-numer
 Home-page: https://github.com/E-C-Ares/
 Author: E.C.Ares
 Author-email: E.C.Ares@outlook.com
 License: MIT DIVIƷON
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `muti.numer-0.0.2/numer/__deps__.py` & `muti.numer-0.0.3/numer/__deps__.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 _fc  =   os.getenv( 'FC_IMP')
 if  bas.ist(_fc,NON) or _fc== '': _fc='tn'
 if 'j' in _fc:
     import jax       as nmb
     import jax.numpy as nmp
     import jax.nn    as nmm
 if 'h' in _fc:
-    import haiku     as nmm
+    pass
+    #import haiku     as nmm
 if 't' in _fc:
     import torch     as nmb
     import torch.nn  as nmm
 if 'n' in _fc:
     import numpy     as nmp
 # t
 ist  =  bas.ist
@@ -43,23 +44,17 @@
     import torch     as nmb
     import torch.nn  as nmm
   if 'n' in _fc:
     import numpy     as nmp
 setnImp( os.getenv( 'FC_IMP'))
 '''
 
-
-
 # FIXME Jax
 TYP[50] = nmb.Tensor
 TYP[60] = nmm.Module
 Unm_sox = Union[TYP[50],TYP[60]]
 
 
-
-
-
-
 #mod = lambda x: phk.transform(x) if else
 # = lambda y: y
     
 if bas.Her(__name__): pass
```

### Comparing `muti.numer-0.0.2/numer/__init__.py` & `muti.numer-0.0.3/numer/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,12 +5,12 @@
 # core.numer
 from .depLam import *
 # 形式转换: mod\dat 放置到 MEM\CPU\GPU\.. ; .tensor .ndarrray 等类转换
 from .iniLam import *
 # 更新 pln or BW\OPT| loss.backward() 网络反向传播, 优化器更新
 from .shfLam import *
 # 初化 for model\optimizer : Model(arg_model)\Optimizer(arg_opt, model.parameters())
-from .updLam import *
+#from .updLam import *
 # 算路              | y = mod.forward(x) : mod = ModLas(cfg)
 from .modLas import *
 # 特函 esp.Los·拉形 | los(y, y')         : los = LosLam(cfg) 
-from .conLam import *
+#from .conLam import *
```

### Comparing `muti.numer-0.0.2/numer/depLam.py` & `muti.numer-0.0.3/numer/depLam.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
  #  num-muti :: dep-lam 依函集
  @  E.C.Ares
  !  MIT DIVIƷON
  `  Lam of deps builtin numer-python
 """
 
-from __deps__ import *
+from .__deps__ import *
 
 
 
 
 # 主要是激活函数名
 _JC_NYM=dict(
     tah='tanh',
```

### Comparing `muti.numer-0.0.2/numer/iniLam.py` & `muti.numer-0.0.3/numer/iniLam.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
  #  bas-muti :: ini-lam 初函集
  @  E.C.Ares
  !  MIT DIVIƷON
  `  Lam of init builtin numer-python
 """
 
-from depLam import *
+from .depLam import *
 # ARES FIXME : nan; 
 def initMod(_nn_mod, _nn_ini_):
   _nn_ini_['bia'](_nn_mod.bias.data)
   _nn_ini_['wei'](_nn_mod.weight.data)
   return _nn_mod
 
 # [22W12] ARES
```

### Comparing `muti.numer-0.0.2/numer/modLas.py` & `muti.numer-0.0.3/numer/modLas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # 
 from   argparse import Namespace as Nym
 import   torch                  as nmb
-from              iniLam import *
-from              shfLam import *
+from              .iniLam import *
+from              .shfLam import *
 
 
 
 class   UMA(nmm.Module):
     def __init__(self, cfx):
         super().__init__()
         self.setnPar(cfx)    # 参数解析
```

### Comparing `muti.numer-0.0.2/numer/shfLam.py` & `muti.numer-0.0.3/numer/shfLam.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
  #  转换函数 shf-lams
  @  E.C.Ares
  !  MIT LICENSE
  `  built in pkp for pyTorch tensor
 """
 # r(import-refs)
 #       r.. im
-from iniLam import *
+from .iniLam import *
 #       r.. as
 pass
 # s
 _JC_NYM = 'lam_shf'
 # to.() = 畨 娄
 _KY_    = ['dtype','device']
 _LC_TAN = ['train','drop','tre',TYP[60].train]
```

### Comparing `muti.numer-0.0.2/setup.py` & `muti.numer-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   url          = "https://github.com/E-C-Ares/",
   name         = "muti.numer",
-  version      = "0.0.2",
+  version      = "0.0.3",
   author       = "E.C.Ares",
   author_email = "E.C.Ares@outlook.com",
   license      = 'MIT DIVIƷON',
   description  = "utils for math-numer",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages     = setuptools.find_packages(),
```

