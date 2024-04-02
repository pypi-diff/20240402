# Comparing `tmp/guisurfer-0.1.8.tar.gz` & `tmp/guisurfer-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guisurfer-0.1.8.tar", max compression
+gzip compressed data, was "guisurfer-0.1.9.tar", max compression
```

## Comparing `guisurfer-0.1.8.tar` & `guisurfer-0.1.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      974 2024-03-12 15:13:00.735993 guisurfer-0.1.8/README.md
--rw-r--r--   0        0        0     6974 2024-03-14 19:51:51.435159 guisurfer-0.1.8/guisurfer/agent/base.py
--rw-r--r--   0        0        0      195 2024-03-13 02:06:32.688285 guisurfer-0.1.8/guisurfer/agent/env.py
--rw-r--r--   0        0        0      255 2024-03-16 23:45:22.399566 guisurfer-0.1.8/guisurfer/agent/models.py
--rw-r--r--   0        0        0    21429 2024-03-17 22:39:09.422900 guisurfer-0.1.8/guisurfer/agent/runtime.py
--rw-r--r--   0        0        0     9777 2024-03-18 04:43:18.952604 guisurfer-0.1.8/guisurfer/agent/task.py
--rw-r--r--   0        0        0     3979 2024-03-12 14:57:30.561570 guisurfer-0.1.8/guisurfer/agent/types.py
--rw-r--r--   0        0        0       23 2024-03-12 14:57:30.562095 guisurfer-0.1.8/guisurfer/auth/default.py
--rw-r--r--   0        0        0     2625 2024-03-12 14:57:30.562294 guisurfer-0.1.8/guisurfer/auth/key.py
--rw-r--r--   0        0        0     3953 2024-03-16 01:54:34.740485 guisurfer-0.1.8/guisurfer/auth/provider.py
--rw-r--r--   0        0        0      735 2024-03-12 14:57:30.562969 guisurfer-0.1.8/guisurfer/auth/transport.py
--rw-r--r--   0        0        0     2204 2024-03-12 14:57:30.563097 guisurfer-0.1.8/guisurfer/auth/user.py
--rw-r--r--   0        0        0     2013 2024-03-16 03:38:43.949108 guisurfer-0.1.8/guisurfer/db/conn.py
--rw-r--r--   0        0        0     4626 2024-03-14 17:05:48.343688 guisurfer-0.1.8/guisurfer/db/models.py
--rw-r--r--   0        0        0      278 2024-03-13 02:22:33.630814 guisurfer-0.1.8/guisurfer/job/agent/base.py
--rw-r--r--   0        0        0     5617 2024-03-16 16:58:47.462558 guisurfer-0.1.8/guisurfer/job/agent/job.py
--rw-r--r--   0        0        0     1398 2024-03-14 16:50:50.739638 guisurfer-0.1.8/guisurfer/job/agent/k8s.py
--rw-r--r--   0        0        0     5678 2024-03-17 22:42:47.259226 guisurfer-0.1.8/guisurfer/job/agent/main.py
--rw-r--r--   0        0        0     4089 2024-03-13 01:50:30.916392 guisurfer-0.1.8/guisurfer/job/base.py
--rw-r--r--   0        0        0        1 2024-03-13 02:36:20.263751 guisurfer-0.1.8/guisurfer/job/env.py
--rw-r--r--   0        0        0     2328 2024-03-14 18:27:55.610267 guisurfer-0.1.8/guisurfer/job/log.py
--rw-r--r--   0        0        0     1305 2024-03-17 03:25:50.141307 guisurfer-0.1.8/guisurfer/server/app.py
--rw-r--r--   0        0        0     1046 2024-03-14 04:26:30.848276 guisurfer-0.1.8/guisurfer/server/boot.py
--rw-r--r--   0        0        0      611 2024-03-13 03:13:33.206920 guisurfer-0.1.8/guisurfer/server/hub.py
--rw-r--r--   0        0        0     4126 2024-03-15 00:50:25.755236 guisurfer-0.1.8/guisurfer/server/key.py
--rw-r--r--   0        0        0     5005 2024-03-18 03:34:12.196407 guisurfer-0.1.8/guisurfer/server/models.py
--rw-r--r--   0        0        0    11070 2024-03-17 20:35:35.640165 guisurfer-0.1.8/guisurfer/server/router/agents.py
--rw-r--r--   0        0        0     4113 2024-03-13 21:53:21.741421 guisurfer-0.1.8/guisurfer/server/router/desktops.py
--rw-r--r--   0        0        0      802 2024-03-13 22:08:03.348200 guisurfer-0.1.8/guisurfer/server/router/job.py
--rw-r--r--   0        0        0     1233 2024-03-13 21:50:46.751451 guisurfer-0.1.8/guisurfer/server/router/keys.py
--rw-r--r--   0        0        0     3449 2024-03-15 03:02:12.619360 guisurfer-0.1.8/guisurfer/server/router/runtime.py
--rw-r--r--   0        0        0     4230 2024-03-17 19:23:50.096569 guisurfer-0.1.8/guisurfer/server/router/task.py
--rw-r--r--   0        0        0     6499 2024-03-17 18:38:15.604179 guisurfer-0.1.8/guisurfer/server/router/vnc.py
--rw-r--r--   0        0        0     6724 2024-03-14 23:20:08.325281 guisurfer-0.1.8/guisurfer/server/runtime.py
--rw-r--r--   0        0        0     1360 2024-03-17 00:30:04.360017 guisurfer-0.1.8/guisurfer/server/test.py
--rw-r--r--   0        0        0      666 2024-03-18 17:46:16.980270 guisurfer-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1831 1970-01-01 00:00:00.000000 guisurfer-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      974 2024-03-12 15:13:00.735993 guisurfer-0.1.9/README.md
+-rw-r--r--   0        0        0     6974 2024-03-14 19:51:51.435159 guisurfer-0.1.9/guisurfer/agent/base.py
+-rw-r--r--   0        0        0      195 2024-03-13 02:06:32.688285 guisurfer-0.1.9/guisurfer/agent/env.py
+-rw-r--r--   0        0        0      255 2024-03-16 23:45:22.399566 guisurfer-0.1.9/guisurfer/agent/models.py
+-rw-r--r--   0        0        0    21429 2024-03-17 22:39:09.422900 guisurfer-0.1.9/guisurfer/agent/runtime.py
+-rw-r--r--   0        0        0     9777 2024-03-18 04:43:18.952604 guisurfer-0.1.9/guisurfer/agent/task.py
+-rw-r--r--   0        0        0     3979 2024-03-12 14:57:30.561570 guisurfer-0.1.9/guisurfer/agent/types.py
+-rw-r--r--   0        0        0       23 2024-03-12 14:57:30.562095 guisurfer-0.1.9/guisurfer/auth/default.py
+-rw-r--r--   0        0        0     2625 2024-03-12 14:57:30.562294 guisurfer-0.1.9/guisurfer/auth/key.py
+-rw-r--r--   0        0        0     3953 2024-03-16 01:54:34.740485 guisurfer-0.1.9/guisurfer/auth/provider.py
+-rw-r--r--   0        0        0      735 2024-03-12 14:57:30.562969 guisurfer-0.1.9/guisurfer/auth/transport.py
+-rw-r--r--   0        0        0     2204 2024-03-12 14:57:30.563097 guisurfer-0.1.9/guisurfer/auth/user.py
+-rw-r--r--   0        0        0     2013 2024-03-16 03:38:43.949108 guisurfer-0.1.9/guisurfer/db/conn.py
+-rw-r--r--   0        0        0     4626 2024-03-14 17:05:48.343688 guisurfer-0.1.9/guisurfer/db/models.py
+-rw-r--r--   0        0        0      278 2024-03-13 02:22:33.630814 guisurfer-0.1.9/guisurfer/job/agent/base.py
+-rw-r--r--   0        0        0     5617 2024-03-16 16:58:47.462558 guisurfer-0.1.9/guisurfer/job/agent/job.py
+-rw-r--r--   0        0        0     1398 2024-03-14 16:50:50.739638 guisurfer-0.1.9/guisurfer/job/agent/k8s.py
+-rw-r--r--   0        0        0     5678 2024-03-17 22:42:47.259226 guisurfer-0.1.9/guisurfer/job/agent/main.py
+-rw-r--r--   0        0        0     4089 2024-03-13 01:50:30.916392 guisurfer-0.1.9/guisurfer/job/base.py
+-rw-r--r--   0        0        0        1 2024-03-13 02:36:20.263751 guisurfer-0.1.9/guisurfer/job/env.py
+-rw-r--r--   0        0        0     2328 2024-03-14 18:27:55.610267 guisurfer-0.1.9/guisurfer/job/log.py
+-rw-r--r--   0        0        0     1305 2024-03-17 03:25:50.141307 guisurfer-0.1.9/guisurfer/server/app.py
+-rw-r--r--   0        0        0     1046 2024-03-14 04:26:30.848276 guisurfer-0.1.9/guisurfer/server/boot.py
+-rw-r--r--   0        0        0      611 2024-03-13 03:13:33.206920 guisurfer-0.1.9/guisurfer/server/hub.py
+-rw-r--r--   0        0        0     4062 2024-03-18 20:17:08.949015 guisurfer-0.1.9/guisurfer/server/key.py
+-rw-r--r--   0        0        0     5005 2024-03-18 03:34:12.196407 guisurfer-0.1.9/guisurfer/server/models.py
+-rw-r--r--   0        0        0    11070 2024-03-18 20:17:59.927644 guisurfer-0.1.9/guisurfer/server/router/agents.py
+-rw-r--r--   0        0        0     4113 2024-03-13 21:53:21.741421 guisurfer-0.1.9/guisurfer/server/router/desktops.py
+-rw-r--r--   0        0        0      802 2024-03-13 22:08:03.348200 guisurfer-0.1.9/guisurfer/server/router/job.py
+-rw-r--r--   0        0        0     1233 2024-03-13 21:50:46.751451 guisurfer-0.1.9/guisurfer/server/router/keys.py
+-rw-r--r--   0        0        0     3449 2024-03-15 03:02:12.619360 guisurfer-0.1.9/guisurfer/server/router/runtime.py
+-rw-r--r--   0        0        0     4230 2024-03-17 19:23:50.096569 guisurfer-0.1.9/guisurfer/server/router/task.py
+-rw-r--r--   0        0        0     6499 2024-03-17 18:38:15.604179 guisurfer-0.1.9/guisurfer/server/router/vnc.py
+-rw-r--r--   0        0        0     6724 2024-03-14 23:20:08.325281 guisurfer-0.1.9/guisurfer/server/runtime.py
+-rw-r--r--   0        0        0     1360 2024-03-17 00:30:04.360017 guisurfer-0.1.9/guisurfer/server/test.py
+-rw-r--r--   0        0        0      666 2024-03-18 20:18:54.061309 guisurfer-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1831 1970-01-01 00:00:00.000000 guisurfer-0.1.9/PKG-INFO
```

### Comparing `guisurfer-0.1.8/README.md` & `guisurfer-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `guisurfer-0.1.8/guisurfer/agent/base.py` & `guisurfer-0.1.9/guisurfer/agent/base.py`

 * *Files identical despite different names*

### Comparing `guisurfer-0.1.8/guisurfer/agent/runtime.py` & `guisurfer-0.1.9/guisurfer/agent/runtime.py`

 * *Files identical despite different names*

### Comparing `guisurfer-0.1.8/guisurfer/agent/task.py` & `guisurfer-0.1.9/guisurfer/agent/task.py`

 * *Files identical despite different names*

### Comparing `guisurfer-0.1.8/guisurfer/agent/types.py` & `guisurfer-0.1.9/guisurfer/agent/types.py`

 * *Files identical despite different names*

### Comparing `guisurfer-0.1.8/guisurfer/auth/key.py` & `guisurfer-0.1.9/guisurfer/auth/key.py`

 * *Files identical despite different names*

### Comparing `guisurfer-0.1.8/guisurfer/auth/provider.py` & `guisurfer-0.1.9/guisurfer/auth/provider.py`

 * *Files identical despite different names*

### Comparing `guisurfer-0.1.8/guisurfer/auth/transport.py` & `guisurfer-0.1.9/guisurfer/auth/transport.py`

 * *Files identical despite different names*

### Comparing `guisurfer-0.1.8/guisurfer/auth/user.py` & `guisurfer-0.1.9/guisurfer/auth/user.py`

 * *Files identical despite different names*

### Comparing `guisurfer-0.1.8/guisurfer/db/conn.py` & `guisurfer-0.1.9/guisurfer/db/conn.py`

 * *Files identical despite different names*

### Comparing `guisurfer-0.1.8/guisurfer/db/models.py` & `guisurfer-0.1.9/guisurfer/db/models.py`

 * *Files identical despite different names*

### Comparing `guisurfer-0.1.8/guisurfer/job/agent/job.py` & `guisurfer-0.1.9/guisurfer/job/agent/job.py`

 * *Files identical despite different names*

### Comparing `guisurfer-0.1.8/guisurfer/job/agent/k8s.py` & `guisurfer-0.1.9/guisurfer/job/agent/k8s.py`

 * *Files identical despite different names*

### Comparing `guisurfer-0.1.8/guisurfer/job/agent/main.py` & `guisurfer-0.1.9/guisurfer/job/agent/main.py`

 * *Files identical despite different names*

### Comparing `guisurfer-0.1.8/guisurfer/job/base.py` & `guisurfer-0.1.9/guisurfer/job/base.py`

 * *Files identical despite different names*

### Comparing `guisurfer-0.1.8/guisurfer/job/log.py` & `guisurfer-0.1.9/guisurfer/job/log.py`

 * *Files identical despite different names*

### Comparing `guisurfer-0.1.8/guisurfer/server/app.py` & `guisurfer-0.1.9/guisurfer/server/app.py`

 * *Files identical despite different names*

### Comparing `guisurfer-0.1.8/guisurfer/server/boot.py` & `guisurfer-0.1.9/guisurfer/server/boot.py`

 * *Files identical despite different names*

### Comparing `guisurfer-0.1.8/guisurfer/server/hub.py` & `guisurfer-0.1.9/guisurfer/server/hub.py`

 * *Files identical despite different names*

### Comparing `guisurfer-0.1.8/guisurfer/server/key.py` & `guisurfer-0.1.9/guisurfer/server/key.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     """An SSH key"""
 
     name: str
     public_key: str
     private_key: str
     owner_id: str
     created: float = field(default_factory=lambda: time.time())
-    updated: float = field(default_factory=lambda: time.time())
     id: str = field(default_factory=lambda: str(uuid.uuid4()))
     metadata: Dict[str, str] = field(default_factory=dict)
 
     def __post_init__(self) -> None:
         self.private_key = self.encrypt_private_key(self.private_key)
         self.save()
```

### Comparing `guisurfer-0.1.8/guisurfer/server/models.py` & `guisurfer-0.1.9/guisurfer/server/models.py`

 * *Files identical despite different names*

### Comparing `guisurfer-0.1.8/guisurfer/server/router/agents.py` & `guisurfer-0.1.9/guisurfer/server/router/agents.py`

 * *Files identical despite different names*

### Comparing `guisurfer-0.1.8/guisurfer/server/router/desktops.py` & `guisurfer-0.1.9/guisurfer/server/router/desktops.py`

 * *Files identical despite different names*

### Comparing `guisurfer-0.1.8/guisurfer/server/router/job.py` & `guisurfer-0.1.9/guisurfer/server/router/job.py`

 * *Files identical despite different names*

### Comparing `guisurfer-0.1.8/guisurfer/server/router/keys.py` & `guisurfer-0.1.9/guisurfer/server/router/keys.py`

 * *Files identical despite different names*

### Comparing `guisurfer-0.1.8/guisurfer/server/router/runtime.py` & `guisurfer-0.1.9/guisurfer/server/router/runtime.py`

 * *Files identical despite different names*

### Comparing `guisurfer-0.1.8/guisurfer/server/router/task.py` & `guisurfer-0.1.9/guisurfer/server/router/task.py`

 * *Files identical despite different names*

### Comparing `guisurfer-0.1.8/guisurfer/server/router/vnc.py` & `guisurfer-0.1.9/guisurfer/server/router/vnc.py`

 * *Files identical despite different names*

### Comparing `guisurfer-0.1.8/guisurfer/server/runtime.py` & `guisurfer-0.1.9/guisurfer/server/runtime.py`

 * *Files identical despite different names*

### Comparing `guisurfer-0.1.8/guisurfer/server/test.py` & `guisurfer-0.1.9/guisurfer/server/test.py`

 * *Files identical despite different names*

### Comparing `guisurfer-0.1.8/pyproject.toml` & `guisurfer-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "guisurfer"
-version = "0.1.8"
+version = "0.1.9"
 description = "GUI surfing agents"
 authors = ["Patrick Barker <patrickbarkerco@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -13,15 +13,15 @@
 fastapi = {version = "0.109.0", extras = ["all"]}
 authlib = "^1.3.0"
 asyncssh = "^2.14.2"
 namesgenerator = "^0.3"
 kubernetes = "^29.0.0"
 rich = "^13.7.1"
 websockets = "^12.0"
-agentdesk = "^0.2.34"
+agentdesk = "^0.2.35"
 
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.29.3"
 six = "^1.16.0"
 websocket-client = "^1.7.0"
```

### Comparing `guisurfer-0.1.8/PKG-INFO` & `guisurfer-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: guisurfer
-Version: 0.1.8
+Version: 0.1.9
 Summary: GUI surfing agents
 License: Apache 2.0
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: agentdesk (>=0.2.34,<0.3.0)
+Requires-Dist: agentdesk (>=0.2.35,<0.3.0)
 Requires-Dist: asyncssh (>=2.14.2,<3.0.0)
 Requires-Dist: authlib (>=1.3.0,<2.0.0)
 Requires-Dist: cryptography (>=42.0.5,<43.0.0)
 Requires-Dist: deepthread (>=0.1.5,<0.2.0)
 Requires-Dist: fastapi[all] (==0.109.0)
 Requires-Dist: kubernetes (>=29.0.0,<30.0.0)
 Requires-Dist: namesgenerator (>=0.3,<0.4)
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: guisurfer Version: 0.1.8 Summary: GUI surfing
+Metadata-Version: 2.1 Name: guisurfer Version: 0.1.9 Summary: GUI surfing
 agents License: Apache 2.0 Author: Patrick Barker Author-email:
 patrickbarkerco@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License ::
 Other/Proprietary License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: agentdesk (>=0.2.34,<0.3.0) Requires-
+Language :: Python :: 3.11 Requires-Dist: agentdesk (>=0.2.35,<0.3.0) Requires-
 Dist: asyncssh (>=2.14.2,<3.0.0) Requires-Dist: authlib (>=1.3.0,<2.0.0)
 Requires-Dist: cryptography (>=42.0.5,<43.0.0) Requires-Dist: deepthread
 (>=0.1.5,<0.2.0) Requires-Dist: fastapi[all] (==0.109.0) Requires-Dist:
 kubernetes (>=29.0.0,<30.0.0) Requires-Dist: namesgenerator (>=0.3,<0.4)
 Requires-Dist: rich (>=13.7.1,<14.0.0) Requires-Dist: websockets (>=12.0,<13.0)
 Description-Content-Type: text/markdown
                            ************ GGUUII SSuurrffeerr ************
```

