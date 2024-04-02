# Comparing `tmp/waymore-4.0.tar.gz` & `tmp/waymore-4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waymore-4.0.tar", last modified: Mon Apr  1 16:43:55 2024, max compression
+gzip compressed data, was "waymore-4.1.tar", last modified: Tue Apr  2 16:37:57 2024, max compression
```

## Comparing `waymore-4.0.tar` & `waymore-4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-04-01 16:43:55.858136 waymore-4.0/
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)     1068 2024-03-20 18:00:02.000000 waymore-4.0/LICENSE
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)    47142 2024-04-01 16:43:55.840693 waymore-4.0/PKG-INFO
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)    46691 2024-04-01 16:15:25.000000 waymore-4.0/README.md
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       38 2024-04-01 16:43:55.861550 waymore-4.0/setup.cfg
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)     2142 2024-04-01 16:43:41.000000 waymore-4.0/setup.py
-drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-04-01 16:43:55.526673 waymore-4.0/waymore/
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       17 2024-03-21 18:17:06.000000 waymore-4.0/waymore/__init__.py
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)   166776 2024-04-01 16:37:51.000000 waymore-4.0/waymore/waymore.py
-drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-04-01 16:43:55.830013 waymore-4.0/waymore.egg-info/
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)    47142 2024-04-01 16:43:55.000000 waymore-4.0/waymore.egg-info/PKG-INFO
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)      253 2024-04-01 16:43:55.000000 waymore-4.0/waymore.egg-info/SOURCES.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)        1 2024-04-01 16:43:55.000000 waymore-4.0/waymore.egg-info/dependency_links.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       49 2024-04-01 16:43:55.000000 waymore-4.0/waymore.egg-info/entry_points.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       63 2024-04-01 16:43:55.000000 waymore-4.0/waymore.egg-info/requires.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)        8 2024-04-01 16:43:55.000000 waymore-4.0/waymore.egg-info/top_level.txt
+drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-04-02 16:37:57.147115 waymore-4.1/
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)     1068 2024-03-20 18:00:02.000000 waymore-4.1/LICENSE
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)    47245 2024-04-02 16:37:57.135640 waymore-4.1/PKG-INFO
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)    46794 2024-04-02 16:34:35.000000 waymore-4.1/README.md
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       38 2024-04-02 16:37:57.148137 waymore-4.1/setup.cfg
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)     2142 2024-04-01 16:43:41.000000 waymore-4.1/setup.py
+drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-04-02 16:37:56.924503 waymore-4.1/waymore/
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       17 2024-04-02 16:35:08.000000 waymore-4.1/waymore/__init__.py
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)   166754 2024-04-02 16:34:25.000000 waymore-4.1/waymore/waymore.py
+drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-04-02 16:37:57.117277 waymore-4.1/waymore.egg-info/
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)    47245 2024-04-02 16:37:56.000000 waymore-4.1/waymore.egg-info/PKG-INFO
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)      253 2024-04-02 16:37:56.000000 waymore-4.1/waymore.egg-info/SOURCES.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)        1 2024-04-02 16:37:56.000000 waymore-4.1/waymore.egg-info/dependency_links.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       49 2024-04-02 16:37:56.000000 waymore-4.1/waymore.egg-info/entry_points.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       63 2024-04-02 16:37:56.000000 waymore-4.1/waymore.egg-info/requires.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)        8 2024-04-02 16:37:56.000000 waymore-4.1/waymore.egg-info/top_level.txt
```

### Comparing `waymore-4.0/LICENSE` & `waymore-4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `waymore-4.0/PKG-INFO` & `waymore-4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waymore
-Version: 4.0
+Version: 4.1
 Summary: Find way more from the Wayback Machine, Common Crawl, Alien Vault OTX, URLScan & VirusTotal!
 Home-page: https://github.com/xnl-h4ck3r/waymore
 Author: @xnl-h4ck3r
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: argparse
 Requires-Dist: requests
@@ -12,15 +12,15 @@
 Requires-Dist: termcolor
 Requires-Dist: psutil
 Requires-Dist: urlparse3
 Requires-Dist: tldextract
 
 <center><img src="https://github.com/xnl-h4ck3r/waymore/blob/main/waymore/images/title.png"></center>
 
-## About - v4.0
+## About - v4.1
 
 The idea behind **waymore** is to find even more links from the Wayback Machine than other existing tools.
 
 👉 The biggest difference between **waymore** and other tools is that it can also **download the archived responses** for URLs on wayback machine so that you can then search these for even more links, developer comments, extra parameters, etc. etc.
 👉 Also, other tools do not currenrtly deal with the rate limiting now in place by the sources, and will often just stop with incomplete results and not let you know they are incomplete.
 
 Anyone who does bug bounty will have likely used the amazing [waybackurls](https://github.com/tomnomnom/waybackurls) by @TomNomNoms. This tool gets URLs from [web.archive.org](https://web.archive.org) and additional links (if any) from one of the index collections on [index.commoncrawl.org](http://index.commoncrawl.org/).
@@ -43,20 +43,32 @@
 
 ## Installation
 
 **NOTE: If you already have a `config.yml` file, it will not be overwritten. The file `config.yml.NEW` will be created in the same directory. If you need the new config, remove `config.yml` and rename `config.yml.NEW` back to `config.yml`.**
 
 `waymore` supports **Python 3**.
 
-Install `waymore` in default(global) python environment.
+Install `waymore` in default (global) python environment.
+
+```bash
+pip install waymore
+```
+
+OR
 
 ```bash
 pip install git+https://github.com/xnl-h4ck3r/waymore.git -v
 ```
 
+You can upgrade with
+
+```bash
+pip install --upgrade waymore
+```
+
 ### pipx
 
 Quick setup in isolated python environment using [pipx](https://pypa.github.io/pipx/)
 
 ```bash
 pipx install git+https://github.com/xnl-h4ck3r/waymore.git
 ```
```

### Comparing `waymore-4.0/README.md` & `waymore-4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <center><img src="https://github.com/xnl-h4ck3r/waymore/blob/main/waymore/images/title.png"></center>
 
-## About - v4.0
+## About - v4.1
 
 The idea behind **waymore** is to find even more links from the Wayback Machine than other existing tools.
 
 👉 The biggest difference between **waymore** and other tools is that it can also **download the archived responses** for URLs on wayback machine so that you can then search these for even more links, developer comments, extra parameters, etc. etc.
 👉 Also, other tools do not currenrtly deal with the rate limiting now in place by the sources, and will often just stop with incomplete results and not let you know they are incomplete.
 
 Anyone who does bug bounty will have likely used the amazing [waybackurls](https://github.com/tomnomnom/waybackurls) by @TomNomNoms. This tool gets URLs from [web.archive.org](https://web.archive.org) and additional links (if any) from one of the index collections on [index.commoncrawl.org](http://index.commoncrawl.org/).
@@ -27,20 +27,32 @@
 
 ## Installation
 
 **NOTE: If you already have a `config.yml` file, it will not be overwritten. The file `config.yml.NEW` will be created in the same directory. If you need the new config, remove `config.yml` and rename `config.yml.NEW` back to `config.yml`.**
 
 `waymore` supports **Python 3**.
 
-Install `waymore` in default(global) python environment.
+Install `waymore` in default (global) python environment.
+
+```bash
+pip install waymore
+```
+
+OR
 
 ```bash
 pip install git+https://github.com/xnl-h4ck3r/waymore.git -v
 ```
 
+You can upgrade with
+
+```bash
+pip install --upgrade waymore
+```
+
 ### pipx
 
 Quick setup in isolated python environment using [pipx](https://pypa.github.io/pipx/)
 
 ```bash
 pipx install git+https://github.com/xnl-h4ck3r/waymore.git
 ```
```

### Comparing `waymore-4.0/setup.py` & `waymore-4.1/setup.py`

 * *Files identical despite different names*

### Comparing `waymore-4.0/waymore/waymore.py` & `waymore-4.1/waymore/waymore.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 import pickle
 import time
 import tldextract
 try:
     from . import __version__
 except:
     pass
-from tqdm import tqdm
 
 # Try to import psutil to show memory usage
 try:
     import psutil
 except:
     currentMemUsage = -1
     maxMemoryUsage = -1
```

### Comparing `waymore-4.0/waymore.egg-info/PKG-INFO` & `waymore-4.1/waymore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waymore
-Version: 4.0
+Version: 4.1
 Summary: Find way more from the Wayback Machine, Common Crawl, Alien Vault OTX, URLScan & VirusTotal!
 Home-page: https://github.com/xnl-h4ck3r/waymore
 Author: @xnl-h4ck3r
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: argparse
 Requires-Dist: requests
@@ -12,15 +12,15 @@
 Requires-Dist: termcolor
 Requires-Dist: psutil
 Requires-Dist: urlparse3
 Requires-Dist: tldextract
 
 <center><img src="https://github.com/xnl-h4ck3r/waymore/blob/main/waymore/images/title.png"></center>
 
-## About - v4.0
+## About - v4.1
 
 The idea behind **waymore** is to find even more links from the Wayback Machine than other existing tools.
 
 👉 The biggest difference between **waymore** and other tools is that it can also **download the archived responses** for URLs on wayback machine so that you can then search these for even more links, developer comments, extra parameters, etc. etc.
 👉 Also, other tools do not currenrtly deal with the rate limiting now in place by the sources, and will often just stop with incomplete results and not let you know they are incomplete.
 
 Anyone who does bug bounty will have likely used the amazing [waybackurls](https://github.com/tomnomnom/waybackurls) by @TomNomNoms. This tool gets URLs from [web.archive.org](https://web.archive.org) and additional links (if any) from one of the index collections on [index.commoncrawl.org](http://index.commoncrawl.org/).
@@ -43,20 +43,32 @@
 
 ## Installation
 
 **NOTE: If you already have a `config.yml` file, it will not be overwritten. The file `config.yml.NEW` will be created in the same directory. If you need the new config, remove `config.yml` and rename `config.yml.NEW` back to `config.yml`.**
 
 `waymore` supports **Python 3**.
 
-Install `waymore` in default(global) python environment.
+Install `waymore` in default (global) python environment.
+
+```bash
+pip install waymore
+```
+
+OR
 
 ```bash
 pip install git+https://github.com/xnl-h4ck3r/waymore.git -v
 ```
 
+You can upgrade with
+
+```bash
+pip install --upgrade waymore
+```
+
 ### pipx
 
 Quick setup in isolated python environment using [pipx](https://pypa.github.io/pipx/)
 
 ```bash
 pipx install git+https://github.com/xnl-h4ck3r/waymore.git
 ```
```

