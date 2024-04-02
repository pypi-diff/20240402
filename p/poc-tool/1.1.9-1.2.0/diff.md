# Comparing `tmp/poc_tool-1.1.9.tar.gz` & `tmp/poc_tool-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poc_tool-1.1.9.tar", last modified: Fri Mar  1 05:55:20 2024, max compression
+gzip compressed data, was "poc_tool-1.2.0.tar", last modified: Tue Apr  2 05:27:08 2024, max compression
```

## Comparing `poc_tool-1.1.9.tar` & `poc_tool-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 zhizhuo    (501) staff       (20)        0 2024-03-01 05:55:20.576994 poc_tool-1.1.9/
--rw-r--r--   0 zhizhuo    (501) staff       (20)     1062 2023-08-10 21:52:31.000000 poc_tool-1.1.9/LICENSE.txt
--rw-r--r--   0 zhizhuo    (501) staff       (20)     2311 2024-03-01 05:55:20.576928 poc_tool-1.1.9/PKG-INFO
--rw-r--r--   0 zhizhuo    (501) staff       (20)     1919 2024-03-01 05:54:16.000000 poc_tool-1.1.9/README.md
-drwxr-xr-x   0 zhizhuo    (501) staff       (20)        0 2024-03-01 05:55:20.573654 poc_tool-1.1.9/poc_tool/
--rw-r--r--   0 zhizhuo    (501) staff       (20)      200 2024-03-01 05:18:35.000000 poc_tool-1.1.9/poc_tool/__init__.py
-drwxr-xr-x   0 zhizhuo    (501) staff       (20)        0 2024-03-01 05:55:20.574757 poc_tool-1.1.9/poc_tool/log/
--rw-r--r--   0 zhizhuo    (501) staff       (20)      187 2023-11-17 04:58:06.000000 poc_tool-1.1.9/poc_tool/log/__init__.py
--rw-r--r--   0 zhizhuo    (501) staff       (20)     2660 2023-11-17 05:05:43.000000 poc_tool-1.1.9/poc_tool/log/logger.py
-drwxr-xr-x   0 zhizhuo    (501) staff       (20)        0 2024-03-01 05:55:20.576209 poc_tool-1.1.9/poc_tool/tools/
--rw-r--r--   0 zhizhuo    (501) staff       (20)    13010 2024-03-01 05:47:16.000000 poc_tool-1.1.9/poc_tool/tools/Tools.py
--rw-r--r--   0 zhizhuo    (501) staff       (20)      165 2024-03-01 05:18:22.000000 poc_tool-1.1.9/poc_tool/tools/__init__.py
-drwxr-xr-x   0 zhizhuo    (501) staff       (20)        0 2024-03-01 05:55:20.574392 poc_tool-1.1.9/poc_tool.egg-info/
--rw-r--r--   0 zhizhuo    (501) staff       (20)     2311 2024-03-01 05:55:20.000000 poc_tool-1.1.9/poc_tool.egg-info/PKG-INFO
--rw-r--r--   0 zhizhuo    (501) staff       (20)      319 2024-03-01 05:55:20.000000 poc_tool-1.1.9/poc_tool.egg-info/SOURCES.txt
--rw-r--r--   0 zhizhuo    (501) staff       (20)        1 2024-03-01 05:55:20.000000 poc_tool-1.1.9/poc_tool.egg-info/dependency_links.txt
--rw-r--r--   0 zhizhuo    (501) staff       (20)       18 2024-03-01 05:55:20.000000 poc_tool-1.1.9/poc_tool.egg-info/requires.txt
--rw-r--r--   0 zhizhuo    (501) staff       (20)        9 2024-03-01 05:55:20.000000 poc_tool-1.1.9/poc_tool.egg-info/top_level.txt
--rw-r--r--   0 zhizhuo    (501) staff       (20)       79 2024-03-01 05:55:20.577244 poc_tool-1.1.9/setup.cfg
--rw-r--r--   0 zhizhuo    (501) staff       (20)      740 2024-03-01 05:55:02.000000 poc_tool-1.1.9/setup.py
+drwxr-xr-x   0 zhizhuo    (501) staff       (20)        0 2024-04-02 05:27:08.683754 poc_tool-1.2.0/
+-rw-r--r--   0 zhizhuo    (501) staff       (20)     1062 2023-08-10 21:52:31.000000 poc_tool-1.2.0/LICENSE.txt
+-rw-r--r--   0 zhizhuo    (501) staff       (20)     2800 2024-04-02 05:27:08.683658 poc_tool-1.2.0/PKG-INFO
+-rw-r--r--   0 zhizhuo    (501) staff       (20)     2354 2024-04-02 05:21:55.000000 poc_tool-1.2.0/README.md
+drwxr-xr-x   0 zhizhuo    (501) staff       (20)        0 2024-04-02 05:27:08.678860 poc_tool-1.2.0/poc_tool/
+-rw-r--r--   0 zhizhuo    (501) staff       (20)      226 2024-04-02 05:09:40.000000 poc_tool-1.2.0/poc_tool/__init__.py
+drwxr-xr-x   0 zhizhuo    (501) staff       (20)        0 2024-04-02 05:27:08.682353 poc_tool-1.2.0/poc_tool/log/
+-rw-r--r--   0 zhizhuo    (501) staff       (20)      187 2023-11-17 04:58:06.000000 poc_tool-1.2.0/poc_tool/log/__init__.py
+-rw-r--r--   0 zhizhuo    (501) staff       (20)     2660 2023-11-17 05:05:43.000000 poc_tool-1.2.0/poc_tool/log/logger.py
+drwxr-xr-x   0 zhizhuo    (501) staff       (20)        0 2024-04-02 05:27:08.683250 poc_tool-1.2.0/poc_tool/tools/
+-rw-r--r--   0 zhizhuo    (501) staff       (20)     1356 2024-04-02 05:25:31.000000 poc_tool-1.2.0/poc_tool/tools/HexDump.py
+-rw-r--r--   0 zhizhuo    (501) staff       (20)    13015 2024-04-02 05:03:39.000000 poc_tool-1.2.0/poc_tool/tools/Tools.py
+-rw-r--r--   0 zhizhuo    (501) staff       (20)      195 2024-04-02 05:09:47.000000 poc_tool-1.2.0/poc_tool/tools/__init__.py
+drwxr-xr-x   0 zhizhuo    (501) staff       (20)        0 2024-04-02 05:27:08.681994 poc_tool-1.2.0/poc_tool.egg-info/
+-rw-r--r--   0 zhizhuo    (501) staff       (20)     2800 2024-04-02 05:27:08.000000 poc_tool-1.2.0/poc_tool.egg-info/PKG-INFO
+-rw-r--r--   0 zhizhuo    (501) staff       (20)      345 2024-04-02 05:27:08.000000 poc_tool-1.2.0/poc_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 zhizhuo    (501) staff       (20)        1 2024-04-02 05:27:08.000000 poc_tool-1.2.0/poc_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 zhizhuo    (501) staff       (20)       18 2024-04-02 05:27:08.000000 poc_tool-1.2.0/poc_tool.egg-info/requires.txt
+-rw-r--r--   0 zhizhuo    (501) staff       (20)        9 2024-04-02 05:27:08.000000 poc_tool-1.2.0/poc_tool.egg-info/top_level.txt
+-rw-r--r--   0 zhizhuo    (501) staff       (20)       79 2024-04-02 05:27:08.683958 poc_tool-1.2.0/setup.cfg
+-rw-r--r--   0 zhizhuo    (501) staff       (20)      794 2024-04-02 05:27:03.000000 poc_tool-1.2.0/setup.py
```

### Comparing `poc_tool-1.1.9/LICENSE.txt` & `poc_tool-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `poc_tool-1.1.9/PKG-INFO` & `poc_tool-1.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: poc_tool
-Version: 1.1.9
-Summary: Python Poc 还原原始http请求数据包以及常用工具集成化封装
-Home-page: https://github.com/zhizhuoshuma/poc_tool
-Author: zhizhuo
-Author-email: zhizhuoshuma@163.com
-License: MIT
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: requests
-Requires-Dist: colorama
-
 # 一个方便安全测试人员书写poc的工具库集合
 
 ## 描述
 
 避免重复造轮子以及代码的简洁，将常用的方法集成化封装到一起，提高代码的整洁和便携。
 
 ## 安装
@@ -102,7 +88,22 @@
 # 使用
 log.info("zhizhuo")
 log.success("zhizhuo")
 log.error("zhizhuo")
 log.warning("zhizhuo")
 log.debug("zhizhuo")
 ```
+
+### 文件hex编码查看，类似于Linux中的xxd命令
+
+```python
+from poc_tool import hex_dump
+
+
+# 或者使用 from poc_tool.tools import hex_dump引入
+# 参数说明，file_path文件路径，bytes_per_line每行的字节大小，默认是16
+# lines获取多少行数据，默认是全部，可以自己定义传入
+
+def hex_test():
+    hex_data = hex_dump(file_path="../poc编写规则.zip", lines=10)
+    print(hex_data)
+```
```

### Comparing `poc_tool-1.1.9/poc_tool/log/logger.py` & `poc_tool-1.2.0/poc_tool/log/logger.py`

 * *Files identical despite different names*

### Comparing `poc_tool-1.1.9/poc_tool/tools/Tools.py` & `poc_tool-1.2.0/poc_tool/tools/Tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import json
 import random
 import re
 import socket
 import string
 import struct
 from urllib.parse import urlparse, quote, unquote
+
 import requests.models
 
 UA = '''
 Mozilla/4.0 (compatible; MSIE 6.0; Windows NT 5.1; zh-cn) Opera 8.65
 Mozilla/5.0 (compatible; MSIE 6.0; Windows NT 5.1; zh-cn) Opera 8.65
 Mozilla/5.0 (Windows NT 5.1; U; zh-cn; rv:1.8.1) Gecko/20061208 Firefox/2.0.0 Opera 9.50
 Mozilla/5.0 (Windows NT 5.1; U; zh-cn; rv:1.9.1.6) Gecko/20091201 Firefox/3.5.6 Opera 10.53
@@ -80,15 +81,15 @@
 
 
 class Tools:
     def __init__(self):
 
         self._ua_list = [u for u in UA.split('\n') if u]
 
-    def get_url_format(self, url: string) -> str:
+    def get_url_format(self, url: str) -> str:
         """
         url格式化，格式成http(s)://example.com
         :param url: IP地址
         :return: url格式化地址
         """
         url = url.rstrip("/") + "/"
         url = f"http://{url}" if not url.startswith(('http://', 'https://')) else url
@@ -271,15 +272,15 @@
         """
         try:
             response = self.get_res_header(res) + res.text
         except Exception:
             response = None
         return response
 
-    def get_res_header(self, res: requests.models.Response):
+    def get_res_header(self, res: requests.models.Response) -> str:
         """
         获取响应头
         :param res: 请求响应对象Response
         :return: 响应头
         """
         try:
             res.encoding = res.apparent_encoding
```

### Comparing `poc_tool-1.1.9/setup.py` & `poc_tool-1.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 current_dir = os.path.abspath(os.path.dirname(__file__))
 with io.open(os.path.join(current_dir, "README.md"), encoding="utf-8") as fd:
     desc = fd.read()
 
 setup(
     name="poc_tool",
     license='MIT',
-    version="1.1.9",
+    version="1.2.0",
     long_description=desc,
     long_description_content_type="text/markdown",
-    description="Python Poc 还原原始http请求数据包以及常用工具集成化封装",
+    description="Python Poc 还原原始http请求数据包以及常用工具集成化封装类，可以更快帮助您完成POC的书写及调试",
     author="zhizhuo",
     author_email="zhizhuoshuma@163.com",
     url='https://github.com/zhizhuoshuma/poc_tool',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "requests",
```

