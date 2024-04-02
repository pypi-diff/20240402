# Comparing `tmp/zen-test-0.0.1.tar.gz` & `tmp/zen-test-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zen-test-0.0.1.tar", last modified: Tue Apr  2 09:10:01 2024, max compression
+gzip compressed data, was "zen-test-0.0.2.tar", last modified: Tue Apr  2 09:17:10 2024, max compression
```

## Comparing `zen-test-0.0.1.tar` & `zen-test-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 09:10:01.113701 zen-test-0.0.1/
--rw-rw-rw-   0        0        0      230 2024-04-02 09:10:01.112521 zen-test-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-02 09:10:01.114219 zen-test-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      558 2024-04-02 09:09:14.000000 zen-test-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 09:10:01.111583 zen-test-0.0.1/zen_test.egg-info/
--rw-rw-rw-   0        0        0      230 2024-04-02 09:10:00.000000 zen-test-0.0.1/zen_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      171 2024-04-02 09:10:01.000000 zen-test-0.0.1/zen_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 09:10:00.000000 zen-test-0.0.1/zen_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-04-02 09:10:01.000000 zen-test-0.0.1/zen_test.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 09:10:01.000000 zen-test-0.0.1/zen_test.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 09:17:10.179598 zen-test-0.0.2/
+-rw-rw-rw-   0        0        0      230 2024-04-02 09:17:10.179355 zen-test-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-02 09:17:10.180266 zen-test-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      559 2024-04-02 09:16:53.000000 zen-test-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 09:17:10.177608 zen-test-0.0.2/zen_test.egg-info/
+-rw-rw-rw-   0        0        0      230 2024-04-02 09:17:10.000000 zen-test-0.0.2/zen_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      171 2024-04-02 09:17:10.000000 zen-test-0.0.2/zen_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 09:17:10.000000 zen-test-0.0.2/zen_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-04-02 09:17:10.000000 zen-test-0.0.2/zen_test.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 09:17:10.000000 zen-test-0.0.2/zen_test.egg-info/top_level.txt
```

### Comparing `zen-test-0.0.1/setup.py` & `zen-test-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup
 
 setup(
     name='zen-test',
-    version='0.0.1',
+    version='0.0.2',
     packages=[],
     install_requires=[],
     entry_points={
         'console_scripts': [
-            'hello = zentest.hello:main'
+            'hello = zen_test.hello:main'
         ],
     },
     author='Zen',
     author_email='mathias.bochet.job@gmail.com',
     description='Test Package',
     long_description='A package to test the pypy packages systems.',
     url='https://github.com/42zen/hello_zen'
```

