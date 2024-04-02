# Comparing `tmp/h2o_lightwave_web-1.1.1-py3-none-any.whl.zip` & `tmp/h2o_lightwave_web-1.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5749473 bytes, number of entries: 830
+Zip file size: 5749474 bytes, number of entries: 830
 -rw-r--r--  2.0 unx     1366 b- defN 20-Feb-02 00:00 h2o_lightwave_web/__init__.py
 -rw-r--r--  2.0 unx       22 b- defN 20-Feb-02 00:00 h2o_lightwave_web/version.py
 -rw-r--r--  2.0 unx    15406 b- defN 20-Feb-02 00:00 h2o_lightwave_web/www/favicon.ico
 -rw-r--r--  2.0 unx     2380 b- defN 20-Feb-02 00:00 h2o_lightwave_web/www/index.html
 -rw-r--r--  2.0 unx     2903 b- defN 20-Feb-02 00:00 h2o_lightwave_web/www/logo192.png
 -rw-r--r--  2.0 unx    10723 b- defN 20-Feb-02 00:00 h2o_lightwave_web/www/logo512.png
 -rw-r--r--  2.0 unx      476 b- defN 20-Feb-02 00:00 h2o_lightwave_web/www/manifest.json
@@ -821,12 +821,12 @@
 -rw-r--r--  2.0 unx     1764 b- defN 20-Feb-02 00:00 h2o_lightwave_web/www/wave-static/yaml-legacy-5fac3622.js
 -rw-r--r--  2.0 unx      270 b- defN 20-Feb-02 00:00 h2o_lightwave_web/www/wave-static/yaml.js-3a05ad15.js
 -rw-r--r--  2.0 unx      376 b- defN 20-Feb-02 00:00 h2o_lightwave_web/www/wave-static/yaml.js-legacy-fd5075f2.js
 -rw-r--r--  2.0 unx     1557 b- defN 20-Feb-02 00:00 h2o_lightwave_web/www/wave-static/zephir-cf2a8bcb.js
 -rw-r--r--  2.0 unx     1626 b- defN 20-Feb-02 00:00 h2o_lightwave_web/www/wave-static/zephir-legacy-56a6ea33.js
 -rw-r--r--  2.0 unx      276 b- defN 20-Feb-02 00:00 h2o_lightwave_web/www/wave-static/zephir.js-fa8df6f1.js
 -rw-r--r--  2.0 unx      382 b- defN 20-Feb-02 00:00 h2o_lightwave_web/www/wave-static/zephir.js-legacy-cf8f00c6.js
-?rw-r--r--  2.0 unx     1347 b- defN 20-Feb-02 00:00 h2o_lightwave_web-1.1.1.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 h2o_lightwave_web-1.1.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx       53 b- defN 20-Feb-02 00:00 h2o_lightwave_web-1.1.1.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx    93868 b- defN 20-Feb-02 00:00 h2o_lightwave_web-1.1.1.dist-info/RECORD
-830 files, 13389248 bytes uncompressed, 5592357 bytes compressed:  58.2%
+?rw-r--r--  2.0 unx     1347 b- defN 20-Feb-02 00:00 h2o_lightwave_web-1.1.2.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 h2o_lightwave_web-1.1.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx       53 b- defN 20-Feb-02 00:00 h2o_lightwave_web-1.1.2.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx    93868 b- defN 20-Feb-02 00:00 h2o_lightwave_web-1.1.2.dist-info/RECORD
+830 files, 13389248 bytes uncompressed, 5592358 bytes compressed:  58.2%
```

## zipnote {}

```diff
@@ -2472,20 +2472,20 @@
 
 Filename: h2o_lightwave_web/www/wave-static/zephir.js-fa8df6f1.js
 Comment: 
 
 Filename: h2o_lightwave_web/www/wave-static/zephir.js-legacy-cf8f00c6.js
 Comment: 
 
-Filename: h2o_lightwave_web-1.1.1.dist-info/METADATA
+Filename: h2o_lightwave_web-1.1.2.dist-info/METADATA
 Comment: 
 
-Filename: h2o_lightwave_web-1.1.1.dist-info/WHEEL
+Filename: h2o_lightwave_web-1.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: h2o_lightwave_web-1.1.1.dist-info/licenses/LICENSE
+Filename: h2o_lightwave_web-1.1.2.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: h2o_lightwave_web-1.1.1.dist-info/RECORD
+Filename: h2o_lightwave_web-1.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## h2o_lightwave_web/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.1.1'
+__version__ = '1.1.2'
```

## Comparing `h2o_lightwave_web-1.1.1.dist-info/METADATA` & `h2o_lightwave_web-1.1.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: h2o_lightwave_web
-Version: 1.1.1
+Version: 1.1.2
 Summary: Web assets package for H2O Lightwave apps.
 Project-URL: Homepage, https://wave.h2o.ai/
 Project-URL: Documentation, https://wave.h2o.ai/
 Project-URL: Repository, https://github.com/h2oai/wave
 Project-URL: Changelog, https://github.com/h2oai/wave/releases
 Author-email: Martin Turoci <martin.turoci@h2o.ai>
 License-Expression: Apache-2.0
```

## Comparing `h2o_lightwave_web-1.1.1.dist-info/RECORD` & `h2o_lightwave_web-1.1.2.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 h2o_lightwave_web/__init__.py,sha256=1P8NujDvF1cYLd8AcbY9DmFPPhinzApMkZtmhjyAHns,1366
-h2o_lightwave_web/version.py,sha256=E-6wAZjiLRVInABFxrWoqdYlO_t-zVhK8XNfNnaDyzI,22
+h2o_lightwave_web/version.py,sha256=YU_42OPd3M71CKuaAhmAM5b8bOg7D_phtEEaKy2kXNg,22
 h2o_lightwave_web/www/favicon.ico,sha256=FPpb5p8o5YGKU3lDfD3oIS5ArCkxsc1rHLdTDUK0VFY,15406
 h2o_lightwave_web/www/index.html,sha256=Jtd0_C0tQTvg-z6xCrAlOv96tD0hebwgClKTPJChp2A,2380
 h2o_lightwave_web/www/logo192.png,sha256=aUspjyZY5NN3YgUo-YI6fCHCYAlS1L5BIc1d5e63mS0,2903
 h2o_lightwave_web/www/logo512.png,sha256=BJgXC3qJrhR6EPlmwrI6qYkhn_Q8cU7Wft--f1ttBEM,10723
 h2o_lightwave_web/www/manifest.json,sha256=yYobweRZfWKMHO_bVylpZ-iXDhDoPIZZ9ZYDpeihiLU,476
 h2o_lightwave_web/www/robots.txt,sha256=kNJLw79pisHhc3OVAimMzKcq3x9WT6sF9IS4xI0crdI,67
 h2o_lightwave_web/www/wave-static/1c-3f7bb63f.js,sha256=2xOnigcwGLAZI5vrdpazJ8lf0FzzfGPSl3skQsfjqlc,55190
@@ -820,11 +820,11 @@
 h2o_lightwave_web/www/wave-static/yaml-legacy-5fac3622.js,sha256=5cvmalvpHA9Oj25k44GAcf1HG7YDniegQ66V4dgE6r0,1764
 h2o_lightwave_web/www/wave-static/yaml.js-3a05ad15.js,sha256=7r7GUqf5L2A1ovmFfzFvHL7P5FaNIdDerYVzfVn1bvs,270
 h2o_lightwave_web/www/wave-static/yaml.js-legacy-fd5075f2.js,sha256=ClJPja2soS-NJRya0i6hEfDn7WytcRrIhyNWWcRF_HA,376
 h2o_lightwave_web/www/wave-static/zephir-cf2a8bcb.js,sha256=ODXXY7gdwlczYMEzETu7RfWMqFB7tKnNjTcS1eqGj6E,1557
 h2o_lightwave_web/www/wave-static/zephir-legacy-56a6ea33.js,sha256=JkDxN65viU3DL5qdbVC2Y9KpHL6JpBGM6vMw1rbCiPI,1626
 h2o_lightwave_web/www/wave-static/zephir.js-fa8df6f1.js,sha256=QDO6mKLWpOMY8efMlYgMPufoQZVYkaBuI324ITQH66Q,276
 h2o_lightwave_web/www/wave-static/zephir.js-legacy-cf8f00c6.js,sha256=0maNcDPP6AvMgcSEQ1YUW_ylVP4o_x132PPKd33pUWg,382
-h2o_lightwave_web-1.1.1.dist-info/METADATA,sha256=baQrJwq4kTfzI7XPqNaVv5hsF7yj6KWEKrRcU_gzwBQ,1347
-h2o_lightwave_web-1.1.1.dist-info/WHEEL,sha256=TJPnKdtrSue7xZ_AVGkp9YXcvDrobsjBds1du3Nx6dc,87
-h2o_lightwave_web-1.1.1.dist-info/licenses/LICENSE,sha256=hpuFayniDwysSKD0tHGELH2KJDVyhUrKS29torRIpqY,53
-h2o_lightwave_web-1.1.1.dist-info/RECORD,,
+h2o_lightwave_web-1.1.2.dist-info/METADATA,sha256=yr92pNkAFoRjIqyzkw9cZGpNfTRo-ekESQpylQnmcag,1347
+h2o_lightwave_web-1.1.2.dist-info/WHEEL,sha256=uNdcs2TADwSd5pVaP0Z_kcjcvvTUklh2S7bxZMF8Uj0,87
+h2o_lightwave_web-1.1.2.dist-info/licenses/LICENSE,sha256=hpuFayniDwysSKD0tHGELH2KJDVyhUrKS29torRIpqY,53
+h2o_lightwave_web-1.1.2.dist-info/RECORD,,
```

