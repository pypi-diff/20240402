# Comparing `tmp/bu9-9.26.tar.gz` & `tmp/bu9-9.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bu9-9.26.tar", last modified: Tue Apr  2 18:48:41 2024, max compression
+gzip compressed data, was "bu9-9.27.tar", last modified: Tue Apr  2 18:55:13 2024, max compression
```

## Comparing `bu9-9.26.tar` & `bu9-9.27.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 18:48:41.715789 bu9-9.26/
--rw-rw-rw-   0        0        0       49 2024-04-02 18:48:41.711790 bu9-9.26/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-02 18:48:41.709792 bu9-9.26/bu9.egg-info/
--rw-rw-rw-   0        0        0       49 2024-04-02 18:48:41.000000 bu9-9.26/bu9.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      153 2024-04-02 18:48:41.000000 bu9-9.26/bu9.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 18:48:41.000000 bu9-9.26/bu9.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-04-02 18:48:41.000000 bu9-9.26/bu9.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        4 2024-04-02 18:48:41.000000 bu9-9.26/bu9.egg-info/top_level.txt
--rw-rw-rw-   0        0        0   326583 2024-04-02 18:47:55.000000 bu9-9.26/bu9.py
--rw-rw-rw-   0        0        0       42 2024-04-02 18:48:41.722785 bu9-9.26/setup.cfg
--rw-rw-rw-   0        0        0      220 2024-04-02 18:48:29.000000 bu9-9.26/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 18:55:13.633273 bu9-9.27/
+-rw-rw-rw-   0        0        0       49 2024-04-02 18:55:13.630274 bu9-9.27/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-02 18:55:13.628275 bu9-9.27/bu9.egg-info/
+-rw-rw-rw-   0        0        0       49 2024-04-02 18:55:13.000000 bu9-9.27/bu9.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      153 2024-04-02 18:55:13.000000 bu9-9.27/bu9.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 18:55:13.000000 bu9-9.27/bu9.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-04-02 18:55:13.000000 bu9-9.27/bu9.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        4 2024-04-02 18:55:13.000000 bu9-9.27/bu9.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0   327348 2024-04-02 18:54:46.000000 bu9-9.27/bu9.py
+-rw-rw-rw-   0        0        0       42 2024-04-02 18:55:13.634272 bu9-9.27/setup.cfg
+-rw-rw-rw-   0        0        0      220 2024-04-02 18:55:02.000000 bu9-9.27/setup.py
```

### Comparing `bu9-9.26/bu9.py` & `bu9-9.27/bu9.py`

 * *Files 1% similar despite different names*

```diff
@@ -3489,39 +3489,41 @@
 
             decode_vmess_file(input_file, output_file)
         if __name__ == '__main__':
             try:
                 a2()
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
-
-            while True:
-                choice = input("(2)continue or hit enter to return to main: ")  
-                if choice == '1':
-                    print("Returning to BUGHUNTERS PRO...")
-                    time.sleep(1)
-                    os.system('cls' if os.name == 'nt' else 'clear')
-                    teamerror()
-                    return
-                if choice == '2':
-                    a2()
-                    sys.exit
-                else:
-                    os.system('cls' if os.name == 'nt' else 'clear')
-                    return
+        time.sleep(1)
+        print("""
+        ===================================
+                    Menu                
+        ===================================
+        Hit enter to Return to main menu
+        1. to return to previous menu 
+        2. Proceed to the script
+        """)
+
+        while True:
+            choice = input("hit enter to return to main: ")       
+            if choice == '1':
+                print("Returning to BUGHUNTERS PRO...")
+                time.sleep(1)
+                os.system('cls' if os.name == 'nt' else 'clear')
                 teamerror()
                 
+            elif choice == '2':
+                a2()
+            else:
+                print("Returning to BUGHUNTERS PRO...")
+                time.sleep(1)
+                os.system('cls' if os.name == 'nt' else 'clear') 
+                script0()  
+                return
+
     def script003():
         
         def z1():
             print("Select an operation:")
             print("1. Replace host or IP address in vmess file")
             print("2. Update IP addresses in ss/vless/hyst file")
             print("3. SNI Replacement")
@@ -3616,38 +3618,41 @@
                             teamerror()
                             # Exit the loop to return to teamerror()
                             break
 
                 except Exception as e:
                     print(f"An error occurred: {e}")
 
-                time.sleep(0.5)
-                print("""
-                ===================================
-                            Menu                
-                ===================================
-                1. Return to main menu
-                2. Proceed to script
-                """)
+        time.sleep(1)
+        print("""
+        ===================================
+                    Menu                
+        ===================================
+        Hit enter to Return to main menu
+        1. to return to previous menu 
+        2. Proceed to the script
+        """)
+
+        while True:
+            choice = input("hit enter to return to main: ")       
+            if choice == '1':
+                print("Returning to BUGHUNTERS PRO...")
+                time.sleep(1)
+                os.system('cls' if os.name == 'nt' else 'clear')
+                teamerror()
+                
+            elif choice == '2':
+                z1()
+            else:
+                print("Returning to BUGHUNTERS PRO...")
+                time.sleep(1)
+                os.system('cls' if os.name == 'nt' else 'clear') 
+                script0()  
+                return
 
-                while True:
-                    choice = input("(2)continue or hit enter to return to main: ")  
-                    if choice == '1':
-                        print("Returning to BUGHUNTERS PRO...")
-                        time.sleep(1)
-                        os.system('cls' if os.name == 'nt' else 'clear')
-                        teamerror()
-                        return
-                    if choice == '2':
-                        z1()
-                        sys.exit
-                    else:
-                        os.system('cls' if os.name == 'nt' else 'clear')
-                        return
-                    teamerror()
             
     def script004():
         import base64
         import json
 
         def reencode_v2ray_data():
             input_file_name = input("Enter the name of the input file (e.g., v2ray_data.txt): ")
@@ -3768,38 +3773,41 @@
 
         if __name__ == '__main__':
                 try:
                     a4()
                 except Exception as e:
                     print(Fore.RED + f"An error occurred: {e} " + ENDC)
 
-                    time.sleep(0.5)
-                print("""
-                ===================================
-                            Menu                
-                ===================================
-                1. Return to main menu
-                2. Proceed to script
-                """)
+        time.sleep(1)
+        print("""
+        ===================================
+                    Menu                
+        ===================================
+        Hit enter to Return to main menu
+        1. to return to previous menu 
+        2. Proceed to the script
+        """)
+
+        while True:
+            choice = input("hit enter to return to main: ")       
+            if choice == '1':
+                print("Returning to BUGHUNTERS PRO...")
+                time.sleep(1)
+                os.system('cls' if os.name == 'nt' else 'clear')
+                teamerror()
+                
+            elif choice == '2':
+                a4()
+            else:
+                print("Returning to BUGHUNTERS PRO...")
+                time.sleep(1)
+                os.system('cls' if os.name == 'nt' else 'clear') 
+                script0()  
+                return
 
-                while True:
-                    choice = input("(2)continue or hit enter to return to main: ")  
-                    if choice == '1':
-                        print("Returning to BUGHUNTERS PRO...")
-                        time.sleep(1)
-                        os.system('cls' if os.name == 'nt' else 'clear')
-                        teamerror()
-                        return
-                    if choice == '2':
-                        a4()
-                        sys.exit
-                    else:
-                        os.system('cls' if os.name == 'nt' else 'clear')
-                        return
-                    teamerror()
                 
     time.sleep(1)
     print("1.""\033[32mGRAB CONFIGS\033[0m""         2.)""\033[32mDECODE vmess \033[0m")                       
     print("3.""\033[95mReplace all host/ip\033\033[0m""  4.)""\033[33mRe-encode Vmess\033[0m")
     print("5.""\033[32mTEST VMESS ONLY\033[0m")
     print("0.""\033[34mReturn to main\033[0m")
 
@@ -3855,14 +3863,41 @@
         it will then scan for subdomains and 
         save the found results to your txt files
         scan time 1hr - 5 mins\033[0m"""
         
         if __name__ == '__main__':
             slowprint(subdomainfinder1)
         return_to_menu()
+        time.sleep(1)
+        print("""
+        ===================================
+                    Menu                
+        ===================================
+        Hit enter to Return to main menu
+        1. to return to previous menu 
+        2. Proceed to the script
+        """)
+
+        while True:
+            choice = input("hit enter to return to main: ")       
+            if choice == '1':
+                print("Returning to BUGHUNTERS PRO...")
+                time.sleep(1)
+                os.system('cls' if os.name == 'nt' else 'clear')
+                teamerror()
+                
+            elif choice == '2':
+                sub_domain_finder()
+            else:
+                print("Returning to BUGHUNTERS PRO...")
+                time.sleep(1)
+                os.system('cls' if os.name == 'nt' else 'clear') 
+                script0()  
+                return
+
 
     def subdomain_enum():
         subdomain_enum_text = "\033[33m" + """     
         SUB DOMAIN ENUM
 
         This script sends a GET request to the Transparency Certificate
         of a website.
```

