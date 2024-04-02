# Comparing `tmp/xcsc_dataapi-1.0.1.tar.gz` & `tmp/xcsc_dataapi-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcsc_dataapi-1.0.1.tar", last modified: Fri Mar 29 08:53:46 2024, max compression
+gzip compressed data, was "xcsc_dataapi-1.0.2.tar", last modified: Tue Apr  2 02:38:14 2024, max compression
```

## Comparing `xcsc_dataapi-1.0.1.tar` & `xcsc_dataapi-1.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-03-29 08:53:46.866522 xcsc_dataapi-1.0.1/
--rw-r--r--   0 root         (0) staff       (20)      885 2024-03-29 08:53:46.866282 xcsc_dataapi-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     6217 2024-03-26 07:35:58.000000 xcsc_dataapi-1.0.1/README.md
--rw-r--r--   0 root         (0) staff       (20)       38 2024-03-29 08:53:46.866562 xcsc_dataapi-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     1497 2024-03-29 08:07:07.000000 xcsc_dataapi-1.0.1/setup.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-03-29 08:53:46.863752 xcsc_dataapi-1.0.1/test/
--rw-r--r--   0 root         (0) staff       (20)        0 2024-03-29 03:30:43.000000 xcsc_dataapi-1.0.1/test/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      404 2024-03-29 03:30:43.000000 xcsc_dataapi-1.0.1/test/dataapi_test.py
--rw-r--r--   0 root         (0) staff       (20)      171 2024-03-29 08:44:14.000000 xcsc_dataapi-1.0.1/test/token_test.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-03-29 08:53:46.864103 xcsc_dataapi-1.0.1/xcsc_dataapi/
--rw-r--r--   0 root         (0) staff       (20)        5 2024-03-29 08:52:44.000000 xcsc_dataapi-1.0.1/xcsc_dataapi/VERSION.txt
--rw-r--r--   0 root         (0) staff       (20)      222 2024-03-29 03:30:43.000000 xcsc_dataapi-1.0.1/xcsc_dataapi/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-03-29 08:53:46.865249 xcsc_dataapi-1.0.1/xcsc_dataapi/data/
--rw-r--r--   0 root         (0) staff       (20)        0 2024-03-29 03:30:43.000000 xcsc_dataapi-1.0.1/xcsc_dataapi/data/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1985 2024-03-29 03:30:43.000000 xcsc_dataapi-1.0.1/xcsc_dataapi/data/client.py
--rw-r--r--   0 root         (0) staff       (20)     2944 2024-03-29 05:44:40.000000 xcsc_dataapi-1.0.1/xcsc_dataapi/data/token.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-03-29 08:53:46.865552 xcsc_dataapi-1.0.1/xcsc_dataapi/util/
--rw-r--r--   0 root         (0) staff       (20)        0 2024-03-29 03:30:43.000000 xcsc_dataapi-1.0.1/xcsc_dataapi/util/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1229 2024-03-29 05:36:22.000000 xcsc_dataapi-1.0.1/xcsc_dataapi/util/sm4_cbc_util.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-03-29 08:53:46.865968 xcsc_dataapi-1.0.1/xcsc_dataapi.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      885 2024-03-29 08:53:46.000000 xcsc_dataapi-1.0.1/xcsc_dataapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      453 2024-03-29 08:53:46.000000 xcsc_dataapi-1.0.1/xcsc_dataapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2024-03-29 08:53:46.000000 xcsc_dataapi-1.0.1/xcsc_dataapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       42 2024-03-29 08:53:46.000000 xcsc_dataapi-1.0.1/xcsc_dataapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       18 2024-03-29 08:53:46.000000 xcsc_dataapi-1.0.1/xcsc_dataapi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-02 02:38:14.429722 xcsc_dataapi-1.0.2/
+-rw-r--r--   0 root         (0) staff       (20)      885 2024-04-02 02:38:14.429502 xcsc_dataapi-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     6217 2024-03-26 07:35:58.000000 xcsc_dataapi-1.0.2/README.md
+-rw-r--r--   0 root         (0) staff       (20)       38 2024-04-02 02:38:14.429764 xcsc_dataapi-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     1497 2024-03-29 08:07:07.000000 xcsc_dataapi-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-02 02:38:14.426999 xcsc_dataapi-1.0.2/test/
+-rw-r--r--   0 root         (0) staff       (20)        0 2024-03-29 03:30:43.000000 xcsc_dataapi-1.0.2/test/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      264 2024-04-02 02:28:41.000000 xcsc_dataapi-1.0.2/test/dataapi_test.py
+-rw-r--r--   0 root         (0) staff       (20)      171 2024-03-29 09:05:28.000000 xcsc_dataapi-1.0.2/test/token_test.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-02 02:38:14.427381 xcsc_dataapi-1.0.2/xcsc_dataapi/
+-rw-r--r--   0 root         (0) staff       (20)        5 2024-04-02 02:27:21.000000 xcsc_dataapi-1.0.2/xcsc_dataapi/VERSION.txt
+-rw-r--r--   0 root         (0) staff       (20)      222 2024-03-29 03:30:43.000000 xcsc_dataapi-1.0.2/xcsc_dataapi/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-02 02:38:14.428558 xcsc_dataapi-1.0.2/xcsc_dataapi/data/
+-rw-r--r--   0 root         (0) staff       (20)        0 2024-03-29 03:30:43.000000 xcsc_dataapi-1.0.2/xcsc_dataapi/data/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1952 2024-04-02 02:28:54.000000 xcsc_dataapi-1.0.2/xcsc_dataapi/data/client.py
+-rw-r--r--   0 root         (0) staff       (20)     2877 2024-04-02 02:29:11.000000 xcsc_dataapi-1.0.2/xcsc_dataapi/data/token.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-02 02:38:14.428883 xcsc_dataapi-1.0.2/xcsc_dataapi/util/
+-rw-r--r--   0 root         (0) staff       (20)        0 2024-03-29 03:30:43.000000 xcsc_dataapi-1.0.2/xcsc_dataapi/util/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1229 2024-03-29 05:36:22.000000 xcsc_dataapi-1.0.2/xcsc_dataapi/util/sm4_cbc_util.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-02 02:38:14.429257 xcsc_dataapi-1.0.2/xcsc_dataapi.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      885 2024-04-02 02:38:14.000000 xcsc_dataapi-1.0.2/xcsc_dataapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      453 2024-04-02 02:38:14.000000 xcsc_dataapi-1.0.2/xcsc_dataapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-04-02 02:38:14.000000 xcsc_dataapi-1.0.2/xcsc_dataapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       42 2024-04-02 02:38:14.000000 xcsc_dataapi-1.0.2/xcsc_dataapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       18 2024-04-02 02:38:14.000000 xcsc_dataapi-1.0.2/xcsc_dataapi.egg-info/top_level.txt
```

### Comparing `xcsc_dataapi-1.0.1/PKG-INFO` & `xcsc_dataapi-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcsc_dataapi
-Version: 1.0.1
+Version: 1.0.2
 Summary: xcsc_data data api
 Home-page: https://www.xcsc.com
 Author: Xiangcai Security
 Author-email: itsupport@xcsc.com
 License: MIT
 Keywords: Financial Data
 Classifier: Development Status :: 4 - Beta
```

### Comparing `xcsc_dataapi-1.0.1/README.md` & `xcsc_dataapi-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `xcsc_dataapi-1.0.1/setup.py` & `xcsc_dataapi-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `xcsc_dataapi-1.0.1/xcsc_dataapi/data/client.py` & `xcsc_dataapi-1.0.2/xcsc_dataapi/data/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,42 +13,42 @@
     __token = ''
     __http_url = 'https://dataapi.xcsc.com/data-api'
 
     def __init__(self, token, timeout=10):
         self.__token = token
         self.__timeout = timeout
 
-    def query(self, api_url='', fields='', current_page='', data_type='', **kwargs):
+    def query(self, api_url='', fields='', current_page='', **kwargs):
         """
                     查询数据
                     :param api_url:接口地址，不包含域名及上下文
                     :param current_page: 当前页数，不传默认是 1
-                    :param fields: 上送字段列表
-                    :param data_type: 返回数据类型，不传默认是 dataframe格式,支持json和dataframe
+                    :param fields: 上送字段列表，不传默认返回全部
                     :return: api data
                     """
         if self.__token == '':
-            return "token值未填"
+            raise Exception('token为空')
         api_headers = {
             'Content-Type': 'application/json',  # 自定义Content-Type头
             'Authorization': self.__token  # init 接口获取到的access_token
         }
         data_dict = kwargs
         # 向字典中添加新的键值对
+        if current_page == '' or current_page is None:
+            current_page = 1
         data_dict["currentPage"] = current_page  # 当前页数，1 代表第一页，2 代表第二页
         data_dict["fieldList"] = fields  # 自定义返回相应参数，不传或者为空默认都是返回全部，传参内容以逗号【,】分割
         api_data = {
             'requestId': time.time_ns(),
             'data': data_dict
         }
         response = requests.post(self.__http_url + api_url, json=api_data, headers=api_headers, verify=False,
                                  timeout=self.__timeout)
         if response.status_code == 200:
-            print('api接口请求成功')
-            print(response.text)
+            print('api数据查询成功')
         else:
-            print('api接口请求失败,' + response.text)
+            raise Exception('api数据请求失败,' + response.text)
 
         return response.text
 
     def __getattr__(self, name):
         return partial(self.query, name)
```

### Comparing `xcsc_dataapi-1.0.1/xcsc_dataapi/data/token.py` & `xcsc_dataapi-1.0.2/xcsc_dataapi/data/token.py`

 * *Files 12% similar despite different names*

```diff
@@ -47,17 +47,16 @@
     access_token_in = ''
     if init_response.status_code == 200:
         init_result = init_response.json()
         code = init_result['code']
         if code == '0':
             # access_token会有失效时间，请在有效期内使用，不要每次请求api都重新生成新的access_token!!!
             access_token_in = init_result['data']['accessToken']  # access_token
-            print('获取令牌token成功, token=' + access_token_in)
         else:
-            print('获取令牌token失败：' + init_result['msg'])
+            Exception('获取令牌token失败：' + init_result['msg'])
 
     else:
         Exception('初始化获取accessToken请求失败,'+init_response.text)
 
     return access_token_in
```

### Comparing `xcsc_dataapi-1.0.1/xcsc_dataapi/util/sm4_cbc_util.py` & `xcsc_dataapi-1.0.2/xcsc_dataapi/util/sm4_cbc_util.py`

 * *Files identical despite different names*

### Comparing `xcsc_dataapi-1.0.1/xcsc_dataapi.egg-info/PKG-INFO` & `xcsc_dataapi-1.0.2/xcsc_dataapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcsc_dataapi
-Version: 1.0.1
+Version: 1.0.2
 Summary: xcsc_data data api
 Home-page: https://www.xcsc.com
 Author: Xiangcai Security
 Author-email: itsupport@xcsc.com
 License: MIT
 Keywords: Financial Data
 Classifier: Development Status :: 4 - Beta
```

