# Comparing `tmp/dorkbot-0.4.7.tar.gz` & `tmp/dorkbot-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dorkbot-0.4.7.tar", last modified: Thu Mar  7 21:42:09 2024, max compression
+gzip compressed data, was "dorkbot-0.4.8.tar", last modified: Tue Apr  2 15:08:20 2024, max compression
```

## Comparing `dorkbot-0.4.7.tar` & `dorkbot-0.4.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jgor       (501) staff       (20)        0 2024-03-07 21:42:09.848278 dorkbot-0.4.7/
--rw-r--r--   0 jgor       (501) staff       (20)    10596 2023-04-19 17:48:56.000000 dorkbot-0.4.7/LICENSE
--rw-r--r--   0 jgor       (501) staff       (20)       35 2023-04-19 17:48:56.000000 dorkbot-0.4.7/MANIFEST.in
--rw-r--r--   0 jgor       (501) staff       (20)    11147 2024-03-07 21:42:09.847800 dorkbot-0.4.7/PKG-INFO
--rw-r--r--   0 jgor       (501) staff       (20)    10745 2023-06-12 15:37:26.000000 dorkbot-0.4.7/README.md
-drwxr-xr-x   0 jgor       (501) staff       (20)        0 2024-03-07 21:42:09.800750 dorkbot-0.4.7/dorkbot/
--rw-r--r--   0 jgor       (501) staff       (20)       34 2023-04-19 17:48:56.000000 dorkbot-0.4.7/dorkbot/__init__.py
--rw-r--r--   0 jgor       (501) staff       (20)       22 2024-03-07 21:41:52.000000 dorkbot-0.4.7/dorkbot/_version.py
--rwxr-xr-x   0 jgor       (501) staff       (20)    33261 2024-03-01 21:15:10.000000 dorkbot-0.4.7/dorkbot/dorkbot.py
-drwxr-xr-x   0 jgor       (501) staff       (20)        0 2024-03-07 21:42:09.833379 dorkbot-0.4.7/dorkbot/indexers/
--rw-r--r--   0 jgor       (501) staff       (20)        0 2023-04-19 17:48:56.000000 dorkbot-0.4.7/dorkbot/indexers/__init__.py
--rw-r--r--   0 jgor       (501) staff       (20)     1870 2023-05-10 00:18:30.000000 dorkbot-0.4.7/dorkbot/indexers/bing_api.py
--rwxr-xr-x   0 jgor       (501) staff       (20)     6027 2024-03-07 21:39:34.000000 dorkbot-0.4.7/dorkbot/indexers/commoncrawl.py
--rw-r--r--   0 jgor       (501) staff       (20)      479 2023-05-10 00:18:30.000000 dorkbot-0.4.7/dorkbot/indexers/example.py
--rw-r--r--   0 jgor       (501) staff       (20)     3131 2023-04-27 19:42:53.000000 dorkbot-0.4.7/dorkbot/indexers/google.js
--rw-r--r--   0 jgor       (501) staff       (20)     2221 2023-05-10 00:18:30.000000 dorkbot-0.4.7/dorkbot/indexers/google.py
--rw-r--r--   0 jgor       (501) staff       (20)     3008 2023-05-10 00:18:30.000000 dorkbot-0.4.7/dorkbot/indexers/google_api.py
--rwxr-xr-x   0 jgor       (501) staff       (20)     6290 2024-03-07 21:39:24.000000 dorkbot-0.4.7/dorkbot/indexers/pywb.py
--rw-r--r--   0 jgor       (501) staff       (20)      562 2023-05-10 00:18:30.000000 dorkbot-0.4.7/dorkbot/indexers/stdin.py
--rwxr-xr-x   0 jgor       (501) staff       (20)     4679 2024-03-07 21:39:49.000000 dorkbot-0.4.7/dorkbot/indexers/wayback.py
-drwxr-xr-x   0 jgor       (501) staff       (20)        0 2024-03-07 21:42:09.846556 dorkbot-0.4.7/dorkbot/scanners/
--rw-r--r--   0 jgor       (501) staff       (20)        0 2023-04-19 17:48:56.000000 dorkbot-0.4.7/dorkbot/scanners/__init__.py
--rw-r--r--   0 jgor       (501) staff       (20)     3397 2023-05-10 00:18:30.000000 dorkbot-0.4.7/dorkbot/scanners/arachni.py
--rw-r--r--   0 jgor       (501) staff       (20)      913 2023-05-10 00:18:30.000000 dorkbot-0.4.7/dorkbot/scanners/example.py
--rw-r--r--   0 jgor       (501) staff       (20)     3160 2023-05-10 00:18:30.000000 dorkbot-0.4.7/dorkbot/scanners/wapiti.py
-drwxr-xr-x   0 jgor       (501) staff       (20)        0 2024-03-07 21:42:09.847239 dorkbot-0.4.7/dorkbot.egg-info/
--rw-r--r--   0 jgor       (501) staff       (20)    11147 2024-03-07 21:42:09.000000 dorkbot-0.4.7/dorkbot.egg-info/PKG-INFO
--rw-r--r--   0 jgor       (501) staff       (20)      659 2024-03-07 21:42:09.000000 dorkbot-0.4.7/dorkbot.egg-info/SOURCES.txt
--rw-r--r--   0 jgor       (501) staff       (20)        1 2024-03-07 21:42:09.000000 dorkbot-0.4.7/dorkbot.egg-info/dependency_links.txt
--rw-r--r--   0 jgor       (501) staff       (20)       49 2024-03-07 21:42:09.000000 dorkbot-0.4.7/dorkbot.egg-info/entry_points.txt
--rw-r--r--   0 jgor       (501) staff       (20)        8 2024-03-07 21:42:09.000000 dorkbot-0.4.7/dorkbot.egg-info/top_level.txt
--rw-r--r--   0 jgor       (501) staff       (20)       74 2024-03-07 21:42:09.849165 dorkbot-0.4.7/setup.cfg
--rw-r--r--   0 jgor       (501) staff       (20)      950 2023-04-19 17:48:56.000000 dorkbot-0.4.7/setup.py
+drwxr-xr-x   0 jgor       (501) staff       (20)        0 2024-04-02 15:08:20.649234 dorkbot-0.4.8/
+-rw-r--r--   0 jgor       (501) staff       (20)    10596 2023-04-19 17:48:56.000000 dorkbot-0.4.8/LICENSE
+-rw-r--r--   0 jgor       (501) staff       (20)       35 2023-04-19 17:48:56.000000 dorkbot-0.4.8/MANIFEST.in
+-rw-r--r--   0 jgor       (501) staff       (20)    11147 2024-04-02 15:08:20.648760 dorkbot-0.4.8/PKG-INFO
+-rw-r--r--   0 jgor       (501) staff       (20)    10745 2023-06-12 15:37:26.000000 dorkbot-0.4.8/README.md
+drwxr-xr-x   0 jgor       (501) staff       (20)        0 2024-04-02 15:08:20.601182 dorkbot-0.4.8/dorkbot/
+-rw-r--r--   0 jgor       (501) staff       (20)       34 2023-04-19 17:48:56.000000 dorkbot-0.4.8/dorkbot/__init__.py
+-rw-r--r--   0 jgor       (501) staff       (20)       22 2024-04-02 15:03:40.000000 dorkbot-0.4.8/dorkbot/_version.py
+-rwxr-xr-x   0 jgor       (501) staff       (20)    33306 2024-03-28 19:59:08.000000 dorkbot-0.4.8/dorkbot/dorkbot.py
+drwxr-xr-x   0 jgor       (501) staff       (20)        0 2024-04-02 15:08:20.640295 dorkbot-0.4.8/dorkbot/indexers/
+-rw-r--r--   0 jgor       (501) staff       (20)        0 2023-04-19 17:48:56.000000 dorkbot-0.4.8/dorkbot/indexers/__init__.py
+-rw-r--r--   0 jgor       (501) staff       (20)     1870 2023-05-10 00:18:30.000000 dorkbot-0.4.8/dorkbot/indexers/bing_api.py
+-rwxr-xr-x   0 jgor       (501) staff       (20)     6027 2024-03-07 21:39:34.000000 dorkbot-0.4.8/dorkbot/indexers/commoncrawl.py
+-rw-r--r--   0 jgor       (501) staff       (20)      479 2023-05-10 00:18:30.000000 dorkbot-0.4.8/dorkbot/indexers/example.py
+-rw-r--r--   0 jgor       (501) staff       (20)     3131 2023-04-27 19:42:53.000000 dorkbot-0.4.8/dorkbot/indexers/google.js
+-rw-r--r--   0 jgor       (501) staff       (20)     2221 2023-05-10 00:18:30.000000 dorkbot-0.4.8/dorkbot/indexers/google.py
+-rw-r--r--   0 jgor       (501) staff       (20)     3008 2023-05-10 00:18:30.000000 dorkbot-0.4.8/dorkbot/indexers/google_api.py
+-rwxr-xr-x   0 jgor       (501) staff       (20)     6290 2024-03-07 21:39:24.000000 dorkbot-0.4.8/dorkbot/indexers/pywb.py
+-rw-r--r--   0 jgor       (501) staff       (20)      562 2023-05-10 00:18:30.000000 dorkbot-0.4.8/dorkbot/indexers/stdin.py
+-rwxr-xr-x   0 jgor       (501) staff       (20)     4679 2024-03-07 21:39:49.000000 dorkbot-0.4.8/dorkbot/indexers/wayback.py
+drwxr-xr-x   0 jgor       (501) staff       (20)        0 2024-04-02 15:08:20.647691 dorkbot-0.4.8/dorkbot/scanners/
+-rw-r--r--   0 jgor       (501) staff       (20)        0 2023-04-19 17:48:56.000000 dorkbot-0.4.8/dorkbot/scanners/__init__.py
+-rw-r--r--   0 jgor       (501) staff       (20)     3397 2023-05-10 00:18:30.000000 dorkbot-0.4.8/dorkbot/scanners/arachni.py
+-rw-r--r--   0 jgor       (501) staff       (20)      913 2023-05-10 00:18:30.000000 dorkbot-0.4.8/dorkbot/scanners/example.py
+-rw-r--r--   0 jgor       (501) staff       (20)     3160 2023-05-10 00:18:30.000000 dorkbot-0.4.8/dorkbot/scanners/wapiti.py
+drwxr-xr-x   0 jgor       (501) staff       (20)        0 2024-04-02 15:08:20.648302 dorkbot-0.4.8/dorkbot.egg-info/
+-rw-r--r--   0 jgor       (501) staff       (20)    11147 2024-04-02 15:08:20.000000 dorkbot-0.4.8/dorkbot.egg-info/PKG-INFO
+-rw-r--r--   0 jgor       (501) staff       (20)      659 2024-04-02 15:08:20.000000 dorkbot-0.4.8/dorkbot.egg-info/SOURCES.txt
+-rw-r--r--   0 jgor       (501) staff       (20)        1 2024-04-02 15:08:20.000000 dorkbot-0.4.8/dorkbot.egg-info/dependency_links.txt
+-rw-r--r--   0 jgor       (501) staff       (20)       49 2024-04-02 15:08:20.000000 dorkbot-0.4.8/dorkbot.egg-info/entry_points.txt
+-rw-r--r--   0 jgor       (501) staff       (20)        8 2024-04-02 15:08:20.000000 dorkbot-0.4.8/dorkbot.egg-info/top_level.txt
+-rw-r--r--   0 jgor       (501) staff       (20)       74 2024-04-02 15:08:20.650030 dorkbot-0.4.8/setup.cfg
+-rw-r--r--   0 jgor       (501) staff       (20)      950 2023-04-19 17:48:56.000000 dorkbot-0.4.8/setup.py
```

### Comparing `dorkbot-0.4.7/LICENSE` & `dorkbot-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.7/PKG-INFO` & `dorkbot-0.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dorkbot
-Version: 0.4.7
+Version: 0.4.8
 Summary: Command-line tool to scan search results for vulnerabilities
 Home-page: http://dorkbot.io
 Author: jgor
 Author-email: jgor@utexas.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: OS Independent
```

### Comparing `dorkbot-0.4.7/README.md` & `dorkbot-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.7/dorkbot/dorkbot.py` & `dorkbot-0.4.8/dorkbot/dorkbot.py`

 * *Files 0% similar despite different names*

```diff
@@ -490,15 +490,15 @@
                         sql += " WHERE "
                     sql += "source = %s" % self.param
                     c.execute(sql, (source,))
                 else:
                     c.execute(sql)
                 urls = [" | ".join(row) for row in c.fetchall()]
         except self.module.Error as e:
-            logging.error("Failed to get targets - %s", str(e))
+            logging.exception("Failed to get targets - %s", str(e))
             sys.exit(1)
 
         if randomize:
             random.shuffle(urls)
 
         return urls
 
@@ -567,15 +567,15 @@
     def get_scanned(self, fingerprint, cursor):
         for i in range(3):
             try:
                 cursor.execute("SELECT fingerprint FROM fingerprints WHERE fingerprint = (%s)" % self.param, (fingerprint,))
                 row = cursor.fetchone()
                 break
             except self.module.Error as e:
-                if "connection already closed" in str(e) or "server closed the connection unexpectedly" in str(e):
+                if "connection already closed" in str(e) or "cursor already closed" in str(e) or "server closed the connection unexpectedly" in str(e):
                     logging.warning("Failed to look up fingerprint (retrying) - %s", str(e))
                     self.connect()
                     continue
                 else:
                     logging.error("Failed to look up fingerprint - %s", str(e))
                     sys.exit(1)
 
@@ -794,15 +794,15 @@
     def read_items(self):
         if self.database:
             try:
                 with self.db, closing(self.db.cursor()) as c:
                     c.execute("SELECT item FROM blocklist")
                     items = [row[0] for row in c.fetchall()]
             except self.module.Error as e:
-                logging.error("Failed to get targets - %s", str(e))
+                logging.exception("Failed to get targets - %s", str(e))
                 sys.exit(1)
         else:
             items = self.blocklist_file.read().splitlines()
 
         return items
 
     def add(self, item):
```

### Comparing `dorkbot-0.4.7/dorkbot/indexers/bing_api.py` & `dorkbot-0.4.8/dorkbot/indexers/bing_api.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.7/dorkbot/indexers/commoncrawl.py` & `dorkbot-0.4.8/dorkbot/indexers/commoncrawl.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.7/dorkbot/indexers/google.js` & `dorkbot-0.4.8/dorkbot/indexers/google.js`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.7/dorkbot/indexers/google.py` & `dorkbot-0.4.8/dorkbot/indexers/google.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.7/dorkbot/indexers/google_api.py` & `dorkbot-0.4.8/dorkbot/indexers/google_api.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.7/dorkbot/indexers/pywb.py` & `dorkbot-0.4.8/dorkbot/indexers/pywb.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.7/dorkbot/indexers/stdin.py` & `dorkbot-0.4.8/dorkbot/indexers/stdin.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.7/dorkbot/indexers/wayback.py` & `dorkbot-0.4.8/dorkbot/indexers/wayback.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.7/dorkbot/scanners/arachni.py` & `dorkbot-0.4.8/dorkbot/scanners/arachni.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.7/dorkbot/scanners/example.py` & `dorkbot-0.4.8/dorkbot/scanners/example.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.7/dorkbot/scanners/wapiti.py` & `dorkbot-0.4.8/dorkbot/scanners/wapiti.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.7/dorkbot.egg-info/PKG-INFO` & `dorkbot-0.4.8/dorkbot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dorkbot
-Version: 0.4.7
+Version: 0.4.8
 Summary: Command-line tool to scan search results for vulnerabilities
 Home-page: http://dorkbot.io
 Author: jgor
 Author-email: jgor@utexas.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: OS Independent
```

### Comparing `dorkbot-0.4.7/dorkbot.egg-info/SOURCES.txt` & `dorkbot-0.4.8/dorkbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.7/setup.py` & `dorkbot-0.4.8/setup.py`

 * *Files identical despite different names*

