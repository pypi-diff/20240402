# Comparing `tmp/dfsync-0.4.8.tar.gz` & `tmp/dfsync-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfsync-0.4.8.tar", max compression
+gzip compressed data, was "dfsync-0.4.9.tar", max compression
```

## Comparing `dfsync-0.4.8.tar` & `dfsync-0.4.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0        0 2023-07-31 08:22:13.656849 dfsync-0.4.8/dfsync/__init__.py
--rw-r--r--   0        0        0       64 2024-03-07 18:04:07.938907 dfsync-0.4.8/dfsync/backends/__init__.py
--rw-r--r--   0        0        0    25594 2024-03-19 04:23:34.296068 dfsync-0.4.8/dfsync/backends/kube.py
--rwxr-xr-x   0        0        0     2198 2023-09-19 03:56:44.162177 dfsync-0.4.8/dfsync/backends/kube_exec.py
--rw-r--r--   0        0        0    10484 2023-09-07 22:00:21.486913 dfsync-0.4.8/dfsync/backends/rsync.py
--rw-r--r--   0        0        0     4149 2024-03-19 04:51:59.690558 dfsync-0.4.8/dfsync/char_ui.py
--rw-r--r--   0        0        0     1334 2024-03-19 04:36:59.575076 dfsync-0.4.8/dfsync/chcli.py
--rw-r--r--   0        0        0      582 2023-07-25 16:18:24.031315 dfsync-0.4.8/dfsync/check_dns.py
--rw-r--r--   0        0        0      148 2023-06-17 21:12:04.987300 dfsync-0.4.8/dfsync/cli.py
--rw-r--r--   0        0        0     2813 2023-10-25 22:06:40.226637 dfsync-0.4.8/dfsync/config.py
--rw-r--r--   0        0        0     4403 2024-01-09 19:06:06.461148 dfsync-0.4.8/dfsync/diffui.py
--rw-r--r--   0        0        0     3977 2024-03-21 10:07:51.363601 dfsync-0.4.8/dfsync/distribution.py
--rw-r--r--   0        0        0     3241 2021-03-30 12:50:07.000000 dfsync-0.4.8/dfsync/exp.py
--rw-r--r--   0        0        0     7193 2023-08-05 10:09:42.805988 dfsync-0.4.8/dfsync/filters.py
--rw-r--r--   0        0        0     7682 2024-03-21 10:15:52.078127 dfsync-0.4.8/dfsync/kube_credentials.py
--rw-r--r--   0        0        0     1075 2024-03-18 10:11:54.096891 dfsync-0.4.8/dfsync/lib.py
--rw-r--r--   0        0        0    16536 2024-03-21 10:03:49.440976 dfsync-0.4.8/dfsync/monitor.py
--rw-r--r--   0        0        0     1366 2024-03-21 10:00:26.274891 dfsync-0.4.8/dfsync/test_dfsync.py
--rw-r--r--   0        0        0      947 2024-03-21 09:59:44.303758 dfsync-0.4.8/dfsync/test_distribution.py
--rw-r--r--   0        0        0     5264 2024-03-21 10:22:20.749341 dfsync-0.4.8/dfsync/test_kube_credentials.py
--rw-r--r--   0        0        0      747 2023-11-04 12:34:08.162114 dfsync-0.4.8/dfsync/test_lib.py
--rw-r--r--   0        0        0     3350 2021-04-28 13:06:18.000000 dfsync-0.4.8/dfsync/transactions.py
--rw-r--r--   0        0        0      698 2024-03-21 10:28:10.346248 dfsync-0.4.8/pyproject.toml
--rw-r--r--   0        0        0      819 1970-01-01 00:00:00.000000 dfsync-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-31 08:22:13.656849 dfsync-0.4.9/dfsync/__init__.py
+-rw-r--r--   0        0        0       64 2024-03-07 18:04:07.938907 dfsync-0.4.9/dfsync/backends/__init__.py
+-rw-r--r--   0        0        0    25594 2024-03-19 04:23:34.296068 dfsync-0.4.9/dfsync/backends/kube.py
+-rwxr-xr-x   0        0        0     2198 2023-09-19 03:56:44.162177 dfsync-0.4.9/dfsync/backends/kube_exec.py
+-rw-r--r--   0        0        0    10484 2023-09-07 22:00:21.486913 dfsync-0.4.9/dfsync/backends/rsync.py
+-rw-r--r--   0        0        0     4149 2024-03-19 04:51:59.690558 dfsync-0.4.9/dfsync/char_ui.py
+-rw-r--r--   0        0        0     1334 2024-03-19 04:36:59.575076 dfsync-0.4.9/dfsync/chcli.py
+-rw-r--r--   0        0        0      582 2023-07-25 16:18:24.031315 dfsync-0.4.9/dfsync/check_dns.py
+-rw-r--r--   0        0        0      148 2023-06-17 21:12:04.987300 dfsync-0.4.9/dfsync/cli.py
+-rw-r--r--   0        0        0     2813 2023-10-25 22:06:40.226637 dfsync-0.4.9/dfsync/config.py
+-rw-r--r--   0        0        0     4403 2024-01-09 19:06:06.461148 dfsync-0.4.9/dfsync/diffui.py
+-rw-r--r--   0        0        0     3977 2024-03-21 10:07:51.363601 dfsync-0.4.9/dfsync/distribution.py
+-rw-r--r--   0        0        0     3241 2021-03-30 12:50:07.000000 dfsync-0.4.9/dfsync/exp.py
+-rw-r--r--   0        0        0     7690 2024-04-02 07:01:10.896135 dfsync-0.4.9/dfsync/filters.py
+-rw-r--r--   0        0        0     7682 2024-03-21 10:15:52.078127 dfsync-0.4.9/dfsync/kube_credentials.py
+-rw-r--r--   0        0        0     1075 2024-03-18 10:11:54.096891 dfsync-0.4.9/dfsync/lib.py
+-rw-r--r--   0        0        0    17234 2024-04-02 07:23:36.654832 dfsync-0.4.9/dfsync/monitor.py
+-rw-r--r--   0        0        0     1366 2024-03-21 10:00:26.274891 dfsync-0.4.9/dfsync/test_dfsync.py
+-rw-r--r--   0        0        0      947 2024-03-21 09:59:44.303758 dfsync-0.4.9/dfsync/test_distribution.py
+-rw-r--r--   0        0        0     5264 2024-03-21 10:22:20.749341 dfsync-0.4.9/dfsync/test_kube_credentials.py
+-rw-r--r--   0        0        0      747 2023-11-04 12:34:08.162114 dfsync-0.4.9/dfsync/test_lib.py
+-rw-r--r--   0        0        0     3350 2021-04-28 13:06:18.000000 dfsync-0.4.9/dfsync/transactions.py
+-rw-r--r--   0        0        0      698 2024-04-02 12:25:16.566591 dfsync-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0      819 1970-01-01 00:00:00.000000 dfsync-0.4.9/PKG-INFO
```

### Comparing `dfsync-0.4.8/dfsync/backends/kube.py` & `dfsync-0.4.9/dfsync/backends/kube.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.8/dfsync/backends/kube_exec.py` & `dfsync-0.4.9/dfsync/backends/kube_exec.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.8/dfsync/backends/rsync.py` & `dfsync-0.4.9/dfsync/backends/rsync.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.8/dfsync/char_ui.py` & `dfsync-0.4.9/dfsync/char_ui.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.8/dfsync/chcli.py` & `dfsync-0.4.9/dfsync/chcli.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.8/dfsync/check_dns.py` & `dfsync-0.4.9/dfsync/check_dns.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.8/dfsync/config.py` & `dfsync-0.4.9/dfsync/config.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.8/dfsync/diffui.py` & `dfsync-0.4.9/dfsync/diffui.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.8/dfsync/distribution.py` & `dfsync-0.4.9/dfsync/distribution.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.8/dfsync/exp.py` & `dfsync-0.4.9/dfsync/exp.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.8/dfsync/filters.py` & `dfsync-0.4.9/dfsync/filters.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-import black, fnmatch
+import black
+import fnmatch
 import os.path
 import git.exc
 import subprocess
 from watchdog.events import FileCreatedEvent, FileModifiedEvent, FileDeletedEvent
 
 
 def exclude_watchdog_directory_events(event=None, **kwargs):
@@ -107,14 +108,18 @@
 
 class UntrackedGitFilesFilter(LoggingFilter):
     def __init__(self):
         super().__init__()
         self._repos = {}
         self._is_repo_initialized = {}
         self._untracked_and_ignored_files = {}
+        self._should_filter_untracked_files = True
+
+    def set_should_filter_untracked_files(self, should_filter_untracked_files: bool = True):
+        self._should_filter_untracked_files = should_filter_untracked_files
 
     def get_untracked_and_ignored_files(self):
         flat_files = []
         for fn in self._untracked_and_ignored_files.values():
             flat_files.extend(fn)
         return flat_files
 
@@ -171,21 +176,25 @@
             self._ignore(src_file_path, "file is in .gitignore")
             return True
 
         if "/.git/" in src_file_path:
             self._ignore(src_file_path, "GIT repo internals")
             return True
 
-        for rel_file_path in repo.untracked_files:
-            abs_file_path = os.path.join(repo.working_dir, rel_file_path)
-            if src_abs_path == abs_file_path:
-                self._ignore(src_file_path, "Untracked GIT file")
-                return True
+        if self._should_filter_untracked_files and self._is_untracked_file(repo, src_abs_path):
+            self._ignore(src_file_path, "Untracked GIT file")
+            return True
+
         return False
 
+    def _is_untracked_file(self, repo, src_abs_path):
+        return any(
+            src_abs_path == os.path.join(repo.working_dir, rel_file_path) for rel_file_path in repo.untracked_files
+        )
+
 
 USER_FILTERS = [EmacsBufferFilter(), PythonBlackFilter()]
 GIT_FILTER = UntrackedGitFilesFilter()
 ALL_FILTERS = [
     exclude_watchdog_directory_events,
     *[f.is_not_filtered for f in USER_FILTERS],
     GIT_FILTER.is_not_filtered,
@@ -211,7 +220,11 @@
         raise ValueError("Expecting non-null user filter")
     USER_FILTERS.append(f)
     ALL_FILTERS.append(f.is_not_filtered)
 
 
 def add_user_ignored_patterns_filter(patterns: [str]):
     add_user_filter(UserConfigFilter(patterns))
+
+
+def set_ignore_untracked_files(should_ignore_untracked_files: bool):
+    GIT_FILTER.set_should_filter_untracked_files(should_ignore_untracked_files)
```

### Comparing `dfsync-0.4.8/dfsync/kube_credentials.py` & `dfsync-0.4.9/dfsync/kube_credentials.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.8/dfsync/lib.py` & `dfsync-0.4.9/dfsync/lib.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.8/dfsync/monitor.py` & `dfsync-0.4.9/dfsync/monitor.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 
 from click_default_group import DefaultGroup
 from contextlib import contextmanager
 from functools import partial
 from watchdog.observers import Observer
 from watchdog.events import FileSystemEventHandler
 
+import dfsync.filters as filters
 from dfsync.backends import rsync_backend, kube_backend
 from dfsync.distribution import (
     get_installed_version,
     get_latest_version,
     is_older_version,
     AsyncVersionChecker,
     is_installed_in_editable_mode,
     update_package,
 )
-from dfsync.filters import add_user_ignored_patterns_filter, ALL_FILTERS
 from dfsync.config import read_config
 from dfsync.char_ui import KeyController
 from dfsync.kube_credentials import contextualize_kube_credentials, update_local_kube_config, normalized_k8s_url
 from dfsync.lib import ControlledThreadedOperation, thread_manager
 
 logging.basicConfig(level=logging.WARN)
 
@@ -50,15 +50,15 @@
         backend: str = "log",
         watched_dir: str = ".",
         all_watched_dirs: list = None,
         input_controller: KeyController = None,
         **kwargs,
     ):
         super().__init__()
-        self.filters = [*ALL_FILTERS]
+        self.filters = [*filters.ALL_FILTERS]
 
         self.backend = backend
         self.backend_options = kwargs
         self.raised_exception = False
         self.watched_dir = watched_dir
         self.abs_watched_dir = os.path.abspath(watched_dir)
         self.input_controller = input_controller
@@ -259,26 +259,40 @@
 
 
 @main.command()
 def version():
     """
     Print the currently installed version
     """
+    _version()
+
+
+def _version():
     installed_version = get_installed_version()
     click.echo(f"{installed_version}")
 
     latest_version = get_latest_version()
     if not is_older_version(installed_version, latest_version):
         return
     elif is_installed_in_editable_mode("dfsync"):
         click.echo(f"Latest version is {latest_version}, please update!")
     else:
         click.echo(f"Latest version is {latest_version}, please update using `dfsync self-update`")
 
 
+@main.command(name="help", context_settings=dict(ignore_unknown_options=True))
+@click.option("--help", is_flag=True, default=False, hidden=True)
+def help(help):
+    """
+    Print the usage/help for dfsync
+    """
+    with click.Context(sync, info_name="dfsync") as ctx:
+        click.echo(sync.get_help(ctx))
+
+
 @main.command()
 def self_update():
     """
     Update dfsync to the latest version published on pypi
     """
     latest_version = get_latest_version()
     installed_version = get_installed_version()
@@ -305,19 +319,23 @@
     patch = contextualize_kube_credentials(normalized_k8s_url(kube_host), credentials)
     update_local_kube_config(patch)
 
 
 @main.command()
 @click.argument("source", nargs=-1)
 @click.argument("destination", default="", nargs=1)
-@click.option("--supervisor/--no-supervisor", default=False, help="Try to install supervisor in container", type=bool)
+@click.option("--supervisor", is_flag=True, default=False, help="Try to install supervisor in container")
 @click.option("--kube-host", default=None, help="Kubernetes api host server address/hostname", type=str)
 @click.option("--pod-timeout", default=30, help="Pod reconfiguration timeout (default is 30 seconds)", type=int)
 @click.option("--full-sync/--no-full-sync", default=True, help="On startup, sync all files to destination", type=bool)
-def sync(source, destination, supervisor, kube_host, pod_timeout, full_sync):
+@click.option("--version", is_flag=True, default=False, help="Print the currently installed version")
+@click.option(
+    "--sync-git-untracked", is_flag=True, default=False, help="Sync git-untracked files instead of ignoring them"
+)
+def sync(source, destination, supervisor, kube_host, pod_timeout, full_sync, version, sync_git_untracked):
     """
     Watches a folder for changes and propagates all file changes to a destination.
 
     SOURCE is a path to the folder that dfsync will monitor for changes (or current dir if missing)
 
     DESTINATION is a destination path / psuedo-url
 
@@ -349,15 +367,22 @@
         level=logging.WARN,
         format="%(asctime)s - %(message)s",
         datefmt="%Y-%m-%d %H:%M:%S",
     )
 
     paths = ["."] if len(source) == 0 else source
     config = read_config(destination, *paths)
-    add_user_ignored_patterns_filter(config.ignore_files)
+    filters.add_user_ignored_patterns_filter(config.ignore_files)
+
+    if sync_git_untracked:
+        filters.set_ignore_untracked_files(False)
+
+    if version:
+        _version()
+        return
 
     destination_dir = destination
     if len(source) == 0 and config.destination and not has_destination_optics(destination):
         destination_dir = config.destination
         paths = [destination] if destination else paths
     missing, paths = filter_missing_paths([*config.additional_sources, *paths])
     if len(missing) > 0 and len(paths) > 0:
```

### Comparing `dfsync-0.4.8/dfsync/test_dfsync.py` & `dfsync-0.4.9/dfsync/test_dfsync.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.8/dfsync/test_distribution.py` & `dfsync-0.4.9/dfsync/test_distribution.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.8/dfsync/test_kube_credentials.py` & `dfsync-0.4.9/dfsync/test_kube_credentials.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.8/dfsync/test_lib.py` & `dfsync-0.4.9/dfsync/test_lib.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.8/dfsync/transactions.py` & `dfsync-0.4.9/dfsync/transactions.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.8/pyproject.toml` & `dfsync-0.4.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dfsync"
-version = "0.4.8"
+version = "0.4.9"
 description = ""
 authors = ["Mihai Balint <balint.mihai@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 watchdog = "^2.0.2"
 gitpython = "^3.1.14"
```

### Comparing `dfsync-0.4.8/PKG-INFO` & `dfsync-0.4.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfsync
-Version: 0.4.8
+Version: 0.4.9
 Summary: 
 Author: Mihai Balint
 Author-email: balint.mihai@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

