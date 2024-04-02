# Comparing `tmp/antfyutils-0.0.3.tar.gz` & `tmp/antfyutils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antfyutils-0.0.3.tar", last modified: Sun Mar 31 14:23:34 2024, max compression
+gzip compressed data, was "antfyutils-0.0.4.tar", last modified: Tue Apr  2 08:30:58 2024, max compression
```

## Comparing `antfyutils-0.0.3.tar` & `antfyutils-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 14:23:34.086676 antfyutils-0.0.3/
--rw-r--r--   0 root         (0) root         (0)      177 2024-03-31 14:23:34.086676 antfyutils-0.0.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 14:23:34.082676 antfyutils-0.0.3/antfyutils/
--rw-r--r--   0 root         (0) root         (0)      115 2024-03-31 14:22:59.000000 antfyutils-0.0.3/antfyutils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1662 2024-03-31 14:22:59.000000 antfyutils-0.0.3/antfyutils/data_obj.py
--rw-r--r--   0 root         (0) root         (0)     2176 2024-03-31 10:25:33.000000 antfyutils-0.0.3/antfyutils/format.py
--rw-r--r--   0 root         (0) root         (0)     1662 2024-03-31 10:25:33.000000 antfyutils-0.0.3/antfyutils/obj.py
--rw-r--r--   0 root         (0) root         (0)     3621 2024-03-31 14:22:59.000000 antfyutils-0.0.3/antfyutils/push_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 14:23:34.086676 antfyutils-0.0.3/antfyutils.egg-info/
--rw-r--r--   0 root         (0) root         (0)      177 2024-03-31 14:23:34.000000 antfyutils-0.0.3/antfyutils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      293 2024-03-31 14:23:34.000000 antfyutils-0.0.3/antfyutils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-31 14:23:34.000000 antfyutils-0.0.3/antfyutils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-03-31 14:23:34.000000 antfyutils-0.0.3/antfyutils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-03-31 14:23:34.000000 antfyutils-0.0.3/antfyutils.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      258 2024-03-31 14:22:59.000000 antfyutils-0.0.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-31 14:23:34.086676 antfyutils-0.0.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 08:30:58.748092 antfyutils-0.0.4/
+-rw-r--r--   0 root         (0) root         (0)      177 2024-04-02 08:30:58.748092 antfyutils-0.0.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 08:30:58.744092 antfyutils-0.0.4/antfyutils/
+-rw-r--r--   0 root         (0) root         (0)      115 2024-03-31 14:22:59.000000 antfyutils-0.0.4/antfyutils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2024-03-31 14:22:59.000000 antfyutils-0.0.4/antfyutils/data_obj.py
+-rw-r--r--   0 root         (0) root         (0)     2176 2024-03-31 10:25:33.000000 antfyutils-0.0.4/antfyutils/format.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2024-03-31 10:25:33.000000 antfyutils-0.0.4/antfyutils/obj.py
+-rw-r--r--   0 root         (0) root         (0)     3693 2024-04-02 08:30:24.000000 antfyutils-0.0.4/antfyutils/push_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 08:30:58.748092 antfyutils-0.0.4/antfyutils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      177 2024-04-02 08:30:58.000000 antfyutils-0.0.4/antfyutils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      293 2024-04-02 08:30:58.000000 antfyutils-0.0.4/antfyutils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 08:30:58.000000 antfyutils-0.0.4/antfyutils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-02 08:30:58.000000 antfyutils-0.0.4/antfyutils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-02 08:30:58.000000 antfyutils-0.0.4/antfyutils.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      258 2024-04-02 08:30:24.000000 antfyutils-0.0.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 08:30:58.748092 antfyutils-0.0.4/setup.cfg
```

### Comparing `antfyutils-0.0.3/antfyutils/data_obj.py` & `antfyutils-0.0.4/antfyutils/data_obj.py`

 * *Files identical despite different names*

### Comparing `antfyutils-0.0.3/antfyutils/format.py` & `antfyutils-0.0.4/antfyutils/format.py`

 * *Files identical despite different names*

### Comparing `antfyutils-0.0.3/antfyutils/obj.py` & `antfyutils-0.0.4/antfyutils/obj.py`

 * *Files identical despite different names*

### Comparing `antfyutils-0.0.3/antfyutils/push_utils.py` & `antfyutils-0.0.4/antfyutils/push_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,15 +53,17 @@
     def stopServer(self):
         if self.thread:
             self.pool.put_nowait(None)
             self.eventloop.stop()
             self.thread.join(timeout=5)
         pass
     def push(self, msg:SendNtfyMessage):
-        self.pool.put_nowait(msg)
+        def put():
+            self.pool.put_nowait(msg)
+        self.eventloop.call_soon_threadsafe(put)
     async def __push(self, msg: SendNtfyMessage):
         if not msg.topic:
             msg.topic = self.cfg.topic
         count = 0
         while True:
             count += 1
             if count >=3:
```

