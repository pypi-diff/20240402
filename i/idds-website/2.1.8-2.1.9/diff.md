# Comparing `tmp/idds-website-2.1.8.tar.gz` & `tmp/idds-website-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idds-website-2.1.8.tar", last modified: Wed Jan 31 16:35:25 2024, max compression
+gzip compressed data, was "idds-website-2.1.9.tar", last modified: Wed Jan 31 17:27:23 2024, max compression
```

## Comparing `idds-website-2.1.8.tar` & `idds-website-2.1.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:25.895248 idds-website-2.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-01-31 16:35:12.000000 idds-website-2.1.8/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-01-31 16:35:25.895248 idds-website-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-01-31 16:35:12.000000 idds-website-2.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:25.879248 idds-website-2.1.8/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:25.879248 idds-website-2.1.8/data/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:25.879248 idds-website-2.1.8/data/assets/css/
--rw-r--r--   0 runner    (1001) docker     (127)    29063 2024-01-31 16:35:12.000000 idds-website-2.1.8/data/assets/css/font-awesome.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    79155 2024-01-31 16:35:12.000000 idds-website-2.1.8/data/assets/css/main.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:25.883248 idds-website-2.1.8/data/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   124988 2024-01-31 16:35:12.000000 idds-website-2.1.8/data/assets/fonts/FontAwesome.otf
--rw-r--r--   0 runner    (1001) docker     (127)    76518 2024-01-31 16:35:12.000000 idds-website-2.1.8/data/assets/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (127)   391622 2024-01-31 16:35:12.000000 idds-website-2.1.8/data/assets/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (127)   152796 2024-01-31 16:35:12.000000 idds-website-2.1.8/data/assets/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    90412 2024-01-31 16:35:12.000000 idds-website-2.1.8/data/assets/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (127)    71896 2024-01-31 16:35:12.000000 idds-website-2.1.8/data/assets/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:25.883248 idds-website-2.1.8/data/assets/js/
--rw-r--r--   0 runner    (1001) docker     (127)    95957 2024-01-31 16:35:12.000000 idds-website-2.1.8/data/assets/js/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-01-31 16:35:12.000000 idds-website-2.1.8/data/assets/js/jquery.scrollex.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     6557 2024-01-31 16:35:12.000000 idds-website-2.1.8/data/assets/js/main.js
--rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-01-31 16:35:12.000000 idds-website-2.1.8/data/assets/js/skel.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    12433 2024-01-31 16:35:12.000000 idds-website-2.1.8/data/assets/js/util.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:25.891248 idds-website-2.1.8/data/images/
--rw-r--r--   0 runner    (1001) docker     (127)   474892 2024-01-31 16:35:12.000000 idds-website-2.1.8/data/images/bg.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    19506 2024-01-31 16:35:12.000000 idds-website-2.1.8/data/images/idds.png
--rw-r--r--   0 runner    (1001) docker     (127)   185271 2024-01-31 16:35:12.000000 idds-website-2.1.8/data/images/idds_architecture.png
--rw-r--r--   0 runner    (1001) docker     (127)   207445 2024-01-31 16:35:12.000000 idds-website-2.1.8/data/images/idds_components.png
--rw-r--r--   0 runner    (1001) docker     (127)   291395 2024-01-31 16:35:12.000000 idds-website-2.1.8/data/images/idds_delivery.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   351386 2024-01-31 16:35:12.000000 idds-website-2.1.8/data/images/idds_full.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   216628 2024-01-31 16:35:12.000000 idds-website-2.1.8/data/images/idds_intelligent.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   245328 2024-01-31 16:35:12.000000 idds-website-2.1.8/data/images/idds_main.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   102173 2024-01-31 16:35:12.000000 idds-website-2.1.8/data/images/idds_orchestration.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   191197 2024-01-31 16:35:12.000000 idds-website-2.1.8/data/images/idds_transform.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-01-31 16:35:12.000000 idds-website-2.1.8/data/images/images.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    62680 2024-01-31 16:35:12.000000 idds-website-2.1.8/data/images/pic01.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    73227 2024-01-31 16:35:12.000000 idds-website-2.1.8/data/images/pic02.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    51569 2024-01-31 16:35:12.000000 idds-website-2.1.8/data/images/pic03.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    55020 2024-01-31 16:35:12.000000 idds-website-2.1.8/data/images/pic04.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   575353 2024-01-31 16:35:12.000000 idds-website-2.1.8/data/images/slide01.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   343913 2024-01-31 16:35:12.000000 idds-website-2.1.8/data/images/slide02.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   547740 2024-01-31 16:35:12.000000 idds-website-2.1.8/data/images/slide03.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   351032 2024-01-31 16:35:12.000000 idds-website-2.1.8/data/images/slide04.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   505742 2024-01-31 16:35:12.000000 idds-website-2.1.8/data/images/slide05.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    11608 2024-01-31 16:35:12.000000 idds-website-2.1.8/data/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:25.879248 idds-website-2.1.8/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:25.891248 idds-website-2.1.8/lib/idds/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-website-2.1.8/lib/idds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:25.891248 idds-website-2.1.8/lib/idds/website/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-website-2.1.8/lib/idds/website/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-01-31 16:35:22.000000 idds-website-2.1.8/lib/idds/website/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:25.895248 idds-website-2.1.8/lib/idds_website.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-01-31 16:35:25.000000 idds-website-2.1.8/lib/idds_website.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-01-31 16:35:25.000000 idds-website-2.1.8/lib/idds_website.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 16:35:25.000000 idds-website-2.1.8/lib/idds_website.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-31 16:35:25.000000 idds-website-2.1.8/lib/idds_website.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-01-31 16:35:25.895248 idds-website-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-01-31 16:35:12.000000 idds-website-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:23.173891 idds-website-2.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-01-31 17:27:09.000000 idds-website-2.1.9/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-01-31 17:27:23.173891 idds-website-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-01-31 17:27:09.000000 idds-website-2.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:23.161891 idds-website-2.1.9/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:23.157891 idds-website-2.1.9/data/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:23.161891 idds-website-2.1.9/data/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    29063 2024-01-31 17:27:09.000000 idds-website-2.1.9/data/assets/css/font-awesome.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    79155 2024-01-31 17:27:09.000000 idds-website-2.1.9/data/assets/css/main.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:23.161891 idds-website-2.1.9/data/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   124988 2024-01-31 17:27:09.000000 idds-website-2.1.9/data/assets/fonts/FontAwesome.otf
+-rw-r--r--   0 runner    (1001) docker     (127)    76518 2024-01-31 17:27:09.000000 idds-website-2.1.9/data/assets/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   391622 2024-01-31 17:27:09.000000 idds-website-2.1.9/data/assets/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   152796 2024-01-31 17:27:09.000000 idds-website-2.1.9/data/assets/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    90412 2024-01-31 17:27:09.000000 idds-website-2.1.9/data/assets/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    71896 2024-01-31 17:27:09.000000 idds-website-2.1.9/data/assets/fonts/fontawesome-webfont.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:23.161891 idds-website-2.1.9/data/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    95957 2024-01-31 17:27:09.000000 idds-website-2.1.9/data/assets/js/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-01-31 17:27:09.000000 idds-website-2.1.9/data/assets/js/jquery.scrollex.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6557 2024-01-31 17:27:09.000000 idds-website-2.1.9/data/assets/js/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-01-31 17:27:09.000000 idds-website-2.1.9/data/assets/js/skel.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12433 2024-01-31 17:27:09.000000 idds-website-2.1.9/data/assets/js/util.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:23.173891 idds-website-2.1.9/data/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   474892 2024-01-31 17:27:09.000000 idds-website-2.1.9/data/images/bg.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    19506 2024-01-31 17:27:09.000000 idds-website-2.1.9/data/images/idds.png
+-rw-r--r--   0 runner    (1001) docker     (127)   185271 2024-01-31 17:27:09.000000 idds-website-2.1.9/data/images/idds_architecture.png
+-rw-r--r--   0 runner    (1001) docker     (127)   207445 2024-01-31 17:27:09.000000 idds-website-2.1.9/data/images/idds_components.png
+-rw-r--r--   0 runner    (1001) docker     (127)   291395 2024-01-31 17:27:09.000000 idds-website-2.1.9/data/images/idds_delivery.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   351386 2024-01-31 17:27:09.000000 idds-website-2.1.9/data/images/idds_full.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   216628 2024-01-31 17:27:09.000000 idds-website-2.1.9/data/images/idds_intelligent.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   245328 2024-01-31 17:27:09.000000 idds-website-2.1.9/data/images/idds_main.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   102173 2024-01-31 17:27:09.000000 idds-website-2.1.9/data/images/idds_orchestration.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   191197 2024-01-31 17:27:09.000000 idds-website-2.1.9/data/images/idds_transform.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-01-31 17:27:09.000000 idds-website-2.1.9/data/images/images.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    62680 2024-01-31 17:27:09.000000 idds-website-2.1.9/data/images/pic01.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    73227 2024-01-31 17:27:09.000000 idds-website-2.1.9/data/images/pic02.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    51569 2024-01-31 17:27:09.000000 idds-website-2.1.9/data/images/pic03.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    55020 2024-01-31 17:27:09.000000 idds-website-2.1.9/data/images/pic04.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   575353 2024-01-31 17:27:09.000000 idds-website-2.1.9/data/images/slide01.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   343913 2024-01-31 17:27:09.000000 idds-website-2.1.9/data/images/slide02.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   547740 2024-01-31 17:27:09.000000 idds-website-2.1.9/data/images/slide03.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   351032 2024-01-31 17:27:09.000000 idds-website-2.1.9/data/images/slide04.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   505742 2024-01-31 17:27:09.000000 idds-website-2.1.9/data/images/slide05.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    11608 2024-01-31 17:27:09.000000 idds-website-2.1.9/data/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:23.157891 idds-website-2.1.9/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:23.173891 idds-website-2.1.9/lib/idds/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-website-2.1.9/lib/idds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:23.173891 idds-website-2.1.9/lib/idds/website/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-website-2.1.9/lib/idds/website/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-01-31 17:27:19.000000 idds-website-2.1.9/lib/idds/website/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:23.173891 idds-website-2.1.9/lib/idds_website.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-01-31 17:27:23.000000 idds-website-2.1.9/lib/idds_website.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-01-31 17:27:23.000000 idds-website-2.1.9/lib/idds_website.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 17:27:23.000000 idds-website-2.1.9/lib/idds_website.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-31 17:27:23.000000 idds-website-2.1.9/lib/idds_website.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-01-31 17:27:23.173891 idds-website-2.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-01-31 17:27:09.000000 idds-website-2.1.9/setup.py
```

### Comparing `idds-website-2.1.8/LICENSE.rst` & `idds-website-2.1.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `idds-website-2.1.8/PKG-INFO` & `idds-website-2.1.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-website
-Version: 2.1.8
+Version: 2.1.9
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-website-2.1.8/data/assets/css/font-awesome.min.css` & `idds-website-2.1.9/data/assets/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `idds-website-2.1.8/data/assets/css/main.css` & `idds-website-2.1.9/data/assets/css/main.css`

 * *Files identical despite different names*

### Comparing `idds-website-2.1.8/data/assets/fonts/FontAwesome.otf` & `idds-website-2.1.9/data/assets/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `idds-website-2.1.8/data/assets/fonts/fontawesome-webfont.eot` & `idds-website-2.1.9/data/assets/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `idds-website-2.1.8/data/assets/fonts/fontawesome-webfont.svg` & `idds-website-2.1.9/data/assets/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `idds-website-2.1.8/data/assets/fonts/fontawesome-webfont.ttf` & `idds-website-2.1.9/data/assets/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `idds-website-2.1.8/data/assets/fonts/fontawesome-webfont.woff` & `idds-website-2.1.9/data/assets/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `idds-website-2.1.8/data/assets/fonts/fontawesome-webfont.woff2` & `idds-website-2.1.9/data/assets/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `idds-website-2.1.8/data/assets/js/jquery.min.js` & `idds-website-2.1.9/data/assets/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `idds-website-2.1.8/data/assets/js/jquery.scrollex.min.js` & `idds-website-2.1.9/data/assets/js/jquery.scrollex.min.js`

 * *Files identical despite different names*

### Comparing `idds-website-2.1.8/data/assets/js/main.js` & `idds-website-2.1.9/data/assets/js/main.js`

 * *Files identical despite different names*

### Comparing `idds-website-2.1.8/data/assets/js/skel.min.js` & `idds-website-2.1.9/data/assets/js/skel.min.js`

 * *Files identical despite different names*

### Comparing `idds-website-2.1.8/data/assets/js/util.js` & `idds-website-2.1.9/data/assets/js/util.js`

 * *Files identical despite different names*

### Comparing `idds-website-2.1.8/data/images/bg.jpg` & `idds-website-2.1.9/data/images/bg.jpg`

 * *Files identical despite different names*

### Comparing `idds-website-2.1.8/data/images/idds.png` & `idds-website-2.1.9/data/images/idds.png`

 * *Files identical despite different names*

### Comparing `idds-website-2.1.8/data/images/idds_architecture.png` & `idds-website-2.1.9/data/images/idds_architecture.png`

 * *Files identical despite different names*

### Comparing `idds-website-2.1.8/data/images/idds_components.png` & `idds-website-2.1.9/data/images/idds_components.png`

 * *Files identical despite different names*

### Comparing `idds-website-2.1.8/data/images/idds_delivery.jpg` & `idds-website-2.1.9/data/images/idds_delivery.jpg`

 * *Files identical despite different names*

### Comparing `idds-website-2.1.8/data/images/idds_full.jpg` & `idds-website-2.1.9/data/images/idds_full.jpg`

 * *Files identical despite different names*

### Comparing `idds-website-2.1.8/data/images/idds_intelligent.jpg` & `idds-website-2.1.9/data/images/idds_intelligent.jpg`

 * *Files identical despite different names*

### Comparing `idds-website-2.1.8/data/images/idds_main.jpg` & `idds-website-2.1.9/data/images/idds_main.jpg`

 * *Files identical despite different names*

### Comparing `idds-website-2.1.8/data/images/idds_orchestration.jpg` & `idds-website-2.1.9/data/images/idds_orchestration.jpg`

 * *Files identical despite different names*

### Comparing `idds-website-2.1.8/data/images/idds_transform.jpg` & `idds-website-2.1.9/data/images/idds_transform.jpg`

 * *Files identical despite different names*

### Comparing `idds-website-2.1.8/data/images/images.jpg` & `idds-website-2.1.9/data/images/images.jpg`

 * *Files identical despite different names*

### Comparing `idds-website-2.1.8/data/images/pic01.jpg` & `idds-website-2.1.9/data/images/pic01.jpg`

 * *Files identical despite different names*

### Comparing `idds-website-2.1.8/data/images/pic02.jpg` & `idds-website-2.1.9/data/images/pic02.jpg`

 * *Files identical despite different names*

### Comparing `idds-website-2.1.8/data/images/pic03.jpg` & `idds-website-2.1.9/data/images/pic03.jpg`

 * *Files identical despite different names*

### Comparing `idds-website-2.1.8/data/images/pic04.jpg` & `idds-website-2.1.9/data/images/pic04.jpg`

 * *Files identical despite different names*

### Comparing `idds-website-2.1.8/data/images/slide01.jpg` & `idds-website-2.1.9/data/images/slide01.jpg`

 * *Files identical despite different names*

### Comparing `idds-website-2.1.8/data/images/slide02.jpg` & `idds-website-2.1.9/data/images/slide02.jpg`

 * *Files identical despite different names*

### Comparing `idds-website-2.1.8/data/images/slide03.jpg` & `idds-website-2.1.9/data/images/slide03.jpg`

 * *Files identical despite different names*

### Comparing `idds-website-2.1.8/data/images/slide04.jpg` & `idds-website-2.1.9/data/images/slide04.jpg`

 * *Files identical despite different names*

### Comparing `idds-website-2.1.8/data/images/slide05.jpg` & `idds-website-2.1.9/data/images/slide05.jpg`

 * *Files identical despite different names*

### Comparing `idds-website-2.1.8/data/index.html` & `idds-website-2.1.9/data/index.html`

 * *Files identical despite different names*

### Comparing `idds-website-2.1.8/lib/idds_website.egg-info/PKG-INFO` & `idds-website-2.1.9/lib/idds_website.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-website
-Version: 2.1.8
+Version: 2.1.9
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-website-2.1.8/lib/idds_website.egg-info/SOURCES.txt` & `idds-website-2.1.9/lib/idds_website.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idds-website-2.1.8/setup.py` & `idds-website-2.1.9/setup.py`

 * *Files identical despite different names*

