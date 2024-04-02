# Comparing `tmp/selestium-0.2.4.tar.gz` & `tmp/selestium-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selestium-0.2.4.tar", last modified: Tue Apr  2 07:44:18 2024, max compression
+gzip compressed data, was "selestium-0.2.5.tar", last modified: Tue Apr  2 07:56:45 2024, max compression
```

## Comparing `selestium-0.2.4.tar` & `selestium-0.2.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 oguz      (1000) oguz      (1000)        0 2024-04-02 07:44:18.636693 selestium-0.2.4/
--rw-r--r--   0 oguz      (1000) oguz      (1000)    35149 2024-03-30 07:47:50.000000 selestium-0.2.4/LICENSE
--rw-r--r--   0 oguz      (1000) oguz      (1000)     3589 2024-04-02 07:44:18.636693 selestium-0.2.4/PKG-INFO
--rw-r--r--   0 oguz      (1000) oguz      (1000)     3266 2024-03-30 11:00:48.000000 selestium-0.2.4/README.md
-drwxr-xr-x   0 oguz      (1000) oguz      (1000)        0 2024-04-02 07:44:18.626693 selestium-0.2.4/Selestium/
--rw-r--r--   0 oguz      (1000) oguz      (1000)      757 2024-03-30 09:49:54.000000 selestium-0.2.4/Selestium/ChromeHandler.py
--rw-r--r--   0 oguz      (1000) oguz      (1000)     2107 2024-03-30 09:56:22.000000 selestium-0.2.4/Selestium/FirefoxHandler.py
--rw-r--r--   0 oguz      (1000) oguz      (1000)      196 2024-04-02 07:39:24.000000 selestium-0.2.4/Selestium/__init__.py
--rw-r--r--   0 oguz      (1000) oguz      (1000)     3723 2024-04-02 07:39:44.000000 selestium-0.2.4/Selestium/selestium.py
-drwxr-xr-x   0 oguz      (1000) oguz      (1000)        0 2024-04-02 07:44:18.636693 selestium-0.2.4/selestium.egg-info/
--rw-r--r--   0 oguz      (1000) oguz      (1000)     3589 2024-04-02 07:44:18.000000 selestium-0.2.4/selestium.egg-info/PKG-INFO
--rw-r--r--   0 oguz      (1000) oguz      (1000)      290 2024-04-02 07:44:18.000000 selestium-0.2.4/selestium.egg-info/SOURCES.txt
--rw-r--r--   0 oguz      (1000) oguz      (1000)        1 2024-04-02 07:44:18.000000 selestium-0.2.4/selestium.egg-info/dependency_links.txt
--rw-r--r--   0 oguz      (1000) oguz      (1000)       33 2024-04-02 07:44:18.000000 selestium-0.2.4/selestium.egg-info/requires.txt
--rw-r--r--   0 oguz      (1000) oguz      (1000)       10 2024-04-02 07:44:18.000000 selestium-0.2.4/selestium.egg-info/top_level.txt
--rw-r--r--   0 oguz      (1000) oguz      (1000)       38 2024-04-02 07:44:18.636693 selestium-0.2.4/setup.cfg
--rw-r--r--   0 oguz      (1000) oguz      (1000)      628 2024-04-02 07:41:43.000000 selestium-0.2.4/setup.py
+drwxr-xr-x   0 oguz      (1000) oguz      (1000)        0 2024-04-02 07:56:45.576691 selestium-0.2.5/
+-rw-r--r--   0 oguz      (1000) oguz      (1000)    35149 2024-03-30 07:47:50.000000 selestium-0.2.5/LICENSE
+-rw-r--r--   0 oguz      (1000) oguz      (1000)     3592 2024-04-02 07:56:45.566691 selestium-0.2.5/PKG-INFO
+-rw-r--r--   0 oguz      (1000) oguz      (1000)     3269 2024-04-02 07:56:04.000000 selestium-0.2.5/README.md
+drwxr-xr-x   0 oguz      (1000) oguz      (1000)        0 2024-04-02 07:56:45.566691 selestium-0.2.5/Selestium/
+-rw-r--r--   0 oguz      (1000) oguz      (1000)      757 2024-03-30 09:49:54.000000 selestium-0.2.5/Selestium/ChromeHandler.py
+-rw-r--r--   0 oguz      (1000) oguz      (1000)     2107 2024-03-30 09:56:22.000000 selestium-0.2.5/Selestium/FirefoxHandler.py
+-rw-r--r--   0 oguz      (1000) oguz      (1000)      199 2024-04-02 07:54:21.000000 selestium-0.2.5/Selestium/__init__.py
+-rw-r--r--   0 oguz      (1000) oguz      (1000)     3725 2024-04-02 07:55:12.000000 selestium-0.2.5/Selestium/selestium.py
+drwxr-xr-x   0 oguz      (1000) oguz      (1000)        0 2024-04-02 07:56:45.566691 selestium-0.2.5/selestium.egg-info/
+-rw-r--r--   0 oguz      (1000) oguz      (1000)     3592 2024-04-02 07:56:45.000000 selestium-0.2.5/selestium.egg-info/PKG-INFO
+-rw-r--r--   0 oguz      (1000) oguz      (1000)      290 2024-04-02 07:56:45.000000 selestium-0.2.5/selestium.egg-info/SOURCES.txt
+-rw-r--r--   0 oguz      (1000) oguz      (1000)        1 2024-04-02 07:56:45.000000 selestium-0.2.5/selestium.egg-info/dependency_links.txt
+-rw-r--r--   0 oguz      (1000) oguz      (1000)       33 2024-04-02 07:56:45.000000 selestium-0.2.5/selestium.egg-info/requires.txt
+-rw-r--r--   0 oguz      (1000) oguz      (1000)       10 2024-04-02 07:56:45.000000 selestium-0.2.5/selestium.egg-info/top_level.txt
+-rw-r--r--   0 oguz      (1000) oguz      (1000)       38 2024-04-02 07:56:45.576691 selestium-0.2.5/setup.cfg
+-rw-r--r--   0 oguz      (1000) oguz      (1000)      628 2024-04-02 07:54:43.000000 selestium-0.2.5/setup.py
```

### Comparing `selestium-0.2.4/LICENSE` & `selestium-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `selestium-0.2.4/PKG-INFO` & `selestium-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selestium
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Python module for web scraping with Selenium and BeautifulSoup
 Home-page: https://github.com/09u2h4n/selestium
 Author: Oğuzhan Yılmaz
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -79,15 +79,15 @@
 # Initialize a HTMLRequests instance with default settings (Firefox browser)
 req = HTMLRequests()
 
 # Make a GET request to a web page without rendering
 response = req.get("https://www.example.com")
 
 # Extract information from the response
-print(response.text)
+print(response.content)
 ```
 
 ### Make a Request With Rendering:
 
 ```python
 from Selestium import HTMLRequests
```

### Comparing `selestium-0.2.4/README.md` & `selestium-0.2.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 # Initialize a HTMLRequests instance with default settings (Firefox browser)
 req = HTMLRequests()
 
 # Make a GET request to a web page without rendering
 response = req.get("https://www.example.com")
 
 # Extract information from the response
-print(response.text)
+print(response.content)
 ```
 
 ### Make a Request With Rendering:
 
 ```python
 from Selestium import HTMLRequests
```

### Comparing `selestium-0.2.4/Selestium/ChromeHandler.py` & `selestium-0.2.5/Selestium/ChromeHandler.py`

 * *Files identical despite different names*

### Comparing `selestium-0.2.4/Selestium/FirefoxHandler.py` & `selestium-0.2.5/Selestium/FirefoxHandler.py`

 * *Files identical despite different names*

### Comparing `selestium-0.2.4/Selestium/selestium.py` & `selestium-0.2.5/Selestium/selestium.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from requests import Session
 from bs4 import BeautifulSoup
-from FirefoxHandler import FirefoxHandler
-from ChromeHandler import ChromeHandler
+from .FirefoxHandler import FirefoxHandler
+from .ChromeHandler import ChromeHandler
 
 class HTMLRequests(Session):
     """
     A class for navigating HTML content using Selenium with Firefox or Chrome browsers.
 
     Args:
         browser (str): The type of browser to use. Can be 'firefox' or 'chrome'. Defaults to 'firefox'.
```

### Comparing `selestium-0.2.4/selestium.egg-info/PKG-INFO` & `selestium-0.2.5/selestium.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selestium
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Python module for web scraping with Selenium and BeautifulSoup
 Home-page: https://github.com/09u2h4n/selestium
 Author: Oğuzhan Yılmaz
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -79,15 +79,15 @@
 # Initialize a HTMLRequests instance with default settings (Firefox browser)
 req = HTMLRequests()
 
 # Make a GET request to a web page without rendering
 response = req.get("https://www.example.com")
 
 # Extract information from the response
-print(response.text)
+print(response.content)
 ```
 
 ### Make a Request With Rendering:
 
 ```python
 from Selestium import HTMLRequests
```

### Comparing `selestium-0.2.4/setup.py` & `selestium-0.2.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of the README file
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='selestium',
-    version='0.2.4',
+    version='0.2.5',
     description='A Python module for web scraping with Selenium and BeautifulSoup',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Oğuzhan Yılmaz',
     url='https://github.com/09u2h4n/selestium',
     packages=find_packages(),
     install_requires=[
```

