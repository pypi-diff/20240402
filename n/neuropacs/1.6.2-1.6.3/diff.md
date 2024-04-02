# Comparing `tmp/neuropacs-1.6.2.tar.gz` & `tmp/neuropacs-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuropacs-1.6.2.tar", last modified: Fri Mar 22 06:08:58 2024, max compression
+gzip compressed data, was "neuropacs-1.6.3.tar", last modified: Tue Apr  2 17:42:49 2024, max compression
```

## Comparing `neuropacs-1.6.2.tar` & `neuropacs-1.6.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-03-22 06:08:58.312586 neuropacs-1.6.2/
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     1061 2024-02-21 03:24:17.000000 neuropacs-1.6.2/LICENSE
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     2708 2024-03-22 06:08:58.312367 neuropacs-1.6.2/PKG-INFO
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     1708 2024-01-04 01:45:39.000000 neuropacs-1.6.2/README.md
-drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-03-22 06:08:58.309717 neuropacs-1.6.2/examples/
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)        0 2023-12-24 02:20:58.000000 neuropacs-1.6.2/examples/__init__.py
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)      906 2024-03-22 02:24:38.000000 neuropacs-1.6.2/examples/example1.py
-drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-03-22 06:08:58.310450 neuropacs-1.6.2/neuropacs/
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)      163 2024-03-22 06:08:56.000000 neuropacs-1.6.2/neuropacs/__init__.py
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     1116 2024-03-22 02:24:02.000000 neuropacs-1.6.2/neuropacs/ex.py
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)    19920 2024-03-22 06:08:48.000000 neuropacs-1.6.2/neuropacs/sdk.py
-drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-03-22 06:08:58.312092 neuropacs-1.6.2/neuropacs.egg-info/
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     2708 2024-03-22 06:08:58.000000 neuropacs-1.6.2/neuropacs.egg-info/PKG-INFO
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)      330 2024-03-22 06:08:58.000000 neuropacs-1.6.2/neuropacs.egg-info/SOURCES.txt
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)        1 2024-03-22 06:08:58.000000 neuropacs-1.6.2/neuropacs.egg-info/dependency_links.txt
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)      285 2024-03-22 06:08:58.000000 neuropacs-1.6.2/neuropacs.egg-info/requires.txt
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)       25 2024-03-22 06:08:58.000000 neuropacs-1.6.2/neuropacs.egg-info/top_level.txt
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)       38 2024-03-22 06:08:58.312628 neuropacs-1.6.2/setup.cfg
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     1346 2024-03-22 06:08:51.000000 neuropacs-1.6.2/setup.py
-drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-03-22 06:08:58.311692 neuropacs-1.6.2/tests/
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)        0 2023-12-09 22:18:09.000000 neuropacs-1.6.2/tests/__init__.py
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)    26402 2024-01-06 03:43:44.000000 neuropacs-1.6.2/tests/tests_neuropacs.py
+drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-04-02 17:42:49.949125 neuropacs-1.6.3/
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     1061 2024-02-21 03:24:17.000000 neuropacs-1.6.3/LICENSE
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     2708 2024-04-02 17:42:49.948851 neuropacs-1.6.3/PKG-INFO
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     1708 2024-01-04 01:45:39.000000 neuropacs-1.6.3/README.md
+drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-04-02 17:42:49.945361 neuropacs-1.6.3/examples/
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)        0 2023-12-24 02:20:58.000000 neuropacs-1.6.3/examples/__init__.py
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)      970 2024-03-28 21:09:19.000000 neuropacs-1.6.3/examples/example1.py
+drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-04-02 17:42:49.946620 neuropacs-1.6.3/neuropacs/
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)      163 2024-04-02 17:42:19.000000 neuropacs-1.6.3/neuropacs/__init__.py
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     1323 2024-04-02 17:36:41.000000 neuropacs-1.6.3/neuropacs/ex.py
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)    19930 2024-04-02 17:40:09.000000 neuropacs-1.6.3/neuropacs/sdk.py
+drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-04-02 17:42:49.948485 neuropacs-1.6.3/neuropacs.egg-info/
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     2708 2024-04-02 17:42:49.000000 neuropacs-1.6.3/neuropacs.egg-info/PKG-INFO
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)      330 2024-04-02 17:42:49.000000 neuropacs-1.6.3/neuropacs.egg-info/SOURCES.txt
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)        1 2024-04-02 17:42:49.000000 neuropacs-1.6.3/neuropacs.egg-info/dependency_links.txt
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)      285 2024-04-02 17:42:49.000000 neuropacs-1.6.3/neuropacs.egg-info/requires.txt
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)       25 2024-04-02 17:42:49.000000 neuropacs-1.6.3/neuropacs.egg-info/top_level.txt
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)       38 2024-04-02 17:42:49.949178 neuropacs-1.6.3/setup.cfg
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     1346 2024-04-02 17:42:15.000000 neuropacs-1.6.3/setup.py
+drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-04-02 17:42:49.948031 neuropacs-1.6.3/tests/
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)        0 2023-12-09 22:18:09.000000 neuropacs-1.6.3/tests/__init__.py
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)    26402 2024-01-06 03:43:44.000000 neuropacs-1.6.3/tests/tests_neuropacs.py
```

### Comparing `neuropacs-1.6.2/LICENSE` & `neuropacs-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `neuropacs-1.6.2/PKG-INFO` & `neuropacs-1.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuropacs
-Version: 1.6.2
+Version: 1.6.3
 Summary: NeuroPACS Python SDK
 Home-page: https://github.com/neuropacs/neuropacs-py-sdk
 Author: Kerrick Cavanaugh
 Author-email: kerrick@neuropacs.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `neuropacs-1.6.2/README.md` & `neuropacs-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `neuropacs-1.6.2/examples/example1.py` & `neuropacs-1.6.3/examples/example1.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,24 +17,27 @@
 
     # CREATE A CONNECTION   
     conn = npcs.connect()
     print(conn)
 
     # # # CREATE A NEW JOB
     order = npcs.new_job()
-    print(order)
+    # print(order)
 
-    # # UPLOAD A DATASET
-    datasetID = npcs.upload_dataset("../dicom_examples/DICOM_small")
-    print(datasetID)
+    # # # UPLOAD A DATASET
+    # datasetID = npcs.upload_dataset("../dicom_examples/DICOM_small")
+    # print(datasetID)
 
     # # START A JOB
-    # job = npcs.run_job(product_id)
+    job = npcs.run_job(product_id)
+    print(job)
 
     # # CHECK STATUS
     # status = npcs.check_status("TEST")
+    # print(status)
 
-    # # GET RESULTS
+    # # # GET RESULTS
     # results = npcs.get_results(result_format, "TEST")
+    # print(results)
 
 
 main()
```

### Comparing `neuropacs-1.6.2/neuropacs/sdk.py` & `neuropacs-1.6.3/neuropacs/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,15 +293,15 @@
             total_files = sum(len(filenames) for _, _, filenames in os.walk(directory))
 
             with tqdm(total=total_files, desc="Uploading", unit="file") as prog_bar:
                 for dirpath, _, filenames in os.walk(directory):
                     for filename in filenames:
                         file_path = os.path.join(dirpath, filename)
                         status = self.upload(file_path, hex_dig, order_id, connection_id)
-                        if status is not 201:
+                        if status != 201:
                             raise Exception({"neuropacsError": "Upload failed!"})
                         prog_bar.update(1)  # Update the outer progress bar for each file
             
             return hex_dig
 
         except Exception as e:
             if(isinstance(e.args[0], dict) and 'neuropacsError' in e.args[0]):
@@ -465,14 +465,16 @@
                     'productID': product_id,
                     'datasetID': dataset_id
                 }
 
             encryptedBody = self.__encrypt_aes_ctr(body, "json", "string")
 
             res = requests.post(f"{self.server_url}/api/runJob/", data=encryptedBody, headers=headers)
+
+            print(res.text)
             
             if not res.ok:
                 raise Exception({"neuropacsError": f"{res.text}"})
 
             return res.status_code
                 
         except Exception as e:
@@ -500,15 +502,15 @@
         try:
 
             headers = {'Content-type': 'text/plain', 'connection-id': connection_id, 'client': self.client}
 
             if dataset_id is not None:
                 body = {
                     'orderID': order_id,
-                    'dataset_id': dataset_id
+                    'datasetID': dataset_id
                 }
             else:
                body = {
                     'orderID': order_id,
                 }
 
 
@@ -524,15 +526,14 @@
             return json
             
         except Exception as e:
             if(isinstance(e.args[0], dict) and 'neuropacsError' in e.args[0]):
                 raise Exception(e.args[0]['neuropacsError'])
             else:
                 raise Exception("Status check failed.")  
-            
 
 
     def get_results(self, format, order_id=None, dataset_id=None, connection_id=None):
         """Get job results
 
         :param str format: Format of file data
         :prarm str order_id: Base64 order_id (optional)
@@ -551,15 +552,15 @@
         
             headers = {'Content-type': 'text/plain', 'connection-id': connection_id, 'client': self.client}
 
             if dataset_id is not None:
                 body = {
                     'orderID': order_id,
                     'format': format,
-                    'dataset_id': dataset_id
+                    'datasetID': dataset_id
                 }
             else:
                 body = {
                     'orderID': order_id,
                     'format': format               
                 }
```

### Comparing `neuropacs-1.6.2/neuropacs.egg-info/PKG-INFO` & `neuropacs-1.6.3/neuropacs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuropacs
-Version: 1.6.2
+Version: 1.6.3
 Summary: NeuroPACS Python SDK
 Home-page: https://github.com/neuropacs/neuropacs-py-sdk
 Author: Kerrick Cavanaugh
 Author-email: kerrick@neuropacs.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `neuropacs-1.6.2/setup.py` & `neuropacs-1.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='neuropacs',
-    version='1.6.2',
+    version='1.6.3',
     description='NeuroPACS Python SDK',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Kerrick Cavanaugh',
     author_email='kerrick@neuropacs.com',
     url='https://github.com/neuropacs/neuropacs-py-sdk',
     packages=find_packages(),
```

### Comparing `neuropacs-1.6.2/tests/tests_neuropacs.py` & `neuropacs-1.6.3/tests/tests_neuropacs.py`

 * *Files identical despite different names*

