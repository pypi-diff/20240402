# Comparing `tmp/direnumerate-3.0rc6.tar.gz` & `tmp/direnumerate-3.0rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "direnumerate-3.0rc6.tar", last modified: Tue Apr  2 13:34:15 2024, max compression
+gzip compressed data, was "direnumerate-3.0rc7.tar", last modified: Tue Apr  2 13:49:25 2024, max compression
```

## Comparing `direnumerate-3.0rc6.tar` & `direnumerate-3.0rc7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-02 13:34:15.409626 direnumerate-3.0rc6/
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    18092 2024-04-02 13:05:27.000000 direnumerate-3.0rc6/LICENSE
--rw-r--r--   0 estoque   (1000) estoque   (1000)     3862 2024-04-02 13:34:15.405626 direnumerate-3.0rc6/PKG-INFO
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     2436 2024-04-02 13:33:22.000000 direnumerate-3.0rc6/README.md
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-02 13:34:15.405626 direnumerate-3.0rc6/direnumerate/
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      553 2024-04-02 13:05:27.000000 direnumerate-3.0rc6/direnumerate/__init__.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    15305 2024-04-02 13:29:35.000000 direnumerate-3.0rc6/direnumerate/__main__.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      125 2024-04-02 13:05:27.000000 direnumerate-3.0rc6/direnumerate/banner.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     3421 2024-04-02 13:30:19.000000 direnumerate-3.0rc6/direnumerate/cli.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      394 2024-04-02 13:05:27.000000 direnumerate-3.0rc6/direnumerate/colors.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    22983 2024-04-02 13:05:27.000000 direnumerate-3.0rc6/direnumerate/createlist.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      170 2024-04-02 13:05:27.000000 direnumerate-3.0rc6/direnumerate/getinfo.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     2966 2024-04-02 13:05:27.000000 direnumerate-3.0rc6/direnumerate/ipcalculator.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       47 2024-04-02 13:05:27.000000 direnumerate-3.0rc6/direnumerate/list_urls_accounts.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       75 2024-04-02 13:30:53.000000 direnumerate-3.0rc6/direnumerate/version.py
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-02 13:34:15.405626 direnumerate-3.0rc6/direnumerate.egg-info/
--rw-r--r--   0 estoque   (1000) estoque   (1000)     3862 2024-04-02 13:34:15.000000 direnumerate-3.0rc6/direnumerate.egg-info/PKG-INFO
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      505 2024-04-02 13:34:15.000000 direnumerate-3.0rc6/direnumerate.egg-info/SOURCES.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)        1 2024-04-02 13:34:15.000000 direnumerate-3.0rc6/direnumerate.egg-info/dependency_links.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       55 2024-04-02 13:34:15.000000 direnumerate-3.0rc6/direnumerate.egg-info/entry_points.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)        9 2024-04-02 13:34:15.000000 direnumerate-3.0rc6/direnumerate.egg-info/requires.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       13 2024-04-02 13:34:15.000000 direnumerate-3.0rc6/direnumerate.egg-info/top_level.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1569 2024-04-02 13:31:01.000000 direnumerate-3.0rc6/pyproject.toml
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       38 2024-04-02 13:34:15.409626 direnumerate-3.0rc6/setup.cfg
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-02 13:49:25.091520 direnumerate-3.0rc7/
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    18092 2024-04-02 13:05:27.000000 direnumerate-3.0rc7/LICENSE
+-rw-r--r--   0 estoque   (1000) estoque   (1000)     3862 2024-04-02 13:49:25.091520 direnumerate-3.0rc7/PKG-INFO
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     2436 2024-04-02 13:33:22.000000 direnumerate-3.0rc7/README.md
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-02 13:49:25.087520 direnumerate-3.0rc7/direnumerate/
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      553 2024-04-02 13:05:27.000000 direnumerate-3.0rc7/direnumerate/__init__.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    15422 2024-04-02 13:47:59.000000 direnumerate-3.0rc7/direnumerate/__main__.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      125 2024-04-02 13:05:27.000000 direnumerate-3.0rc7/direnumerate/banner.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     3421 2024-04-02 13:48:03.000000 direnumerate-3.0rc7/direnumerate/cli.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      394 2024-04-02 13:05:27.000000 direnumerate-3.0rc7/direnumerate/colors.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    22983 2024-04-02 13:05:27.000000 direnumerate-3.0rc7/direnumerate/createlist.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      170 2024-04-02 13:05:27.000000 direnumerate-3.0rc7/direnumerate/getinfo.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     2966 2024-04-02 13:05:27.000000 direnumerate-3.0rc7/direnumerate/ipcalculator.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       47 2024-04-02 13:05:27.000000 direnumerate-3.0rc7/direnumerate/list_urls_accounts.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       75 2024-04-02 13:48:12.000000 direnumerate-3.0rc7/direnumerate/version.py
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-02 13:49:25.087520 direnumerate-3.0rc7/direnumerate.egg-info/
+-rw-r--r--   0 estoque   (1000) estoque   (1000)     3862 2024-04-02 13:49:25.000000 direnumerate-3.0rc7/direnumerate.egg-info/PKG-INFO
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      505 2024-04-02 13:49:25.000000 direnumerate-3.0rc7/direnumerate.egg-info/SOURCES.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)        1 2024-04-02 13:49:25.000000 direnumerate-3.0rc7/direnumerate.egg-info/dependency_links.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       55 2024-04-02 13:49:25.000000 direnumerate-3.0rc7/direnumerate.egg-info/entry_points.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)        9 2024-04-02 13:49:25.000000 direnumerate-3.0rc7/direnumerate.egg-info/requires.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       13 2024-04-02 13:49:25.000000 direnumerate-3.0rc7/direnumerate.egg-info/top_level.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     1569 2024-04-02 13:48:19.000000 direnumerate-3.0rc7/pyproject.toml
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       38 2024-04-02 13:49:25.091520 direnumerate-3.0rc7/setup.cfg
```

### Comparing `direnumerate-3.0rc6/LICENSE` & `direnumerate-3.0rc7/LICENSE`

 * *Files identical despite different names*

### Comparing `direnumerate-3.0rc6/PKG-INFO` & `direnumerate-3.0rc7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: direnumerate
-Version: 3.0rc6
+Version: 3.0rc7
 Summary: Python 3 library for directory enumeration tool in web applications.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: GPLv2 license
 Project-URL: Homepage, https://github.com/juanbindez/direnumerate
 Project-URL: Bug Reports, https://github.com/juanbindez/direnumerate/issues
 Project-URL: Read the Docs, http://direnumerate.readthedocs.io/
 Keywords: web,enumerate,directory,tools,cli,scan
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: direnumerate Version: 3.0rc6 Summary: Python 3
+Metadata-Version: 2.1 Name: direnumerate Version: 3.0rc7 Summary: Python 3
 library for directory enumeration tool in web applications. Author-email: Juan
 Bindez
 gmail.com> License: GPLv2 license Project-URL: Homepage, https://github.com/
 juanbindez/direnumerate Project-URL: Bug Reports, https://github.com/
 juanbindez/direnumerate/issues Project-URL: Read the Docs, http://
 direnumerate.readthedocs.io/ Keywords: web,enumerate,directory,tools,cli,scan
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
```

### Comparing `direnumerate-3.0rc6/README.md` & `direnumerate-3.0rc7/README.md`

 * *Files identical despite different names*

### Comparing `direnumerate-3.0rc6/direnumerate/__init__.py` & `direnumerate-3.0rc7/direnumerate/__init__.py`

 * *Files identical despite different names*

### Comparing `direnumerate-3.0rc6/direnumerate/__main__.py` & `direnumerate-3.0rc7/direnumerate/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,22 +169,26 @@
                 sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
                 sock.settimeout(1)
 
                 result = sock.connect_ex((self.host, port))
 
                 if result == 0:
                     self.open_ports.append(port)
-                    return f"{Color.GREEN} [http://{self.host}] port: {port} is open", {Color.RESET}
+                    results = f"{Color.GREEN} [http://{self.host}] port: {port} is open", {Color.RESET}
+                    
+                    return results
                 else:
-                    print(Color.RED + f"Target -> [http://{self.host}] port: {port} is closed" + Color.RESET)
-                sock.close()
+                    results = f"{Color.RED} [http://{self.host}] port: {port} is closed, {Color.RESET}"
+                    
+                    return results
+                
         except socket.gaierror as sq:
             print(sq)
             print(Color.RED + "[Error] Don't put http:// in hosts, the software already does that" + Color.RESET)
-
+        sock.close()
 
 class FindPattern:
     """
     A class for searching for a keyword in a log file.
 
     Attributes:
         file_log (str): The path to the log file.
```

### Comparing `direnumerate-3.0rc6/direnumerate/cli.py` & `direnumerate-3.0rc7/direnumerate/cli.py`

 * *Files identical despite different names*

### Comparing `direnumerate-3.0rc6/direnumerate/createlist.py` & `direnumerate-3.0rc7/direnumerate/createlist.py`

 * *Files identical despite different names*

### Comparing `direnumerate-3.0rc6/direnumerate/ipcalculator.py` & `direnumerate-3.0rc7/direnumerate/ipcalculator.py`

 * *Files identical despite different names*

### Comparing `direnumerate-3.0rc6/direnumerate.egg-info/PKG-INFO` & `direnumerate-3.0rc7/direnumerate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: direnumerate
-Version: 3.0rc6
+Version: 3.0rc7
 Summary: Python 3 library for directory enumeration tool in web applications.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: GPLv2 license
 Project-URL: Homepage, https://github.com/juanbindez/direnumerate
 Project-URL: Bug Reports, https://github.com/juanbindez/direnumerate/issues
 Project-URL: Read the Docs, http://direnumerate.readthedocs.io/
 Keywords: web,enumerate,directory,tools,cli,scan
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: direnumerate Version: 3.0rc6 Summary: Python 3
+Metadata-Version: 2.1 Name: direnumerate Version: 3.0rc7 Summary: Python 3
 library for directory enumeration tool in web applications. Author-email: Juan
 Bindez
 gmail.com> License: GPLv2 license Project-URL: Homepage, https://github.com/
 juanbindez/direnumerate Project-URL: Bug Reports, https://github.com/
 juanbindez/direnumerate/issues Project-URL: Read the Docs, http://
 direnumerate.readthedocs.io/ Keywords: web,enumerate,directory,tools,cli,scan
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
```

### Comparing `direnumerate-3.0rc6/pyproject.toml` & `direnumerate-3.0rc7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "direnumerate"
-version = "3.0-rc6"
+version = "3.0-rc7"
 authors = [
   { name="Juan Bindez", email="juanbindez780@gmail.com" },
 ]
 description = "Python 3 library for directory enumeration tool in web applications."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "GPLv2 license"}
```

