# Comparing `tmp/olscrypto-0.1.6.tar.gz` & `tmp/olscrypto-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olscrypto-0.1.6.tar", last modified: Tue Apr  2 04:12:41 2024, max compression
+gzip compressed data, was "olscrypto-0.1.7.tar", last modified: Tue Apr  2 04:57:32 2024, max compression
```

## Comparing `olscrypto-0.1.6.tar` & `olscrypto-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 dirmich    (503) admin       (80)        0 2024-04-02 04:12:41.000000 olscrypto-0.1.6/
--rw-r--r--   0 dirmich    (503) admin       (80)      649 2024-04-02 04:12:41.000000 olscrypto-0.1.6/PKG-INFO
--rw-r--r--   0 dirmich    (503) admin       (80)      190 2024-02-13 05:01:01.000000 olscrypto-0.1.6/README.md
-drwxr-xr-x   0 dirmich    (503) admin       (80)        0 2024-04-02 04:12:41.000000 olscrypto-0.1.6/olscrypto/
--rw-r--r--   0 dirmich    (503) admin       (80)       41 2024-02-13 04:33:57.000000 olscrypto-0.1.6/olscrypto/__init__.py
--rw-r--r--   0 dirmich    (503) admin       (80)     1927 2024-04-02 03:48:52.000000 olscrypto-0.1.6/olscrypto/decryptor.py
-drwxr-xr-x   0 dirmich    (503) admin       (80)        0 2024-04-02 04:12:41.000000 olscrypto-0.1.6/olscrypto.egg-info/
--rw-r--r--   0 dirmich    (503) admin       (80)      649 2024-04-02 04:12:41.000000 olscrypto-0.1.6/olscrypto.egg-info/PKG-INFO
--rw-r--r--   0 dirmich    (503) admin       (80)      249 2024-04-02 04:12:41.000000 olscrypto-0.1.6/olscrypto.egg-info/SOURCES.txt
--rw-r--r--   0 dirmich    (503) admin       (80)        1 2024-04-02 04:12:41.000000 olscrypto-0.1.6/olscrypto.egg-info/dependency_links.txt
--rw-r--r--   0 dirmich    (503) admin       (80)        9 2024-04-02 04:12:41.000000 olscrypto-0.1.6/olscrypto.egg-info/requires.txt
--rw-r--r--   0 dirmich    (503) admin       (80)       10 2024-04-02 04:12:41.000000 olscrypto-0.1.6/olscrypto.egg-info/top_level.txt
--rw-r--r--   0 dirmich    (503) admin       (80)       38 2024-04-02 04:12:41.000000 olscrypto-0.1.6/setup.cfg
--rw-r--r--   0 dirmich    (503) admin       (80)      997 2024-04-02 04:12:38.000000 olscrypto-0.1.6/setup.py
-drwxr-xr-x   0 dirmich    (503) admin       (80)        0 2024-04-02 04:12:41.000000 olscrypto-0.1.6/tests/
--rw-r--r--   0 dirmich    (503) admin       (80)       32 2024-01-09 07:25:14.000000 olscrypto-0.1.6/tests/test_decrypt.py
+drwxr-xr-x   0 dirmich    (503) admin       (80)        0 2024-04-02 04:57:32.000000 olscrypto-0.1.7/
+-rw-r--r--   0 dirmich    (503) admin       (80)      649 2024-04-02 04:57:32.000000 olscrypto-0.1.7/PKG-INFO
+-rw-r--r--   0 dirmich    (503) admin       (80)      190 2024-02-13 05:01:01.000000 olscrypto-0.1.7/README.md
+drwxr-xr-x   0 dirmich    (503) admin       (80)        0 2024-04-02 04:57:32.000000 olscrypto-0.1.7/olscrypto/
+-rw-r--r--   0 dirmich    (503) admin       (80)       41 2024-02-13 04:33:57.000000 olscrypto-0.1.7/olscrypto/__init__.py
+-rw-r--r--   0 dirmich    (503) admin       (80)     1927 2024-04-02 03:48:52.000000 olscrypto-0.1.7/olscrypto/decryptor.py
+drwxr-xr-x   0 dirmich    (503) admin       (80)        0 2024-04-02 04:57:32.000000 olscrypto-0.1.7/olscrypto.egg-info/
+-rw-r--r--   0 dirmich    (503) admin       (80)      649 2024-04-02 04:57:31.000000 olscrypto-0.1.7/olscrypto.egg-info/PKG-INFO
+-rw-r--r--   0 dirmich    (503) admin       (80)      249 2024-04-02 04:57:31.000000 olscrypto-0.1.7/olscrypto.egg-info/SOURCES.txt
+-rw-r--r--   0 dirmich    (503) admin       (80)        1 2024-04-02 04:57:31.000000 olscrypto-0.1.7/olscrypto.egg-info/dependency_links.txt
+-rw-r--r--   0 dirmich    (503) admin       (80)       21 2024-04-02 04:57:31.000000 olscrypto-0.1.7/olscrypto.egg-info/requires.txt
+-rw-r--r--   0 dirmich    (503) admin       (80)       10 2024-04-02 04:57:31.000000 olscrypto-0.1.7/olscrypto.egg-info/top_level.txt
+-rw-r--r--   0 dirmich    (503) admin       (80)       38 2024-04-02 04:57:32.000000 olscrypto-0.1.7/setup.cfg
+-rw-r--r--   0 dirmich    (503) admin       (80)     1009 2024-04-02 04:56:00.000000 olscrypto-0.1.7/setup.py
+drwxr-xr-x   0 dirmich    (503) admin       (80)        0 2024-04-02 04:57:32.000000 olscrypto-0.1.7/tests/
+-rw-r--r--   0 dirmich    (503) admin       (80)       32 2024-01-09 07:25:14.000000 olscrypto-0.1.7/tests/test_decrypt.py
```

### Comparing `olscrypto-0.1.6/PKG-INFO` & `olscrypto-0.1.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olscrypto
-Version: 0.1.6
+Version: 0.1.7
 Summary: OLS decrypt library
 Author: Highmaru, Inc.
 Author-email: dhshin@highmaru.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `olscrypto-0.1.6/olscrypto/decryptor.py` & `olscrypto-0.1.7/olscrypto/decryptor.py`

 * *Files identical despite different names*

### Comparing `olscrypto-0.1.6/olscrypto.egg-info/PKG-INFO` & `olscrypto-0.1.7/olscrypto.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olscrypto
-Version: 0.1.6
+Version: 0.1.7
 Summary: OLS decrypt library
 Author: Highmaru, Inc.
 Author-email: dhshin@highmaru.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `olscrypto-0.1.6/setup.py` & `olscrypto-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 DESCRIPTION = 'OLS decrypt library'
 setup(
     name='olscrypto',
     packages=find_packages(include=['olscrypto']),
-    version='0.1.6',
+    version='0.1.7',
     author='Highmaru, Inc.',
     author_email="dhshin@highmaru.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     # setup_requires=['pytest-runner'],
     # tests_require=['pytest==4.4.1'],
     # test_suite='tests'
-    install_requires=['pycrypto'],
+    install_requires=['pycryptodome>=3.20.0'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
```

