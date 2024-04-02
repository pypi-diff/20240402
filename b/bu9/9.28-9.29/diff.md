# Comparing `tmp/bu9-9.28.tar.gz` & `tmp/bu9-9.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bu9-9.28.tar", last modified: Tue Apr  2 19:04:46 2024, max compression
+gzip compressed data, was "bu9-9.29.tar", last modified: Tue Apr  2 19:14:37 2024, max compression
```

## Comparing `bu9-9.28.tar` & `bu9-9.29.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 19:04:46.799059 bu9-9.28/
--rw-rw-rw-   0        0        0       49 2024-04-02 19:04:46.793063 bu9-9.28/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-02 19:04:46.791063 bu9-9.28/bu9.egg-info/
--rw-rw-rw-   0        0        0       49 2024-04-02 19:04:46.000000 bu9-9.28/bu9.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      153 2024-04-02 19:04:46.000000 bu9-9.28/bu9.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 19:04:46.000000 bu9-9.28/bu9.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-04-02 19:04:46.000000 bu9-9.28/bu9.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        4 2024-04-02 19:04:46.000000 bu9-9.28/bu9.egg-info/top_level.txt
--rw-rw-rw-   0        0        0   328054 2024-04-02 19:03:50.000000 bu9-9.28/bu9.py
--rw-rw-rw-   0        0        0       42 2024-04-02 19:04:46.800059 bu9-9.28/setup.cfg
--rw-rw-rw-   0        0        0      220 2024-04-02 19:04:31.000000 bu9-9.28/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:14:37.769118 bu9-9.29/
+-rw-rw-rw-   0        0        0       49 2024-04-02 19:14:37.763126 bu9-9.29/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-02 19:14:37.758123 bu9-9.29/bu9.egg-info/
+-rw-rw-rw-   0        0        0       49 2024-04-02 19:14:37.000000 bu9-9.29/bu9.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      153 2024-04-02 19:14:37.000000 bu9-9.29/bu9.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 19:14:37.000000 bu9-9.29/bu9.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-04-02 19:14:37.000000 bu9-9.29/bu9.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        4 2024-04-02 19:14:37.000000 bu9-9.29/bu9.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0   328691 2024-04-02 19:14:14.000000 bu9-9.29/bu9.py
+-rw-rw-rw-   0        0        0       42 2024-04-02 19:14:37.769118 bu9-9.29/setup.cfg
+-rw-rw-rw-   0        0        0      220 2024-04-02 19:14:21.000000 bu9-9.29/setup.py
```

### Comparing `bu9-9.28/bu9.py` & `bu9-9.29/bu9.py`

 * *Files 0% similar despite different names*

```diff
@@ -4064,16 +4064,15 @@
         if choice == '1':
             print("Returning to BUGHUNTERS PRO...")
             time.sleep(1)
             os.system('cls' if os.name == 'nt' else 'clear')
             script0()
             return
         if choice == '2':
-            help()
-            sys.exit
+            helpmain()
         else:
             os.system('cls' if os.name == 'nt' else 'clear')
             return
         script0()
 
 def script22():
     import sys
@@ -4662,15 +4661,37 @@
         if num_domains > 0:
             print("Archived URLs:")
             print(result)
             save_output_to_file(result)
 
     time.sleep(2)
     os.system('cls' if os.name == 'nt' else 'clear')
-    get_input_from_file_or_domain()   
+    # Menu
+    print("""
+    ===================================
+                  Menu                
+    ===================================
+    1. Return to main menu
+    2. Proceed to script
+    """)
+
+    while True:
+        choice = input("(2)continue or hit enter to return to main: ")  
+        if choice == '1':
+            print("Returning to BUGHUNTERS PRO...")
+            time.sleep(1)
+            os.system('cls' if os.name == 'nt' else 'clear')
+            script0()
+            return
+        if choice == '2':
+            get_input_from_file_or_domain()
+        else:
+            os.system('cls' if os.name == 'nt' else 'clear')
+            return
+      
     
 def script26():
     import ssl
     from cryptography import x509
     from cryptography.hazmat.backends import default_backend
     import certifi
     import os
```

