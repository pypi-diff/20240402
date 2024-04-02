# Comparing `tmp/direnumerate-3.0rc5.tar.gz` & `tmp/direnumerate-3.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "direnumerate-3.0rc5.tar", last modified: Mon Apr  1 19:44:54 2024, max compression
+gzip compressed data, was "direnumerate-3.0rc6.tar", last modified: Tue Apr  2 13:34:15 2024, max compression
```

## Comparing `direnumerate-3.0rc5.tar` & `direnumerate-3.0rc6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-01 19:44:54.951133 direnumerate-3.0rc5/
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    18092 2024-04-01 19:42:13.000000 direnumerate-3.0rc5/LICENSE
--rw-r--r--   0 estoque   (1000) estoque   (1000)     3869 2024-04-01 19:44:54.951133 direnumerate-3.0rc5/PKG-INFO
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     2443 2024-04-01 19:42:13.000000 direnumerate-3.0rc5/README.md
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-01 19:44:54.947133 direnumerate-3.0rc5/direnumerate/
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      553 2024-04-01 19:42:13.000000 direnumerate-3.0rc5/direnumerate/__init__.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    16028 2024-04-01 19:42:13.000000 direnumerate-3.0rc5/direnumerate/__main__.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      125 2024-04-01 19:42:13.000000 direnumerate-3.0rc5/direnumerate/banner.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     3435 2024-04-01 19:43:33.000000 direnumerate-3.0rc5/direnumerate/cli.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      394 2024-04-01 19:42:13.000000 direnumerate-3.0rc5/direnumerate/colors.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    22983 2024-04-01 19:42:13.000000 direnumerate-3.0rc5/direnumerate/createlist.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      170 2024-04-01 19:42:13.000000 direnumerate-3.0rc5/direnumerate/getinfo.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     2966 2024-04-01 19:42:13.000000 direnumerate-3.0rc5/direnumerate/ipcalculator.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       47 2024-04-01 19:42:13.000000 direnumerate-3.0rc5/direnumerate/list_urls_accounts.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       75 2024-04-01 19:43:44.000000 direnumerate-3.0rc5/direnumerate/version.py
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-01 19:44:54.951133 direnumerate-3.0rc5/direnumerate.egg-info/
--rw-r--r--   0 estoque   (1000) estoque   (1000)     3869 2024-04-01 19:44:54.000000 direnumerate-3.0rc5/direnumerate.egg-info/PKG-INFO
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      505 2024-04-01 19:44:54.000000 direnumerate-3.0rc5/direnumerate.egg-info/SOURCES.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)        1 2024-04-01 19:44:54.000000 direnumerate-3.0rc5/direnumerate.egg-info/dependency_links.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       55 2024-04-01 19:44:54.000000 direnumerate-3.0rc5/direnumerate.egg-info/entry_points.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)        9 2024-04-01 19:44:54.000000 direnumerate-3.0rc5/direnumerate.egg-info/requires.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       13 2024-04-01 19:44:54.000000 direnumerate-3.0rc5/direnumerate.egg-info/top_level.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1569 2024-04-01 19:43:53.000000 direnumerate-3.0rc5/pyproject.toml
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       38 2024-04-01 19:44:54.951133 direnumerate-3.0rc5/setup.cfg
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-02 13:34:15.409626 direnumerate-3.0rc6/
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    18092 2024-04-02 13:05:27.000000 direnumerate-3.0rc6/LICENSE
+-rw-r--r--   0 estoque   (1000) estoque   (1000)     3862 2024-04-02 13:34:15.405626 direnumerate-3.0rc6/PKG-INFO
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     2436 2024-04-02 13:33:22.000000 direnumerate-3.0rc6/README.md
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-02 13:34:15.405626 direnumerate-3.0rc6/direnumerate/
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      553 2024-04-02 13:05:27.000000 direnumerate-3.0rc6/direnumerate/__init__.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    15305 2024-04-02 13:29:35.000000 direnumerate-3.0rc6/direnumerate/__main__.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      125 2024-04-02 13:05:27.000000 direnumerate-3.0rc6/direnumerate/banner.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     3421 2024-04-02 13:30:19.000000 direnumerate-3.0rc6/direnumerate/cli.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      394 2024-04-02 13:05:27.000000 direnumerate-3.0rc6/direnumerate/colors.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    22983 2024-04-02 13:05:27.000000 direnumerate-3.0rc6/direnumerate/createlist.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      170 2024-04-02 13:05:27.000000 direnumerate-3.0rc6/direnumerate/getinfo.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     2966 2024-04-02 13:05:27.000000 direnumerate-3.0rc6/direnumerate/ipcalculator.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       47 2024-04-02 13:05:27.000000 direnumerate-3.0rc6/direnumerate/list_urls_accounts.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       75 2024-04-02 13:30:53.000000 direnumerate-3.0rc6/direnumerate/version.py
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-02 13:34:15.405626 direnumerate-3.0rc6/direnumerate.egg-info/
+-rw-r--r--   0 estoque   (1000) estoque   (1000)     3862 2024-04-02 13:34:15.000000 direnumerate-3.0rc6/direnumerate.egg-info/PKG-INFO
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      505 2024-04-02 13:34:15.000000 direnumerate-3.0rc6/direnumerate.egg-info/SOURCES.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)        1 2024-04-02 13:34:15.000000 direnumerate-3.0rc6/direnumerate.egg-info/dependency_links.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       55 2024-04-02 13:34:15.000000 direnumerate-3.0rc6/direnumerate.egg-info/entry_points.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)        9 2024-04-02 13:34:15.000000 direnumerate-3.0rc6/direnumerate.egg-info/requires.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       13 2024-04-02 13:34:15.000000 direnumerate-3.0rc6/direnumerate.egg-info/top_level.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     1569 2024-04-02 13:31:01.000000 direnumerate-3.0rc6/pyproject.toml
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       38 2024-04-02 13:34:15.409626 direnumerate-3.0rc6/setup.cfg
```

### Comparing `direnumerate-3.0rc5/LICENSE` & `direnumerate-3.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `direnumerate-3.0rc5/PKG-INFO` & `direnumerate-3.0rc6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: direnumerate
-Version: 3.0rc5
+Version: 3.0rc6
 Summary: Python 3 library for directory enumeration tool in web applications.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: GPLv2 license
 Project-URL: Homepage, https://github.com/juanbindez/direnumerate
 Project-URL: Bug Reports, https://github.com/juanbindez/direnumerate/issues
 Project-URL: Read the Docs, http://direnumerate.readthedocs.io/
 Keywords: web,enumerate,directory,tools,cli,scan
@@ -67,27 +67,27 @@
     pip install direnumerate --break-system-packages
 ----------
 
 ## Command line usage:
 
 ### Directory Scan:
 
-    direnumerate Ds -t testphp.vulnweb.com -w wordlist.txt
+    direnumerate -t testphp.vulnweb.com -w wordlist.txt
 
 ### Post Scan:
 
-    direnumerate Ps -t 44.228.249.3 -p 22 80 443
+    direnumerate -t 44.228.249.3 -p 22 80 443
 
 ### Finds patterns in logs:
 
-    direnumerate Fp -log test.log -key ERROR
+    direnumerate -log test.log -key ERROR
 
 ### IP Info:
 
-    direnumerate info -t 8.8.8.8
+    direnumerate --info -t 8.8.8.8
 
 
 ## Scripts usage:
 
 ### Directory Scan in Websites:
 
 ```python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: direnumerate Version: 3.0rc5 Summary: Python 3
+Metadata-Version: 2.1 Name: direnumerate Version: 3.0rc6 Summary: Python 3
 library for directory enumeration tool in web applications. Author-email: Juan
 Bindez
 gmail.com> License: GPLv2 license Project-URL: Homepage, https://github.com/
 juanbindez/direnumerate Project-URL: Bug Reports, https://github.com/
 juanbindez/direnumerate/issues Project-URL: Read the Docs, http://
 direnumerate.readthedocs.io/ Keywords: web,enumerate,directory,tools,cli,scan
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
@@ -30,22 +30,22 @@
 directory and file enumeration on web servers. It is useful for security
 professionals and system administrators who want to identify hidden resources
 and assess the security of web applications. ## Key Features - Enumeration of
 directories and files on web servers. - Creates a wordlist automatically -
 Wordlist customization. - Detailed output of findings. - Support for multiple
 URL schemes (http, https, etc.). ## install: pip install direnumerate ---------
 -------- ## install in ubuntu: pip install direnumerate --break-system-packages
----------- ## Command line usage: ### Directory Scan: direnumerate Ds -
-t testphp.vulnweb.com -w wordlist.txt ### Post Scan: direnumerate Ps -
-t 44.228.249.3 -p 22 80 443 ### Finds patterns in logs: direnumerate Fp -log
-test.log -key ERROR ### IP Info: direnumerate info -t 8.8.8.8 ## Scripts usage:
-### Directory Scan in Websites: ```python from direnumerate import DirScan url
-= "testphp.vulnweb.com" wordlist = "wordlist.txt" enum = DirScan(url)
-enum.dir_enum(wordlist) ``` ---------- ### User Accont Scan: ```python from
-direnumerate import UserScan user = "username" found = UserScan(user)
+---------- ## Command line usage: ### Directory Scan: direnumerate -
+t testphp.vulnweb.com -w wordlist.txt ### Post Scan: direnumerate -
+t 44.228.249.3 -p 22 80 443 ### Finds patterns in logs: direnumerate -log
+test.log -key ERROR ### IP Info: direnumerate --info -t 8.8.8.8 ## Scripts
+usage: ### Directory Scan in Websites: ```python from direnumerate import
+DirScan url = "testphp.vulnweb.com" wordlist = "wordlist.txt" enum = DirScan
+(url) enum.dir_enum(wordlist) ``` ---------- ### User Accont Scan: ```python
+from direnumerate import UserScan user = "username" found = UserScan(user)
 found.found_users() ``` ---------- ### Port Scan: ```python from direnumerate
 import PortScan ip = "44.228.249.3" list_ports = [22, 80, 443] scan = PortScan
 (ip) scan.scan_ports(list_ports) ``` ---------- ### Finds patterns in logs:
 ```python from direnumerate import FindPatterns log = "test.log" key = "ERROR"
 fp = FindPatterns(log) fp.find_in_log(keyword=key) ``` ### IP Info: ```python
 from direnumerate import InfoIp ip = "8.8.8.8" ipinfo = InfoIp(ip)
 ipinfo.show_info() ``` ----------
```

### Comparing `direnumerate-3.0rc5/README.md` & `direnumerate-3.0rc6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -34,27 +34,27 @@
     pip install direnumerate --break-system-packages
 ----------
 
 ## Command line usage:
 
 ### Directory Scan:
 
-    direnumerate Ds -t testphp.vulnweb.com -w wordlist.txt
+    direnumerate -t testphp.vulnweb.com -w wordlist.txt
 
 ### Post Scan:
 
-    direnumerate Ps -t 44.228.249.3 -p 22 80 443
+    direnumerate -t 44.228.249.3 -p 22 80 443
 
 ### Finds patterns in logs:
 
-    direnumerate Fp -log test.log -key ERROR
+    direnumerate -log test.log -key ERROR
 
 ### IP Info:
 
-    direnumerate info -t 8.8.8.8
+    direnumerate --info -t 8.8.8.8
 
 
 ## Scripts usage:
 
 ### Directory Scan in Websites:
 
 ```python
```

#### html2text {}

```diff
@@ -10,22 +10,22 @@
 directory and file enumeration on web servers. It is useful for security
 professionals and system administrators who want to identify hidden resources
 and assess the security of web applications. ## Key Features - Enumeration of
 directories and files on web servers. - Creates a wordlist automatically -
 Wordlist customization. - Detailed output of findings. - Support for multiple
 URL schemes (http, https, etc.). ## install: pip install direnumerate ---------
 -------- ## install in ubuntu: pip install direnumerate --break-system-packages
----------- ## Command line usage: ### Directory Scan: direnumerate Ds -
-t testphp.vulnweb.com -w wordlist.txt ### Post Scan: direnumerate Ps -
-t 44.228.249.3 -p 22 80 443 ### Finds patterns in logs: direnumerate Fp -log
-test.log -key ERROR ### IP Info: direnumerate info -t 8.8.8.8 ## Scripts usage:
-### Directory Scan in Websites: ```python from direnumerate import DirScan url
-= "testphp.vulnweb.com" wordlist = "wordlist.txt" enum = DirScan(url)
-enum.dir_enum(wordlist) ``` ---------- ### User Accont Scan: ```python from
-direnumerate import UserScan user = "username" found = UserScan(user)
+---------- ## Command line usage: ### Directory Scan: direnumerate -
+t testphp.vulnweb.com -w wordlist.txt ### Post Scan: direnumerate -
+t 44.228.249.3 -p 22 80 443 ### Finds patterns in logs: direnumerate -log
+test.log -key ERROR ### IP Info: direnumerate --info -t 8.8.8.8 ## Scripts
+usage: ### Directory Scan in Websites: ```python from direnumerate import
+DirScan url = "testphp.vulnweb.com" wordlist = "wordlist.txt" enum = DirScan
+(url) enum.dir_enum(wordlist) ``` ---------- ### User Accont Scan: ```python
+from direnumerate import UserScan user = "username" found = UserScan(user)
 found.found_users() ``` ---------- ### Port Scan: ```python from direnumerate
 import PortScan ip = "44.228.249.3" list_ports = [22, 80, 443] scan = PortScan
 (ip) scan.scan_ports(list_ports) ``` ---------- ### Finds patterns in logs:
 ```python from direnumerate import FindPatterns log = "test.log" key = "ERROR"
 fp = FindPatterns(log) fp.find_in_log(keyword=key) ``` ### IP Info: ```python
 from direnumerate import InfoIp ip = "8.8.8.8" ipinfo = InfoIp(ip)
 ipinfo.show_info() ``` ----------
```

### Comparing `direnumerate-3.0rc5/direnumerate/__init__.py` & `direnumerate-3.0rc6/direnumerate/__init__.py`

 * *Files identical despite different names*

### Comparing `direnumerate-3.0rc5/direnumerate/__main__.py` & `direnumerate-3.0rc6/direnumerate/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -74,27 +74,28 @@
                 with open(self.wordlist_file, "r") as self.wordlist_file:
                     for line in self.wordlist_file:
                         path = line.strip()
                         full_url = self.url + "/" + path
                         response = requests.get(full_url)
                         
                         if response.status_code == 200:
-                            print(Color.GREEN + f"Target access [Found]: -> {Color.RESET + full_url}")
+                            return f"{Color.GREEN}[Found]:{Color.RESET} {full_url}"
                         elif response.status_code == 204:
-                            print(Color.BLUE + f"Target access [No Content]: -> {Color.RESET+ full_url}")
+                            return f"{Color.BLUE}[No Content]:{Color.RESET} {full_url}"
                         elif response.status_code == 400:
-                            print(Color.YELLOW + f"Target access [Bad Request]: -> {Color.RESET+ full_url}")
+                            return f"{Color.YELLOW}[Bad Request]:{Color.RESET} {full_url}"
                         elif response.status_code == 401:
-                            print(Color.RED + f"Target access [Unauthorized]: -> {Color.RESET+ full_url}")
+                            return f"{Color.RED}[Unauthorized]:{Color.RESET} {full_url}"
                         elif response.status_code == 403:
-                            print(Color.RED + f"Target access [Forbidden]: -> {Color.RESET+ full_url}")
+                            return f"{Color.RED}[Forbidden]:{Color.RESET} {full_url}"
                         elif response.status_code == 404:
-                            print(Color.YELLOW + f"Target access [Not Found]: -> {Color.RESET+ full_url}")
+                            return f"{Color.YELLOW}[Not Found]:{Color.RESET} {full_url}"
                         elif response.status_code == 500:
-                            print(Color.BLUE + f"Target access [Internal Server Error]: -> {Color.RESET+ full_url}")
+                            return f"{Color.BLUE}[Internal Server Error]:{Color.RESET} {full_url}"
+
             except FileNotFoundError:
                 print(Color.RED + "Word list file not found." + Color.RESET)
                 
             except TypeError:
                 print(Color.GREEN + "-------------------- Scan Finished --------------------" + Color.RESET)
                 
             except KeyboardInterrupt:
@@ -109,15 +110,15 @@
                 with open(self.wordlist_file, "r") as self.wordlist_file:
                         for line in self.wordlist_file:
                             path = line.strip()
                             full_url = self.url + "/" + path
                             response = requests.get(full_url)
                             
                             if response.status_code == 200:
-                                print(Color.GREEN + f"Target access [Found]: -> {Color.RESET + full_url}")
+                                return f"{Color.GREEN}[Found]:{Color.RESET} {full_url}"
             
             except FileNotFoundError:
                 print(Color.RED + "Word list file not found." + Color.RESET)
                 
             except TypeError:
                 print(Color.GREEN + "-------------------- Scan Finished --------------------" + Color.RESET)
                 
@@ -168,15 +169,15 @@
                 sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
                 sock.settimeout(1)
 
                 result = sock.connect_ex((self.host, port))
 
                 if result == 0:
                     self.open_ports.append(port)
-                    print(Color.GREEN + f"Target -> [http://{self.host}] port: {port} is open" + Color.RESET)
+                    return f"{Color.GREEN} [http://{self.host}] port: {port} is open", {Color.RESET}
                 else:
                     print(Color.RED + f"Target -> [http://{self.host}] port: {port} is closed" + Color.RESET)
                 sock.close()
         except socket.gaierror as sq:
             print(sq)
             print(Color.RED + "[Error] Don't put http:// in hosts, the software already does that" + Color.RESET)
 
@@ -339,38 +340,42 @@
             None
 
         Note:
             This method relies on external functions (not provided in this code snippet) for its functionality.
         """
         
         informations = get_info_ip(self.ip)
-        print(Color.GREEN + "Information about the IP address:" + Color.RESET, self.ip)
-        print(Color.GREEN + "IP:" + Color.RESET, informations["ip"])
-        print(Color.GREEN + "Hostname:" + Color.RESET, informations["hostname"])
-        print(Color.GREEN + "Location:" + Color.RESET, informations["loc"])
-        print(Color.GREEN + "City:" + Color.RESET, informations["city"])
-        print(Color.GREEN + "Region:" + Color.RESET, informations["region"])
-        print(Color.GREEN + "Country:" + Color.RESET, informations["country"])
-        print(Color.GREEN + "Internet Service Provider:" + Color.RESET, informations["org"])
 
+        ip_info = {
+        "Information about the IP address": self.ip,
+        "IP": informations["ip"],
+        "Hostname": informations["hostname"],
+        "Location": informations["loc"],
+        "City": informations["city"],
+        "Region": informations["region"],
+        "Country": informations["country"],
+        "Internet Service Provider": informations["org"],
         # Additional information (if available)
-        print(Color.GREEN + "Postal Code:" + Color.RESET, informations.get("postal"))
-        print(Color.GREEN + "Time Zone:" + Color.RESET, informations.get("timezone"))
-        print(Color.GREEN + "Coordinates:" + Color.RESET, informations.get("loc"))
-        print(Color.GREEN + "Company Name:" + Color.RESET, informations.get("company"))
-        print(Color.GREEN + "ASN (Autonomous System Number):" + Color.RESET, informations.get("asn"))
-        print(Color.GREEN + "Network Prefix:" + Color.RESET, informations.get("network"))
-        print(Color.GREEN + "Network Prefix CIDR:" + Color.RESET, informations.get("cidr"))
-        print(Color.GREEN + "Connection Type:" + Color.RESET, informations.get("type"))
-        print(Color.GREEN + "Regional Internet Registry (RIR):" + Color.RESET, informations.get("region"))
-        print(Color.GREEN + "IP Block:" + Color.RESET, informations.get("ip_block"))
-
+        "Postal Code": informations.get("postal"),
+        "Time Zone": informations.get("timezone"),
+        "Coordinates": informations.get("loc"),
+        "Company Name": informations.get("company"),
+        "ASN (Autonomous System Number)": informations.get("asn"),
+        "Network Prefix": informations.get("network"),
+        "Network Prefix CIDR": informations.get("cidr"),
+        "Connection Type": informations.get("type"),
+        "Regional Internet Registry (RIR)": informations.get("region"),
+        "IP Block": informations.get("ip_block")
+        }
+        
         ic = InfoIp(self.ip)
         ic.ip_calculator(all=True)
 
+        return ip_info
+
 
 class UserScan:
     def __init__(self, user_name):
         self.user_name = user_name
 
     def found_users(self):
         for user in list_accounts:
```

### Comparing `direnumerate-3.0rc5/direnumerate/cli.py` & `direnumerate-3.0rc6/direnumerate/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,22 +92,22 @@
     parser.add_argument("-p", "--ports", nargs='+', type=int, help="Ports to scan (e.g., 22 80 443)")
     
     # Add arguments for log scanning
     parser.add_argument("-log", "--logname", help="Log Name")
     parser.add_argument("-key", "--keyword", help="Key Word")
     
     # Add arguments for IP info scanning
-    parser.add_argument("--info-target", help="Target host for info scanning")
+    parser.add_argument("--info", help="Target host for info scanning")
 
     args = parser.parse_args()
     
     if args.logname and args.keyword:
         find_pattern(args)
     elif args.ports:
         port_scan(args)
-    elif args.info_target:
+    elif args.info:
         show_info_ip(args)
     else:
         dir_scan(args)
 
 if __name__ == "__main__":
     main()
```

### Comparing `direnumerate-3.0rc5/direnumerate/createlist.py` & `direnumerate-3.0rc6/direnumerate/createlist.py`

 * *Files identical despite different names*

### Comparing `direnumerate-3.0rc5/direnumerate/ipcalculator.py` & `direnumerate-3.0rc6/direnumerate/ipcalculator.py`

 * *Files identical despite different names*

### Comparing `direnumerate-3.0rc5/direnumerate.egg-info/PKG-INFO` & `direnumerate-3.0rc6/direnumerate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: direnumerate
-Version: 3.0rc5
+Version: 3.0rc6
 Summary: Python 3 library for directory enumeration tool in web applications.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: GPLv2 license
 Project-URL: Homepage, https://github.com/juanbindez/direnumerate
 Project-URL: Bug Reports, https://github.com/juanbindez/direnumerate/issues
 Project-URL: Read the Docs, http://direnumerate.readthedocs.io/
 Keywords: web,enumerate,directory,tools,cli,scan
@@ -67,27 +67,27 @@
     pip install direnumerate --break-system-packages
 ----------
 
 ## Command line usage:
 
 ### Directory Scan:
 
-    direnumerate Ds -t testphp.vulnweb.com -w wordlist.txt
+    direnumerate -t testphp.vulnweb.com -w wordlist.txt
 
 ### Post Scan:
 
-    direnumerate Ps -t 44.228.249.3 -p 22 80 443
+    direnumerate -t 44.228.249.3 -p 22 80 443
 
 ### Finds patterns in logs:
 
-    direnumerate Fp -log test.log -key ERROR
+    direnumerate -log test.log -key ERROR
 
 ### IP Info:
 
-    direnumerate info -t 8.8.8.8
+    direnumerate --info -t 8.8.8.8
 
 
 ## Scripts usage:
 
 ### Directory Scan in Websites:
 
 ```python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: direnumerate Version: 3.0rc5 Summary: Python 3
+Metadata-Version: 2.1 Name: direnumerate Version: 3.0rc6 Summary: Python 3
 library for directory enumeration tool in web applications. Author-email: Juan
 Bindez
 gmail.com> License: GPLv2 license Project-URL: Homepage, https://github.com/
 juanbindez/direnumerate Project-URL: Bug Reports, https://github.com/
 juanbindez/direnumerate/issues Project-URL: Read the Docs, http://
 direnumerate.readthedocs.io/ Keywords: web,enumerate,directory,tools,cli,scan
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
@@ -30,22 +30,22 @@
 directory and file enumeration on web servers. It is useful for security
 professionals and system administrators who want to identify hidden resources
 and assess the security of web applications. ## Key Features - Enumeration of
 directories and files on web servers. - Creates a wordlist automatically -
 Wordlist customization. - Detailed output of findings. - Support for multiple
 URL schemes (http, https, etc.). ## install: pip install direnumerate ---------
 -------- ## install in ubuntu: pip install direnumerate --break-system-packages
----------- ## Command line usage: ### Directory Scan: direnumerate Ds -
-t testphp.vulnweb.com -w wordlist.txt ### Post Scan: direnumerate Ps -
-t 44.228.249.3 -p 22 80 443 ### Finds patterns in logs: direnumerate Fp -log
-test.log -key ERROR ### IP Info: direnumerate info -t 8.8.8.8 ## Scripts usage:
-### Directory Scan in Websites: ```python from direnumerate import DirScan url
-= "testphp.vulnweb.com" wordlist = "wordlist.txt" enum = DirScan(url)
-enum.dir_enum(wordlist) ``` ---------- ### User Accont Scan: ```python from
-direnumerate import UserScan user = "username" found = UserScan(user)
+---------- ## Command line usage: ### Directory Scan: direnumerate -
+t testphp.vulnweb.com -w wordlist.txt ### Post Scan: direnumerate -
+t 44.228.249.3 -p 22 80 443 ### Finds patterns in logs: direnumerate -log
+test.log -key ERROR ### IP Info: direnumerate --info -t 8.8.8.8 ## Scripts
+usage: ### Directory Scan in Websites: ```python from direnumerate import
+DirScan url = "testphp.vulnweb.com" wordlist = "wordlist.txt" enum = DirScan
+(url) enum.dir_enum(wordlist) ``` ---------- ### User Accont Scan: ```python
+from direnumerate import UserScan user = "username" found = UserScan(user)
 found.found_users() ``` ---------- ### Port Scan: ```python from direnumerate
 import PortScan ip = "44.228.249.3" list_ports = [22, 80, 443] scan = PortScan
 (ip) scan.scan_ports(list_ports) ``` ---------- ### Finds patterns in logs:
 ```python from direnumerate import FindPatterns log = "test.log" key = "ERROR"
 fp = FindPatterns(log) fp.find_in_log(keyword=key) ``` ### IP Info: ```python
 from direnumerate import InfoIp ip = "8.8.8.8" ipinfo = InfoIp(ip)
 ipinfo.show_info() ``` ----------
```

### Comparing `direnumerate-3.0rc5/pyproject.toml` & `direnumerate-3.0rc6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "direnumerate"
-version = "3.0-rc5"
+version = "3.0-rc6"
 authors = [
   { name="Juan Bindez", email="juanbindez780@gmail.com" },
 ]
 description = "Python 3 library for directory enumeration tool in web applications."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "GPLv2 license"}
```

