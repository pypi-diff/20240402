# Comparing `tmp/lljz_tools-0.2.5.tar.gz` & `tmp/lljz_tools-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lljz_tools-0.2.5.tar", last modified: Tue Apr  2 10:00:32 2024, max compression
+gzip compressed data, was "lljz_tools-0.2.6.tar", last modified: Tue Apr  2 10:37:34 2024, max compression
```

## Comparing `lljz_tools-0.2.5.tar` & `lljz_tools-0.2.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 10:00:32.872407 lljz_tools-0.2.5/
--rw-rw-rw-   0        0        0     1073 2024-02-02 08:09:22.000000 lljz_tools-0.2.5/LICENSE
--rw-rw-rw-   0        0        0     4233 2024-04-02 10:00:32.871407 lljz_tools-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     3755 2024-02-03 07:02:42.000000 lljz_tools-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 10:00:32.855408 lljz_tools-0.2.5/lljz_tools.egg-info/
--rw-rw-rw-   0        0        0     4233 2024-04-02 10:00:32.000000 lljz_tools-0.2.5/lljz_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      511 2024-04-02 10:00:32.000000 lljz_tools-0.2.5/lljz_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 10:00:32.000000 lljz_tools-0.2.5/lljz_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-04-02 10:00:32.000000 lljz_tools-0.2.5/lljz_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-02 10:00:32.000000 lljz_tools-0.2.5/lljz_tools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-02 10:00:32.863407 lljz_tools-0.2.5/my_tools/
--rw-rw-rw-   0        0        0      179 2024-02-02 08:07:00.000000 lljz_tools-0.2.5/my_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 10:00:32.866407 lljz_tools-0.2.5/my_tools/attribute_dict/
--rw-rw-rw-   0        0        0      261 2024-02-03 06:30:03.000000 lljz_tools-0.2.5/my_tools/attribute_dict/__init__.py
--rw-rw-rw-   0        0        0     5886 2024-02-03 06:29:33.000000 lljz_tools-0.2.5/my_tools/attribute_dict/model.py
-drwxrwxrwx   0        0        0        0 2024-04-02 10:00:32.870408 lljz_tools-0.2.5/my_tools/client/
--rw-rw-rw-   0        0        0      179 2024-02-08 04:17:05.000000 lljz_tools-0.2.5/my_tools/client/__init__.py
--rw-rw-rw-   0        0        0     5155 2024-02-28 03:49:18.000000 lljz_tools-0.2.5/my_tools/client/db_client.py
--rw-rw-rw-   0        0        0      432 2024-02-28 06:33:46.000000 lljz_tools-0.2.5/my_tools/client/http_client.py
--rw-rw-rw-   0        0        0     1417 2024-04-02 09:57:01.000000 lljz_tools-0.2.5/my_tools/color.py
--rw-rw-rw-   0        0        0     2486 2024-04-02 09:58:38.000000 lljz_tools-0.2.5/my_tools/console_table.py
--rw-rw-rw-   0        0        0     5328 2024-02-28 03:20:05.000000 lljz_tools-0.2.5/my_tools/decorators.py
--rw-rw-rw-   0        0        0     3659 2024-02-29 18:00:07.000000 lljz_tools-0.2.5/my_tools/excel.py
--rw-rw-rw-   0        0        0     4332 2024-02-22 09:50:16.000000 lljz_tools-0.2.5/my_tools/log_manager.py
--rw-rw-rw-   0        0        0     1595 2024-02-22 09:50:16.000000 lljz_tools-0.2.5/my_tools/monkey.py
--rw-rw-rw-   0        0        0       85 2024-04-02 10:00:32.874410 lljz_tools-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      684 2024-04-02 10:00:10.000000 lljz_tools-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:37:34.881381 lljz_tools-0.2.6/
+-rw-rw-rw-   0        0        0     1073 2024-02-02 08:09:22.000000 lljz_tools-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0     4233 2024-04-02 10:37:34.881381 lljz_tools-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3755 2024-02-03 07:02:42.000000 lljz_tools-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 10:37:34.868378 lljz_tools-0.2.6/lljz_tools.egg-info/
+-rw-rw-rw-   0        0        0     4233 2024-04-02 10:37:34.000000 lljz_tools-0.2.6/lljz_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      511 2024-04-02 10:37:34.000000 lljz_tools-0.2.6/lljz_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 10:37:34.000000 lljz_tools-0.2.6/lljz_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-04-02 10:37:34.000000 lljz_tools-0.2.6/lljz_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-02 10:37:34.000000 lljz_tools-0.2.6/lljz_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 10:37:34.875379 lljz_tools-0.2.6/my_tools/
+-rw-rw-rw-   0        0        0      179 2024-02-02 08:07:00.000000 lljz_tools-0.2.6/my_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:37:34.877379 lljz_tools-0.2.6/my_tools/attribute_dict/
+-rw-rw-rw-   0        0        0      261 2024-02-03 06:30:03.000000 lljz_tools-0.2.6/my_tools/attribute_dict/__init__.py
+-rw-rw-rw-   0        0        0     5886 2024-02-03 06:29:33.000000 lljz_tools-0.2.6/my_tools/attribute_dict/model.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:37:34.880378 lljz_tools-0.2.6/my_tools/client/
+-rw-rw-rw-   0        0        0      179 2024-02-08 04:17:05.000000 lljz_tools-0.2.6/my_tools/client/__init__.py
+-rw-rw-rw-   0        0        0     5155 2024-02-28 03:49:18.000000 lljz_tools-0.2.6/my_tools/client/db_client.py
+-rw-rw-rw-   0        0        0      432 2024-02-28 06:33:46.000000 lljz_tools-0.2.6/my_tools/client/http_client.py
+-rw-rw-rw-   0        0        0     1417 2024-04-02 09:57:01.000000 lljz_tools-0.2.6/my_tools/color.py
+-rw-rw-rw-   0        0        0     2486 2024-04-02 09:58:38.000000 lljz_tools-0.2.6/my_tools/console_table.py
+-rw-rw-rw-   0        0        0     5328 2024-02-28 03:20:05.000000 lljz_tools-0.2.6/my_tools/decorators.py
+-rw-rw-rw-   0        0        0     3659 2024-02-29 18:00:07.000000 lljz_tools-0.2.6/my_tools/excel.py
+-rw-rw-rw-   0        0        0     5180 2024-04-02 10:36:48.000000 lljz_tools-0.2.6/my_tools/log_manager.py
+-rw-rw-rw-   0        0        0     1595 2024-02-22 09:50:16.000000 lljz_tools-0.2.6/my_tools/monkey.py
+-rw-rw-rw-   0        0        0       85 2024-04-02 10:37:34.883380 lljz_tools-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      684 2024-04-02 10:37:33.000000 lljz_tools-0.2.6/setup.py
```

### Comparing `lljz_tools-0.2.5/LICENSE` & `lljz_tools-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lljz_tools-0.2.5/PKG-INFO` & `lljz_tools-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lljz_tools
-Version: 0.2.5
+Version: 0.2.6
 Summary: 常用工具封装
 Home-page: 
 Author: liulangjuanzhou
 Author-email: liulangjuanzhou@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lljz_tools-0.2.5/README.md` & `lljz_tools-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `lljz_tools-0.2.5/lljz_tools.egg-info/PKG-INFO` & `lljz_tools-0.2.6/lljz_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lljz-tools
-Version: 0.2.5
+Version: 0.2.6
 Summary: 常用工具封装
 Home-page: 
 Author: liulangjuanzhou
 Author-email: liulangjuanzhou@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lljz_tools-0.2.5/my_tools/attribute_dict/model.py` & `lljz_tools-0.2.6/my_tools/attribute_dict/model.py`

 * *Files identical despite different names*

### Comparing `lljz_tools-0.2.5/my_tools/client/db_client.py` & `lljz_tools-0.2.6/my_tools/client/db_client.py`

 * *Files identical despite different names*

### Comparing `lljz_tools-0.2.5/my_tools/color.py` & `lljz_tools-0.2.6/my_tools/color.py`

 * *Files identical despite different names*

### Comparing `lljz_tools-0.2.5/my_tools/console_table.py` & `lljz_tools-0.2.6/my_tools/console_table.py`

 * *Files identical despite different names*

### Comparing `lljz_tools-0.2.5/my_tools/decorators.py` & `lljz_tools-0.2.6/my_tools/decorators.py`

 * *Files identical despite different names*

### Comparing `lljz_tools-0.2.5/my_tools/excel.py` & `lljz_tools-0.2.6/my_tools/excel.py`

 * *Files identical despite different names*

### Comparing `lljz_tools-0.2.5/my_tools/log_manager.py` & `lljz_tools-0.2.6/my_tools/log_manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,66 +3,80 @@
 import logging
 import os.path
 import sys
 from logging.handlers import TimedRotatingFileHandler
 
 import colorlog
 
+from my_tools.color import Color
+
 
 class LogManager:
 
     def __init__(self, log_name, level=logging.DEBUG, formatter: str = None, to_console=True, console_colors=None,
-                 log_file='/pythonlog/out.log',
+                 log_file: str =None,
+                 # log_file='/pythonlog/out.log',
                  file_formatter: str = None, file_level=None,
-                 error_log_file='/pythonlog/error.log', error_level=logging.ERROR
+                 error_log_file: str = None, error_level=logging.ERROR
                  ):
+        def _init_log_file_path(default_path):
+            if 'PYTHONPATH' in os.environ:
+                python_path = os.environ['PYTHONPATH']
+                log_path = os.path.join(python_path, 'logs')
+                if not os.path.exists(log_path):
+                    os.mkdir(path=log_path)
+                return log_path
+            print(Color.yellow(f'没有指定PYTHONPATH环境变量，使用默认路径：{default_path}'))
+            return default_path
+
         if not formatter:
             formatter = '%(asctime)s.%(msecs)03d - %(name)s - "%(pathname)s:%(lineno)d" - ' \
                         '%(levelname)s - %(funcName)s : %(message)s'
         if not file_formatter:
             file_formatter = formatter
         self._colors = console_colors or {}
         self.formatter = '%(log_color)s' + formatter
         self._file_formatter = file_formatter
         if not file_level:
             file_level = level
-        self._log_file = log_file
-        self._error_log_file = error_log_file
+        self._log_file = os.path.join(_init_log_file_path('/pythonlog'), 'out.log') if not log_file else log_file
+        self._error_log_file = os.path.join(_init_log_file_path('/pythonlog'), 'error.log') if not error_log_file else error_log_file
         self._file_level = file_level
         self._error_file_level = error_level
         logging.root.setLevel(logging.NOTSET)
         self._logger = logging.getLogger(log_name)
         self._logger.setLevel(level)
 
         self._to_console = to_console
         self._console = to_console
 
+
     @staticmethod
     def _make_dir(path):
         parent_dir = os.path.dirname(os.path.abspath(path))
         if not os.path.exists(parent_dir):
             os.makedirs(parent_dir)
 
     def get_logger(self):
         if self._logger.handlers:
             return self._logger
         if self._to_console:
-            default_colors = {
-                'DEBUG': 'blue',  # cyan white
-                'INFO': 'green',
+            colors = {
+                'DEBUG': 'white',  # cyan white green black
+                'INFO': 'blue',
                 'WARNING': 'yellow',
                 'ERROR': 'red',
-                'CRITICAL': 'bold_red',
+                'CRITICAL': 'purple',
             }
-            default_colors.update(self._colors)
+            colors.update(self._colors)
             # 输出到控制台
             console_formatter = colorlog.ColoredFormatter(
                 fmt=self.formatter,
                 datefmt='%Y-%m-%d %H:%M:%S',
-                log_colors=default_colors,
+                log_colors=colors,
             )
             console_handler = logging.StreamHandler()
             console_handler.setLevel(logging.DEBUG)
             console_handler.setFormatter(console_formatter)
             self._logger.addHandler(console_handler)
             console_handler.close()
         if self._log_file:
@@ -106,10 +120,15 @@
             self._logger.addHandler(error_file_handler)
             error_file_handler.close()
 
         return self._logger
 
 
 if __name__ == '__main__':
+
     logger2 = LogManager("my log").get_logger()
 
+    logger2.debug("Hello World")
     logger2.info("Hello World")
+    logger2.warning("Hello World")
+    logger2.error("Hello World")
+    logger2.critical("Hello World")
```

### Comparing `lljz_tools-0.2.5/my_tools/monkey.py` & `lljz_tools-0.2.6/my_tools/monkey.py`

 * *Files identical despite different names*

### Comparing `lljz_tools-0.2.5/setup.py` & `lljz_tools-0.2.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lljz_tools",
-    version="0.2.5",
+    version="0.2.6",
     author="liulangjuanzhou",
     author_email="liulangjuanzhou@gmail.com",
     description="常用工具封装",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

