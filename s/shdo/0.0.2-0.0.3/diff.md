# Comparing `tmp/shdo-0.0.2.tar.gz` & `tmp/shdo-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shdo-0.0.2.tar", last modified: Tue Apr  2 11:59:28 2024, max compression
+gzip compressed data, was "shdo-0.0.3.tar", last modified: Tue Apr  2 12:11:44 2024, max compression
```

## Comparing `shdo-0.0.2.tar` & `shdo-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 11:59:28.249157 shdo-0.0.2/
--rw-rw-rw-   0        0        0       51 2024-04-02 11:59:28.245487 shdo-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-02 11:59:28.250121 shdo-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      263 2024-04-02 11:59:25.000000 shdo-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 11:59:28.242506 shdo-0.0.2/shdo.egg-info/
--rw-rw-rw-   0        0        0       51 2024-04-02 11:59:27.000000 shdo-0.0.2/shdo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      169 2024-04-02 11:59:28.000000 shdo-0.0.2/shdo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 11:59:27.000000 shdo-0.0.2/shdo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-04-02 11:59:27.000000 shdo-0.0.2/shdo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-04-02 11:59:27.000000 shdo-0.0.2/shdo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    12801 2024-04-02 11:59:00.000000 shdo-0.0.2/shdo.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:11:44.779994 shdo-0.0.3/
+-rw-rw-rw-   0        0        0      329 2024-04-02 12:11:44.778647 shdo-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-02 12:11:44.780592 shdo-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      580 2024-04-02 12:10:17.000000 shdo-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:11:44.776865 shdo-0.0.3/shdo.egg-info/
+-rw-rw-rw-   0        0        0      329 2024-04-02 12:11:44.000000 shdo-0.0.3/shdo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      169 2024-04-02 12:11:44.000000 shdo-0.0.3/shdo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 12:11:44.000000 shdo-0.0.3/shdo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-04-02 12:11:44.000000 shdo-0.0.3/shdo.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-04-02 12:11:44.000000 shdo-0.0.3/shdo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    12848 2024-04-02 12:05:54.000000 shdo-0.0.3/shdo.py
```

### Comparing `shdo-0.0.2/shdo.py` & `shdo-0.0.3/shdo.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     # build the command
     parameters = ""
     if argc >= 3:
         for parameter in argv[2:]:
             parameters += f" '{parameter}'"
 
     # run the command
-    result = run_command(argv[1], parameters, verbose=True)
+    result = run_command(argv[1], parameters, verbose=False)
     if result is None:
         return 1
     
     # end of process
     return result
 
 
@@ -68,18 +68,15 @@
     # check if we are already connected
     if _adb.is_connected(verbose=verbose) == False:
 
         # connect to the adb server
         if _adb.connect(verbose=verbose) == False:
 
             # print the error if needed
-            if verbose == True:
-                print("Error: Couldn't connect to the adb server.")
-                print("Are you sure the adb server is paired with Termux ?")
-                print("Are you sure the adb wi-fi is on ?")
+            print("Error: Couldn't connect to the adb server. Are you sure the adb server is paired with Termux ? Are you sure the adb wi-fi is on ?")
             
             # couldn't connect to the adb server
             return None
         
     # auto-bounce the file or executable if needed
     if SHDO_AUTO_BOUNCE == True:
 
@@ -214,14 +211,18 @@
         if adb_server_port is not None:
             if _adb.try_connect(adb_server_port, verbose=verbose) == True:
                 return True
         
         # find all the opened tcp ports
         possible_ports = _network.scan_tcp_ports(verbose=verbose)
 
+        # print if verbose is enabled
+        if verbose == True:
+            print("[*] Trying to connect to the open ports...")
+
         # find the new adb server port with brute-forcing
         current_adb_port = None
         threads = []
         for port in possible_ports:
             thread = Thread(target=_adb.try_connect, args=(port, verbose))
             thread.start()
             threads.append(thread)
```

