# Comparing `tmp/helm-hawk-0.0.1.tar.gz` & `tmp/helm-hawk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helm-hawk-0.0.1.tar", last modified: Mon Apr  1 12:20:27 2024, max compression
+gzip compressed data, was "helm-hawk-0.0.2.tar", last modified: Tue Apr  2 12:32:04 2024, max compression
```

## Comparing `helm-hawk-0.0.1.tar` & `helm-hawk-0.0.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 12:20:27.910774 helm-hawk-0.0.1/
--rw-r--r--   0 vsts      (1001) docker     (127)       68 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     4531 2024-04-01 12:20:27.910774 helm-hawk-0.0.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     4168 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 12:20:27.906774 helm-hawk-0.0.1/cli/
--rw-r--r--   0 vsts      (1001) docker     (127)       21 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 12:20:27.906774 helm-hawk-0.0.1/cli/diff/
--rw-r--r--   0 vsts      (1001) docker     (127)       36 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/diff/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 12:20:27.906774 helm-hawk-0.0.1/cli/diff/commands/
--rw-r--r--   0 vsts      (1001) docker     (127)      112 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/diff/commands/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      785 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/diff/commands/diff_revision.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1142 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/diff/commands/diff_upgrade.py
--rw-r--r--   0 vsts      (1001) docker     (127)      299 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/diff/diff.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 12:20:27.906774 helm-hawk-0.0.1/cli/get/
--rw-r--r--   0 vsts      (1001) docker     (127)       33 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/get/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 12:20:27.906774 helm-hawk-0.0.1/cli/get/commands/
--rw-r--r--   0 vsts      (1001) docker     (127)       39 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/get/commands/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      924 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/get/commands/get_values.py
--rw-r--r--   0 vsts      (1001) docker     (127)      223 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/get/get.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 12:20:27.910774 helm-hawk-0.0.1/cli/history/
--rw-r--r--   0 vsts      (1001) docker     (127)       48 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/history/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      682 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/history/history.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 12:20:27.910774 helm-hawk-0.0.1/cli/list/
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/list/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1019 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/list/list.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1114 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/main.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 12:20:27.910774 helm-hawk-0.0.1/cli/pull/
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/pull/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1494 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/pull/pull.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 12:20:27.910774 helm-hawk-0.0.1/cli/repo/
--rw-r--r--   0 vsts      (1001) docker     (127)       36 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/repo/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 12:20:27.910774 helm-hawk-0.0.1/cli/repo/commands/
--rw-r--r--   0 vsts      (1001) docker     (127)      142 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/repo/commands/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      683 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/repo/commands/add.py
--rw-r--r--   0 vsts      (1001) docker     (127)      369 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/repo/commands/list.py
--rw-r--r--   0 vsts      (1001) docker     (127)      270 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/repo/commands/remove.py
--rw-r--r--   0 vsts      (1001) docker     (127)      329 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/repo/commands/update.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1048 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/repo/repo.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 12:20:27.910774 helm-hawk-0.0.1/cli/rollback/
--rw-r--r--   0 vsts      (1001) docker     (127)       50 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/rollback/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1162 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/rollback/rollback.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 12:20:27.910774 helm-hawk-0.0.1/cli/status/
--rw-r--r--   0 vsts      (1001) docker     (127)       44 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/status/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1526 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/status/status.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 12:20:27.910774 helm-hawk-0.0.1/cli/template/
--rw-r--r--   0 vsts      (1001) docker     (127)       50 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/template/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1081 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/template/template.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 12:20:27.910774 helm-hawk-0.0.1/cli/uninstall/
--rw-r--r--   0 vsts      (1001) docker     (127)       53 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/uninstall/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      675 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/uninstall/uninstall.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 12:20:27.910774 helm-hawk-0.0.1/cli/upgrade/
--rw-r--r--   0 vsts      (1001) docker     (127)       49 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/upgrade/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      965 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/upgrade/upgrade.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 12:20:27.910774 helm-hawk-0.0.1/cli/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)       51 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11955 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/utils/helm.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1376 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/cli/utils/kubectl.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 12:20:27.910774 helm-hawk-0.0.1/helm_hawk.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     4531 2024-04-01 12:20:27.000000 helm-hawk-0.0.1/helm_hawk.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     1103 2024-04-01 12:20:27.000000 helm-hawk-0.0.1/helm_hawk.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-01 12:20:27.000000 helm-hawk-0.0.1/helm_hawk.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       43 2024-04-01 12:20:27.000000 helm-hawk-0.0.1/helm_hawk.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       15 2024-04-01 12:20:27.000000 helm-hawk-0.0.1/helm_hawk.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        4 2024-04-01 12:20:27.000000 helm-hawk-0.0.1/helm_hawk.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      121 2024-04-01 12:20:27.914774 helm-hawk-0.0.1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)      956 2024-04-01 12:20:15.000000 helm-hawk-0.0.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 12:32:04.115272 helm-hawk-0.0.2/
+-rw-r--r--   0 vsts      (1001) docker     (127)       68 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     4531 2024-04-02 12:32:04.115272 helm-hawk-0.0.2/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     4168 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 12:32:04.099271 helm-hawk-0.0.2/cli/
+-rw-r--r--   0 vsts      (1001) docker     (127)       21 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/cli/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 12:32:04.103272 helm-hawk-0.0.2/cli/diff/
+-rw-r--r--   0 vsts      (1001) docker     (127)       36 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/cli/diff/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 12:32:04.103272 helm-hawk-0.0.2/cli/diff/commands/
+-rw-r--r--   0 vsts      (1001) docker     (127)      112 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/cli/diff/commands/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      785 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/cli/diff/commands/diff_revision.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      919 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/cli/diff/commands/diff_upgrade.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      299 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/cli/diff/diff.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 12:32:04.103272 helm-hawk-0.0.2/cli/get/
+-rw-r--r--   0 vsts      (1001) docker     (127)       33 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/cli/get/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 12:32:04.103272 helm-hawk-0.0.2/cli/get/commands/
+-rw-r--r--   0 vsts      (1001) docker     (127)       39 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/cli/get/commands/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      924 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/cli/get/commands/get_values.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      223 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/cli/get/get.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 12:32:04.103272 helm-hawk-0.0.2/cli/history/
+-rw-r--r--   0 vsts      (1001) docker     (127)       48 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/cli/history/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      682 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/cli/history/history.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 12:32:04.103272 helm-hawk-0.0.2/cli/list/
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/cli/list/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1019 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/cli/list/list.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1114 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/cli/main.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 12:32:04.107272 helm-hawk-0.0.2/cli/pull/
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/cli/pull/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1494 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/cli/pull/pull.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 12:32:04.107272 helm-hawk-0.0.2/cli/repo/
+-rw-r--r--   0 vsts      (1001) docker     (127)       36 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/cli/repo/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 12:32:04.107272 helm-hawk-0.0.2/cli/repo/commands/
+-rw-r--r--   0 vsts      (1001) docker     (127)      142 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/cli/repo/commands/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      683 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/cli/repo/commands/add.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      369 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/cli/repo/commands/list.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      270 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/cli/repo/commands/remove.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      329 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/cli/repo/commands/update.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1048 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/cli/repo/repo.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 12:32:04.107272 helm-hawk-0.0.2/cli/rollback/
+-rw-r--r--   0 vsts      (1001) docker     (127)       50 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/cli/rollback/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1162 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/cli/rollback/rollback.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 12:32:04.107272 helm-hawk-0.0.2/cli/status/
+-rw-r--r--   0 vsts      (1001) docker     (127)       44 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/cli/status/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1526 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/cli/status/status.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 12:32:04.111271 helm-hawk-0.0.2/cli/template/
+-rw-r--r--   0 vsts      (1001) docker     (127)       50 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/cli/template/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1081 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/cli/template/template.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 12:32:04.111271 helm-hawk-0.0.2/cli/uninstall/
+-rw-r--r--   0 vsts      (1001) docker     (127)       53 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/cli/uninstall/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      675 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/cli/uninstall/uninstall.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 12:32:04.111271 helm-hawk-0.0.2/cli/upgrade/
+-rw-r--r--   0 vsts      (1001) docker     (127)       49 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/cli/upgrade/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1134 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/cli/upgrade/upgrade.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 12:32:04.111271 helm-hawk-0.0.2/cli/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)       51 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/cli/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11955 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/cli/utils/helm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1376 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/cli/utils/kubectl.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 12:32:04.115272 helm-hawk-0.0.2/helm_hawk.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4531 2024-04-02 12:32:04.000000 helm-hawk-0.0.2/helm_hawk.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     1103 2024-04-02 12:32:04.000000 helm-hawk-0.0.2/helm_hawk.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-02 12:32:04.000000 helm-hawk-0.0.2/helm_hawk.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       43 2024-04-02 12:32:04.000000 helm-hawk-0.0.2/helm_hawk.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       15 2024-04-02 12:32:04.000000 helm-hawk-0.0.2/helm_hawk.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        4 2024-04-02 12:32:04.000000 helm-hawk-0.0.2/helm_hawk.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      121 2024-04-02 12:32:04.115272 helm-hawk-0.0.2/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)      956 2024-04-02 12:31:46.000000 helm-hawk-0.0.2/setup.py
```

### Comparing `helm-hawk-0.0.1/PKG-INFO` & `helm-hawk-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helm-hawk
-Version: 0.0.1
+Version: 0.0.2
 Author: Ankit Singh
 Author-email: as8356047@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `helm-hawk-0.0.1/README.md` & `helm-hawk-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `helm-hawk-0.0.1/cli/diff/commands/diff_revision.py` & `helm-hawk-0.0.2/cli/diff/commands/diff_revision.py`

 * *Files identical despite different names*

### Comparing `helm-hawk-0.0.1/cli/diff/commands/diff_upgrade.py` & `helm-hawk-0.0.2/cli/upgrade/upgrade.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 import click
 from cli.utils.helm import Helm
 
 
-
-
-@click.command(name='upgrade')
-@click.argument('release_name',type=click.types.STRING,required=True)
-@click.argument('chart_path',type=click.Path(exists=True),required=True)
-@click.option('--values','-f',help=f"Provide values file path",type=click.Path(exists=True),multiple=True)
+@click.command(name="upgrade",help="This command upgrades a release to a new version of a chart.")
+@click.argument('release_name',type=click.STRING,required=True)
+@click.argument('chart_path', type=click.Path(exists=True),required=True)
+@click.option("--values", "-f", multiple=True, help="Specify values in a YAML file (can specify multiple)")
 @click.option('--context','-c',help="Context that you want to use",type=click.STRING)
 @click.option('--namespace','-n',help="Namespace you want to use",type=click.STRING)
-def diff_upgrade(chart_path,release_name,values,context,namespace):
-    '''Show a diff explaining what a helm upgrade would change.'''
-    helm=Helm(context=context,namespace=namespace)
-    click.echo("Validating charts...")
+@click.option('--dry-run',help="Simulate the upgrade",is_flag=True)
+def upgrade_command(release_name,chart_path,values,context,namespace,dry_run):
+    helm=Helm(namespace=namespace,context=context)
     validation=helm.validate_chart(chart_path)
     if validation is not True:
         return click.echo(validation)
     output=helm.diff(release_name,chart_path,values)
     click.echo(output)
-    # show prompt for to upgrade from diff
     prompt=input("enter Yes to perform the upgrade: ")
     if prompt.lower() == "yes":
         output=helm.upgrade(release_name,chart_path,values,False)
         click.echo(output)
```

### Comparing `helm-hawk-0.0.1/cli/get/commands/get_values.py` & `helm-hawk-0.0.2/cli/get/commands/get_values.py`

 * *Files identical despite different names*

### Comparing `helm-hawk-0.0.1/cli/history/history.py` & `helm-hawk-0.0.2/cli/history/history.py`

 * *Files identical despite different names*

### Comparing `helm-hawk-0.0.1/cli/list/list.py` & `helm-hawk-0.0.2/cli/list/list.py`

 * *Files identical despite different names*

### Comparing `helm-hawk-0.0.1/cli/main.py` & `helm-hawk-0.0.2/cli/main.py`

 * *Files identical despite different names*

### Comparing `helm-hawk-0.0.1/cli/pull/pull.py` & `helm-hawk-0.0.2/cli/pull/pull.py`

 * *Files identical despite different names*

### Comparing `helm-hawk-0.0.1/cli/repo/commands/add.py` & `helm-hawk-0.0.2/cli/repo/commands/add.py`

 * *Files identical despite different names*

### Comparing `helm-hawk-0.0.1/cli/repo/repo.py` & `helm-hawk-0.0.2/cli/repo/repo.py`

 * *Files identical despite different names*

### Comparing `helm-hawk-0.0.1/cli/rollback/rollback.py` & `helm-hawk-0.0.2/cli/rollback/rollback.py`

 * *Files identical despite different names*

### Comparing `helm-hawk-0.0.1/cli/status/status.py` & `helm-hawk-0.0.2/cli/status/status.py`

 * *Files identical despite different names*

### Comparing `helm-hawk-0.0.1/cli/template/template.py` & `helm-hawk-0.0.2/cli/template/template.py`

 * *Files identical despite different names*

### Comparing `helm-hawk-0.0.1/cli/uninstall/uninstall.py` & `helm-hawk-0.0.2/cli/uninstall/uninstall.py`

 * *Files identical despite different names*

### Comparing `helm-hawk-0.0.1/cli/utils/helm.py` & `helm-hawk-0.0.2/cli/utils/helm.py`

 * *Files identical despite different names*

### Comparing `helm-hawk-0.0.1/cli/utils/kubectl.py` & `helm-hawk-0.0.2/cli/utils/kubectl.py`

 * *Files identical despite different names*

### Comparing `helm-hawk-0.0.1/helm_hawk.egg-info/PKG-INFO` & `helm-hawk-0.0.2/helm_hawk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helm-hawk
-Version: 0.0.1
+Version: 0.0.2
 Author: Ankit Singh
 Author-email: as8356047@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `helm-hawk-0.0.1/helm_hawk.egg-info/SOURCES.txt` & `helm-hawk-0.0.2/helm_hawk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `helm-hawk-0.0.1/setup.py` & `helm-hawk-0.0.2/setup.py`

 * *Files identical despite different names*

