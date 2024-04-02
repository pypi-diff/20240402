# Comparing `tmp/eezo-0.1.4.tar.gz` & `tmp/eezo-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/eezo-0.1.4.tar", last modified: Wed Mar 27 14:22:12 2024, max compression
+gzip compressed data, was "eezo-0.1.5.tar", last modified: Tue Apr  2 20:38:15 2024, max compression
```

## Comparing `eezo-0.1.4.tar` & `eezo-0.1.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-03-27 14:22:12.000000 eezo-0.1.4/
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1270 2024-03-27 14:22:12.000000 eezo-0.1.4/PKG-INFO
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1558 2024-03-19 14:53:56.000000 eezo-0.1.4/README.md
-drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-03-27 14:22:12.000000 eezo-0.1.4/eezo/
-drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-03-27 14:22:12.000000 eezo-0.1.4/eezo/interface/
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     3027 2024-03-19 14:09:37.000000 eezo-0.1.4/eezo/interface/interface.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)       78 2024-03-19 12:03:08.000000 eezo-0.1.4/eezo/interface/__init__.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1330 2024-03-19 12:03:08.000000 eezo-0.1.4/eezo/interface/message.py
-drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-03-27 14:22:12.000000 eezo-0.1.4/eezo/interface/components/
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      329 2024-03-19 12:03:08.000000 eezo-0.1.4/eezo/interface/components/__init__.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1743 2024-03-19 12:03:08.000000 eezo-0.1.4/eezo/interface/components/chart.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      283 2024-03-19 12:03:08.000000 eezo-0.1.4/eezo/interface/components/youtube_video.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      246 2024-03-19 12:03:08.000000 eezo-0.1.4/eezo/interface/components/text.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      159 2024-03-19 12:03:08.000000 eezo-0.1.4/eezo/interface/components/component.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      243 2024-03-19 12:03:08.000000 eezo-0.1.4/eezo/interface/components/image.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     4509 2024-03-25 13:19:55.000000 eezo-0.1.4/eezo/client.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)       86 2024-03-19 12:03:08.000000 eezo-0.1.4/eezo/__init__.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     4462 2024-03-27 14:19:55.000000 eezo-0.1.4/eezo/async_client.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     9789 2024-03-27 14:19:36.000000 eezo-0.1.4/eezo/connector.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1921 2024-03-27 14:20:34.000000 eezo-0.1.4/setup.py
-drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-03-27 14:22:12.000000 eezo-0.1.4/eezo.egg-info/
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1270 2024-03-27 14:22:12.000000 eezo-0.1.4/eezo.egg-info/PKG-INFO
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      533 2024-03-27 14:22:12.000000 eezo-0.1.4/eezo.egg-info/SOURCES.txt
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      353 2024-03-27 14:22:12.000000 eezo-0.1.4/eezo.egg-info/requires.txt
--rw-r--r--   0 danielschonbohm   (501) staff       (20)        5 2024-03-27 14:22:12.000000 eezo-0.1.4/eezo.egg-info/top_level.txt
--rw-r--r--   0 danielschonbohm   (501) staff       (20)        1 2024-03-27 14:22:12.000000 eezo-0.1.4/eezo.egg-info/dependency_links.txt
--rw-r--r--   0 danielschonbohm   (501) staff       (20)       38 2024-03-27 14:22:12.000000 eezo-0.1.4/setup.cfg
+drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-02 20:38:15.326860 eezo-0.1.5/
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     1259 2024-04-02 20:38:15.326742 eezo-0.1.5/PKG-INFO
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     1558 2024-03-19 14:53:56.000000 eezo-0.1.5/README.md
+drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-02 20:38:15.324906 eezo-0.1.5/eezo/
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)       86 2024-03-19 12:03:08.000000 eezo-0.1.5/eezo/__init__.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     4495 2024-04-02 19:37:54.000000 eezo-0.1.5/eezo/async_client.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     4542 2024-03-27 15:07:04.000000 eezo-0.1.5/eezo/client.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)    10624 2024-04-02 20:32:55.000000 eezo-0.1.5/eezo/connector.py
+drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-02 20:38:15.325848 eezo-0.1.5/eezo/interface/
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)       78 2024-03-19 12:03:08.000000 eezo-0.1.5/eezo/interface/__init__.py
+drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-02 20:38:15.326591 eezo-0.1.5/eezo/interface/components/
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      329 2024-03-19 12:03:08.000000 eezo-0.1.5/eezo/interface/components/__init__.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     1743 2024-03-19 12:03:08.000000 eezo-0.1.5/eezo/interface/components/chart.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      159 2024-03-19 12:03:08.000000 eezo-0.1.5/eezo/interface/components/component.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      243 2024-03-19 12:03:08.000000 eezo-0.1.5/eezo/interface/components/image.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      246 2024-03-19 12:03:08.000000 eezo-0.1.5/eezo/interface/components/text.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      283 2024-03-19 12:03:08.000000 eezo-0.1.5/eezo/interface/components/youtube_video.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     3027 2024-03-19 14:09:37.000000 eezo-0.1.5/eezo/interface/interface.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     1330 2024-03-19 12:03:08.000000 eezo-0.1.5/eezo/interface/message.py
+drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-02 20:38:15.325520 eezo-0.1.5/eezo.egg-info/
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     1259 2024-04-02 20:38:15.000000 eezo-0.1.5/eezo.egg-info/PKG-INFO
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      533 2024-04-02 20:38:15.000000 eezo-0.1.5/eezo.egg-info/SOURCES.txt
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)        1 2024-04-02 20:38:15.000000 eezo-0.1.5/eezo.egg-info/dependency_links.txt
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      353 2024-04-02 20:38:15.000000 eezo-0.1.5/eezo.egg-info/requires.txt
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)        5 2024-04-02 20:38:15.000000 eezo-0.1.5/eezo.egg-info/top_level.txt
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)       38 2024-04-02 20:38:15.327023 eezo-0.1.5/setup.cfg
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     1921 2024-04-02 20:36:22.000000 eezo-0.1.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `eezo-0.1.4/PKG-INFO` & `eezo-0.1.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: eezo
-Version: 0.1.4
+Version: 0.1.5
 Summary: Eezo's Dashboard streamlines the management of AI agents via its API, offering a user-friendly interface that requires minimal coding. It enables easy access for all team members, fostering agent interaction and collaboration. The platform also features real-time data sharing with interactive charts, making it an ideal solution for developers and companies looking to centralize their AI tools and processes.
 Home-page: UNKNOWN
 Author: Daniel Schoenbohm
 Author-email: daniel@eezo.ai
 License: UNKNOWN
-Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -18,7 +17,10 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
+
+UNKNOWN
+
```

### Comparing `eezo-0.1.4/README.md` & `eezo-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `eezo-0.1.4/eezo/interface/interface.py` & `eezo-0.1.5/eezo/interface/interface.py`

 * *Files identical despite different names*

### Comparing `eezo-0.1.4/eezo/interface/message.py` & `eezo-0.1.5/eezo/interface/message.py`

 * *Files identical despite different names*

### Comparing `eezo-0.1.4/eezo/interface/components/chart.py` & `eezo-0.1.5/eezo/interface/components/chart.py`

 * *Files identical despite different names*

### Comparing `eezo-0.1.4/eezo/client.py` & `eezo-0.1.5/eezo/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import concurrent.futures
 import requests
 import sys
 import os
 
 SERVER = "https://api-service-bofkvbi4va-ey.a.run.app"
 if os.environ.get("EEZO_DEV_MODE") == "True":
+    print("Running in dev mode")
     SERVER = "http://localhost:8082"
 
 CREATE_MESSAGE_ENDPOINT = SERVER + "/v1/create-message/"
 READ_MESSAGE_ENDPOINT = SERVER + "/v1/read-message/"
 DELETE_MESSAGE_ENDPOINT = SERVER + "/v1/delete-message/"
```

### Comparing `eezo-0.1.4/eezo/async_client.py` & `eezo-0.1.5/eezo/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import asyncio
 import aiohttp
 import sys
 import os
 
 SERVER = "https://api-service-bofkvbi4va-ey.a.run.app"
 if os.environ.get("EEZO_DEV_MODE") == "True":
+    print("Running in dev mode")
     SERVER = "http://localhost:8082"
 
 CREATE_MESSAGE_ENDPOINT = SERVER + "/v1/create-message/"
 READ_MESSAGE_ENDPOINT = SERVER + "/v1/read-message/"
 DELETE_MESSAGE_ENDPOINT = SERVER + "/v1/delete-message/"
```

### Comparing `eezo-0.1.4/eezo/connector.py` & `eezo-0.1.5/eezo/connector.py`

 * *Files 6% similar despite different names*

```diff
@@ -144,14 +144,24 @@
                         self.__log("   Retrying to connect...")
                     await asyncio.sleep(5)
                 else:
                     break
             except KeyboardInterrupt:
                 self.run_loop = False
                 break
+            except Exception as e:
+                if self.run_loop:
+                    if self.logger:
+                        self.__log(
+                            f" ✖ Connector {self.connector_id} failed to connect with error: {e}"
+                        )
+                        self.__log("   Retrying to connect...")
+                    await asyncio.sleep(5)
+                else:
+                    break
 
         await self.sio.disconnect()
 
 
 class Connector:
     def __init__(self, api_key, connector_id, connector_function, logger=False):
         self.api_key = api_key
@@ -264,9 +274,19 @@
                         self.__log("   Retrying to connect...")
                     time.sleep(5)
                 else:
                     break
             except KeyboardInterrupt:
                 self.run_loop = False
                 break
+            except Exception as e:
+                if self.run_loop:
+                    if self.logger:
+                        self.__log(
+                            f" ✖ Connector {self.connector_id} failed to connect with error: {e}"
+                        )
+                        self.__log("   Retrying to connect...")
+                    time.sleep(5)
+                else:
+                    break
 
         self.sio.disconnect()
```

### Comparing `eezo-0.1.4/setup.py` & `eezo-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="eezo",
-    version="0.1.4",
+    version="0.1.5",
     description="Eezo's Dashboard streamlines the management of AI agents via its API, offering a user-friendly interface that requires minimal coding. It enables easy access for all team members, fostering agent interaction and collaboration. The platform also features real-time data sharing with interactive charts, making it an ideal solution for developers and companies looking to centralize their AI tools and processes.",
     author="Daniel Schoenbohm",
     author_email="daniel@eezo.ai",
     packages=find_packages(),
     install_requires=[
         "aiohttp==3.9.3",
         "aiosignal==1.3.1",
```

### Comparing `eezo-0.1.4/eezo.egg-info/PKG-INFO` & `eezo-0.1.5/eezo.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: eezo
-Version: 0.1.4
+Version: 0.1.5
 Summary: Eezo's Dashboard streamlines the management of AI agents via its API, offering a user-friendly interface that requires minimal coding. It enables easy access for all team members, fostering agent interaction and collaboration. The platform also features real-time data sharing with interactive charts, making it an ideal solution for developers and companies looking to centralize their AI tools and processes.
 Home-page: UNKNOWN
 Author: Daniel Schoenbohm
 Author-email: daniel@eezo.ai
 License: UNKNOWN
-Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -18,7 +17,10 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
+
+UNKNOWN
+
```

### Comparing `eezo-0.1.4/eezo.egg-info/SOURCES.txt` & `eezo-0.1.5/eezo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

