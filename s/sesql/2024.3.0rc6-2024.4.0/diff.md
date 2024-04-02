# Comparing `tmp/sesql-2024.3.0rc6.tar.gz` & `tmp/sesql-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sesql-2024.3.0rc6.tar", last modified: Mon Apr  1 02:01:07 2024, max compression
+gzip compressed data, was "sesql-2024.4.0.tar", last modified: Tue Apr  2 00:44:56 2024, max compression
```

## Comparing `sesql-2024.3.0rc6.tar` & `sesql-2024.4.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-04-01 02:01:07.800062 sesql-2024.3.0rc6/
--rw-r--r--   0 rjd        (501) staff       (20)     1078 2023-12-26 02:50:39.000000 sesql-2024.3.0rc6/License.md
--rw-r--r--   0 rjd        (501) staff       (20)     1718 2024-04-01 02:01:07.799849 sesql-2024.3.0rc6/PKG-INFO
--rw-r--r--   0 rjd        (501) staff       (20)       55 2024-03-02 03:37:34.000000 sesql-2024.3.0rc6/ReadMe.md
--rw-r--r--   0 rjd        (501) staff       (20)      808 2024-03-31 00:07:50.000000 sesql-2024.3.0rc6/pyproject.toml
-drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-04-01 02:01:07.794081 sesql-2024.3.0rc6/seCore/
--rw-r--r--   0 rjd        (501) staff       (20)      839 2024-03-30 23:03:58.000000 sesql-2024.3.0rc6/seCore/CustomLogging.py
--rw-r--r--   0 rjd        (501) staff       (20)        0 2024-03-17 19:54:29.000000 sesql-2024.3.0rc6/seCore/__init__.py
-drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-04-01 02:01:07.794377 sesql-2024.3.0rc6/seSql/
--rw-r--r--   0 rjd        (501) staff       (20)      204 2024-03-30 23:33:30.000000 sesql-2024.3.0rc6/seSql/__init__.py
--rw-r--r--   0 rjd        (501) staff       (20)      316 2024-04-01 02:01:05.000000 sesql-2024.3.0rc6/seSql/_version.py
-drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-04-01 02:01:07.795134 sesql-2024.3.0rc6/seSql/dbc/
--rw-r--r--   0 rjd        (501) staff       (20)     2383 2024-03-03 23:41:30.000000 sesql-2024.3.0rc6/seSql/dbc/Exceptions.py
--rw-r--r--   0 rjd        (501) staff       (20)     7393 2024-04-01 01:51:00.000000 sesql-2024.3.0rc6/seSql/dbc/JDBC.py
--rw-r--r--   0 rjd        (501) staff       (20)     6868 2024-04-01 01:54:33.000000 sesql-2024.3.0rc6/seSql/dbc/ODBC.py
--rw-r--r--   0 rjd        (501) staff       (20)     5936 2024-02-29 01:59:07.000000 sesql-2024.3.0rc6/seSql/dbc/ODBCError.py
--rw-r--r--   0 rjd        (501) staff       (20)      726 2024-04-01 01:40:37.000000 sesql-2024.3.0rc6/seSql/dbc/Utilities.py
--rw-r--r--   0 rjd        (501) staff       (20)        0 2024-03-17 19:54:29.000000 sesql-2024.3.0rc6/seSql/dbc/__init__.py
-drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-04-01 02:01:07.795242 sesql-2024.3.0rc6/seSql/dbc/jars/
--rw-r--r--   0 rjd        (501) staff       (20)  1438398 2024-03-01 01:47:02.000000 sesql-2024.3.0rc6/seSql/dbc/jars/mssql-jdbc-12.4.2.jre8.jar
--rw-r--r--   0 rjd        (501) staff       (20)     3712 2024-04-01 01:46:48.000000 sesql-2024.3.0rc6/seSql/sql.py
-drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-04-01 02:01:07.799618 sesql-2024.3.0rc6/sesql.egg-info/
--rw-r--r--   0 rjd        (501) staff       (20)     1718 2024-04-01 02:01:07.000000 sesql-2024.3.0rc6/sesql.egg-info/PKG-INFO
--rw-r--r--   0 rjd        (501) staff       (20)      556 2024-04-01 02:01:07.000000 sesql-2024.3.0rc6/sesql.egg-info/SOURCES.txt
--rw-r--r--   0 rjd        (501) staff       (20)        1 2024-04-01 02:01:07.000000 sesql-2024.3.0rc6/sesql.egg-info/dependency_links.txt
--rw-r--r--   0 rjd        (501) staff       (20)       56 2024-04-01 02:01:07.000000 sesql-2024.3.0rc6/sesql.egg-info/requires.txt
--rw-r--r--   0 rjd        (501) staff       (20)       13 2024-04-01 02:01:07.000000 sesql-2024.3.0rc6/sesql.egg-info/top_level.txt
--rw-r--r--   0 rjd        (501) staff       (20)       38 2024-04-01 02:01:07.800102 sesql-2024.3.0rc6/setup.cfg
-drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-04-01 02:01:07.799436 sesql-2024.3.0rc6/tests/
--rw-r--r--   0 rjd        (501) staff       (20)     1790 2024-03-31 01:39:23.000000 sesql-2024.3.0rc6/tests/test_Exceptions.py
--rw-r--r--   0 rjd        (501) staff       (20)      222 2024-03-31 23:51:30.000000 sesql-2024.3.0rc6/tests/test_customlogging.py
--rw-r--r--   0 rjd        (501) staff       (20)      987 2024-04-01 01:44:20.000000 sesql-2024.3.0rc6/tests/test_jdbc.py
--rw-r--r--   0 rjd        (501) staff       (20)      690 2024-04-01 01:35:26.000000 sesql-2024.3.0rc6/tests/test_odbc.py
--rw-r--r--   0 rjd        (501) staff       (20)      238 2024-04-01 01:39:41.000000 sesql-2024.3.0rc6/tests/test_utilities.py
+drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-04-02 00:44:56.075851 sesql-2024.4.0/
+-rw-r--r--   0 rjd        (501) staff       (20)     1078 2023-12-26 02:50:39.000000 sesql-2024.4.0/License.md
+-rw-r--r--   0 rjd        (501) staff       (20)     5894 2024-04-02 00:44:56.075651 sesql-2024.4.0/PKG-INFO
+-rw-r--r--   0 rjd        (501) staff       (20)     4234 2024-04-02 00:43:29.000000 sesql-2024.4.0/ReadMe.md
+-rw-r--r--   0 rjd        (501) staff       (20)      808 2024-03-31 00:07:50.000000 sesql-2024.4.0/pyproject.toml
+drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-04-02 00:44:56.069751 sesql-2024.4.0/seCore/
+-rw-r--r--   0 rjd        (501) staff       (20)      839 2024-03-30 23:03:58.000000 sesql-2024.4.0/seCore/CustomLogging.py
+-rw-r--r--   0 rjd        (501) staff       (20)        0 2024-03-17 19:54:29.000000 sesql-2024.4.0/seCore/__init__.py
+drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-04-02 00:44:56.070060 sesql-2024.4.0/seSql/
+-rw-r--r--   0 rjd        (501) staff       (20)      280 2024-04-01 23:44:41.000000 sesql-2024.4.0/seSql/__init__.py
+-rw-r--r--   0 rjd        (501) staff       (20)      295 2024-04-02 00:44:53.000000 sesql-2024.4.0/seSql/_version.py
+drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-04-02 00:44:56.070832 sesql-2024.4.0/seSql/dbc/
+-rw-r--r--   0 rjd        (501) staff       (20)     2383 2024-03-03 23:41:30.000000 sesql-2024.4.0/seSql/dbc/Exceptions.py
+-rw-r--r--   0 rjd        (501) staff       (20)     7393 2024-04-01 01:51:00.000000 sesql-2024.4.0/seSql/dbc/JDBC.py
+-rw-r--r--   0 rjd        (501) staff       (20)     6868 2024-04-01 01:54:33.000000 sesql-2024.4.0/seSql/dbc/ODBC.py
+-rw-r--r--   0 rjd        (501) staff       (20)     5936 2024-02-29 01:59:07.000000 sesql-2024.4.0/seSql/dbc/ODBCError.py
+-rw-r--r--   0 rjd        (501) staff       (20)      726 2024-04-01 01:40:37.000000 sesql-2024.4.0/seSql/dbc/Utilities.py
+-rw-r--r--   0 rjd        (501) staff       (20)        0 2024-03-17 19:54:29.000000 sesql-2024.4.0/seSql/dbc/__init__.py
+drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-04-02 00:44:56.070927 sesql-2024.4.0/seSql/dbc/jars/
+-rw-r--r--   0 rjd        (501) staff       (20)  1438398 2024-03-01 01:47:02.000000 sesql-2024.4.0/seSql/dbc/jars/mssql-jdbc-12.4.2.jre8.jar
+-rw-r--r--   0 rjd        (501) staff       (20)     4183 2024-04-02 00:13:12.000000 sesql-2024.4.0/seSql/sql.py
+drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-04-02 00:44:56.075430 sesql-2024.4.0/sesql.egg-info/
+-rw-r--r--   0 rjd        (501) staff       (20)     5894 2024-04-02 00:44:56.000000 sesql-2024.4.0/sesql.egg-info/PKG-INFO
+-rw-r--r--   0 rjd        (501) staff       (20)      556 2024-04-02 00:44:56.000000 sesql-2024.4.0/sesql.egg-info/SOURCES.txt
+-rw-r--r--   0 rjd        (501) staff       (20)        1 2024-04-02 00:44:56.000000 sesql-2024.4.0/sesql.egg-info/dependency_links.txt
+-rw-r--r--   0 rjd        (501) staff       (20)       56 2024-04-02 00:44:56.000000 sesql-2024.4.0/sesql.egg-info/requires.txt
+-rw-r--r--   0 rjd        (501) staff       (20)       13 2024-04-02 00:44:56.000000 sesql-2024.4.0/sesql.egg-info/top_level.txt
+-rw-r--r--   0 rjd        (501) staff       (20)       38 2024-04-02 00:44:56.075900 sesql-2024.4.0/setup.cfg
+drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-04-02 00:44:56.075126 sesql-2024.4.0/tests/
+-rw-r--r--   0 rjd        (501) staff       (20)     1790 2024-03-31 01:39:23.000000 sesql-2024.4.0/tests/test_Exceptions.py
+-rw-r--r--   0 rjd        (501) staff       (20)      222 2024-03-31 23:51:30.000000 sesql-2024.4.0/tests/test_customlogging.py
+-rw-r--r--   0 rjd        (501) staff       (20)      987 2024-04-01 01:44:20.000000 sesql-2024.4.0/tests/test_jdbc.py
+-rw-r--r--   0 rjd        (501) staff       (20)      690 2024-04-01 01:35:26.000000 sesql-2024.4.0/tests/test_odbc.py
+-rw-r--r--   0 rjd        (501) staff       (20)      238 2024-04-01 01:39:41.000000 sesql-2024.4.0/tests/test_utilities.py
```

### Comparing `sesql-2024.3.0rc6/License.md` & `sesql-2024.4.0/License.md`

 * *Files identical despite different names*

### Comparing `sesql-2024.3.0rc6/pyproject.toml` & `sesql-2024.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sesql-2024.3.0rc6/seCore/CustomLogging.py` & `sesql-2024.4.0/seCore/CustomLogging.py`

 * *Files identical despite different names*

### Comparing `sesql-2024.3.0rc6/seSql/dbc/Exceptions.py` & `sesql-2024.4.0/seSql/dbc/Exceptions.py`

 * *Files identical despite different names*

### Comparing `sesql-2024.3.0rc6/seSql/dbc/JDBC.py` & `sesql-2024.4.0/seSql/dbc/JDBC.py`

 * *Files identical despite different names*

### Comparing `sesql-2024.3.0rc6/seSql/dbc/ODBC.py` & `sesql-2024.4.0/seSql/dbc/ODBC.py`

 * *Files identical despite different names*

### Comparing `sesql-2024.3.0rc6/seSql/dbc/ODBCError.py` & `sesql-2024.4.0/seSql/dbc/ODBCError.py`

 * *Files identical despite different names*

### Comparing `sesql-2024.3.0rc6/seSql/dbc/Utilities.py` & `sesql-2024.4.0/seSql/dbc/Utilities.py`

 * *Files identical despite different names*

### Comparing `sesql-2024.3.0rc6/seSql/dbc/jars/mssql-jdbc-12.4.2.jre8.jar` & `sesql-2024.4.0/seSql/dbc/jars/mssql-jdbc-12.4.2.jre8.jar`

 * *Files identical despite different names*

### Comparing `sesql-2024.3.0rc6/seSql/sql.py` & `sesql-2024.4.0/seSql/sql.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,25 +3,23 @@
 from typing import Optional
 from seCore.CustomLogging import logger
 from .dbc.JDBC import jdbcLoaded, jdbcDriver, jdbcEngine
 from .dbc.ODBC import odbcLoaded, odbcDriver, odbcEngine
 
 
 class sql:
-    def __init__(self, enableLogging: Optional[bool] = True):
+    def __init__(self):
         self.__cnxn = None
         self.__isConnected = False
         self.__driverOverride = None
         self.__jdbcDriver = None
         self.__jdbcLoaded = None
         self.__odbcDriver = None
         self.__odbcLoaded = None
         self.__connStr = None
-        self.enableLogging = enableLogging
-
 
     def connect(self,
                 server: Optional[str] = None,
                 port: Optional[int] = None,
                 user: Optional[str] = None,
                 password: Optional[str] = None,
                 trust: Optional[str] = None,
@@ -42,15 +40,14 @@
             "user": user,
             "password": password,
             "trust": trust,
             "db": db,
             "trustServerCertificate": trustServerCertificate,
             "driverOverride": driverOverride
         }
-        logger.info(json.dumps(self.__connStr))
 
         if self.__driverOverride == "odbc" and self.__odbcLoaded:
             self.__driverOverride = "odbc"
         elif self.__driverOverride == "jdbc" and self.__jdbcLoaded:
             self.__driverOverride = "jdbc"
         else:  # pragma: no cover
             self.__driverOverride = "jdbc"
@@ -61,14 +58,15 @@
                     server=self.__connStr['server'],
                     port=self.__connStr['port'],
                     db=self.__connStr['db'],
                     user=self.__connStr['user'],
                     password=self.__connStr['password'],
                     trust=self.__connStr['trust']
                 )
+                self._logging()
 
                 try:
                     self.__cnxn.connect()
                     self.__isConnected = self.__cnxn.isConnected
                 except Exception as e:  # pragma: no cover
                     logger.error(e)
 
@@ -76,29 +74,47 @@
                 self.__cnxn = jdbcEngine(
                     server=self.__connStr['server'],
                     port=self.__connStr['port'],
                     user=self.__connStr['user'],
                     password=self.__connStr['password'],
                     trustServerCertificate=self.__connStr['trustServerCertificate']
                 )
+                self._logging()
 
                 try:
                     self.__cnxn.connect()
                     self.__isConnected = self.__cnxn.isConnected
-
                 except Exception as e:  # pragma: no cover
                     logger.error(e)
 
     def query(self,
               query: str):
         try:
             return self.__cnxn.query(query)
         except Exception as e:
             raise SQLQueryException(f'{e}')
 
+    def _logging(self):
+        oSqlDriver = {
+            "driver-info":
+                {
+                    "using": self.__driverOverride,
+                    "odbc": {
+                        "loaded": self.__odbcLoaded,
+                        "driver": self.__odbcDriver
+                    },
+                    "jdbc": {
+                        "loaded": self.__jdbcLoaded,
+                        "driver": self.__jdbcDriver
+                    }
+                }
+        }
+        logger.info(f'{json.dumps(oSqlDriver)}')
+
+
     @property
     def isConnected(self) -> bool:
         # return self.__isConnected
         return True
 
 
 class SQLQueryException(Exception):
```

### Comparing `sesql-2024.3.0rc6/sesql.egg-info/SOURCES.txt` & `sesql-2024.4.0/sesql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sesql-2024.3.0rc6/tests/test_Exceptions.py` & `sesql-2024.4.0/tests/test_Exceptions.py`

 * *Files identical despite different names*

### Comparing `sesql-2024.3.0rc6/tests/test_jdbc.py` & `sesql-2024.4.0/tests/test_jdbc.py`

 * *Files identical despite different names*

### Comparing `sesql-2024.3.0rc6/tests/test_odbc.py` & `sesql-2024.4.0/tests/test_odbc.py`

 * *Files identical despite different names*

