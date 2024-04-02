# Comparing `tmp/bu9-9.22.tar.gz` & `tmp/bu9-9.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bu9-9.22.tar", last modified: Tue Apr  2 13:41:37 2024, max compression
+gzip compressed data, was "bu9-9.23.tar", last modified: Tue Apr  2 14:11:38 2024, max compression
```

## Comparing `bu9-9.22.tar` & `bu9-9.23.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 13:41:37.067893 bu9-9.22/
--rw-rw-rw-   0        0        0       49 2024-04-02 13:41:37.064894 bu9-9.22/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-02 13:41:37.063894 bu9-9.22/bu9.egg-info/
--rw-rw-rw-   0        0        0       49 2024-04-02 13:41:36.000000 bu9-9.22/bu9.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      153 2024-04-02 13:41:36.000000 bu9-9.22/bu9.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 13:41:36.000000 bu9-9.22/bu9.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-04-02 13:41:36.000000 bu9-9.22/bu9.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        4 2024-04-02 13:41:36.000000 bu9-9.22/bu9.egg-info/top_level.txt
--rw-rw-rw-   0        0        0   321177 2024-04-02 13:32:57.000000 bu9-9.22/bu9.py
--rw-rw-rw-   0        0        0       42 2024-04-02 13:41:37.068892 bu9-9.22/setup.cfg
--rw-rw-rw-   0        0        0      220 2024-04-02 13:41:32.000000 bu9-9.22/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 14:11:38.639865 bu9-9.23/
+-rw-rw-rw-   0        0        0       49 2024-04-02 14:11:38.634870 bu9-9.23/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-02 14:11:38.632871 bu9-9.23/bu9.egg-info/
+-rw-rw-rw-   0        0        0       49 2024-04-02 14:11:38.000000 bu9-9.23/bu9.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      153 2024-04-02 14:11:38.000000 bu9-9.23/bu9.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 14:11:38.000000 bu9-9.23/bu9.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-04-02 14:11:38.000000 bu9-9.23/bu9.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        4 2024-04-02 14:11:38.000000 bu9-9.23/bu9.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0   326510 2024-04-02 14:10:46.000000 bu9-9.23/bu9.py
+-rw-rw-rw-   0        0        0       42 2024-04-02 14:11:38.640867 bu9-9.23/setup.cfg
+-rw-rw-rw-   0        0        0      220 2024-04-02 14:11:27.000000 bu9-9.23/setup.py
```

### Comparing `bu9-9.22/bu9.py` & `bu9-9.23/bu9.py`

 * *Files 1% similar despite different names*

```diff
@@ -3286,16 +3286,15 @@
         if choice == '2':
             o()
             sys.exit
         else:
             os.system('cls' if os.name == 'nt' else 'clear')
             return
             menu2()
-
-           
+   
 def teamerror():
     import requests
     import time
     import base64
     import os
     import re
     from tqdm import tqdm
@@ -3411,19 +3410,39 @@
                 time.sleep(0.5)
 
         if __name__ == '__main__':
             try:
                 a1()
             except Exception as e:
                 print(f"An error occurred: {e}")
-            finally:
-                time.sleep(2)
-                os.system('cls' if os.name == 'nt' else 'clear')
+            time.sleep(0.5)
+            print("""
+            ===================================
+                        Menu                
+            ===================================
+            1. Return to main menu
+            2. Proceed to script
+            """)
+
+            while True:
+                choice = input("(2)continue or hit enter to return to main: ")  
+                if choice == '1':
+                    print("Returning to BUGHUNTERS PRO...")
+                    time.sleep(1)
+                    os.system('cls' if os.name == 'nt' else 'clear')
+                    script0()
+                    return
+                if choice == '2':
+                    a1()
+                    sys.exit
+                else:
+                    os.system('cls' if os.name == 'nt' else 'clear')
+                    return
                 teamerror()
-                    
+                
     def script002():
         
                          
         def decode_vmess_file(input_file, output_file):
             try:
                 with open(input_file, 'r') as file:
                     file_content = file.read()
@@ -3466,19 +3485,39 @@
 
             decode_vmess_file(input_file, output_file)
         if __name__ == '__main__':
             try:
                 a2()
             except Exception as e:
                 print(f"An error occurred: {e}")
-            finally:
-                time.sleep(2)
-                os.system('cls' if os.name == 'nt' else 'clear')
+            time.sleep(0.5)
+            print("""
+            ===================================
+                        Menu                
+            ===================================
+            1. Return to main menu
+            2. Proceed to script
+            """)
+
+            while True:
+                choice = input("(2)continue or hit enter to return to main: ")  
+                if choice == '1':
+                    print("Returning to BUGHUNTERS PRO...")
+                    time.sleep(1)
+                    os.system('cls' if os.name == 'nt' else 'clear')
+                    script0()
+                    return
+                if choice == '2':
+                    a2()
+                    sys.exit
+                else:
+                    os.system('cls' if os.name == 'nt' else 'clear')
+                    return
                 teamerror()
-        
+                
     def script003():
         
         def z1():
             print("Select an operation:")
             print("1. Replace host or IP address in vmess file")
             print("2. Update IP addresses in ss/vless/hyst file")
             print("3. SNI Replacement")
@@ -3573,18 +3612,38 @@
                             teamerror()
                             # Exit the loop to return to teamerror()
                             break
 
                 except Exception as e:
                     print(f"An error occurred: {e}")
 
-                finally:
-                    time.sleep(2)
-                    os.system('cls' if os.name == 'nt' else 'clear')
-                    teamerror()  # Assuming you want to call teamerror() after the loop exits
+                time.sleep(0.5)
+                print("""
+                ===================================
+                            Menu                
+                ===================================
+                1. Return to main menu
+                2. Proceed to script
+                """)
+
+                while True:
+                    choice = input("(2)continue or hit enter to return to main: ")  
+                    if choice == '1':
+                        print("Returning to BUGHUNTERS PRO...")
+                        time.sleep(1)
+                        os.system('cls' if os.name == 'nt' else 'clear')
+                        script0()
+                        return
+                    if choice == '2':
+                        z1()
+                        sys.exit
+                    else:
+                        os.system('cls' if os.name == 'nt' else 'clear')
+                        return
+                    teamerror()
             
     def script004():
         import base64
         import json
 
         def reencode_v2ray_data():
             input_file_name = input("Enter the name of the input file (e.g., v2ray_data.txt): ")
@@ -3622,17 +3681,37 @@
             
             reencode_v2ray_data()
         if __name__ == '__main__':
                 try:
                     a3()
                 except Exception as e:
                     print(f"An error occurred: {e}")
-                finally:
-                    time.sleep(2)
-                    os.system('cls' if os.name == 'nt' else 'clear')
+                    time.sleep(0.5)
+                print("""
+                ===================================
+                            Menu                
+                ===================================
+                1. Return to main menu
+                2. Proceed to script
+                """)
+
+                while True:
+                    choice = input("(2)continue or hit enter to return to main: ")  
+                    if choice == '1':
+                        print("Returning to BUGHUNTERS PRO...")
+                        time.sleep(1)
+                        os.system('cls' if os.name == 'nt' else 'clear')
+                        script0()
+                        return
+                    if choice == '2':
+                        a3()
+                        sys.exit
+                    else:
+                        os.system('cls' if os.name == 'nt' else 'clear')
+                        return
                     teamerror()
                     
     def script005():
         
         def test_vmess_url(vmess_url):
             try:
                 decoded_vmess = base64.urlsafe_b64decode(vmess_url.split("://")[1]).decode("utf-8")
@@ -3685,17 +3764,37 @@
 
         if __name__ == '__main__':
                 try:
                     a4()
                 except Exception as e:
                     print(Fore.RED + f"An error occurred: {e} " + ENDC)
 
-                finally:
-                    time.sleep(2)
-                    os.system('cls' if os.name == 'nt' else 'clear')
+                    time.sleep(0.5)
+                print("""
+                ===================================
+                            Menu                
+                ===================================
+                1. Return to main menu
+                2. Proceed to script
+                """)
+
+                while True:
+                    choice = input("(2)continue or hit enter to return to main: ")  
+                    if choice == '1':
+                        print("Returning to BUGHUNTERS PRO...")
+                        time.sleep(1)
+                        os.system('cls' if os.name == 'nt' else 'clear')
+                        script0()
+                        return
+                    if choice == '2':
+                        a4()
+                        sys.exit
+                    else:
+                        os.system('cls' if os.name == 'nt' else 'clear')
+                        return
                     teamerror()
                 
     time.sleep(1)
     print("1.""\033[32mGRAB CONFIGS\033[0m""         2.)""\033[32mDECODE vmess \033[0m")                       
     print("3.""\033[95mReplace all host/ip\033\033[0m""  4.)""\033[33mRe-encode Vmess\033[0m")
     print("5.""\033[32mTEST VMESS ONLY\033[0m")
     print("0.""\033[34mReturn to main\033[0m")
@@ -3906,14 +4005,15 @@
             crypto_installer()
         else:
             os.system('cls' if os.name == 'nt' else 'clear')
             script0()
 
     if __name__ == "__main__":
         helpmain()
+        
 
 def script22():
     import sys
     lime = fg('#00FF00')
     blue = fg('#0000A5')
     pink = fg('#FF69B4')
     yuh_fada = '\033[0m'
@@ -4264,17 +4364,38 @@
                 file_name = input("Enter the file name (without extension): ")
                 file_path = os.path.join(os.path.dirname(__file__), f"{file_name}.txt")
                 save_to_file(file_path, result_lines)
         else:
             print("No results found.")
     if __name__ == "__main__":
         az()
-        time.sleep(2)
-        os.system('cls' if os.name == 'nt' else 'clear')
-        menu2()   
+        time.sleep(0.5)
+        print("""
+        ===================================
+                    Menu                
+        ===================================
+        1. Return to main menu
+        2. Proceed to script
+        """)
+
+        while True:
+            choice = input("(2)continue or hit enter to return to main: ")  
+            if choice == '1':
+                print("Returning to BUGHUNTERS PRO...")
+                time.sleep(1)
+                os.system('cls' if os.name == 'nt' else 'clear')
+                script0()
+                return
+            if choice == '2':
+                az()
+                sys.exit
+            else:
+                os.system('cls' if os.name == 'nt' else 'clear')
+                return
+            menu2()   
         
 def script24():
     import aiohttp
     import asyncio
     import socket
     import signal
     from urllib.parse import urlparse, urljoin
@@ -4342,18 +4463,39 @@
         save_output()
 
     if __name__ == "__main__":
         try:
             asyncio.run(ax())
         except KeyboardInterrupt:
             handle_interrupt()
-            time.sleep(2)
-            os.system('cls' if os.name == 'nt' else 'clear')
-            menu2()   
+            time.sleep(0.5)
+        print("""
+        ===================================
+                    Menu                
+        ===================================
+        1. Return to main menu
+        2. Proceed to script
+        """)
 
+        while True:
+            choice = input("(2)continue or hit enter to return to main: ")  
+            if choice == '1':
+                print("Returning to BUGHUNTERS PRO...")
+                time.sleep(1)
+                os.system('cls' if os.name == 'nt' else 'clear')
+                script0()
+                return
+            if choice == '2':
+                ax()
+                sys.exit
+            else:
+                os.system('cls' if os.name == 'nt' else 'clear')
+                return
+            menu2()
+            
 def script25():
     import datetime
     import json
     import os
     from requests import get
     from requests.exceptions import ConnectionError
     
@@ -4456,15 +4598,15 @@
         if num_domains > 0:
             print("Archived URLs:")
             print(result)
             save_output_to_file(result)
 
     time.sleep(2)
     os.system('cls' if os.name == 'nt' else 'clear')
-    menu2()   
+    get_input_from_file_or_domain()   
     
 def script26():
     import ssl
     from cryptography import x509
     from cryptography.hazmat.backends import default_backend
     import certifi
     import os
```

