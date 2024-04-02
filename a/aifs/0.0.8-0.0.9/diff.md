# Comparing `tmp/aifs-0.0.8.tar.gz` & `tmp/aifs-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aifs-0.0.8.tar", max compression
+gzip compressed data, was "aifs-0.0.9.tar", max compression
```

## Comparing `aifs-0.0.8.tar` & `aifs-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11357 2024-02-04 01:52:13.158570 aifs-0.0.8/LICENSE
--rw-r--r--   0        0        0     2573 2024-02-10 11:15:09.741298 aifs-0.0.8/README.md
--rw-r--r--   0        0        0       26 2024-01-16 09:04:43.894880 aifs-0.0.8/aifs/__init__.py
--rw-r--r--   0        0        0     7713 2024-02-08 19:49:43.247120 aifs-0.0.8/aifs/search.py
--rw-r--r--   0        0        0      270 2024-02-08 19:47:13.944446 aifs-0.0.8/aifs/test.py
--rw-r--r--   0        0        0    94943 2024-02-04 01:52:13.162217 aifs-0.0.8/aifs/testfuncs/_.aifs
--rw-r--r--   0        0        0       94 2024-02-04 01:52:13.162605 aifs-0.0.8/aifs/testfuncs/bookTicket.py
--rw-r--r--   0        0        0      104 2024-02-04 01:52:13.162812 aifs-0.0.8/aifs/testfuncs/browseWeb.py
--rw-r--r--   0        0        0       88 2024-02-04 01:52:13.162998 aifs-0.0.8/aifs/testfuncs/cookDish.py
--rw-r--r--   0        0        0       93 2024-02-04 01:52:13.163167 aifs-0.0.8/aifs/testfuncs/doLaundry.py
--rw-r--r--   0        0        0       95 2024-02-04 01:52:13.163334 aifs-0.0.8/aifs/testfuncs/drinkAlcohol.py
--rw-r--r--   0        0        0      102 2024-02-04 01:52:13.163531 aifs-0.0.8/aifs/testfuncs/executiveAssistant.py
--rw-r--r--   0        0        0       95 2024-02-04 01:52:13.163758 aifs-0.0.8/aifs/testfuncs/liftWeights.py
--rw-r--r--   0        0        0      125 2024-02-04 01:52:13.163961 aifs-0.0.8/aifs/testfuncs/lowerBrightness.py
--rw-r--r--   0        0        0       92 2024-02-04 01:52:13.164133 aifs-0.0.8/aifs/testfuncs/playTennis.py
--rw-r--r--   0        0        0       90 2024-02-04 01:52:13.164332 aifs-0.0.8/aifs/testfuncs/sendEmail.py
--rw-r--r--   0        0        0       87 2024-02-04 01:52:13.164533 aifs-0.0.8/aifs/testfuncs/setAlarm.py
--rw-r--r--   0        0        0      435 2024-02-10 11:15:34.242140 aifs-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3208 1970-01-01 00:00:00.000000 aifs-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-02-04 01:52:13.158570 aifs-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2573 2024-02-10 11:15:09.741298 aifs-0.0.9/README.md
+-rw-r--r--   0        0        0       26 2024-01-16 09:04:43.894880 aifs-0.0.9/aifs/__init__.py
+-rw-r--r--   0        0        0    10264 2024-02-19 04:49:32.243708 aifs-0.0.9/aifs/search.py
+-rw-r--r--   0        0        0      270 2024-02-08 19:47:13.944446 aifs-0.0.9/aifs/test.py
+-rw-r--r--   0        0        0    94943 2024-02-04 01:52:13.162217 aifs-0.0.9/aifs/testfuncs/_.aifs
+-rw-r--r--   0        0        0       94 2024-02-04 01:52:13.162605 aifs-0.0.9/aifs/testfuncs/bookTicket.py
+-rw-r--r--   0        0        0      104 2024-02-04 01:52:13.162812 aifs-0.0.9/aifs/testfuncs/browseWeb.py
+-rw-r--r--   0        0        0       88 2024-02-04 01:52:13.162998 aifs-0.0.9/aifs/testfuncs/cookDish.py
+-rw-r--r--   0        0        0       93 2024-02-04 01:52:13.163167 aifs-0.0.9/aifs/testfuncs/doLaundry.py
+-rw-r--r--   0        0        0       95 2024-02-04 01:52:13.163334 aifs-0.0.9/aifs/testfuncs/drinkAlcohol.py
+-rw-r--r--   0        0        0      102 2024-02-04 01:52:13.163531 aifs-0.0.9/aifs/testfuncs/executiveAssistant.py
+-rw-r--r--   0        0        0       95 2024-02-04 01:52:13.163758 aifs-0.0.9/aifs/testfuncs/liftWeights.py
+-rw-r--r--   0        0        0      125 2024-02-04 01:52:13.163961 aifs-0.0.9/aifs/testfuncs/lowerBrightness.py
+-rw-r--r--   0        0        0       92 2024-02-04 01:52:13.164133 aifs-0.0.9/aifs/testfuncs/playTennis.py
+-rw-r--r--   0        0        0       90 2024-02-04 01:52:13.164332 aifs-0.0.9/aifs/testfuncs/sendEmail.py
+-rw-r--r--   0        0        0       87 2024-02-04 01:52:13.164533 aifs-0.0.9/aifs/testfuncs/setAlarm.py
+-rw-r--r--   0        0        0      435 2024-02-19 04:49:45.684649 aifs-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3208 1970-01-01 00:00:00.000000 aifs-0.0.9/PKG-INFO
```

### Comparing `aifs-0.0.8/LICENSE` & `aifs-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aifs-0.0.8/README.md` & `aifs-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `aifs-0.0.8/aifs/testfuncs/_.aifs` & `aifs-0.0.9/aifs/testfuncs/_.aifs`

 * *Files identical despite different names*

### Comparing `aifs-0.0.8/PKG-INFO` & `aifs-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aifs
-Version: 0.0.8
+Version: 0.0.9
 Summary: Local semantic search. Stupidly simple.
 License: MIT
 Author: Killian Lucas
 Author-email: killian@openinterpreter.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

