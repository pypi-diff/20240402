# Comparing `tmp/lyylog-1.2.tar.gz` & `tmp/lyylog-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyylog-1.2.tar", last modified: Fri Dec 15 00:15:35 2023, max compression
+gzip compressed data, was "lyylog-1.3.tar", last modified: Tue Apr  2 11:03:46 2024, max compression
```

## Comparing `lyylog-1.2.tar` & `lyylog-1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-12-15 00:15:35.656717 lyylog-1.2/
--rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyylog-1.2/LICENSE
--rw-rw-rw-   0        0        0      142 2023-12-15 00:15:35.654717 lyylog-1.2/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyylog-1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-12-15 00:15:35.652717 lyylog-1.2/lyylog.egg-info/
--rw-rw-rw-   0        0        0      142 2023-12-15 00:15:35.000000 lyylog-1.2/lyylog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      156 2023-12-15 00:15:35.000000 lyylog-1.2/lyylog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-15 00:15:35.000000 lyylog-1.2/lyylog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-12-15 00:15:35.000000 lyylog-1.2/lyylog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3498 2023-12-15 00:14:09.000000 lyylog-1.2/lyylog.py
--rw-rw-rw-   0        0        0       42 2023-12-15 00:15:35.656717 lyylog-1.2/setup.cfg
--rw-rw-rw-   0        0        0      245 2023-12-15 00:15:34.000000 lyylog-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:03:46.598817 lyylog-1.3/
+-rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyylog-1.3/LICENSE
+-rw-rw-rw-   0        0        0      142 2024-04-02 11:03:46.598817 lyylog-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyylog-1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 11:03:46.596816 lyylog-1.3/lyylog.egg-info/
+-rw-rw-rw-   0        0        0      142 2024-04-02 11:03:46.000000 lyylog-1.3/lyylog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      156 2024-04-02 11:03:46.000000 lyylog-1.3/lyylog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 11:03:46.000000 lyylog-1.3/lyylog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-02 11:03:46.000000 lyylog-1.3/lyylog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3703 2024-04-02 11:03:36.000000 lyylog-1.3/lyylog.py
+-rw-rw-rw-   0        0        0       42 2024-04-02 11:03:46.599817 lyylog-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      245 2024-04-02 11:03:43.000000 lyylog-1.3/setup.py
```

### Comparing `lyylog-1.2/LICENSE` & `lyylog-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lyylog-1.2/lyylog.py` & `lyylog-1.3/lyylog.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#1.10.21
+# 1.10.21
 
 from datetime import datetime
 import sys, os
 
 import logging
 from logging.handlers import TimedRotatingFileHandler
 
@@ -16,79 +16,82 @@
 
 exe_file_name = os.path.basename(sys.argv[0])
 log_filename_prefix = f"log_{exe_file_name }.log"
 print("Star lyylog. Log filename  is ", script_dir, "/subdir_name/", log_filename_prefix)
 
 
 class CustomTimedRotatingFileHandler(TimedRotatingFileHandler):
-
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
 
 
-def log(message, subdir_namne="lyylog", prefix=log_filename_prefix, if_print=True):
-    #fastest way to logging to the module what called this function. like log_mudule_name.log.
-    #This log file is readable and writable (cannot be deleted by other similar modules at runtime), and its name will change as the log evolves.
+def log(*args, subdir_name="lyylog", prefix="log_filename_prefix", if_print=True):
+    # 将所有参数转换为字符串并用空格连接
+    message = ' '.join(str(arg) for arg in args)
+    # fastest way to logging to the module what called this function. like log_mudule_name.log.
+    # This log file is readable and writable (cannot be deleted by other similar modules at runtime), and its name will change as the log evolves.
     if not os.path.exists(subdir_namne):
         os.makedirs(subdir_namne)
     if if_print:
         print(message)
     global handler
     if handler is None:
         today = datetime.now().strftime("%Y-%m-%d")
-        handler = CustomTimedRotatingFileHandler(f'{subdir_namne}/{prefix}_{today}.log', when='midnight', interval=1, backupCount=7)
+        handler = CustomTimedRotatingFileHandler(f"{subdir_namne}/{prefix}_{today}.log", when="midnight", interval=1, backupCount=7)
         handler.suffix = "%Y-%m-%d"
-        formatter = logging.Formatter('%(asctime)s %(levelname)s: %(message)s', "%Y-%m-%d %H:%M:%S")
+        formatter = logging.Formatter("%(asctime)s : %(message)s", "%Y-%m-%d %H:%M:%S")
         handler.setFormatter(formatter)
         logger.addHandler(handler)
     with handler:
         logger.info(str(message))
 
 
-def logg(log_filename_prefix, message, if_print=True):
-    #logg can define log filename by youself
+def logg(subdir_namne, log_filename_prefix, message, if_print=True):
+    # logg can define log filename by youself
+    if not os.path.exists(subdir_namne):
+        os.makedirs(subdir_namne)
     if if_print:
         print(message)
     global handler
     if handler is None:
         today = datetime.now().strftime("%Y-%m-%d")
-        handler = CustomTimedRotatingFileHandler(f'lyylog_{log_filename_prefix}_{today}.log', when='midnight', interval=1, backupCount=7)
+        handler = CustomTimedRotatingFileHandler(f"{subdir_namne}/lyylog_{log_filename_prefix}_{today}.log", when="midnight", interval=1, backupCount=7)
         handler.suffix = "%Y-%m-%d"
-        formatter = logging.Formatter('%(asctime)s %(levelname)s: %(message)s', "%Y-%m-%d %H:%M:%S")
+        formatter = logging.Formatter("%(asctime)s %(levelname)s: %(message)s", "%Y-%m-%d %H:%M:%S")
         handler.setFormatter(formatter)
         logger.addHandler(handler)
     with handler:
         logger.info(str(message))
 
 
 def logwithdir(dirname, message, if_print=True):
-    #fastest way to logging to the module what called this function. like log_mudule_name.log.
-    #This log file is readable and writable (cannot be deleted by other similar modules at runtime), and its name will change as the log evolves.
+    # fastest way to logging to the module what called this function. like log_mudule_name.log.
+    # This log file is readable and writable (cannot be deleted by other similar modules at runtime), and its name will change as the log evolves.
     log_filename_prefix = os.path.basename(sys.argv[0])
     if if_print:
         print(message)
     global handler
     if handler is None:
         today = datetime.now().strftime("%Y-%m-%d")
-        handler = CustomTimedRotatingFileHandler(f'{dirname}/lyylog_{log_filename_prefix}_{today}.log', when='midnight', interval=1, backupCount=7)
+        handler = CustomTimedRotatingFileHandler(f"{dirname}/lyylog_{log_filename_prefix}_{today}.log", when="midnight", interval=1, backupCount=7)
         handler.suffix = "%Y-%m-%d"
-        formatter = logging.Formatter('%(asctime)s %(levelname)s: %(message)s', "%Y-%m-%d %H:%M:%S")
+        formatter = logging.Formatter("%(asctime)s %(levelname)s: %(message)s", "%Y-%m-%d %H:%M:%S")
         handler.setFormatter(formatter)
         logger.addHandler(handler)
     with handler:
         logger.info(str(message))
 
 
 def run_with_error_handling(func):
     try:
         func()
     except Exception as e:
         # 处理异常，可以打印日志或执行其他操作
         log(f"模块 {func.__name__} 出现异常: {e}")
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     # exit()
     log("testest")
```

