# Comparing `tmp/elicznik-2.0.0.tar.gz` & `tmp/elicznik-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elicznik-2.0.0.tar", last modified: Mon Nov 13 18:37:13 2023, max compression
+gzip compressed data, was "elicznik-2.1.0.tar", last modified: Tue Apr  2 19:40:44 2024, max compression
```

## Comparing `elicznik-2.0.0.tar` & `elicznik-2.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 mlesniew  (1000) mlesniew  (1000)        0 2023-11-13 18:37:13.778543 elicznik-2.0.0/
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)     1074 2023-11-09 15:22:01.000000 elicznik-2.0.0/LICENSE
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)     6529 2023-11-13 18:37:13.778543 elicznik-2.0.0/PKG-INFO
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)     5834 2023-11-12 17:25:18.000000 elicznik-2.0.0/README.md
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)       74 2023-11-13 18:37:13.778543 elicznik-2.0.0/setup.cfg
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)     1180 2023-11-13 18:33:27.000000 elicznik-2.0.0/setup.py
-drwxrwxr-x   0 mlesniew  (1000) mlesniew  (1000)        0 2023-11-13 18:37:13.774543 elicznik-2.0.0/src/
-drwxrwxr-x   0 mlesniew  (1000) mlesniew  (1000)        0 2023-11-13 18:37:13.778543 elicznik-2.0.0/src/elicznik/
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)       59 2023-11-09 15:22:01.000000 elicznik-2.0.0/src/elicznik/__init__.py
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)     2200 2023-11-12 17:21:18.000000 elicznik-2.0.0/src/elicznik/__main__.py
--rwxrwxr-x   0 mlesniew  (1000) mlesniew  (1000)     4774 2023-11-12 17:21:18.000000 elicznik-2.0.0/src/elicznik/elicznik.py
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)      774 2023-11-09 15:22:01.000000 elicznik-2.0.0/src/elicznik/session.py
-drwxrwxr-x   0 mlesniew  (1000) mlesniew  (1000)        0 2023-11-13 18:37:13.778543 elicznik-2.0.0/src/elicznik.egg-info/
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)     6529 2023-11-13 18:37:13.000000 elicznik-2.0.0/src/elicznik.egg-info/PKG-INFO
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)      353 2023-11-13 18:37:13.000000 elicznik-2.0.0/src/elicznik.egg-info/SOURCES.txt
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)        1 2023-11-13 18:37:13.000000 elicznik-2.0.0/src/elicznik.egg-info/dependency_links.txt
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)       52 2023-11-13 18:37:13.000000 elicznik-2.0.0/src/elicznik.egg-info/entry_points.txt
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)       18 2023-11-13 18:37:13.000000 elicznik-2.0.0/src/elicznik.egg-info/requires.txt
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)        9 2023-11-13 18:37:13.000000 elicznik-2.0.0/src/elicznik.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:40:44.667510 elicznik-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-02 19:40:38.000000 elicznik-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-04-02 19:40:44.667510 elicznik-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-04-02 19:40:38.000000 elicznik-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-02 19:40:44.671510 elicznik-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-02 19:40:38.000000 elicznik-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:40:44.667510 elicznik-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:40:44.667510 elicznik-2.1.0/src/elicznik/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-02 19:40:38.000000 elicznik-2.1.0/src/elicznik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-02 19:40:38.000000 elicznik-2.1.0/src/elicznik/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4774 2024-04-02 19:40:38.000000 elicznik-2.1.0/src/elicznik/elicznik.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-02 19:40:38.000000 elicznik-2.1.0/src/elicznik/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:40:44.667510 elicznik-2.1.0/src/elicznik.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-04-02 19:40:44.000000 elicznik-2.1.0/src/elicznik.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-02 19:40:44.000000 elicznik-2.1.0/src/elicznik.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:40:44.000000 elicznik-2.1.0/src/elicznik.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-02 19:40:44.000000 elicznik-2.1.0/src/elicznik.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 19:40:44.000000 elicznik-2.1.0/src/elicznik.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 19:40:44.000000 elicznik-2.1.0/src/elicznik.egg-info/top_level.txt
```

### Comparing `elicznik-2.0.0/LICENSE` & `elicznik-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `elicznik-2.0.0/PKG-INFO` & `elicznik-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elicznik
-Version: 2.0.0
+Version: 2.1.0
 Summary: Tauron eLicznik scrapper
 Home-page: https://github.com/mlesniew/elicznik
 Author: Michał Leśniewski
 Author-email: mlesniew@gmail.com
 Keywords: elicznik,tauron,scrapper
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -14,14 +14,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Internet
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: tabulate
 
 # Tauron eLicznik Scraper
 
 This Python 3 package allows to read electric energy meter reading history from the 
 [Tauron eLicznik](https://elicznik.tauron-dystrybucja.pl/) website.
```

### Comparing `elicznik-2.0.0/README.md` & `elicznik-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `elicznik-2.0.0/setup.py` & `elicznik-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='elicznik',
-    version='2.0.0',
+    version='2.1.0',
     description='Tauron eLicznik scrapper',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/mlesniew/elicznik',
     author='Michał Leśniewski',
     author_email='mlesniew@gmail.com',
     classifiers=[
```

### Comparing `elicznik-2.0.0/src/elicznik/__main__.py` & `elicznik-2.1.0/src/elicznik/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,13 +61,13 @@
                         "net consumption",
                         "net production",
                     ],
                 )
             )
         else:
             writer = csv.writer(sys.stdout)
-            for timestamp, consumed, produced in result:
-                writer.writerow((timestamp.isoformat(), consumed, produced))
+            for timestamp, consumed, produced, net_consumed, net_produced in result:
+                writer.writerow((timestamp.isoformat(), consumed, produced, net_consumed, net_produced))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `elicznik-2.0.0/src/elicznik/elicznik.py` & `elicznik-2.1.0/src/elicznik/elicznik.py`

 * *Files identical despite different names*

### Comparing `elicznik-2.0.0/src/elicznik.egg-info/PKG-INFO` & `elicznik-2.1.0/src/elicznik.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elicznik
-Version: 2.0.0
+Version: 2.1.0
 Summary: Tauron eLicznik scrapper
 Home-page: https://github.com/mlesniew/elicznik
 Author: Michał Leśniewski
 Author-email: mlesniew@gmail.com
 Keywords: elicznik,tauron,scrapper
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -14,14 +14,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Internet
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: tabulate
 
 # Tauron eLicznik Scraper
 
 This Python 3 package allows to read electric energy meter reading history from the 
 [Tauron eLicznik](https://elicznik.tauron-dystrybucja.pl/) website.
```

