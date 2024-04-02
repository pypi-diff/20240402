# Comparing `tmp/vxutils-20240331.tar.gz` & `tmp/vxutils-20240401.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vxutils-20240331.tar", max compression
+gzip compressed data, was "vxutils-20240401.tar", max compression
```

## Comparing `vxutils-20240331.tar` & `vxutils-20240401.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1998 2024-03-31 01:59:38.802957 vxutils-20240331/pyproject.toml
--rw-r--r--   0        0        0       24 2024-02-28 02:40:58.487414 vxutils-20240331/README.md
--rw-r--r--   0        0        0      418 2024-03-31 05:45:56.658824 vxutils-20240331/src/vxsched/__init__.py
--rw-r--r--   0        0        0     1370 2024-03-31 05:45:50.712223 vxutils-20240331/src/vxsched/__main__.py
--rw-r--r--   0        0        0     7776 2024-03-15 02:21:02.576581 vxutils-20240331/src/vxsched/core.py
--rw-r--r--   0        0        0    11734 2024-03-07 05:59:56.919198 vxutils-20240331/src/vxsched/event.py
--rw-r--r--   0        0        0        0 2024-03-07 06:18:59.347092 vxutils-20240331/src/vxsched/py.typed
--rw-r--r--   0        0        0     1199 2024-03-07 03:35:33.730867 vxutils-20240331/src/vxsched/subpubs.py
--rw-r--r--   0        0        0     1307 2024-03-31 05:45:44.565049 vxutils-20240331/src/vxutils/__init__.py
--rw-r--r--   0        0        0     3738 2024-03-31 05:45:39.670502 vxutils-20240331/src/vxutils/context.py
--rw-r--r--   0        0        0     9225 2024-02-20 02:25:26.235753 vxutils-20240331/src/vxutils/convertors.py
--rw-r--r--   0        0        0        0 2024-02-17 13:24:20.316286 vxutils-20240331/src/vxutils/datamodel/__init__.py
--rw-r--r--   0        0        0     4214 2024-02-18 02:09:20.092983 vxutils-20240331/src/vxutils/datamodel/adapter.py
--rw-r--r--   0        0        0     2369 2024-03-07 04:24:54.189680 vxutils-20240331/src/vxutils/datamodel/core.py
--rw-r--r--   0        0        0    15247 2024-03-12 05:04:59.968100 vxutils-20240331/src/vxutils/datamodel/dborm.py
--rw-r--r--   0        0        0     7973 2024-03-15 02:15:36.559220 vxutils-20240331/src/vxutils/decorators.py
--rw-r--r--   0        0        0     5365 2024-03-11 02:27:17.709011 vxutils-20240331/src/vxutils/dtutils.py
--rw-r--r--   0        0        0     7344 2024-03-31 03:46:11.067709 vxutils-20240331/src/vxutils/logger.py
--rw-r--r--   0        0        0    14529 2024-02-20 08:56:31.979240 vxutils-20240331/src/vxutils/networking/requests.py
--rw-r--r--   0        0        0     7987 2024-03-31 01:34:06.580192 vxutils-20240331/src/vxutils/networking/wechat.py
--rw-r--r--   0        0        0     6173 2024-03-15 02:47:00.420052 vxutils-20240331/src/vxutils/provider.py
--rw-r--r--   0        0        0        0 2024-02-15 15:46:34.000000 vxutils-20240331/src/vxutils/py.typed
--rw-r--r--   0        0        0      446 2024-03-10 03:13:04.515372 vxutils-20240331/src/vxutils/typehints.py
--rw-r--r--   0        0        0     1067 1970-01-01 00:00:00.000000 vxutils-20240331/PKG-INFO
+-rw-r--r--   0        0        0     1998 2024-04-02 03:12:27.344434 vxutils-20240401/pyproject.toml
+-rw-r--r--   0        0        0       24 2024-02-28 02:40:58.487414 vxutils-20240401/README.md
+-rw-r--r--   0        0        0      421 2024-04-02 02:11:16.355963 vxutils-20240401/src/vxsched/__init__.py
+-rw-r--r--   0        0        0     1370 2024-03-31 05:45:50.712223 vxutils-20240401/src/vxsched/__main__.py
+-rw-r--r--   0        0        0     7776 2024-03-15 02:21:02.576581 vxutils-20240401/src/vxsched/core.py
+-rw-r--r--   0        0        0    11734 2024-03-07 05:59:56.919198 vxutils-20240401/src/vxsched/event.py
+-rw-r--r--   0        0        0        0 2024-03-07 06:18:59.347092 vxutils-20240401/src/vxsched/py.typed
+-rw-r--r--   0        0        0     1202 2024-04-02 02:11:10.194079 vxutils-20240401/src/vxsched/subpubs.py
+-rw-r--r--   0        0        0     1307 2024-03-31 05:45:44.565049 vxutils-20240401/src/vxutils/__init__.py
+-rw-r--r--   0        0        0     3738 2024-03-31 05:45:39.670502 vxutils-20240401/src/vxutils/context.py
+-rw-r--r--   0        0        0     9225 2024-02-20 02:25:26.235753 vxutils-20240401/src/vxutils/convertors.py
+-rw-r--r--   0        0        0        0 2024-02-17 13:24:20.316286 vxutils-20240401/src/vxutils/datamodel/__init__.py
+-rw-r--r--   0        0        0     4214 2024-02-18 02:09:20.092983 vxutils-20240401/src/vxutils/datamodel/adapter.py
+-rw-r--r--   0        0        0     2369 2024-03-07 04:24:54.189680 vxutils-20240401/src/vxutils/datamodel/core.py
+-rw-r--r--   0        0        0    15247 2024-03-12 05:04:59.968100 vxutils-20240401/src/vxutils/datamodel/dborm.py
+-rw-r--r--   0        0        0     7849 2024-04-02 03:12:05.121190 vxutils-20240401/src/vxutils/decorators.py
+-rw-r--r--   0        0        0     5365 2024-03-11 02:27:17.709011 vxutils-20240401/src/vxutils/dtutils.py
+-rw-r--r--   0        0        0     7344 2024-03-31 03:46:11.067709 vxutils-20240401/src/vxutils/logger.py
+-rw-r--r--   0        0        0    14529 2024-02-20 08:56:31.979240 vxutils-20240401/src/vxutils/networking/requests.py
+-rw-r--r--   0        0        0     7987 2024-03-31 01:34:06.580192 vxutils-20240401/src/vxutils/networking/wechat.py
+-rw-r--r--   0        0        0     6173 2024-03-15 02:47:00.420052 vxutils-20240401/src/vxutils/provider.py
+-rw-r--r--   0        0        0        0 2024-02-15 15:46:34.000000 vxutils-20240401/src/vxutils/py.typed
+-rw-r--r--   0        0        0      446 2024-03-10 03:13:04.515372 vxutils-20240401/src/vxutils/typehints.py
+-rw-r--r--   0        0        0     1067 1970-01-01 00:00:00.000000 vxutils-20240401/PKG-INFO
```

### Comparing `vxutils-20240331/pyproject.toml` & `vxutils-20240401/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vxutils"
-version = "20240331"
+version = "20240401"
 description = "python 常用工具箱"
 license = "MIT"
 authors = ["vex1023 <vex1023@qq.com>"]
 homepage = "https://gitee.com/vxquant/vxutils"
 keywords = ["quant", "tools"]
 readme = "README.md"
```

### Comparing `vxutils-20240331/src/vxsched/__main__.py` & `vxutils-20240401/src/vxsched/__main__.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240331/src/vxsched/core.py` & `vxutils-20240401/src/vxsched/core.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240331/src/vxsched/event.py` & `vxutils-20240401/src/vxsched/event.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240331/src/vxsched/subpubs.py` & `vxutils-20240401/src/vxsched/subpubs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """事件处理器模块"""
 
 import logging
 from typing import Any, Optional, Union, Dict
 from vxsched.event import VXEventQueue, VXEvent, VXTrigger
 
 
-class VXSubscribe:
+class VXSubscriber:
     """订阅器"""
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         pass
 
     def __call__(self) -> VXEvent:
         raise NotImplementedError
 
 
-class VXPublish:
+class VXPublisher:
     """发布器"""
 
     def __init__(self, event_queue: VXEventQueue) -> None:
         self._queue = event_queue
 
     def __call__(
         self,
```

### Comparing `vxutils-20240331/src/vxutils/__init__.py` & `vxutils-20240401/src/vxutils/__init__.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240331/src/vxutils/context.py` & `vxutils-20240401/src/vxutils/context.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240331/src/vxutils/convertors.py` & `vxutils-20240401/src/vxutils/convertors.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240331/src/vxutils/datamodel/adapter.py` & `vxutils-20240401/src/vxutils/datamodel/adapter.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240331/src/vxutils/datamodel/core.py` & `vxutils-20240401/src/vxutils/datamodel/core.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240331/src/vxutils/datamodel/dborm.py` & `vxutils-20240401/src/vxutils/datamodel/dborm.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240331/src/vxutils/decorators.py` & `vxutils-20240401/src/vxutils/decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -206,19 +206,17 @@
 _NOSET = object()
 
 
 class VXAsyncResult:
     def __init__(
         self,
         async_result: Future,
-        on_error: Literal["ignore", "logging", "raise"] = "logging",
     ) -> None:
         self._future = async_result
         self._result = _NOSET
-        self._on_error = on_error
 
     def result(self) -> Any:
         """运行结果
 
         Returns:
             Any -- 运行结果
         """
@@ -247,56 +245,60 @@
     """
 
     __executor__ = ThreadPoolExecutor(thread_name_prefix="async_task")
 
     def __init__(
         self,
         max_workers: int = 5,
-        on_error: Literal["ignore", "raise", "logging"] = "logging",
+        on_error: Literal["ignore", "raise"] = "raise",
     ) -> None:
         self._semaphore = Semaphore(max_workers)
         self._on_error = on_error
 
     def __call__(self, func: Callable[..., Any]) -> Callable[..., Any]:
 
         def semaphore_func(*args: Any, **kwargs: Any) -> Any:
             with self._semaphore:
                 try:
                     return func(*args, **kwargs)
                 except Exception as err:
+                    logging.error(
+                        "async_task error: %s",
+                        err,
+                        exc_info=True,
+                        stack_info=True,
+                    )
                     if self._on_error == "raise":
-                        raise err
-                    elif self._on_error == "logging":
-                        logging.error(
-                            "async_task error: %s",
-                            err,
-                            exc_info=True,
-                            stack_info=True,
-                        )
+                        raise err from err
+
                     return None
 
         @wraps(func)
         def wrapper(*args: Any, **kwargs: Any) -> VXAsyncResult:
             fn = self.__executor__.submit(semaphore_func, *args, **kwargs)
-            return VXAsyncResult(fn, self._on_error)
+            return VXAsyncResult(fn)
 
         return wrapper
 
+    @property
+    def executor(self) -> ThreadPoolExecutor:
+        return self.__executor__
+
     @classmethod
     def set_executor(cls, executor: ThreadPoolExecutor) -> None:
         try:
             cls.__executor__.shutdown()
             cls.__executor__ = executor
         except Exception as err:
             logging.error("set executor error: %s", err, exc_info=True)
 
 
 if __name__ == "__main__":
 
-    @async_task(on_error="logging")
+    @async_task()
     def test(i: int) -> int:
         print("test", i, end="\n")
         time.sleep(1)
         return i + 1
 
     results = [test(i) for i in range(10)]
     print([result for result in results])
```

### Comparing `vxutils-20240331/src/vxutils/dtutils.py` & `vxutils-20240401/src/vxutils/dtutils.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240331/src/vxutils/logger.py` & `vxutils-20240401/src/vxutils/logger.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240331/src/vxutils/networking/requests.py` & `vxutils-20240401/src/vxutils/networking/requests.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240331/src/vxutils/networking/wechat.py` & `vxutils-20240401/src/vxutils/networking/wechat.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240331/src/vxutils/provider.py` & `vxutils-20240401/src/vxutils/provider.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240331/PKG-INFO` & `vxutils-20240401/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vxutils
-Version: 20240331
+Version: 20240401
 Summary: python 常用工具箱
 Home-page: https://gitee.com/vxquant/vxutils
 License: MIT
 Keywords: quant,tools
 Author: vex1023
 Author-email: vex1023@qq.com
 Requires-Python: >=3.8,<4.0
```

