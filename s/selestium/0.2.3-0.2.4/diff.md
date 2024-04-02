# Comparing `tmp/selestium-0.2.3.tar.gz` & `tmp/selestium-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selestium-0.2.3.tar", last modified: Sat Mar 30 11:13:06 2024, max compression
+gzip compressed data, was "selestium-0.2.4.tar", last modified: Tue Apr  2 07:44:18 2024, max compression
```

## Comparing `selestium-0.2.3.tar` & `selestium-0.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 oguz      (1000) oguz      (1000)        0 2024-03-30 11:13:06.488343 selestium-0.2.3/
--rw-r--r--   0 oguz      (1000) oguz      (1000)    35149 2024-03-30 07:47:50.000000 selestium-0.2.3/LICENSE
--rw-r--r--   0 oguz      (1000) oguz      (1000)     3589 2024-03-30 11:13:06.488343 selestium-0.2.3/PKG-INFO
--rw-r--r--   0 oguz      (1000) oguz      (1000)     3266 2024-03-30 11:00:48.000000 selestium-0.2.3/README.md
-drwxr-xr-x   0 oguz      (1000) oguz      (1000)        0 2024-03-30 11:13:06.488343 selestium-0.2.3/Selestium/
--rw-r--r--   0 oguz      (1000) oguz      (1000)      757 2024-03-30 09:49:54.000000 selestium-0.2.3/Selestium/ChromeHandler.py
--rw-r--r--   0 oguz      (1000) oguz      (1000)     2107 2024-03-30 09:56:22.000000 selestium-0.2.3/Selestium/FirefoxHandler.py
--rw-r--r--   0 oguz      (1000) oguz      (1000)      199 2024-03-30 11:03:08.000000 selestium-0.2.3/Selestium/__init__.py
--rw-r--r--   0 oguz      (1000) oguz      (1000)     3730 2024-03-30 11:11:42.000000 selestium-0.2.3/Selestium/selestium.py
-drwxr-xr-x   0 oguz      (1000) oguz      (1000)        0 2024-03-30 11:13:06.488343 selestium-0.2.3/selestium.egg-info/
--rw-r--r--   0 oguz      (1000) oguz      (1000)     3589 2024-03-30 11:13:06.000000 selestium-0.2.3/selestium.egg-info/PKG-INFO
--rw-r--r--   0 oguz      (1000) oguz      (1000)      290 2024-03-30 11:13:06.000000 selestium-0.2.3/selestium.egg-info/SOURCES.txt
--rw-r--r--   0 oguz      (1000) oguz      (1000)        1 2024-03-30 11:13:06.000000 selestium-0.2.3/selestium.egg-info/dependency_links.txt
--rw-r--r--   0 oguz      (1000) oguz      (1000)       33 2024-03-30 11:13:06.000000 selestium-0.2.3/selestium.egg-info/requires.txt
--rw-r--r--   0 oguz      (1000) oguz      (1000)       10 2024-03-30 11:13:06.000000 selestium-0.2.3/selestium.egg-info/top_level.txt
--rw-r--r--   0 oguz      (1000) oguz      (1000)       38 2024-03-30 11:13:06.488343 selestium-0.2.3/setup.cfg
--rw-r--r--   0 oguz      (1000) oguz      (1000)      628 2024-03-30 11:11:49.000000 selestium-0.2.3/setup.py
+drwxr-xr-x   0 oguz      (1000) oguz      (1000)        0 2024-04-02 07:44:18.636693 selestium-0.2.4/
+-rw-r--r--   0 oguz      (1000) oguz      (1000)    35149 2024-03-30 07:47:50.000000 selestium-0.2.4/LICENSE
+-rw-r--r--   0 oguz      (1000) oguz      (1000)     3589 2024-04-02 07:44:18.636693 selestium-0.2.4/PKG-INFO
+-rw-r--r--   0 oguz      (1000) oguz      (1000)     3266 2024-03-30 11:00:48.000000 selestium-0.2.4/README.md
+drwxr-xr-x   0 oguz      (1000) oguz      (1000)        0 2024-04-02 07:44:18.626693 selestium-0.2.4/Selestium/
+-rw-r--r--   0 oguz      (1000) oguz      (1000)      757 2024-03-30 09:49:54.000000 selestium-0.2.4/Selestium/ChromeHandler.py
+-rw-r--r--   0 oguz      (1000) oguz      (1000)     2107 2024-03-30 09:56:22.000000 selestium-0.2.4/Selestium/FirefoxHandler.py
+-rw-r--r--   0 oguz      (1000) oguz      (1000)      196 2024-04-02 07:39:24.000000 selestium-0.2.4/Selestium/__init__.py
+-rw-r--r--   0 oguz      (1000) oguz      (1000)     3723 2024-04-02 07:39:44.000000 selestium-0.2.4/Selestium/selestium.py
+drwxr-xr-x   0 oguz      (1000) oguz      (1000)        0 2024-04-02 07:44:18.636693 selestium-0.2.4/selestium.egg-info/
+-rw-r--r--   0 oguz      (1000) oguz      (1000)     3589 2024-04-02 07:44:18.000000 selestium-0.2.4/selestium.egg-info/PKG-INFO
+-rw-r--r--   0 oguz      (1000) oguz      (1000)      290 2024-04-02 07:44:18.000000 selestium-0.2.4/selestium.egg-info/SOURCES.txt
+-rw-r--r--   0 oguz      (1000) oguz      (1000)        1 2024-04-02 07:44:18.000000 selestium-0.2.4/selestium.egg-info/dependency_links.txt
+-rw-r--r--   0 oguz      (1000) oguz      (1000)       33 2024-04-02 07:44:18.000000 selestium-0.2.4/selestium.egg-info/requires.txt
+-rw-r--r--   0 oguz      (1000) oguz      (1000)       10 2024-04-02 07:44:18.000000 selestium-0.2.4/selestium.egg-info/top_level.txt
+-rw-r--r--   0 oguz      (1000) oguz      (1000)       38 2024-04-02 07:44:18.636693 selestium-0.2.4/setup.cfg
+-rw-r--r--   0 oguz      (1000) oguz      (1000)      628 2024-04-02 07:41:43.000000 selestium-0.2.4/setup.py
```

### Comparing `selestium-0.2.3/LICENSE` & `selestium-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `selestium-0.2.3/PKG-INFO` & `selestium-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selestium
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Python module for web scraping with Selenium and BeautifulSoup
 Home-page: https://github.com/09u2h4n/selestium
 Author: Oğuzhan Yılmaz
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `selestium-0.2.3/README.md` & `selestium-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `selestium-0.2.3/Selestium/ChromeHandler.py` & `selestium-0.2.4/Selestium/ChromeHandler.py`

 * *Files identical despite different names*

### Comparing `selestium-0.2.3/Selestium/FirefoxHandler.py` & `selestium-0.2.4/Selestium/FirefoxHandler.py`

 * *Files identical despite different names*

### Comparing `selestium-0.2.3/Selestium/selestium.py` & `selestium-0.2.4/Selestium/selestium.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from requests import Session
 from bs4 import BeautifulSoup
-from .FirefoxHandler import FirefoxHandler
-from .ChromeHandler import ChromeHandler
+from FirefoxHandler import FirefoxHandler
+from ChromeHandler import ChromeHandler
 
 class HTMLRequests(Session):
     """
     A class for navigating HTML content using Selenium with Firefox or Chrome browsers.
 
     Args:
         browser (str): The type of browser to use. Can be 'firefox' or 'chrome'. Defaults to 'firefox'.
@@ -82,21 +82,21 @@
         response (bytes): The response content.
     """
 
     def __init__(self, response):
         self.response = response
     
     @property
-    def text(self):
-        """str: The response content as a string."""
+    def content(self):
+        """str: The response content."""
         return self.response
 
     def html(self):
         """BeautifulSoup: A BeautifulSoup object representing the parsed HTML."""
-        return BeautifulSoup(self.text, "html.parser")
+        return BeautifulSoup(self.content, "html.parser")
 
     def find(self, selector):
         """
         Finds all elements that match the given CSS selector.
 
         Args:
             selector (str): The CSS selector to search for.
@@ -105,11 +105,11 @@
             list: A list of BeautifulSoup Tag objects matching the selector.
         """
         return self.html().select(selector)
 
 if __name__ == "__main__":
     # Example usage
     requests = HTMLRequests(browser='firefox')
-    response = requests.get("https://www.whatismybrowser.com/detect/is-javascript-enabled", render=True)
+    response = requests.get("https://www.whatismybrowser.com/detect/is-javascript-enabled", render=False)
     print(response.find("#detected_value")[0].get_text())
     #driver = navigator.browser_controller()
     #driver.get()
```

### Comparing `selestium-0.2.3/selestium.egg-info/PKG-INFO` & `selestium-0.2.4/selestium.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selestium
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Python module for web scraping with Selenium and BeautifulSoup
 Home-page: https://github.com/09u2h4n/selestium
 Author: Oğuzhan Yılmaz
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `selestium-0.2.3/setup.py` & `selestium-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of the README file
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='selestium',
-    version='0.2.3',
+    version='0.2.4',
     description='A Python module for web scraping with Selenium and BeautifulSoup',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Oğuzhan Yılmaz',
     url='https://github.com/09u2h4n/selestium',
     packages=find_packages(),
     install_requires=[
```

