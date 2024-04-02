# Comparing `tmp/logicplum-ai-1.3.7.tar.gz` & `tmp/logicplum-ai-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\WORK\AI CLOUD 4.0\package pYpI\aicloudlp\aicloud-lp-new\dist\.tmp-xpew3ygn\logicplum-ai-1.3.7.tar", last modified: Thu Mar  7 07:30:56 2024, max compression
+gzip compressed data, was "C:\WORK\AI CLOUD 4.0\package pYpI\aicloudlp\aicloud-lp-new\dist\.tmp-ez7bt7r7\logicplum-ai-1.3.8.tar", last modified: Tue Apr  2 11:11:03 2024, max compression
```

## Comparing `logicplum-ai-1.3.7.tar` & `logicplum-ai-1.3.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-03-07 07:30:56.305496 logicplum-ai-1.3.7/
--rw-rw-rw-   0        0        0     2105 2024-03-07 07:30:28.000000 logicplum-ai-1.3.7/CHANGELOG.md
--rw-rw-rw-   0        0        0     2280 2024-03-07 07:30:56.302966 logicplum-ai-1.3.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-07 07:30:56.262509 logicplum-ai-1.3.7/logicplum/
--rw-rw-rw-   0        0        0        0 2023-12-14 07:41:33.000000 logicplum-ai-1.3.7/logicplum/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-07 07:30:56.265668 logicplum-ai-1.3.7/logicplum/aicloud/
--rw-rw-rw-   0        0        0        0 2023-12-19 05:50:45.000000 logicplum-ai-1.3.7/logicplum/aicloud/__init__.py
--rw-rw-rw-   0        0        0      141 2024-02-15 09:04:54.000000 logicplum-ai-1.3.7/logicplum/aicloud/config.py
-drwxrwxrwx   0        0        0        0 2024-03-07 07:30:56.267682 logicplum-ai-1.3.7/logicplum/aicloud/modeling/
--rw-rw-rw-   0        0        0       97 2023-12-19 05:50:45.000000 logicplum-ai-1.3.7/logicplum/aicloud/modeling/__init__.py
--rw-rw-rw-   0        0        0     5424 2024-03-06 08:02:58.000000 logicplum-ai-1.3.7/logicplum/aicloud/modeling/training.py
-drwxrwxrwx   0        0        0        0 2024-03-07 07:30:56.269671 logicplum-ai-1.3.7/logicplum/aicloud/monitoring/
--rw-rw-rw-   0        0        0       31 2023-12-19 05:50:45.000000 logicplum-ai-1.3.7/logicplum/aicloud/monitoring/__init__.py
--rw-rw-rw-   0        0        0     3552 2024-03-06 08:23:49.000000 logicplum-ai-1.3.7/logicplum/aicloud/monitoring/model_monitoring.py
-drwxrwxrwx   0        0        0        0 2024-03-07 07:30:56.277226 logicplum-ai-1.3.7/logicplum/aicloud/plots/
--rw-rw-rw-   0        0        0       26 2023-12-19 05:50:46.000000 logicplum-ai-1.3.7/logicplum/aicloud/plots/__init__.py
--rw-rw-rw-   0        0        0     3484 2024-03-06 08:24:00.000000 logicplum-ai-1.3.7/logicplum/aicloud/plots/graph_plots.py
-drwxrwxrwx   0        0        0        0 2024-03-07 07:30:56.282226 logicplum-ai-1.3.7/logicplum/aicloud/prediction/
--rw-rw-rw-   0        0        0       29 2023-12-19 05:50:46.000000 logicplum-ai-1.3.7/logicplum/aicloud/prediction/__init__.py
--rw-rw-rw-   0        0        0     2190 2024-03-06 08:32:18.000000 logicplum-ai-1.3.7/logicplum/aicloud/prediction/get_prediction.py
-drwxrwxrwx   0        0        0        0 2024-03-07 07:30:56.284227 logicplum-ai-1.3.7/logicplum/aicloud/reports/
--rw-rw-rw-   0        0        0       25 2023-12-19 05:50:46.000000 logicplum-ai-1.3.7/logicplum/aicloud/reports/__init__.py
--rw-rw-rw-   0        0        0     1482 2024-03-06 08:31:59.000000 logicplum-ai-1.3.7/logicplum/aicloud/reports/get_report.py
-drwxrwxrwx   0        0        0        0 2024-03-07 07:30:56.286354 logicplum-ai-1.3.7/logicplum/aicloud/status/
--rw-rw-rw-   0        0        0       25 2023-12-19 05:50:46.000000 logicplum-ai-1.3.7/logicplum/aicloud/status/__init__.py
--rw-rw-rw-   0        0        0      795 2024-03-06 08:31:52.000000 logicplum-ai-1.3.7/logicplum/aicloud/status/get_status.py
-drwxrwxrwx   0        0        0        0 2024-03-07 07:30:56.294357 logicplum-ai-1.3.7/logicplum/aicloud/users/
--rw-rw-rw-   0        0        0       21 2023-12-19 05:50:46.000000 logicplum-ai-1.3.7/logicplum/aicloud/users/__init__.py
--rw-rw-rw-   0        0        0     1190 2024-03-07 07:29:54.000000 logicplum-ai-1.3.7/logicplum/aicloud/users/client.py
-drwxrwxrwx   0        0        0        0 2024-03-07 07:30:56.301460 logicplum-ai-1.3.7/logicplum_ai.egg-info/
--rw-rw-rw-   0        0        0     2280 2024-03-07 07:30:56.000000 logicplum-ai-1.3.7/logicplum_ai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      835 2024-03-07 07:30:56.000000 logicplum-ai-1.3.7/logicplum_ai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-07 07:30:56.000000 logicplum-ai-1.3.7/logicplum_ai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-03-07 07:30:56.000000 logicplum-ai-1.3.7/logicplum_ai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-07 07:30:56.000000 logicplum-ai-1.3.7/logicplum_ai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-07 07:30:56.305496 logicplum-ai-1.3.7/setup.cfg
--rw-rw-rw-   0        0        0      580 2024-03-07 07:30:34.000000 logicplum-ai-1.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:11:03.123609 logicplum-ai-1.3.8/
+-rw-rw-rw-   0        0        0     2161 2024-04-02 11:09:11.000000 logicplum-ai-1.3.8/CHANGELOG.md
+-rw-rw-rw-   0        0        0     2313 2024-04-02 11:11:03.123609 logicplum-ai-1.3.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-02 11:11:03.092364 logicplum-ai-1.3.8/logicplum/
+-rw-rw-rw-   0        0        0        0 2023-12-14 07:41:33.000000 logicplum-ai-1.3.8/logicplum/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:11:03.092364 logicplum-ai-1.3.8/logicplum/aicloud/
+-rw-rw-rw-   0        0        0        0 2023-12-19 05:50:45.000000 logicplum-ai-1.3.8/logicplum/aicloud/__init__.py
+-rw-rw-rw-   0        0        0      141 2024-02-15 09:04:54.000000 logicplum-ai-1.3.8/logicplum/aicloud/config.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:11:03.092364 logicplum-ai-1.3.8/logicplum/aicloud/modeling/
+-rw-rw-rw-   0        0        0       97 2023-12-19 05:50:45.000000 logicplum-ai-1.3.8/logicplum/aicloud/modeling/__init__.py
+-rw-rw-rw-   0        0        0     5424 2024-03-06 08:02:58.000000 logicplum-ai-1.3.8/logicplum/aicloud/modeling/training.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:11:03.092364 logicplum-ai-1.3.8/logicplum/aicloud/monitoring/
+-rw-rw-rw-   0        0        0       31 2023-12-19 05:50:45.000000 logicplum-ai-1.3.8/logicplum/aicloud/monitoring/__init__.py
+-rw-rw-rw-   0        0        0     3552 2024-03-06 08:23:49.000000 logicplum-ai-1.3.8/logicplum/aicloud/monitoring/model_monitoring.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:11:03.107984 logicplum-ai-1.3.8/logicplum/aicloud/plots/
+-rw-rw-rw-   0        0        0       26 2023-12-19 05:50:46.000000 logicplum-ai-1.3.8/logicplum/aicloud/plots/__init__.py
+-rw-rw-rw-   0        0        0     3484 2024-03-06 08:24:00.000000 logicplum-ai-1.3.8/logicplum/aicloud/plots/graph_plots.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:11:03.107984 logicplum-ai-1.3.8/logicplum/aicloud/prediction/
+-rw-rw-rw-   0        0        0       29 2023-12-19 05:50:46.000000 logicplum-ai-1.3.8/logicplum/aicloud/prediction/__init__.py
+-rw-rw-rw-   0        0        0     2190 2024-03-06 08:32:18.000000 logicplum-ai-1.3.8/logicplum/aicloud/prediction/get_prediction.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:11:03.107984 logicplum-ai-1.3.8/logicplum/aicloud/reports/
+-rw-rw-rw-   0        0        0       25 2023-12-19 05:50:46.000000 logicplum-ai-1.3.8/logicplum/aicloud/reports/__init__.py
+-rw-rw-rw-   0        0        0     1482 2024-03-06 08:31:59.000000 logicplum-ai-1.3.8/logicplum/aicloud/reports/get_report.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:11:03.107984 logicplum-ai-1.3.8/logicplum/aicloud/status/
+-rw-rw-rw-   0        0        0       25 2023-12-19 05:50:46.000000 logicplum-ai-1.3.8/logicplum/aicloud/status/__init__.py
+-rw-rw-rw-   0        0        0      795 2024-03-06 08:31:52.000000 logicplum-ai-1.3.8/logicplum/aicloud/status/get_status.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:11:03.107984 logicplum-ai-1.3.8/logicplum/aicloud/users/
+-rw-rw-rw-   0        0        0       21 2023-12-19 05:50:46.000000 logicplum-ai-1.3.8/logicplum/aicloud/users/__init__.py
+-rw-rw-rw-   0        0        0     1190 2024-03-07 07:29:54.000000 logicplum-ai-1.3.8/logicplum/aicloud/users/client.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:11:03.123609 logicplum-ai-1.3.8/logicplum_ai.egg-info/
+-rw-rw-rw-   0        0        0     2313 2024-04-02 11:11:03.000000 logicplum-ai-1.3.8/logicplum_ai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      835 2024-04-02 11:11:03.000000 logicplum-ai-1.3.8/logicplum_ai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 11:11:03.000000 logicplum-ai-1.3.8/logicplum_ai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-02 11:11:03.000000 logicplum-ai-1.3.8/logicplum_ai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-02 11:11:03.000000 logicplum-ai-1.3.8/logicplum_ai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 11:11:03.123609 logicplum-ai-1.3.8/setup.cfg
+-rw-rw-rw-   0        0        0      561 2024-04-02 11:10:23.000000 logicplum-ai-1.3.8/setup.py
```

### Comparing `logicplum-ai-1.3.7/CHANGELOG.md` & `logicplum-ai-1.3.8/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -110,8 +110,11 @@
 ## [1.3.5] - 2023-12-08
 - fixes.
 
 ## [1.3.6] - 2023-12-08
 - fixes.
 
 ## [1.3.7] - 2023-12-08
-- fixes.
+- fixes.
+
+## [1.3.8] - 2024-04-02
+- removed unwanted modules.
```

### Comparing `logicplum-ai-1.3.7/PKG-INFO` & `logicplum-ai-1.3.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: logicplum-ai
-Version: 1.3.7
+Version: 1.3.8
 Description-Content-Type: text/markdown
 Requires-Dist: requests
-Requires-Dist: pandas
 Requires-Dist: Pillow
 
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 ## [1.0.0] - 2023-12-08
@@ -119,7 +118,10 @@
 - fixes.
 
 ## [1.3.6] - 2023-12-08
 - fixes.
 
 ## [1.3.7] - 2023-12-08
 - fixes.
+
+## [1.3.8] - 2024-04-02
+- removed unwanted modules.
```

### Comparing `logicplum-ai-1.3.7/logicplum/aicloud/modeling/training.py` & `logicplum-ai-1.3.8/logicplum/aicloud/modeling/training.py`

 * *Files identical despite different names*

### Comparing `logicplum-ai-1.3.7/logicplum/aicloud/monitoring/model_monitoring.py` & `logicplum-ai-1.3.8/logicplum/aicloud/monitoring/model_monitoring.py`

 * *Files identical despite different names*

### Comparing `logicplum-ai-1.3.7/logicplum/aicloud/plots/graph_plots.py` & `logicplum-ai-1.3.8/logicplum/aicloud/plots/graph_plots.py`

 * *Files identical despite different names*

### Comparing `logicplum-ai-1.3.7/logicplum/aicloud/prediction/get_prediction.py` & `logicplum-ai-1.3.8/logicplum/aicloud/prediction/get_prediction.py`

 * *Files identical despite different names*

### Comparing `logicplum-ai-1.3.7/logicplum/aicloud/reports/get_report.py` & `logicplum-ai-1.3.8/logicplum/aicloud/reports/get_report.py`

 * *Files identical despite different names*

### Comparing `logicplum-ai-1.3.7/logicplum/aicloud/status/get_status.py` & `logicplum-ai-1.3.8/logicplum/aicloud/status/get_status.py`

 * *Files identical despite different names*

### Comparing `logicplum-ai-1.3.7/logicplum/aicloud/users/client.py` & `logicplum-ai-1.3.8/logicplum/aicloud/users/client.py`

 * *Files identical despite different names*

### Comparing `logicplum-ai-1.3.7/logicplum_ai.egg-info/PKG-INFO` & `logicplum-ai-1.3.8/logicplum_ai.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: logicplum-ai
-Version: 1.3.7
+Version: 1.3.8
 Description-Content-Type: text/markdown
 Requires-Dist: requests
-Requires-Dist: pandas
 Requires-Dist: Pillow
 
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 ## [1.0.0] - 2023-12-08
@@ -119,7 +118,10 @@
 - fixes.
 
 ## [1.3.6] - 2023-12-08
 - fixes.
 
 ## [1.3.7] - 2023-12-08
 - fixes.
+
+## [1.3.8] - 2024-04-02
+- removed unwanted modules.
```

### Comparing `logicplum-ai-1.3.7/logicplum_ai.egg-info/SOURCES.txt` & `logicplum-ai-1.3.8/logicplum_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logicplum-ai-1.3.7/setup.py` & `logicplum-ai-1.3.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 current_dir = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(current_dir, "CHANGELOG.md"), "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='logicplum-ai',
-    version='1.3.7',  # Update the version number
+    version='1.3.8',  # Update the version number
     packages=find_packages(),
     install_requires=[
         'requests',
-        'pandas',
         'Pillow'
     ],
     long_description=long_description,
     long_description_content_type="text/markdown",
 )
```

