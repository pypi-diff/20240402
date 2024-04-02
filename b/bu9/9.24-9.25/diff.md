# Comparing `tmp/bu9-9.24.tar.gz` & `tmp/bu9-9.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bu9-9.24.tar", last modified: Tue Apr  2 17:26:49 2024, max compression
+gzip compressed data, was "bu9-9.25.tar", last modified: Tue Apr  2 18:39:32 2024, max compression
```

## Comparing `bu9-9.24.tar` & `bu9-9.25.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 17:26:49.763514 bu9-9.24/
--rw-rw-rw-   0        0        0       49 2024-04-02 17:26:49.760515 bu9-9.24/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-02 17:26:49.757519 bu9-9.24/bu9.egg-info/
--rw-rw-rw-   0        0        0       49 2024-04-02 17:26:49.000000 bu9-9.24/bu9.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      153 2024-04-02 17:26:49.000000 bu9-9.24/bu9.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 17:26:49.000000 bu9-9.24/bu9.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-04-02 17:26:49.000000 bu9-9.24/bu9.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        4 2024-04-02 17:26:49.000000 bu9-9.24/bu9.egg-info/top_level.txt
--rw-rw-rw-   0        0        0   326568 2024-04-02 17:25:48.000000 bu9-9.24/bu9.py
--rw-rw-rw-   0        0        0       42 2024-04-02 17:26:49.765513 bu9-9.24/setup.cfg
--rw-rw-rw-   0        0        0      220 2024-04-02 17:26:38.000000 bu9-9.24/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 18:39:32.065046 bu9-9.25/
+-rw-rw-rw-   0        0        0       49 2024-04-02 18:39:32.063048 bu9-9.25/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-02 18:39:32.062048 bu9-9.25/bu9.egg-info/
+-rw-rw-rw-   0        0        0       49 2024-04-02 18:39:31.000000 bu9-9.25/bu9.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      153 2024-04-02 18:39:31.000000 bu9-9.25/bu9.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 18:39:31.000000 bu9-9.25/bu9.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-04-02 18:39:31.000000 bu9-9.25/bu9.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        4 2024-04-02 18:39:31.000000 bu9-9.25/bu9.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0   326568 2024-04-02 18:38:46.000000 bu9-9.25/bu9.py
+-rw-rw-rw-   0        0        0       42 2024-04-02 18:39:32.066046 bu9-9.25/setup.cfg
+-rw-rw-rw-   0        0        0      220 2024-04-02 18:39:23.000000 bu9-9.25/setup.py
```

### Comparing `bu9-9.24/bu9.py` & `bu9-9.25/bu9.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #programmed by ssskingsss for python
-
+def main():
+    os.system('cls' if os.name == 'nt' else 'clear')
 
 import subprocess
 import sys
 
 required_modules = [
     ('time', None),
     ('os', None),
@@ -4892,10 +4893,9 @@
   if choice == "99":
     print("\033[96mThank you for using\nBUGHUNGERS PRO ®\033[0m")
     time.sleep(1)
     print("\033[96mHave Nice Day ;) \033[0m")
     time.sleep(1.5)
     os.system('cls' if os.name == 'nt' else 'clear')
     menu_loop = False
-def main():
-    os.system('cls' if os.name == 'nt' else 'clear')
+
```

