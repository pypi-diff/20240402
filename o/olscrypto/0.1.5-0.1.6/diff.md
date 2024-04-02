# Comparing `tmp/olscrypto-0.1.5.tar.gz` & `tmp/olscrypto-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olscrypto-0.1.5.tar", last modified: Tue Feb 13 05:01:12 2024, max compression
+gzip compressed data, was "olscrypto-0.1.6.tar", last modified: Tue Apr  2 04:12:41 2024, max compression
```

## Comparing `olscrypto-0.1.5.tar` & `olscrypto-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 dirmich    (503) admin       (80)        0 2024-02-13 05:01:12.000000 olscrypto-0.1.5/
--rw-r--r--   0 dirmich    (503) admin       (80)      649 2024-02-13 05:01:12.000000 olscrypto-0.1.5/PKG-INFO
--rw-r--r--   0 dirmich    (503) admin       (80)      190 2024-02-13 05:01:01.000000 olscrypto-0.1.5/README.md
-drwxr-xr-x   0 dirmich    (503) admin       (80)        0 2024-02-13 05:01:12.000000 olscrypto-0.1.5/olscrypto/
--rw-r--r--   0 dirmich    (503) admin       (80)       41 2024-02-13 04:33:57.000000 olscrypto-0.1.5/olscrypto/__init__.py
--rw-r--r--   0 dirmich    (503) admin       (80)     1906 2024-01-09 07:25:48.000000 olscrypto-0.1.5/olscrypto/decryptor.py
-drwxr-xr-x   0 dirmich    (503) admin       (80)        0 2024-02-13 05:01:12.000000 olscrypto-0.1.5/olscrypto.egg-info/
--rw-r--r--   0 dirmich    (503) admin       (80)      649 2024-02-13 05:01:12.000000 olscrypto-0.1.5/olscrypto.egg-info/PKG-INFO
--rw-r--r--   0 dirmich    (503) admin       (80)      267 2024-02-13 05:01:12.000000 olscrypto-0.1.5/olscrypto.egg-info/SOURCES.txt
--rw-r--r--   0 dirmich    (503) admin       (80)        1 2024-02-13 05:01:12.000000 olscrypto-0.1.5/olscrypto.egg-info/dependency_links.txt
--rw-r--r--   0 dirmich    (503) admin       (80)        9 2024-02-13 05:01:12.000000 olscrypto-0.1.5/olscrypto.egg-info/requires.txt
--rw-r--r--   0 dirmich    (503) admin       (80)       16 2024-02-13 05:01:12.000000 olscrypto-0.1.5/olscrypto.egg-info/top_level.txt
--rw-r--r--   0 dirmich    (503) admin       (80)       38 2024-02-13 05:01:12.000000 olscrypto-0.1.5/setup.cfg
--rw-r--r--   0 dirmich    (503) admin       (80)      976 2024-02-13 05:01:08.000000 olscrypto-0.1.5/setup.py
-drwxr-xr-x   0 dirmich    (503) admin       (80)        0 2024-02-13 05:01:12.000000 olscrypto-0.1.5/tests/
--rw-r--r--   0 dirmich    (503) admin       (80)        0 2024-01-07 04:12:52.000000 olscrypto-0.1.5/tests/__init__.py
--rw-r--r--   0 dirmich    (503) admin       (80)       32 2024-01-09 07:25:14.000000 olscrypto-0.1.5/tests/test_decrypt.py
+drwxr-xr-x   0 dirmich    (503) admin       (80)        0 2024-04-02 04:12:41.000000 olscrypto-0.1.6/
+-rw-r--r--   0 dirmich    (503) admin       (80)      649 2024-04-02 04:12:41.000000 olscrypto-0.1.6/PKG-INFO
+-rw-r--r--   0 dirmich    (503) admin       (80)      190 2024-02-13 05:01:01.000000 olscrypto-0.1.6/README.md
+drwxr-xr-x   0 dirmich    (503) admin       (80)        0 2024-04-02 04:12:41.000000 olscrypto-0.1.6/olscrypto/
+-rw-r--r--   0 dirmich    (503) admin       (80)       41 2024-02-13 04:33:57.000000 olscrypto-0.1.6/olscrypto/__init__.py
+-rw-r--r--   0 dirmich    (503) admin       (80)     1927 2024-04-02 03:48:52.000000 olscrypto-0.1.6/olscrypto/decryptor.py
+drwxr-xr-x   0 dirmich    (503) admin       (80)        0 2024-04-02 04:12:41.000000 olscrypto-0.1.6/olscrypto.egg-info/
+-rw-r--r--   0 dirmich    (503) admin       (80)      649 2024-04-02 04:12:41.000000 olscrypto-0.1.6/olscrypto.egg-info/PKG-INFO
+-rw-r--r--   0 dirmich    (503) admin       (80)      249 2024-04-02 04:12:41.000000 olscrypto-0.1.6/olscrypto.egg-info/SOURCES.txt
+-rw-r--r--   0 dirmich    (503) admin       (80)        1 2024-04-02 04:12:41.000000 olscrypto-0.1.6/olscrypto.egg-info/dependency_links.txt
+-rw-r--r--   0 dirmich    (503) admin       (80)        9 2024-04-02 04:12:41.000000 olscrypto-0.1.6/olscrypto.egg-info/requires.txt
+-rw-r--r--   0 dirmich    (503) admin       (80)       10 2024-04-02 04:12:41.000000 olscrypto-0.1.6/olscrypto.egg-info/top_level.txt
+-rw-r--r--   0 dirmich    (503) admin       (80)       38 2024-04-02 04:12:41.000000 olscrypto-0.1.6/setup.cfg
+-rw-r--r--   0 dirmich    (503) admin       (80)      997 2024-04-02 04:12:38.000000 olscrypto-0.1.6/setup.py
+drwxr-xr-x   0 dirmich    (503) admin       (80)        0 2024-04-02 04:12:41.000000 olscrypto-0.1.6/tests/
+-rw-r--r--   0 dirmich    (503) admin       (80)       32 2024-01-09 07:25:14.000000 olscrypto-0.1.6/tests/test_decrypt.py
```

### Comparing `olscrypto-0.1.5/PKG-INFO` & `olscrypto-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olscrypto
-Version: 0.1.5
+Version: 0.1.6
 Summary: OLS decrypt library
 Author: Highmaru, Inc.
 Author-email: dhshin@highmaru.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `olscrypto-0.1.5/olscrypto/decryptor.py` & `olscrypto-0.1.6/olscrypto/decryptor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+import os
 from hashlib import sha256
 from Crypto import Random
 from Crypto.Cipher import AES
 import zipfile
 IV_LENGTH = 16
 ENCODING = 'utf-8'
 HEADER_LENGTH = 32
@@ -27,27 +28,30 @@
             enc = data
         # iv = enc[:IV_LENGTH]
         header = enc[:HEADER_LENGTH]
         iv = header[:IV_LENGTH]
         version = header[IV_LENGTH:]
         
         cipher = AES.new(self.key,AES.MODE_CBC, iv)
-        # decrypted = unpad(cipher.decrypt(enc[HEADER_LENGTH:]))
         decrypted = self.unpad(cipher.decrypt(enc[HEADER_LENGTH:]))
         print('iv',iv.hex(),len(iv))
         print('version',version.hex(),version.decode(),len(version))
         print('key',self.key.hex(),len(self.key))
-        # print('enc',enc[IV_LENGTH:].hex())
-        # print('dec',decrypted.hex())
-        # return decrypted.rstrip(b'\0').decode(ENCODING)
-        # return re.sub(b'\x00*$',b'',decrypted) #.decode(ENCODING)
         return decrypted
     
     def decryptfile(self,encrypted_input,outputfile):
         with open(encrypted_input,'rb') as file:
             ciphertext = file.read()
         decrypted = self.decrypt(ciphertext)
         with open(outputfile,'wb') as file:
             file.write(decrypted) #.encode(ENCODING))
     def unzip(self,file,path):
         with zipfile.ZipFile(file,'r') as zip:
             zip.extractall(path)
+    def decryptUnzip(self,encrypted_file,outpath):
+        try:
+            self.decryptfile(encrypted_file,'tmp.zip')
+            self.unzip('tmp.zip',outpath)
+            os.remove('tmp.zip')
+        except Exception as err:
+            print('Error:{}'.format(err))
+            raise
```

### Comparing `olscrypto-0.1.5/olscrypto.egg-info/PKG-INFO` & `olscrypto-0.1.6/olscrypto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olscrypto
-Version: 0.1.5
+Version: 0.1.6
 Summary: OLS decrypt library
 Author: Highmaru, Inc.
 Author-email: dhshin@highmaru.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `olscrypto-0.1.5/setup.py` & `olscrypto-0.1.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 DESCRIPTION = 'OLS decrypt library'
 setup(
     name='olscrypto',
-    packages=find_packages(),
-    version='0.1.5',
+    packages=find_packages(include=['olscrypto']),
+    version='0.1.6',
     author='Highmaru, Inc.',
     author_email="dhshin@highmaru.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     # setup_requires=['pytest-runner'],
     # tests_require=['pytest==4.4.1'],
```

