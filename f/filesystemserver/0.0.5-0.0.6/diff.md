# Comparing `tmp/filesystemserver-0.0.5-py3-none-any.whl.zip` & `tmp/filesystemserver-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 12020 bytes, number of entries: 12
+Zip file size: 12083 bytes, number of entries: 12
 -rw-r--r--  2.0 unx       82 b- defN 20-Feb-02 00:00 filesystemserver/__init__.py
--rw-r--r--  2.0 unx    11673 b- defN 20-Feb-02 00:00 filesystemserver/filesystemserver.py
+-rw-r--r--  2.0 unx    11882 b- defN 20-Feb-02 00:00 filesystemserver/filesystemserver.py
 -rw-r--r--  2.0 unx     2941 b- defN 20-Feb-02 00:00 filesystemserver/data/plugin/fss/favicon.png
 -rw-r--r--  2.0 unx     1542 b- defN 20-Feb-02 00:00 filesystemserver/data/plugin/fss/fss.js
 -rw-r--r--  2.0 unx     1811 b- defN 20-Feb-02 00:00 filesystemserver/data/plugin/fss/browser/app.js
 -rw-r--r--  2.0 unx      353 b- defN 20-Feb-02 00:00 filesystemserver/data/plugin/fss/browser/index.html
 -rw-r--r--  2.0 unx      472 b- defN 20-Feb-02 00:00 filesystemserver/data/plugin/fss/browser/style.css
-?rw-r--r--  2.0 unx     2757 b- defN 20-Feb-02 00:00 filesystemserver-0.0.5.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 filesystemserver-0.0.5.dist-info/WHEEL
-?rw-r--r--  2.0 unx       46 b- defN 20-Feb-02 00:00 filesystemserver-0.0.5.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1058 b- defN 20-Feb-02 00:00 filesystemserver-0.0.5.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     1134 b- defN 20-Feb-02 00:00 filesystemserver-0.0.5.dist-info/RECORD
-12 files, 23956 bytes uncompressed, 10064 bytes compressed:  58.0%
+?rw-r--r--  2.0 unx     2757 b- defN 20-Feb-02 00:00 filesystemserver-0.0.6.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 filesystemserver-0.0.6.dist-info/WHEEL
+?rw-r--r--  2.0 unx       46 b- defN 20-Feb-02 00:00 filesystemserver-0.0.6.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1058 b- defN 20-Feb-02 00:00 filesystemserver-0.0.6.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1134 b- defN 20-Feb-02 00:00 filesystemserver-0.0.6.dist-info/RECORD
+12 files, 24165 bytes uncompressed, 10127 bytes compressed:  58.1%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: filesystemserver/data/plugin/fss/browser/index.html
 Comment: 
 
 Filename: filesystemserver/data/plugin/fss/browser/style.css
 Comment: 
 
-Filename: filesystemserver-0.0.5.dist-info/METADATA
+Filename: filesystemserver-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: filesystemserver-0.0.5.dist-info/WHEEL
+Filename: filesystemserver-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: filesystemserver-0.0.5.dist-info/entry_points.txt
+Filename: filesystemserver-0.0.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: filesystemserver-0.0.5.dist-info/licenses/LICENSE
+Filename: filesystemserver-0.0.6.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: filesystemserver-0.0.5.dist-info/RECORD
+Filename: filesystemserver-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## filesystemserver/__init__.py

```diff
@@ -1,3 +1,3 @@
 from .filesystemserver import install, update, serve, main
 
-__version__ = "0.0.5"
+__version__ = "0.0.6"
```

## filesystemserver/filesystemserver.py

```diff
@@ -16,22 +16,22 @@
     sys.version_info.minor,
 ) < (3, 11):
     import tomli as toml
 else:
     import tomllib as toml
 
 
-def resolve_git_repo(url):
+def resolve_git_repo(url, ssh=False):
     if (
         not url.startswith("http")
         and not url.startswith("ssh")
         and not url.startswith("git@")
     ):
-        url = f"https://github.com/{url}"
-    plugin_dir = "/".join(url.split("/")[-2:])
+        url = f"git@github.com:{url}.git" if ssh else f"https://github.com/{url}"
+    plugin_dir = "/".join(url.split(":")[-1].split("/")[-2:]).strip(".git")
     return url, plugin_dir
 
 
 def installed_plugins(plugin_dir):
     index = "index.html"
     prefix_len = len(plugin_dir) + 1
     postfix_len = len(index) + 1
@@ -60,15 +60,15 @@
         sys.exit(1)
     except subprocess.CalledProcessError:
         print(f"Error: {help_message}", file=sys.stderr)
         sys.exit(1)
 
 
 def install(args):
-    repo, plugin_dir = resolve_git_repo(args.plugin)
+    repo, plugin_dir = resolve_git_repo(args.plugin, ssh=args.ssh)
     git(
         "clone",
         repo,
         plugin_dir,
         cwd=args.plugin_dir,
         help_message="Perhaps the plugin specified is already installed, did you mean to run `update`?",
     )
@@ -310,14 +310,19 @@
         aliases=["i"],
         help="""install a plugin
     - either github project path `nicholashaydensmith/gallery.fss`
     - or full git URL `https://github.com/nicholashaydensmith/gallery.fss.git`""",
     )
     install_parser.set_defaults(func=install)
     install_parser.add_argument(
+        "--ssh",
+        action="store_true",
+        help="Clone via ssh",
+    )
+    install_parser.add_argument(
         "plugin",
         help="plugin to install",
     )
 
     update_parser = subparsers.add_parser(
         "update", aliases=["u"], help="update installed plugins"
     )
```

## Comparing `filesystemserver-0.0.5.dist-info/METADATA` & `filesystemserver-0.0.6.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: filesystemserver
-Version: 0.0.5
+Version: 0.0.6
 Summary: File System Server
 Project-URL: Homepage, https://github.com/nicholashaydensmith/filesystemserver
 Project-URL: Issues, https://github.com/nicholashaydensmith/filesystemserver/issues
 Author-email: Nicholas Smith <thesmithdynasty@gmail.com>
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `filesystemserver-0.0.5.dist-info/licenses/LICENSE` & `filesystemserver-0.0.6.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `filesystemserver-0.0.5.dist-info/RECORD` & `filesystemserver-0.0.6.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-filesystemserver/__init__.py,sha256=stMXE3Lde2NzKNP0-S8A7l4BaloJdTITQNL8tmCEi0w,82
-filesystemserver/filesystemserver.py,sha256=dsWeHS-arPfijOreWyiIYl0B0fm3rrXMxY3oRyFN4aM,11673
+filesystemserver/__init__.py,sha256=Id3ThB5yiSJ_RRz3aRIg8vZpvNl7Ab3pf-Md8XReVBw,82
+filesystemserver/filesystemserver.py,sha256=bptP3_d-_7owQ_4W0N1X2FS1bHTiCUrs4pYERTY63H0,11882
 filesystemserver/data/plugin/fss/favicon.png,sha256=jfu_rDdgAb0ulGnX9TxdM1vj4f0ZpRkEE0DpB1I4cNM,2941
 filesystemserver/data/plugin/fss/fss.js,sha256=gHeQgbKESwUWWLXUpke2xmOY89QR5waOCtkSKV-8L2U,1542
 filesystemserver/data/plugin/fss/browser/app.js,sha256=DtxRIt8wm_RskX-LZWQJiroBUK7AIXqIy34EVaHUtvA,1811
 filesystemserver/data/plugin/fss/browser/index.html,sha256=aU5EcD4xZ_UrEWLXPmHMYDe86Tyu7V7B6vB0qjJ8sdY,353
 filesystemserver/data/plugin/fss/browser/style.css,sha256=8VNeUDCQV5APkjShPTa3vAWKAu-uPkoTXxvWygh_D70,472
-filesystemserver-0.0.5.dist-info/METADATA,sha256=9bCFuJL40Hp34U9l2M7FQrbr9uVesxRqn5G-m6v02CM,2757
-filesystemserver-0.0.5.dist-info/WHEEL,sha256=uNdcs2TADwSd5pVaP0Z_kcjcvvTUklh2S7bxZMF8Uj0,87
-filesystemserver-0.0.5.dist-info/entry_points.txt,sha256=v8bckKCYnwAeArNNyRB1mYpv_LCSZHDKQDWPypN0tf8,46
-filesystemserver-0.0.5.dist-info/licenses/LICENSE,sha256=Ks3vDJNeEsRGdqidSQvxrke32irrL4Xez7qVE4DBEik,1058
-filesystemserver-0.0.5.dist-info/RECORD,,
+filesystemserver-0.0.6.dist-info/METADATA,sha256=XX-JVNrAEx05OvkA6eEBm98rlCjFP2kl6yNipyL6Bvc,2757
+filesystemserver-0.0.6.dist-info/WHEEL,sha256=uNdcs2TADwSd5pVaP0Z_kcjcvvTUklh2S7bxZMF8Uj0,87
+filesystemserver-0.0.6.dist-info/entry_points.txt,sha256=v8bckKCYnwAeArNNyRB1mYpv_LCSZHDKQDWPypN0tf8,46
+filesystemserver-0.0.6.dist-info/licenses/LICENSE,sha256=Ks3vDJNeEsRGdqidSQvxrke32irrL4Xez7qVE4DBEik,1058
+filesystemserver-0.0.6.dist-info/RECORD,,
```

