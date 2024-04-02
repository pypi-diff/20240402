# Comparing `tmp/schwab-py-0.0.0a1.tar.gz` & `tmp/schwab-py-0.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schwab-py-0.0.0a1.tar", last modified: Wed Jan 11 13:55:33 2023, max compression
+gzip compressed data, was "schwab-py-0.0.0a2.tar", last modified: Tue Apr  2 04:23:50 2024, max compression
```

## Comparing `schwab-py-0.0.0a1.tar` & `schwab-py-0.0.0a2.tar`

### file list

```diff
@@ -1,15 +1,23 @@
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2023-01-11 13:55:33.513413 schwab-py-0.0.0a1/
--rw-r--r--   0 alexgolec   (501) staff       (20)     1067 2023-01-03 13:06:31.000000 schwab-py-0.0.0a1/LICENSE
--rw-r--r--   0 alexgolec   (501) staff       (20)     3093 2023-01-11 13:55:33.513483 schwab-py-0.0.0a1/PKG-INFO
--rw-r--r--   0 alexgolec   (501) staff       (20)     2075 2023-01-11 13:54:44.000000 schwab-py-0.0.0a1/README.rst
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2023-01-11 13:55:33.512749 schwab-py-0.0.0a1/schwab/
--rw-r--r--   0 alexgolec   (501) staff       (20)        0 2023-01-03 13:14:47.000000 schwab-py-0.0.0a1/schwab/__init__.py
--rw-r--r--   0 alexgolec   (501) staff       (20)       20 2023-01-11 13:55:04.000000 schwab-py-0.0.0a1/schwab/version.py
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2023-01-11 13:55:33.513312 schwab-py-0.0.0a1/schwab_py.egg-info/
--rw-r--r--   0 alexgolec   (501) staff       (20)     3093 2023-01-11 13:55:33.000000 schwab-py-0.0.0a1/schwab_py.egg-info/PKG-INFO
--rw-r--r--   0 alexgolec   (501) staff       (20)      238 2023-01-11 13:55:33.000000 schwab-py-0.0.0a1/schwab_py.egg-info/SOURCES.txt
--rw-r--r--   0 alexgolec   (501) staff       (20)        1 2023-01-11 13:55:33.000000 schwab-py-0.0.0a1/schwab_py.egg-info/dependency_links.txt
--rw-r--r--   0 alexgolec   (501) staff       (20)       13 2023-01-11 13:55:33.000000 schwab-py-0.0.0a1/schwab_py.egg-info/requires.txt
--rw-r--r--   0 alexgolec   (501) staff       (20)        7 2023-01-11 13:55:33.000000 schwab-py-0.0.0a1/schwab_py.egg-info/top_level.txt
--rw-r--r--   0 alexgolec   (501) staff       (20)      565 2023-01-11 13:55:33.513803 schwab-py-0.0.0a1/setup.cfg
--rw-r--r--   0 alexgolec   (501) staff       (20)     1533 2023-01-11 13:53:08.000000 schwab-py-0.0.0a1/setup.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-02 04:23:50.678370 schwab-py-0.0.0a2/
+-rw-r--r--   0 alexgolec   (501) staff       (20)     1067 2024-03-26 01:18:54.000000 schwab-py-0.0.0a2/LICENSE
+-rw-r--r--   0 alexgolec   (501) staff       (20)     3361 2024-04-02 04:23:50.678304 schwab-py-0.0.0a2/PKG-INFO
+-rw-r--r--   0 alexgolec   (501) staff       (20)     2075 2024-03-26 01:18:54.000000 schwab-py-0.0.0a2/README.rst
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-02 04:23:50.676721 schwab-py-0.0.0a2/schwab/
+-rw-r--r--   0 alexgolec   (501) staff       (20)        0 2024-04-01 11:30:18.000000 schwab-py-0.0.0a2/schwab/__init__.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    24222 2024-04-01 12:04:09.000000 schwab-py-0.0.0a2/schwab/auth.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-02 04:23:50.677182 schwab-py-0.0.0a2/schwab/client/
+-rw-r--r--   0 alexgolec   (501) staff       (20)       70 2024-04-01 12:04:09.000000 schwab-py-0.0.0a2/schwab/client/__init__.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     2619 2024-04-01 12:04:09.000000 schwab-py-0.0.0a2/schwab/client/asynchronous.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     4704 2024-04-01 12:04:09.000000 schwab-py-0.0.0a2/schwab/client/base.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     2474 2024-04-01 12:04:09.000000 schwab-py-0.0.0a2/schwab/client/synchronous.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     5481 2024-03-31 12:18:58.000000 schwab-py-0.0.0a2/schwab/debug.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     5097 2024-04-01 12:04:09.000000 schwab-py-0.0.0a2/schwab/utils.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)       20 2024-04-02 04:23:49.000000 schwab-py-0.0.0a2/schwab/version.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-02 04:23:50.677930 schwab-py-0.0.0a2/schwab_py.egg-info/
+-rw-r--r--   0 alexgolec   (501) staff       (20)     3361 2024-04-02 04:23:50.000000 schwab-py-0.0.0a2/schwab_py.egg-info/PKG-INFO
+-rw-r--r--   0 alexgolec   (501) staff       (20)      392 2024-04-02 04:23:50.000000 schwab-py-0.0.0a2/schwab_py.egg-info/SOURCES.txt
+-rw-r--r--   0 alexgolec   (501) staff       (20)        1 2024-04-02 04:23:50.000000 schwab-py-0.0.0a2/schwab_py.egg-info/dependency_links.txt
+-rw-r--r--   0 alexgolec   (501) staff       (20)       96 2024-04-02 04:23:50.000000 schwab-py-0.0.0a2/schwab_py.egg-info/requires.txt
+-rw-r--r--   0 alexgolec   (501) staff       (20)        7 2024-04-02 04:23:50.000000 schwab-py-0.0.0a2/schwab_py.egg-info/top_level.txt
+-rw-r--r--   0 alexgolec   (501) staff       (20)      565 2024-04-02 04:23:50.678688 schwab-py-0.0.0a2/setup.cfg
+-rw-r--r--   0 alexgolec   (501) staff       (20)     1721 2024-04-02 04:18:54.000000 schwab-py-0.0.0a2/setup.py
```

### Comparing `schwab-py-0.0.0a1/LICENSE` & `schwab-py-0.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a1/PKG-INFO` & `schwab-py-0.0.0a2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 Metadata-Version: 2.1
 Name: schwab-py
-Version: 0.0.0a1
-Summary: Unofficial API wrapper for the upcoming Schwab REST API
+Version: 0.0.0a2
+Summary: Unofficial API wrapper for the upcoming Schwab HTTP API
 Home-page: https://github.com/alexgolec/schwab
 Author: Alex Golec
 Author-email: bottomless.septic.tank@gmail.com
 License: MIT
 Project-URL: Documentation, https://schwab-api.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/alexgolec/schwab-api
 Project-URL: Tracker, https://github.com/alexgolec/schwab-api/issues
 Keywords: finance trading equities bonds options research
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 1 - Planning
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Office/Business :: Financial :: Investment
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: authlib
+Requires-Dist: httpx
+Requires-Dist: prompt_toolkit
+Requires-Dist: python-dateutil
+Requires-Dist: selenium
+Provides-Extra: dev
+Requires-Dist: nose; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: sphinx_rtd_theme; extra == "dev"
+Requires-Dist: twine; extra == "dev"
 
 ``schwab-py``: A Schwab API Wrapper
 ========================================
 
 .. image:: https://img.shields.io/discord/720378361880248621.svg?label=&logo=discord&logoColor=ffffff&color=7389D8&labelColor=6A7EC2
   :target: https://discord.gg/BEr6y6Xqyv
 
@@ -66,9 +74,7 @@
 
 **Disclaimer:** *schwab-api is an unofficial API wrapper. It is in no way 
 endorsed by or affiliated with TD Ameritrade, Charles Schwab or any associated 
 organization. Make sure to read and understand the terms of service of the 
 underlying API before using this package. The authors accept no responsibility 
 for any damage that might stem from use of this package. See the LICENSE file 
 for more details.*
-
-
```

### Comparing `schwab-py-0.0.0a1/README.rst` & `schwab-py-0.0.0a2/README.rst`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a1/schwab_py.egg-info/PKG-INFO` & `schwab-py-0.0.0a2/schwab_py.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 Metadata-Version: 2.1
 Name: schwab-py
-Version: 0.0.0a1
-Summary: Unofficial API wrapper for the upcoming Schwab REST API
+Version: 0.0.0a2
+Summary: Unofficial API wrapper for the upcoming Schwab HTTP API
 Home-page: https://github.com/alexgolec/schwab
 Author: Alex Golec
 Author-email: bottomless.septic.tank@gmail.com
 License: MIT
 Project-URL: Documentation, https://schwab-api.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/alexgolec/schwab-api
 Project-URL: Tracker, https://github.com/alexgolec/schwab-api/issues
 Keywords: finance trading equities bonds options research
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 1 - Planning
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Office/Business :: Financial :: Investment
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: authlib
+Requires-Dist: httpx
+Requires-Dist: prompt_toolkit
+Requires-Dist: python-dateutil
+Requires-Dist: selenium
+Provides-Extra: dev
+Requires-Dist: nose; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: sphinx_rtd_theme; extra == "dev"
+Requires-Dist: twine; extra == "dev"
 
 ``schwab-py``: A Schwab API Wrapper
 ========================================
 
 .. image:: https://img.shields.io/discord/720378361880248621.svg?label=&logo=discord&logoColor=ffffff&color=7389D8&labelColor=6A7EC2
   :target: https://discord.gg/BEr6y6Xqyv
 
@@ -66,9 +74,7 @@
 
 **Disclaimer:** *schwab-api is an unofficial API wrapper. It is in no way 
 endorsed by or affiliated with TD Ameritrade, Charles Schwab or any associated 
 organization. Make sure to read and understand the terms of service of the 
 underlying API before using this package. The authors accept no responsibility 
 for any damage that might stem from use of this package. See the LICENSE file 
 for more details.*
-
-
```

### Comparing `schwab-py-0.0.0a1/setup.cfg` & `schwab-py-0.0.0a2/setup.cfg`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a1/setup.py` & `schwab-py-0.0.0a2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,33 +9,42 @@
     version = version[1:-1]
 
 setuptools.setup(
     name='schwab-py',
     version=version,
     author='Alex Golec',
     author_email='bottomless.septic.tank@gmail.com',
-    description='Unofficial API wrapper for the upcoming Schwab REST API',
+    description='Unofficial API wrapper for the upcoming Schwab HTTP API',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     url='https://github.com/alexgolec/schwab',
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Intended Audience :: Developers',
         'Development Status :: 1 - Planning',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Topic :: Office/Business :: Financial :: Investment',
     ],
-    python_requires='>=3.7',
-    install_requires=[],
+    python_requires='>=3.8',
+    install_requires=[
+        'authlib',
+        'httpx',
+        'prompt_toolkit',
+        'python-dateutil',
+        'selenium',
+    ],
     extras_require={
         'dev': [
+            'nose',
+            'pytest',
+            'sphinx_rtd_theme',
             'twine',
         ]
     },
     keywords='finance trading equities bonds options research',
     project_urls={
         'Documentation': 'https://schwab-api.readthedocs.io/en/latest/',
         'Source': 'https://github.com/alexgolec/schwab-api',
```

