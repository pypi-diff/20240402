# Comparing `tmp/LdShell-2.0.0.tar.gz` & `tmp/LdShell-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LdShell-2.0.0.tar", last modified: Tue Apr  2 04:57:08 2024, max compression
+gzip compressed data, was "LdShell-2.0.1.tar", last modified: Tue Apr  2 05:17:54 2024, max compression
```

## Comparing `LdShell-2.0.0.tar` & `LdShell-2.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 04:57:08.577240 LdShell-2.0.0/
--rw-rw-rw-   0        0        0     1060 2024-03-21 08:18:32.000000 LdShell-2.0.0/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-02 04:57:08.572360 LdShell-2.0.0/LdShell/
--rw-rw-rw-   0        0        0       20 2024-03-21 08:18:32.000000 LdShell-2.0.0/LdShell/__init__.py
--rw-rw-rw-   0        0        0      352 2024-03-21 08:18:32.000000 LdShell-2.0.0/LdShell/__version__.py
--rw-rw-rw-   0        0        0     8263 2024-04-02 04:50:28.000000 LdShell-2.0.0/LdShell/core.py
-drwxrwxrwx   0        0        0        0 2024-04-02 04:57:08.575288 LdShell-2.0.0/LdShell.egg-info/
--rw-rw-rw-   0        0        0     3038 2024-04-02 04:57:08.000000 LdShell-2.0.0/LdShell.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2024-04-02 04:57:08.000000 LdShell-2.0.0/LdShell.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 04:57:08.000000 LdShell-2.0.0/LdShell.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-02 04:57:08.000000 LdShell-2.0.0/LdShell.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       26 2024-03-21 08:18:32.000000 LdShell-2.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3038 2024-04-02 04:57:08.576264 LdShell-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2338 2024-03-21 08:18:32.000000 LdShell-2.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-02 04:57:08.577240 LdShell-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     3767 2024-04-02 04:57:00.000000 LdShell-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 05:17:54.021877 LdShell-2.0.1/
+-rw-rw-rw-   0        0        0     1060 2024-03-21 08:18:32.000000 LdShell-2.0.1/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-02 05:17:54.015465 LdShell-2.0.1/LdShell/
+-rw-rw-rw-   0        0        0       20 2024-03-21 08:18:32.000000 LdShell-2.0.1/LdShell/__init__.py
+-rw-rw-rw-   0        0        0      352 2024-03-21 08:18:32.000000 LdShell-2.0.1/LdShell/__version__.py
+-rw-rw-rw-   0        0        0     8287 2024-04-02 05:16:25.000000 LdShell-2.0.1/LdShell/core.py
+drwxrwxrwx   0        0        0        0 2024-04-02 05:17:54.019924 LdShell-2.0.1/LdShell.egg-info/
+-rw-rw-rw-   0        0        0     3038 2024-04-02 05:17:53.000000 LdShell-2.0.1/LdShell.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2024-04-02 05:17:53.000000 LdShell-2.0.1/LdShell.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 05:17:53.000000 LdShell-2.0.1/LdShell.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-02 05:17:53.000000 LdShell-2.0.1/LdShell.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       26 2024-03-21 08:18:32.000000 LdShell-2.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3038 2024-04-02 05:17:54.020901 LdShell-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2338 2024-03-21 08:18:32.000000 LdShell-2.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-02 05:17:54.021877 LdShell-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     3767 2024-04-02 05:17:27.000000 LdShell-2.0.1/setup.py
```

### Comparing `LdShell-2.0.0/LICENSE` & `LdShell-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `LdShell-2.0.0/LdShell/core.py` & `LdShell-2.0.1/LdShell/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                 url = 'http://127.0.0.1:33221/ldshell/'
                 if(InitLdPlayer._debug):
                     print(url)
                     print(json.dumps(self.lds))
 
                 res = requests.post( url=url,data=json.dumps(self.lds),timeout=30)
                 if(InitLdPlayer._debug):
-                    print(res)
+                    print(json.dumps(res))
                 return bool(res.text)
             except Exception as e:
                 if(InitLdPlayer._debug):
                     print(e)
                 time.sleep(1)
                 pass
         return False;
@@ -96,15 +96,15 @@
 
                 if(InitLdPlayer._debug):
                     print(url)
                     print(json.dumps(self.lds))
                 res = requests.post(url=url,data=json.dumps(self.lds),timeout=30)
 
                 if(InitLdPlayer._debug):
-                    print(res)
+                    print(json.dumps(res))
                     
                 return res.text
             except Exception as e:
                 if(InitLdPlayer._debug):
                     print(e)
                 time.sleep(1)
                 pass
```

### Comparing `LdShell-2.0.0/LdShell.egg-info/PKG-INFO` & `LdShell-2.0.1/LdShell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LdShell
-Version: 2.0.0
+Version: 2.0.1
 Summary: My short description for my project.
 Home-page: http://www.google.com/
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `LdShell-2.0.0/PKG-INFO` & `LdShell-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LdShell
-Version: 2.0.0
+Version: 2.0.1
 Summary: My short description for my project.
 Home-page: http://www.google.com/
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `LdShell-2.0.0/README.md` & `LdShell-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `LdShell-2.0.0/setup.py` & `LdShell-2.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'LdShell'
 DESCRIPTION = 'My short description for my project.'
 URL="http://www.google.com/"
 EMAIL = 'me@example.com'
 AUTHOR = 'Awesome Soul'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '2.0.0'
+VERSION = '2.0.1'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

