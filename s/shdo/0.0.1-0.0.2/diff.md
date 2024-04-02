# Comparing `tmp/shdo-0.0.1.tar.gz` & `tmp/shdo-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shdo-0.0.1.tar", last modified: Tue Apr  2 11:55:08 2024, max compression
+gzip compressed data, was "shdo-0.0.2.tar", last modified: Tue Apr  2 11:59:28 2024, max compression
```

## Comparing `shdo-0.0.1.tar` & `shdo-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 11:55:08.572340 shdo-0.0.1/
--rw-rw-rw-   0        0        0       51 2024-04-02 11:55:08.569855 shdo-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-02 11:55:08.572842 shdo-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      263 2024-04-02 11:54:25.000000 shdo-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 11:55:08.567562 shdo-0.0.1/shdo.egg-info/
--rw-rw-rw-   0        0        0       51 2024-04-02 11:55:08.000000 shdo-0.0.1/shdo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      169 2024-04-02 11:55:08.000000 shdo-0.0.1/shdo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 11:55:08.000000 shdo-0.0.1/shdo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-04-02 11:55:08.000000 shdo-0.0.1/shdo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-04-02 11:55:08.000000 shdo-0.0.1/shdo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    12744 2024-04-02 11:54:42.000000 shdo-0.0.1/shdo.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:59:28.249157 shdo-0.0.2/
+-rw-rw-rw-   0        0        0       51 2024-04-02 11:59:28.245487 shdo-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-02 11:59:28.250121 shdo-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      263 2024-04-02 11:59:25.000000 shdo-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:59:28.242506 shdo-0.0.2/shdo.egg-info/
+-rw-rw-rw-   0        0        0       51 2024-04-02 11:59:27.000000 shdo-0.0.2/shdo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      169 2024-04-02 11:59:28.000000 shdo-0.0.2/shdo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 11:59:27.000000 shdo-0.0.2/shdo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-04-02 11:59:27.000000 shdo-0.0.2/shdo.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-04-02 11:59:27.000000 shdo-0.0.2/shdo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    12801 2024-04-02 11:59:00.000000 shdo-0.0.2/shdo.py
```

### Comparing `shdo-0.0.1/shdo.py` & `shdo-0.0.2/shdo.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,19 @@
 
 # shdo global variables
 current_adb_port = None
 connected_adb_port = None
 
 
 # main function
-def main(argc, argv):
+def main():
+
+    # parse the command line parameters
+    argc = len(sys_argv)
+    argv = sys_argv
 
     # check usage
     if argc <= 1:
         print("Usage: shdo <command> [parameters]")
         return 1
     
     # build the command
@@ -397,8 +401,8 @@
 
         # the port is assigned
         return False
 
 
 # entry point
 if __name__ == "__main__":
-    exit(main(len(sys_argv), sys_argv))
+    exit(main())
```

