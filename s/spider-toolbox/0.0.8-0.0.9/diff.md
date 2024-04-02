# Comparing `tmp/spider_toolbox-0.0.8.tar.gz` & `tmp/spider_toolbox-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spider_toolbox-0.0.8.tar", last modified: Sat Sep 16 12:58:32 2023, max compression
+gzip compressed data, was "spider_toolbox-0.0.9.tar", last modified: Sun Sep 17 04:06:12 2023, max compression
```

## Comparing `spider_toolbox-0.0.8.tar` & `spider_toolbox-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-09-16 12:58:32.291212 spider_toolbox-0.0.8/
--rw-rw-rw-   0        0        0     1085 2023-08-04 07:53:17.000000 spider_toolbox-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      503 2023-09-16 12:58:32.281705 spider_toolbox-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       66 2023-09-05 09:56:57.000000 spider_toolbox-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-09-16 12:58:32.292213 spider_toolbox-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      783 2023-09-16 12:58:27.000000 spider_toolbox-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-09-16 12:58:32.274705 spider_toolbox-0.0.8/spider_toolbox.egg-info/
--rw-rw-rw-   0        0        0      503 2023-09-16 12:58:32.000000 spider_toolbox-0.0.8/spider_toolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-09-16 12:58:32.000000 spider_toolbox-0.0.8/spider_toolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-16 12:58:32.000000 spider_toolbox-0.0.8/spider_toolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-09-16 12:58:32.000000 spider_toolbox-0.0.8/spider_toolbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-09-16 12:58:32.000000 spider_toolbox-0.0.8/spider_toolbox.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-09-16 12:58:32.279706 spider_toolbox-0.0.8/src/
--rw-rw-rw-   0        0        0     1906 2023-09-10 04:14:04.000000 spider_toolbox-0.0.8/src/decrypt_tools.py
--rw-rw-rw-   0        0        0     2019 2023-09-05 09:56:12.000000 spider_toolbox-0.0.8/src/file_tools.py
--rw-rw-rw-   0        0        0     1416 2023-09-16 12:58:06.000000 spider_toolbox-0.0.8/src/requests_tools.py
+drwxrwxrwx   0        0        0        0 2023-09-17 04:06:12.384457 spider_toolbox-0.0.9/
+-rw-rw-rw-   0        0        0     1085 2023-08-04 07:53:17.000000 spider_toolbox-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      503 2023-09-17 04:06:12.383480 spider_toolbox-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       66 2023-09-05 09:56:57.000000 spider_toolbox-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-09-17 04:06:12.384457 spider_toolbox-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      783 2023-09-17 04:05:56.000000 spider_toolbox-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-09-17 04:06:12.375669 spider_toolbox-0.0.9/spider_toolbox.egg-info/
+-rw-rw-rw-   0        0        0      503 2023-09-17 04:06:12.000000 spider_toolbox-0.0.9/spider_toolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-09-17 04:06:12.000000 spider_toolbox-0.0.9/spider_toolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-09-17 04:06:12.000000 spider_toolbox-0.0.9/spider_toolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-09-17 04:06:12.000000 spider_toolbox-0.0.9/spider_toolbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-09-17 04:06:12.000000 spider_toolbox-0.0.9/spider_toolbox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-09-17 04:06:12.381528 spider_toolbox-0.0.9/src/
+-rw-rw-rw-   0        0        0     1906 2023-09-10 04:14:04.000000 spider_toolbox-0.0.9/src/decrypt_tools.py
+-rw-rw-rw-   0        0        0     2019 2023-09-05 09:56:12.000000 spider_toolbox-0.0.9/src/file_tools.py
+-rw-rw-rw-   0        0        0     1789 2023-09-17 04:05:42.000000 spider_toolbox-0.0.9/src/requests_tools.py
```

### Comparing `spider_toolbox-0.0.8/LICENSE` & `spider_toolbox-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spider_toolbox-0.0.8/setup.py` & `spider_toolbox-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open('README.md', mode='r', encoding='utf-8') as f:
     long_description = f.read()
 setup(
     name='spider_toolbox',
-    version='0.0.8',
+    version='0.0.9',
     author='neco_arc',
     author_email='3306601284@qq.com',
     description='爬虫工具库',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/sweetnotice/spider_toolbox',
     classifiers=[
```

### Comparing `spider_toolbox-0.0.8/src/decrypt_tools.py` & `spider_toolbox-0.0.9/src/decrypt_tools.py`

 * *Files identical despite different names*

### Comparing `spider_toolbox-0.0.8/src/file_tools.py` & `spider_toolbox-0.0.9/src/file_tools.py`

 * *Files identical despite different names*

