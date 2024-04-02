# Comparing `tmp/hltv_async_api-0.2.4.tar.gz` & `tmp/hltv_async_api-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hltv_async_api-0.2.4.tar", last modified: Tue Apr  2 14:54:09 2024, max compression
+gzip compressed data, was "hltv_async_api-0.2.5.tar", last modified: Tue Apr  2 15:09:24 2024, max compression
```

## Comparing `hltv_async_api-0.2.4.tar` & `hltv_async_api-0.2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 14:54:09.763562 hltv_async_api-0.2.4/
--rw-rw-rw-   0        0        0     1091 2024-04-02 00:22:12.000000 hltv_async_api-0.2.4/LICENSE
--rw-rw-rw-   0        0        0     2357 2024-04-02 14:54:09.761565 hltv_async_api-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     1734 2024-04-02 13:35:07.000000 hltv_async_api-0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 14:54:09.740564 hltv_async_api-0.2.4/hltv_async_api/
--rw-rw-rw-   0        0        0      124 2024-04-02 14:45:39.000000 hltv_async_api-0.2.4/hltv_async_api/__init__.py
--rw-rw-rw-   0        0        0    24378 2024-04-02 13:43:04.000000 hltv_async_api-0.2.4/hltv_async_api/aiohltv.py
-drwxrwxrwx   0        0        0        0 2024-04-02 14:54:09.760561 hltv_async_api-0.2.4/hltv_async_api.egg-info/
--rw-rw-rw-   0        0        0     2357 2024-04-02 14:54:09.000000 hltv_async_api-0.2.4/hltv_async_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-04-02 14:54:09.000000 hltv_async_api-0.2.4/hltv_async_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 14:54:09.000000 hltv_async_api-0.2.4/hltv_async_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-02 14:54:09.000000 hltv_async_api-0.2.4/hltv_async_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      537 2024-04-02 14:53:47.000000 hltv_async_api-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-02 14:54:09.763562 hltv_async_api-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      922 2024-04-02 14:54:05.000000 hltv_async_api-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 15:09:24.531181 hltv_async_api-0.2.5/
+-rw-rw-rw-   0        0        0     1091 2024-04-02 00:22:12.000000 hltv_async_api-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0     2449 2024-04-02 15:09:24.521569 hltv_async_api-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1826 2024-04-02 15:07:09.000000 hltv_async_api-0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 15:09:24.241148 hltv_async_api-0.2.5/hltv_async_api/
+-rw-rw-rw-   0        0        0      124 2024-04-02 15:09:19.000000 hltv_async_api-0.2.5/hltv_async_api/__init__.py
+-rw-rw-rw-   0        0        0    24390 2024-04-02 15:05:31.000000 hltv_async_api-0.2.5/hltv_async_api/aiohltv.py
+drwxrwxrwx   0        0        0        0 2024-04-02 15:09:24.517824 hltv_async_api-0.2.5/hltv_async_api.egg-info/
+-rw-rw-rw-   0        0        0     2449 2024-04-02 15:09:23.000000 hltv_async_api-0.2.5/hltv_async_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-04-02 15:09:23.000000 hltv_async_api-0.2.5/hltv_async_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 15:09:23.000000 hltv_async_api-0.2.5/hltv_async_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-02 15:09:23.000000 hltv_async_api-0.2.5/hltv_async_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      537 2024-04-02 15:09:19.000000 hltv_async_api-0.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-02 15:09:24.533713 hltv_async_api-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      922 2024-04-02 15:09:19.000000 hltv_async_api-0.2.5/setup.py
```

### Comparing `hltv_async_api-0.2.4/LICENSE` & `hltv_async_api-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.2.4/PKG-INFO` & `hltv_async_api-0.2.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: hltv_async_api
-Version: 0.2.4
+Version: 0.2.5
 Summary: Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python
 Home-page: https://github.com/akimerslys/aiohltv
 Author: akimerslys
 Author-email: Akim Slys <akimslys2003@gmail.com>
 Project-URL: Homepage, https://github.com/akimerslys/aiohltv
 Project-URL: Issues, https://github.com/akimerslys/aiohltv/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python
+# hltv-async-api an unofficial asynchronous HLTV API Wrapper for Python
 
 # Features
 
 * New and modern fully async library
 
 * Supports proxy usage for rate-limiting and privacy
 
@@ -26,24 +26,24 @@
 
 
 ---
 
 # Installation
 
 ```
-pip install hltv-aio
+pip install hltv_async_api
 ```
 
 ---
 
 
 # Simple Usage
 
 ```
-from hltv-aio import Hltv
+from hltv_async_api import Hltv
 
 hltv = Hltv()
 live_matches = await hltv.get_live_matches()
 ```
 
 ---
 
@@ -79,27 +79,33 @@
 ```
 ---
 # Examples
 
 ****Simple Example****
 
 ```
+from hltv_async_api import Hltv
+
+
 async def test():
 
     hltv = Hltv()
     
     print(await hltv.get_event_info(7148, 'pgl-cs2-major-copenhagen-2024'))
 
 if __name__ == "__main__":
     asyncio.run(test())
 ```
 
 
 ****Proxy Parser****
 ```
+from hltv_async_api import Hltv
+
+
 async def test():
 
     hltv = Hltv(debug=True, use_proxy=True, proxy_path='proxy_test.txt', timeout=1, remove_proxy=True, proxy_protocol='http')
     
     print(await hltv.get_event_info(7148, 'pgl-cs2-major-copenhagen-2024'))
 
 if __name__ == "__main__":
```

### Comparing `hltv_async_api-0.2.4/README.md` & `hltv_async_api-0.2.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python
+# hltv-async-api an unofficial asynchronous HLTV API Wrapper for Python
 
 # Features
 
 * New and modern fully async library
 
 * Supports proxy usage for rate-limiting and privacy
 
@@ -10,24 +10,24 @@
 
 
 ---
 
 # Installation
 
 ```
-pip install hltv-aio
+pip install hltv_async_api
 ```
 
 ---
 
 
 # Simple Usage
 
 ```
-from hltv-aio import Hltv
+from hltv_async_api import Hltv
 
 hltv = Hltv()
 live_matches = await hltv.get_live_matches()
 ```
 
 ---
 
@@ -63,27 +63,33 @@
 ```
 ---
 # Examples
 
 ****Simple Example****
 
 ```
+from hltv_async_api import Hltv
+
+
 async def test():
 
     hltv = Hltv()
     
     print(await hltv.get_event_info(7148, 'pgl-cs2-major-copenhagen-2024'))
 
 if __name__ == "__main__":
     asyncio.run(test())
 ```
 
 
 ****Proxy Parser****
 ```
+from hltv_async_api import Hltv
+
+
 async def test():
 
     hltv = Hltv(debug=True, use_proxy=True, proxy_path='proxy_test.txt', timeout=1, remove_proxy=True, proxy_protocol='http')
     
     print(await hltv.get_event_info(7148, 'pgl-cs2-major-copenhagen-2024'))
 
 if __name__ == "__main__":
```

### Comparing `hltv_async_api-0.2.4/hltv_async_api/aiohltv.py` & `hltv_async_api-0.2.5/hltv_async_api/aiohltv.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,20 +141,20 @@
             # delay, only for non proxy users. (default = 1-15s)
             await asyncio.sleep(delay)
         try:
             async with session.get(url, headers=self.headers, proxy=proxy, timeout=self.timeout, ) as response:
                 self.logger.info(f"Fetching {url}, code: {response.status}")
                 if response.status == 403 or response.status == 404:
                     self.logger.debug("Got 403 forbitten")
-                    return False, self.parse_error_handler(proxy, delay)
+                    return False, await self.parse_error_handler(proxy, delay)
 
                 # checking for challenge page.
                 result = await response.text()
                 if await self.cloudflare_check(result):
-                    return False, self.parse_error_handler(proxy, delay)
+                    return False, await self.parse_error_handler(proxy, delay)
 
                 return True, result
         except (ClientProxyConnectionError, ClientResponseError, ClientOSError,
                 ServerDisconnectedError, TimeoutError, ClientHttpProxyError) as e:
             delay = await self.parse_error_handler(proxy, delay)
             return False, delay
```

### Comparing `hltv_async_api-0.2.4/hltv_async_api.egg-info/PKG-INFO` & `hltv_async_api-0.2.5/hltv_async_api.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: hltv_async_api
-Version: 0.2.4
+Version: 0.2.5
 Summary: Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python
 Home-page: https://github.com/akimerslys/aiohltv
 Author: akimerslys
 Author-email: Akim Slys <akimslys2003@gmail.com>
 Project-URL: Homepage, https://github.com/akimerslys/aiohltv
 Project-URL: Issues, https://github.com/akimerslys/aiohltv/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python
+# hltv-async-api an unofficial asynchronous HLTV API Wrapper for Python
 
 # Features
 
 * New and modern fully async library
 
 * Supports proxy usage for rate-limiting and privacy
 
@@ -26,24 +26,24 @@
 
 
 ---
 
 # Installation
 
 ```
-pip install hltv-aio
+pip install hltv_async_api
 ```
 
 ---
 
 
 # Simple Usage
 
 ```
-from hltv-aio import Hltv
+from hltv_async_api import Hltv
 
 hltv = Hltv()
 live_matches = await hltv.get_live_matches()
 ```
 
 ---
 
@@ -79,27 +79,33 @@
 ```
 ---
 # Examples
 
 ****Simple Example****
 
 ```
+from hltv_async_api import Hltv
+
+
 async def test():
 
     hltv = Hltv()
     
     print(await hltv.get_event_info(7148, 'pgl-cs2-major-copenhagen-2024'))
 
 if __name__ == "__main__":
     asyncio.run(test())
 ```
 
 
 ****Proxy Parser****
 ```
+from hltv_async_api import Hltv
+
+
 async def test():
 
     hltv = Hltv(debug=True, use_proxy=True, proxy_path='proxy_test.txt', timeout=1, remove_proxy=True, proxy_protocol='http')
     
     print(await hltv.get_event_info(7148, 'pgl-cs2-major-copenhagen-2024'))
 
 if __name__ == "__main__":
```

### Comparing `hltv_async_api-0.2.4/pyproject.toml` & `hltv_async_api-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hltv_async_api"
-version = "0.2.4"
+version = "0.2.5"
 authors = [
   { name="Akim Slys", email="akimslys2003@gmail.com" },
 ]
 description = "Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `hltv_async_api-0.2.4/setup.py` & `hltv_async_api-0.2.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='hltv_async_api',
-    version='0.2.4',
+    version='0.2.5',
     author='akimerslys',
     author_email='akimslys2003@gmail.com',
     description='Hltv-aio: An unofficial asynchronous HLTV API Wrapper for Python',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/akimerslys/aiohltv',
     packages=find_packages(),
```

