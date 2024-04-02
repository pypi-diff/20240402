# Comparing `tmp/goodip-0.0.1b0.tar.gz` & `tmp/goodip-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goodip-0.0.1b0.tar", last modified: Tue Apr  2 14:13:02 2024, max compression
+gzip compressed data, was "goodip-0.0.2.tar", last modified: Tue Apr  2 15:05:52 2024, max compression
```

## Comparing `goodip-0.0.1b0.tar` & `goodip-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 14:13:02.366692 goodip-0.0.1b0/
--rw-rw-rw-   0        0        0     1071 2024-02-01 09:40:20.000000 goodip-0.0.1b0/LICENSE
--rw-rw-rw-   0        0        0      863 2024-04-02 14:13:02.191398 goodip-0.0.1b0/PKG-INFO
--rw-rw-rw-   0        0        0       14 2024-04-02 14:10:10.000000 goodip-0.0.1b0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 14:13:01.378532 goodip-0.0.1b0/goodip/
--rw-rw-rw-   0        0        0       18 2024-04-02 14:09:05.000000 goodip-0.0.1b0/goodip/__init__.py
--rw-rw-rw-   0        0        0      298 2024-04-02 13:33:13.000000 goodip-0.0.1b0/goodip/connection_check.py
--rw-rw-rw-   0        0        0     2053 2024-04-02 13:50:45.000000 goodip-0.0.1b0/goodip/ip.py
-drwxrwxrwx   0        0        0        0 2024-04-02 14:13:02.191398 goodip-0.0.1b0/goodip.egg-info/
--rw-rw-rw-   0        0        0      863 2024-04-02 14:13:00.000000 goodip-0.0.1b0/goodip.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2024-04-02 14:13:01.000000 goodip-0.0.1b0/goodip.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 14:13:00.000000 goodip-0.0.1b0/goodip.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-04-02 14:13:00.000000 goodip-0.0.1b0/goodip.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-02 14:13:00.000000 goodip-0.0.1b0/goodip.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 14:13:02.366692 goodip-0.0.1b0/setup.cfg
--rw-rw-rw-   0        0        0     1022 2024-04-02 14:09:59.000000 goodip-0.0.1b0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 15:05:52.223682 goodip-0.0.2/
+-rw-rw-rw-   0        0        0     1071 2024-02-01 09:40:20.000000 goodip-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      861 2024-04-02 15:05:52.219618 goodip-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2024-04-02 14:10:10.000000 goodip-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 15:05:52.046568 goodip-0.0.2/goodip/
+-rw-rw-rw-   0        0        0      330 2024-04-02 14:25:53.000000 goodip-0.0.2/goodip/__init__.py
+-rw-rw-rw-   0        0        0      298 2024-04-02 13:33:13.000000 goodip-0.0.2/goodip/connection_check.py
+-rw-rw-rw-   0        0        0     1390 2024-04-02 14:55:21.000000 goodip-0.0.2/goodip/ip.py
+drwxrwxrwx   0        0        0        0 2024-04-02 15:05:52.213973 goodip-0.0.2/goodip.egg-info/
+-rw-rw-rw-   0        0        0      861 2024-04-02 15:05:51.000000 goodip-0.0.2/goodip.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2024-04-02 15:05:51.000000 goodip-0.0.2/goodip.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 15:05:51.000000 goodip-0.0.2/goodip.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-04-02 15:05:51.000000 goodip-0.0.2/goodip.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-02 15:05:51.000000 goodip-0.0.2/goodip.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 15:05:52.228716 goodip-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1017 2024-04-02 14:55:45.000000 goodip-0.0.2/setup.py
```

### Comparing `goodip-0.0.1b0/LICENSE` & `goodip-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `goodip-0.0.1b0/PKG-INFO` & `goodip-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: goodip
-Version: 0.0.1b0
+Version: 0.0.2
 Summary: you can get your ip address and get its information.
-Home-page: https://github.com/Erfan-Bafandeh/pyrotel
+Home-page: https://github.com/Erfan-Bafandeh/goodip
 Author: Erfan Bafandeh
 Author-email: user.enbh@gmail.com
 Keywords: ip,myip,goodip,checkip
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -15,10 +15,10 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: colorama
-Requires-Dist: BeautifulSoup
+Requires-Dist: beautifulsoup4
 
 ## beta vesion
```

### Comparing `goodip-0.0.1b0/goodip/ip.py` & `goodip-0.0.2/goodip/ip.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,23 @@
 from .connection_check import connection_check
 from bs4 import BeautifulSoup
 from requests import get
 from sys import exit
-from os import system
-from colorama import Fore
 
 class ip:
-    def __init__(self, ):
+    def __init__(self):
         if connection_check() == False:
             print("please turn on your internet :|")
             exit()
-        print("Loading . .")
-
-        lib_name = "goodip"
-        version = get(f"https://pypi.org/pypi/{lib_name}/json").json()["info"]["version"]
-
-        libs = system("pip freeze").split("\n")
-
-        for i in range(len(libs)):
-            info = libs[i].split("==")
-            if info[0] == lib_name:
-                last_version = info[1]
-        if last_version != version:
-            print(f"""
-you have a new update !
-lib name: {Fore.LIGHTCYAN_EX}{lib_name}{Fore.RESET}
-version: {Fore.LIGHTCYAN_EX}{last_version}{Fore.RESET}
-new vesion: {Fore.LIGHTCYAN_EX}{version}{Fore.RESET}
-""")
         response = get("https://browserleaks.com/ip").text
         html = BeautifulSoup(response, "html.parser")
         self.ip = html.find_all("span", {"class":"flag-text wball"})[0].text
         self.region = html.find_all("tbody")[0].find_all("tr")[5].find_all("td")[1].text
         self.city = html.find_all("tbody")[0].find_all("tr")[6].find_all("td")[1].text
         self.isp = html.find_all("tbody")[0].find_all("tr")[7].find_all("td")[1].text
         self.organization = html.find_all("tbody")[0].find_all("tr")[8].find_all("td")[1].text
         self.network = html.find_all("tbody")[0].find_all("tr")[9].find_all("td")[1].text
         self.usage_type = html.find_all("tbody")[0].find_all("tr")[10].find_all("td")[1].text
         self.timezone = html.find_all("tbody")[0].find_all("tr")[11].find_all("td")[1].text
         self.local_time = html.find_all("tbody")[0].find_all("tr")[12].find_all("td")[1].text
         self.coordinates = html.find_all("tbody")[0].find_all("tr")[13].find_all("td")[1].text
-        self.os = html.find_all("tbody")[3].find_all("tr")[1].find_all("td")[1].text
+        self.os = html.find_all("tbody")[3].find_all("tr")[1].find_all("td")[1].text
```

### Comparing `goodip-0.0.1b0/goodip.egg-info/PKG-INFO` & `goodip-0.0.2/goodip.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: goodip
-Version: 0.0.1b0
+Version: 0.0.2
 Summary: you can get your ip address and get its information.
-Home-page: https://github.com/Erfan-Bafandeh/pyrotel
+Home-page: https://github.com/Erfan-Bafandeh/goodip
 Author: Erfan Bafandeh
 Author-email: user.enbh@gmail.com
 Keywords: ip,myip,goodip,checkip
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -15,10 +15,10 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: colorama
-Requires-Dist: BeautifulSoup
+Requires-Dist: beautifulsoup4
 
 ## beta vesion
```

### Comparing `goodip-0.0.1b0/setup.py` & `goodip-0.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'goodip',
-    version = '0.0.1-beta',
+    version = '0.0.2',
     author= 'Erfan Bafandeh',
     author_email = 'user.enbh@gmail.com',
     description = 'you can get your ip address and get its information.',
     keywords = ['ip', 'myip', 'goodip', 'checkip'],
     long_description = open("README.md", encoding="utf-8").read(),
     python_requires="~=3.6",
     long_description_content_type = 'text/markdown',
-    url = 'https://github.com/Erfan-Bafandeh/pyrotel',
+    url = 'https://github.com/Erfan-Bafandeh/goodip',
     packages = find_packages(),
-    install_requires = ["requests", "colorama", "BeautifulSoup"],
+    install_requires = ["requests", "colorama", "beautifulsoup4"],
     classifiers = [
     	"Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
```

