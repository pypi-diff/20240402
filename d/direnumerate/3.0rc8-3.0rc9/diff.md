# Comparing `tmp/direnumerate-3.0rc8.tar.gz` & `tmp/direnumerate-3.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "direnumerate-3.0rc8.tar", last modified: Tue Apr  2 13:59:29 2024, max compression
+gzip compressed data, was "direnumerate-3.0rc9.tar", last modified: Tue Apr  2 14:21:02 2024, max compression
```

## Comparing `direnumerate-3.0rc8.tar` & `direnumerate-3.0rc9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-02 13:59:29.335206 direnumerate-3.0rc8/
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    18092 2024-04-02 13:05:27.000000 direnumerate-3.0rc8/LICENSE
--rw-r--r--   0 estoque   (1000) estoque   (1000)     3862 2024-04-02 13:59:29.335206 direnumerate-3.0rc8/PKG-INFO
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     2436 2024-04-02 13:33:22.000000 direnumerate-3.0rc8/README.md
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-02 13:59:29.335206 direnumerate-3.0rc8/direnumerate/
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      553 2024-04-02 13:05:27.000000 direnumerate-3.0rc8/direnumerate/__init__.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    16094 2024-04-02 13:57:56.000000 direnumerate-3.0rc8/direnumerate/__main__.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      125 2024-04-02 13:05:27.000000 direnumerate-3.0rc8/direnumerate/banner.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     3421 2024-04-02 13:48:03.000000 direnumerate-3.0rc8/direnumerate/cli.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      394 2024-04-02 13:05:27.000000 direnumerate-3.0rc8/direnumerate/colors.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    22983 2024-04-02 13:05:27.000000 direnumerate-3.0rc8/direnumerate/createlist.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      170 2024-04-02 13:05:27.000000 direnumerate-3.0rc8/direnumerate/getinfo.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     2966 2024-04-02 13:05:27.000000 direnumerate-3.0rc8/direnumerate/ipcalculator.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       47 2024-04-02 13:05:27.000000 direnumerate-3.0rc8/direnumerate/list_urls_accounts.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       75 2024-04-02 13:58:02.000000 direnumerate-3.0rc8/direnumerate/version.py
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-02 13:59:29.335206 direnumerate-3.0rc8/direnumerate.egg-info/
--rw-r--r--   0 estoque   (1000) estoque   (1000)     3862 2024-04-02 13:59:29.000000 direnumerate-3.0rc8/direnumerate.egg-info/PKG-INFO
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      505 2024-04-02 13:59:29.000000 direnumerate-3.0rc8/direnumerate.egg-info/SOURCES.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)        1 2024-04-02 13:59:29.000000 direnumerate-3.0rc8/direnumerate.egg-info/dependency_links.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       55 2024-04-02 13:59:29.000000 direnumerate-3.0rc8/direnumerate.egg-info/entry_points.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)        9 2024-04-02 13:59:29.000000 direnumerate-3.0rc8/direnumerate.egg-info/requires.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       13 2024-04-02 13:59:29.000000 direnumerate-3.0rc8/direnumerate.egg-info/top_level.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1569 2024-04-02 13:58:39.000000 direnumerate-3.0rc8/pyproject.toml
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       38 2024-04-02 13:59:29.335206 direnumerate-3.0rc8/setup.cfg
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-02 14:21:02.076798 direnumerate-3.0rc9/
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    18092 2024-04-02 13:05:27.000000 direnumerate-3.0rc9/LICENSE
+-rw-r--r--   0 estoque   (1000) estoque   (1000)     3862 2024-04-02 14:21:02.076798 direnumerate-3.0rc9/PKG-INFO
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     2436 2024-04-02 13:33:22.000000 direnumerate-3.0rc9/README.md
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-02 14:21:02.072798 direnumerate-3.0rc9/direnumerate/
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      553 2024-04-02 13:05:27.000000 direnumerate-3.0rc9/direnumerate/__init__.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    15909 2024-04-02 14:19:49.000000 direnumerate-3.0rc9/direnumerate/__main__.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      125 2024-04-02 13:05:27.000000 direnumerate-3.0rc9/direnumerate/banner.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     3421 2024-04-02 13:48:03.000000 direnumerate-3.0rc9/direnumerate/cli.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      394 2024-04-02 13:05:27.000000 direnumerate-3.0rc9/direnumerate/colors.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    22983 2024-04-02 13:05:27.000000 direnumerate-3.0rc9/direnumerate/createlist.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      170 2024-04-02 13:05:27.000000 direnumerate-3.0rc9/direnumerate/getinfo.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     2966 2024-04-02 13:05:27.000000 direnumerate-3.0rc9/direnumerate/ipcalculator.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       47 2024-04-02 13:05:27.000000 direnumerate-3.0rc9/direnumerate/list_urls_accounts.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       75 2024-04-02 14:20:18.000000 direnumerate-3.0rc9/direnumerate/version.py
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-02 14:21:02.076798 direnumerate-3.0rc9/direnumerate.egg-info/
+-rw-r--r--   0 estoque   (1000) estoque   (1000)     3862 2024-04-02 14:21:02.000000 direnumerate-3.0rc9/direnumerate.egg-info/PKG-INFO
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      505 2024-04-02 14:21:02.000000 direnumerate-3.0rc9/direnumerate.egg-info/SOURCES.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)        1 2024-04-02 14:21:02.000000 direnumerate-3.0rc9/direnumerate.egg-info/dependency_links.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       55 2024-04-02 14:21:02.000000 direnumerate-3.0rc9/direnumerate.egg-info/entry_points.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)        9 2024-04-02 14:21:02.000000 direnumerate-3.0rc9/direnumerate.egg-info/requires.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       13 2024-04-02 14:21:02.000000 direnumerate-3.0rc9/direnumerate.egg-info/top_level.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     1569 2024-04-02 14:20:04.000000 direnumerate-3.0rc9/pyproject.toml
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       38 2024-04-02 14:21:02.076798 direnumerate-3.0rc9/setup.cfg
```

### Comparing `direnumerate-3.0rc8/LICENSE` & `direnumerate-3.0rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `direnumerate-3.0rc8/PKG-INFO` & `direnumerate-3.0rc9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: direnumerate
-Version: 3.0rc8
+Version: 3.0rc9
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
-Metadata-Version: 2.1 Name: direnumerate Version: 3.0rc8 Summary: Python 3
+Metadata-Version: 2.1 Name: direnumerate Version: 3.0rc9 Summary: Python 3
 library for directory enumeration tool in web applications. Author-email: Juan
 Bindez
 gmail.com> License: GPLv2 license Project-URL: Homepage, https://github.com/
 juanbindez/direnumerate Project-URL: Bug Reports, https://github.com/
 juanbindez/direnumerate/issues Project-URL: Read the Docs, http://
 direnumerate.readthedocs.io/ Keywords: web,enumerate,directory,tools,cli,scan
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
```

### Comparing `direnumerate-3.0rc8/README.md` & `direnumerate-3.0rc9/README.md`

 * *Files identical despite different names*

### Comparing `direnumerate-3.0rc8/direnumerate/__init__.py` & `direnumerate-3.0rc9/direnumerate/__init__.py`

 * *Files identical despite different names*

### Comparing `direnumerate-3.0rc8/direnumerate/__main__.py` & `direnumerate-3.0rc9/direnumerate/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,40 +75,41 @@
                     for line in self.wordlist_file:
                         path = line.strip()
                         full_url = self.url + "/" + path
                         response = requests.get(full_url)
                         
                         if response.status_code == 200:
                             results = f"{Color.GREEN}[Found]:{Color.RESET} {full_url}"
-                            print(results)
-                            return results
+                            
+                            
                         elif response.status_code == 204:
                             results = f"{Color.BLUE}[No Content]:{Color.RESET} {full_url}"
-                            print(results)
-                            return results
+                            
+                            
                         elif response.status_code == 400:
                             results = f"{Color.YELLOW}[Bad Request]:{Color.RESET} {full_url}"
-                            print(results)
-                            return results
+                            
+                            
                         elif response.status_code == 401:
                             results = f"{Color.RED}[Unauthorized]:{Color.RESET} {full_url}"
-                            print(results)
-                            return results
+                            
+                            
                         elif response.status_code == 403:
                             results = f"{Color.RED}[Forbidden]:{Color.RESET} {full_url}"
-                            print(results)
-                            return results
+                            
+                            
                         elif response.status_code == 404:
                             results =f"{Color.YELLOW}[Not Found]:{Color.RESET} {full_url}"
-                            print(results)
-                            return results
+                           
+                            
                         elif response.status_code == 500:
                             results = f"{Color.BLUE}[Internal Server Error]:{Color.RESET} {full_url}"
-                            print(results)
-                            return results
+                        
+                        return results
+                            
 
             except FileNotFoundError:
                 print(Color.RED + "Word list file not found." + Color.RESET)
                 
             except TypeError:
                 print(Color.GREEN + "-------------------- Scan Finished --------------------" + Color.RESET)
                 
@@ -124,15 +125,16 @@
                 with open(self.wordlist_file, "r") as self.wordlist_file:
                         for line in self.wordlist_file:
                             path = line.strip()
                             full_url = self.url + "/" + path
                             response = requests.get(full_url)
                             
                             if response.status_code == 200:
-                                return f"{Color.GREEN}[Found]:{Color.RESET} {full_url}"
+                                results = f"{Color.GREEN}[Found]:{Color.RESET} {full_url}"
+                                print(results)
             
             except FileNotFoundError:
                 print(Color.RED + "Word list file not found." + Color.RESET)
                 
             except TypeError:
                 print(Color.GREEN + "-------------------- Scan Finished --------------------" + Color.RESET)
                 
@@ -184,22 +186,20 @@
                 sock.settimeout(1)
 
                 result = sock.connect_ex((self.host, port))
 
                 if result == 0:
                     self.open_ports.append(port)
                     results = f"{Color.GREEN} [http://{self.host}] port: {port} is open", {Color.RESET}
-                    print(results)
                     
-                    return results
+                   
                 else:
                     results = f"{Color.RED} [http://{self.host}] port: {port} is closed, {Color.RESET}"
-                    print(results)
-
-                    return results
+                
+                return results
                 
         except socket.gaierror as sq:
             print(sq)
             print(Color.RED + "[Error] Don't put http:// in hosts, the software already does that" + Color.RESET)
         sock.close()
 
 class FindPattern:
```

### Comparing `direnumerate-3.0rc8/direnumerate/cli.py` & `direnumerate-3.0rc9/direnumerate/cli.py`

 * *Files identical despite different names*

### Comparing `direnumerate-3.0rc8/direnumerate/createlist.py` & `direnumerate-3.0rc9/direnumerate/createlist.py`

 * *Files identical despite different names*

### Comparing `direnumerate-3.0rc8/direnumerate/ipcalculator.py` & `direnumerate-3.0rc9/direnumerate/ipcalculator.py`

 * *Files identical despite different names*

### Comparing `direnumerate-3.0rc8/direnumerate.egg-info/PKG-INFO` & `direnumerate-3.0rc9/direnumerate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: direnumerate
-Version: 3.0rc8
+Version: 3.0rc9
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
-Metadata-Version: 2.1 Name: direnumerate Version: 3.0rc8 Summary: Python 3
+Metadata-Version: 2.1 Name: direnumerate Version: 3.0rc9 Summary: Python 3
 library for directory enumeration tool in web applications. Author-email: Juan
 Bindez
 gmail.com> License: GPLv2 license Project-URL: Homepage, https://github.com/
 juanbindez/direnumerate Project-URL: Bug Reports, https://github.com/
 juanbindez/direnumerate/issues Project-URL: Read the Docs, http://
 direnumerate.readthedocs.io/ Keywords: web,enumerate,directory,tools,cli,scan
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
```

### Comparing `direnumerate-3.0rc8/pyproject.toml` & `direnumerate-3.0rc9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "direnumerate"
-version = "3.0-rc8"
+version = "3.0-rc9"
 authors = [
   { name="Juan Bindez", email="juanbindez780@gmail.com" },
 ]
 description = "Python 3 library for directory enumeration tool in web applications."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "GPLv2 license"}
```

