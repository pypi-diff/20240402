# Comparing `tmp/archerdfu.core-1.0.1.tar.gz` & `tmp/archerdfu.core-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archerdfu.core-1.0.1.tar", last modified: Fri Mar  1 10:32:14 2024, max compression
+gzip compressed data, was "archerdfu.core-1.0.2.tar", last modified: Tue Apr  2 07:07:25 2024, max compression
```

## Comparing `archerdfu.core-1.0.1.tar` & `archerdfu.core-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 10:32:14.146206 archerdfu.core-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35130 2024-03-01 10:32:08.000000 archerdfu.core-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    41786 2024-03-01 10:32:14.146206 archerdfu.core-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-01 10:32:08.000000 archerdfu.core-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 10:32:14.142206 archerdfu.core-1.0.1/archerdfu/
--rw-r--r--   0 runner    (1001) docker     (127)    11922 2024-03-01 10:32:08.000000 archerdfu.core-1.0.1/archerdfu/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 10:32:14.142206 archerdfu.core-1.0.1/archerdfu.core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    41786 2024-03-01 10:32:14.000000 archerdfu.core-1.0.1/archerdfu.core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-01 10:32:14.000000 archerdfu.core-1.0.1/archerdfu.core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 10:32:14.000000 archerdfu.core-1.0.1/archerdfu.core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-01 10:32:14.000000 archerdfu.core-1.0.1/archerdfu.core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-01 10:32:14.000000 archerdfu.core-1.0.1/archerdfu.core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-03-01 10:32:08.000000 archerdfu.core-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 10:32:14.146206 archerdfu.core-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-01 10:32:08.000000 archerdfu.core-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:07:25.521733 archerdfu.core-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35130 2024-04-02 07:07:19.000000 archerdfu.core-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    41786 2024-04-02 07:07:25.521733 archerdfu.core-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-02 07:07:19.000000 archerdfu.core-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:07:25.517733 archerdfu.core-1.0.2/archerdfu/
+-rw-r--r--   0 runner    (1001) docker     (127)    11841 2024-04-02 07:07:19.000000 archerdfu.core-1.0.2/archerdfu/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:07:25.521733 archerdfu.core-1.0.2/archerdfu.core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    41786 2024-04-02 07:07:25.000000 archerdfu.core-1.0.2/archerdfu.core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-02 07:07:25.000000 archerdfu.core-1.0.2/archerdfu.core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 07:07:25.000000 archerdfu.core-1.0.2/archerdfu.core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-02 07:07:25.000000 archerdfu.core-1.0.2/archerdfu.core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-02 07:07:25.000000 archerdfu.core-1.0.2/archerdfu.core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-02 07:07:19.000000 archerdfu.core-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 07:07:25.521733 archerdfu.core-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-02 07:07:19.000000 archerdfu.core-1.0.2/setup.py
```

### Comparing `archerdfu.core-1.0.1/LICENSE` & `archerdfu.core-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `archerdfu.core-1.0.1/PKG-INFO` & `archerdfu.core-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archerdfu.core
-Version: 1.0.1
+Version: 1.0.2
 Summary: PyDfuUtil binds for archerdfu library
 Author: o-murphy
 License:  GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -692,15 +692,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pydfuutil>=0.0.1b4
+Requires-Dist: pydfuutil>=0.0.2b0
 Requires-Dist: rich>=13.7.0
 
 ## archerdfu.core
 ### pydfuutil binds for archerdfu library
 
 > [NOTE!]
 > This package is part of **[archerdfu](https://github.com/archerdfu)** project
```

### Comparing `archerdfu.core-1.0.1/archerdfu/core.py` & `archerdfu.core-1.0.2/archerdfu/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 
     def dfu_init(self, dfu_timeout=None, num_connect_attempts=5):
         self.dfu_interface: usb.core.Interface | None = None
         self.dfu_descriptor: dict | None = None
 
         self.num_connect_attempts = num_connect_attempts
 
-        dfu.dfu_init(dfu_timeout if dfu_timeout else 5000)
+        dfu.init(dfu_timeout if dfu_timeout else 5000)
         # dfu.dfu_debug(logging.INFO)
 
     @property
     def dfu_intf(self) -> [int, None]:
         if self.dfu_interface is not None:
             return self.dfu_interface.bInterfaceNumber
         self.get_dfu_interface()
@@ -133,58 +133,58 @@
                 self.dfu_descriptor = dfu_desc
                 break
 
         if not self.dfu_interface:
             raise ConnectionError(f'No DFU interface found: {self._str()}')
 
     def get_status(self) -> (int, dict):
-        _, status = dfu.dfu_get_status(self, self.dfu_intf)
+        _, status = dfu.get_status(self, self.dfu_intf)
         sleep(status.bwPollTimeout)
         sleep(0.5)
         return _, status
 
     def is_connect_valid(self):
         _, status = self.get_status()
-        while status.bState != dfu.DFUState.DFU_IDLE:
+        while status.bState != dfu.State.DFU_IDLE:
 
-            if status.bState in [dfu.DFUState.APP_IDLE, dfu.DFUState.APP_DETACH]:
+            if status.bState in [dfu.State.APP_IDLE, dfu.State.APP_DETACH]:
                 return False
-            elif status.bState == dfu.DFUState.DFU_ERROR:
-                if dfu.dfu_clear_status(self, self.dfu_intf) < 0:
+            elif status.bState == dfu.State.DFU_ERROR:
+                if dfu.clear_status(self, self.dfu_intf) < 0:
                     return False
                 _, status = self.get_status()
-            elif status.bState in [dfu.DFUState.DFU_DOWNLOAD_IDLE, dfu.DFUState.DFU_UPLOAD_IDLE]:
-                if dfu.dfu_abort(self, self.dfu_intf) < 0:
+            elif status.bState in [dfu.State.DFU_DOWNLOAD_IDLE, dfu.State.DFU_UPLOAD_IDLE]:
+                if dfu.abort(self, self.dfu_intf) < 0:
                     return False
                 _, status = self.get_status()
             else:
                 break
 
-        if status.bStatus != dfu.DFUStatus.OK:
-            if dfu.dfu_clear_status(self, self.dfu_intf) < 0:
+        if status.bStatus != dfu.Status.OK:
+            if dfu.clear_status(self, self.dfu_intf) < 0:
                 return False
             _, status = self.get_status()
             if _ < 0:
                 return False
-            if status.bStatus != dfu.DFUStatus.OK:
+            if status.bStatus != dfu.Status.OK:
                 return False
             sleep(status.bwPollTimeout)
 
         return True
 
     @property
     def usb_port(self):
         port = self.port_numbers
         enc_address = ":".join(f"{num:02X}" for num in port[:6]) + ":00" * (6 - len(port))
         return enc_address
 
     def dfu_detach(self) -> int:
         detach_timeout = self.dfu_descriptor.wDetachTimeOut / 10000
         detach_timeout = math.ceil(detach_timeout)
-        dfu.dfu_detach(self, self.dfu_intf, 1000)
+        dfu.detach(self, self.dfu_intf, 1000)
         sleep(1)
         return detach_timeout
 
     def connect(self, hold_port=True):
         if self.num_connect_attempts > 0:
             self.num_connect_attempts -= 1
             self.get_dfu_interface()
@@ -272,15 +272,15 @@
             upload_task = DFU_PROGRESS.add_task(
                 task_desc_fmt.format(color='magenta1', port=self.usb_port, desc='Uploading...'),
                 total=total, callback=callback
             )
 
         while True:
 
-            rc = dfu.dfu_upload(self, self.dfu_intf, page, USB_PAGE),
+            rc = dfu.upload(self, self.dfu_intf, page, USB_PAGE),
             page += 1
 
             if len(rc[0]) < 0:
                 ret = rc
                 break
 
             DFU_PROGRESS.update(
@@ -293,15 +293,15 @@
             )
 
             ret += rc[0]
 
             if len(rc[0]) < USB_PAGE or (len(ret) >= total >= 0):
                 break
 
-        dfu.dfu_upload(self, self.dfu_intf, page, 0),
+        dfu.upload(self, self.dfu_intf, page, 0),
 
         DFU_PROGRESS.update(
             upload_task, advance=0,
             description=task_desc_fmt.format(
                 color='green', port=self.usb_port, desc='Uploading OK!'
             )
         )
@@ -324,28 +324,28 @@
             )
 
         part_num = 0
 
         while True:
 
             part = data[part_num * page_size:part_num * page_size + page_size]
-            rc = dfu.dfu_download(self, self.dfu_intf, page, part)
+            rc = dfu.download(self, self.dfu_intf, page, part)
 
             _, status = None, None
             while True:
-                _, status = dfu.dfu_get_status(self, self.dfu_intf)
+                _, status = dfu.get_status(self, self.dfu_intf)
 
                 if _ < 0:
                     return part_num * page_size + page_size
 
-                if status.bState in (dfu.DFUState.DFU_DOWNLOAD_IDLE, dfu.DFUState.DFU_ERROR):
+                if status.bState in (dfu.State.DFU_DOWNLOAD_IDLE, dfu.State.DFU_ERROR):
                     break
 
-            if status.bStatus != dfu.DFUStatus.OK:
-                raise IOError(dfu.dfu_state_to_string(status.bState))
+            if status.bStatus != dfu.Status.OK:
+                raise IOError(dfu.state_to_string(status.bState))
 
             page += 1
             part_num += 1
 
             if rc < 0:
                 ret = rc
                 break
@@ -360,15 +360,15 @@
             )
 
             ret += rc
 
             if rc < page_size or ret >= total >= 0:
                 break
 
-        dfu.dfu_download(self, self.dfu_intf, page, 0),
+        dfu.download(self, self.dfu_intf, page, 0),
 
         DFU_PROGRESS.update(
             download_task, advance=0,
             description=task_desc_fmt.format(
                 color='deep_sky_blue1', port=self.usb_port, desc='Downloading OK!'
             )
         )
```

### Comparing `archerdfu.core-1.0.1/archerdfu.core.egg-info/PKG-INFO` & `archerdfu.core-1.0.2/archerdfu.core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archerdfu.core
-Version: 1.0.1
+Version: 1.0.2
 Summary: PyDfuUtil binds for archerdfu library
 Author: o-murphy
 License:  GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -692,15 +692,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pydfuutil>=0.0.1b4
+Requires-Dist: pydfuutil>=0.0.2b0
 Requires-Dist: rich>=13.7.0
 
 ## archerdfu.core
 ### pydfuutil binds for archerdfu library
 
 > [NOTE!]
 > This package is part of **[archerdfu](https://github.com/archerdfu)** project
```

### Comparing `archerdfu.core-1.0.1/pyproject.toml` & `archerdfu.core-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "archerdfu.core"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
     { name="o-murphy" },
 ]
 
 description = "PyDfuUtil binds for archerdfu library"
 readme = "README.md"
 requires-python = ">=3.9"
@@ -25,15 +25,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
 ]
 dependencies = [
-    'pydfuutil>=0.0.1b4',
+    'pydfuutil>=0.0.2b0',
     'rich>=13.7.0'
 ]
 
 
 [project.urls]
 "Homepage" = "https://github.com/archerdfu/archerdfu.core"
 "Bug Reports" = "https://github.com/archerdfu/archerdfu.core/issues"
```

