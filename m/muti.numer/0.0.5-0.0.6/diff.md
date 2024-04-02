# Comparing `tmp/muti.numer-0.0.5.tar.gz` & `tmp/muti.numer-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muti.numer-0.0.5.tar", last modified: Tue Apr  2 08:50:55 2024, max compression
+gzip compressed data, was "muti.numer-0.0.6.tar", last modified: Tue Apr  2 10:21:58 2024, max compression
```

## Comparing `muti.numer-0.0.5.tar` & `muti.numer-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 08:50:55.553149 muti.numer-0.0.5/
--rw-rw-rw-   0        0        0     1089 2024-03-22 08:37:41.000000 muti.numer-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      767 2024-04-02 08:50:55.553149 muti.numer-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      346 2024-03-29 10:24:16.000000 muti.numer-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 08:50:55.552148 muti.numer-0.0.5/muti.numer.egg-info/
--rw-rw-rw-   0        0        0      767 2024-04-02 08:50:55.000000 muti.numer-0.0.5/muti.numer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2024-04-02 08:50:55.000000 muti.numer-0.0.5/muti.numer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 08:50:55.000000 muti.numer-0.0.5/muti.numer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-02 08:50:55.000000 muti.numer-0.0.5/muti.numer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-02 08:50:55.551148 muti.numer-0.0.5/numer/
--rw-rw-rw-   0        0        0     1348 2024-04-02 08:47:13.000000 muti.numer-0.0.5/numer/__deps__.py
--rw-rw-rw-   0        0        0      562 2024-04-02 06:49:33.000000 muti.numer-0.0.5/numer/__init__.py
--rw-rw-rw-   0        0        0     2326 2024-04-02 06:48:19.000000 muti.numer-0.0.5/numer/depLam.py
--rw-rw-rw-   0        0        0      903 2024-04-02 08:49:06.000000 muti.numer-0.0.5/numer/iniLam.py
--rw-rw-rw-   0        0        0     1765 2024-04-02 08:48:37.000000 muti.numer-0.0.5/numer/modLas.py
--rw-rw-rw-   0        0        0    11583 2024-04-02 08:40:13.000000 muti.numer-0.0.5/numer/shfLam.py
--rw-rw-rw-   0        0        0       42 2024-04-02 08:50:55.554148 muti.numer-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      653 2024-04-02 08:50:52.000000 muti.numer-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:21:58.076244 muti.numer-0.0.6/
+-rw-rw-rw-   0        0        0     1089 2024-03-22 08:37:41.000000 muti.numer-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      767 2024-04-02 10:21:58.074952 muti.numer-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2024-03-29 10:24:16.000000 muti.numer-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 10:21:58.074952 muti.numer-0.0.6/muti.numer.egg-info/
+-rw-rw-rw-   0        0        0      767 2024-04-02 10:21:57.000000 muti.numer-0.0.6/muti.numer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2024-04-02 10:21:58.000000 muti.numer-0.0.6/muti.numer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 10:21:57.000000 muti.numer-0.0.6/muti.numer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-02 10:21:57.000000 muti.numer-0.0.6/muti.numer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 10:21:58.073951 muti.numer-0.0.6/numer/
+-rw-rw-rw-   0        0        0     1371 2024-04-02 09:56:52.000000 muti.numer-0.0.6/numer/__deps__.py
+-rw-rw-rw-   0        0        0      562 2024-04-02 06:49:33.000000 muti.numer-0.0.6/numer/__init__.py
+-rw-rw-rw-   0        0        0      280 2024-04-02 09:11:21.000000 muti.numer-0.0.6/numer/betLam.py
+-rw-rw-rw-   0        0        0     2326 2024-04-02 06:48:19.000000 muti.numer-0.0.6/numer/depLam.py
+-rw-rw-rw-   0        0        0      146 2024-04-02 09:14:41.000000 muti.numer-0.0.6/numer/getLam.py
+-rw-rw-rw-   0        0        0      903 2024-04-02 08:49:06.000000 muti.numer-0.0.6/numer/iniLam.py
+-rw-rw-rw-   0        0        0     1765 2024-04-02 08:48:37.000000 muti.numer-0.0.6/numer/modLas.py
+-rw-rw-rw-   0        0        0     9356 2024-04-02 10:20:10.000000 muti.numer-0.0.6/numer/shfLam.py
+-rw-rw-rw-   0        0        0       42 2024-04-02 10:21:58.076244 muti.numer-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      653 2024-04-02 10:21:51.000000 muti.numer-0.0.6/setup.py
```

### Comparing `muti.numer-0.0.5/LICENSE` & `muti.numer-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `muti.numer-0.0.5/PKG-INFO` & `muti.numer-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muti.numer
-Version: 0.0.5
+Version: 0.0.6
 Summary: utils for math-numer
 Home-page: https://github.com/E-C-Ares/
 Author: E.C.Ares
 Author-email: E.C.Ares@outlook.com
 License: MIT DIVIƷON
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `muti.numer-0.0.5/muti.numer.egg-info/PKG-INFO` & `muti.numer-0.0.6/muti.numer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muti.numer
-Version: 0.0.5
+Version: 0.0.6
 Summary: utils for math-numer
 Home-page: https://github.com/E-C-Ares/
 Author: E.C.Ares
 Author-email: E.C.Ares@outlook.com
 License: MIT DIVIƷON
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `muti.numer-0.0.5/numer/__deps__.py` & `muti.numer-0.0.6/numer/__deps__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,18 +11,19 @@
 from typing          import TypedDict, Iterable, Optional, Any, Union, Sequence#, Queue
 # s
 NON  =  None
 TRU  =  True
 FAL  = False
 TYP  =  bas.TYP.copy()
 # FIXME Jax
-TYP[50] = nmb.Tensor
+TYP[50] = nmp.ndarray
+TYP[51] = nmb.Tensor
 TYP[60] = nmm.Module
 TYP     = TypedDict('TYP', TYP)
-Unm_sox = Union[TYP[50],TYP[60]]
+Unm_sox = Union[TYP[51],TYP[60]]
 
 _fc  =   os.getenv( 'FC_IMP')
 if  bas.ist(_fc,NON) or _fc== '': _fc='tn'
 if 'j' in _fc:
     import jax       as nmb
     import jax.numpy as nmp
     import jax.nn    as nmm
```

### Comparing `muti.numer-0.0.5/numer/__init__.py` & `muti.numer-0.0.6/numer/__init__.py`

 * *Files identical despite different names*

### Comparing `muti.numer-0.0.5/numer/depLam.py` & `muti.numer-0.0.6/numer/depLam.py`

 * *Files identical despite different names*

### Comparing `muti.numer-0.0.5/numer/iniLam.py` & `muti.numer-0.0.6/numer/iniLam.py`

 * *Files identical despite different names*

### Comparing `muti.numer-0.0.5/numer/modLas.py` & `muti.numer-0.0.6/numer/modLas.py`

 * *Files identical despite different names*

### Comparing `muti.numer-0.0.5/numer/shfLam.py` & `muti.numer-0.0.6/numer/shfLam.py`

 * *Files 16% similar despite different names*

```diff
@@ -44,29 +44,31 @@
 # TODO Place Params
 def tʃumMod( ox:TYP[60], lc):
     nmb.save(ox, lc)
     print(f"[{_JC_NYM} | [T]mod.mPrm] : savt {lc}")
 
 LaiXPrm = dict(
   otg   = None,
-  non   = None
+  non   = initMod_ran
 )
+
+#re-set parameters of mod by ptr else _fc
 def LaiRMod(mod, fc, mm='cuda',_fb=False):
     print(f"[{_JC_NYM} | mod] : load {mod._jc} by { fc}")
-    if fc in _LC3REV: pass# nPrm_[ fc](mod)
+    if fc in _LC3REV: LaiXPrm[ fc](mod)
     else:
-      _lc = bas.getPath(fc)
+      _lc = bas.Pth(fc)
       _mm = mm if len(mm) <= 4 else mm[:4] 
       loadMod(mod,_lc,_mm)
 
 def LaiPMod( ox:TYP[60], fc, fb=TRU):
     if fb :  ox= ox.state_dict() # 只存其参
     if fc[:3]in _LC3PEV:
-            _lc=bas.getPath(fc[:3]) + fc[3:] # FIXME
-    else  : _lc=bas.getPath( fc, TRU) # os.makedirs(os.path.dirname(_fc))
+            _lc=bas.Pth(fc[:3]) + fc[3:] # FIXME
+    else  : _lc=bas.Pth( fc, TRU) # os.makedirs(os.path.dirname(_fc))
     try   : tʃumMod( ox,_lc)
     except: print(f"[{_JC_NYM} | [E]mod.mPrm] : not-dir {_lc}")
 
 # 更改设备放置 memory <-> cpu, cuda <-> cpu, cuda
 def Lai_Mod( ox:TYP[60], fh    ):
     if      bas.iseKDic( fh,'m'):
       if fh['d'][:3] in _LC3DEV :
@@ -88,41 +90,69 @@
     #if ist(ox, str): FIXME elif
     if 'int' in  ox:  ret[_KY_[0]] = nmb.int32
     else           :  ret[_KY_[0]] = nmb.float32     # if 'float' in dmm
     if 'cpu' in  ox:  ret[_KY_[1]] = nmb.device('cpu')
     else           :  ret[_KY_[1]] = nmb.device('cuda' if nmb.cuda.is_available() else 'cpu')
     return ret
 
+# TODO layout
 def fmrtDmm( fx):
     _fh_Dmm= fx if ist( fx,TYP[42]) else shftLanDdic(fx)
     if _fh_Dmm['t'] == 'm': return _fh_Dmm
     _fh_Dmm.setdefault(_KY_[0],nmb.float32) 
     _fh_Dmm.setdefault(_KY_[1],nmb.device('cuda' if nmb.cuda.is_available() else 'cpu')) 
     return _fh_Dmm
 
 def shftLai( ox, fh): return ox.to(**fmrtDmm(fh))
 
 def shftLarTNum( ox:nmb.Tensor): return ox.detach().cpu().numpy()
+tsr =  lambda x,dt:nmb.as_tensor(x) if dt is None else nmb.tensor(x, dtype=dt)
+
 #def shftLar_num(ox): return ox.detach().cpu().numpy()
 def shftLar_Num( ox:Any, fh={'t':NON}):
     # FIXME
-    if   ox is  NON: return NON
+    if      ist( ox,NON    ):return NON
     _fc_typ= fh['t']
-    if      ist( ox,TYP[30]): return shftLarTNum(ox).astype(_fc_typ) if _fc_typ else shftLarTNum(ox)
-    if      ist( ox,TYP[20]): return ox.astype(_fc_typ)  if _fc_typ else ox
-    if      ist( ox,TYP[10]): return ox
+    if      ist( ox,TYP[30]):return shftLarTNum(ox).astype(_fc_typ) if _fc_typ else shftLarTNum(ox)
+    if      ist( ox,TYP[20]):return ox.astype(_fc_typ)  if _fc_typ else ox
+    if      ist( ox,TYP[10]):return ox
     # namedtuple
-    if  hasattr( ox,'_fields'):        return type(ox)(*[shftLar_Num(ex, fh) for ex in ox])
-    if      ist( ox,TYP[14],TYP[41]):  return None if  len( ox) == 0 else [shftLar_Num(ex, fh) for ex in ox]
-    if      ist( ox,TYP[42]):          return {k:shftLar_Num(ex, fh) for k, ex in ox.items()}
-    if nmp.isscalar(ox):               return nmp.array(ox)
+    if      ist( ox,'it'   ):return type(ox)(*[shftLar_Num(ex, fh) for ex in ox])
+    if      ist( ox,TYP[14],
+                    TYP[41]):return None if  len( ox) == 0 else [shftLar_Num(ex, fh) for ex in ox]
+    if      ist( ox,TYP[42]):return {k:shftLar_Num(ex, fh) for k, ex in ox.items()}
+    if      ist( ox,   'sc'):return nmp.array(ox)
     raise TypeError("not support item type: {}".format(type(ox)))
-
 def toN( *c,**g): return shftLar_Num( *c,**g)
 
+
+# ik ignore key
+def shftLar_Tsr( ox:Any, dt:Optional[nmb.dtype] = None, ik: list = ['SCL'], gk=[], fb=False):
+    # FIXME
+    if      ist( ox,NON    ):return NON
+    if      ist( ox,TYP[51]):return      ox.to(  dt) if dt is not None else ox
+    if      ist( ox,TYP[42]):return bas.typ( ox)((k,toT(v, dt, ik)) for k,v in ox.items()) if fb\
+                               else Tsr_Dix(     {k:toT(v, dt, ik)  for k,v in ox.items()}, gk)
+    if      ist( ox,'it'   ):return bas.typ( ox)( *[toT(t, dt)      for t   in ox])
+    if      ist( ox,TYP[41],
+                    TYP[14]):return bas.typ( ox)([]) if  len( ox) == 0\
+                               else     tsr( ox, dt) if ist(ox[0], Integral) or ist(ox[0], Real)\
+                               else bas.typ( ox)([toT(v, dt, ik) for v in ox])
+    if      ist( ox,TYP[50]):return nmb.from_numpy(ox).to(dt) if dt is not None\
+                               else nmb.FloatTensor(ox) if ox.dtype == nmp.float64\
+                               else nmb.from_numpy(ox)
+    if      ist( ox,TYP[10],
+                    TYP[40]):return  ox # FIXME
+    if      ist( ox,   'sc'):return  ox if fb\
+                               else nmb.as_tensor(ox).to(dt) if dt is not NON\
+                               else nmb.as_tensor(ox)
+    raise TypeError("not support item type: {}".format(type(ox)))
+def toT( *c,**g): return shftLar_Tsr( *c,**g)
+
+
 shftLar_ = dict(
     n    = shftLar_Num
 )
 def shftLar( ox, fc='n'): return shftLar_[fc](ox)
 def shftLas( ox, fc='n'): return ox.detach().cpu().numpy()
 
 def shftLan( ox, fc='n'): return ox.detach().cpu().numpy()
@@ -141,219 +171,95 @@
 '''
 nPrm_ = dict(
   otg = nPrm_ort,
   ran = nPrm_ran
 )
 '''
 
-def    toD( ox: Any, device: str, ignore_keys: list = []):
+def    toD( ox: Any, dev: str, igk: list = []):
   if   ist( ox, nmb.nn.Module):
-    return  ox.to(device)
+    return  ox.to(dev)
   elif ist( ox, nmb.Tensor):
-    return  ox.to(device)
+    return  ox.to(dev)
   elif ist( ox, Sequence):
     if ist( ox, str):
       return  ox
     else:
-      return [toD(t, device) for t in  ox]
+      return [toD(t, dev) for t in  ox]
   elif ist( ox, dict):
     new_item = {}
     for k in  ox.keys():
-      if k in ignore_keys:
+      if k in igk:
         new_item[k] =  ox[k]
       else:
-        new_item[k] = toD( ox[k], device)
+        new_item[k] = toD( ox[k], dev)
     return new_item
   elif ist( ox, Integral) or ist( ox, Real):
     return  ox
   elif ist( ox, nmp.ndarray) or ist( ox, nmp.bool_):
     return  ox
   elif  ox is None or ist( ox, str):
     return  ox
   else:
     raise TypeError("not support item type: {}".format(type( ox)))
 
-def to_tensor(
-    item: Any,
-    dtype: Optional[nmb.dtype] = None,
-    ignore_keys: list = [],
-    transform_scalar: bool = True
-):
-  r"""
-  Overview:
-    Change `numpy.ndarray`, sequence of scalars to nmb.Tensor, and keep other data types unchanged.
-  Arguments:
-    - item (:obj:`Any`): the item to be changed
-    - dtype (:obj:`type`): the type of wanted tensor
-  Returns:
-    - item (:obj:`nmb.Tensor`): the change tensor
 
-  .. note:
+# 包含数值的张量 [23A90] afc:.pop() -> .popleft()
+def Tsr_Dix(tfc, afc=['stp']):
+  ugd = tfc[afc[0]].unsqueeze(-1)
+  #afc.popleft()
+  if len(afc) > 1:
+    for fc in afc[1:]:
+      ugd = nmb.cat((ugd,tfc[fc].unsqueeze(-1)), -1)
+  return ugd
 
-    Now supports item type: :obj:`dict`, :obj:`list`, :obj:`tuple` and :obj:`None`
-  """
+def Tsr_Lix(tfc, afc=['stp']):
+  ugd = tfc[afc[0]].unsqueeze(-1)
+  #afc.popleft()
+  if len(afc) > 1:
+    for fc in afc[1:]:
+      ugd = nmb.cat((ugd,tfc[fc].unsqueeze(-1)), -1)
+  return ugd
 
-  def transform(d):
-    if dtype is None:
-      return nmb.as_tensor(d)
-    else:
-      return nmb.tensor(d, dtype=dtype)
 
-  if ist(item, dict):
-    new_data = {}
-    for k, v in item.items():
-      if k in ignore_keys:
-        new_data[k] = v
-      else:
-        new_data[k] = to_tensor(v, dtype, ignore_keys, transform_scalar)
-    return new_data
-  elif ist(item, list) or ist(item, tuple):
-    if len(item) == 0:
-      return []
-    elif ist(item[0], Integral) or ist(item[0], Real):
-      return transform(item)
-    elif hasattr(item, '_fields'):  # namedtuple
-      return type(item)(*[to_tensor(t, dtype) for t in item])
-    else:
-      new_data = []
-      for t in item:
-        new_data.append(to_tensor(t, dtype, ignore_keys, transform_scalar))
-      return new_data
-  elif ist(item, nmp.ndarray):
-    if dtype is None:
-      if item.dtype == nmp.float64:
-        return nmb.FloatTensor(item)
-      else:
-        return nmb.from_numpy(item)
-    else:
-      return nmb.from_numpy(item).to(dtype)
-  elif ist(item, bool) or ist(item, str):
-    return item
-  elif nmp.isscalar(item):
-    if transform_scalar:
-      if dtype is None:
-        return nmb.as_tensor(item)
-      else:
-        return nmb.as_tensor(item).to(dtype)
-    else:
-      return item
-  elif item is None:
-    return None
-  elif ist(item, nmb.Tensor):
-    if dtype is None:
-      return item
-    else:
-      return item.to(dtype)
-  else:
-    raise TypeError("not support item type: {}".format(type(item)))
 
-def to_list(item):
 
-  r"""
-  Overview:
-    Transform `nmb.Tensor`, `numpy.ndarray` to `list`, keep other data types unchanged
-  Arguments:
-    - item (:obj:`Any`): the item to be transformed
-  Returns:
-    - item (:obj:`list`): the list after transformation
-  .. note::
-    Now supports item type: :obj:`nmb.Tensor`, :obj:`numpy.ndarray`, :obj:`dict`, :obj:`list`, \
-    :obj:`tuple` and :obj:`None`
-  """
+
+def toL(item):
 
   if item is None:
     return item
   elif ist(item, nmb.Tensor):
     return item.tolist()
   elif ist(item, nmp.ndarray):
     return item.tolist()
   elif ist(item, list) or ist(item, tuple):
-    return [to_list(t) for t in item]
+    return [toL(t) for t in item]
   elif ist(item, dict):
-    return {k: to_list(v) for k, v in item.items()}
+    return {k: toL(v) for k, v in item.items()}
   elif nmp.isscalar(item):
     return item
   else:
     raise TypeError("not support item type: {}".format(type(item)))
 
-
 def tensor_to_list(item):
-  r"""
-  Overview:
-    Transform `nmb.Tensor` to `list`, keep other data types unchanged
-  Arguments:
-    - item (:obj:`Any`): the item to be transformed
-  Returns:
-    - item (:obj:`list`): the list after transformation
-
-  .. note::
-
-    Now supports item type: :obj:`nmb.Tensor`, :obj:`dict`, :obj:`list`, :obj:`tuple` and :obj:`None`
-  """
   if item is None:
     return item
   elif ist(item, nmb.Tensor):
     return item.tolist()
   elif ist(item, list) or ist(item, tuple):
     return [tensor_to_list(t) for t in item]
   elif ist(item, dict):
     return {k: tensor_to_list(v) for k, v in item.items()}
   elif nmp.isscalar(item):
     return item
   else:
     raise TypeError("not support item type: {}".format(type(item)))
 
 
-def same_shape(data: list):
-  r"""
-  Overview:
-    Judge whether all data elements in a list have the same shape.
-  Arguments:
-    - data (:obj:`list`): the list of data
-  Returns:
-    - same (:obj:`bool`): whether the list of data all have the same shape
-  """
-  assert (ist(data, list))
-  shapes = [t.shape for t in data]
-  return len(set(shapes)) == 1
-
-
-class LogDict(dict):
-  '''
-  Overview:
-    Derived from ``dict``; Would transform ``nmb.Tensor`` to ``list`` for convenient logging.
-  '''
-
-  def _transform(self, data):
-    if ist(data, nmb.Tensor):
-      new_data = data.tolist()
-    else:
-      new_data = data
-    return new_data
-
-  def __setitem__(self, key, value):
-    new_value = self._transform(value)
-    super().__setitem__(key, new_value)
-
-  def update(self, data):
-    for k, v in data.items():
-      self.__setitem__(k, v)
-
-
-def build_log_buffer():
-  r"""
-  Overview:
-    Builg log buffer, a subclass of dict, which can transform the input data into log format.
-  Returns:
-    - log_buffer (:obj:`LogDict`): Log buffer dict
-  """
-  return LogDict()
-
-
-
 
 def get_tensor_data(data: Any) -> Any:
   """
   Overview:
     Get pure tensor data from the given data(without disturbing grad computation graph)
   """
   if ist(data, nmb.Tensor):
@@ -374,20 +280,12 @@
   elif ist(data, Sequence):
     return [unsqueeze(d) for d in data]
   elif ist(data, dict):
     return {k: unsqueeze(v, 0) for k, v in data.items()}
   else:
     raise TypeError("not support type in unsqueeze: {}".format(type(data)))
 
-# [23A90] afc:.pop() -> .popleft()
-def rTsr(tfc, afc=['stp']):
-  ugd = tfc[afc[0]].unsqueeze(-1)
-  #afc.popleft()
-  if len(afc) > 1:
-    for fc in afc[1:]:
-      ugd = nmb.cat((ugd,tfc[fc].unsqueeze(-1)), -1)
-  return ugd
 
 if  bas.Her(__name__):
     a = nmb.tensor([1.0, 1.0])
     b = shftLarTNum(a)
     print(b)
```

### Comparing `muti.numer-0.0.5/setup.py` & `muti.numer-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   url          = "https://github.com/E-C-Ares/",
   name         = "muti.numer",
-  version      = "0.0.5",
+  version      = "0.0.6",
   author       = "E.C.Ares",
   author_email = "E.C.Ares@outlook.com",
   license      = 'MIT DIVIƷON',
   description  = "utils for math-numer",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages     = setuptools.find_packages(),
```

