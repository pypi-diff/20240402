# Comparing `tmp/selestium-0.2.5.tar.gz` & `tmp/selestium-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selestium-0.2.5.tar", last modified: Tue Apr  2 07:56:45 2024, max compression
+gzip compressed data, was "selestium-0.2.6.tar", last modified: Tue Apr  2 09:02:37 2024, max compression
```

## Comparing `selestium-0.2.5.tar` & `selestium-0.2.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 oguz      (1000) oguz      (1000)        0 2024-04-02 07:56:45.576691 selestium-0.2.5/
--rw-r--r--   0 oguz      (1000) oguz      (1000)    35149 2024-03-30 07:47:50.000000 selestium-0.2.5/LICENSE
--rw-r--r--   0 oguz      (1000) oguz      (1000)     3592 2024-04-02 07:56:45.566691 selestium-0.2.5/PKG-INFO
--rw-r--r--   0 oguz      (1000) oguz      (1000)     3269 2024-04-02 07:56:04.000000 selestium-0.2.5/README.md
-drwxr-xr-x   0 oguz      (1000) oguz      (1000)        0 2024-04-02 07:56:45.566691 selestium-0.2.5/Selestium/
--rw-r--r--   0 oguz      (1000) oguz      (1000)      757 2024-03-30 09:49:54.000000 selestium-0.2.5/Selestium/ChromeHandler.py
--rw-r--r--   0 oguz      (1000) oguz      (1000)     2107 2024-03-30 09:56:22.000000 selestium-0.2.5/Selestium/FirefoxHandler.py
--rw-r--r--   0 oguz      (1000) oguz      (1000)      199 2024-04-02 07:54:21.000000 selestium-0.2.5/Selestium/__init__.py
--rw-r--r--   0 oguz      (1000) oguz      (1000)     3725 2024-04-02 07:55:12.000000 selestium-0.2.5/Selestium/selestium.py
-drwxr-xr-x   0 oguz      (1000) oguz      (1000)        0 2024-04-02 07:56:45.566691 selestium-0.2.5/selestium.egg-info/
--rw-r--r--   0 oguz      (1000) oguz      (1000)     3592 2024-04-02 07:56:45.000000 selestium-0.2.5/selestium.egg-info/PKG-INFO
--rw-r--r--   0 oguz      (1000) oguz      (1000)      290 2024-04-02 07:56:45.000000 selestium-0.2.5/selestium.egg-info/SOURCES.txt
--rw-r--r--   0 oguz      (1000) oguz      (1000)        1 2024-04-02 07:56:45.000000 selestium-0.2.5/selestium.egg-info/dependency_links.txt
--rw-r--r--   0 oguz      (1000) oguz      (1000)       33 2024-04-02 07:56:45.000000 selestium-0.2.5/selestium.egg-info/requires.txt
--rw-r--r--   0 oguz      (1000) oguz      (1000)       10 2024-04-02 07:56:45.000000 selestium-0.2.5/selestium.egg-info/top_level.txt
--rw-r--r--   0 oguz      (1000) oguz      (1000)       38 2024-04-02 07:56:45.576691 selestium-0.2.5/setup.cfg
--rw-r--r--   0 oguz      (1000) oguz      (1000)      628 2024-04-02 07:54:43.000000 selestium-0.2.5/setup.py
+drwxr-xr-x   0 oguz      (1000) oguz      (1000)        0 2024-04-02 09:02:37.536695 selestium-0.2.6/
+-rw-r--r--   0 oguz      (1000) oguz      (1000)    35149 2024-03-30 07:47:50.000000 selestium-0.2.6/LICENSE
+-rw-r--r--   0 oguz      (1000) oguz      (1000)     3592 2024-04-02 09:02:37.536695 selestium-0.2.6/PKG-INFO
+-rw-r--r--   0 oguz      (1000) oguz      (1000)     3269 2024-04-02 07:56:04.000000 selestium-0.2.6/README.md
+drwxr-xr-x   0 oguz      (1000) oguz      (1000)        0 2024-04-02 09:02:37.526695 selestium-0.2.6/Selestium/
+-rw-r--r--   0 oguz      (1000) oguz      (1000)      757 2024-03-30 09:49:54.000000 selestium-0.2.6/Selestium/ChromeHandler.py
+-rw-r--r--   0 oguz      (1000) oguz      (1000)     2107 2024-03-30 09:56:22.000000 selestium-0.2.6/Selestium/FirefoxHandler.py
+-rw-r--r--   0 oguz      (1000) oguz      (1000)      199 2024-04-02 07:54:21.000000 selestium-0.2.6/Selestium/__init__.py
+-rw-r--r--   0 oguz      (1000) oguz      (1000)     4204 2024-04-02 08:59:32.000000 selestium-0.2.6/Selestium/selestium.py
+drwxr-xr-x   0 oguz      (1000) oguz      (1000)        0 2024-04-02 09:02:37.526695 selestium-0.2.6/selestium.egg-info/
+-rw-r--r--   0 oguz      (1000) oguz      (1000)     3592 2024-04-02 09:02:37.000000 selestium-0.2.6/selestium.egg-info/PKG-INFO
+-rw-r--r--   0 oguz      (1000) oguz      (1000)      290 2024-04-02 09:02:37.000000 selestium-0.2.6/selestium.egg-info/SOURCES.txt
+-rw-r--r--   0 oguz      (1000) oguz      (1000)        1 2024-04-02 09:02:37.000000 selestium-0.2.6/selestium.egg-info/dependency_links.txt
+-rw-r--r--   0 oguz      (1000) oguz      (1000)       33 2024-04-02 09:02:37.000000 selestium-0.2.6/selestium.egg-info/requires.txt
+-rw-r--r--   0 oguz      (1000) oguz      (1000)       10 2024-04-02 09:02:37.000000 selestium-0.2.6/selestium.egg-info/top_level.txt
+-rw-r--r--   0 oguz      (1000) oguz      (1000)       38 2024-04-02 09:02:37.536695 selestium-0.2.6/setup.cfg
+-rw-r--r--   0 oguz      (1000) oguz      (1000)      628 2024-04-02 09:01:51.000000 selestium-0.2.6/setup.py
```

### Comparing `selestium-0.2.5/LICENSE` & `selestium-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `selestium-0.2.5/PKG-INFO` & `selestium-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selestium
-Version: 0.2.5
+Version: 0.2.6
 Summary: A Python module for web scraping with Selenium and BeautifulSoup
 Home-page: https://github.com/09u2h4n/selestium
 Author: Oğuzhan Yılmaz
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `selestium-0.2.5/README.md` & `selestium-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `selestium-0.2.5/Selestium/ChromeHandler.py` & `selestium-0.2.6/Selestium/ChromeHandler.py`

 * *Files identical despite different names*

### Comparing `selestium-0.2.5/Selestium/FirefoxHandler.py` & `selestium-0.2.6/Selestium/FirefoxHandler.py`

 * *Files identical despite different names*

### Comparing `selestium-0.2.5/Selestium/selestium.py` & `selestium-0.2.6/Selestium/selestium.py`

 * *Files 11% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         if render:
             if not self.driver:
                 self.driver = self.handler.initialize_driver()
             return self.render(url)
         else:
             response = super().get(url, **kwargs)
             response.raise_for_status()
-            return HTMLResponse(response.content)
+            return HTMLResponse(response.content, original_response=response)
 
     def render(self, url):
         """
         Renders the HTML content of the specified URL using a browser.
 
         Args:
             url (str): The URL to render.
@@ -76,18 +76,20 @@
 
 class HTMLResponse:
     """
     A class representing an HTML response.
 
     Args:
         response (bytes): The response content.
+        original_response (requests.Response): The original requests Response object.
     """
 
-    def __init__(self, response):
+    def __init__(self, response, original_response=None):
         self.response = response
+        self.original_response = original_response
     
     @property
     def content(self):
         """str: The response content."""
         return self.response
 
     def html(self):
@@ -102,14 +104,21 @@
             selector (str): The CSS selector to search for.
 
         Returns:
             list: A list of BeautifulSoup Tag objects matching the selector.
         """
         return self.html().select(selector)
 
+    # Forward other method calls to the original response object
+    def __getattr__(self, name):
+        if self.original_response:
+            return getattr(self.original_response, name)
+        else:
+            raise AttributeError(f"'HTMLResponse' object has no attribute '{name}'")
+
 if __name__ == "__main__":
     # Example usage
     requests = HTMLRequests(browser='firefox')
     response = requests.get("https://www.whatismybrowser.com/detect/is-javascript-enabled", render=False)
     print(response.find("#detected_value")[0].get_text())
     #driver = navigator.browser_controller()
     #driver.get()
```

### Comparing `selestium-0.2.5/selestium.egg-info/PKG-INFO` & `selestium-0.2.6/selestium.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selestium
-Version: 0.2.5
+Version: 0.2.6
 Summary: A Python module for web scraping with Selenium and BeautifulSoup
 Home-page: https://github.com/09u2h4n/selestium
 Author: Oğuzhan Yılmaz
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `selestium-0.2.5/setup.py` & `selestium-0.2.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of the README file
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='selestium',
-    version='0.2.5',
+    version='0.2.6',
     description='A Python module for web scraping with Selenium and BeautifulSoup',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Oğuzhan Yılmaz',
     url='https://github.com/09u2h4n/selestium',
     packages=find_packages(),
     install_requires=[
```

