# Comparing `tmp/h2o_lightwave-1.1.1-py3-none-any.whl.zip` & `tmp/h2o_lightwave-1.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 124100 bytes, number of entries: 14
+Zip file size: 124104 bytes, number of entries: 14
 -rw-r--r--  2.0 unx     1140 b- defN 20-Feb-02 00:00 h2o_lightwave/__init__.py
 -rw-r--r--  2.0 unx    15363 b- defN 20-Feb-02 00:00 h2o_lightwave/core.py
 -rw-r--r--  2.0 unx    25866 b- defN 20-Feb-02 00:00 h2o_lightwave/graphics.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 h2o_lightwave/py.typed
 -rw-r--r--  2.0 unx    10592 b- defN 20-Feb-02 00:00 h2o_lightwave/routing.py
 -rw-r--r--  2.0 unx     3850 b- defN 20-Feb-02 00:00 h2o_lightwave/server.py
 -rw-r--r--  2.0 unx   653120 b- defN 20-Feb-02 00:00 h2o_lightwave/types.py
 -rw-r--r--  2.0 unx   170389 b- defN 20-Feb-02 00:00 h2o_lightwave/ui.py
 -rw-r--r--  2.0 unx     2325 b- defN 20-Feb-02 00:00 h2o_lightwave/ui_ext.py
 -rw-r--r--  2.0 unx       22 b- defN 20-Feb-02 00:00 h2o_lightwave/version.py
-?rw-r--r--  2.0 unx     6323 b- defN 20-Feb-02 00:00 h2o_lightwave-1.1.1.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 h2o_lightwave-1.1.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx       53 b- defN 20-Feb-02 00:00 h2o_lightwave-1.1.1.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     1125 b- defN 20-Feb-02 00:00 h2o_lightwave-1.1.1.dist-info/RECORD
-14 files, 890255 bytes uncompressed, 122248 bytes compressed:  86.3%
+?rw-r--r--  2.0 unx     6323 b- defN 20-Feb-02 00:00 h2o_lightwave-1.1.2.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 h2o_lightwave-1.1.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx       53 b- defN 20-Feb-02 00:00 h2o_lightwave-1.1.2.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1125 b- defN 20-Feb-02 00:00 h2o_lightwave-1.1.2.dist-info/RECORD
+14 files, 890255 bytes uncompressed, 122252 bytes compressed:  86.3%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: h2o_lightwave/ui_ext.py
 Comment: 
 
 Filename: h2o_lightwave/version.py
 Comment: 
 
-Filename: h2o_lightwave-1.1.1.dist-info/METADATA
+Filename: h2o_lightwave-1.1.2.dist-info/METADATA
 Comment: 
 
-Filename: h2o_lightwave-1.1.1.dist-info/WHEEL
+Filename: h2o_lightwave-1.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: h2o_lightwave-1.1.1.dist-info/licenses/LICENSE
+Filename: h2o_lightwave-1.1.2.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: h2o_lightwave-1.1.1.dist-info/RECORD
+Filename: h2o_lightwave-1.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## h2o_lightwave/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.1.1'
+__version__ = '1.1.2'
```

## Comparing `h2o_lightwave-1.1.1.dist-info/METADATA` & `h2o_lightwave-1.1.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: h2o_lightwave
-Version: 1.1.1
+Version: 1.1.2
 Summary: H2O Wave Python driver for integration with arbitrary python web frameworks.
 Project-URL: Homepage, https://wave.h2o.ai/
 Project-URL: Documentation, https://wave.h2o.ai/
 Project-URL: Repository, https://github.com/h2oai/wave
 Project-URL: Changelog, https://github.com/h2oai/wave/releases
 Author-email: Martin Turoci <martin.turoci@h2o.ai>
 License-Expression: Apache-2.0
@@ -22,15 +22,15 @@
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Widget Sets
 Requires-Python: >=3.8
 Provides-Extra: web
-Requires-Dist: h2o-lightwave-web==1.1.1; extra == 'web'
+Requires-Dist: h2o-lightwave-web==1.1.2; extra == 'web'
 Description-Content-Type: text/markdown
 
 # H2O Lightwave
 
 H2O Lightwave is a lightweight, pure-Python version of [H2O Wave](https://wave.h2o.ai/) that can be embedded in popular async web frameworks like FastAPI, Starlette, etc.
 
 In other words, H2O Lightwave works without the Wave server.
```

## Comparing `h2o_lightwave-1.1.1.dist-info/RECORD` & `h2o_lightwave-1.1.2.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -3,12 +3,12 @@
 h2o_lightwave/graphics.py,sha256=HLYrX-lwsMKbyLmy2ClG5L46DA2_hSCEPTsv0gPVoyg,25866
 h2o_lightwave/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 h2o_lightwave/routing.py,sha256=de8GVfUAb6bwFXtsWj6NXmjMVGELknlZb03F-R4ManY,10592
 h2o_lightwave/server.py,sha256=g0qj5W0NLesG9ghZlgwTOI74OgHY8XErw1BQWuljumI,3850
 h2o_lightwave/types.py,sha256=Wxe-osfyCgtN9ihYLpEfTlbX7sHzAN6UHxIBdIbaBSs,653120
 h2o_lightwave/ui.py,sha256=3L07AhP0z2yl61gO9eeJp3RIgJQFwC_fUIkibPnHXJc,170389
 h2o_lightwave/ui_ext.py,sha256=zx_2Ec2-p_ztm8brfVaVF0fTQWVDrb_YxcGfVb-wA10,2325
-h2o_lightwave/version.py,sha256=E-6wAZjiLRVInABFxrWoqdYlO_t-zVhK8XNfNnaDyzI,22
-h2o_lightwave-1.1.1.dist-info/METADATA,sha256=2YuPuxlVr43S7pFUk8iVA1To402gitCPGr5vdQXie20,6323
-h2o_lightwave-1.1.1.dist-info/WHEEL,sha256=TJPnKdtrSue7xZ_AVGkp9YXcvDrobsjBds1du3Nx6dc,87
-h2o_lightwave-1.1.1.dist-info/licenses/LICENSE,sha256=hpuFayniDwysSKD0tHGELH2KJDVyhUrKS29torRIpqY,53
-h2o_lightwave-1.1.1.dist-info/RECORD,,
+h2o_lightwave/version.py,sha256=YU_42OPd3M71CKuaAhmAM5b8bOg7D_phtEEaKy2kXNg,22
+h2o_lightwave-1.1.2.dist-info/METADATA,sha256=DpidgiVsniE78qGoBpOclAX5HmX1V9RIxxPtdCKbfe4,6323
+h2o_lightwave-1.1.2.dist-info/WHEEL,sha256=uNdcs2TADwSd5pVaP0Z_kcjcvvTUklh2S7bxZMF8Uj0,87
+h2o_lightwave-1.1.2.dist-info/licenses/LICENSE,sha256=hpuFayniDwysSKD0tHGELH2KJDVyhUrKS29torRIpqY,53
+h2o_lightwave-1.1.2.dist-info/RECORD,,
```

