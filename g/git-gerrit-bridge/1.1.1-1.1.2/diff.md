# Comparing `tmp/git_gerrit_bridge-1.1.1.tar.gz` & `tmp/git_gerrit_bridge-1.1.2.tar.gz`

## Comparing `git_gerrit_bridge-1.1.1.tar` & `git_gerrit_bridge-1.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.1/git_gerrit/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.1/git_gerrit/__init__.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.1/git_gerrit/__main__.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.1/git_gerrit/cli/__init__.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.1/git_gerrit/cli/checkout.py
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.1/git_gerrit/cli/clean.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.1/git_gerrit/cli/new.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.1/git_gerrit/cli/push.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.1/git_gerrit/cli/rebase.py
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.1/git_gerrit/cli/status.py
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.1/git_gerrit/cli/sync.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.1/git_gerrit/utils/__init__.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.1/git_gerrit/utils/branch.py
--rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.1/git_gerrit/utils/change.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.1/git_gerrit/utils/changebase.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.1/git_gerrit/utils/gerrit.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.1/git_gerrit/utils/git.py
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.1/git_gerrit/utils/localchange.py
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.1/git_gerrit/utils/remotechange.py
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.1/git_gerrit/utils/version.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.1/.gitignore
--rw-r--r--   0        0        0    34670 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.1/LICENSE.txt
--rw-r--r--   0        0        0     5004 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.1/README.md
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     6213 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/__init__.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/__main__.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/cli/__init__.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/cli/checkout.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/cli/clean.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/cli/new.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/cli/push.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/cli/rebase.py
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/cli/status.py
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/cli/sync.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/utils/__init__.py
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/utils/branch.py
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/utils/change.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/utils/changebase.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/utils/gerrit.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/utils/git.py
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/utils/localchange.py
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/utils/remotechange.py
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/git_gerrit/utils/version.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/.gitignore
+-rw-r--r--   0        0        0    34670 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/LICENSE.txt
+-rw-r--r--   0        0        0     5004 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/README.md
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6213 2020-02-02 00:00:00.000000 git_gerrit_bridge-1.1.2/PKG-INFO
```

### Comparing `git_gerrit_bridge-1.1.1/.github/workflows/pypi-publish.yml` & `git_gerrit_bridge-1.1.2/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `git_gerrit_bridge-1.1.1/git_gerrit/cli/__init__.py` & `git_gerrit_bridge-1.1.2/git_gerrit/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `git_gerrit_bridge-1.1.1/git_gerrit/cli/checkout.py` & `git_gerrit_bridge-1.1.2/git_gerrit/cli/checkout.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,8 +19,8 @@
         change = changes[0]
         if name is None:
             name = change.recommend_branch_name()
 
         git["fetch", GitConfig.remote(), change.gerrit_ref].run_fg()
         git["branch", name, "FETCH_HEAD"].run_fg() # create new branch
         git["branch", "--set-upstream-to", f"{GitConfig.remote()}/{change.branch_remote}", name].run_fg()
-        git["switch", name].run_fg()
+        git["switch", name].run_fg(retcode=None)
```

### Comparing `git_gerrit_bridge-1.1.1/git_gerrit/cli/clean.py` & `git_gerrit_bridge-1.1.2/git_gerrit/cli/clean.py`

 * *Files identical despite different names*

### Comparing `git_gerrit_bridge-1.1.1/git_gerrit/cli/push.py` & `git_gerrit_bridge-1.1.2/git_gerrit/cli/push.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,9 +22,9 @@
         b = LocalBranch.from_head() or LocalBranch.from_rebase()
         if b is None:
             print("Current branch not known, no branch checked out?")
             return 1
         if b.remote_name == "":
             print("Current branch has no remote, cannot push to gerrit")
             return 1
-        cmd = ["push", GitConfig.remote(), f"HEAD:refs/for/{b.remote_name}", "-o", f"hashtag=branch:{b.local_name}"] + self.options
-        git[cmd].run_fg()
+        cmd = ["push", b.remote, f"HEAD:refs/for/{b.remote_name}", "-o", f"hashtag=branch:{b.local_name}"] + self.options
+        git[cmd].run_fg(retcode=None)
```

### Comparing `git_gerrit_bridge-1.1.1/git_gerrit/cli/rebase.py` & `git_gerrit_bridge-1.1.2/git_gerrit/cli/rebase.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,8 +17,8 @@
             print("Current branch not known, no branch checked out?")
             return 1
         num_changes = len(b.get_changes())
         if num_changes == 0:
             print("Nothing to rebase")
             return 0
         console.print(f"Starting interactive rebase of [magenta1]{b.local_name}[/] with {num_changes} Changes...")
-        git["rebase", "-i", f"HEAD~{num_changes}"].run_fg()
+        git["rebase", "-i", f"HEAD~{num_changes}"].run_fg(retcode=None)
```

### Comparing `git_gerrit_bridge-1.1.1/git_gerrit/cli/status.py` & `git_gerrit_bridge-1.1.2/git_gerrit/cli/status.py`

 * *Files identical despite different names*

### Comparing `git_gerrit_bridge-1.1.1/git_gerrit/cli/sync.py` & `git_gerrit_bridge-1.1.2/git_gerrit/cli/sync.py`

 * *Files identical despite different names*

### Comparing `git_gerrit_bridge-1.1.1/git_gerrit/utils/branch.py` & `git_gerrit_bridge-1.1.2/git_gerrit/utils/branch.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,15 +7,18 @@
 from git_gerrit.utils.localchange import LocalChange
 from git_gerrit.utils.git import GitConfig, git
 
 class LocalBranch:
     def __init__(self, ref: str):
         self.local_name = git["rev-parse", "--abbrev-ref", ref]().strip()
         self.remote_ref = git["for-each-ref", "--format=%(upstream:short)", ref]().strip()
-        self.remote_name = self.remote_ref.replace(f"{GitConfig.remote()}/", "")
+        split = self.remote_ref.split("/")
+        assert len(split) > 0 and len(split) <= 2, f"Unexpected/supported remote name {self.remote_ref}"
+        self.remote = split[0]
+        self.remote_name = split[1] if len(split) > 1 else ""
 
     def has_remote(self):
         return self.remote_ref != ""
 
     def get_changes(self) -> list[LocalChange]:
         if not self.has_remote():
             return []
```

### Comparing `git_gerrit_bridge-1.1.1/git_gerrit/utils/change.py` & `git_gerrit_bridge-1.1.2/git_gerrit/utils/change.py`

 * *Files identical despite different names*

### Comparing `git_gerrit_bridge-1.1.1/git_gerrit/utils/gerrit.py` & `git_gerrit_bridge-1.1.2/git_gerrit/utils/gerrit.py`

 * *Files identical despite different names*

### Comparing `git_gerrit_bridge-1.1.1/git_gerrit/utils/git.py` & `git_gerrit_bridge-1.1.2/git_gerrit/utils/git.py`

 * *Files identical despite different names*

### Comparing `git_gerrit_bridge-1.1.1/git_gerrit/utils/localchange.py` & `git_gerrit_bridge-1.1.2/git_gerrit/utils/localchange.py`

 * *Files identical despite different names*

### Comparing `git_gerrit_bridge-1.1.1/git_gerrit/utils/remotechange.py` & `git_gerrit_bridge-1.1.2/git_gerrit/utils/remotechange.py`

 * *Files identical despite different names*

### Comparing `git_gerrit_bridge-1.1.1/git_gerrit/utils/version.py` & `git_gerrit_bridge-1.1.2/git_gerrit/utils/version.py`

 * *Files identical despite different names*

### Comparing `git_gerrit_bridge-1.1.1/LICENSE.txt` & `git_gerrit_bridge-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `git_gerrit_bridge-1.1.1/README.md` & `git_gerrit_bridge-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `git_gerrit_bridge-1.1.1/pyproject.toml` & `git_gerrit_bridge-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `git_gerrit_bridge-1.1.1/PKG-INFO` & `git_gerrit_bridge-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: git-gerrit-bridge
-Version: 1.1.1
+Version: 1.1.2
 Summary: Git subcommand to ease local branch management with gerrit.
 Project-URL: Documentation, https://github.com/Scheirle/git-gerrit-bridget#readme
 Project-URL: Issues, https://github.com/Scheirle/git-gerrit-bridge/issues
 Project-URL: Source, https://github.com/Scheirle/git-gerrit-bridge
 Author-email: Bernhard Scheirle <bernhard@scheirle.de>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE.txt
```

