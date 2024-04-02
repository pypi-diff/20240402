# Comparing `tmp/fontquery-1.8.tar.gz` & `tmp/fontquery-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fontquery-1.8.tar", last modified: Thu Feb  1 09:33:47 2024, max compression
+gzip compressed data, was "fontquery-1.9.tar", last modified: Mon Mar 11 07:14:40 2024, max compression
```

## Comparing `fontquery-1.8.tar` & `fontquery-1.9.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 tagoh     (1000) tagoh     (1000)        0 2024-02-01 09:33:47.989669 fontquery-1.8/
--rw-r--r--   0 tagoh     (1000) tagoh     (1000)     1070 2023-05-16 06:35:25.000000 fontquery-1.8/LICENSE
--rw-r--r--   0 tagoh     (1000) tagoh     (1000)     4289 2024-02-01 09:33:47.989669 fontquery-1.8/PKG-INFO
--rw-r--r--   0 tagoh     (1000) tagoh     (1000)     2339 2024-02-01 06:57:57.000000 fontquery-1.8/README.md
-drwxr-xr-x   0 tagoh     (1000) tagoh     (1000)        0 2024-02-01 09:33:47.988669 fontquery-1.8/fontquery/
--rw-r--r--   0 tagoh     (1000) tagoh     (1000)     1084 2023-05-23 05:52:52.000000 fontquery-1.8/fontquery/__init__.py
--rw-r--r--   0 tagoh     (1000) tagoh     (1000)    10807 2024-02-01 06:41:44.000000 fontquery-1.8/fontquery/build.py
--rw-r--r--   0 tagoh     (1000) tagoh     (1000)     1975 2024-01-31 08:56:46.000000 fontquery-1.8/fontquery/cache.py
--rw-r--r--   0 tagoh     (1000) tagoh     (1000)     6235 2024-02-01 06:42:59.000000 fontquery-1.8/fontquery/client.py
--rw-r--r--   0 tagoh     (1000) tagoh     (1000)     9372 2024-02-01 06:45:03.000000 fontquery-1.8/fontquery/container.py
-drwxr-xr-x   0 tagoh     (1000) tagoh     (1000)        0 2024-02-01 09:33:47.988669 fontquery-1.8/fontquery/data/
--rw-r--r--   0 tagoh     (1000) tagoh     (1000)     1818 2023-11-21 09:22:09.000000 fontquery-1.8/fontquery/data/Containerfile
--rw-r--r--   0 tagoh     (1000) tagoh     (1000)     6600 2024-02-01 06:59:04.000000 fontquery-1.8/fontquery/diff.py
--rw-r--r--   0 tagoh     (1000) tagoh     (1000)    23967 2024-02-01 06:46:27.000000 fontquery-1.8/fontquery/htmlformatter.py
-drwxr-xr-x   0 tagoh     (1000) tagoh     (1000)        0 2024-02-01 09:33:47.988669 fontquery-1.8/fontquery/scripts/
--rwxr-xr-x   0 tagoh     (1000) tagoh     (1000)     3798 2023-11-22 07:47:24.000000 fontquery-1.8/fontquery/scripts/fontquery-setup.sh
--rw-r--r--   0 tagoh     (1000) tagoh     (1000)     1350 2023-10-31 13:55:21.000000 fontquery-1.8/fontquery/version.py
--rw-r--r--   0 tagoh     (1000) tagoh     (1000)       15 2023-11-30 08:47:59.000000 fontquery-1.8/fontquery/version.txt
-drwxr-xr-x   0 tagoh     (1000) tagoh     (1000)        0 2024-02-01 09:33:47.988669 fontquery-1.8/fontquery.egg-info/
--rw-r--r--   0 tagoh     (1000) tagoh     (1000)     4289 2024-02-01 09:33:47.000000 fontquery-1.8/fontquery.egg-info/PKG-INFO
--rw-r--r--   0 tagoh     (1000) tagoh     (1000)      489 2024-02-01 09:33:47.000000 fontquery-1.8/fontquery.egg-info/SOURCES.txt
--rw-r--r--   0 tagoh     (1000) tagoh     (1000)        1 2024-02-01 09:33:47.000000 fontquery-1.8/fontquery.egg-info/dependency_links.txt
--rw-r--r--   0 tagoh     (1000) tagoh     (1000)      214 2024-02-01 09:33:47.000000 fontquery-1.8/fontquery.egg-info/entry_points.txt
--rw-r--r--   0 tagoh     (1000) tagoh     (1000)       35 2024-02-01 09:33:47.000000 fontquery-1.8/fontquery.egg-info/requires.txt
--rw-r--r--   0 tagoh     (1000) tagoh     (1000)       45 2024-02-01 09:33:47.000000 fontquery-1.8/fontquery.egg-info/top_level.txt
--rw-r--r--   0 tagoh     (1000) tagoh     (1000)     1267 2024-02-01 09:33:09.000000 fontquery-1.8/pyproject.toml
--rw-r--r--   0 tagoh     (1000) tagoh     (1000)       38 2024-02-01 09:33:47.989669 fontquery-1.8/setup.cfg
+drwxr-xr-x   0 tagoh     (1000) tagoh     (1000)        0 2024-03-11 07:14:40.452620 fontquery-1.9/
+-rw-r--r--   0 tagoh     (1000) tagoh     (1000)     1070 2023-05-16 06:35:25.000000 fontquery-1.9/LICENSE
+-rw-r--r--   0 tagoh     (1000) tagoh     (1000)     4476 2024-03-11 07:14:40.452620 fontquery-1.9/PKG-INFO
+-rw-r--r--   0 tagoh     (1000) tagoh     (1000)     2526 2024-02-01 09:37:36.000000 fontquery-1.9/README.md
+drwxr-xr-x   0 tagoh     (1000) tagoh     (1000)        0 2024-03-11 07:14:40.451620 fontquery-1.9/fontquery/
+-rw-r--r--   0 tagoh     (1000) tagoh     (1000)     1084 2023-05-23 05:52:52.000000 fontquery-1.9/fontquery/__init__.py
+-rw-r--r--   0 tagoh     (1000) tagoh     (1000)    10807 2024-02-01 06:41:44.000000 fontquery-1.9/fontquery/build.py
+-rw-r--r--   0 tagoh     (1000) tagoh     (1000)     2164 2024-02-02 09:55:54.000000 fontquery-1.9/fontquery/cache.py
+-rw-r--r--   0 tagoh     (1000) tagoh     (1000)     6447 2024-03-11 07:10:58.000000 fontquery-1.9/fontquery/client.py
+-rw-r--r--   0 tagoh     (1000) tagoh     (1000)     9372 2024-02-01 06:45:03.000000 fontquery-1.9/fontquery/container.py
+drwxr-xr-x   0 tagoh     (1000) tagoh     (1000)        0 2024-03-11 07:14:40.451620 fontquery-1.9/fontquery/data/
+-rw-r--r--   0 tagoh     (1000) tagoh     (1000)     1818 2023-11-21 09:22:09.000000 fontquery-1.9/fontquery/data/Containerfile
+-rw-r--r--   0 tagoh     (1000) tagoh     (1000)     7028 2024-03-11 06:46:52.000000 fontquery-1.9/fontquery/diff.py
+drwxr-xr-x   0 tagoh     (1000) tagoh     (1000)        0 2024-03-11 07:14:40.451620 fontquery-1.9/fontquery/fontquery_debug/
+-rw-r--r--   0 tagoh     (1000) tagoh     (1000)      204 2024-03-11 04:06:03.000000 fontquery-1.9/fontquery/fontquery_debug/__init__.py
+-rw-r--r--   0 tagoh     (1000) tagoh     (1000)    24262 2024-03-11 07:10:58.000000 fontquery-1.9/fontquery/htmlformatter.py
+drwxr-xr-x   0 tagoh     (1000) tagoh     (1000)        0 2024-03-11 07:14:40.451620 fontquery-1.9/fontquery/scripts/
+-rwxr-xr-x   0 tagoh     (1000) tagoh     (1000)     3798 2023-11-22 07:47:24.000000 fontquery-1.9/fontquery/scripts/fontquery-setup.sh
+-rw-r--r--   0 tagoh     (1000) tagoh     (1000)     1350 2023-10-31 13:55:21.000000 fontquery-1.9/fontquery/version.py
+-rw-r--r--   0 tagoh     (1000) tagoh     (1000)       15 2023-11-30 08:47:59.000000 fontquery-1.9/fontquery/version.txt
+drwxr-xr-x   0 tagoh     (1000) tagoh     (1000)        0 2024-03-11 07:14:40.452620 fontquery-1.9/fontquery.egg-info/
+-rw-r--r--   0 tagoh     (1000) tagoh     (1000)     4476 2024-03-11 07:14:40.000000 fontquery-1.9/fontquery.egg-info/PKG-INFO
+-rw-r--r--   0 tagoh     (1000) tagoh     (1000)      527 2024-03-11 07:14:40.000000 fontquery-1.9/fontquery.egg-info/SOURCES.txt
+-rw-r--r--   0 tagoh     (1000) tagoh     (1000)        1 2024-03-11 07:14:40.000000 fontquery-1.9/fontquery.egg-info/dependency_links.txt
+-rw-r--r--   0 tagoh     (1000) tagoh     (1000)      214 2024-03-11 07:14:40.000000 fontquery-1.9/fontquery.egg-info/entry_points.txt
+-rw-r--r--   0 tagoh     (1000) tagoh     (1000)       35 2024-03-11 07:14:40.000000 fontquery-1.9/fontquery.egg-info/requires.txt
+-rw-r--r--   0 tagoh     (1000) tagoh     (1000)       45 2024-03-11 07:14:40.000000 fontquery-1.9/fontquery.egg-info/top_level.txt
+-rw-r--r--   0 tagoh     (1000) tagoh     (1000)     1307 2024-03-11 07:12:10.000000 fontquery-1.9/pyproject.toml
+-rw-r--r--   0 tagoh     (1000) tagoh     (1000)       38 2024-03-11 07:14:40.452620 fontquery-1.9/setup.cfg
```

### Comparing `fontquery-1.8/LICENSE` & `fontquery-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fontquery-1.8/PKG-INFO` & `fontquery-1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fontquery
-Version: 1.8
+Version: 1.9
 Summary: Query a font in Fedora release
 Author-email: Akira TAGOH <akira@tagoh.org>
 License: MIT License
         
         Copyright (c) 2022 Red Hat, Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -50,22 +50,36 @@
 
 ## How to install
 
 ``` shell
 $ pip3 install fontquery
 ```
 
+Or in Fedora,
+
+``` shell
+# dnf install fontquery
+```
+
 ## How to install from git
 
 ``` shell
 $ pip3 install --user build wheel
 $ python3 -m build
 $ pip3 install --user dist/fontquery*.whl
 ```
 
+Or in Fedora,
+
+``` shell
+# dnf install python3-build python3-wheel
+$ python3 -m build
+$ pip3 install --user dist/fontquery*.whl
+```
+
 ## Usage
 
 ```
 usage: fontquery [-h] [-r RELEASE] [-l LANG] [-m {fcmatch,fclist,json}] [-t {comps,langpacks,both,all}] [-v]
                  [args ...]
 
 Query fonts
```

### Comparing `fontquery-1.8/README.md` & `fontquery-1.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -7,22 +7,36 @@
 
 ## How to install
 
 ``` shell
 $ pip3 install fontquery
 ```
 
+Or in Fedora,
+
+``` shell
+# dnf install fontquery
+```
+
 ## How to install from git
 
 ``` shell
 $ pip3 install --user build wheel
 $ python3 -m build
 $ pip3 install --user dist/fontquery*.whl
 ```
 
+Or in Fedora,
+
+``` shell
+# dnf install python3-build python3-wheel
+$ python3 -m build
+$ pip3 install --user dist/fontquery*.whl
+```
+
 ## Usage
 
 ```
 usage: fontquery [-h] [-r RELEASE] [-l LANG] [-m {fcmatch,fclist,json}] [-t {comps,langpacks,both,all}] [-v]
                  [args ...]
 
 Query fonts
```

### Comparing `fontquery-1.8/fontquery/__init__.py` & `fontquery-1.9/fontquery/__init__.py`

 * *Files identical despite different names*

### Comparing `fontquery-1.8/fontquery/build.py` & `fontquery-1.9/fontquery/build.py`

 * *Files identical despite different names*

### Comparing `fontquery-1.8/fontquery/cache.py` & `fontquery-1.9/fontquery/cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,19 @@
         tag = self._get_current_revision()
         return self._cachedir / (tag + '.json')
 
     def _get_current_revision(self) -> str:
         cmdline = [
             'podman', 'images', '-a', '--no-trunc', self._repo
         ]
-        out = subprocess.run(cmdline, stdout=subprocess.PIPE).stdout.decode('utf-8')
+        res = subprocess.run(cmdline, stdout=subprocess.PIPE)
+        if res.returncode != 0:
+            sys.tracebacklimit = 0
+            raise RuntimeError('`podman images\' failed with the error code {}'.format(res.returncode))
+        out = res.stdout.decode('utf-8')
         result = []
         for l in out.splitlines():
             result.append(l.split())
         if len(result) < 2:
             raise RuntimeError('No images available: {}'.format(self._repo))
         tag = result[1][[i for i in range(len(result[0])) if result[0][i] == 'IMAGE'][0]]
         cmdline = [
```

### Comparing `fontquery-1.8/fontquery/client.py` & `fontquery-1.9/fontquery/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,21 @@
              else []) + ([] if args.lang is None else
                          [' '.join(['-l=' + ls
                                     for ls in args.lang])]) + args.args
 
     if args.verbose:
         print('# ' + ' '.join(cmdline), file=sys.stderr)
 
-    return subprocess.run(cmdline, stdout=subprocess.PIPE).stdout.decode('utf-8')
+    result = subprocess.run(cmdline, stdout=subprocess.PIPE)
+    if result.returncode != 0:
+        sys.tracebacklimit = 0
+        raise RuntimeError('`podman run\' failed with the error code {}'.format(result.returncode))
+    print(result.returncode)
+
+    return result.stdout.decode('utf-8')
 
 def load(release, args, fcache):
     out = None
 
     if release == 'local':
         out = run(release, args)
     else:
```

### Comparing `fontquery-1.8/fontquery/container.py` & `fontquery-1.9/fontquery/container.py`

 * *Files identical despite different names*

### Comparing `fontquery-1.8/fontquery/data/Containerfile` & `fontquery-1.9/fontquery/data/Containerfile`

 * *Files identical despite different names*

### Comparing `fontquery-1.8/fontquery/diff.py` & `fontquery-1.9/fontquery/diff.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,15 +62,19 @@
              else []) + ([] if args.lang is None else
                          [' '.join(['-l=' + ls
                                     for ls in args.lang])])
 
     if args.verbose:
         print('# ' + ' '.join(cmdline), file=sys.stderr)
 
-    out = subprocess.run(cmdline, stdout=subprocess.PIPE).stdout.decode('utf-8')
+    result = subprocess.run(cmdline, stdout=subprocess.PIPE)
+    if result.returncode != 0:
+        sys.tracebacklimit = 0
+        raise RuntimeError('`podman run\' failed with the error code {}'.format(result.returncode))
+    out = result.stdout.decode('utf-8')
 
     return out
 
 def load_json(release, args, fcache):
     out = None
 
     if release == 'local':
@@ -112,14 +116,17 @@
     parser.add_argument('--disable-cache',
                         action='store_true',
                         help='Enforce processing everything even if not updating')
     parser.add_argument('-l',
                         '--lang',
                         action='append',
                         help='Language list to dump fonts data into JSON')
+    parser.add_argument('--loose-comparison',
+                        action='store_true',
+                        help='Do not compare results accurately')
     parser.add_argument('-o', '--output',
                         type=argparse.FileType('w'),
                         default='-',
                         help='Output file')
     parser.add_argument('-R', '--render',
                         default='text',
                         choices=renderer.keys())
@@ -161,14 +168,17 @@
 
     retval_a = load_json(args.compare_a, args,
                          not args.disable_cache and not args.lang)
     retval_b = load_json(args.compare_b, args,
                          not args.disable_cache and not args.lang)
 
     with args.output:
-        for s in htmlformatter.generate_diff(renderer[args.render](), '',
-                                             json.loads(retval_a),
-                                             json.loads(retval_b)):
+        g = htmlformatter.generate_diff(renderer[args.render](), '',
+                                        json.loads(retval_a),
+                                        json.loads(retval_b), not args.loose_comparison)
+        for s in next(g):
             args.output.write(s)
+        ret = next(g)
+    sys.exit(0 if ret else 1)
 
 if __name__ == '__main__':
     main()
```

### Comparing `fontquery-1.8/fontquery/htmlformatter.py` & `fontquery-1.9/fontquery/htmlformatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -478,18 +478,20 @@
                     cols.append(ColoredText(data[k][kk]['family'], 'red'))
             for s in TextRenderer.format_line(cols):
                 out.append(s)
 
         yield '\n'.join(out) + '\n'
 
 
-def json2data(data: dict[str, Any]) -> dict[str, dict[str, Any]]:
+def json2data(data: dict[str, Any], ignore_file: bool) -> dict[str, dict[str, Any]]:
     """Restructure JSON format."""
     retval = {}
     for d in data['fonts']:
+        if ignore_file:
+            del d['file']
         key = d['lang_name']
         if key not in retval:
             retval[key] = {}
         alias = d['alias']
         retval[key][alias] = d
 
     return retval
@@ -525,25 +527,25 @@
         retval[key][k] = [v, diffdata[k]]
 
     return retval
 
 
 def generate_table(renderer: DataRenderer, title: str, data: dict[str, Any]) -> Iterator[str]:
     """Format data to HTML."""
-    sorteddata = json2data(data)
+    sorteddata = json2data(data, False)
     renderer.title = title
     renderer.imagetype = data['pattern']
     yield from renderer.render_table(sorteddata)
 
 
 def generate_diff(renderer: DataRenderer, title: str, data: dict[str, Any],
-                  diffdata: dict[str, Any]) -> Iterator[str]:
+                  diffdata: dict[str, Any], compare_accurately: bool) -> Iterator[str]:
     """Format difference between two JSONs to HTML."""
-    sorteddata = json2data(data)
-    sorteddiffdata = json2data(diffdata)
+    sorteddata = json2data(data, not compare_accurately)
+    sorteddiffdata = json2data(diffdata, not compare_accurately)
     matched = {}
     notmatched = {}
     missing_b = {}
     for k in sorted(sorteddata.keys()):
         if k not in sorteddiffdata:
             missing_b[k] = sorteddata[k]
         else:
@@ -558,14 +560,15 @@
     langdiffdata = json2langgroupdiff(notmatched, sorteddiffdata)
 
     renderer.title = title
     renderer.imagetype = data['pattern']
     renderer.imagedifftype = diffdata['pattern']
 
     yield from renderer.render_diff(langdata, missing_a, missing_b, langdiffdata)
+    yield True if not missing_a and not missing_b else False
 
 
 def main():
     """Endpoint to execute fq2html program."""
     fmc = argparse.ArgumentDefaultsHelpFormatter
     parser = argparse.ArgumentParser(description=('HTML formatter '
                                                   'for fontquery'),
@@ -610,13 +613,16 @@
             for s in generate_table(renderer[args.render](), args.title, data):
                 args.output.write(s)
     else:
         with args.diff:
             diffdata = json.load(args.diff)
 
         with args.output:
-            for s in generate_diff(renderer[args.render](), args.title, data, diffdata):
+            g = generate_diff(renderer[args.render](), args.title, data, diffdata)
+            for s in next(g):
                 args.output.write(s)
+            ret = next(g)
+        sys.exit(0 if ret else 1)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `fontquery-1.8/fontquery/scripts/fontquery-setup.sh` & `fontquery-1.9/fontquery/scripts/fontquery-setup.sh`

 * *Files identical despite different names*

### Comparing `fontquery-1.8/fontquery/version.py` & `fontquery-1.9/fontquery/version.py`

 * *Files identical despite different names*

### Comparing `fontquery-1.8/fontquery.egg-info/PKG-INFO` & `fontquery-1.9/fontquery.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fontquery
-Version: 1.8
+Version: 1.9
 Summary: Query a font in Fedora release
 Author-email: Akira TAGOH <akira@tagoh.org>
 License: MIT License
         
         Copyright (c) 2022 Red Hat, Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -50,22 +50,36 @@
 
 ## How to install
 
 ``` shell
 $ pip3 install fontquery
 ```
 
+Or in Fedora,
+
+``` shell
+# dnf install fontquery
+```
+
 ## How to install from git
 
 ``` shell
 $ pip3 install --user build wheel
 $ python3 -m build
 $ pip3 install --user dist/fontquery*.whl
 ```
 
+Or in Fedora,
+
+``` shell
+# dnf install python3-build python3-wheel
+$ python3 -m build
+$ pip3 install --user dist/fontquery*.whl
+```
+
 ## Usage
 
 ```
 usage: fontquery [-h] [-r RELEASE] [-l LANG] [-m {fcmatch,fclist,json}] [-t {comps,langpacks,both,all}] [-v]
                  [args ...]
 
 Query fonts
```

### Comparing `fontquery-1.8/pyproject.toml` & `fontquery-1.9/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fontquery"
-version = "1.8"
+version = "1.9"
 authors = [
   { name = "Akira TAGOH", email="akira@tagoh.org" }
 ]
 description = "Query a font in Fedora release"
 readme = "README.md"
 requires-python = ">= 3.11"
 license.file = "LICENSE"
@@ -37,15 +37,18 @@
 [project.entry-points.console_scripts]
 "fontquery-container" = "fontquery.container:main"
 "fontquery" = "fontquery.client:main"
 "fontquery-build" = "fontquery.build:main"
 "fq2html" = "fontquery.htmlformatter:main"
 "fontquery-diff" = "fontquery.diff:main"
 
+[tool.setuptools]
+include-package-data = false
+
 [tool.setuptools.packages.find]
 namespaces = true
-exclude = [ "fontquery_debug" ]
+exclude = [ "*debug*" ]
 
 [tool.setuptools.package-data]
 fontquery = [ "version.txt" ]
 "fontquery.scripts" = [ "fontquery-setup.sh" ]
 "fontquery.data" = [ "Containerfile*" ]
```

