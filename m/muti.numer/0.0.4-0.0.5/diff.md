# Comparing `tmp/muti.numer-0.0.4.tar.gz` & `tmp/muti.numer-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muti.numer-0.0.4.tar", last modified: Tue Apr  2 07:19:34 2024, max compression
+gzip compressed data, was "muti.numer-0.0.5.tar", last modified: Tue Apr  2 08:50:55 2024, max compression
```

## Comparing `muti.numer-0.0.4.tar` & `muti.numer-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 07:19:34.824556 muti.numer-0.0.4/
--rw-rw-rw-   0        0        0     1089 2024-03-22 08:37:41.000000 muti.numer-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      767 2024-04-02 07:19:34.823556 muti.numer-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      346 2024-03-29 10:24:16.000000 muti.numer-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 07:19:34.823556 muti.numer-0.0.4/muti.numer.egg-info/
--rw-rw-rw-   0        0        0      767 2024-04-02 07:19:34.000000 muti.numer-0.0.4/muti.numer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2024-04-02 07:19:34.000000 muti.numer-0.0.4/muti.numer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 07:19:34.000000 muti.numer-0.0.4/muti.numer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-02 07:19:34.000000 muti.numer-0.0.4/muti.numer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-02 07:19:34.822557 muti.numer-0.0.4/numer/
--rw-rw-rw-   0        0        0     1300 2024-04-02 06:48:06.000000 muti.numer-0.0.4/numer/__deps__.py
--rw-rw-rw-   0        0        0      562 2024-04-02 06:49:33.000000 muti.numer-0.0.4/numer/__init__.py
--rw-rw-rw-   0        0        0     2326 2024-04-02 06:48:19.000000 muti.numer-0.0.4/numer/depLam.py
--rw-rw-rw-   0        0        0      903 2024-04-02 06:49:59.000000 muti.numer-0.0.4/numer/iniLam.py
--rw-rw-rw-   0        0        0     1762 2024-04-02 07:18:35.000000 muti.numer-0.0.4/numer/modLas.py
--rw-rw-rw-   0        0        0    11574 2024-04-02 06:48:45.000000 muti.numer-0.0.4/numer/shfLam.py
--rw-rw-rw-   0        0        0       42 2024-04-02 07:19:34.824556 muti.numer-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      653 2024-04-02 07:19:24.000000 muti.numer-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 08:50:55.553149 muti.numer-0.0.5/
+-rw-rw-rw-   0        0        0     1089 2024-03-22 08:37:41.000000 muti.numer-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      767 2024-04-02 08:50:55.553149 muti.numer-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2024-03-29 10:24:16.000000 muti.numer-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 08:50:55.552148 muti.numer-0.0.5/muti.numer.egg-info/
+-rw-rw-rw-   0        0        0      767 2024-04-02 08:50:55.000000 muti.numer-0.0.5/muti.numer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2024-04-02 08:50:55.000000 muti.numer-0.0.5/muti.numer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 08:50:55.000000 muti.numer-0.0.5/muti.numer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-02 08:50:55.000000 muti.numer-0.0.5/muti.numer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 08:50:55.551148 muti.numer-0.0.5/numer/
+-rw-rw-rw-   0        0        0     1348 2024-04-02 08:47:13.000000 muti.numer-0.0.5/numer/__deps__.py
+-rw-rw-rw-   0        0        0      562 2024-04-02 06:49:33.000000 muti.numer-0.0.5/numer/__init__.py
+-rw-rw-rw-   0        0        0     2326 2024-04-02 06:48:19.000000 muti.numer-0.0.5/numer/depLam.py
+-rw-rw-rw-   0        0        0      903 2024-04-02 08:49:06.000000 muti.numer-0.0.5/numer/iniLam.py
+-rw-rw-rw-   0        0        0     1765 2024-04-02 08:48:37.000000 muti.numer-0.0.5/numer/modLas.py
+-rw-rw-rw-   0        0        0    11583 2024-04-02 08:40:13.000000 muti.numer-0.0.5/numer/shfLam.py
+-rw-rw-rw-   0        0        0       42 2024-04-02 08:50:55.554148 muti.numer-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      653 2024-04-02 08:50:52.000000 muti.numer-0.0.5/setup.py
```

### Comparing `muti.numer-0.0.4/LICENSE` & `muti.numer-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `muti.numer-0.0.4/PKG-INFO` & `muti.numer-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muti.numer
-Version: 0.0.4
+Version: 0.0.5
 Summary: utils for math-numer
 Home-page: https://github.com/E-C-Ares/
 Author: E.C.Ares
 Author-email: E.C.Ares@outlook.com
 License: MIT DIVIƷON
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `muti.numer-0.0.4/muti.numer.egg-info/PKG-INFO` & `muti.numer-0.0.5/muti.numer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muti.numer
-Version: 0.0.4
+Version: 0.0.5
 Summary: utils for math-numer
 Home-page: https://github.com/E-C-Ares/
 Author: E.C.Ares
 Author-email: E.C.Ares@outlook.com
 License: MIT DIVIƷON
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `muti.numer-0.0.4/numer/__deps__.py` & `muti.numer-0.0.5/numer/__deps__.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,20 +4,26 @@
  !  MIT DIVIƷON
  `  __deps__ builtin numer-python 蟒算
 """
 # r
 import basic as bas
 import os
 from numbers         import Integral, Real
-from typing          import Iterable, Optional, Any, Union, Sequence#, Queue
+from typing          import TypedDict, Iterable, Optional, Any, Union, Sequence#, Queue
 # s
 NON  =  None
 TRU  =  True
 FAL  = False
 TYP  =  bas.TYP.copy()
+# FIXME Jax
+TYP[50] = nmb.Tensor
+TYP[60] = nmm.Module
+TYP     = TypedDict('TYP', TYP)
+Unm_sox = Union[TYP[50],TYP[60]]
+
 _fc  =   os.getenv( 'FC_IMP')
 if  bas.ist(_fc,NON) or _fc== '': _fc='tn'
 if 'j' in _fc:
     import jax       as nmb
     import jax.numpy as nmp
     import jax.nn    as nmm
 if 'h' in _fc:
@@ -44,17 +50,14 @@
     import torch     as nmb
     import torch.nn  as nmm
   if 'n' in _fc:
     import numpy     as nmp
 setnImp( os.getenv( 'FC_IMP'))
 '''
 
-# FIXME Jax
-TYP[50] = nmb.Tensor
-TYP[60] = nmm.Module
-Unm_sox = Union[TYP[50],TYP[60]]
+
 
 
 #mod = lambda x: phk.transform(x) if else
 # = lambda y: y
     
 if bas.Her(__name__): pass
```

### Comparing `muti.numer-0.0.4/numer/__init__.py` & `muti.numer-0.0.5/numer/__init__.py`

 * *Files identical despite different names*

### Comparing `muti.numer-0.0.4/numer/depLam.py` & `muti.numer-0.0.5/numer/depLam.py`

 * *Files identical despite different names*

### Comparing `muti.numer-0.0.4/numer/iniLam.py` & `muti.numer-0.0.5/numer/iniLam.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 def initMod(_nn_mod, _nn_ini_):
   _nn_ini_['bia'](_nn_mod.bias.data)
   _nn_ini_['wei'](_nn_mod.weight.data)
   return _nn_mod
 
 # [22W12] ARES
 def initMod_ran( ox:TYP[60]):
-  for m in mod.modules():
+  for m in  ox.modules():
     if ist(m, nmb.nn.Conv2d):
       nmb.nn.init.xavier_normal_(m.weight.data)
       #nn.init.kaiming_normal_(m.weight, mode='fan_in', nonlinearity='relu')
       if m.bias is not None:
         m.bias.data.zero_()
         #nn.init.constant_(m.bias, 0)
     elif ist(m, nmb.nn.BatchNorm2d):
```

### Comparing `muti.numer-0.0.4/numer/modLas.py` & `muti.numer-0.0.5/numer/modLas.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,13 +32,13 @@
     # 初始化参数
     def initCat(self):
         pass
 
     def addnMod(self, mod, nym): return self.add_module(nym, mod)
     def getrWrd(self,*i)       : return self.forward(*i)
     def set_dmm(self,mm)       : shftLai(self, mm) # gpu cpu ipu cuda 123 empty sbe called before constructing optimizer
-    def set_rmm(self,nm='c')   : nRnm(self.module(), nm) # test, train(mode), eval, run
+    def set_rmm(self,nm='tre') : Lam_mod(self.module(), nm) # test, train(mode), eval, run
     def getrPat(self, rec=True): return self.parameters(recurse=rec) # self.get_parameter()
     def detrMod(self)          :
         for child in self.children(): yield child
     def getrChi(self)          :
         for child in self.children(): yield child
```

### Comparing `muti.numer-0.0.4/numer/shfLam.py` & `muti.numer-0.0.5/numer/shfLam.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 LaiXPrm = dict(
   otg   = None,
   non   = None
 )
 def LaiRMod(mod, fc, mm='cuda',_fb=False):
     print(f"[{_JC_NYM} | mod] : load {mod._jc} by { fc}")
-    if fc in _LC3REV: nPrm_[ fc](mod)
+    if fc in _LC3REV: pass# nPrm_[ fc](mod)
     else:
       _lc = bas.getPath(fc)
       _mm = mm if len(mm) <= 4 else mm[:4] 
       loadMod(mod,_lc,_mm)
 
 def LaiPMod( ox:TYP[60], fc, fb=TRU):
     if fb :  ox= ox.state_dict() # 只存其参
@@ -95,15 +95,15 @@
 def fmrtDmm( fx):
     _fh_Dmm= fx if ist( fx,TYP[42]) else shftLanDdic(fx)
     if _fh_Dmm['t'] == 'm': return _fh_Dmm
     _fh_Dmm.setdefault(_KY_[0],nmb.float32) 
     _fh_Dmm.setdefault(_KY_[1],nmb.device('cuda' if nmb.cuda.is_available() else 'cpu')) 
     return _fh_Dmm
 
-def shftLai( ox, fh): return ox.to(**tDmm(fh))
+def shftLai( ox, fh): return ox.to(**fmrtDmm(fh))
 
 def shftLarTNum( ox:nmb.Tensor): return ox.detach().cpu().numpy()
 #def shftLar_num(ox): return ox.detach().cpu().numpy()
 def shftLar_Num( ox:Any, fh={'t':NON}):
     # FIXME
     if   ox is  NON: return NON
     _fc_typ= fh['t']
@@ -161,15 +161,15 @@
       if k in ignore_keys:
         new_item[k] =  ox[k]
       else:
         new_item[k] = toD( ox[k], device)
     return new_item
   elif ist( ox, Integral) or ist( ox, Real):
     return  ox
-  elif ist( ox, _np.ndarray) or ist( ox, _np.bool_):
+  elif ist( ox, nmp.ndarray) or ist( ox, nmp.bool_):
     return  ox
   elif  ox is None or ist( ox, str):
     return  ox
   else:
     raise TypeError("not support item type: {}".format(type( ox)))
 
 def to_tensor(
@@ -214,25 +214,25 @@
     elif hasattr(item, '_fields'):  # namedtuple
       return type(item)(*[to_tensor(t, dtype) for t in item])
     else:
       new_data = []
       for t in item:
         new_data.append(to_tensor(t, dtype, ignore_keys, transform_scalar))
       return new_data
-  elif ist(item, _np.ndarray):
+  elif ist(item, nmp.ndarray):
     if dtype is None:
-      if item.dtype == _np.float64:
+      if item.dtype == nmp.float64:
         return nmb.FloatTensor(item)
       else:
         return nmb.from_numpy(item)
     else:
       return nmb.from_numpy(item).to(dtype)
   elif ist(item, bool) or ist(item, str):
     return item
-  elif _np.isscalar(item):
+  elif nmp.isscalar(item):
     if transform_scalar:
       if dtype is None:
         return nmb.as_tensor(item)
       else:
         return nmb.as_tensor(item).to(dtype)
     else:
       return item
@@ -260,21 +260,21 @@
     :obj:`tuple` and :obj:`None`
   """
 
   if item is None:
     return item
   elif ist(item, nmb.Tensor):
     return item.tolist()
-  elif ist(item, _np.ndarray):
+  elif ist(item, nmp.ndarray):
     return item.tolist()
   elif ist(item, list) or ist(item, tuple):
     return [to_list(t) for t in item]
   elif ist(item, dict):
     return {k: to_list(v) for k, v in item.items()}
-  elif _np.isscalar(item):
+  elif nmp.isscalar(item):
     return item
   else:
     raise TypeError("not support item type: {}".format(type(item)))
 
 
 def tensor_to_list(item):
   r"""
@@ -293,15 +293,15 @@
     return item
   elif ist(item, nmb.Tensor):
     return item.tolist()
   elif ist(item, list) or ist(item, tuple):
     return [tensor_to_list(t) for t in item]
   elif ist(item, dict):
     return {k: tensor_to_list(v) for k, v in item.items()}
-  elif _np.isscalar(item):
+  elif nmp.isscalar(item):
     return item
   else:
     raise TypeError("not support item type: {}".format(type(item)))
 
 
 def same_shape(data: list):
   r"""
```

### Comparing `muti.numer-0.0.4/setup.py` & `muti.numer-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   url          = "https://github.com/E-C-Ares/",
   name         = "muti.numer",
-  version      = "0.0.4",
+  version      = "0.0.5",
   author       = "E.C.Ares",
   author_email = "E.C.Ares@outlook.com",
   license      = 'MIT DIVIƷON',
   description  = "utils for math-numer",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages     = setuptools.find_packages(),
```

