# Comparing `tmp/apkpatcher-0.1.1.tar.gz` & `tmp/apkpatcher-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apkpatcher-0.1.1.tar", last modified: Sat Mar 23 19:01:11 2024, max compression
+gzip compressed data, was "apkpatcher-0.1.2.tar", last modified: Tue Apr  2 21:37:07 2024, max compression
```

## Comparing `apkpatcher-0.1.1.tar` & `apkpatcher-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-23 19:01:11.805752 apkpatcher-0.1.1/
--rw-rw-rw-   0 root         (0) root         (0)    18046 2024-03-23 19:00:45.000000 apkpatcher-0.1.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      131 2024-03-23 19:00:45.000000 apkpatcher-0.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    23045 2024-03-23 19:01:11.805752 apkpatcher-0.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1581 2024-03-23 19:00:45.000000 apkpatcher-0.1.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-03-23 19:00:45.000000 apkpatcher-0.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-23 19:01:11.805752 apkpatcher-0.1.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-23 19:01:11.802085 apkpatcher-0.1.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-23 19:01:11.803918 apkpatcher-0.1.1/src/apkpatcher/
--rw-rw-rw-   0 root         (0) root         (0)    26473 2024-03-23 19:00:45.000000 apkpatcher-0.1.1/src/apkpatcher/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      155 2024-03-23 19:00:45.000000 apkpatcher-0.1.1/src/apkpatcher/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     2748 2024-03-23 19:00:45.000000 apkpatcher-0.1.1/src/apkpatcher/cli.py
--rw-rw-rw-   0 root         (0) root         (0)       17 2024-03-23 19:00:45.000000 apkpatcher-0.1.1/src/apkpatcher/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-23 19:01:11.804835 apkpatcher-0.1.1/src/apkpatcher.egg-info/
--rw-r--r--   0 root         (0) root         (0)    23045 2024-03-23 19:01:11.000000 apkpatcher-0.1.1/src/apkpatcher.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      373 2024-03-23 19:01:11.000000 apkpatcher-0.1.1/src/apkpatcher.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-23 19:01:11.000000 apkpatcher-0.1.1/src/apkpatcher.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2024-03-23 19:01:11.000000 apkpatcher-0.1.1/src/apkpatcher.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       36 2024-03-23 19:01:11.000000 apkpatcher-0.1.1/src/apkpatcher.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-03-23 19:01:11.000000 apkpatcher-0.1.1/src/apkpatcher.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 21:37:07.659760 apkpatcher-0.1.2/
+-rw-rw-rw-   0 root         (0) root         (0)    18046 2024-04-02 21:36:40.000000 apkpatcher-0.1.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      131 2024-04-02 21:36:40.000000 apkpatcher-0.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    23045 2024-04-02 21:37:07.658760 apkpatcher-0.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1581 2024-04-02 21:36:40.000000 apkpatcher-0.1.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-02 21:36:40.000000 apkpatcher-0.1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 21:37:07.659760 apkpatcher-0.1.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 21:37:07.654760 apkpatcher-0.1.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 21:37:07.656760 apkpatcher-0.1.2/src/apkpatcher/
+-rw-rw-rw-   0 root         (0) root         (0)    26650 2024-04-02 21:36:40.000000 apkpatcher-0.1.2/src/apkpatcher/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      155 2024-04-02 21:36:40.000000 apkpatcher-0.1.2/src/apkpatcher/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2937 2024-04-02 21:36:40.000000 apkpatcher-0.1.2/src/apkpatcher/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-04-02 21:36:40.000000 apkpatcher-0.1.2/src/apkpatcher/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 21:37:07.658760 apkpatcher-0.1.2/src/apkpatcher.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    23045 2024-04-02 21:37:07.000000 apkpatcher-0.1.2/src/apkpatcher.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      373 2024-04-02 21:37:07.000000 apkpatcher-0.1.2/src/apkpatcher.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 21:37:07.000000 apkpatcher-0.1.2/src/apkpatcher.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2024-04-02 21:37:07.000000 apkpatcher-0.1.2/src/apkpatcher.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2024-04-02 21:37:07.000000 apkpatcher-0.1.2/src/apkpatcher.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-02 21:37:07.000000 apkpatcher-0.1.2/src/apkpatcher.egg-info/top_level.txt
```

### Comparing `apkpatcher-0.1.1/LICENSE` & `apkpatcher-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `apkpatcher-0.1.1/PKG-INFO` & `apkpatcher-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkpatcher
-Version: 0.1.1
+Version: 0.1.2
 Summary: Tool use as library or in cli to patch an APK, inject some libraries inside the APK or add a custom certificate
 Author-email: "Benoit Forgette (MadSquirrel)" <benoit.forgette@ci-yow.com>
 Maintainer-email: "Benoit Forgette (MadSquirrel)" <benoit.forgette@ci-yow.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc., <http://fsf.org/>
@@ -348,15 +348,15 @@
 Project-URL: Repository, https://gitlab.com/MadSquirrels/mobile/apkpatcher
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: sty
-Requires-Dist: pyaxml==0.0.6
+Requires-Dist: pyaxml==0.0.7
 Requires-Dist: androguard==4.1.1
 
 # README
 
 
 ## GENERAL INFO
```

### Comparing `apkpatcher-0.1.1/README.md` & `apkpatcher-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `apkpatcher-0.1.1/pyproject.toml` & `apkpatcher-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apkpatcher"
 dynamic = ["version", "readme"]
 dependencies = [
   'sty',
-  'pyaxml==0.0.6',
+  'pyaxml==0.0.7',
   'androguard==4.1.1',
 ]
 requires-python = ">=3.5"
 authors = [
   {name = "Benoit Forgette (MadSquirrel)", email = "benoit.forgette@ci-yow.com"},
 ]
 maintainers = [
```

### Comparing `apkpatcher-0.1.1/src/apkpatcher/__init__.py` & `apkpatcher-0.1.2/src/apkpatcher/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
         '''
         self.apk = apk
         self.arch = None
         self.sdktools = sdktools
         self.version = version
         self.final_dir = None
         self._pause = False
+        self.plugin = None
         self.path_build_tools = f"{sdktools}/build-tools/{version}/" if \
                 (sdktools and version) else ""
         self.network_certificates = []
 
 ################################################################################
 #                                                                              #
 #            CERTIFICATES                                                      #
@@ -309,23 +310,28 @@
 
         logging.info('The apk was signed!')
 
         logging.info('The file was optimized!')
 
     def pause(self, pause):
         self._pause = pause
+    
+    def set_plugin(self, plugin):
+        self.plugin = plugin
 
     def repackage_apk(self, target_file=None):
         '''
         repackage the apk
 
         Parameters:
                     - target_file (str) : the path of the new apk created if
                       none, a new apk will be created with suffix "_patched.apk"
         '''
+        if self.plugin:
+            subprocess.run([self.plugin, self.final_dir])
         if self._pause:
             print(f"You can modify the apk here: {self.final_dir}")
             input()
         if target_file is None:
             current_path = os.getcwd()
             target_file = os.path.join(current_path, self.apk.replace('.apk', '_patched.apk'))
```

### Comparing `apkpatcher-0.1.1/src/apkpatcher/cli.py` & `apkpatcher-0.1.2/src/apkpatcher/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -21,14 +21,15 @@
                         action='store_true')
     parser.add_argument('-c', '--custom-certificate', help='Install a custom network certificate inside the apk')
 
     parser.add_argument('-o', '--output-file', help='Specify the output file (patched)')
 
     parser.add_argument('-p', '--pause', help='pause before repackage the apk',
             action="store_true")
+    parser.add_argument('--plugin', help='execute load plugin (a python file with as argument the folder before the packaging)')
     parser.add_argument('-V', '--version', help='version of apkpatcher', action='store_true')
 
     args = parser.parse_args()
 
     if args.version:
         print(f"version {conf.VERSION}")
         return 0
@@ -52,14 +53,16 @@
 
     patcher = Patcher(args.apk, args.sdktools, args.version_buildtools)
     if args.custom_certificate:
         patcher.add_network_certificate(args.custom_certificate)
     if args.arch:
         patcher.set_arch(args.arch)
     patcher.pause(args.pause)
+    if args.plugin:
+        patcher.set_plugin(args.plugin)
     if args.output_file:
         patcher.patching(args.gadget,
                 output_file=args.output_file,
                 user_certificate=args.enable_user_certificates)
     else:
         patcher.patching(args.gadget,
                 user_certificate=args.enable_user_certificates)
```

### Comparing `apkpatcher-0.1.1/src/apkpatcher.egg-info/PKG-INFO` & `apkpatcher-0.1.2/src/apkpatcher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkpatcher
-Version: 0.1.1
+Version: 0.1.2
 Summary: Tool use as library or in cli to patch an APK, inject some libraries inside the APK or add a custom certificate
 Author-email: "Benoit Forgette (MadSquirrel)" <benoit.forgette@ci-yow.com>
 Maintainer-email: "Benoit Forgette (MadSquirrel)" <benoit.forgette@ci-yow.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc., <http://fsf.org/>
@@ -348,15 +348,15 @@
 Project-URL: Repository, https://gitlab.com/MadSquirrels/mobile/apkpatcher
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: sty
-Requires-Dist: pyaxml==0.0.6
+Requires-Dist: pyaxml==0.0.7
 Requires-Dist: androguard==4.1.1
 
 # README
 
 
 ## GENERAL INFO
```

