# Comparing `tmp/ncm-0.0.29.tar.gz` & `tmp/ncm-0.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncm-0.0.29.tar", last modified: Mon Apr  1 16:34:15 2024, max compression
+gzip compressed data, was "ncm-0.0.30.tar", last modified: Mon Apr  1 16:51:03 2024, max compression
```

## Comparing `ncm-0.0.29.tar` & `ncm-0.0.30.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)        0 2024-04-01 16:34:15.946784 ncm-0.0.29/
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)     1083 2024-04-01 16:31:07.000000 ncm-0.0.29/LICENSE
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)     2304 2024-04-01 16:34:15.946784 ncm-0.0.29/PKG-INFO
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)     1932 2024-04-01 16:31:07.000000 ncm-0.0.29/README.md
-drwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)        0 2024-04-01 16:34:15.945784 ncm-0.0.29/ncm/
--rwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)        0 2024-04-01 16:31:07.000000 ncm-0.0.29/ncm/__init__.py
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)   149446 2024-04-01 16:31:07.000000 ncm-0.0.29/ncm/ncm.py
-drwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)        0 2024-04-01 16:34:15.946784 ncm-0.0.29/ncm.egg-info/
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)     2304 2024-04-01 16:34:15.000000 ncm-0.0.29/ncm.egg-info/PKG-INFO
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)      187 2024-04-01 16:34:15.000000 ncm-0.0.29/ncm.egg-info/SOURCES.txt
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)        1 2024-04-01 16:34:15.000000 ncm-0.0.29/ncm.egg-info/dependency_links.txt
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)       17 2024-04-01 16:34:15.000000 ncm-0.0.29/ncm.egg-info/requires.txt
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)        4 2024-04-01 16:34:15.000000 ncm-0.0.29/ncm.egg-info/top_level.txt
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)       38 2024-04-01 16:34:15.946784 ncm-0.0.29/setup.cfg
--rwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)      590 2024-04-01 16:32:08.000000 ncm-0.0.29/setup.py
+drwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)        0 2024-04-01 16:51:03.696205 ncm-0.0.30/
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)     1083 2024-04-01 16:31:07.000000 ncm-0.0.30/LICENSE
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)     2316 2024-04-01 16:51:03.696205 ncm-0.0.30/PKG-INFO
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)     1932 2024-04-01 16:31:07.000000 ncm-0.0.30/README.md
+drwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)        0 2024-04-01 16:51:03.695204 ncm-0.0.30/ncm/
+-rwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)        0 2024-04-01 16:31:07.000000 ncm-0.0.30/ncm/__init__.py
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)   150110 2024-04-01 16:50:10.000000 ncm-0.0.30/ncm/ncm.py
+drwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)        0 2024-04-01 16:51:03.696205 ncm-0.0.30/ncm.egg-info/
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)     2316 2024-04-01 16:51:03.000000 ncm-0.0.30/ncm.egg-info/PKG-INFO
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)      187 2024-04-01 16:51:03.000000 ncm-0.0.30/ncm.egg-info/SOURCES.txt
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)        1 2024-04-01 16:51:03.000000 ncm-0.0.30/ncm.egg-info/dependency_links.txt
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)       17 2024-04-01 16:51:03.000000 ncm-0.0.30/ncm.egg-info/requires.txt
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)        4 2024-04-01 16:51:03.000000 ncm-0.0.30/ncm.egg-info/top_level.txt
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)       38 2024-04-01 16:51:03.696205 ncm-0.0.30/setup.cfg
+-rwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)      602 2024-04-01 16:50:10.000000 ncm-0.0.30/setup.py
```

### Comparing `ncm-0.0.29/LICENSE` & `ncm-0.0.30/LICENSE`

 * *Files identical despite different names*

### Comparing `ncm-0.0.29/PKG-INFO` & `ncm-0.0.30/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ncm
-Version: 0.0.29
+Version: 0.0.30
 Summary: Python client library for Cradlepoint NCM API
-Home-page: https://github.com/cradlepoint/api-samples/ncm
+Home-page: https://github.com/cradlepoint/api-samples/tree/master/ncm
 Author: Nathan Wiens - Cradlepoint
 Author-email: nathan.wiens@cradlepoint.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: urllib3
```

### Comparing `ncm-0.0.29/README.md` & `ncm-0.0.30/README.md`

 * *Files identical despite different names*

### Comparing `ncm-0.0.29/ncm/ncm.py` & `ncm-0.0.30/ncm/ncm.py`

 * *Files 1% similar despite different names*

```diff
@@ -568,14 +568,32 @@
 
         ncm = self.session.patch(
             '{0}/groups/{1}/'.format(self.base_url, str(group_id)),
             data=json.dumps(payload))  # Patch indie config with new values
         result = self._return_handler(ncm.status_code, ncm.text, call_type)
         return result
 
+    def put_group_configuration(self, group_id, config_json):
+        """
+        This method puts a group configuration for associated group id.
+        :param group_id: ID of group to update
+        :param config_json: JSON of the "configuration" field of the
+          group config
+        :return:
+        """
+        call_type = 'Configuration Manager'
+
+        payload = config_json
+
+        ncm = self.session.put(
+            '{0}/groups/{1}/'.format(self.base_url, str(group_id)),
+            data=json.dumps(payload))  # put group config with new values
+        result = self.__return_handler(ncm.status_code, ncm.text, call_type)
+        return result
+
     def copy_router_configuration(self, src_router_id, dst_router_id):
         """
         Copies the Configuration Manager config of one router to another.
         This function will not copy any passwords as they are encrypted.
         :param src_router_id: Router ID to copy from
         :param dst_router_id: Router ID to copy to
         :return: Should return HTTP Status Code 202 if successful
```

### Comparing `ncm-0.0.29/ncm.egg-info/PKG-INFO` & `ncm-0.0.30/ncm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ncm
-Version: 0.0.29
+Version: 0.0.30
 Summary: Python client library for Cradlepoint NCM API
-Home-page: https://github.com/cradlepoint/api-samples/ncm
+Home-page: https://github.com/cradlepoint/api-samples/tree/master/ncm
 Author: Nathan Wiens - Cradlepoint
 Author-email: nathan.wiens@cradlepoint.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: urllib3
```

### Comparing `ncm-0.0.29/setup.py` & `ncm-0.0.30/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="ncm",
-    version="0.0.29",
+    version="0.0.30",
     author="Nathan Wiens - Cradlepoint",
     author_email="nathan.wiens@cradlepoint.com",
     description="Python client library for Cradlepoint NCM API",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/cradlepoint/api-samples/ncm",
+    url="https://github.com/cradlepoint/api-samples/tree/master/ncm",
     packages=find_packages(),
     python_requires='>=3.6',
     install_requires=[
         'requests',
         'urllib3'
     ]
 )
```

