# Comparing `tmp/feno-0.0.5.tar.gz` & `tmp/feno-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feno-0.0.5.tar", last modified: Wed Mar 27 19:40:36 2024, max compression
+gzip compressed data, was "feno-0.0.6.tar", last modified: Tue Apr  2 01:52:54 2024, max compression
```

## Comparing `feno-0.0.5.tar` & `feno-0.0.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-03-27 19:40:36.346663 feno-0.0.5/
--rw-r--r--   0 lion      (1000) lion      (1000)     1043 2024-03-26 18:23:42.000000 feno-0.0.5/LICENSE
--rw-r--r--   0 lion      (1000) lion      (1000)      191 2024-03-26 18:23:42.000000 feno-0.0.5/MANIFEST.in
--rw-r--r--   0 lion      (1000) lion      (1000)      918 2024-03-27 19:40:36.346663 feno-0.0.5/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)       46 2024-03-27 17:52:43.000000 feno-0.0.5/README.md
--rw-r--r--   0 lion      (1000) lion      (1000)      244 2024-03-26 18:23:42.000000 feno-0.0.5/changelog.md
--rw-r--r--   0 lion      (1000) lion      (1000)      310 2024-03-27 17:54:40.000000 feno-0.0.5/requirements.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-03-27 19:40:36.346663 feno-0.0.5/setup.cfg
--rw-r--r--   0 lion      (1000) lion      (1000)     3082 2024-03-27 17:53:37.000000 feno-0.0.5/setup.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-03-27 19:40:36.313330 feno-0.0.5/src/
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-03-27 19:40:36.333330 feno-0.0.5/src/feno/
--rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-03-27 19:40:25.000000 feno-0.0.5/src/feno/__init__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1934 2024-03-27 19:38:45.000000 feno-0.0.5/src/feno/__main__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     4220 2024-03-27 19:07:56.000000 feno-0.0.5/src/feno/actions.py
--rw-r--r--   0 lion      (1000) lion      (1000)      550 2024-03-26 19:17:45.000000 feno-0.0.5/src/feno/cases.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1274 2024-03-26 19:21:50.000000 feno-0.0.5/src/feno/check.py
--rw-r--r--   0 lion      (1000) lion      (1000)      938 2024-03-26 19:19:40.000000 feno-0.0.5/src/feno/css_style.py
--rw-r--r--   0 lion      (1000) lion      (1000)     3821 2024-03-27 17:09:25.000000 feno-0.0.5/src/feno/filter.py
--rw-r--r--   0 lion      (1000) lion      (1000)      823 2024-03-27 13:14:00.000000 feno-0.0.5/src/feno/html.py
--rw-r--r--   0 lion      (1000) lion      (1000)     2494 2024-03-27 13:44:12.000000 feno-0.0.5/src/feno/indexer.py
--rw-r--r--   0 lion      (1000) lion      (1000)     3326 2024-03-27 13:09:44.000000 feno-0.0.5/src/feno/jsontools.py
--rw-r--r--   0 lion      (1000) lion      (1000)      324 2024-03-27 15:51:58.000000 feno-0.0.5/src/feno/log.py
--rw-r--r--   0 lion      (1000) lion      (1000)    10327 2024-03-27 17:02:47.000000 feno-0.0.5/src/feno/mdpp.py
--rw-r--r--   0 lion      (1000) lion      (1000)     4859 2024-03-27 17:39:57.000000 feno-0.0.5/src/feno/remote_md.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1545 2024-03-27 16:55:35.000000 feno-0.0.5/src/feno/tree.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-03-27 19:40:36.343330 feno-0.0.5/src/feno.egg-info/
--rw-r--r--   0 lion      (1000) lion      (1000)      918 2024-03-27 19:40:36.000000 feno-0.0.5/src/feno.egg-info/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)      542 2024-03-27 19:40:36.000000 feno-0.0.5/src/feno.egg-info/SOURCES.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-03-27 19:40:36.000000 feno-0.0.5/src/feno.egg-info/dependency_links.txt
--rw-r--r--   0 lion      (1000) lion      (1000)      120 2024-03-27 19:40:36.000000 feno-0.0.5/src/feno.egg-info/entry_points.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       55 2024-03-27 19:40:36.000000 feno-0.0.5/src/feno.egg-info/requires.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        5 2024-03-27 19:40:36.000000 feno-0.0.5/src/feno.egg-info/top_level.txt
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-02 01:52:54.536522 feno-0.0.6/
+-rw-r--r--   0 lion      (1000) lion      (1000)     1043 2024-03-26 18:23:42.000000 feno-0.0.6/LICENSE
+-rw-r--r--   0 lion      (1000) lion      (1000)      191 2024-03-26 18:23:42.000000 feno-0.0.6/MANIFEST.in
+-rw-r--r--   0 lion      (1000) lion      (1000)      918 2024-04-02 01:52:54.536522 feno-0.0.6/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)       46 2024-03-27 17:52:43.000000 feno-0.0.6/README.md
+-rw-r--r--   0 lion      (1000) lion      (1000)      244 2024-03-26 18:23:42.000000 feno-0.0.6/changelog.md
+-rw-r--r--   0 lion      (1000) lion      (1000)      310 2024-03-27 17:54:40.000000 feno-0.0.6/requirements.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-04-02 01:52:54.539856 feno-0.0.6/setup.cfg
+-rw-r--r--   0 lion      (1000) lion      (1000)     3107 2024-04-01 17:24:14.000000 feno-0.0.6/setup.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-02 01:52:54.523189 feno-0.0.6/src/
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-02 01:52:54.533189 feno-0.0.6/src/feno/
+-rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-04-01 17:41:26.000000 feno-0.0.6/src/feno/__init__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     1851 2024-04-02 01:38:15.000000 feno-0.0.6/src/feno/__main__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     5019 2024-04-02 01:38:03.000000 feno-0.0.6/src/feno/actions.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      550 2024-03-26 19:17:45.000000 feno-0.0.6/src/feno/cases.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     1699 2024-04-01 17:39:49.000000 feno-0.0.6/src/feno/check.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      938 2024-03-26 19:19:40.000000 feno-0.0.6/src/feno/css_style.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     3821 2024-03-27 17:09:25.000000 feno-0.0.6/src/feno/filter.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     6915 2024-04-02 01:52:43.000000 feno-0.0.6/src/feno/html.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     2494 2024-03-27 13:44:12.000000 feno-0.0.6/src/feno/indexer.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     3326 2024-03-27 13:09:44.000000 feno-0.0.6/src/feno/jsontools.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      393 2024-04-01 23:10:29.000000 feno-0.0.6/src/feno/log.py
+-rw-r--r--   0 lion      (1000) lion      (1000)    10327 2024-03-27 17:02:47.000000 feno-0.0.6/src/feno/mdpp.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     4989 2024-04-01 23:31:38.000000 feno-0.0.6/src/feno/remote_md.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     1559 2024-04-02 00:04:11.000000 feno-0.0.6/src/feno/tree.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-02 01:52:54.536522 feno-0.0.6/src/feno.egg-info/
+-rw-r--r--   0 lion      (1000) lion      (1000)      918 2024-04-02 01:52:54.000000 feno-0.0.6/src/feno.egg-info/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)      542 2024-04-02 01:52:54.000000 feno-0.0.6/src/feno.egg-info/SOURCES.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-04-02 01:52:54.000000 feno-0.0.6/src/feno.egg-info/dependency_links.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)      144 2024-04-02 01:52:54.000000 feno-0.0.6/src/feno.egg-info/entry_points.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       55 2024-04-02 01:52:54.000000 feno-0.0.6/src/feno.egg-info/requires.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        5 2024-04-02 01:52:54.000000 feno-0.0.6/src/feno.egg-info/top_level.txt
```

### Comparing `feno-0.0.5/LICENSE` & `feno-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `feno-0.0.5/PKG-INFO` & `feno-0.0.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feno
-Version: 0.0.5
+Version: 0.0.6
 Summary: feno: Flexible Exercise Notation Organizer
 Home-page: https://github.com/senapk/feno
 Author: David Sena Oliveira
 Author-email: sena@ufc.br
 Project-URL: Bug Reports, https://github.com/senapk/feno/issues
 Project-URL: Source, https://github.com/senapk/feno/
 Keywords: programming,learning
```

### Comparing `feno-0.0.5/setup.py` & `feno-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,13 +48,13 @@
     # dependencies). Users will be able to install these using the "extras"
     # syntax, for example: $ pip install sampleproject[dev]
     # Similar to `install_requires` above, these must be valid existing projects
     extras_require={'dev': ['check-manifest'],
                     'test': ['coverage'],
                     },  # Optional
 
-    entry_points={'console_scripts': ['feno=feno.__main__:main', 'mdpp=feno.mdpp:main', 'filter=feno.filter:main', 'indexer=feno.indexer:main'], },
+    entry_points={'console_scripts': ['feno=feno.__main__:main', 'mdpp=feno.mdpp:main', 'filter=feno.filter:main', 'indexer=feno.indexer:main', 'check=feno.check:main'], },
 
     project_urls={'Bug Reports': 'https://github.com/senapk/feno/issues',
                   'Source': 'https://github.com/senapk/feno/',
                   },  # Optional https://packaging.python.org/specifications/core-metadata/#project-url-multiple-use
 )
```

### Comparing `feno-0.0.5/src/feno/__main__.py` & `feno-0.0.6/src/feno/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,64 +1,60 @@
-from __future__ import annotations
-
 import argparse
 import sys
-
+import os
 
 from .actions import Actions
 from .__init__ import __version__
 from .log import Log
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument('targets', metavar='T', type=str, nargs='*', help='Readmes or folders')
     parser.add_argument("--check", "-c", action="store_true", help="Check if the file needs to be rebuilt")
     parser.add_argument("--preamble", "-p", action="store_true", help="disable qxcode preamble")
-    parser.add_argument("--version", "-v", action="store_true", help="Prints the version")
-    parser.add_argument("--debug", "-d", action="store_true", help="Verbose mode")
+    parser.add_argument("--version", action="store_true", help="Prints the version")
+    parser.add_argument("--verbose", "-v", action="store_true", help="Verbose mode")
     parser.add_argument("--keep", "-k", action="store_true", help="Keep the cache files")
     parser.add_argument("--remote", "-r", type=str, help="remote config file")
     
     args = parser.parse_args()
-    Log.verbose = args.debug
+    Log.set_verbose(args.verbose)
     
     if args.version:
         print(__version__)
         sys.exit(0)
 
     if len(args.targets) == 0:
-        print("No targets specified")
+        print("fail: No targets specified")
         exit(1)
 
     for target in args.targets:
+        hook = os.path.basename(os.path.abspath(target))
+
         actions = Actions(target, args.remote)
-        
+        Log.resume(hook, end=": [ ")
+        Log.verbose(hook)
+
         if not actions.validate():
             continue
+
         actions.load_title()
         actions.create_cache()
         actions.update_markdown()
 
-        if args.check and not actions.check_rebuild():
-            return
-
-        Log.write(actions.hook, ": Changes found [ ")
-        actions.recreate_cache() # erase .cache
-        actions.remote_md(args.preamble)         
-        actions.html()
-        actions.build_cases()
-        actions.copy_drafts()
-        actions.run_local_sh()
-        actions.init_vpl()
-        actions.create_mapi()
-        Log.write("\n")
-        if not args.keep:
-            actions.clean()
-        else:
-            print("html: ", actions.target_html)
-            print("cases: ", actions.cases)
+        if not args.check or actions.need_rebuild():
+            actions.recreate_cache() # erase .cache
+            actions.remote_md(args.preamble)
+            actions.html()
+            actions.build_cases()
+            actions.copy_drafts()
+            actions.run_local_sh()
+            actions.init_vpl()
+            actions.create_mapi()
+            actions.clean(args.keep)
 
+        Log.resume("]")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `feno-0.0.5/src/feno/actions.py` & `feno-0.0.6/src/feno/actions.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,33 +17,32 @@
 
 class Actions:
     def __init__(self, source_dir, remote_config: Optional[str]=None):
         self.cache = norm_join(source_dir, ".cache")
         self.target = norm_join(self.cache, "mapi.json")
         self.source_dir = source_dir
         self.hook = os.path.basename(os.path.abspath(source_dir))
-        Log.debug("hook", self.hook)
         self.source_readme = norm_join(self.source_dir, "Readme.md")
         self.remote_readme = norm_join(self.cache, "Readme.md")
         self.target_html = norm_join(self.cache, "q.html")
         self.title = ""
         self.cases = norm_join(self.cache, "q.tio")
         self.config_json = norm_join(self.source_dir, "config.json")
         self.mapi_json = norm_join(self.cache, "mapi.json")
         self.draft_tree = {}
         self.cache_src = norm_join(self.cache, "lang")
         self.vpl = None
         self.remote_config: Optional[str] = remote_config
 
     def validate(self):
         if not os.path.isdir(self.source_dir):
-            print(f"fail: {self.source_dir} is not a directory")
+            print(f"\n    fail: {self.source_dir} is not a directory")
             return False
         if not os.path.isfile(self.source_readme):
-            print(f"fail: {self.source_readme} not found")
+            print(f"\n    fail: {self.source_readme} not found")
             return False
         return True
 
     def load_title(self):
         self.title = Title.extract_title(self.source_readme)
 
     def create_cache(self):
@@ -52,69 +51,84 @@
         return self
     
     def recreate_cache(self):
         shutil.rmtree(self.cache)
         os.makedirs(self.cache)
         return self
     
-    def check_rebuild(self):
-        [_path, changes_found] = Check.check_rebuild(self.source_dir, self.target)
-        return changes_found
+    def need_rebuild(self):
+        if Check.need_rebuild(self.source_dir, self.target):
+            Log.resume("Changes ", end="")
+            return True
+            
+        Log.verbose(f"    no changes in {self.source_dir}")
+        return False
     
     def remote_md(self, disable_preamble=False):
         cfg = RemoteCfg()
         if self.remote_config is not None:
             cfg.read(self.remote_config)
         else:
             cfg_path = RemoteCfg.search_cfg_path(self.source_dir)
             if cfg_path is None:
-                print("fail: no remote.cfg found in the parent folders")
-                exit()
-            cfg.read(cfg_path)
+                print("\n    fail: no remote.cfg found in the parent folders")
+                print("\n    fail: proceeding without make absolute links")
+            else:
+                Log.verbose(f"    remote.cfg: {cfg_path}")
+                cfg.read(cfg_path)
         RemoteMd.run(cfg, self.source_readme, self.remote_readme, self.hook, disable_preamble)
-        Log.write("RemoteMd ")
+        Log.resume("AbsoluteMd ", end="")
     
     # uses pandoc to generate html from markdown
     def html(self):
         title = Title.extract_title(self.source_readme)
-        HTML.generate_html(title, self.remote_readme, self.target_html, True)
-        Log.write("HTML ")
+        HTML.generate_html_with_pandoc(title, self.remote_readme, self.target_html, True)
+        Log.resume("HTML ", end="")
+        Log.verbose(f"    HTML  file: {self.target_html}")
 
     # uses tko to generate cases file
     def build_cases(self):
         Cases.run(self.cases, self.source_readme, self.source_dir)
-        Log.write("Cases ")
+        Log.resume("Cases ", end="")
+        Log.verbose(f"    Cases file: {self.cases}")
 
     def copy_drafts(self):
         source_src = norm_join(self.source_dir, "src")
         if os.path.isdir(source_src):
+            Log.resume("Drafts ", end="")
+            Log.verbose(f"    Drafts dir: {source_src}")
             Tree.deep_filter_copy(source_src, self.cache_src, self.draft_tree, 5)
-            Log.debug("Drafts ", self.draft_tree)
 
     def run_local_sh(self):
         local_sh = norm_join(self.source_dir, "local.sh")
         actual_chdir = os.getcwd()
         if os.path.isfile(local_sh):
             os.chdir(self.source_dir)
             subprocess.run("bash local.sh", shell=True)
             os.chdir(actual_chdir)
+            Log.resume("Local.sh ", end="")
+            Log.verbose(f"    local.sh executed")
 
     def init_vpl(self):
         self.vpl = JsonVPL(self.title, open(self.target_html).read())
         self.vpl.set_cases(self.cases)
         if self.vpl.load_config_json(self.config_json, self.source_dir):
-            Log.write("Required ")
+            Log.resume("Required ", end="")
+            Log.verbose(f"    Config mapi file: {self.config_json}")
         if self.vpl.load_draft_tree(self.draft_tree, self.cache_src):
-            Log.write("Drafts ")
-        Log.write("] ")
+            Log.resume("Drafts ", end="")
 
     def create_mapi(self):
         open(self.mapi_json, "w").write(str(self.vpl) + "\n")
-        Log.write("DONE")
+        Log.resume("Mapi ", end="")
+        Log.verbose(f"    Mapi  file: {self.mapi_json}")
 
-    def clean(self):
-        os.remove(self.cases)
-        os.remove(self.target_html)
+    def clean(self, keep: bool):
+        if not keep:
+            Log.resume("Cleaning ", end="")
+            Log.verbose("    Cleaning  : html and cases files")
+            os.remove(self.cases)
+            os.remove(self.target_html)
 
     # run mdpp script on source readme
     def update_markdown(self):
         Mdpp.update_file(self.source_readme)
```

### Comparing `feno-0.0.5/src/feno/cases.py` & `feno-0.0.6/src/feno/cases.py`

 * *Files identical despite different names*

### Comparing `feno-0.0.5/src/feno/check.py` & `feno-0.0.6/src/feno/check.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Tuple
 import os
 import glob
 from os.path import getmtime
+import argparse
 
 
 class Check:
     # return the last update for the most recent file in the directory
     @staticmethod
     def last_update(path) -> Tuple[str, float]:
         value = 0
@@ -22,16 +23,29 @@
                 juntos = [(f, getmtime(f)) for f in file_list]
                 value = max(juntos, key=lambda x: x[1])
         # print (value)
         return value
 
     # retorna se tem atualização e o arquivo mais recente
     @staticmethod
-    def check_rebuild(source: str, target: str) -> Tuple[str, bool]:
+    def need_rebuild(source: str, target: str) -> Tuple[str, bool]:
         if not os.path.exists(target):
             return [source, True]
-        [source_path, source_time] = Check.last_update(source)
-        [target_path, target_time] = Check.last_update(target)
+        [_source_path, source_time] = Check.last_update(source)
+        [_target_path, target_time] = Check.last_update(target)
         # source tem novas alterações
-        return (source_path, source_time > target_time)
+        return source_time > target_time
 
 
+def main():
+    parser = argparse.ArgumentParser(description='Check if the source has changed')
+    parser.add_argument('source', type=str, help='Source directory')
+    parser.add_argument('target', type=str, help='Target file')
+
+    args = parser.parse_args()
+
+    need = Check.need_rebuild(args.source, args.target)
+    print("Precisa Rebuild" if need else "Não precisa Rebuild")
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `feno-0.0.5/src/feno/css_style.py` & `feno-0.0.6/src/feno/css_style.py`

 * *Files identical despite different names*

### Comparing `feno-0.0.5/src/feno/filter.py` & `feno-0.0.6/src/feno/filter.py`

 * *Files identical despite different names*

### Comparing `feno-0.0.5/src/feno/indexer.py` & `feno-0.0.6/src/feno/indexer.py`

 * *Files identical despite different names*

### Comparing `feno-0.0.5/src/feno/jsontools.py` & `feno-0.0.6/src/feno/jsontools.py`

 * *Files identical despite different names*

### Comparing `feno-0.0.5/src/feno/mdpp.py` & `feno-0.0.6/src/feno/mdpp.py`

 * *Files identical despite different names*

### Comparing `feno-0.0.5/src/feno/remote_md.py` & `feno-0.0.6/src/feno/remote_md.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,37 +16,39 @@
         return title
 
 class RemoteCfg:
     def __init__(self):
         self.user = ""
         self.repo = ""
         self.base = ""
+        self.branch = "master"
 
     def read(self, cfg_path: str):
         if not os.path.isfile(cfg_path):
             print("no remote.cfg found")
 
         config = configparser.ConfigParser()
         config.read(cfg_path)
 
         self.user = config["DEFAULT"]["user"]
         self.repo = config["DEFAULT"]["rep"]
         self.base = config["DEFAULT"]["base"]
+        if "branch" in config["DEFAULT"]:
+            self.branch = config["DEFAULT"]["branch"]
 
     @staticmethod
     def search_cfg_path(source_dir) -> Optional[str]:
         # look for the remote.cfg file in the current folder
         # if not found, look for it in the parent folder
         # if not found, look for it in the parent's parent folder ...
 
         path = os.path.abspath(source_dir)
         while path != "/":
             cfg_path = os.path.join(path, "remote.cfg")
             if os.path.isfile(cfg_path):
-                Log.debug("remote.cfg found at: ", cfg_path)
                 return cfg_path
             path = os.path.dirname(path)
         
         return None
 
 class Absolute:
 
@@ -77,17 +79,17 @@
 
         return result
 
     @staticmethod
     def relative_to_absolute(content: str, cfg: RemoteCfg, hook):
         base_hook = os.path.join(cfg.base, hook)
         user_repo = os.path.join(cfg.user, cfg.repo)
-        remote_raw    = os.path.join("https://raw.githubusercontent.com", user_repo, "master" , base_hook)
-        remote_view    = os.path.join("https://github.com/", user_repo, "blob/master", base_hook)
-        remote_folder = os.path.join("https://github.com/", user_repo, "tree/master", base_hook)
+        remote_raw    = os.path.join("https://raw.githubusercontent.com", user_repo, cfg.branch , base_hook)
+        remote_view    = os.path.join("https://github.com/", user_repo, "blob", cfg.branch, base_hook)
+        remote_folder = os.path.join("https://github.com/", user_repo, "tree", cfg.branch, base_hook)
         return Absolute.__replace_remote(content, remote_raw, remote_view, remote_folder)
 
     @staticmethod
     def from_file(source_file, output_file, cfg: RemoteCfg, hook):
         content = open(source_file).read()
         content = Absolute.relative_to_absolute(content, cfg, hook)
         open(output_file, "w").write(content)
@@ -108,25 +110,26 @@
         return lines
 
     @staticmethod
     def insert_qxcode_preamble(cfg: RemoteCfg, content: str, hook) -> str:
         base_hook = os.path.join(cfg.base, hook)
 
         lines = content.split("\n")
-        online_readme_link = os.path.join("https://github.com", cfg.user, cfg.repo, "blob/master", base_hook, "Readme.md")
+        online_readme_link = os.path.join("https://github.com", cfg.user, cfg.repo, "blob", cfg.branch, base_hook, "Readme.md")
         tkodown = "tko down " + cfg.user[6:] + " " + hook
         lines = RemoteMd.insert_preamble(lines, online_readme_link, tkodown)
         return "\n".join(lines)
 
     @staticmethod
     def run(remote_cfg: RemoteCfg, source: str, target: str, hook, disable_preamble: bool) -> bool:    
         content = open(source).read()
-        if not disable_preamble:
-            content = RemoteMd.insert_qxcode_preamble(remote_cfg, content, hook)
-        content = Absolute.relative_to_absolute(content, remote_cfg, hook)
+        if remote_cfg is not None:
+            if not disable_preamble:
+                content = RemoteMd.insert_qxcode_preamble(remote_cfg, content, hook)
+            content = Absolute.relative_to_absolute(content, remote_cfg, hook)
         open(target, "w").write(content)
 
 if __name__ == "__main__":
     remote_cfg = RemoteCfg()
     remote_cfg.read(RemoteCfg.get_default_cfg_path())
     hook = os.path.basename(os.path.abspath("."))
     RemoteMd.run(remote_cfg, "Readme.md", ".cache/Readme.md")
```

### Comparing `feno-0.0.5/src/feno/tree.py` & `feno-0.0.6/src/feno/tree.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,13 +28,13 @@
 
             if not any([filename.endswith(ext) for ext in text_extensions]):
                 return
             content = open(source, "r").read()
             processed = Filter(filename).process(content)
             with open(destiny, "w") as f:
                 if processed != content:
-                    Log.debug("(filtered): ", end="")
+                    Log.verbose("         draft: ", end="")
                 else:
-                    Log.debug("(        ): ", end="")
+                    Log.verbose("         =====: ", end="")
                 f.write(processed)
-                Log.debug(destiny)
+                Log.verbose(destiny)
```

### Comparing `feno-0.0.5/src/feno.egg-info/PKG-INFO` & `feno-0.0.6/src/feno.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feno
-Version: 0.0.5
+Version: 0.0.6
 Summary: feno: Flexible Exercise Notation Organizer
 Home-page: https://github.com/senapk/feno
 Author: David Sena Oliveira
 Author-email: sena@ufc.br
 Project-URL: Bug Reports, https://github.com/senapk/feno/issues
 Project-URL: Source, https://github.com/senapk/feno/
 Keywords: programming,learning
```

### Comparing `feno-0.0.5/src/feno.egg-info/SOURCES.txt` & `feno-0.0.6/src/feno.egg-info/SOURCES.txt`

 * *Files identical despite different names*

