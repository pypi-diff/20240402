# Comparing `tmp/whispers-2.2.0.tar.gz` & `tmp/whispers-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whispers-2.2.0.tar", last modified: Tue Oct 24 20:33:58 2023, max compression
+gzip compressed data, was "whispers-2.2.1.tar", last modified: Tue Apr  2 20:00:51 2024, max compression
```

## Comparing `whispers-2.2.0.tar` & `whispers-2.2.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 20:33:58.198267 whispers-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2023-10-24 20:31:53.000000 whispers-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-10-24 20:31:53.000000 whispers-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10729 2023-10-24 20:33:58.198267 whispers-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2023-10-24 20:31:53.000000 whispers-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      122 2023-10-24 20:31:53.000000 whispers-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      546 2023-10-24 20:33:58.202267 whispers-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2023-10-24 20:31:53.000000 whispers-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 20:33:58.194267 whispers-2.2.0/whispers/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 20:33:58.194267 whispers-2.2.0/whispers/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/core/args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4876 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/core/pairs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/core/rules.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/core/scope.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/core/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6904 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 20:33:58.194267 whispers-2.2.0/whispers/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/models/appconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/models/pair.py
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/models/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 20:33:58.198267 whispers-2.2.0/whispers/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/plugins/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/plugins/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/plugins/dockercfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/plugins/dockerfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/plugins/gradle.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/plugins/html.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/plugins/htpasswd.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/plugins/jproperties.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/plugins/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/plugins/npmrc.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/plugins/pip.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/plugins/plaintext.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/plugins/pypirc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5241 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/plugins/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/plugins/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/plugins/traverse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/plugins/xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/plugins/yml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 20:33:58.198267 whispers-2.2.0/whispers/rules/
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/rules/files.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/rules/infra.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/rules/keys.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/rules/misc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      520 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/rules/passwords.yml
--rw-r--r--   0 runner    (1001) docker     (127)      622 2023-10-24 20:31:53.000000 whispers-2.2.0/whispers/rules/python.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 20:33:58.194267 whispers-2.2.0/whispers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10729 2023-10-24 20:33:58.000000 whispers-2.2.0/whispers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2023-10-24 20:33:58.000000 whispers-2.2.0/whispers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-24 20:33:58.000000 whispers-2.2.0/whispers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-10-24 20:33:58.000000 whispers-2.2.0/whispers.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      256 2023-10-24 20:33:58.000000 whispers-2.2.0/whispers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-10-24 20:33:58.000000 whispers-2.2.0/whispers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:00:51.193823 whispers-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-02 19:59:42.000000 whispers-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 19:59:42.000000 whispers-2.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-04-02 20:00:51.193823 whispers-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10719 2024-04-02 19:59:42.000000 whispers-2.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-02 19:59:42.000000 whispers-2.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-02 20:00:51.193823 whispers-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-02 19:59:42.000000 whispers-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:00:51.185823 whispers-2.2.1/whispers/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:00:51.185823 whispers-2.2.1/whispers/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/core/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4876 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/core/pairs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/core/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/core/scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/core/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:00:51.189823 whispers-2.2.1/whispers/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/models/appconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/models/pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/models/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:00:51.189823 whispers-2.2.1/whispers/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/plugins/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/plugins/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/plugins/dockercfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/plugins/dockerfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/plugins/gradle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/plugins/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/plugins/htpasswd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/plugins/jproperties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/plugins/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/plugins/npmrc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/plugins/pip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/plugins/plaintext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/plugins/pypirc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/plugins/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/plugins/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/plugins/traverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/plugins/xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/plugins/yml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:00:51.193823 whispers-2.2.1/whispers/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/rules/files.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/rules/infra.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/rules/keys.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/rules/misc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/rules/passwords.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-02 19:59:42.000000 whispers-2.2.1/whispers/rules/python.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:00:51.185823 whispers-2.2.1/whispers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-04-02 20:00:51.000000 whispers-2.2.1/whispers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-02 20:00:51.000000 whispers-2.2.1/whispers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 20:00:51.000000 whispers-2.2.1/whispers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-02 20:00:51.000000 whispers-2.2.1/whispers.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-02 20:00:51.000000 whispers-2.2.1/whispers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 20:00:51.000000 whispers-2.2.1/whispers.egg-info/top_level.txt
```

### Comparing `whispers-2.2.0/LICENSE` & `whispers-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `whispers-2.2.0/PKG-INFO` & `whispers-2.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whispers
-Version: 2.2.0
+Version: 2.2.1
 Summary: Identify secrets in static structured text
 Home-page: https://github.com/adeptex/whispers
 Author: Artëm Tsvetkov
 Author-email: adeptex@users.noreply.github.com
 Platform: any
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/markdown
@@ -172,40 +172,43 @@
 
 * File path specifications are lists of globs
 * Key and value specifications are lists of regular expressions 
 * Rule specifications are lists of rule IDs or inline rule definitions
 * Everything else is a list of strings
 
 
-### Simple examples
+### Config examples
 
 Exclude all log files:
 
 ```yaml
 exclude:
   files:
     - .*\.log
 ```
 
-Only scan for  level findings in .npmrc files, excluding a known testing value:
+Only scan for *High* level findings in .npmrc files, excluding a known testing value:
 
 ```yaml
 include:
   files:
     - "**/*.npmrc"
   severity:
     - High
 
 exclude:
   values: 
     - ^token_for_testing$
 ```
 
 
-### General config format
+### Config format
+
+See [whispers/models/appconfig.py](https://github.com/adeptex/whispers/blob/master/whispers/models/appconfig.py) for available fields and their defaults.
+
 
 ```yaml
 include:
   files:
     - "**/*.yml"  # glob
   rules:
     - password
@@ -278,15 +281,17 @@
 
 Rules specify the actual things that should be pulled out from key-value pairs. There are several common ones that come built-in, such as AWS keys and passwords, but the tool is made to be easily expandable with new rules.
 
 - Custom rules can be defined in the main config file under `rules:` key
 - Custom rules can be added to [whispers/rules](https://github.com/adeptex/whispers/blob/master/whispers/rules/) directory
 
 
-### General rule format
+### Rule format
+
+See [whispers/models/rule.py](https://github.com/adeptex/whispers/blob/master/whispers/models/rule.py) for available fields and their defaults.
 
 ```yaml
 - id: rule-id                 # unique rule name
   group: rule-group           # rule group name
   description: Values formatted like AWS Session Token
   message: AWS Session Token  # report will show this message
   severity: Critical           # one of Critical, High, Medium, Low, Info
@@ -298,14 +303,15 @@
   value:                      # specify value format
     regex: ^(?=.*[a-z])(?=.*[A-Z])[A-Za-z0-9\+\/]{270,450}$
     ignorecase: False         # case-sensitive matching
     minlen: 270               # value is at least this long
     isBase64: True            # value is base64-encoded
     isAscii: False            # value is binary data when decoded
     isUri: False              # value is not formatted like a URI
+    isFile: False             # value doesn't match filenames
 
   similar: 0.35               # maximum allowed Jaro-Winkler similarity
                               # between key and value (1.0 being exactly the same)
 ```
 
 
 ## Plugins
@@ -329,14 +335,14 @@
 
 ## Development
 
 ```bash
 git clone https://github.com/adeptex/whispers
 cd whispers
 make install-dev
-make test
+make format test
 ```
 
 
 ## License
 
 [BSD 3-Clause License](https://github.com/adeptex/whispers/blob/master/LICENSE)
```

### Comparing `whispers-2.2.0/README.md` & `whispers-2.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -159,40 +159,43 @@
 
 * File path specifications are lists of globs
 * Key and value specifications are lists of regular expressions 
 * Rule specifications are lists of rule IDs or inline rule definitions
 * Everything else is a list of strings
 
 
-### Simple examples
+### Config examples
 
 Exclude all log files:
 
 ```yaml
 exclude:
   files:
     - .*\.log
 ```
 
-Only scan for  level findings in .npmrc files, excluding a known testing value:
+Only scan for *High* level findings in .npmrc files, excluding a known testing value:
 
 ```yaml
 include:
   files:
     - "**/*.npmrc"
   severity:
     - High
 
 exclude:
   values: 
     - ^token_for_testing$
 ```
 
 
-### General config format
+### Config format
+
+See [whispers/models/appconfig.py](https://github.com/adeptex/whispers/blob/master/whispers/models/appconfig.py) for available fields and their defaults.
+
 
 ```yaml
 include:
   files:
     - "**/*.yml"  # glob
   rules:
     - password
@@ -265,15 +268,17 @@
 
 Rules specify the actual things that should be pulled out from key-value pairs. There are several common ones that come built-in, such as AWS keys and passwords, but the tool is made to be easily expandable with new rules.
 
 - Custom rules can be defined in the main config file under `rules:` key
 - Custom rules can be added to [whispers/rules](https://github.com/adeptex/whispers/blob/master/whispers/rules/) directory
 
 
-### General rule format
+### Rule format
+
+See [whispers/models/rule.py](https://github.com/adeptex/whispers/blob/master/whispers/models/rule.py) for available fields and their defaults.
 
 ```yaml
 - id: rule-id                 # unique rule name
   group: rule-group           # rule group name
   description: Values formatted like AWS Session Token
   message: AWS Session Token  # report will show this message
   severity: Critical           # one of Critical, High, Medium, Low, Info
@@ -285,14 +290,15 @@
   value:                      # specify value format
     regex: ^(?=.*[a-z])(?=.*[A-Z])[A-Za-z0-9\+\/]{270,450}$
     ignorecase: False         # case-sensitive matching
     minlen: 270               # value is at least this long
     isBase64: True            # value is base64-encoded
     isAscii: False            # value is binary data when decoded
     isUri: False              # value is not formatted like a URI
+    isFile: False             # value doesn't match filenames
 
   similar: 0.35               # maximum allowed Jaro-Winkler similarity
                               # between key and value (1.0 being exactly the same)
 ```
 
 
 ## Plugins
@@ -316,14 +322,14 @@
 
 ## Development
 
 ```bash
 git clone https://github.com/adeptex/whispers
 cd whispers
 make install-dev
-make test
+make format test
 ```
 
 
 ## License
 
 [BSD 3-Clause License](https://github.com/adeptex/whispers/blob/master/LICENSE)
```

### Comparing `whispers-2.2.0/setup.cfg` & `whispers-2.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `whispers-2.2.0/setup.py` & `whispers-2.2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,16 @@
     "lxml",
     "pyyaml",
 ]
 
 dev_requires = [
     "autoflake~=1.4",
     "autopep8~=1.7",
-    "black~=22.8",
+    "black==22.8; python_version <= '3.6'",
+    "black~=24.3; python_version > '3.6'",
     "build~=0.8",
     "coverage~=4.5",
     "coverage-badge~=1.0",
     "flake8~=5.0",
     "isort~=5.9",
     "pytest~=7.0",
     "pytest-mock~=3.6",
```

### Comparing `whispers-2.2.0/whispers/__version__.py` & `whispers-2.2.1/whispers/__version__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-VERSION = (2, 2, 0)
+VERSION = (2, 2, 1)
 
 __version__ = ".".join(map(str, VERSION))
 
 __whispers__ = """
  █     █░ ██░ ██  ██▓  ██████  ██▓███  ▓█████  ██▀███    ██████ 
 ▓█░ █ ░█░▓██░ ██▒▓██▒▒██    ▒ ▓██░  ██▒▓█   ▀ ▓██ ▒ ██▒▒██    ▒ 
 ▒█░ █ ░█ ▒██▀▀██░▒██▒░ ▓██▄   ▓██░ ██▓▒▒███   ▓██ ░▄█ ▒░ ▓██▄
```

### Comparing `whispers-2.2.0/whispers/core/args.py` & `whispers-2.2.1/whispers/core/args.py`

 * *Files identical despite different names*

### Comparing `whispers-2.2.0/whispers/core/config.py` & `whispers-2.2.1/whispers/core/config.py`

 * *Files identical despite different names*

### Comparing `whispers-2.2.0/whispers/core/constants.py` & `whispers-2.2.1/whispers/core/constants.py`

 * *Files identical despite different names*

### Comparing `whispers-2.2.0/whispers/core/pairs.py` & `whispers-2.2.1/whispers/core/pairs.py`

 * *Files identical despite different names*

### Comparing `whispers-2.2.0/whispers/core/rules.py` & `whispers-2.2.1/whispers/core/rules.py`

 * *Files identical despite different names*

### Comparing `whispers-2.2.0/whispers/core/scope.py` & `whispers-2.2.1/whispers/core/scope.py`

 * *Files identical despite different names*

### Comparing `whispers-2.2.0/whispers/core/secrets.py` & `whispers-2.2.1/whispers/core/secrets.py`

 * *Files identical despite different names*

### Comparing `whispers-2.2.0/whispers/core/utils.py` & `whispers-2.2.1/whispers/core/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 from luhn import verify as luhn_verify
 from yaml import safe_load, safe_load_all
 
 from whispers.core.constants import DEFAULT_PATH, REGEX_ENVVAR, REGEX_IAC, REGEX_PATH, REGEX_URI
 from whispers.models.pair import KeyValuePair
 
 
-def global_exception_handler(file: Union[str, Path], data: str):
+def global_exception_handler(file: Union[str, Path], data: str = ""):
     """Global Exception Handler"""
-    logging.exception(f"Failed parsing file '{str(file)}' with {data}")
+    logging.debug(f"Failed parsing file '{str(file)}'", exc_info=True)
 
 
 def load_regex(regex: str, flags: Optional[re.RegexFlag] = 0) -> Pattern:
     """Try to compile a regex statement"""
     try:
         return re.compile(regex, flags=flags)
```

### Comparing `whispers-2.2.0/whispers/main.py` & `whispers-2.2.1/whispers/main.py`

 * *Files identical despite different names*

### Comparing `whispers-2.2.0/whispers/models/appconfig.py` & `whispers-2.2.1/whispers/models/appconfig.py`

 * *Files identical despite different names*

### Comparing `whispers-2.2.0/whispers/models/pair.py` & `whispers-2.2.1/whispers/models/pair.py`

 * *Files identical despite different names*

### Comparing `whispers-2.2.0/whispers/models/rule.py` & `whispers-2.2.1/whispers/models/rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     regex: Optional[Pattern] = None
     ignorecase: Optional[bool] = False
     minlen: Optional[int] = 0
     isBase64: Optional[bool] = None
     isAscii: Optional[bool] = None
     isUri: Optional[bool] = None
     isLuhn: Optional[bool] = None
+    isFile: Optional[bool] = False
 
     def __post_init__(self) -> None:
         """Compile regex with explicit ignorecase"""
         if self.regex is None:
             return None
 
         flags = re.IGNORECASE if self.ignorecase else 0
@@ -82,15 +83,15 @@
         if not value:
             raise IndexError(f"Missing rule '{idx}' specification: '{rule}'")
 
         return value
 
     @staticmethod
     def _get_spec(idx: str, rule: Dict) -> Optional[Specification]:
-        """Get an optional rule specification"""
+        """Get an optional rule specification."""
         spec = rule.get(idx, False)
         if not spec:
             return None
 
         if isinstance(spec, dict):
             return Specification(**spec)
 
@@ -102,8 +103,11 @@
 
         if self.value and not self.value.matches(pair.value):
             return False
 
         if is_similar(pair.key, pair.value, self.similar):
             return False
 
+        if pair.key == "file" and not self.value.isFile:
+            return False
+
         return True
```

### Comparing `whispers-2.2.0/whispers/plugins/common.py` & `whispers-2.2.1/whispers/plugins/common.py`

 * *Files identical despite different names*

### Comparing `whispers-2.2.0/whispers/plugins/config.py` & `whispers-2.2.1/whispers/plugins/config.py`

 * *Files identical despite different names*

### Comparing `whispers-2.2.0/whispers/plugins/dockercfg.py` & `whispers-2.2.1/whispers/plugins/dockercfg.py`

 * *Files identical despite different names*

### Comparing `whispers-2.2.0/whispers/plugins/dockerfile.py` & `whispers-2.2.1/whispers/plugins/dockerfile.py`

 * *Files identical despite different names*

### Comparing `whispers-2.2.0/whispers/plugins/html.py` & `whispers-2.2.1/whispers/plugins/html.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 from whispers.models.pair import KeyValuePair
 
 
 class Html:
     def pairs(self, filepath: Path) -> Iterator[KeyValuePair]:
         soup = BeautifulSoup(filepath.read_text(), "lxml")
         key = "comment"
-        for comment in soup.find_all(text=lambda text: isinstance(text, Comment)):
+        for comment in soup.find_all(string=lambda text: isinstance(text, Comment)):
             comment = truncate_all_space(comment.extract()).strip()
             if comment:
                 yield KeyValuePair(key, comment, [key])
```

### Comparing `whispers-2.2.0/whispers/plugins/htpasswd.py` & `whispers-2.2.1/whispers/plugins/htpasswd.py`

 * *Files identical despite different names*

### Comparing `whispers-2.2.0/whispers/plugins/json.py` & `whispers-2.2.1/whispers/plugins/yml.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,56 @@
-import json
 import re
 from pathlib import Path
 from typing import Iterator
 
+import yaml
+from yaml.parser import ParserError
+from yaml.resolver import Resolver
+
 from whispers.core.utils import global_exception_handler
 from whispers.models.pair import KeyValuePair
 from whispers.plugins.traverse import StructuredDocument
 
 
-class Json(StructuredDocument):
+class Yml(StructuredDocument):
+    def __init__(self):
+        super().__init__()
+
+        # Remove resolvers for on/off/yes/no
+        list(map(lambda idx: Resolver.yaml_implicit_resolvers.pop(idx, None), "OoYyNn"))
+
     def pairs(self, filepath: Path) -> Iterator[KeyValuePair]:
+        def _constructor(loader, tag_suffix, node):
+            """This is needed to parse IaC syntax"""
+            ret = loader.construct_scalar(node)
+            return f"{tag_suffix} {ret}"
+
         """
-        Convert custom JSON to parsable JSON
-        - Remove lines that start with // comments
-        - Strip // comments from the end the line
+        Convert custom YAML to parsable YAML
+        - Skip ---
+        - Quote unquoted values such as {{ placeholder }}
+        - Remove text between <% %> and {% %}
+        - Remove comments that start with #
         """
+        regex_unquoted = re.compile(r".+(\[)?\{\{.*\}\}(\])?")
         document = ""
+
         for line in filepath.open("r").readlines():
-            if line.startswith("//"):
+            if line.startswith("---"):
                 continue
-            line = re.sub(r" // ?.*$", "", line)
+
+            if regex_unquoted.match(line):
+                line = line.replace("{{", "'{{").replace("}}", "}}'")
+
             document += line
 
-        # Load converted JSON
+        document = re.sub(r"[<{]%.*?%[}>]", "", document, flags=re.MULTILINE | re.DOTALL)
+        document = re.sub(r"^#.*$", "", document)
+
+        # Load converted YAML
         try:
-            document = json.loads(document)
-            yield from self.traverse(document)
-        except Exception:
+            yaml.add_multi_constructor("", _constructor, Loader=yaml.SafeLoader)
+            code = yaml.safe_load(document)
+            yield from self.traverse(code)
+
+        except ParserError:
             global_exception_handler(filepath.as_posix(), document)
```

### Comparing `whispers-2.2.0/whispers/plugins/pip.py` & `whispers-2.2.1/whispers/plugins/pip.py`

 * *Files identical despite different names*

### Comparing `whispers-2.2.0/whispers/plugins/plaintext.py` & `whispers-2.2.1/whispers/plugins/plaintext.py`

 * *Files identical despite different names*

### Comparing `whispers-2.2.0/whispers/plugins/python.py` & `whispers-2.2.1/whispers/plugins/python.py`

 * *Files identical despite different names*

### Comparing `whispers-2.2.0/whispers/plugins/shell.py` & `whispers-2.2.1/whispers/plugins/shell.py`

 * *Files identical despite different names*

### Comparing `whispers-2.2.0/whispers/plugins/traverse.py` & `whispers-2.2.1/whispers/plugins/traverse.py`

 * *Files identical despite different names*

### Comparing `whispers-2.2.0/whispers/plugins/xml.py` & `whispers-2.2.1/whispers/plugins/xml.py`

 * *Files identical despite different names*

### Comparing `whispers-2.2.0/whispers/rules/files.yml` & `whispers-2.2.1/whispers/rules/files.yml`

 * *Files 8% similar despite different names*

```diff
@@ -27,7 +27,8 @@
       (robomongo|heroku|remote-sync|deployment-config|docker/config)\\.json|\
       otr\\.private_key|journal\\.txt|\\.(exports|functions|extra)|\
       Favorites\\.plist|configuration\\.user\\.xpl|\
       mongoid\\.ya?ml|salesforce\\.js|\
       ventrilo(-|_)srv.ini|muttrc|trc|ovpn|dayone|tugboat|esmtprc|ftpconfig|\
       backup|back|bck|~1)$"
     ignorecase: True
+    isFile: True
```

### Comparing `whispers-2.2.0/whispers/rules/infra.yml` & `whispers-2.2.1/whispers/rules/infra.yml`

 * *Files identical despite different names*

### Comparing `whispers-2.2.0/whispers/rules/keys.yml` & `whispers-2.2.1/whispers/rules/keys.yml`

 * *Files identical despite different names*

### Comparing `whispers-2.2.0/whispers/rules/misc.yml` & `whispers-2.2.1/whispers/rules/misc.yml`

 * *Files identical despite different names*

### Comparing `whispers-2.2.0/whispers/rules/passwords.yml` & `whispers-2.2.1/whispers/rules/passwords.yml`

 * *Files identical despite different names*

### Comparing `whispers-2.2.0/whispers/rules/python.yml` & `whispers-2.2.1/whispers/rules/python.yml`

 * *Files identical despite different names*

### Comparing `whispers-2.2.0/whispers.egg-info/PKG-INFO` & `whispers-2.2.1/whispers.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whispers
-Version: 2.2.0
+Version: 2.2.1
 Summary: Identify secrets in static structured text
 Home-page: https://github.com/adeptex/whispers
 Author: Artëm Tsvetkov
 Author-email: adeptex@users.noreply.github.com
 Platform: any
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/markdown
@@ -172,40 +172,43 @@
 
 * File path specifications are lists of globs
 * Key and value specifications are lists of regular expressions 
 * Rule specifications are lists of rule IDs or inline rule definitions
 * Everything else is a list of strings
 
 
-### Simple examples
+### Config examples
 
 Exclude all log files:
 
 ```yaml
 exclude:
   files:
     - .*\.log
 ```
 
-Only scan for  level findings in .npmrc files, excluding a known testing value:
+Only scan for *High* level findings in .npmrc files, excluding a known testing value:
 
 ```yaml
 include:
   files:
     - "**/*.npmrc"
   severity:
     - High
 
 exclude:
   values: 
     - ^token_for_testing$
 ```
 
 
-### General config format
+### Config format
+
+See [whispers/models/appconfig.py](https://github.com/adeptex/whispers/blob/master/whispers/models/appconfig.py) for available fields and their defaults.
+
 
 ```yaml
 include:
   files:
     - "**/*.yml"  # glob
   rules:
     - password
@@ -278,15 +281,17 @@
 
 Rules specify the actual things that should be pulled out from key-value pairs. There are several common ones that come built-in, such as AWS keys and passwords, but the tool is made to be easily expandable with new rules.
 
 - Custom rules can be defined in the main config file under `rules:` key
 - Custom rules can be added to [whispers/rules](https://github.com/adeptex/whispers/blob/master/whispers/rules/) directory
 
 
-### General rule format
+### Rule format
+
+See [whispers/models/rule.py](https://github.com/adeptex/whispers/blob/master/whispers/models/rule.py) for available fields and their defaults.
 
 ```yaml
 - id: rule-id                 # unique rule name
   group: rule-group           # rule group name
   description: Values formatted like AWS Session Token
   message: AWS Session Token  # report will show this message
   severity: Critical           # one of Critical, High, Medium, Low, Info
@@ -298,14 +303,15 @@
   value:                      # specify value format
     regex: ^(?=.*[a-z])(?=.*[A-Z])[A-Za-z0-9\+\/]{270,450}$
     ignorecase: False         # case-sensitive matching
     minlen: 270               # value is at least this long
     isBase64: True            # value is base64-encoded
     isAscii: False            # value is binary data when decoded
     isUri: False              # value is not formatted like a URI
+    isFile: False             # value doesn't match filenames
 
   similar: 0.35               # maximum allowed Jaro-Winkler similarity
                               # between key and value (1.0 being exactly the same)
 ```
 
 
 ## Plugins
@@ -329,14 +335,14 @@
 
 ## Development
 
 ```bash
 git clone https://github.com/adeptex/whispers
 cd whispers
 make install-dev
-make test
+make format test
 ```
 
 
 ## License
 
 [BSD 3-Clause License](https://github.com/adeptex/whispers/blob/master/LICENSE)
```

### Comparing `whispers-2.2.0/whispers.egg-info/SOURCES.txt` & `whispers-2.2.1/whispers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

