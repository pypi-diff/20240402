# Comparing `tmp/ctqkit-0.1.1b1.tar.gz` & `tmp/ctqkit-0.1.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctqkit-0.1.1b1.tar", max compression
+gzip compressed data, was "ctqkit-0.1.1b2.tar", max compression
```

## Comparing `ctqkit-0.1.1b1.tar` & `ctqkit-0.1.1b2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1060 2024-03-05 02:31:31.872856 ctqkit-0.1.1b1/LICENSE.txt
--rw-r--r--   0        0        0      946 2024-04-02 10:39:49.758673 ctqkit-0.1.1b1/pyproject.toml
--rw-r--r--   0        0        0       42 2024-03-04 09:21:32.455518 ctqkit-0.1.1b1/README.md
--rw-r--r--   0        0        0       62 2024-03-28 02:46:26.350830 ctqkit-0.1.1b1/src/CtqKit/__init__.py
--rw-r--r--   0        0        0     2919 2024-04-02 07:04:18.419446 ctqkit-0.1.1b1/src/CtqKit/account.py
--rw-r--r--   0        0        0    31261 2024-04-02 09:57:49.463053 ctqkit-0.1.1b1/src/CtqKit/platform.py
--rw-r--r--   0        0        0      806 1970-01-01 00:00:00.000000 ctqkit-0.1.1b1/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-03-05 02:31:31.872856 ctqkit-0.1.1b2/LICENSE.txt
+-rw-r--r--   0        0        0      946 2024-04-02 11:09:13.415422 ctqkit-0.1.1b2/pyproject.toml
+-rw-r--r--   0        0        0       42 2024-03-04 09:21:32.455518 ctqkit-0.1.1b2/README.md
+-rw-r--r--   0        0        0       62 2024-03-28 02:46:26.350830 ctqkit-0.1.1b2/src/CtqKit/__init__.py
+-rw-r--r--   0        0        0     2919 2024-04-02 07:04:18.419446 ctqkit-0.1.1b2/src/CtqKit/account.py
+-rw-r--r--   0        0        0    31196 2024-04-02 11:09:06.105188 ctqkit-0.1.1b2/src/CtqKit/platform.py
+-rw-r--r--   0        0        0      806 1970-01-01 00:00:00.000000 ctqkit-0.1.1b2/PKG-INFO
```

### Comparing `ctqkit-0.1.1b1/LICENSE.txt` & `ctqkit-0.1.1b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ctqkit-0.1.1b1/pyproject.toml` & `ctqkit-0.1.1b2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "CtqKit"
-version = "0.1.1-beta.1"
+version = "0.1.1-beta.2"
 description = "中国电信天衍量子计算云平台 Python SDK (ChinaTelecom Quantum Kit)"
 authors = ["Gao Jianjian <jianjian001@outlook.com>"]
 readme = "README.md"
 license = "MIT"
 documentation = "https://qc.zdxlz.com/informationSpace"
 homepage = "https://qc.zdxlz.com/"
 classifiers = [
```

### Comparing `ctqkit-0.1.1b1/src/CtqKit/account.py` & `ctqkit-0.1.1b2/src/CtqKit/account.py`

 * *Files identical despite different names*

### Comparing `ctqkit-0.1.1b1/src/CtqKit/platform.py` & `ctqkit-0.1.1b2/src/CtqKit/platform.py`

 * *Files 2% similar despite different names*

```diff
@@ -290,16 +290,15 @@
     def _run_experiment(self, data):
         """
         提交任务，并运行
 
         :param data:
         :return:
         """
-        # url = f'{self.account.base_url}/qccp-quantum/experiment/sdkCommit'
-        url = f'{self.account.base_url}/experiment/sdkCommit'
+        url = f'{self.account.base_url}/qccp-quantum/experiment/sdkCommit'
         headers = {
             "Authorization": f'Bearer {self.account.access_token}',
             'ApiCode': 'commit',
             'RequestTime': datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
         }
         res = requests.post(url, json=data, headers=headers)
         status_code = res.status_code
```

### Comparing `ctqkit-0.1.1b1/PKG-INFO` & `ctqkit-0.1.1b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CtqKit
-Version: 0.1.1b1
+Version: 0.1.1b2
 Summary: 中国电信天衍量子计算云平台 Python SDK (ChinaTelecom Quantum Kit)
 Home-page: https://qc.zdxlz.com/
 License: MIT
 Author: Gao Jianjian
 Author-email: jianjian001@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

