# Comparing `tmp/discogs_scraper-0.8.tar.gz` & `tmp/discogs_scraper-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discogs_scraper-0.8.tar", last modified: Sun Feb  4 17:49:39 2024, max compression
+gzip compressed data, was "discogs_scraper-0.9.tar", last modified: Sun Feb  4 18:00:58 2024, max compression
```

## Comparing `discogs_scraper-0.8.tar` & `discogs_scraper-0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 casperdancy   (501) staff       (20)        0 2024-02-04 17:49:39.247039 discogs_scraper-0.8/
--rw-r--r--   0 casperdancy   (501) staff       (20)     1116 2024-02-04 16:37:00.000000 discogs_scraper-0.8/LICENSE.txt
--rw-r--r--   0 casperdancy   (501) staff       (20)      781 2024-02-04 17:49:39.246754 discogs_scraper-0.8/PKG-INFO
--rw-r--r--   0 casperdancy   (501) staff       (20)      865 2024-02-04 16:48:11.000000 discogs_scraper-0.8/README.md
-drwxr-xr-x   0 casperdancy   (501) staff       (20)        0 2024-02-04 17:49:39.245734 discogs_scraper-0.8/discogs_scraper/
--rw-r--r--   0 casperdancy   (501) staff       (20)       46 2024-02-04 12:02:03.000000 discogs_scraper-0.8/discogs_scraper/__init__.py
--rw-r--r--   0 casperdancy   (501) staff       (20)     5366 2024-02-04 17:49:27.000000 discogs_scraper-0.8/discogs_scraper/discogScraper.py
-drwxr-xr-x   0 casperdancy   (501) staff       (20)        0 2024-02-04 17:49:39.246528 discogs_scraper-0.8/discogs_scraper.egg-info/
--rw-r--r--   0 casperdancy   (501) staff       (20)      781 2024-02-04 17:49:39.000000 discogs_scraper-0.8/discogs_scraper.egg-info/PKG-INFO
--rw-r--r--   0 casperdancy   (501) staff       (20)      285 2024-02-04 17:49:39.000000 discogs_scraper-0.8/discogs_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 casperdancy   (501) staff       (20)        1 2024-02-04 17:49:39.000000 discogs_scraper-0.8/discogs_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 casperdancy   (501) staff       (20)       15 2024-02-04 17:49:39.000000 discogs_scraper-0.8/discogs_scraper.egg-info/requires.txt
--rw-r--r--   0 casperdancy   (501) staff       (20)       16 2024-02-04 17:49:39.000000 discogs_scraper-0.8/discogs_scraper.egg-info/top_level.txt
--rw-r--r--   0 casperdancy   (501) staff       (20)       38 2024-02-04 17:49:39.247090 discogs_scraper-0.8/setup.cfg
--rw-r--r--   0 casperdancy   (501) staff       (20)     1540 2024-02-04 17:49:27.000000 discogs_scraper-0.8/setup.py
+drwxr-xr-x   0 casperdancy   (501) staff       (20)        0 2024-02-04 18:00:58.495632 discogs_scraper-0.9/
+-rw-r--r--   0 casperdancy   (501) staff       (20)     1116 2024-02-04 16:37:00.000000 discogs_scraper-0.9/LICENSE.txt
+-rw-r--r--   0 casperdancy   (501) staff       (20)      781 2024-02-04 18:00:58.495192 discogs_scraper-0.9/PKG-INFO
+-rw-r--r--   0 casperdancy   (501) staff       (20)      865 2024-02-04 16:48:11.000000 discogs_scraper-0.9/README.md
+drwxr-xr-x   0 casperdancy   (501) staff       (20)        0 2024-02-04 18:00:58.492341 discogs_scraper-0.9/discogs_scraper/
+-rw-r--r--   0 casperdancy   (501) staff       (20)       46 2024-02-04 12:02:03.000000 discogs_scraper-0.9/discogs_scraper/__init__.py
+-rw-r--r--   0 casperdancy   (501) staff       (20)     5444 2024-02-04 18:00:56.000000 discogs_scraper-0.9/discogs_scraper/discogScraper.py
+drwxr-xr-x   0 casperdancy   (501) staff       (20)        0 2024-02-04 18:00:58.494474 discogs_scraper-0.9/discogs_scraper.egg-info/
+-rw-r--r--   0 casperdancy   (501) staff       (20)      781 2024-02-04 18:00:58.000000 discogs_scraper-0.9/discogs_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 casperdancy   (501) staff       (20)      285 2024-02-04 18:00:58.000000 discogs_scraper-0.9/discogs_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 casperdancy   (501) staff       (20)        1 2024-02-04 18:00:58.000000 discogs_scraper-0.9/discogs_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 casperdancy   (501) staff       (20)       15 2024-02-04 18:00:58.000000 discogs_scraper-0.9/discogs_scraper.egg-info/requires.txt
+-rw-r--r--   0 casperdancy   (501) staff       (20)       16 2024-02-04 18:00:58.000000 discogs_scraper-0.9/discogs_scraper.egg-info/top_level.txt
+-rw-r--r--   0 casperdancy   (501) staff       (20)       38 2024-02-04 18:00:58.495750 discogs_scraper-0.9/setup.cfg
+-rw-r--r--   0 casperdancy   (501) staff       (20)     1540 2024-02-04 18:00:56.000000 discogs_scraper-0.9/setup.py
```

### Comparing `discogs_scraper-0.8/LICENSE.txt` & `discogs_scraper-0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `discogs_scraper-0.8/PKG-INFO` & `discogs_scraper-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discogs_scraper
-Version: 0.8
+Version: 0.9
 Summary: Scrapes discogs website based on urls and then outputs csv
 Home-page: https://github.com/casperUoS/discogs-Scraper
 Download-URL: https://github.com/casperUoS/discogs-Scraper/archive/refs/tags/0.7.tar.gz
 Author: Casper Dancy
 Author-email: casperdancy@gmail.com
 License: MIT
 Keywords: SOME,MEANINGFULL,KEYWORDS
```

### Comparing `discogs_scraper-0.8/README.md` & `discogs_scraper-0.9/README.md`

 * *Files identical despite different names*

### Comparing `discogs_scraper-0.8/discogs_scraper/discogScraper.py` & `discogs_scraper-0.9/discogs_scraper/discogScraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,19 @@
     f = open(fileName,"r")
     lines = f.readlines()
     f.close()
     releases = []
     sub1 = "release/"
     sub2 = "-"
     for line in lines:
-        id = ''.join(line.split(sub1)[1].split(sub2)[0])
-        releases.append(dis.release(id))
+        if len(line.strip()) == 0 :
+            id = ""
+        else:
+            id = ''.join(line.split(sub1)[1].split(sub2)[0])
+            releases.append(dis.release(id))
     return releases
 
 
 def getTracks1(release):
     tracks = ""
     if int(release.formats[0]['qty']) > 1:
         tracks += release.formats[0]['name'] + "1: "
```

### Comparing `discogs_scraper-0.8/discogs_scraper.egg-info/PKG-INFO` & `discogs_scraper-0.9/discogs_scraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discogs_scraper
-Version: 0.8
+Version: 0.9
 Summary: Scrapes discogs website based on urls and then outputs csv
 Home-page: https://github.com/casperUoS/discogs-Scraper
 Download-URL: https://github.com/casperUoS/discogs-Scraper/archive/refs/tags/0.7.tar.gz
 Author: Casper Dancy
 Author-email: casperdancy@gmail.com
 License: MIT
 Keywords: SOME,MEANINGFULL,KEYWORDS
```

### Comparing `discogs_scraper-0.8/setup.py` & `discogs_scraper-0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 from setuptools import setup
 
 setup(
   name = 'discogs_scraper',
   packages= ['discogs_scraper'],# How you named your package folder (MyLib)
-  version = '0.8',      # Start with a small number and increase it with every change you make
+  version = '0.9',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Scrapes discogs website based on urls and then outputs csv',   # Give a short description about your library
   author = 'Casper Dancy',                   # Type in your name
   author_email = 'casperdancy@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/casperUoS/discogs-Scraper',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/casperUoS/discogs-Scraper/archive/refs/tags/0.7.tar.gz',
   keywords = ['SOME', 'MEANINGFULL', 'KEYWORDS'],   # Keywords that define your package best
```

