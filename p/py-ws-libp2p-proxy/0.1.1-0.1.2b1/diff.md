# Comparing `tmp/py_ws_libp2p_proxy-0.1.1.tar.gz` & `tmp/py_ws_libp2p_proxy-0.1.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_ws_libp2p_proxy-0.1.1.tar", max compression
+gzip compressed data, was "py_ws_libp2p_proxy-0.1.2b1.tar", max compression
```

## Comparing `py_ws_libp2p_proxy-0.1.1.tar` & `py_ws_libp2p_proxy-0.1.2b1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11344 2024-03-28 13:23:12.467479 py_ws_libp2p_proxy-0.1.1/LICENSE
--rw-r--r--   0        0        0      257 2024-03-28 13:23:12.467479 py_ws_libp2p_proxy-0.1.1/README.md
--rw-r--r--   0        0        0      517 2024-03-28 13:23:12.467479 py_ws_libp2p_proxy-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3877 2024-03-28 13:23:12.467479 py_ws_libp2p_proxy-0.1.1/pyproxy/__init__.py
--rw-r--r--   0        0        0        0 2024-03-28 13:23:12.467479 py_ws_libp2p_proxy-0.1.1/pyproxy/utils/__init__.py
--rw-r--r--   0        0        0     2358 2024-03-28 13:23:12.467479 py_ws_libp2p_proxy-0.1.1/pyproxy/utils/decorators.py
--rw-r--r--   0        0        0       53 2024-03-28 13:23:12.467479 py_ws_libp2p_proxy-0.1.1/pyproxy/utils/logger.py
--rw-r--r--   0        0        0      588 2024-03-28 13:23:12.467479 py_ws_libp2p_proxy-0.1.1/pyproxy/utils/message.py
--rw-r--r--   0        0        0      663 2024-03-28 13:23:12.467479 py_ws_libp2p_proxy-0.1.1/pyproxy/utils/protocols_manager.py
--rw-r--r--   0        0        0     3452 2024-03-28 13:23:12.467479 py_ws_libp2p_proxy-0.1.1/pyproxy/utils/websocket.py
--rw-r--r--   0        0        0      992 1970-01-01 00:00:00.000000 py_ws_libp2p_proxy-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11344 2024-04-02 11:52:10.396510 py_ws_libp2p_proxy-0.1.2b1/LICENSE
+-rw-r--r--   0        0        0      257 2024-04-02 11:52:10.396510 py_ws_libp2p_proxy-0.1.2b1/README.md
+-rw-r--r--   0        0        0      524 2024-04-02 11:52:10.396510 py_ws_libp2p_proxy-0.1.2b1/pyproject.toml
+-rw-r--r--   0        0        0     3877 2024-04-02 11:52:10.396510 py_ws_libp2p_proxy-0.1.2b1/pyproxy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 11:52:10.396510 py_ws_libp2p_proxy-0.1.2b1/pyproxy/utils/__init__.py
+-rw-r--r--   0        0        0     2358 2024-04-02 11:52:10.396510 py_ws_libp2p_proxy-0.1.2b1/pyproxy/utils/decorators.py
+-rw-r--r--   0        0        0       53 2024-04-02 11:52:10.396510 py_ws_libp2p_proxy-0.1.2b1/pyproxy/utils/logger.py
+-rw-r--r--   0        0        0      780 2024-04-02 11:52:10.396510 py_ws_libp2p_proxy-0.1.2b1/pyproxy/utils/message.py
+-rw-r--r--   0        0        0      663 2024-04-02 11:52:10.396510 py_ws_libp2p_proxy-0.1.2b1/pyproxy/utils/protocols_manager.py
+-rw-r--r--   0        0        0     3452 2024-04-02 11:52:10.396510 py_ws_libp2p_proxy-0.1.2b1/pyproxy/utils/websocket.py
+-rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 py_ws_libp2p_proxy-0.1.2b1/PKG-INFO
```

### Comparing `py_ws_libp2p_proxy-0.1.1/LICENSE` & `py_ws_libp2p_proxy-0.1.2b1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_ws_libp2p_proxy-0.1.1/pyproject.toml` & `py_ws_libp2p_proxy-0.1.2b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-ws-libp2p-proxy"
-version = "0.1.1"
+version = "0.1.2-beta-1"
 description = "API for libp2p-ws-proxy"
 authors = [
     "Mariia Livshits <m.bystramovich@gmail.com>",
 ]
 license = "Apache-2.0"
 
 repository = "https://github.com/tubleronchik/py-libp2p-proxy"
```

### Comparing `py_ws_libp2p_proxy-0.1.1/pyproxy/__init__.py` & `py_ws_libp2p_proxy-0.1.2b1/pyproxy/__init__.py`

 * *Files identical despite different names*

### Comparing `py_ws_libp2p_proxy-0.1.1/pyproxy/utils/decorators.py` & `py_ws_libp2p_proxy-0.1.2b1/pyproxy/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `py_ws_libp2p_proxy-0.1.1/pyproxy/utils/protocols_manager.py` & `py_ws_libp2p_proxy-0.1.2b1/pyproxy/utils/protocols_manager.py`

 * *Files identical despite different names*

### Comparing `py_ws_libp2p_proxy-0.1.1/pyproxy/utils/websocket.py` & `py_ws_libp2p_proxy-0.1.2b1/pyproxy/utils/websocket.py`

 * *Files identical despite different names*

### Comparing `py_ws_libp2p_proxy-0.1.1/PKG-INFO` & `py_ws_libp2p_proxy-0.1.2b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-ws-libp2p-proxy
-Version: 0.1.1
+Version: 0.1.2b1
 Summary: API for libp2p-ws-proxy
 Home-page: https://github.com/tubleronchik/py-libp2p-proxy
 License: Apache-2.0
 Author: Mariia Livshits
 Author-email: m.bystramovich@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

