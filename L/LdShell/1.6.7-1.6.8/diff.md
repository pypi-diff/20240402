# Comparing `tmp/LdShell-1.6.7.tar.gz` & `tmp/LdShell-1.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LdShell-1.6.7.tar", last modified: Mon Apr  1 09:42:50 2024, max compression
+gzip compressed data, was "LdShell-1.6.8.tar", last modified: Tue Apr  2 04:53:12 2024, max compression
```

## Comparing `LdShell-1.6.7.tar` & `LdShell-1.6.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 09:42:50.668486 LdShell-1.6.7/
--rw-rw-rw-   0        0        0     1060 2024-03-21 08:18:32.000000 LdShell-1.6.7/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-01 09:42:50.661913 LdShell-1.6.7/LdShell/
--rw-rw-rw-   0        0        0       20 2024-03-21 08:18:32.000000 LdShell-1.6.7/LdShell/__init__.py
--rw-rw-rw-   0        0        0      352 2024-03-21 08:18:32.000000 LdShell-1.6.7/LdShell/__version__.py
--rw-rw-rw-   0        0        0     8036 2024-04-01 09:40:54.000000 LdShell-1.6.7/LdShell/core.py
-drwxrwxrwx   0        0        0        0 2024-04-01 09:42:50.665816 LdShell-1.6.7/LdShell.egg-info/
--rw-rw-rw-   0        0        0     3038 2024-04-01 09:42:50.000000 LdShell-1.6.7/LdShell.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2024-04-01 09:42:50.000000 LdShell-1.6.7/LdShell.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 09:42:50.000000 LdShell-1.6.7/LdShell.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-01 09:42:50.000000 LdShell-1.6.7/LdShell.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       26 2024-03-21 08:18:32.000000 LdShell-1.6.7/MANIFEST.in
--rw-rw-rw-   0        0        0     3038 2024-04-01 09:42:50.667002 LdShell-1.6.7/PKG-INFO
--rw-rw-rw-   0        0        0     2338 2024-03-21 08:18:32.000000 LdShell-1.6.7/README.md
--rw-rw-rw-   0        0        0       42 2024-04-01 09:42:50.668486 LdShell-1.6.7/setup.cfg
--rw-rw-rw-   0        0        0     3767 2024-04-01 09:42:25.000000 LdShell-1.6.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:53:12.020937 LdShell-1.6.8/
+-rw-rw-rw-   0        0        0     1060 2024-03-21 08:18:32.000000 LdShell-1.6.8/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-02 04:53:12.016056 LdShell-1.6.8/LdShell/
+-rw-rw-rw-   0        0        0       20 2024-03-21 08:18:32.000000 LdShell-1.6.8/LdShell/__init__.py
+-rw-rw-rw-   0        0        0      352 2024-03-21 08:18:32.000000 LdShell-1.6.8/LdShell/__version__.py
+-rw-rw-rw-   0        0        0     8263 2024-04-02 04:50:28.000000 LdShell-1.6.8/LdShell/core.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:53:12.019960 LdShell-1.6.8/LdShell.egg-info/
+-rw-rw-rw-   0        0        0     3038 2024-04-02 04:53:11.000000 LdShell-1.6.8/LdShell.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2024-04-02 04:53:11.000000 LdShell-1.6.8/LdShell.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 04:53:11.000000 LdShell-1.6.8/LdShell.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-02 04:53:11.000000 LdShell-1.6.8/LdShell.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       26 2024-03-21 08:18:32.000000 LdShell-1.6.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     3038 2024-04-02 04:53:12.019960 LdShell-1.6.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2338 2024-03-21 08:18:32.000000 LdShell-1.6.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-02 04:53:12.020937 LdShell-1.6.8/setup.cfg
+-rw-rw-rw-   0        0        0     3767 2024-04-02 04:51:21.000000 LdShell-1.6.8/setup.py
```

### Comparing `LdShell-1.6.7/LICENSE` & `LdShell-1.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `LdShell-1.6.7/LdShell/core.py` & `LdShell-1.6.8/LdShell/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,16 +118,24 @@
     def Input(self,txt):
         self.input_text=txt
         return self.IniPost(LdType.Input)
 
     # 下面定义了一个Exists方法
     def Exists(self):
         return self.IniPost(LdType.Exists)
+    
+    # 下面定义了一个Wait方法
+    def Wait(self,timeout=30):
+        for a in range(timeout):
+            if self.IniPost(LdType.Exists):
+                return True
+            time.sleep(3)
+        return False
 
-    # 下面定义了一个Exists方法
+    # 下面定义了一个Checked方法
     def Checked(self):
         return self.IniPost(LdType.Checked)
 
     # 下面定义了一个 Swipe 方法
     def Swipe(self,xy):
         self.input_text=xy
         return self.IniPost(LdType.Swipe)
```

### Comparing `LdShell-1.6.7/LdShell.egg-info/PKG-INFO` & `LdShell-1.6.8/LdShell.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LdShell
-Version: 1.6.7
+Version: 1.6.8
 Summary: My short description for my project.
 Home-page: http://www.google.com/
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `LdShell-1.6.7/PKG-INFO` & `LdShell-1.6.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LdShell
-Version: 1.6.7
+Version: 1.6.8
 Summary: My short description for my project.
 Home-page: http://www.google.com/
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `LdShell-1.6.7/README.md` & `LdShell-1.6.8/README.md`

 * *Files identical despite different names*

### Comparing `LdShell-1.6.7/setup.py` & `LdShell-1.6.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'LdShell'
 DESCRIPTION = 'My short description for my project.'
 URL="http://www.google.com/"
 EMAIL = 'me@example.com'
 AUTHOR = 'Awesome Soul'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '1.6.7'
+VERSION = '1.6.8'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

