# Comparing `tmp/bu9-9.25.tar.gz` & `tmp/bu9-9.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bu9-9.25.tar", last modified: Tue Apr  2 18:39:32 2024, max compression
+gzip compressed data, was "bu9-9.26.tar", last modified: Tue Apr  2 18:48:41 2024, max compression
```

## Comparing `bu9-9.25.tar` & `bu9-9.26.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 18:39:32.065046 bu9-9.25/
--rw-rw-rw-   0        0        0       49 2024-04-02 18:39:32.063048 bu9-9.25/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-02 18:39:32.062048 bu9-9.25/bu9.egg-info/
--rw-rw-rw-   0        0        0       49 2024-04-02 18:39:31.000000 bu9-9.25/bu9.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      153 2024-04-02 18:39:31.000000 bu9-9.25/bu9.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 18:39:31.000000 bu9-9.25/bu9.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-04-02 18:39:31.000000 bu9-9.25/bu9.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        4 2024-04-02 18:39:31.000000 bu9-9.25/bu9.egg-info/top_level.txt
--rw-rw-rw-   0        0        0   326568 2024-04-02 18:38:46.000000 bu9-9.25/bu9.py
--rw-rw-rw-   0        0        0       42 2024-04-02 18:39:32.066046 bu9-9.25/setup.cfg
--rw-rw-rw-   0        0        0      220 2024-04-02 18:39:23.000000 bu9-9.25/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 18:48:41.715789 bu9-9.26/
+-rw-rw-rw-   0        0        0       49 2024-04-02 18:48:41.711790 bu9-9.26/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-02 18:48:41.709792 bu9-9.26/bu9.egg-info/
+-rw-rw-rw-   0        0        0       49 2024-04-02 18:48:41.000000 bu9-9.26/bu9.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      153 2024-04-02 18:48:41.000000 bu9-9.26/bu9.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 18:48:41.000000 bu9-9.26/bu9.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-04-02 18:48:41.000000 bu9-9.26/bu9.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        4 2024-04-02 18:48:41.000000 bu9-9.26/bu9.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0   326583 2024-04-02 18:47:55.000000 bu9-9.26/bu9.py
+-rw-rw-rw-   0        0        0       42 2024-04-02 18:48:41.722785 bu9-9.26/setup.cfg
+-rw-rw-rw-   0        0        0      220 2024-04-02 18:48:29.000000 bu9-9.26/setup.py
```

### Comparing `bu9-9.25/bu9.py` & `bu9-9.26/bu9.py`

 * *Files 0% similar despite different names*

```diff
@@ -3411,39 +3411,42 @@
                 time.sleep(0.5)
 
         if __name__ == '__main__':
             try:
                 a1()
             except Exception as e:
                 print(f"An error occurred: {e}")
-            time.sleep(0.5)
-            print("""
-            ===================================
-                        Menu                
-            ===================================
-            1. Return to main menu
-            2. Proceed to script
-            """)
+        time.sleep(1)
+        print("""
+        ===================================
+                    Menu                
+        ===================================
+        Hit enter to Return to main menu
+        1. to return to previous menu 
+        2. Proceed to the script
+        """)
 
-            while True:
-                choice = input("(2)continue or hit enter to return to main: ")  
-                if choice == '1':
-                    print("Returning to BUGHUNTERS PRO...")
-                    time.sleep(1)
-                    os.system('cls' if os.name == 'nt' else 'clear')
-                    teamerror()
-                    return
-                if choice == '2':
-                    a1()
-                    sys.exit
-                else:
-                    os.system('cls' if os.name == 'nt' else 'clear')
-                    return
+        while True:
+            choice = input("hit enter to return to main: ")       
+            if choice == '1':
+                print("Returning to BUGHUNTERS PRO...")
+                time.sleep(1)
+                os.system('cls' if os.name == 'nt' else 'clear')
                 teamerror()
                 
+            elif choice == '2':
+                a1()
+            else:
+                print("Returning to BUGHUNTERS PRO...")
+                time.sleep(1)
+                os.system('cls' if os.name == 'nt' else 'clear') 
+                script0()  
+                return
+
+                
     def script002():
         
                          
         def decode_vmess_file(input_file, output_file):
             try:
                 with open(input_file, 'r') as file:
                     file_content = file.read()
```

