# Comparing `tmp/dbservice-2.1.1.tar.gz` & `tmp/dbservice-2.1.2.tar.gz`

## Comparing `dbservice-2.1.1.tar` & `dbservice-2.1.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 dbservice-2.1.1/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 dbservice-2.1.1/src/.DS_Store
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 dbservice-2.1.1/src/__init__.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 dbservice-2.1.1/src/DBService/__init__.py
--rw-r--r--   0        0        0    17962 2020-02-02 00:00:00.000000 dbservice-2.1.1/src/DBService/dbcore.py
--rw-r--r--   0        0        0    26116 2020-02-02 00:00:00.000000 dbservice-2.1.1/src/DBService/dbcore_old.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 dbservice-2.1.1/test/__init__.py
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 dbservice-2.1.1/test/test.py
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 dbservice-2.1.1/test/testMysql_gone_away.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 dbservice-2.1.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 dbservice-2.1.1/LICENSE
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 dbservice-2.1.1/README.md
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dbservice-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 dbservice-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 dbservice-2.1.2/.DS_Store
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 dbservice-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 dbservice-2.1.2/src/.DS_Store
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 dbservice-2.1.2/src/__init__.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 dbservice-2.1.2/src/DBService/__init__.py
+-rw-r--r--   0        0        0    17929 2020-02-02 00:00:00.000000 dbservice-2.1.2/src/DBService/dbcore.py
+-rw-r--r--   0        0        0    26116 2020-02-02 00:00:00.000000 dbservice-2.1.2/src/DBService/dbcore_old.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 dbservice-2.1.2/test/__init__.py
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 dbservice-2.1.2/test/test.py
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 dbservice-2.1.2/test/testMysql_gone_away.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 dbservice-2.1.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 dbservice-2.1.2/LICENSE
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 dbservice-2.1.2/README.md
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dbservice-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 dbservice-2.1.2/PKG-INFO
```

### Comparing `dbservice-2.1.1/.DS_Store` & `dbservice-2.1.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `dbservice-2.1.1/src/.DS_Store` & `dbservice-2.1.2/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `dbservice-2.1.1/src/DBService/dbcore.py` & `dbservice-2.1.2/src/DBService/dbcore.py`

 * *Files 1% similar despite different names*

```diff
@@ -391,15 +391,14 @@
             port=self.port,
             user=self.user,
             password=self.password,
             db=self.db,
             minsize=self.minsize,
             maxsize=self.maxsize
         )
-        print('创建连接池')
 
     async def close_pool(self):
         # 关闭连接池
         self.pool.close()
         await self.pool.wait_closed()
 
     async def query(self, query, params=None, fetch_all=True):
```

### Comparing `dbservice-2.1.1/src/DBService/dbcore_old.py` & `dbservice-2.1.2/src/DBService/dbcore_old.py`

 * *Files identical despite different names*

### Comparing `dbservice-2.1.1/test/test.py` & `dbservice-2.1.2/test/test.py`

 * *Files identical despite different names*

### Comparing `dbservice-2.1.1/test/testMysql_gone_away.py` & `dbservice-2.1.2/test/testMysql_gone_away.py`

 * *Files identical despite different names*

### Comparing `dbservice-2.1.1/LICENSE` & `dbservice-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbservice-2.1.1/README.md` & `dbservice-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `dbservice-2.1.1/pyproject.toml` & `dbservice-2.1.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "DBService"
-version = "2.1.1"
+version = "2.1.2"
 authors = [
   { name="hang.zhang", email="hhczy1003@163.com"},
   { name="Marrin.Hu", email="himarrin@gmail.com"},
 ]
 description = "a Database Wrapper for Redis and MySQL"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `dbservice-2.1.1/PKG-INFO` & `dbservice-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DBService
-Version: 2.1.1
+Version: 2.1.2
 Summary: a Database Wrapper for Redis and MySQL
 Project-URL: Homepage, https://pypi.org/project/DBService/
 Author-email: "hang.zhang" <hhczy1003@163.com>, "Marrin.Hu" <himarrin@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

