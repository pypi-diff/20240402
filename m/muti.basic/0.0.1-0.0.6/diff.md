# Comparing `tmp/muti.basic-0.0.1.tar.gz` & `tmp/muti.basic-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muti.basic-0.0.1.tar", last modified: Tue Mar 26 03:00:09 2024, max compression
+gzip compressed data, was "muti.basic-0.0.6.tar", last modified: Tue Apr  2 02:24:33 2024, max compression
```

## Comparing `muti.basic-0.0.1.tar` & `muti.basic-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-03-26 03:00:09.961561 muti.basic-0.0.1/
--rw-rw-rw-   0        0        0     1089 2024-03-25 07:12:08.000000 muti.basic-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      437 2024-03-26 03:00:09.960562 muti.basic-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-03-25 03:22:38.000000 muti.basic-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-26 03:00:09.939005 muti.basic-0.0.1/basic/
--rw-rw-rw-   0        0        0     2541 2024-03-25 10:16:44.000000 muti.basic-0.0.1/basic/__deps__.py
--rw-rw-rw-   0        0        0       70 2024-03-25 09:24:42.000000 muti.basic-0.0.1/basic/__init__.py
--rw-rw-rw-   0        0        0     3731 2024-03-26 02:55:45.000000 muti.basic-0.0.1/basic/getLam.py
--rw-rw-rw-   0        0        0     2161 2024-03-26 02:55:16.000000 muti.basic-0.0.1/basic/parLam.py
-drwxrwxrwx   0        0        0        0 2024-03-26 03:00:09.960562 muti.basic-0.0.1/muti.basic.egg-info/
--rw-rw-rw-   0        0        0      437 2024-03-26 03:00:09.000000 muti.basic-0.0.1/muti.basic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2024-03-26 03:00:09.000000 muti.basic-0.0.1/muti.basic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-26 03:00:09.000000 muti.basic-0.0.1/muti.basic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-03-26 03:00:09.000000 muti.basic-0.0.1/muti.basic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-26 03:00:09.961561 muti.basic-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      580 2024-03-26 02:58:19.000000 muti.basic-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 02:24:33.831671 muti.basic-0.0.6/
+-rw-rw-rw-   0        0        0     1088 2024-03-26 07:23:35.000000 muti.basic-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      437 2024-04-02 02:24:33.830671 muti.basic-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-03-25 03:22:38.000000 muti.basic-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 02:24:33.819141 muti.basic-0.0.6/basic/
+-rw-rw-rw-   0        0        0      695 2024-03-29 10:47:00.000000 muti.basic-0.0.6/basic/__deps__.py
+-rw-rw-rw-   0        0        0      139 2024-04-02 01:56:47.000000 muti.basic-0.0.6/basic/__init__.py
+-rw-rw-rw-   0        0        0   246355 2024-04-02 01:56:39.000000 muti.basic-0.0.6/basic/carLam.py
+-rw-rw-rw-   0        0        0     3576 2024-04-02 01:56:33.000000 muti.basic-0.0.6/basic/depLam.py
+-rw-rw-rw-   0        0        0     3027 2024-04-02 01:57:00.000000 muti.basic-0.0.6/basic/getLam.py
+-rw-rw-rw-   0        0        0     3400 2024-04-02 01:57:04.000000 muti.basic-0.0.6/basic/parLam.py
+-rw-rw-rw-   0        0        0     2185 2024-04-02 01:58:44.000000 muti.basic-0.0.6/basic/typLas.py
+drwxrwxrwx   0        0        0        0 2024-04-02 02:24:33.830671 muti.basic-0.0.6/muti.basic.egg-info/
+-rw-rw-rw-   0        0        0      437 2024-04-02 02:24:33.000000 muti.basic-0.0.6/muti.basic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-04-02 02:24:33.000000 muti.basic-0.0.6/muti.basic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 02:24:33.000000 muti.basic-0.0.6/muti.basic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-02 02:24:33.000000 muti.basic-0.0.6/muti.basic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 02:24:33.831671 muti.basic-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      616 2024-04-02 02:24:29.000000 muti.basic-0.0.6/setup.py
```

### Comparing `muti.basic-0.0.1/LICENSE` & `muti.basic-0.0.6/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 MIT License
 
 Copyright (c) 王氾超 E.Codeine.Ares 2014
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `muti.basic-0.0.1/basic/__deps__.py` & `muti.basic-0.0.6/basic/depLam.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,19 @@
-import os,sys
-
+"""
+ #  bas-muti :: dep-lam 公函集
+ @  E.C.Ares
+ !  MIT DIVIƷON
+ `  Lam of deps builtin basic-python
+"""
+# r
+from .__deps__ import *
 NON = None
-TLA_=[globals(),locals()]
-
+TRU = True
+FAL = False
+# 
 #exptNon = lambda _or, *cfg, **tfg: try: return _or(*cfg, **tfg); except: return None
 def dddfOut_cfc(_or_, fc,*cfg,**tfg): return       _or_[fc](     *cfg,**tfg)
 def dddfOut_afc(_or_,afc,*cfg,**tfg): return {fc : _or_[fc](     *cfg,**tfg) for fc     in afc                 } 
 def dddfOut_tfc(_or_,tfc,*cfg,**tfg): return {fc : _or_[fc]( jc ,*cfg,**tfg) for fc, jc in tfc.items(         )}
 def dddfOut_nfc(_or_,nfc,*cfg,**tfg): return {fc : _or_[fc]( jc ,*cfg,**tfg) for fc, jc in nfc.__dict__.items()}
 def dddfOut_mfc(_or_,nfc,*cfg,**tfg): raise  NotImplementedError
 dddfOut_ = {
@@ -54,8 +61,41 @@
     tfg_ret = {}    # events-like, return not nessary
     for   fc    in  _fc:
       try   :tfg_ret[fc]=_or_[ fc](     *cfg,  tfg[ fc])
       except:pass
     return tfg_ret  # get 方法..
   else:
     try     :return      _or_[_fc](     *cfg,  tfg[_fc])
-    except  :return      None
+    except  :return      None
+
+
+def rec(  a=[ ], *c): pass
+ 
+def r1c( *c,  f=NON):
+    if f is NON     : f  =   c[0] is not NON
+    return    c[0] if f else c[1]
+
+def rtc( *c,  f=NON):
+    if f is NON     : f  =   c[0] is not NON
+    return    c[0] if f else c[1](c[0])
+
+#   ist = lambda x, *args: isinstance(x, tuple(*args))
+def ist( ox,*fh):
+  fh = list( fh)
+  if NON in  fh :
+    if   ox  is NON :return True 
+    fh.remove(NON)
+  if    len( fh)==0 :return False
+  if    len( fh)==1 :
+     if fh[0]=='lam':return   callable(ox)
+     else           :return isinstance(ox, fh[0])
+  return                    isinstance(ox, tuple(fh))
+
+
+#def lcpnDic( od, ox): od = pickle.loads(pickle.dumps(original_dict))
+def lcp( ox): return pickle.loads(pickle.dumps( ox))
+
+def setnDic( od, ox):
+    for _eh  in  ox.items():  setattr(od, *_eh)
+# betrHer default False
+def Her( fc=  __name__):
+  return fc=="__main__"
```

### Comparing `muti.basic-0.0.1/basic/getLam.py` & `muti.basic-0.0.6/basic/getLam.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,27 @@
 """
- #  取得函集 get-lams
+ #  bas-muti :: get-lam 取函集
  @  E.C.Ares
- !  MIT LICENSE
- `  built in pkp for basic-python mio
+ !  MIT DIVIƷON
+ `  Lam of gets builtin basic-python
 """
 # r(import-refs)
 #       r.. im
-from __deps__       import *
-from parLam         import Imp
+from .depLam         import *
+from .parLam         import Imp, Pth
 from threading       import Thread
-from numbers         import Integral, Real
-from typing          import Iterable, Optional, Any, Union
-from collections.abc import Sequence#, Queue
 #       r.. as
 import      numpy        as _np
 import      torch        as _tc
 import  itertools        as _it
 # s
 _JC_NYM = 'lam_get'
 
 
-#   ist = lambda x, *args: isinstance(x, tuple(*args))
-def ist( ox,*fh):
-  if NON in  fh :
-    if   ox  is NON: return True 
-    fh.remove(NON)
-  if    len( fh)==0: return False
-  if    len( fh)==1: return isinstance(ox, fh[0])
-  return                    isinstance(ox, tuple(fh))
-
-
-TYP = {
-  10: bool,
-  11: int,
-  12: float,
-  13: str,
-  14: tuple,
-  21: Integral,
-  22: Real,
-  41: list,
-  42: dict,
-  20: _np.ndarray,
-  30: _tc.Tensor,
-  50: object}
+
 
 _KY_ = ['dtype','device']
 
 def isn_Lis( ox, ex): return ex in ox
 def ism_Lis( ox,aex): return [ex in ox for ex in aex]
 def ish_Lis( ox,aex): return all(ish_Lis( ox,aex))
 def isx_Lis( ox,aex): return any(ish_Lis( ox,aex))
@@ -98,30 +73,28 @@
     fc        = _fc
     return   ox.get( fc, ar)
 
 # FIXME PARALL
 for _fc in _FC_AT_: TLA_[0][ 'Var'+_fc+'LaK'] =lambda ox, ex:TLA_[0]['Var'+_fc+'DiK'](ox.__dict__, ex)
 
 
-# betrHer
-def Her( fc):
-    if   fc == 'n'  : return  __name__ == "__main__"
-    return  False
+
 
 _LC_HER = os.getcwd()
 # input configs
 def Inp( jc, lc=_LC_HER, fb_deb=True):
-    _lc  =   os.path.join(   lc, jc)
+    _lc  =  Pth( jc, lc)
     _jh  =   os.path.splitext(   jc)
     _jc  =  _jh[ 0]
     _fc  =  _jh[-1][ 1]
     if fb_deb:print(_lc)
     return  Imp(_lc,_fc)
 
 def Him(imp):
     print('pause')
     pass
 
 #if __name__ == "__main__":
-if  Her('n'):
+if  Her(__name__):
+    
     #him()
-    Him(Inp('tests.yml'))
+    Him(Inp('tests.yml','..'))
```

### Comparing `muti.basic-0.0.1/basic/parLam.py` & `muti.basic-0.0.6/basic/parLam.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
- #  取得函集 get-lams
+ #  bas-muti :: par-lam 析函集
  @  E.C.Ares
- !  MIT LICENSE
- `  built in pkp for basic-python mio
+ !  MIT DIVIƷON
+ `  Lam of part builtin basic-python
 """
 # r(import-refs)
 #       r.. im
-from __deps__       import *
+from   .depLam       import *
 import argparse as arg
 import json
 import yaml  # ruamel.yaml pyyaml
 import importlib.util as pyth
 # s
 _JC_NYM = 'lam_par'
 
@@ -60,8 +60,33 @@
 Imp_ = dict(
    p = Imp_Cfg,
    j = Imp_Cfp,
    y = Imp_Cfp)
 
 def Imp( lc, fc, *c,**g):
     #if lc[1] not in [':','h']:
-    return Imp_[fc](lc, fc, *c,**g)
+    return Imp_[fc](lc, fc, *c,**g)
+
+_LC_HER = os.getcwd()
+
+_JC_TOK_={
+    'r' :['rut','root','/','\\'],
+    'a' :['aut','ares','~','D:'],
+    'b' :['but','base','_','..'],
+    'c' :['cut','cwdb','.','__']}
+
+_LC_RUT = os.path.abspath(os.sep)
+_LC_HOM = os.path.expanduser("~")
+# 得到合法的 lc/jc 路径, 若 fb 且 lc不存在 则创建
+def Pth( jc, lc=NON, fb=TRU) :
+    _lc                              =  os.path.dirname(             jc) # '' 或 jc前缀
+    _jc                              =  os.path.basename(            jc)
+    if  ist( lc,NON):           _lc  =  os.path.abspath(            _lc)\
+                                    if  os.path.isdir(              _lc)\
+                                   else os.path.join(os.getcwd(),   _lc)
+    elif lc  in _JC_TOK_['r']:  _lc  =  os.path.join(_LC_RUT    ,   _lc)
+    elif lc  in _JC_TOK_['a']:  _lc  =  os.path.join(_LC_HOM    ,   _lc)
+    elif lc  in _JC_TOK_['b']:  _lc  =  os.path.join(os.getcwd(),   _lc) 
+    elif lc  in _JC_TOK_['c']:  _lc  =  os.path.join(os.getcwd(),   _lc) #os.getcwdb()
+    else:                       _lc  =  os.path.join(os.path.abspath(lc),_lc)
+    if fb and not os.path.isdir(_lc) :  os.makedirs( _lc)
+    return        os.path.join( _lc,_jc)
```

### Comparing `muti.basic-0.0.1/setup.py` & `muti.basic-0.0.6/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
-  name    = "muti.basic",
-  version = "0.0.1",
-  author  = "E.C.Ares",
-  author_email="E.C.Ares@outlook.com",
-  description ="utils for pytorch",
-  long_description=long_description,
-  long_description_content_type="text/markdown",
-  url="https://github.com/E-C-Ares/",
-  packages=setuptools.find_packages(),
-  classifiers=[
+  name         = "muti.basic",
+  version      = "0.0.6",
+  author       = "E.C.Ares",
+  author_email = "E.C.Ares@outlook.com",
+  url          = "https://github.com/E-C-Ares/",
+  description  = "utils for pytorch",
+  packages     = setuptools.find_packages(),
+  classifiers  = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   ],
-)
+  long_description=long_description,
+  long_description_content_type="text/markdown")
```

