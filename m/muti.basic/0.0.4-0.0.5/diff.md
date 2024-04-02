# Comparing `tmp/muti.basic-0.0.4.tar.gz` & `tmp/muti.basic-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muti.basic-0.0.4.tar", last modified: Thu Mar 28 01:55:19 2024, max compression
+gzip compressed data, was "muti.basic-0.0.5.tar", last modified: Tue Apr  2 01:51:45 2024, max compression
```

## Comparing `muti.basic-0.0.4.tar` & `muti.basic-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-03-28 01:55:19.990408 muti.basic-0.0.4/
--rw-rw-rw-   0        0        0     1088 2024-03-26 07:23:35.000000 muti.basic-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      437 2024-03-28 01:55:19.989207 muti.basic-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-03-25 03:22:38.000000 muti.basic-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-03-28 01:55:19.963656 muti.basic-0.0.4/basic/
--rw-rw-rw-   0        0        0      677 2024-03-28 01:50:42.000000 muti.basic-0.0.4/basic/__deps__.py
--rw-rw-rw-   0        0        0       70 2024-03-25 09:24:42.000000 muti.basic-0.0.4/basic/__init__.py
--rw-rw-rw-   0        0        0     3132 2024-03-27 05:34:32.000000 muti.basic-0.0.4/basic/depLam.py
--rw-rw-rw-   0        0        0     3010 2024-03-27 09:34:48.000000 muti.basic-0.0.4/basic/getLam.py
--rw-rw-rw-   0        0        0     2165 2024-03-26 06:34:43.000000 muti.basic-0.0.4/basic/parLam.py
--rw-rw-rw-   0        0        0     1077 2024-03-28 01:51:12.000000 muti.basic-0.0.4/basic/typLas.py
-drwxrwxrwx   0        0        0        0 2024-03-28 01:55:19.987290 muti.basic-0.0.4/muti.basic.egg-info/
--rw-rw-rw-   0        0        0      437 2024-03-28 01:55:19.000000 muti.basic-0.0.4/muti.basic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2024-03-28 01:55:19.000000 muti.basic-0.0.4/muti.basic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-28 01:55:19.000000 muti.basic-0.0.4/muti.basic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-03-28 01:55:19.000000 muti.basic-0.0.4/muti.basic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-28 01:55:19.990408 muti.basic-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      580 2024-03-28 01:55:08.000000 muti.basic-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 01:51:45.738629 muti.basic-0.0.5/
+-rw-rw-rw-   0        0        0     1088 2024-03-26 07:23:35.000000 muti.basic-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      437 2024-04-02 01:51:45.737630 muti.basic-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-03-25 03:22:38.000000 muti.basic-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 01:51:45.718091 muti.basic-0.0.5/basic/
+-rw-rw-rw-   0        0        0      695 2024-03-29 10:47:00.000000 muti.basic-0.0.5/basic/__deps__.py
+-rw-rw-rw-   0        0        0       70 2024-04-02 01:45:36.000000 muti.basic-0.0.5/basic/__init__.py
+-rw-rw-rw-   0        0        0   246354 2024-04-02 01:46:11.000000 muti.basic-0.0.5/basic/carLam.py
+-rw-rw-rw-   0        0        0     3575 2024-04-01 15:39:36.000000 muti.basic-0.0.5/basic/depLam.py
+-rw-rw-rw-   0        0        0     3025 2024-04-02 01:45:58.000000 muti.basic-0.0.5/basic/getLam.py
+-rw-rw-rw-   0        0        0     3399 2024-04-02 01:46:03.000000 muti.basic-0.0.5/basic/parLam.py
+-rw-rw-rw-   0        0        0     2184 2024-04-02 01:48:18.000000 muti.basic-0.0.5/basic/typLas.py
+drwxrwxrwx   0        0        0        0 2024-04-02 01:51:45.736640 muti.basic-0.0.5/muti.basic.egg-info/
+-rw-rw-rw-   0        0        0      437 2024-04-02 01:51:45.000000 muti.basic-0.0.5/muti.basic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-04-02 01:51:45.000000 muti.basic-0.0.5/muti.basic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 01:51:45.000000 muti.basic-0.0.5/muti.basic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-02 01:51:45.000000 muti.basic-0.0.5/muti.basic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 01:51:45.738629 muti.basic-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      616 2024-04-02 01:51:36.000000 muti.basic-0.0.5/setup.py
```

### Comparing `muti.basic-0.0.4/LICENSE` & `muti.basic-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `muti.basic-0.0.4/basic/depLam.py` & `muti.basic-0.0.5/basic/depLam.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,19 @@
+"""
+ #  bas-muti :: dep-lam 公函集
+ @  E.C.Ares
+ !  MIT DIVIƷON
+ `  Lam of deps builtin basic-python
+"""
+# r
 from __deps__ import *
-
+NON = None
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
@@ -66,18 +76,26 @@
 
 def rtc( *c,  f=NON):
     if f is NON     : f  =   c[0] is not NON
     return    c[0] if f else c[1](c[0])
 
 #   ist = lambda x, *args: isinstance(x, tuple(*args))
 def ist( ox,*fh):
+  fh = list( fh)
   if NON in  fh :
-    if   ox  is NON: return True 
+    if   ox  is NON :return True 
     fh.remove(NON)
-  if    len( fh)==0: return False
-  if    len( fh)==1: return isinstance(ox, fh[0])
+  if    len( fh)==0 :return False
+  if    len( fh)==1 :
+     if fh[0]=='lam':return   callable(ox)
+     else           :return isinstance(ox, fh[0])
   return                    isinstance(ox, tuple(fh))
 
 
+#def lcpnDic( od, ox): od = pickle.loads(pickle.dumps(original_dict))
+def lcp( ox): return pickle.loads(pickle.dumps( ox))
+
+def setnDic( od, ox):
+    for _eh  in  ox.items():  setattr(od, *_eh)
 # betrHer default False
 def Her( fc=  __name__):
   return fc=="__main__"
```

### Comparing `muti.basic-0.0.4/basic/getLam.py` & `muti.basic-0.0.5/basic/getLam.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
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
-from .depLam         import *
-from .parLam         import Imp
+from depLam         import *
+from parLam         import Imp, Pth
 from threading       import Thread
 #       r.. as
 import      numpy        as _np
 import      torch        as _tc
 import  itertools        as _it
 # s
 _JC_NYM = 'lam_get'
@@ -78,22 +78,23 @@
 
 
 
 
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

### Comparing `muti.basic-0.0.4/setup.py` & `muti.basic-0.0.5/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
-  name    = "muti.basic",
-  version = "0.0.4",
-  author  = "E.C.Ares",
-  author_email="E.C.Ares@outlook.com",
-  description ="utils for pytorch",
-  long_description=long_description,
-  long_description_content_type="text/markdown",
-  url="https://github.com/E-C-Ares/",
-  packages=setuptools.find_packages(),
-  classifiers=[
+  name         = "muti.basic",
+  version      = "0.0.5",
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

