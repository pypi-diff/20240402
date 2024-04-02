# Comparing `tmp/maadsbml-1.3.4.tar.gz` & `tmp/maadsbml-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maadsbml-1.3.4.tar", last modified: Mon Apr  1 04:08:44 2024, max compression
+gzip compressed data, was "maadsbml-1.3.5.tar", last modified: Tue Apr  2 18:14:28 2024, max compression
```

## Comparing `maadsbml-1.3.4.tar` & `maadsbml-1.3.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 04:08:44.178448 maadsbml-1.3.4/
--rw-rw-rw-   0        0        0     1067 2021-04-28 21:31:09.000000 maadsbml-1.3.4/LICENSE.txt
--rw-rw-rw-   0        0        0       65 2021-01-25 23:03:44.000000 maadsbml-1.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0     8814 2024-04-01 04:08:44.178448 maadsbml-1.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     8277 2024-04-01 04:08:00.000000 maadsbml-1.3.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 04:08:44.160239 maadsbml-1.3.4/maadsbml/
--rw-rw-rw-   0        0        0      204 2024-03-29 17:59:02.000000 maadsbml-1.3.4/maadsbml/__init__.py
--rw-rw-rw-   0        0        0     8841 2020-10-18 21:34:32.000000 maadsbml-1.3.4/maadsbml/balancedata.py
--rw-rw-rw-   0        0        0     5395 2020-06-27 20:48:48.000000 maadsbml-1.3.4/maadsbml/callmas.py
--rw-rw-rw-   0        0        0     6983 2024-04-01 04:05:22.000000 maadsbml-1.3.4/maadsbml/sendfiles.py
-drwxrwxrwx   0        0        0        0 2024-04-01 04:08:44.177446 maadsbml-1.3.4/maadsbml.egg-info/
--rw-rw-rw-   0        0        0     8814 2024-04-01 04:08:43.000000 maadsbml-1.3.4/maadsbml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2024-04-01 04:08:44.000000 maadsbml-1.3.4/maadsbml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 04:08:43.000000 maadsbml-1.3.4/maadsbml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2024-04-01 04:08:43.000000 maadsbml-1.3.4/maadsbml.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-01 04:08:43.000000 maadsbml-1.3.4/maadsbml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      122 2021-02-05 16:13:30.000000 maadsbml-1.3.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 04:08:44.179640 maadsbml-1.3.4/setup.cfg
--rw-rw-rw-   0        0        0     1026 2024-04-01 04:05:31.000000 maadsbml-1.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 18:14:28.623361 maadsbml-1.3.5/
+-rw-rw-rw-   0        0        0     1067 2021-04-28 21:31:09.000000 maadsbml-1.3.5/LICENSE.txt
+-rw-rw-rw-   0        0        0       65 2021-01-25 23:03:44.000000 maadsbml-1.3.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     8814 2024-04-02 18:14:28.623361 maadsbml-1.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     8277 2024-04-01 04:08:00.000000 maadsbml-1.3.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 18:14:28.593637 maadsbml-1.3.5/maadsbml/
+-rw-rw-rw-   0        0        0      204 2024-03-29 17:59:02.000000 maadsbml-1.3.5/maadsbml/__init__.py
+-rw-rw-rw-   0        0        0     8841 2020-10-18 21:34:32.000000 maadsbml-1.3.5/maadsbml/balancedata.py
+-rw-rw-rw-   0        0        0     5395 2020-06-27 20:48:48.000000 maadsbml-1.3.5/maadsbml/callmas.py
+-rw-rw-rw-   0        0        0     6985 2024-04-02 18:13:18.000000 maadsbml-1.3.5/maadsbml/sendfiles.py
+drwxrwxrwx   0        0        0        0 2024-04-02 18:14:28.621854 maadsbml-1.3.5/maadsbml.egg-info/
+-rw-rw-rw-   0        0        0     8814 2024-04-02 18:14:28.000000 maadsbml-1.3.5/maadsbml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2024-04-02 18:14:28.000000 maadsbml-1.3.5/maadsbml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 18:14:28.000000 maadsbml-1.3.5/maadsbml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2024-04-02 18:14:28.000000 maadsbml-1.3.5/maadsbml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-02 18:14:28.000000 maadsbml-1.3.5/maadsbml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      122 2021-02-05 16:13:30.000000 maadsbml-1.3.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 18:14:28.624717 maadsbml-1.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     1026 2024-04-02 18:14:20.000000 maadsbml-1.3.5/setup.py
```

### Comparing `maadsbml-1.3.4/LICENSE.txt` & `maadsbml-1.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maadsbml-1.3.4/PKG-INFO` & `maadsbml-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maadsbml
-Version: 1.3.4
+Version: 1.3.5
 Summary: Multi-Agent Accelerator for Data Science (MAADS) Batch AutoML
 Home-page: https://github.com/smaurice101/acnsmauricedsmas
 Author: Sebastian Maurice
 Author-email: sebastian.maurice@otics.ca
 License: MIT License
 Keywords: multi-agent, data science, batch automl, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence,predictive analytics,advanced analytics
 Description-Content-Type: text/markdown
```

### Comparing `maadsbml-1.3.4/README.md` & `maadsbml-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `maadsbml-1.3.4/maadsbml/balancedata.py` & `maadsbml-1.3.5/maadsbml/balancedata.py`

 * *Files identical despite different names*

### Comparing `maadsbml-1.3.4/maadsbml/callmas.py` & `maadsbml-1.3.5/maadsbml/callmas.py`

 * *Files identical despite different names*

### Comparing `maadsbml-1.3.4/maadsbml/sendfiles.py` & `maadsbml-1.3.5/maadsbml/sendfiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
     loop = asyncio.get_event_loop()
     val=loop.run_until_complete(tcp_echo_clienttrain(value, loop,host,port,microserviceid,timeout))
 #    loop.close()
     return val
 
 def abort(host,port=10000):
 
-    url = "%s:10000/?abort=1" % (host)
+    url = "%s:%s/?abort=1" % (host,port)
     mainurl = url
 
     print(mainurl)
   
     value="%s" % (mainurl)
     loop = asyncio.get_event_loop()
     val=loop.run_until_complete(tcp_echo_clienttrain(value, loop,host,port,''))
```

### Comparing `maadsbml-1.3.4/maadsbml.egg-info/PKG-INFO` & `maadsbml-1.3.5/maadsbml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maadsbml
-Version: 1.3.4
+Version: 1.3.5
 Summary: Multi-Agent Accelerator for Data Science (MAADS) Batch AutoML
 Home-page: https://github.com/smaurice101/acnsmauricedsmas
 Author: Sebastian Maurice
 Author-email: sebastian.maurice@otics.ca
 License: MIT License
 Keywords: multi-agent, data science, batch automl, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence,predictive analytics,advanced analytics
 Description-Content-Type: text/markdown
```

### Comparing `maadsbml-1.3.4/setup.py` & `maadsbml-1.3.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 	
 
 with open("requirements.txt","r") as f:
     required = f.read().splitlines()
     
 setuptools.setup(
     name='maadsbml',
-    version='1.3.4',
+    version='1.3.5',
     description='Multi-Agent Accelerator for Data Science (MAADS) Batch AutoML',
     license='MIT License',
     packages=['maadsbml'],
     author='Sebastian Maurice',
     author_email='sebastian.maurice@otics.ca',
     keywords=['multi-agent, data science, batch automl, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence', 'predictive analytics', 'advanced analytics'],
     long_description=long_description,
```

