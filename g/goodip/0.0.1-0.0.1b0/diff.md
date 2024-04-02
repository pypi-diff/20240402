# Comparing `tmp/goodip-0.0.1.tar.gz` & `tmp/goodip-0.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goodip-0.0.1.tar", last modified: Tue Apr  2 14:32:46 2024, max compression
+gzip compressed data, was "goodip-0.0.1b0.tar", last modified: Tue Apr  2 14:13:02 2024, max compression
```

## Comparing `goodip-0.0.1.tar` & `goodip-0.0.1b0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 14:32:46.889324 goodip-0.0.1/
--rw-rw-rw-   0        0        0     1071 2024-02-01 09:40:20.000000 goodip-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      861 2024-04-02 14:32:46.883327 goodip-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       14 2024-04-02 14:10:10.000000 goodip-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 14:32:46.772295 goodip-0.0.1/goodip/
--rw-rw-rw-   0        0        0      330 2024-04-02 14:25:53.000000 goodip-0.0.1/goodip/__init__.py
--rw-rw-rw-   0        0        0      298 2024-04-02 13:33:13.000000 goodip-0.0.1/goodip/connection_check.py
--rw-rw-rw-   0        0        0     2053 2024-04-02 13:50:45.000000 goodip-0.0.1/goodip/ip.py
-drwxrwxrwx   0        0        0        0 2024-04-02 14:32:46.880324 goodip-0.0.1/goodip.egg-info/
--rw-rw-rw-   0        0        0      861 2024-04-02 14:32:46.000000 goodip-0.0.1/goodip.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2024-04-02 14:32:46.000000 goodip-0.0.1/goodip.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 14:32:46.000000 goodip-0.0.1/goodip.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-04-02 14:32:46.000000 goodip-0.0.1/goodip.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-02 14:32:46.000000 goodip-0.0.1/goodip.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 14:32:46.892326 goodip-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1017 2024-04-02 14:25:37.000000 goodip-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 14:13:02.366692 goodip-0.0.1b0/
+-rw-rw-rw-   0        0        0     1071 2024-02-01 09:40:20.000000 goodip-0.0.1b0/LICENSE
+-rw-rw-rw-   0        0        0      863 2024-04-02 14:13:02.191398 goodip-0.0.1b0/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2024-04-02 14:10:10.000000 goodip-0.0.1b0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 14:13:01.378532 goodip-0.0.1b0/goodip/
+-rw-rw-rw-   0        0        0       18 2024-04-02 14:09:05.000000 goodip-0.0.1b0/goodip/__init__.py
+-rw-rw-rw-   0        0        0      298 2024-04-02 13:33:13.000000 goodip-0.0.1b0/goodip/connection_check.py
+-rw-rw-rw-   0        0        0     2053 2024-04-02 13:50:45.000000 goodip-0.0.1b0/goodip/ip.py
+drwxrwxrwx   0        0        0        0 2024-04-02 14:13:02.191398 goodip-0.0.1b0/goodip.egg-info/
+-rw-rw-rw-   0        0        0      863 2024-04-02 14:13:00.000000 goodip-0.0.1b0/goodip.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2024-04-02 14:13:01.000000 goodip-0.0.1b0/goodip.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 14:13:00.000000 goodip-0.0.1b0/goodip.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-04-02 14:13:00.000000 goodip-0.0.1b0/goodip.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-02 14:13:00.000000 goodip-0.0.1b0/goodip.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 14:13:02.366692 goodip-0.0.1b0/setup.cfg
+-rw-rw-rw-   0        0        0     1022 2024-04-02 14:09:59.000000 goodip-0.0.1b0/setup.py
```

### Comparing `goodip-0.0.1/LICENSE` & `goodip-0.0.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `goodip-0.0.1/PKG-INFO` & `goodip-0.0.1b0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: goodip
-Version: 0.0.1
+Version: 0.0.1b0
 Summary: you can get your ip address and get its information.
-Home-page: https://github.com/Erfan-Bafandeh/goodip
+Home-page: https://github.com/Erfan-Bafandeh/pyrotel
 Author: Erfan Bafandeh
 Author-email: user.enbh@gmail.com
 Keywords: ip,myip,goodip,checkip
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -15,10 +15,10 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: colorama
-Requires-Dist: beautifulsoup4
+Requires-Dist: BeautifulSoup
 
 ## beta vesion
```

### Comparing `goodip-0.0.1/goodip/ip.py` & `goodip-0.0.1b0/goodip/ip.py`

 * *Files identical despite different names*

### Comparing `goodip-0.0.1/goodip.egg-info/PKG-INFO` & `goodip-0.0.1b0/goodip.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: goodip
-Version: 0.0.1
+Version: 0.0.1b0
 Summary: you can get your ip address and get its information.
-Home-page: https://github.com/Erfan-Bafandeh/goodip
+Home-page: https://github.com/Erfan-Bafandeh/pyrotel
 Author: Erfan Bafandeh
 Author-email: user.enbh@gmail.com
 Keywords: ip,myip,goodip,checkip
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -15,10 +15,10 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: colorama
-Requires-Dist: beautifulsoup4
+Requires-Dist: BeautifulSoup
 
 ## beta vesion
```

### Comparing `goodip-0.0.1/setup.py` & `goodip-0.0.1b0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'goodip',
-    version = '0.0.1',
+    version = '0.0.1-beta',
     author= 'Erfan Bafandeh',
     author_email = 'user.enbh@gmail.com',
     description = 'you can get your ip address and get its information.',
     keywords = ['ip', 'myip', 'goodip', 'checkip'],
     long_description = open("README.md", encoding="utf-8").read(),
     python_requires="~=3.6",
     long_description_content_type = 'text/markdown',
-    url = 'https://github.com/Erfan-Bafandeh/goodip',
+    url = 'https://github.com/Erfan-Bafandeh/pyrotel',
     packages = find_packages(),
-    install_requires = ["requests", "colorama", "beautifulsoup4"],
+    install_requires = ["requests", "colorama", "BeautifulSoup"],
     classifiers = [
     	"Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
```

