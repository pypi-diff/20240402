# Comparing `tmp/froggius-0.1.3.post2.tar.gz` & `tmp/froggius-0.1.4.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "froggius-0.1.3.post2.tar", last modified: Mon Apr  1 14:21:41 2024, max compression
+gzip compressed data, was "froggius-0.1.4.post1.tar", last modified: Mon Apr  1 15:15:42 2024, max compression
```

## Comparing `froggius-0.1.3.post2.tar` & `froggius-0.1.4.post1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:41.890987 froggius-0.1.3.post2/
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-01 14:21:33.000000 froggius-0.1.3.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-01 14:21:41.890987 froggius-0.1.3.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-01 14:21:33.000000 froggius-0.1.3.post2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:41.890987 froggius-0.1.3.post2/froggius/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:33.000000 froggius-0.1.3.post2/froggius/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-01 14:21:39.000000 froggius-0.1.3.post2/froggius/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:41.890987 froggius-0.1.3.post2/froggius.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-01 14:21:41.000000 froggius-0.1.3.post2/froggius.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-01 14:21:41.000000 froggius-0.1.3.post2/froggius.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:21:41.000000 froggius-0.1.3.post2/froggius.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 14:21:41.000000 froggius-0.1.3.post2/froggius.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 14:21:41.890987 froggius-0.1.3.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-01 14:21:39.000000 froggius-0.1.3.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:15:42.198522 froggius-0.1.4.post1/
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-01 15:15:36.000000 froggius-0.1.4.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-01 15:15:42.198522 froggius-0.1.4.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-04-01 15:15:36.000000 froggius-0.1.4.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:15:42.198522 froggius-0.1.4.post1/froggius/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 15:15:36.000000 froggius-0.1.4.post1/froggius/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-01 15:15:39.000000 froggius-0.1.4.post1/froggius/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:15:42.198522 froggius-0.1.4.post1/froggius.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-01 15:15:42.000000 froggius-0.1.4.post1/froggius.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-01 15:15:42.000000 froggius-0.1.4.post1/froggius.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:15:42.000000 froggius-0.1.4.post1/froggius.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 15:15:42.000000 froggius-0.1.4.post1/froggius.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 15:15:42.198522 froggius-0.1.4.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-01 15:15:39.000000 froggius-0.1.4.post1/setup.py
```

### Comparing `froggius-0.1.3.post2/LICENSE` & `froggius-0.1.4.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `froggius-0.1.3.post2/PKG-INFO` & `froggius-0.1.4.post1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: froggius
-Version: 0.1.3.post2
+Version: 0.1.4.post1
 Summary: Froggius is a dumb easy logging tool for python
 Home-page: https://github.com/zlElo/Froggius
 Author: zlElo
 Author-email: mail@zlelo.de
 License: MPL-2.0
 Keywords: logging,logger,easy-to-use,log
 Classifier: Intended Audience :: Developers
@@ -54,15 +54,14 @@
 from froggius.logger import Froggius
 ```
 
 ### Using debugger/logger
 Use it as debugger/logger with following possible arguments:
 - log_msg (log message)
 - file_path (None by default, used to set up a log file [...] to append to this file. The file does not have to already exist, if it does not exist, it will be created)
-- highliting (True by deafult, used to colorize [DBG] etc.)
 - print_out (True by default, used to setup printing to console and stdout)
 
 ```py
 # Example normal logging
 Froggius.debug('This is a normal debug log')
 
 # This writes the log to a log file
@@ -81,14 +80,44 @@
 # Example error
 Froggius.error('This is an error log')
 
 # This writes the error to a log file
 Froggius.error('This is an error log', 'tests/example.log', print_out=False)
 ```
 
+### Using information logger
+Use it as information logger with following possible arguments:
+- log_msg (log message)
+- file_path (None by default, used to set up a log file [...] to append to this file. The file does not have to already exist, if it does not exist, it will be created)
+- highliting (True by default, used to colorize [INF] etc.)
+- print_out (True by default, used to setup printing to console and stdout)
+
+```py
+# Example information
+Froggius.information('This is an information log')
+
+# This writes the information to a log file
+Froggius.information('This is an information log', 'tests/example.log', print_out=False)
+```
+
+### Using warning logger
+Use it as warning logger with following possible arguments:
+- log_msg (log message)
+- file_path (None by default, used to set up a log file [...] to append to this file. The file does not have to already exist, if it does not exist, it will be created)
+- highliting (True by default, used to colorize [WRN] etc.)
+- print_out (True by default, used to setup printing to console and stdout)
+
+```py
+# Example warning
+Froggius.warning('This is a warning log')
+
+# This writes the warning to a log file
+Froggius.warning('This is a warning log', 'tests/example.log', print_out=False)
+```
+
 ### Using catching errors
 Use the catching errors methode, to catch and handle unexpected errors, warnings etc:
 
 ```py
 @Froggius.catch(file_path='tests/example.log')
 def example_function():
     """
```

### Comparing `froggius-0.1.3.post2/README.md` & `froggius-0.1.4.post1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 from froggius.logger import Froggius
 ```
 
 ### Using debugger/logger
 Use it as debugger/logger with following possible arguments:
 - log_msg (log message)
 - file_path (None by default, used to set up a log file [...] to append to this file. The file does not have to already exist, if it does not exist, it will be created)
-- highliting (True by deafult, used to colorize [DBG] etc.)
 - print_out (True by default, used to setup printing to console and stdout)
 
 ```py
 # Example normal logging
 Froggius.debug('This is a normal debug log')
 
 # This writes the log to a log file
@@ -64,14 +63,44 @@
 # Example error
 Froggius.error('This is an error log')
 
 # This writes the error to a log file
 Froggius.error('This is an error log', 'tests/example.log', print_out=False)
 ```
 
+### Using information logger
+Use it as information logger with following possible arguments:
+- log_msg (log message)
+- file_path (None by default, used to set up a log file [...] to append to this file. The file does not have to already exist, if it does not exist, it will be created)
+- highliting (True by default, used to colorize [INF] etc.)
+- print_out (True by default, used to setup printing to console and stdout)
+
+```py
+# Example information
+Froggius.information('This is an information log')
+
+# This writes the information to a log file
+Froggius.information('This is an information log', 'tests/example.log', print_out=False)
+```
+
+### Using warning logger
+Use it as warning logger with following possible arguments:
+- log_msg (log message)
+- file_path (None by default, used to set up a log file [...] to append to this file. The file does not have to already exist, if it does not exist, it will be created)
+- highliting (True by default, used to colorize [WRN] etc.)
+- print_out (True by default, used to setup printing to console and stdout)
+
+```py
+# Example warning
+Froggius.warning('This is a warning log')
+
+# This writes the warning to a log file
+Froggius.warning('This is a warning log', 'tests/example.log', print_out=False)
+```
+
 ### Using catching errors
 Use the catching errors methode, to catch and handle unexpected errors, warnings etc:
 
 ```py
 @Froggius.catch(file_path='tests/example.log')
 def example_function():
     """
```

### Comparing `froggius-0.1.3.post2/froggius/logger.py` & `froggius-0.1.4.post1/froggius/logger.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,53 +9,41 @@
 
 class Froggius:
     """
     Main class of Froggius
     Includes logging methods
     """
 
-    def debug(log_msg, file_path=None, highliting=True, print_out=True):
+    def debug(log_msg, file_path=None, print_out=True):
         """
         Writes logs, optionally to a file.
 
         Parameters
         ----------
         log_msg : str
             The message to be logged.
         file_path : str, optional
             The path to the file where the log should be saved, by default None
         highliting : bool, optional
             Whether the DEBUG tag should be highlighted with ANSI escape sequences, by default True
         print_out : bool, optional
             Whether the log should be printed to the stdout, by default True
-
-        Returns
-        -------
-        str
-            The log string if print_out is set to False
         """
         current_date = datetime.datetime.now()
-        if highliting:
-            log_string = f'\033[92m[DBG]\033[0m [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg}'
-        else:
-            log_string = (
-                f'[DBG] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg}'
-            )
+        log_string = f'[DBG] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg}'
 
         # check for filepath
         if file_path is not None:
             with open(file_path, "a") as log:
                 log.write(
                     f'\n[DBG] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg}'
                 )
 
         if print_out:
             print(log_string, file=sys.stdout)
-        else:
-            return log_string
 
     def error(log_msg, file_path=None, highlighting=True, print_out=True, line=None):
         """
         Writes errors, optionally to a file.
 
         Parameters
         ----------
@@ -68,19 +56,14 @@
             by default True
         print_out : bool, optional
             Whether the log should be printed to the stdout, by default True
         line : List[str], optional
             A list containing information about the line where the error occurred,
             by default None. The list should contain [line number, file name,
             function name].
-
-        Returns
-        -------
-        str or None
-            The log string if print_out is set to False
         """
 
         # get datetime
         current_date = datetime.datetime.now()
         if highlighting == True:
             log_string = f'[\033[91mERR\033[0m] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg} {f"| Occured on line: {line[0]} in {line[1]}, {line[2]}()" if line is not None else ""}'
         else:
@@ -90,26 +73,25 @@
         if file_path is not None:
             with open(file_path, "a") as log:
                 log.write(
                     f'\n[ERR] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg} {f"| Occured on line: {line[0]} in {line[1]}, {line[2]}()" if line is not None else ""}'
                 )
 
         if print_out == True:
-            print(log_string, file=sys.stdout)
-        else:
-            return log_string
+            print(log_string, file=sys.stderr)
 
     @staticmethod
-    def catch(file_path=None):
+    def catch(file_path=None, continue_onexpception=True):
         """
         A decorator that catches exceptions and logs them with LogMx.error
 
         Parameters
         ----------
         file_path : str, optional
+        contiune_onexpception : bool, optional
 
         Returns
         -------
         decorator
         """
 
         def decorator(func):
@@ -127,10 +109,63 @@
                         log_msg=str(e),
                         highlighting=True,
                         print_out=True,
                         line=[line, file, function_name],
                         file_path=file_path,
                     )
 
+                    if not continue_onexpception:
+                        raise e
+
             return wrapper
 
         return decorator
+
+    def information(log_msg, file_path=None, highlighting=True, print_out=True):
+        """
+        A function to log information with optional file output and highlighting.
+
+        Parameters:
+            log_msg (str): The message to be logged.
+            file_path (str, optional): The file path to log to. Defaults to None.
+            highlighting (bool, optional): Whether to highlight the log message. Defaults to True.
+            print_out (bool, optional): Whether to print the log message. Defaults to True.
+        """
+
+        current_date = datetime.datetime.now()
+
+        if highlighting:
+            log_string = f'[\033[32mINF\033[0m] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg}'
+        else:
+            log_string = (
+                f'[INF] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg}'
+            )
+
+        # check for filepath
+        if file_path is not None:
+            with open(file_path, "a") as log:
+                log.write(
+                    f'\n[INF] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg}'
+                )
+
+        if print_out == True:
+            print(log_string, file=sys.stdout)
+
+    def warning(log_msg, file_path=None, highlighting=True, print_out=True):
+        current_date = datetime.datetime.now()
+
+        if highlighting:
+            log_string = f'[\033[93mWRN\033[0m] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg}'
+        else:
+            log_string = (
+                f'[WRN] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg}'
+            )
+
+        # check for filepath
+        if file_path is not None:
+            with open(file_path, "a") as log:
+                log.write(
+                    f'\n[WRN] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg}'
+                )
+
+        if print_out == True:
+            print(log_string, file=sys.stdout)
```

### Comparing `froggius-0.1.3.post2/froggius.egg-info/PKG-INFO` & `froggius-0.1.4.post1/froggius.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: froggius
-Version: 0.1.3.post2
+Version: 0.1.4.post1
 Summary: Froggius is a dumb easy logging tool for python
 Home-page: https://github.com/zlElo/Froggius
 Author: zlElo
 Author-email: mail@zlelo.de
 License: MPL-2.0
 Keywords: logging,logger,easy-to-use,log
 Classifier: Intended Audience :: Developers
@@ -54,15 +54,14 @@
 from froggius.logger import Froggius
 ```
 
 ### Using debugger/logger
 Use it as debugger/logger with following possible arguments:
 - log_msg (log message)
 - file_path (None by default, used to set up a log file [...] to append to this file. The file does not have to already exist, if it does not exist, it will be created)
-- highliting (True by deafult, used to colorize [DBG] etc.)
 - print_out (True by default, used to setup printing to console and stdout)
 
 ```py
 # Example normal logging
 Froggius.debug('This is a normal debug log')
 
 # This writes the log to a log file
@@ -81,14 +80,44 @@
 # Example error
 Froggius.error('This is an error log')
 
 # This writes the error to a log file
 Froggius.error('This is an error log', 'tests/example.log', print_out=False)
 ```
 
+### Using information logger
+Use it as information logger with following possible arguments:
+- log_msg (log message)
+- file_path (None by default, used to set up a log file [...] to append to this file. The file does not have to already exist, if it does not exist, it will be created)
+- highliting (True by default, used to colorize [INF] etc.)
+- print_out (True by default, used to setup printing to console and stdout)
+
+```py
+# Example information
+Froggius.information('This is an information log')
+
+# This writes the information to a log file
+Froggius.information('This is an information log', 'tests/example.log', print_out=False)
+```
+
+### Using warning logger
+Use it as warning logger with following possible arguments:
+- log_msg (log message)
+- file_path (None by default, used to set up a log file [...] to append to this file. The file does not have to already exist, if it does not exist, it will be created)
+- highliting (True by default, used to colorize [WRN] etc.)
+- print_out (True by default, used to setup printing to console and stdout)
+
+```py
+# Example warning
+Froggius.warning('This is a warning log')
+
+# This writes the warning to a log file
+Froggius.warning('This is a warning log', 'tests/example.log', print_out=False)
+```
+
 ### Using catching errors
 Use the catching errors methode, to catch and handle unexpected errors, warnings etc:
 
 ```py
 @Froggius.catch(file_path='tests/example.log')
 def example_function():
     """
```

### Comparing `froggius-0.1.3.post2/setup.py` & `froggius-0.1.4.post1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 setup(
     name="froggius",
     packages=find_packages(include=["froggius"]),
     description="Froggius is a dumb easy logging tool for python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MPL-2.0",
-    version="0.1.3-2",
+    version="0.1.4-1",
     author="zlElo",
     author_email="mail@zlelo.de",
     url="https://github.com/zlElo/Froggius",
     keywords=["logging", "logger", "easy-to-use", "log"],
     classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
```

