# Comparing `tmp/marioutils-0.0.2.tar.gz` & `tmp/marioutils-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marioutils-0.0.2.tar", last modified: Fri Mar 29 19:50:19 2024, max compression
+gzip compressed data, was "marioutils-1.0.1.tar", last modified: Tue Apr  2 01:49:09 2024, max compression
```

## Comparing `marioutils-0.0.2.tar` & `marioutils-1.0.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 19:50:19.891576 marioutils-0.0.2/
--rw-rw-rw-   0        0        0     1088 2024-03-29 19:37:30.000000 marioutils-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      970 2024-03-29 19:50:19.890600 marioutils-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-29 19:50:19.367625 marioutils-0.0.2/mario_utils/
--rw-rw-rw-   0        0        0        0 2024-03-29 19:37:30.000000 marioutils-0.0.2/mario_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-29 19:50:19.369215 marioutils-0.0.2/mario_utils/databasemanagement/
--rw-rw-rw-   0        0        0       45 2024-03-29 19:37:30.000000 marioutils-0.0.2/mario_utils/databasemanagement/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-29 19:50:19.475461 marioutils-0.0.2/mario_utils/databasemanagement/src/
--rw-rw-rw-   0        0        0       49 2024-03-29 19:37:30.000000 marioutils-0.0.2/mario_utils/databasemanagement/src/__init__.py
--rw-rw-rw-   0        0        0     1360 2024-03-29 19:37:30.000000 marioutils-0.0.2/mario_utils/databasemanagement/src/exceptions.py
--rw-rw-rw-   0        0        0     5073 2024-03-29 19:37:30.000000 marioutils-0.0.2/mario_utils/databasemanagement/src/manager.py
-drwxrwxrwx   0        0        0        0 2024-03-29 19:50:19.477950 marioutils-0.0.2/mario_utils/databasemanagement/tests/
--rw-rw-rw-   0        0        0        0 2024-03-29 19:37:30.000000 marioutils-0.0.2/mario_utils/databasemanagement/tests/__init__.py
--rw-rw-rw-   0        0        0     1720 2024-03-29 19:37:30.000000 marioutils-0.0.2/mario_utils/databasemanagement/tests/test_.py
-drwxrwxrwx   0        0        0        0 2024-03-29 19:50:19.478927 marioutils-0.0.2/mario_utils/logger/
--rw-rw-rw-   0        0        0       34 2024-03-29 19:37:30.000000 marioutils-0.0.2/mario_utils/logger/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-29 19:50:19.589152 marioutils-0.0.2/mario_utils/logger/src/
--rw-rw-rw-   0        0        0       37 2024-03-29 19:37:30.000000 marioutils-0.0.2/mario_utils/logger/src/__init__.py
--rw-rw-rw-   0        0        0     1042 2024-03-29 19:37:30.000000 marioutils-0.0.2/mario_utils/logger/src/logger.py
-drwxrwxrwx   0        0        0        0 2024-03-29 19:50:19.592616 marioutils-0.0.2/mario_utils/logger/test/
--rw-rw-rw-   0        0        0        0 2024-03-29 19:37:30.000000 marioutils-0.0.2/mario_utils/logger/test/__init__.py
--rw-rw-rw-   0        0        0      555 2024-03-29 19:37:30.000000 marioutils-0.0.2/mario_utils/logger/test/test_logger.py
-drwxrwxrwx   0        0        0        0 2024-03-29 19:50:19.848426 marioutils-0.0.2/marioutils.egg-info/
--rw-rw-rw-   0        0        0      970 2024-03-29 19:50:19.000000 marioutils-0.0.2/marioutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      667 2024-03-29 19:50:19.000000 marioutils-0.0.2/marioutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 19:50:19.000000 marioutils-0.0.2/marioutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2024-03-29 19:50:19.000000 marioutils-0.0.2/marioutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-29 19:50:19.000000 marioutils-0.0.2/marioutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-29 19:50:19.892555 marioutils-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1076 2024-03-29 19:50:07.000000 marioutils-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 01:49:09.551270 marioutils-1.0.1/
+-rw-rw-rw-   0        0        0     1088 2024-03-29 19:37:30.000000 marioutils-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      925 2024-04-02 01:49:09.550272 marioutils-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-02 01:49:09.085092 marioutils-1.0.1/mario_utils/
+-rw-rw-rw-   0        0        0      166 2024-04-02 00:21:18.000000 marioutils-1.0.1/mario_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 01:49:09.123092 marioutils-1.0.1/mario_utils/databasemanagement/
+-rw-rw-rw-   0        0        0       93 2024-04-02 00:18:26.000000 marioutils-1.0.1/mario_utils/databasemanagement/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 01:49:09.192803 marioutils-1.0.1/mario_utils/databasemanagement/src/
+-rw-rw-rw-   0        0        0       99 2024-04-01 21:45:12.000000 marioutils-1.0.1/mario_utils/databasemanagement/src/__init__.py
+-rw-rw-rw-   0        0        0     1360 2024-03-29 19:37:30.000000 marioutils-1.0.1/mario_utils/databasemanagement/src/exceptions.py
+-rw-rw-rw-   0        0        0     5073 2024-03-29 19:37:30.000000 marioutils-1.0.1/mario_utils/databasemanagement/src/manager.py
+drwxrwxrwx   0        0        0        0 2024-04-02 01:49:09.195805 marioutils-1.0.1/mario_utils/databasemanagement/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-29 19:37:30.000000 marioutils-1.0.1/mario_utils/databasemanagement/tests/__init__.py
+-rw-rw-rw-   0        0        0     1982 2024-04-02 00:43:58.000000 marioutils-1.0.1/mario_utils/databasemanagement/tests/test_.py
+drwxrwxrwx   0        0        0        0 2024-04-02 01:49:09.197804 marioutils-1.0.1/mario_utils/logger/
+-rw-rw-rw-   0        0        0       67 2024-04-01 21:49:53.000000 marioutils-1.0.1/mario_utils/logger/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 01:49:09.291620 marioutils-1.0.1/mario_utils/logger/src/
+-rw-rw-rw-   0        0        0       70 2024-04-01 21:48:54.000000 marioutils-1.0.1/mario_utils/logger/src/__init__.py
+-rw-rw-rw-   0        0        0      982 2024-04-02 00:23:57.000000 marioutils-1.0.1/mario_utils/logger/src/logger.py
+drwxrwxrwx   0        0        0        0 2024-04-02 01:49:09.293621 marioutils-1.0.1/mario_utils/logger/test/
+-rw-rw-rw-   0        0        0        0 2024-03-29 19:37:30.000000 marioutils-1.0.1/mario_utils/logger/test/__init__.py
+-rw-rw-rw-   0        0        0      572 2024-04-02 00:22:14.000000 marioutils-1.0.1/mario_utils/logger/test/test_logger.py
+drwxrwxrwx   0        0        0        0 2024-04-02 01:49:09.517272 marioutils-1.0.1/marioutils.egg-info/
+-rw-rw-rw-   0        0        0      925 2024-04-02 01:49:08.000000 marioutils-1.0.1/marioutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      667 2024-04-02 01:49:09.000000 marioutils-1.0.1/marioutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 01:49:08.000000 marioutils-1.0.1/marioutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-04-02 01:49:08.000000 marioutils-1.0.1/marioutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-02 01:49:08.000000 marioutils-1.0.1/marioutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 01:49:09.552272 marioutils-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1023 2024-04-02 01:49:04.000000 marioutils-1.0.1/setup.py
```

### Comparing `marioutils-0.0.2/LICENSE.txt` & `marioutils-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `marioutils-0.0.2/PKG-INFO` & `marioutils-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marioutils
-Version: 0.0.2
+Version: 1.0.1
 Summary: Utils library for DB connection and logging
 Home-page: https://github.com/MarioHdzCtu/MarioUtils
 Author: Mario Hernandez
 Author-email: mariohertu@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
@@ -13,15 +13,14 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pymssql>=2.2.11
 Requires-Dist: sqlalchemy>=2.0.25
 Requires-Dist: mariadb>=1.1.10
 Provides-Extra: dev
 Requires-Dist: pytest>=8.0.0; extra == "dev"
-Requires-Dist: twine>=4.0.2; extra == "dev"
 
 
 # Mario Utils
 
 This project is used as a Python library for managing database connections (Now just supporting SQLServer over pymssql) and Logging for future scripts, avoiding boilerplate code.
```

### Comparing `marioutils-0.0.2/mario_utils/databasemanagement/src/exceptions.py` & `marioutils-1.0.1/mario_utils/databasemanagement/src/exceptions.py`

 * *Files identical despite different names*

### Comparing `marioutils-0.0.2/mario_utils/databasemanagement/src/manager.py` & `marioutils-1.0.1/mario_utils/databasemanagement/src/manager.py`

 * *Files identical despite different names*

### Comparing `marioutils-0.0.2/mario_utils/logger/src/logger.py` & `marioutils-1.0.1/mario_utils/logger/src/logger.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 import logging
 from logging import FileHandler
 from enum import Enum
 
+
 class Levels(Enum):
     CRITICAL = 50
     FATAL = CRITICAL
     ERROR = 40
     WARNING = 30
     WARN = WARNING
     INFO = 20
     DEBUG = 10
     NOTSET = 0
 
-def my_logger(name: str = 'basic', level: int | str = Levels.DEBUG.value):
 
-    logging.basicConfig(level=level)
+def logger(name: str = 'basic', level: Levels = Levels.DEBUG):
+
+    logging.basicConfig(level=level.value)
 
     logger = logging.getLogger(name)
-    logger.setLevel(level)
+    logger.setLevel(level.value)
 
     handler = FileHandler(
-        filename= name,
+        filename=name,
         mode='a',
         encoding='UTF-8'
     )
-    handler.setLevel(level)
+    handler.setLevel(level.value)
     formatter = logging.Formatter(
         fmt='%(levelname)s - %(asctime)s - %(message)s',
         datefmt="%Y-%m-%d %H:%M:%S"
     )
     handler.setFormatter(formatter)
 
     logger.addHandler(handler)
 
     return logger
 
+
 if __name__ == '__main__':
-    logger = my_logger(name='test.log')
+    logger = logger(name='test.log')
     logger.debug('Debug')
     logger.info('Info')
     logger.warning('Warning')
     logger.critical('Prueba')
-
-    # with open('basic.log', 'r') as f:
-    #     print(f.read())
```

### Comparing `marioutils-0.0.2/marioutils.egg-info/PKG-INFO` & `marioutils-1.0.1/marioutils.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marioutils
-Version: 0.0.2
+Version: 1.0.1
 Summary: Utils library for DB connection and logging
 Home-page: https://github.com/MarioHdzCtu/MarioUtils
 Author: Mario Hernandez
 Author-email: mariohertu@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
@@ -13,15 +13,14 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pymssql>=2.2.11
 Requires-Dist: sqlalchemy>=2.0.25
 Requires-Dist: mariadb>=1.1.10
 Provides-Extra: dev
 Requires-Dist: pytest>=8.0.0; extra == "dev"
-Requires-Dist: twine>=4.0.2; extra == "dev"
 
 
 # Mario Utils
 
 This project is used as a Python library for managing database connections (Now just supporting SQLServer over pymssql) and Logging for future scripts, avoiding boilerplate code.
```

### Comparing `marioutils-0.0.2/marioutils.egg-info/SOURCES.txt` & `marioutils-1.0.1/marioutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `marioutils-0.0.2/setup.py` & `marioutils-1.0.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
-with open("./mario_utils/README.md", 'r') as f:
+with open("mario_utils\README.md", 'r') as f:
     long_description = f.read()
 
 setup(
     name="marioutils",
-    version="0.0.2",
+    version="1.0.1",
     description="Utils library for DB connection and logging",
     packages=find_packages(),
     package_data={'mario_utils':['databasemanagement/*'],'mario_utils':['logger/*']},
     include_package_data=True,
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MarioHdzCtu/MarioUtils",
@@ -17,18 +17,14 @@
     author_email="mariohertu@gmail.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent"
     ],
-    install_requires=[
-        "pymssql >= 2.2.11",
-        "sqlalchemy >= 2.0.25",
-        "mariadb >= 1.1.10"
-    ],
+    install_requires=["pymssql >= 2.2.11", "sqlalchemy >= 2.0.25", "mariadb >= 1.1.10"],
     extras_require={
-        "dev": ["pytest>=8.0.0", "twine >=4.0.2"]
+        "dev": ["pytest>=8.0.0"]
     },
     python_requires=">=3.10.12",
     include_dirs=True
 )
```

