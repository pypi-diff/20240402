# Comparing `tmp/cheeselog-0.3.1.tar.gz` & `tmp/cheeselog-0.3.2.tar.gz`

## Comparing `cheeselog-0.3.1.tar` & `cheeselog-0.3.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cheeselog-0.3.1/CheeseLog/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 cheeselog-0.3.1/CheeseLog/level.py
--rw-r--r--   0        0        0     9876 2020-02-02 00:00:00.000000 cheeselog-0.3.1/CheeseLog/logger.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 cheeselog-0.3.1/CheeseLog/progressBar.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 cheeselog-0.3.1/CheeseLog/style.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 cheeselog-0.3.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeselog-0.3.1/LICENSE
--rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 cheeselog-0.3.1/README.md
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 cheeselog-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 cheeselog-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cheeselog-0.3.2/CheeseLog/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 cheeselog-0.3.2/CheeseLog/level.py
+-rw-r--r--   0        0        0     9834 2020-02-02 00:00:00.000000 cheeselog-0.3.2/CheeseLog/logger.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 cheeselog-0.3.2/CheeseLog/progressBar.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 cheeselog-0.3.2/CheeseLog/style.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 cheeselog-0.3.2/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeselog-0.3.2/LICENSE
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 cheeselog-0.3.2/README.md
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 cheeselog-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 cheeselog-0.3.2/PKG-INFO
```

### Comparing `cheeselog-0.3.1/CheeseLog/logger.py` & `cheeselog-0.3.2/CheeseLog/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-import inspect, datetime, sys, re, os, multiprocessing, queue, time
+import inspect, datetime, sys, re, os, multiprocessing, time
 from typing import Dict, Set
+from multiprocessing.synchronize import Event
 
-import setproctitle, psutil
+import setproctitle
 
 from CheeseLog import style
 from CheeseLog.level import Level
 
 class Logger:
     def __init__(self):
         self.messageTemplate: str = '(%l) %t > %c'
@@ -36,47 +37,42 @@
 
         self.styled: bool = True
 
         self._filePath: str = ''
         self.fileExpire: datetime.timedelta = datetime.timedelta(seconds = 0)
 
         self._processHandler: multiprocessing.Process | None = None
+        self._event: Event = multiprocessing.Event()
         self._queue: multiprocessing.Queue = multiprocessing.Queue()
 
     def _processHandle(self):
         setproctitle.setproctitle(setproctitle.getproctitle() + ':CheeseLog')
 
-        flag = True
-        parentProcess = psutil.Process(os.getppid())
-
-        while flag or not self._queue.empty():
+        while not self._event.is_set():
             try:
                 if self.fileExpire.total_seconds():
                     try:
                         fileExpire = (datetime.datetime.now() - self.fileExpire).strftime(self.filePath)
                         os.remove(fileExpire)
                     except:
                         ...
 
-                data = self._queue.get(timeout = 0.016)
+                data = self._queue.get()
                 message = data[2].strftime(data[3].replace('%l', data[0]).replace('%c', data[1]).replace('%t', data[4])).replace('\n', '\n    ').replace('&lt;', '<').replace('&gt;', '>') + '\n'
 
                 try:
                     filePath = time.strftime(self.filePath)
                 except:
                     filePath = self.filePath
 
                 os.makedirs(os.path.dirname(filePath), exist_ok = True)
                 with open(filePath, 'a', encoding = 'utf-8') as f:
                     f.write(message)
-            except queue.Empty:
-                if not parentProcess.is_running():
-                    flag = False
             except KeyboardInterrupt:
-                flag = False
+                ...
 
     def default(self, level: str, message: str, styledMessage: str | None = None, *, end: str = '\n', refreshed: bool = False):
         if level not in self.levels:
             raise KeyError('No level with this key')
 
         if self.levels[level].weight < self.weightFilter:
             return
@@ -113,43 +109,45 @@
                 _message = re.sub(r'<.+?>', lambda s: '\033[' + getattr(style, s[0][1:-1].upper())[0] + 'm', re.sub(r'</.+?>', lambda s: '\033[' + getattr(style, s[0][2:-1].upper())[1] + 'm', now.strftime((self.levels[level].styledMessageTemplate or self.styledMessageTemplate).replace('%l', level).replace('%c', styledMessage or message).replace('%t', self.timerTemplate)))).replace('\n', '\n    ')
             else:
                 _message = now.strftime((self.levels[level].messageTemplate or self.messageTemplate).replace('%l', level).replace('%c', message).replace('%t', self.timerTemplate)).replace('\n', '\n    ')
             if refreshed:
                 _message = '\033[F\033[K' + _message
             print(_message.replace('&lt;', '<').replace('&gt;', '>'), end = end)
 
-        if self.filePath:
-            if self.levels[level].weight < self.logger_weightFilter:
-                return
+        if not self.filePath:
+            return
 
-            if level in self.logger_levelFilter:
-                return
+        if self.levels[level].weight < self.logger_weightFilter:
+            return
 
-            if self.logger_moduleFilter:
-                for key, value in self.logger_moduleFilter.items():
-                    flag = False
-                    for frame in stack:
-                        callingModule = frame.frame.f_locals.get('__name__')
-                        if callingModule and callingModule == key:
-                            flag = True
-                            if isinstance(value, int):
-                                if self.levels[level].weight <= value:
-                                    return
-                            elif isinstance(value, Set):
-                                if level in value:
-                                    return
-                            break
-                    if flag:
+        if level in self.logger_levelFilter:
+            return
+
+        if self.logger_moduleFilter:
+            for key, value in self.logger_moduleFilter.items():
+                flag = False
+                for frame in stack:
+                    callingModule = frame.frame.f_locals.get('__name__')
+                    if callingModule and callingModule == key:
+                        flag = True
+                        if isinstance(value, int):
+                            if self.levels[level].weight <= value:
+                                return
+                        elif isinstance(value, Set):
+                            if level in value:
+                                return
                         break
+                if flag:
+                    break
 
-            for pattern in self.logger_contentFilter:
-                if re.search(pattern, message):
-                    return
+        for pattern in self.logger_contentFilter:
+            if re.search(pattern, message):
+                return
 
-            self._queue.put((level, message, now, self.levels[level].messageTemplate or self.messageTemplate, self.timerTemplate))
+        self._queue.put((level, message, now, self.levels[level].messageTemplate or self.messageTemplate, self.timerTemplate))
 
     def debug(self, message: str, styledMessage: str | None = None, *, end: str = '\n', refreshed: bool = False):
         self.default('DEBUG', message, styledMessage, end = end, refreshed = refreshed)
 
     def info(self, message: str, styledMessage: str | None = None, *, end: str = '\n', refreshed: bool = False):
         self.default('INFO', message, styledMessage, end = end, refreshed = refreshed)
 
@@ -179,24 +177,31 @@
 
     def loading(self, message: str, styledMessage: str | None = None, *, end: str = '\n', refreshed: bool = True):
         self.default('LOADING', message, styledMessage, end = end, refreshed = refreshed)
 
     def encode(self, message: str) -> str:
         return message.replace('<', '&lt;').replace('>', '&gt;').replace('%', '%%')
 
+    def destroy(self):
+        self._event.set()
+        self._processHandler.join()
+        self._event.clear()
+        self._processHandler = None
+
     @property
     def filePath(self) -> str:
         return self._filePath
 
     @filePath.setter
     def filePath(self, value: str):
         self._filePath = value
 
         if self.filePath and not self._processHandler:
             self._processHandler = multiprocessing.Process(target = self._processHandle, name = setproctitle.getproctitle() + ':CheeseLog')
             self._processHandler.start()
         elif not self.filePath and self._processHandler:
-            self._processHandler.terminate()
+            self._event.set()
             self._processHandler.join()
+            self._event.clear()
             self._processHandler = None
 
 logger = Logger()
```

### Comparing `cheeselog-0.3.1/CheeseLog/progressBar.py` & `cheeselog-0.3.2/CheeseLog/progressBar.py`

 * *Files identical despite different names*

### Comparing `cheeselog-0.3.1/CheeseLog/style.py` & `cheeselog-0.3.2/CheeseLog/style.py`

 * *Files identical despite different names*

### Comparing `cheeselog-0.3.1/LICENSE` & `cheeselog-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cheeselog-0.3.1/README.md` & `cheeselog-0.3.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -64,14 +64,16 @@
 
 logger.filePath = './myLog.log'
 
 logger.debug('Hello World')
 # 中途修改输出日志是可以的
 logger.filePath = './yourLog.log'
 logger.debug('Hello World')
+
+logger.destroy() # 使用输出日志功能后请使用该函数摧毁
 ```
 
 ### **消息过滤**
 
 更多消息过滤信息请看[Logger](https://github.com/CheeseUnknown/CheeseLog/blob/master/documents/Logger.md)。
 
 更多消息等级信息请看[Level](https://github.com/CheeseUnknown/CheeseLog/blob/master/documents/Level.md)。
```

### Comparing `cheeselog-0.3.1/pyproject.toml` & `cheeselog-0.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [build-system]
 requires = [ "hatchling" ]
 build-backend = "hatchling.build"
 
 [project]
 name = "CheeseLog"
-version = "0.3.1"
+version = "0.3.2"
 description = "日志系统。可在控制台输出一定格式的、可选颜色的内容，并支持写入指定的日志文件。"
 readme = "README.md"
 license-files = { paths = [ "LICENSE" ] }
 authors = [
     { name = "Cheese Unknown", email = "cheese@cheese.ren" }
 ]
 keywords = [ 'log', 'logger' ]
 
 dependencies = [
-    "setproctitle",
-    "psutil"
+    "setproctitle"
 ]
 
 [project.urls]
 Source = "https://github.com/CheeseUnknown/CheeseLog"
 
 [tool.hatch.build.targets.sdist]
 include = [ "/CheeseLog" ]
```

### Comparing `cheeselog-0.3.1/PKG-INFO` & `cheeselog-0.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.3
 Name: CheeseLog
-Version: 0.3.1
+Version: 0.3.2
 Summary: 日志系统。可在控制台输出一定格式的、可选颜色的内容，并支持写入指定的日志文件。
 Project-URL: Source, https://github.com/CheeseUnknown/CheeseLog
 Author-email: Cheese Unknown <cheese@cheese.ren>
 License-File: LICENSE
 Keywords: log,logger
-Requires-Dist: psutil
 Requires-Dist: setproctitle
 Description-Content-Type: text/markdown
 
 # **CheeseLog**
 
 ## **介绍**
 
@@ -76,14 +75,16 @@
 
 logger.filePath = './myLog.log'
 
 logger.debug('Hello World')
 # 中途修改输出日志是可以的
 logger.filePath = './yourLog.log'
 logger.debug('Hello World')
+
+logger.destroy() # 使用输出日志功能后请使用该函数摧毁
 ```
 
 ### **消息过滤**
 
 更多消息过滤信息请看[Logger](https://github.com/CheeseUnknown/CheeseLog/blob/master/documents/Logger.md)。
 
 更多消息等级信息请看[Level](https://github.com/CheeseUnknown/CheeseLog/blob/master/documents/Level.md)。
```

