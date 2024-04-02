# Comparing `tmp/bu9-9.27.tar.gz` & `tmp/bu9-9.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bu9-9.27.tar", last modified: Tue Apr  2 18:55:13 2024, max compression
+gzip compressed data, was "bu9-9.28.tar", last modified: Tue Apr  2 19:04:46 2024, max compression
```

## Comparing `bu9-9.27.tar` & `bu9-9.28.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 18:55:13.633273 bu9-9.27/
--rw-rw-rw-   0        0        0       49 2024-04-02 18:55:13.630274 bu9-9.27/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-02 18:55:13.628275 bu9-9.27/bu9.egg-info/
--rw-rw-rw-   0        0        0       49 2024-04-02 18:55:13.000000 bu9-9.27/bu9.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      153 2024-04-02 18:55:13.000000 bu9-9.27/bu9.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 18:55:13.000000 bu9-9.27/bu9.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-04-02 18:55:13.000000 bu9-9.27/bu9.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        4 2024-04-02 18:55:13.000000 bu9-9.27/bu9.egg-info/top_level.txt
--rw-rw-rw-   0        0        0   327348 2024-04-02 18:54:46.000000 bu9-9.27/bu9.py
--rw-rw-rw-   0        0        0       42 2024-04-02 18:55:13.634272 bu9-9.27/setup.cfg
--rw-rw-rw-   0        0        0      220 2024-04-02 18:55:02.000000 bu9-9.27/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 19:04:46.799059 bu9-9.28/
+-rw-rw-rw-   0        0        0       49 2024-04-02 19:04:46.793063 bu9-9.28/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-02 19:04:46.791063 bu9-9.28/bu9.egg-info/
+-rw-rw-rw-   0        0        0       49 2024-04-02 19:04:46.000000 bu9-9.28/bu9.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      153 2024-04-02 19:04:46.000000 bu9-9.28/bu9.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 19:04:46.000000 bu9-9.28/bu9.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-04-02 19:04:46.000000 bu9-9.28/bu9.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        4 2024-04-02 19:04:46.000000 bu9-9.28/bu9.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0   328054 2024-04-02 19:03:50.000000 bu9-9.28/bu9.py
+-rw-rw-rw-   0        0        0       42 2024-04-02 19:04:46.800059 bu9-9.28/setup.cfg
+-rw-rw-rw-   0        0        0      220 2024-04-02 19:04:31.000000 bu9-9.28/setup.py
```

### Comparing `bu9-9.27/bu9.py` & `bu9-9.28/bu9.py`

 * *Files 1% similar despite different names*

```diff
@@ -4045,16 +4045,40 @@
             os.system('cls' if os.name == 'nt' else 'clear')
             crypto_installer()
         else:
             os.system('cls' if os.name == 'nt' else 'clear')
             script0()
 
     if __name__ == "__main__":
-        helpmain()
-        
+        helpmain()    
+    time.sleep(0.5)
+    print("""
+    ===================================
+                Menu                
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
+            help()
+            sys.exit
+        else:
+            os.system('cls' if os.name == 'nt' else 'clear')
+            return
+        script0()
+
 def script22():
     import sys
     lime = fg('#00FF00')
     blue = fg('#0000A5')
     pink = fg('#FF69B4')
     yuh_fada = '\033[0m'
```

