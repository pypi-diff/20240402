# Comparing `tmp/marioutils-1.0.1.tar.gz` & `tmp/marioutils-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marioutils-1.0.1.tar", last modified: Tue Apr  2 01:49:09 2024, max compression
+gzip compressed data, was "marioutils-1.1.0.tar", last modified: Tue Apr  2 20:11:52 2024, max compression
```

## Comparing `marioutils-1.0.1.tar` & `marioutils-1.1.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 01:49:09.551270 marioutils-1.0.1/
--rw-rw-rw-   0        0        0     1088 2024-03-29 19:37:30.000000 marioutils-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      925 2024-04-02 01:49:09.550272 marioutils-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-02 01:49:09.085092 marioutils-1.0.1/mario_utils/
--rw-rw-rw-   0        0        0      166 2024-04-02 00:21:18.000000 marioutils-1.0.1/mario_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 01:49:09.123092 marioutils-1.0.1/mario_utils/databasemanagement/
--rw-rw-rw-   0        0        0       93 2024-04-02 00:18:26.000000 marioutils-1.0.1/mario_utils/databasemanagement/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 01:49:09.192803 marioutils-1.0.1/mario_utils/databasemanagement/src/
--rw-rw-rw-   0        0        0       99 2024-04-01 21:45:12.000000 marioutils-1.0.1/mario_utils/databasemanagement/src/__init__.py
--rw-rw-rw-   0        0        0     1360 2024-03-29 19:37:30.000000 marioutils-1.0.1/mario_utils/databasemanagement/src/exceptions.py
--rw-rw-rw-   0        0        0     5073 2024-03-29 19:37:30.000000 marioutils-1.0.1/mario_utils/databasemanagement/src/manager.py
-drwxrwxrwx   0        0        0        0 2024-04-02 01:49:09.195805 marioutils-1.0.1/mario_utils/databasemanagement/tests/
--rw-rw-rw-   0        0        0        0 2024-03-29 19:37:30.000000 marioutils-1.0.1/mario_utils/databasemanagement/tests/__init__.py
--rw-rw-rw-   0        0        0     1982 2024-04-02 00:43:58.000000 marioutils-1.0.1/mario_utils/databasemanagement/tests/test_.py
-drwxrwxrwx   0        0        0        0 2024-04-02 01:49:09.197804 marioutils-1.0.1/mario_utils/logger/
--rw-rw-rw-   0        0        0       67 2024-04-01 21:49:53.000000 marioutils-1.0.1/mario_utils/logger/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 01:49:09.291620 marioutils-1.0.1/mario_utils/logger/src/
--rw-rw-rw-   0        0        0       70 2024-04-01 21:48:54.000000 marioutils-1.0.1/mario_utils/logger/src/__init__.py
--rw-rw-rw-   0        0        0      982 2024-04-02 00:23:57.000000 marioutils-1.0.1/mario_utils/logger/src/logger.py
-drwxrwxrwx   0        0        0        0 2024-04-02 01:49:09.293621 marioutils-1.0.1/mario_utils/logger/test/
--rw-rw-rw-   0        0        0        0 2024-03-29 19:37:30.000000 marioutils-1.0.1/mario_utils/logger/test/__init__.py
--rw-rw-rw-   0        0        0      572 2024-04-02 00:22:14.000000 marioutils-1.0.1/mario_utils/logger/test/test_logger.py
-drwxrwxrwx   0        0        0        0 2024-04-02 01:49:09.517272 marioutils-1.0.1/marioutils.egg-info/
--rw-rw-rw-   0        0        0      925 2024-04-02 01:49:08.000000 marioutils-1.0.1/marioutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      667 2024-04-02 01:49:09.000000 marioutils-1.0.1/marioutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 01:49:08.000000 marioutils-1.0.1/marioutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-04-02 01:49:08.000000 marioutils-1.0.1/marioutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-02 01:49:08.000000 marioutils-1.0.1/marioutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 01:49:09.552272 marioutils-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1023 2024-04-02 01:49:04.000000 marioutils-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:11:52.388792 marioutils-1.1.0/
+-rw-rw-rw-   0        0        0     1088 2024-03-29 19:37:30.000000 marioutils-1.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      925 2024-04-02 20:11:52.386791 marioutils-1.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-02 20:11:51.961732 marioutils-1.1.0/mario_utils/
+-rw-rw-rw-   0        0        0      269 2024-03-29 19:37:30.000000 marioutils-1.1.0/mario_utils/README.md
+-rw-rw-rw-   0        0        0      166 2024-04-02 00:21:18.000000 marioutils-1.1.0/mario_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:11:51.994887 marioutils-1.1.0/mario_utils/databasemanagement/
+-rw-rw-rw-   0        0        0       93 2024-04-02 00:18:26.000000 marioutils-1.1.0/mario_utils/databasemanagement/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:11:52.063584 marioutils-1.1.0/mario_utils/databasemanagement/src/
+-rw-rw-rw-   0        0        0       99 2024-04-01 21:45:12.000000 marioutils-1.1.0/mario_utils/databasemanagement/src/__init__.py
+-rw-rw-rw-   0        0        0     1360 2024-03-29 19:37:30.000000 marioutils-1.1.0/mario_utils/databasemanagement/src/exceptions.py
+-rw-rw-rw-   0        0        0     5672 2024-04-02 19:57:09.000000 marioutils-1.1.0/mario_utils/databasemanagement/src/manager.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:11:52.065925 marioutils-1.1.0/mario_utils/databasemanagement/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-29 19:37:30.000000 marioutils-1.1.0/mario_utils/databasemanagement/tests/__init__.py
+-rw-rw-rw-   0        0        0     2243 2024-04-02 20:06:55.000000 marioutils-1.1.0/mario_utils/databasemanagement/tests/test_.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:11:52.067928 marioutils-1.1.0/mario_utils/logger/
+-rw-rw-rw-   0        0        0       67 2024-04-01 21:49:53.000000 marioutils-1.1.0/mario_utils/logger/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:11:52.153130 marioutils-1.1.0/mario_utils/logger/src/
+-rw-rw-rw-   0        0        0       70 2024-04-01 21:48:54.000000 marioutils-1.1.0/mario_utils/logger/src/__init__.py
+-rw-rw-rw-   0        0        0      982 2024-04-02 00:23:57.000000 marioutils-1.1.0/mario_utils/logger/src/logger.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:11:52.156644 marioutils-1.1.0/mario_utils/logger/test/
+-rw-rw-rw-   0        0        0        0 2024-03-29 19:37:30.000000 marioutils-1.1.0/mario_utils/logger/test/__init__.py
+-rw-rw-rw-   0        0        0      572 2024-04-02 00:22:14.000000 marioutils-1.1.0/mario_utils/logger/test/test_logger.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:11:52.353057 marioutils-1.1.0/marioutils.egg-info/
+-rw-rw-rw-   0        0        0      925 2024-04-02 20:11:51.000000 marioutils-1.1.0/marioutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      689 2024-04-02 20:11:51.000000 marioutils-1.1.0/marioutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 20:11:51.000000 marioutils-1.1.0/marioutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-04-02 20:11:51.000000 marioutils-1.1.0/marioutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-02 20:11:51.000000 marioutils-1.1.0/marioutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 20:11:52.389791 marioutils-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1044 2024-04-02 20:11:37.000000 marioutils-1.1.0/setup.py
```

### Comparing `marioutils-1.0.1/LICENSE.txt` & `marioutils-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `marioutils-1.0.1/PKG-INFO` & `marioutils-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marioutils
-Version: 1.0.1
+Version: 1.1.0
 Summary: Utils library for DB connection and logging
 Home-page: https://github.com/MarioHdzCtu/MarioUtils
 Author: Mario Hernandez
 Author-email: mariohertu@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `marioutils-1.0.1/mario_utils/databasemanagement/src/exceptions.py` & `marioutils-1.1.0/mario_utils/databasemanagement/src/exceptions.py`

 * *Files identical despite different names*

### Comparing `marioutils-1.0.1/mario_utils/databasemanagement/src/manager.py` & `marioutils-1.1.0/mario_utils/databasemanagement/src/manager.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 import pymssql
 from . import exceptions
 import sqlalchemy
 import mariadb
 
+
 class Database:
 
-    def __init__(self, server: str, user: str, password: str, database: str = None, as_dict: bool = True,port: int = 1333, pool_size: int | sqlalchemy.pool.NullPool = 5, max_overflow: int = 10):
+    def __init__(
+            self,
+            server: str,
+            user: str,
+            password: str,
+            database: str = None,
+            as_dict: bool = True,
+            port: int = 1333,
+            pool_size: int | sqlalchemy.pool.NullPool = 5,
+            max_overflow: int = 10):
         self.server = server
         self.user = user
         self.password = password
         self.database = database
         self.port = port
         self.as_dict = as_dict
         self.pool_size = pool_size
@@ -25,135 +35,174 @@
             if self.max_overflow < self.pool_size:
                 raise exceptions.MaxOverflowSizeException
 
     def __enter__(self):
         self.connect()
         self.get_cursor()
         return self
-    
+
     def __exit__(self, exception_type, exception_value, exception_traceback):
         self.close_connection()
 
     def get_connection(self):
         pass
 
     def connect(self):
         self._connection = self._pool.connect()
 
     @property
     def connection(self):
         return self._connection
-    
+
     @property
     def connected(self) -> bool:
         try:
             conn = self._pool.connect()
             cursor = conn.cursor()
             cursor.execute('SELECT 1 AS test')
             return True
         except Exception:
             return False
 
     @property
     def cursor(self):
         return self._cursor
-    
+
     def get_cursor(self):
         if self._connection is None:
             raise exceptions.ConnectionException
         if self._cursor is None:
             self._cursor = self.connection.cursor()
 
     def create_pool(self):
         if self._pool is None:
-            self._pool = sqlalchemy.pool.QueuePool(self.get_connection, max_overflow=10, pool_size=5)
+            self._pool = sqlalchemy.pool.QueuePool(
+                self.get_connection,
+                max_overflow=10,
+                pool_size=5)
 
     @property
     def pool(self):
         return self._pool
-   
-    def execute(self, query: str):
+
+    def execute(self, query: str, vals: tuple = ()):
         if self._cursor is None:
             raise exceptions.CursorException
         try:
-            self._cursor.execute(query)
+            self._cursor.execute(query, vals)
         except Exception as e:
             return e
         else:
             return self.fetchall()
         finally:
             self.close_connection()
 
     def fetchall(self):
         try:
             res = self._cursor.fetchall()
         except Exception as e:
             return e
         else:
             return res
-        return 
+        return
 
     def close_connection(self):
         self._connection.close()
 
+
 class MsSQLDatabase(Database):
 
-    def __init__(self, server: str, user: str, password: str, database: str = None, as_dict: bool = True, port: int = 1433, pool_size: int | sqlalchemy.pool.NullPool = 5, max_overflow: int = 10) -> pymssql.Connection:
-        super().__init__(server, user, password, database, as_dict, pool_size, max_overflow)
+    def __init__(
+            self,
+            server: str,
+            user: str,
+            password: str,
+            database: str = None,
+            as_dict: bool = True,
+            port: int = 1433,
+            pool_size: int | sqlalchemy.pool.NullPool = 5,
+            max_overflow: int = 10) -> pymssql.Connection:
+        super().__init__(
+            server,
+            user,
+            password,
+            database,
+            as_dict,
+            pool_size,
+            max_overflow)
         self.create_pool()
-    
+
     def get_connection(self):
         c = pymssql.connect(
             server=self.server,
             user=self.user,
             password=self.password,
             database=self.database,
             as_dict=self.as_dict,
             login_timeout=20,
             timeout=20
         )
         return c
-    
+
     def get_cursor(self):
         if self._connection is None:
             raise exceptions.ConnectionException
         if self._cursor is None:
             self._cursor = self.connection.cursor()
 
+
 class MariaDatabase(Database):
-    def __init__(self, server: str, user: str, password: str, database: str = None, as_dict: bool = True, port: int = 3306, pool_size: int | sqlalchemy.pool.NullPool = 5, max_overflow: int = 10):
-        super().__init__(server, user, password, database, as_dict, port, pool_size, max_overflow)
+    def __init__(
+            self,
+            server: str,
+            user: str,
+            password: str,
+            database: str = None,
+            as_dict: bool = True,
+            port: int = 3306,
+            pool_size: int | sqlalchemy.pool.NullPool = 5,
+            max_overflow: int = 10):
+        super().__init__(
+            server,
+            user,
+            password,
+            database,
+            as_dict,
+            port,
+            pool_size,
+            max_overflow)
         self.create_pool()
 
     def get_connection(self):
         c = mariadb.connect(
-            user = self.user,
-            password = self.password,
-            host = self.server,
-            port = self.port,
-            database = self.database
+            user=self.user,
+            password=self.password,
+            host=self.server,
+            port=self.port,
+            database=self.database
         )
         return c
 
     def get_cursor(self):
         if self._connection is None:
             raise exceptions.ConnectionException
         if self._cursor is None:
             self._cursor = self.connection.cursor()
         else:
             return self._cursor
-        
+
     def fetchall(self):
         try:
             res = self._cursor.fetchall()
             if not self.as_dict:
                 return res
             else:
                 columns = [a[0] for a in self._cursor.description]
                 results = [{c: v for c, v in zip(columns, r)} for r in res]
                 return results
         except Exception as e:
             return e
-        
+
 
 if __name__ == '__main__':
-    print("This package is not meant to run as a main file. If needed to test, use the pytest set in this package.")
+    print("""This package is not meant to run as a main file.
+          If needed to test, use the pytest set in this package.""")
```

### Comparing `marioutils-1.0.1/mario_utils/databasemanagement/tests/test_.py` & `marioutils-1.1.0/mario_utils/databasemanagement/tests/test_.py`

 * *Files 15% similar despite different names*

```diff
@@ -44,26 +44,36 @@
     db_error = src.MariaDatabase(
             server=os.getenv('DB_mariadb_SERVER'),
             user=os.getenv('DB_mariadb_USER_ERROR'),
             password=os.getenv('DB_mariadb_PASSWORD_ERROR'),
             database=os.getenv('DB_mariadb_DATABASE'))
     yield db_error
 
+
 @pytest.mark.skip('Not implemented')
 def test_mssql_db_error(mssql_db_error):
     with pytest.raises(pymssql._pymssql.OperationalError):
         mssql_db_error.connected
 
 
 def test_maria_db_error(maria_db_error):
     with pytest.raises(mariadb.Error):
         with maria_db_error as conn:
             conn.connected
 
+
 @pytest.mark.skip('Not implemented')
 def test_mssql_db_success(mssql_db):
     assert mssql_db.connected
 
 
 def test_maria_db_success(maria_db):
     with maria_db as conn:
         assert conn.connected
+
+
+def test_maria_db_execute(maria_db):
+    with maria_db as conn:
+        query = "SELECT * FROM tests.test WHERE id = ?"
+        vals = (1,)
+        res = conn.execute(query=query, vals=vals)
+        assert res == [{'id': 1, 'test_name': 'test1'}]
```

### Comparing `marioutils-1.0.1/mario_utils/logger/src/logger.py` & `marioutils-1.1.0/mario_utils/logger/src/logger.py`

 * *Files identical despite different names*

### Comparing `marioutils-1.0.1/mario_utils/logger/test/test_logger.py` & `marioutils-1.1.0/mario_utils/logger/test/test_logger.py`

 * *Files identical despite different names*

### Comparing `marioutils-1.0.1/marioutils.egg-info/PKG-INFO` & `marioutils-1.1.0/marioutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marioutils
-Version: 1.0.1
+Version: 1.1.0
 Summary: Utils library for DB connection and logging
 Home-page: https://github.com/MarioHdzCtu/MarioUtils
 Author: Mario Hernandez
 Author-email: mariohertu@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `marioutils-1.0.1/marioutils.egg-info/SOURCES.txt` & `marioutils-1.1.0/marioutils.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE.txt
 setup.py
+mario_utils/README.md
 mario_utils/__init__.py
 mario_utils/databasemanagement/__init__.py
 mario_utils/databasemanagement/src/__init__.py
 mario_utils/databasemanagement/src/exceptions.py
 mario_utils/databasemanagement/src/manager.py
 mario_utils/databasemanagement/tests/__init__.py
 mario_utils/databasemanagement/tests/test_.py
```

### Comparing `marioutils-1.0.1/setup.py` & `marioutils-1.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 from setuptools import find_packages, setup
 
-with open("mario_utils\README.md", 'r') as f:
+with open("mario_utils/README.md", 'r') as f:
     long_description = f.read()
 
 setup(
     name="marioutils",
-    version="1.0.1",
+    version="1.1.0",
     description="Utils library for DB connection and logging",
     packages=find_packages(),
-    package_data={'mario_utils':['databasemanagement/*'],'mario_utils':['logger/*']},
+    package_data={'mario_utils': ['databasemanagement/*', 'logger/*', '*']},
     include_package_data=True,
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MarioHdzCtu/MarioUtils",
     author="Mario Hernandez",
     author_email="mariohertu@gmail.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent"
     ],
-    install_requires=["pymssql >= 2.2.11", "sqlalchemy >= 2.0.25", "mariadb >= 1.1.10"],
+    install_requires=[
+        "pymssql >= 2.2.11",
+        "sqlalchemy >= 2.0.25",
+        "mariadb >= 1.1.10"],
     extras_require={
         "dev": ["pytest>=8.0.0"]
     },
     python_requires=">=3.10.12",
     include_dirs=True
-)
+)
```

