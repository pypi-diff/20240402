# Comparing `tmp/lambkid-0.0.8.tar.gz` & `tmp/lambkid-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lambkid-0.0.8.tar", last modified: Mon Apr  1 08:23:48 2024, max compression
+gzip compressed data, was "lambkid-0.0.9.tar", last modified: Mon Apr  1 08:27:50 2024, max compression
```

## Comparing `lambkid-0.0.8.tar` & `lambkid-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 08:23:48.824912 lambkid-0.0.8/
--rw-rw-rw-   0        0        0     1089 2024-03-27 01:13:02.000000 lambkid-0.0.8/LICENSE
--rw-rw-rw-   0        0        0       27 2024-04-01 08:22:25.000000 lambkid-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1630 2024-04-01 08:23:48.822918 lambkid-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      386 2024-04-01 07:56:09.000000 lambkid-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 08:23:48.809952 lambkid-0.0.8/docs/
--rw-rw-rw-   0        0        0       54 2024-03-31 06:58:42.000000 lambkid-0.0.8/docs/install.md
--rw-rw-rw-   0        0        0      769 2024-03-31 07:14:12.000000 lambkid-0.0.8/docs/log.md
--rw-rw-rw-   0        0        0     1878 2024-04-01 07:39:19.000000 lambkid-0.0.8/docs/sshclient.md
-drwxrwxrwx   0        0        0        0 2024-04-01 08:23:48.810950 lambkid-0.0.8/lambkid/
--rw-rw-rw-   0        0        0      113 2024-04-01 07:23:01.000000 lambkid-0.0.8/lambkid/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:23:48.819926 lambkid-0.0.8/lambkid/libs/
--rw-rw-rw-   0        0        0        0 2024-03-31 06:59:08.000000 lambkid-0.0.8/lambkid/libs/__init__.py
--rw-rw-rw-   0        0        0     1236 2024-03-31 17:42:20.000000 lambkid-0.0.8/lambkid/libs/log.py
--rw-rw-rw-   0        0        0     6613 2024-04-01 07:39:19.000000 lambkid-0.0.8/lambkid/libs/ssh.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:23:48.821921 lambkid-0.0.8/lambkid.egg-info/
--rw-rw-rw-   0        0        0     1630 2024-04-01 08:23:48.000000 lambkid-0.0.8/lambkid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-04-01 08:23:48.000000 lambkid-0.0.8/lambkid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 08:23:48.000000 lambkid-0.0.8/lambkid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-04-01 08:23:48.000000 lambkid-0.0.8/lambkid.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-01 08:23:48.000000 lambkid-0.0.8/lambkid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 08:23:48.824912 lambkid-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1722 2024-04-01 08:22:47.000000 lambkid-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 08:27:50.581574 lambkid-0.0.9/
+-rw-rw-rw-   0        0        0     1089 2024-03-27 01:13:02.000000 lambkid-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       27 2024-04-01 08:22:25.000000 lambkid-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1698 2024-04-01 08:27:50.580577 lambkid-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      386 2024-04-01 07:56:09.000000 lambkid-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 08:27:50.568610 lambkid-0.0.9/docs/
+-rw-rw-rw-   0        0        0       54 2024-03-31 06:58:42.000000 lambkid-0.0.9/docs/install.md
+-rw-rw-rw-   0        0        0      769 2024-03-31 07:14:12.000000 lambkid-0.0.9/docs/log.md
+-rw-rw-rw-   0        0        0     1878 2024-04-01 07:39:19.000000 lambkid-0.0.9/docs/sshclient.md
+drwxrwxrwx   0        0        0        0 2024-04-01 08:27:50.569607 lambkid-0.0.9/lambkid/
+-rw-rw-rw-   0        0        0      113 2024-04-01 07:23:01.000000 lambkid-0.0.9/lambkid/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 08:27:50.578583 lambkid-0.0.9/lambkid/libs/
+-rw-rw-rw-   0        0        0        0 2024-03-31 06:59:08.000000 lambkid-0.0.9/lambkid/libs/__init__.py
+-rw-rw-rw-   0        0        0     1236 2024-03-31 17:42:20.000000 lambkid-0.0.9/lambkid/libs/log.py
+-rw-rw-rw-   0        0        0     6613 2024-04-01 07:39:19.000000 lambkid-0.0.9/lambkid/libs/ssh.py
+drwxrwxrwx   0        0        0        0 2024-04-01 08:27:50.579604 lambkid-0.0.9/lambkid.egg-info/
+-rw-rw-rw-   0        0        0     1698 2024-04-01 08:27:50.000000 lambkid-0.0.9/lambkid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-04-01 08:27:50.000000 lambkid-0.0.9/lambkid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 08:27:50.000000 lambkid-0.0.9/lambkid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-04-01 08:27:50.000000 lambkid-0.0.9/lambkid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-01 08:27:50.000000 lambkid-0.0.9/lambkid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-01 08:27:50.581574 lambkid-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1817 2024-04-01 08:27:42.000000 lambkid-0.0.9/setup.py
```

### Comparing `lambkid-0.0.8/LICENSE` & `lambkid-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lambkid-0.0.8/PKG-INFO` & `lambkid-0.0.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: lambkid
-Version: 0.0.8
+Version: 0.0.9
 Summary: lambkid is an advance abstract from some common pyton lib, it aim to make you write python more easily and more fewer code.
 Home-page: https://github.com/redrose2100/lambkid
 Author: redrose2100
 Author-email: hitredrose@163.com
 Maintainer: redrose2100
 Maintainer-email: hitredrose@163.com
 License: MIT
+Project-URL: Documentation, https://github.com/redrose2100/lambkid
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: System :: Logging
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
```

### Comparing `lambkid-0.0.8/docs/log.md` & `lambkid-0.0.9/docs/log.md`

 * *Files identical despite different names*

### Comparing `lambkid-0.0.8/docs/sshclient.md` & `lambkid-0.0.9/docs/sshclient.md`

 * *Files identical despite different names*

### Comparing `lambkid-0.0.8/lambkid/libs/log.py` & `lambkid-0.0.9/lambkid/libs/log.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.0.8/lambkid/libs/ssh.py` & `lambkid-0.0.9/lambkid/libs/ssh.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.0.8/lambkid.egg-info/PKG-INFO` & `lambkid-0.0.9/lambkid.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: lambkid
-Version: 0.0.8
+Version: 0.0.9
 Summary: lambkid is an advance abstract from some common pyton lib, it aim to make you write python more easily and more fewer code.
 Home-page: https://github.com/redrose2100/lambkid
 Author: redrose2100
 Author-email: hitredrose@163.com
 Maintainer: redrose2100
 Maintainer-email: hitredrose@163.com
 License: MIT
+Project-URL: Documentation, https://github.com/redrose2100/lambkid
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: System :: Logging
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
```

### Comparing `lambkid-0.0.8/setup.py` & `lambkid-0.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,17 @@
     long_description=long_desc,
     long_description_content_type="text/markdown",
     author="redrose2100",
     author_email="hitredrose@163.com",
     maintainer="redrose2100",
     maintainer_email="hitredrose@163.com",
     url="https://github.com/redrose2100/lambkid",
+    project_urls={
+        "Documentation": "https://github.com/redrose2100/lambkid"
+    },
     license="MIT",
     install_requires =[
         "concurrent_log_handler",
         "paramiko"
     ],
     include_package_data=True,
     classifiers=[
```

