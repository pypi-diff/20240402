# Comparing `tmp/scratchcommunication-2.2.8.tar.gz` & `tmp/scratchcommunication-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchcommunication-2.2.8.tar", last modified: Thu Mar  7 17:22:00 2024, max compression
+gzip compressed data, was "scratchcommunication-2.2.9.tar", last modified: Fri Mar  8 09:26:59 2024, max compression
```

## Comparing `scratchcommunication-2.2.8.tar` & `scratchcommunication-2.2.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 17:22:00.569902 scratchcommunication-2.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-03-07 17:21:56.000000 scratchcommunication-2.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10576 2024-03-07 17:22:00.569902 scratchcommunication-2.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9746 2024-03-07 17:21:56.000000 scratchcommunication-2.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 17:22:00.565902 scratchcommunication-2.2.8/scratchcommunication/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-07 17:21:56.000000 scratchcommunication-2.2.8/scratchcommunication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14674 2024-03-07 17:21:56.000000 scratchcommunication-2.2.8/scratchcommunication/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    12292 2024-03-07 17:21:56.000000 scratchcommunication-2.2.8/scratchcommunication/cloud_socket.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-03-07 17:21:56.000000 scratchcommunication-2.2.8/scratchcommunication/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-07 17:21:56.000000 scratchcommunication-2.2.8/scratchcommunication/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-03-07 17:21:56.000000 scratchcommunication-2.2.8/scratchcommunication/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-03-07 17:21:56.000000 scratchcommunication-2.2.8/scratchcommunication/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 17:22:00.569902 scratchcommunication-2.2.8/scratchcommunication.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10576 2024-03-07 17:22:00.000000 scratchcommunication-2.2.8/scratchcommunication.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-03-07 17:22:00.000000 scratchcommunication-2.2.8/scratchcommunication.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 17:22:00.000000 scratchcommunication-2.2.8/scratchcommunication.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-07 17:22:00.000000 scratchcommunication-2.2.8/scratchcommunication.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-07 17:22:00.000000 scratchcommunication-2.2.8/scratchcommunication.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 17:22:00.569902 scratchcommunication-2.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-07 17:21:56.000000 scratchcommunication-2.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 09:26:59.156059 scratchcommunication-2.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-03-08 09:26:55.000000 scratchcommunication-2.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10576 2024-03-08 09:26:59.156059 scratchcommunication-2.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9746 2024-03-08 09:26:55.000000 scratchcommunication-2.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 09:26:59.156059 scratchcommunication-2.2.9/scratchcommunication/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-08 09:26:55.000000 scratchcommunication-2.2.9/scratchcommunication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14674 2024-03-08 09:26:55.000000 scratchcommunication-2.2.9/scratchcommunication/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12292 2024-03-08 09:26:55.000000 scratchcommunication-2.2.9/scratchcommunication/cloud_socket.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-03-08 09:26:55.000000 scratchcommunication-2.2.9/scratchcommunication/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-08 09:26:55.000000 scratchcommunication-2.2.9/scratchcommunication/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-03-08 09:26:55.000000 scratchcommunication-2.2.9/scratchcommunication/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-03-08 09:26:55.000000 scratchcommunication-2.2.9/scratchcommunication/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 09:26:59.156059 scratchcommunication-2.2.9/scratchcommunication.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10576 2024-03-08 09:26:59.000000 scratchcommunication-2.2.9/scratchcommunication.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-03-08 09:26:59.000000 scratchcommunication-2.2.9/scratchcommunication.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 09:26:59.000000 scratchcommunication-2.2.9/scratchcommunication.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-08 09:26:59.000000 scratchcommunication-2.2.9/scratchcommunication.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-08 09:26:59.000000 scratchcommunication-2.2.9/scratchcommunication.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 09:26:59.156059 scratchcommunication-2.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-08 09:26:55.000000 scratchcommunication-2.2.9/setup.py
```

### Comparing `scratchcommunication-2.2.8/LICENSE` & `scratchcommunication-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.2.8/PKG-INFO` & `scratchcommunication-2.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchcommunication
-Version: 2.2.8
+Version: 2.2.9
 Summary: A python module for communicating with scratch projects
 Home-page: https://github.com/thecommcraft/scratchcommunication
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchcommunication-2.2.8/README.md` & `scratchcommunication-2.2.9/README.md`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.2.8/scratchcommunication/cloud.py` & `scratchcommunication-2.2.9/scratchcommunication/cloud.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.2.8/scratchcommunication/cloud_socket.py` & `scratchcommunication-2.2.9/scratchcommunication/cloud_socket.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,15 +279,15 @@
     def __exit__(self, exc_type, exc_value, traceback):
         pass
     
     def _secure_send(self, data : str):
         """
         Use for sending data to the client if secure
         """
-        packets = ["".join(i) for i in batched(data, self.cloud_socket.packet_size // 2 - 15)]
+        packets = ["".join(i) for i in batched(data, self.cloud_socket.packet_size // 2 - 25)]
         packet_idx = 0
         for packet in packets[:-1]:
             salt = int(time.time() * 100)
             packet = self.cloud_socket._encode(self.encrypter.encrypt(packet, salt=salt))
             self.cloud_socket.cloud.set_variable(name=f"TO_CLIENT_{random.randint(1, 4)}", value=f"-{packet}{str(salt).zfill(15)}.{self.client_id}{packet_idx}")
             packet_idx += 1
         salt = int(time.time() * 100)
```

### Comparing `scratchcommunication-2.2.8/scratchcommunication/security.py` & `scratchcommunication-2.2.9/scratchcommunication/security.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.2.8/scratchcommunication/session.py` & `scratchcommunication-2.2.9/scratchcommunication/session.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.2.8/scratchcommunication.egg-info/PKG-INFO` & `scratchcommunication-2.2.9/scratchcommunication.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchcommunication
-Version: 2.2.8
+Version: 2.2.9
 Summary: A python module for communicating with scratch projects
 Home-page: https://github.com/thecommcraft/scratchcommunication
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchcommunication-2.2.8/setup.py` & `scratchcommunication-2.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='scratchcommunication',
-    version='2.2.8',
+    version='2.2.9',
     author='Simon Gilde',
     author_email='simon.c.gilde@gmail.com',
     description='A python module for communicating with scratch projects',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/thecommcraft/scratchcommunication',
     packages=find_packages(exclude=[]),
```

