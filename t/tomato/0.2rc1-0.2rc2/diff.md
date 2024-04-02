# Comparing `tmp/tomato-0.2rc1.tar.gz` & `tmp/tomato-0.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomato-0.2rc1.tar", last modified: Tue Aug 23 06:03:30 2022, max compression
+gzip compressed data, was "tomato-0.2rc2.tar", last modified: Tue Aug 30 08:42:24 2022, max compression
```

## Comparing `tomato-0.2rc1.tar` & `tomato-0.2rc2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2022-08-23 06:03:30.828774 tomato-0.2rc1/
--rw-rw-rw-   0        0        0    35823 2022-02-08 15:13:29.000000 tomato-0.2rc1/LICENSE
--rw-rw-rw-   0        0        0       55 2022-06-13 07:32:21.000000 tomato-0.2rc1/MANIFEST.in
--rw-rw-rw-   0        0        0     1478 2022-08-23 06:03:30.829770 tomato-0.2rc1/PKG-INFO
--rw-rw-rw-   0        0        0      846 2022-08-03 08:27:58.000000 tomato-0.2rc1/README.md
--rw-rw-rw-   0        0        0      217 2022-08-23 06:03:30.841739 tomato-0.2rc1/setup.cfg
--rw-rw-rw-   0        0        0     1672 2022-08-02 12:30:01.000000 tomato-0.2rc1/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-23 06:03:30.558457 tomato-0.2rc1/src/
-drwxrwxrwx   0        0        0        0 2022-08-23 06:03:30.843764 tomato-0.2rc1/src/tomato/
--rw-rw-rw-   0        0        0      181 2022-06-13 07:32:21.000000 tomato-0.2rc1/src/tomato/__init__.py
--rw-rw-rw-   0        0        0      519 2022-08-23 06:03:30.843764 tomato-0.2rc1/src/tomato/_version.py
-drwxrwxrwx   0        0        0        0 2022-08-23 06:03:30.697500 tomato-0.2rc1/src/tomato/daemon/
--rw-rw-rw-   0        0        0       29 2022-06-13 07:32:21.000000 tomato-0.2rc1/src/tomato/daemon/__init__.py
--rw-rw-rw-   0        0        0     5702 2022-08-22 11:41:01.000000 tomato-0.2rc1/src/tomato/daemon/main.py
-drwxrwxrwx   0        0        0        0 2022-08-23 06:03:30.703510 tomato-0.2rc1/src/tomato/dbhandler/
--rw-rw-rw-   0        0        0       23 2022-06-13 07:32:21.000000 tomato-0.2rc1/src/tomato/dbhandler/__init__.py
--rw-rw-rw-   0        0        0     8400 2022-08-22 11:41:01.000000 tomato-0.2rc1/src/tomato/dbhandler/sqlite.py
-drwxrwxrwx   0        0        0        0 2022-08-23 06:03:30.734400 tomato-0.2rc1/src/tomato/drivers/
--rw-rw-rw-   0        0        0      212 2022-08-18 12:19:10.000000 tomato-0.2rc1/src/tomato/drivers/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-23 06:03:30.767936 tomato-0.2rc1/src/tomato/drivers/biologic/
--rw-rw-rw-   0        0        0     6235 2022-08-18 12:19:10.000000 tomato-0.2rc1/src/tomato/drivers/biologic/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-23 06:03:30.803871 tomato-0.2rc1/src/tomato/drivers/biologic/kbio/
--rw-rw-rw-   0        0        0        0 2022-06-13 07:32:21.000000 tomato-0.2rc1/src/tomato/drivers/biologic/kbio/__init__.py
--rw-rw-rw-   0        0        0     4044 2022-06-13 07:32:21.000000 tomato-0.2rc1/src/tomato/drivers/biologic/kbio/c_utils.py
--rw-rw-rw-   0        0        0    33003 2022-08-18 12:19:10.000000 tomato-0.2rc1/src/tomato/drivers/biologic/kbio/kbio_api.py
--rw-rw-rw-   0        0        0     4161 2022-06-13 07:32:21.000000 tomato-0.2rc1/src/tomato/drivers/biologic/kbio/kbio_tech.py
--rw-rw-rw-   0        0        0    18710 2022-06-13 07:32:21.000000 tomato-0.2rc1/src/tomato/drivers/biologic/kbio/kbio_types.py
--rw-rw-rw-   0        0        0     3070 2022-06-13 07:32:21.000000 tomato-0.2rc1/src/tomato/drivers/biologic/kbio/tech_types.py
--rw-rw-rw-   0        0        0     2932 2022-06-13 07:32:21.000000 tomato-0.2rc1/src/tomato/drivers/biologic/kbio/utils.py
--rw-rw-rw-   0        0        0    11072 2022-06-13 07:32:21.000000 tomato-0.2rc1/src/tomato/drivers/biologic/kbio_wrapper.py
--rw-rw-rw-   0        0        0     7381 2022-07-21 06:16:39.000000 tomato-0.2rc1/src/tomato/drivers/biologic/main.py
--rw-rw-rw-   0        0        0     2377 2022-06-13 07:32:21.000000 tomato-0.2rc1/src/tomato/drivers/biologic/tech_params.py
--rw-rw-rw-   0        0        0    10797 2022-08-03 08:27:58.000000 tomato-0.2rc1/src/tomato/drivers/driver_funcs.py
-drwxrwxrwx   0        0        0        0 2022-08-23 06:03:30.811824 tomato-0.2rc1/src/tomato/drivers/dummy/
--rw-rw-rw-   0        0        0     1014 2022-08-18 12:19:10.000000 tomato-0.2rc1/src/tomato/drivers/dummy/__init__.py
--rw-rw-rw-   0        0        0     5104 2022-08-22 10:37:04.000000 tomato-0.2rc1/src/tomato/drivers/dummy/main.py
--rw-rw-rw-   0        0        0      728 2022-06-13 07:32:21.000000 tomato-0.2rc1/src/tomato/drivers/logger_funcs.py
--rw-rw-rw-   0        0        0     1848 2022-08-02 12:30:01.000000 tomato-0.2rc1/src/tomato/drivers/yadg_funcs.py
-drwxrwxrwx   0        0        0        0 2022-08-23 06:03:30.819797 tomato-0.2rc1/src/tomato/ketchup/
--rw-rw-rw-   0        0        0      896 2022-08-16 11:45:00.000000 tomato-0.2rc1/src/tomato/ketchup/__init__.py
--rw-rw-rw-   0        0        0    17279 2022-08-22 10:37:04.000000 tomato-0.2rc1/src/tomato/ketchup/functions.py
--rw-rw-rw-   0        0        0     5903 2022-08-16 11:45:00.000000 tomato-0.2rc1/src/tomato/main.py
-drwxrwxrwx   0        0        0        0 2022-08-23 06:03:30.826779 tomato-0.2rc1/src/tomato/setlib/
--rw-rw-rw-   0        0        0       62 2022-06-13 07:32:21.000000 tomato-0.2rc1/src/tomato/setlib/__init__.py
--rw-rw-rw-   0        0        0     4759 2022-06-13 07:32:21.000000 tomato-0.2rc1/src/tomato/setlib/functions.py
-drwxrwxrwx   0        0        0        0 2022-08-23 06:03:30.683535 tomato-0.2rc1/src/tomato.egg-info/
--rw-rw-rw-   0        0        0     1478 2022-08-23 06:03:30.000000 tomato-0.2rc1/src/tomato.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1260 2022-08-23 06:03:30.000000 tomato-0.2rc1/src/tomato.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-23 06:03:30.000000 tomato-0.2rc1/src/tomato.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2022-08-23 06:03:30.000000 tomato-0.2rc1/src/tomato.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      172 2022-08-23 06:03:30.000000 tomato-0.2rc1/src/tomato.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-08-23 06:03:30.000000 tomato-0.2rc1/src/tomato.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    83320 2022-06-13 07:32:22.000000 tomato-0.2rc1/versioneer.py
+drwxrwxrwx   0        0        0        0 2022-08-30 08:42:24.026369 tomato-0.2rc2/
+-rw-rw-rw-   0        0        0    35823 2022-02-08 15:13:29.000000 tomato-0.2rc2/LICENSE
+-rw-rw-rw-   0        0        0       55 2022-06-13 07:32:21.000000 tomato-0.2rc2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1478 2022-08-30 08:42:24.026369 tomato-0.2rc2/PKG-INFO
+-rw-rw-rw-   0        0        0      846 2022-08-03 08:27:58.000000 tomato-0.2rc2/README.md
+-rw-rw-rw-   0        0        0      217 2022-08-30 08:42:24.029360 tomato-0.2rc2/setup.cfg
+-rw-rw-rw-   0        0        0     1676 2022-08-30 08:21:21.000000 tomato-0.2rc2/setup.py
+drwxrwxrwx   0        0        0        0 2022-08-30 08:42:23.770440 tomato-0.2rc2/src/
+drwxrwxrwx   0        0        0        0 2022-08-30 08:42:24.030357 tomato-0.2rc2/src/tomato/
+-rw-rw-rw-   0        0        0      181 2022-06-13 07:32:21.000000 tomato-0.2rc2/src/tomato/__init__.py
+-rw-rw-rw-   0        0        0      519 2022-08-30 08:42:24.031355 tomato-0.2rc2/src/tomato/_version.py
+drwxrwxrwx   0        0        0        0 2022-08-30 08:42:23.850838 tomato-0.2rc2/src/tomato/daemon/
+-rw-rw-rw-   0        0        0       29 2022-06-13 07:32:21.000000 tomato-0.2rc2/src/tomato/daemon/__init__.py
+-rw-rw-rw-   0        0        0     6095 2022-08-30 08:21:21.000000 tomato-0.2rc2/src/tomato/daemon/main.py
+drwxrwxrwx   0        0        0        0 2022-08-30 08:42:23.855825 tomato-0.2rc2/src/tomato/dbhandler/
+-rw-rw-rw-   0        0        0       23 2022-06-13 07:32:21.000000 tomato-0.2rc2/src/tomato/dbhandler/__init__.py
+-rw-rw-rw-   0        0        0     8400 2022-08-22 11:41:01.000000 tomato-0.2rc2/src/tomato/dbhandler/sqlite.py
+drwxrwxrwx   0        0        0        0 2022-08-30 08:42:23.889735 tomato-0.2rc2/src/tomato/drivers/
+-rw-rw-rw-   0        0        0      212 2022-08-18 12:19:10.000000 tomato-0.2rc2/src/tomato/drivers/__init__.py
+drwxrwxrwx   0        0        0        0 2022-08-30 08:42:23.929628 tomato-0.2rc2/src/tomato/drivers/biologic/
+-rw-rw-rw-   0        0        0     6235 2022-08-18 12:19:10.000000 tomato-0.2rc2/src/tomato/drivers/biologic/__init__.py
+drwxrwxrwx   0        0        0        0 2022-08-30 08:42:23.996448 tomato-0.2rc2/src/tomato/drivers/biologic/kbio/
+-rw-rw-rw-   0        0        0        0 2022-06-13 07:32:21.000000 tomato-0.2rc2/src/tomato/drivers/biologic/kbio/__init__.py
+-rw-rw-rw-   0        0        0     4044 2022-06-13 07:32:21.000000 tomato-0.2rc2/src/tomato/drivers/biologic/kbio/c_utils.py
+-rw-rw-rw-   0        0        0    33003 2022-08-18 12:19:10.000000 tomato-0.2rc2/src/tomato/drivers/biologic/kbio/kbio_api.py
+-rw-rw-rw-   0        0        0     4161 2022-06-13 07:32:21.000000 tomato-0.2rc2/src/tomato/drivers/biologic/kbio/kbio_tech.py
+-rw-rw-rw-   0        0        0    18710 2022-06-13 07:32:21.000000 tomato-0.2rc2/src/tomato/drivers/biologic/kbio/kbio_types.py
+-rw-rw-rw-   0        0        0     3070 2022-06-13 07:32:21.000000 tomato-0.2rc2/src/tomato/drivers/biologic/kbio/tech_types.py
+-rw-rw-rw-   0        0        0     2932 2022-06-13 07:32:21.000000 tomato-0.2rc2/src/tomato/drivers/biologic/kbio/utils.py
+-rw-rw-rw-   0        0        0    11072 2022-06-13 07:32:21.000000 tomato-0.2rc2/src/tomato/drivers/biologic/kbio_wrapper.py
+-rw-rw-rw-   0        0        0     7381 2022-07-21 06:16:39.000000 tomato-0.2rc2/src/tomato/drivers/biologic/main.py
+-rw-rw-rw-   0        0        0     2377 2022-06-13 07:32:21.000000 tomato-0.2rc2/src/tomato/drivers/biologic/tech_params.py
+-rw-rw-rw-   0        0        0    10797 2022-08-03 08:27:58.000000 tomato-0.2rc2/src/tomato/drivers/driver_funcs.py
+drwxrwxrwx   0        0        0        0 2022-08-30 08:42:24.015398 tomato-0.2rc2/src/tomato/drivers/dummy/
+-rw-rw-rw-   0        0        0     1014 2022-08-18 12:19:10.000000 tomato-0.2rc2/src/tomato/drivers/dummy/__init__.py
+-rw-rw-rw-   0        0        0     5104 2022-08-22 10:37:04.000000 tomato-0.2rc2/src/tomato/drivers/dummy/main.py
+-rw-rw-rw-   0        0        0      728 2022-06-13 07:32:21.000000 tomato-0.2rc2/src/tomato/drivers/logger_funcs.py
+-rw-rw-rw-   0        0        0     1846 2022-08-30 08:21:21.000000 tomato-0.2rc2/src/tomato/drivers/yadg_funcs.py
+drwxrwxrwx   0        0        0        0 2022-08-30 08:42:24.020385 tomato-0.2rc2/src/tomato/ketchup/
+-rw-rw-rw-   0        0        0      896 2022-08-16 11:45:00.000000 tomato-0.2rc2/src/tomato/ketchup/__init__.py
+-rw-rw-rw-   0        0        0    17279 2022-08-22 10:37:04.000000 tomato-0.2rc2/src/tomato/ketchup/functions.py
+-rw-rw-rw-   0        0        0     5921 2022-08-30 08:21:21.000000 tomato-0.2rc2/src/tomato/main.py
+drwxrwxrwx   0        0        0        0 2022-08-30 08:42:24.024374 tomato-0.2rc2/src/tomato/setlib/
+-rw-rw-rw-   0        0        0       62 2022-06-13 07:32:21.000000 tomato-0.2rc2/src/tomato/setlib/__init__.py
+-rw-rw-rw-   0        0        0     4759 2022-06-13 07:32:21.000000 tomato-0.2rc2/src/tomato/setlib/functions.py
+drwxrwxrwx   0        0        0        0 2022-08-30 08:42:23.846848 tomato-0.2rc2/src/tomato.egg-info/
+-rw-rw-rw-   0        0        0     1478 2022-08-30 08:42:23.000000 tomato-0.2rc2/src/tomato.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1260 2022-08-30 08:42:23.000000 tomato-0.2rc2/src/tomato.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-08-30 08:42:23.000000 tomato-0.2rc2/src/tomato.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2022-08-30 08:42:23.000000 tomato-0.2rc2/src/tomato.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      176 2022-08-30 08:42:23.000000 tomato-0.2rc2/src/tomato.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2022-08-30 08:42:23.000000 tomato-0.2rc2/src/tomato.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    83320 2022-06-13 07:32:22.000000 tomato-0.2rc2/versioneer.py
```

### Comparing `tomato-0.2rc1/LICENSE` & `tomato-0.2rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `tomato-0.2rc1/PKG-INFO` & `tomato-0.2rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomato
-Version: 0.2rc1
+Version: 0.2rc2
 Summary: au-tomation without pain!
 Home-page: https://github.com/dgbowl/tomato
 Author: Peter Kraus
 Author-email: peter@tondon.de
 Project-URL: Bug Tracker, https://github.com/dgbowl/tomato/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `tomato-0.2rc1/README.md` & `tomato-0.2rc2/README.md`

 * *Files identical despite different names*

### Comparing `tomato-0.2rc1/setup.py` & `tomato-0.2rc2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     packages=setuptools.find_packages(where=packagedir),
     python_requires=">=3.9",
     install_requires=[
         "appdirs>=1.4.0",
         "toml",
         "pyyaml",
         "psutil",
-        "yadg>=4.1",
+        "yadg>=4.2<5.0",
         "dgbowl_schemas>=108",
         "filelock",
     ],
     extras_require={
         "testing": [
             "pytest",
         ],
```

### Comparing `tomato-0.2rc1/src/tomato/_version.py` & `tomato-0.2rc2/src/tomato/_version.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2022-08-22T13:40:40+0200",
+ "date": "2022-08-30T10:19:39+0200",
  "dirty": false,
  "error": null,
- "full-revisionid": "ea713c60819fee837010a2ec0fddf4fa5a77a2e4",
- "version": "0.2rc1"
+ "full-revisionid": "567314536eca768e07ca3b0429cf6da5bf8077f4",
+ "version": "0.2rc2"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

### Comparing `tomato-0.2rc1/src/tomato/daemon/main.py` & `tomato-0.2rc2/src/tomato/daemon/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,28 +7,40 @@
 from .. import dbhandler
 
 log = logging.getLogger(__name__)
 
 
 def _kill_tomato_job(proc):
     pc = proc.children()
-    log.warning(f"{proc.name()=}, {proc.pid=}, {pc=}")
+    log.warning(
+        "killing proc: name='%s', pid=%d, children=%d", proc.name(), proc.pid, len(pc)
+    )
     if psutil.WINDOWS:
         for proc in pc:
             if proc.name() in {"conhost.exe"}:
                 continue
             ppc = proc.children()
             for proc in ppc:
-                log.debug(f"{proc.name()=}, {proc.pid=}, {proc.children()=}")
-                proc.terminate()
+                try:
+                    proc.terminate()
+                except psutil.NoSuchProcess:
+                    log.warning(
+                        "dead proc: name='%s', pid=%d", proc.name(), proc.pid
+                    )
+                    continue
             gone, alive = psutil.wait_procs(ppc, timeout=10)
     elif psutil.POSIX:
         for proc in pc:
-            log.debug(f"{proc.name()=}, {proc.pid=}, {proc.children()=}")
-            proc.terminate()
+            try:
+                proc.terminate()
+            except psutil.NoSuchProcess:
+                log.warning(
+                    "dead proc: name='%s', pid=%d", proc.name(), proc.pid
+                )
+                continue
         gone, alive = psutil.wait_procs(pc, timeout=10)
     log.debug(f"{gone=}")
     log.debug(f"{alive=}")
 
 
 def _find_matching_pipelines(pipelines: list, method: list[dict]) -> list[str]:
     req_names = set([item["device"] for item in method])
@@ -59,14 +71,15 @@
         if sample["name"] == sampleid:
             return True
         else:
             return False
 
 
 def main_loop(settings: dict, pipelines: dict, test: bool = False) -> None:
+    log.info("Entered 'main_loop'.")
     qup = settings["queue"]["path"]
     qut = settings["queue"]["type"]
     stp = settings["state"]["path"]
     stt = settings["state"]["type"]
     while True:
         # check existing PIDs in state
         ret = dbhandler.pipeline_get_running(stp, type=stt)
```

### Comparing `tomato-0.2rc1/src/tomato/dbhandler/sqlite.py` & `tomato-0.2rc2/src/tomato/dbhandler/sqlite.py`

 * *Files identical despite different names*

### Comparing `tomato-0.2rc1/src/tomato/drivers/biologic/__init__.py` & `tomato-0.2rc2/src/tomato/drivers/biologic/__init__.py`

 * *Files identical despite different names*

### Comparing `tomato-0.2rc1/src/tomato/drivers/biologic/kbio/c_utils.py` & `tomato-0.2rc2/src/tomato/drivers/biologic/kbio/c_utils.py`

 * *Files identical despite different names*

### Comparing `tomato-0.2rc1/src/tomato/drivers/biologic/kbio/kbio_api.py` & `tomato-0.2rc2/src/tomato/drivers/biologic/kbio/kbio_api.py`

 * *Files identical despite different names*

### Comparing `tomato-0.2rc1/src/tomato/drivers/biologic/kbio/kbio_tech.py` & `tomato-0.2rc2/src/tomato/drivers/biologic/kbio/kbio_tech.py`

 * *Files identical despite different names*

### Comparing `tomato-0.2rc1/src/tomato/drivers/biologic/kbio/kbio_types.py` & `tomato-0.2rc2/src/tomato/drivers/biologic/kbio/kbio_types.py`

 * *Files identical despite different names*

### Comparing `tomato-0.2rc1/src/tomato/drivers/biologic/kbio/tech_types.py` & `tomato-0.2rc2/src/tomato/drivers/biologic/kbio/tech_types.py`

 * *Files identical despite different names*

### Comparing `tomato-0.2rc1/src/tomato/drivers/biologic/kbio/utils.py` & `tomato-0.2rc2/src/tomato/drivers/biologic/kbio/utils.py`

 * *Files identical despite different names*

### Comparing `tomato-0.2rc1/src/tomato/drivers/biologic/kbio_wrapper.py` & `tomato-0.2rc2/src/tomato/drivers/biologic/kbio_wrapper.py`

 * *Files identical despite different names*

### Comparing `tomato-0.2rc1/src/tomato/drivers/biologic/main.py` & `tomato-0.2rc2/src/tomato/drivers/biologic/main.py`

 * *Files identical despite different names*

### Comparing `tomato-0.2rc1/src/tomato/drivers/biologic/tech_params.py` & `tomato-0.2rc2/src/tomato/drivers/biologic/tech_params.py`

 * *Files identical despite different names*

### Comparing `tomato-0.2rc1/src/tomato/drivers/driver_funcs.py` & `tomato-0.2rc2/src/tomato/drivers/driver_funcs.py`

 * *Files identical despite different names*

### Comparing `tomato-0.2rc1/src/tomato/drivers/dummy/__init__.py` & `tomato-0.2rc2/src/tomato/drivers/dummy/__init__.py`

 * *Files identical despite different names*

### Comparing `tomato-0.2rc1/src/tomato/drivers/dummy/main.py` & `tomato-0.2rc2/src/tomato/drivers/dummy/main.py`

 * *Files identical despite different names*

### Comparing `tomato-0.2rc1/src/tomato/drivers/logger_funcs.py` & `tomato-0.2rc2/src/tomato/drivers/logger_funcs.py`

 * *Files identical despite different names*

### Comparing `tomato-0.2rc1/src/tomato/drivers/yadg_funcs.py` & `tomato-0.2rc2/src/tomato/drivers/yadg_funcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "biologic": "electrochem",
 }
 
 
 def get_yadg_preset(method: list[dict], pipeline: dict) -> dict:
     preset = {
         "metadata": {
-            "version": "4.1.1",
+            "version": "4.2",
             "provenance": {"type": "tomato"},
             "timezone": "localtime",
         },
         "steps": [],
     }
 
     devices = {item["tag"]: item["driver"] for item in pipeline["devices"]}
```

### Comparing `tomato-0.2rc1/src/tomato/ketchup/__init__.py` & `tomato-0.2rc2/src/tomato/ketchup/__init__.py`

 * *Files identical despite different names*

### Comparing `tomato-0.2rc1/src/tomato/ketchup/functions.py` & `tomato-0.2rc2/src/tomato/ketchup/functions.py`

 * *Files identical despite different names*

### Comparing `tomato-0.2rc1/src/tomato/main.py` & `tomato-0.2rc2/src/tomato/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,17 +79,16 @@
     _logging_setup(args)
 
     if psutil.WINDOWS:
         pid = os.getppid()
     elif psutil.POSIX:
         pid = os.getpid()
 
-    toms = [
-        p.pid for p in psutil.process_iter() if p.name() in {"tomato", "tomato.exe"}
-    ]
+    procs = psutil.process_iter(['pid', 'name'])
+    toms = [p.pid for p in procs if p.name() in {"tomato", "tomato.exe"}]
     toms.pop(toms.index(pid))
     if len(toms) > 0 and not args.test:
         logging.critical("cannot run more than one instance of 'tomato'")
         logging.info(f"'tomato' is currently running as pid {toms}")
         return
 
     dirs = setlib.get_dirs(args.test)
```

### Comparing `tomato-0.2rc1/src/tomato/setlib/functions.py` & `tomato-0.2rc2/src/tomato/setlib/functions.py`

 * *Files identical despite different names*

### Comparing `tomato-0.2rc1/src/tomato.egg-info/PKG-INFO` & `tomato-0.2rc2/src/tomato.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomato
-Version: 0.2rc1
+Version: 0.2rc2
 Summary: au-tomation without pain!
 Home-page: https://github.com/dgbowl/tomato
 Author: Peter Kraus
 Author-email: peter@tondon.de
 Project-URL: Bug Tracker, https://github.com/dgbowl/tomato/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `tomato-0.2rc1/src/tomato.egg-info/SOURCES.txt` & `tomato-0.2rc2/src/tomato.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tomato-0.2rc1/versioneer.py` & `tomato-0.2rc2/versioneer.py`

 * *Files identical despite different names*

