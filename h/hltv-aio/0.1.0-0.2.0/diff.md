# Comparing `tmp/hltv-aio-0.1.0.tar.gz` & `tmp/hltv-aio-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hltv-aio-0.1.0.tar", last modified: Tue Apr  2 00:47:02 2024, max compression
+gzip compressed data, was "hltv-aio-0.2.0.tar", last modified: Tue Apr  2 13:59:32 2024, max compression
```

## Comparing `hltv-aio-0.1.0.tar` & `hltv-aio-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 00:47:02.093599 hltv-aio-0.1.0/
--rw-rw-rw-   0        0        0     1091 2024-04-02 00:22:12.000000 hltv-aio-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1493 2024-04-02 00:47:02.091589 hltv-aio-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      877 2024-04-02 00:46:58.000000 hltv-aio-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 00:47:02.088052 hltv-aio-0.1.0/hltv_aio.egg-info/
--rw-rw-rw-   0        0        0     1493 2024-04-02 00:47:01.000000 hltv-aio-0.1.0/hltv_aio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      169 2024-04-02 00:47:01.000000 hltv-aio-0.1.0/hltv_aio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 00:47:01.000000 hltv-aio-0.1.0/hltv_aio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 00:47:01.000000 hltv-aio-0.1.0/hltv_aio.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      531 2024-04-02 00:46:58.000000 hltv-aio-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-02 00:47:02.093599 hltv-aio-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      913 2024-04-02 00:46:58.000000 hltv-aio-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 13:59:32.027820 hltv-aio-0.2.0/
+-rw-rw-rw-   0        0        0     1091 2024-04-02 00:22:12.000000 hltv-aio-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     2350 2024-04-02 13:59:32.024824 hltv-aio-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1734 2024-04-02 13:35:07.000000 hltv-aio-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 13:59:32.023826 hltv-aio-0.2.0/hltv_aio.egg-info/
+-rw-rw-rw-   0        0        0     2350 2024-04-02 13:59:31.000000 hltv-aio-0.2.0/hltv_aio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      169 2024-04-02 13:59:31.000000 hltv-aio-0.2.0/hltv_aio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 13:59:31.000000 hltv-aio-0.2.0/hltv_aio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 13:59:31.000000 hltv-aio-0.2.0/hltv_aio.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      531 2024-04-02 13:52:37.000000 hltv-aio-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-02 13:59:32.027820 hltv-aio-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      913 2024-04-02 13:52:19.000000 hltv-aio-0.2.0/setup.py
```

### Comparing `hltv-aio-0.1.0/LICENSE` & `hltv-aio-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hltv-aio-0.1.0/README.md` & `hltv-aio-0.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -17,38 +17,83 @@
 pip install hltv-aio
 ```
 
 ---
 
 
 # Simple Usage
+
 ```
 from hltv-aio import Hltv
 
-
 hltv = Hltv()
 live_matches = await hltv.get_live_matches()
 ```
 
 ---
 
 # Proxy Usage
+
+**Load Proxies from list**
+
+```
+proxy_list = ['http://120.234.203.171:9002', 'http://110.38.68.38:80']
+
+hltv = Hltv(use_proxy=True, proxy_list=proxy_list)
+```
+
 **Load Proxies from file**
 
 ```
 hltv = Hltv(use_proxy=True, proxy_path='PATH_TO_PROXY.TXT')
 ```
 
-**Load Proxies from list**
+
+**Remove bad proxy from file**
+
+```
+hltv = Hltv(use_proxy=True, proxy_path='PATH_TO_PROXY.TXT', remove_proxy=True)
 ```
-proxy_list = ['http://120.234.203.171:9002', 'http://110.38.68.38:80']
 
-hltv = Hltv(use_proxy=True, proxy_list=proxy_list)
+**Add proxy protocol**
+
+```
+proxy_list = ['120.234.203.171:9002', '110.38.68.38:80']
+
+hltv = Hltv(use_proxy=True, proxy_list=proxy_list, proxy_protocol='http')
 ```
 ---
+# Examples
+
+****Simple Example****
+
+```
+async def test():
+
+    hltv = Hltv()
+    
+    print(await hltv.get_event_info(7148, 'pgl-cs2-major-copenhagen-2024'))
+
+if __name__ == "__main__":
+    asyncio.run(test())
+```
+
+
+****Proxy Parser****
+```
+async def test():
+
+    hltv = Hltv(debug=True, use_proxy=True, proxy_path='proxy_test.txt', timeout=1, remove_proxy=True, proxy_protocol='http')
+    
+    print(await hltv.get_event_info(7148, 'pgl-cs2-major-copenhagen-2024'))
+
+if __name__ == "__main__":
+    asyncio.run(test())
+```
+
 
 # Requirements:
 
 Python 3.9+
 
 License:
 HLTV Async is licensed under the MIT License, allowing for personal and commercial use with minimal restrictions.
```

### Comparing `hltv-aio-0.1.0/pyproject.toml` & `hltv-aio-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hltv-aio"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   { name="Akim Slys", email="akimslys2003@gmail.com" },
 ]
 description = "Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `hltv-aio-0.1.0/setup.py` & `hltv-aio-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='hltv-aio',
-    version='0.1.0',
+    version='0.2.0',
     author='Akim Slys',
     author_email='akimslys2003@gmail.com',
     description='Hltv-aio: An unofficial asynchronous HLTV API Wrapper for Python',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/akimerslys/aiohltv',
     packages=find_packages(),
```

