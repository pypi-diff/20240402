# Comparing `tmp/loggerjava-0.0.7.1.tar.gz` & `tmp/loggerjava-0.0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggerjava-0.0.7.1.tar", last modified: Fri Jan 12 12:18:48 2024, max compression
+gzip compressed data, was "loggerjava-0.0.7.4.tar", last modified: Tue Apr  2 11:24:02 2024, max compression
```

## Comparing `loggerjava-0.0.7.1.tar` & `loggerjava-0.0.7.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 12:18:48.191967 loggerjava-0.0.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-01-12 12:18:39.000000 loggerjava-0.0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-01-12 12:18:48.187967 loggerjava-0.0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-01-12 12:18:39.000000 loggerjava-0.0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 12:18:48.187967 loggerjava-0.0.7.1/loggerjava/
--rw-r--r--   0 runner    (1001) docker     (127)    12711 2024-01-12 12:18:39.000000 loggerjava-0.0.7.1/loggerjava/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-01-12 12:18:39.000000 loggerjava-0.0.7.1/loggerjava/loggerjava.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-01-12 12:18:39.000000 loggerjava-0.0.7.1/loggerjava/test_loggerjava.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 12:18:48.187967 loggerjava-0.0.7.1/loggerjava.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-01-12 12:18:48.000000 loggerjava-0.0.7.1/loggerjava.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-01-12 12:18:48.000000 loggerjava-0.0.7.1/loggerjava.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 12:18:48.000000 loggerjava-0.0.7.1/loggerjava.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-12 12:18:48.000000 loggerjava-0.0.7.1/loggerjava.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-01-12 12:18:39.000000 loggerjava-0.0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-12 12:18:48.191967 loggerjava-0.0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-01-12 12:18:39.000000 loggerjava-0.0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:24:02.334785 loggerjava-0.0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-02 11:23:58.000000 loggerjava-0.0.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-04-02 11:24:02.334785 loggerjava-0.0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-02 11:23:58.000000 loggerjava-0.0.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:24:02.334785 loggerjava-0.0.7.4/loggerjava/
+-rw-r--r--   0 runner    (1001) docker     (127)    13411 2024-04-02 11:23:58.000000 loggerjava-0.0.7.4/loggerjava/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-04-02 11:23:58.000000 loggerjava-0.0.7.4/loggerjava/loggerjava.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-02 11:23:58.000000 loggerjava-0.0.7.4/loggerjava/test_loggerjava.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:24:02.334785 loggerjava-0.0.7.4/loggerjava.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-04-02 11:24:02.000000 loggerjava-0.0.7.4/loggerjava.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-02 11:24:02.000000 loggerjava-0.0.7.4/loggerjava.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 11:24:02.000000 loggerjava-0.0.7.4/loggerjava.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 11:24:02.000000 loggerjava-0.0.7.4/loggerjava.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-02 11:23:58.000000 loggerjava-0.0.7.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 11:24:02.334785 loggerjava-0.0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-02 11:23:58.000000 loggerjava-0.0.7.4/setup.py
```

### Comparing `loggerjava-0.0.7.1/LICENSE` & `loggerjava-0.0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `loggerjava-0.0.7.1/PKG-INFO` & `loggerjava-0.0.7.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggerjava
-Version: 0.0.7.1
+Version: 0.0.7.4
 Summary: an easy logger outputs like java logs
 Author: HTony03
 Author-email: HTony03 <HTony03@foxmail.com>
 Project-URL: Homepage, https://github.com/HTony03/loggerjava
 Project-URL: Issues, https://github.com/HTony03/loggerjava/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -61,22 +61,26 @@
 
 file_encoding : change the file encoding method
 
 showdetailedtime : whether to show detailed time in the log file
 
 showinconsole : whether to show the log in the python console
 
+fatalexit : whether to exit the program after a fatal log
+
 :return:
 """
 ```
 using `logger.exportconfig()` to export your current config
 
 and using `logger.inportconfig(inputconfig)` to inport your config
 ### Versions
 
+`v0.0.7.2` adding the "fatalexit" feature,adding an easier log function(not completed)
+
 `v0.0.7.1` adding debug config,adding debug
 
 `v0.0.7` no actual updates, updating version num to ver x.x.x
 
 `0.0.6.1` update readme
 
 `0.0.6` change the config method, adding file_encoding,absolutepath,filetype config
```

### Comparing `loggerjava-0.0.7.1/README.md` & `loggerjava-0.0.7.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -46,22 +46,26 @@
 
 file_encoding : change the file encoding method
 
 showdetailedtime : whether to show detailed time in the log file
 
 showinconsole : whether to show the log in the python console
 
+fatalexit : whether to exit the program after a fatal log
+
 :return:
 """
 ```
 using `logger.exportconfig()` to export your current config
 
 and using `logger.inportconfig(inputconfig)` to inport your config
 ### Versions
 
+`v0.0.7.2` adding the "fatalexit" feature,adding an easier log function(not completed)
+
 `v0.0.7.1` adding debug config,adding debug
 
 `v0.0.7` no actual updates, updating version num to ver x.x.x
 
 `0.0.6.1` update readme
 
 `0.0.6` change the config method, adding file_encoding,absolutepath,filetype config
```

### Comparing `loggerjava-0.0.7.1/loggerjava/__init__.py` & `loggerjava-0.0.7.4/loggerjava/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import time
 if __name__ == '__main__':
     pass
 
-ver = "v0.0.7.1"
+ver = "v0.0.7.4"
 name = "log"
 absolutepath = False
 showdetailedtime = False
 showinconsole = True
 filetype = ".log"
 file_encoding = "utf-8"
 route = r"log.log"
 debugin = False
+fatalclose = False
 
 
 # noinspection PyTypeChecker
 def debug(txt, pos="main"):
     """
         :param txt: the detail description of this log
         :param pos: show where the log's actual called positon in the code
-        :return:
+        :return: debug log
         """
     level = 'debug'
     if absolutepath:
         f = open(route, mode="at+", encoding=file_encoding)
     else:
         f = open(name + filetype, mode="at+", encoding=file_encoding)
     if showdetailedtime and showinconsole:
@@ -42,15 +43,15 @@
     f.close()
 
 
 def info(txt, pos="main"):
     """
         :param txt: the detail description of this log
         :param pos: show where the log's actual called positon in the code
-        :return:
+        :return: info log
         """
     level = 'INFO'
     if absolutepath:
         f = open(route, mode="at+", encoding=file_encoding)
     else:
         f = open(name + filetype, mode="at+", encoding=file_encoding)
     if showdetailedtime and showinconsole:
@@ -71,15 +72,15 @@
     f.close()
 
 
 def warn(txt, pos="main"):
     """
         :param txt: the detail description of this log
         :param pos: show where the log's actual called positon in the code
-        :return:
+        :return: warning log
         """
     level = 'WARN'
     if absolutepath:
         f = open(route, mode="at+", encoding=file_encoding)
     else:
         f = open(name + filetype, mode="at+", encoding=file_encoding)
     if showdetailedtime and showinconsole:
@@ -99,15 +100,15 @@
     f.close()
 
 
 def error(txt, pos="main"):
     """
         :param txt: the detail description of this log
         :param pos: show where the log's actual called positon in the code
-        :return:
+        :return: error log
         """
     level = 'ERROR'
     if absolutepath:
         f = open(route, mode="at+", encoding=file_encoding)
     else:
         f = open(name + filetype, mode="at+", encoding=file_encoding)
     if showdetailedtime and showinconsole:
@@ -127,15 +128,15 @@
     f.close()
 
 
 def fatal(txt, pos="main"):
     """
     :param txt: the detail description of this log
     :param pos: show where the log's actual called positon in the code
-    :return:
+    :return: fatal log
     """
     level = 'FATAL'
     if absolutepath:
         f = open(route, mode="at+", encoding=file_encoding)
     else:
         f = open(name + filetype, mode="at+", encoding=file_encoding)
     if showdetailedtime and showinconsole:
@@ -149,14 +150,16 @@
     else:
         f.write(_output.format(_output.time1(), pos, level, txt))
     if debugin and not showdetailedtime:
         return _output.format(_output.time1(), pos, level, txt)
     elif debugin and showdetailedtime:
         return _output.format(time.asctime(), pos, level, txt)
     f.close()
+    if fatalclose:
+        exit(10)
 
 
 def config(**kwargs):
     """
     :param kwargs:input config names and config data
     format: config_name = config_data
 
@@ -174,14 +177,16 @@
 
     file_encoding : change the file encoding method
 
     showdetailedtime : whether to show detailed time in the log file
 
     showinconsole : whether to show the log in the python console
 
+    fatalexit : whether to exit the program after a fatal log
+
     :return:
     """
     global showinconsole, showdetailedtime, absolutepath, name, filetype, file_encoding, route,debugin
     for configname, configdata in kwargs.items():
 
         if configname == "name":
             name = configdata
@@ -249,14 +254,20 @@
                 showinconsole = tmpin
                 absolutepath = False
                 f = open(name + filetype, mode="w", encoding=file_encoding)
                 f.close()
                 del tmpin
         elif configname == "debuging":
             debugin = configdata
+        elif configname == "fatalexit":
+            if configdata or not configdata:
+                fatalclose = configdata
+            else:
+                warn("wrong fatal exit config.this config is set to normal", pos="main_loggerjava")
+                fatalclose = False                
 
 
 def version():
     """
     show the current version of loggerjava
     :return:
     """
@@ -331,14 +342,21 @@
         showinconsole = True
         warn("wrong show in console config.this config is set to normal", pos="main_loggerjava")
 
 # noinspection PyMethodParameters
 
 
 class _output:
+    def typeformat(type):
+        debugformat = ["D","d","DEBUG","debug"]
+        infoformat = ["I","i","INFO","info"]
+        if type in debugformat:
+            return "DEBUG"
+        elif type in infoformat:
+            return "INFO"
 
     def format(time1, place, level, txt):
         return "[%s] [%s/%s]: %s\n" % (time1, place, level, txt)
 
     def time1():
         return str(time.localtime().tm_hour).rjust(2, "0") + ":" + \
             str(time.localtime().tm_min).rjust(2, "0") + ":" + str(time.localtime().tm_sec).rjust(2, "0")
```

### Comparing `loggerjava-0.0.7.1/loggerjava/loggerjava.py` & `loggerjava-0.0.7.4/loggerjava/loggerjava.py`

 * *Files identical despite different names*

### Comparing `loggerjava-0.0.7.1/loggerjava/test_loggerjava.py` & `loggerjava-0.0.7.4/loggerjava/test_loggerjava.py`

 * *Files identical despite different names*

### Comparing `loggerjava-0.0.7.1/loggerjava.egg-info/PKG-INFO` & `loggerjava-0.0.7.4/loggerjava.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggerjava
-Version: 0.0.7.1
+Version: 0.0.7.4
 Summary: an easy logger outputs like java logs
 Author: HTony03
 Author-email: HTony03 <HTony03@foxmail.com>
 Project-URL: Homepage, https://github.com/HTony03/loggerjava
 Project-URL: Issues, https://github.com/HTony03/loggerjava/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -61,22 +61,26 @@
 
 file_encoding : change the file encoding method
 
 showdetailedtime : whether to show detailed time in the log file
 
 showinconsole : whether to show the log in the python console
 
+fatalexit : whether to exit the program after a fatal log
+
 :return:
 """
 ```
 using `logger.exportconfig()` to export your current config
 
 and using `logger.inportconfig(inputconfig)` to inport your config
 ### Versions
 
+`v0.0.7.2` adding the "fatalexit" feature,adding an easier log function(not completed)
+
 `v0.0.7.1` adding debug config,adding debug
 
 `v0.0.7` no actual updates, updating version num to ver x.x.x
 
 `0.0.6.1` update readme
 
 `0.0.6` change the config method, adding file_encoding,absolutepath,filetype config
```

### Comparing `loggerjava-0.0.7.1/setup.py` & `loggerjava-0.0.7.4/setup.py`

 * *Files identical despite different names*

