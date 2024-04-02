# Comparing `tmp/devopsdriver-0.1.32.tar.gz` & `tmp/devopsdriver-0.1.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devopsdriver-0.1.32.tar", last modified: Mon Apr  1 03:27:04 2024, max compression
+gzip compressed data, was "devopsdriver-0.1.34.tar", last modified: Tue Apr  2 00:28:54 2024, max compression
```

## Comparing `devopsdriver-0.1.32.tar` & `devopsdriver-0.1.34.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-01 03:27:04.119831 devopsdriver-0.1.32/
--rw-r--r--   0 marcp      (501) staff       (20)     1211 2024-03-30 20:53:59.000000 devopsdriver-0.1.32/LICENSE
--rw-r--r--   0 marcp      (501) staff       (20)     4738 2024-04-01 03:27:04.119609 devopsdriver-0.1.32/PKG-INFO
--rw-r--r--   0 marcp      (501) staff       (20)     2271 2024-04-01 02:36:01.000000 devopsdriver-0.1.32/README.md
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-01 03:27:04.117931 devopsdriver-0.1.32/devopsdriver/
--rw-r--r--   0 marcp      (501) staff       (20)       87 2024-04-01 03:25:54.000000 devopsdriver-0.1.32/devopsdriver/__init__.py
--rw-r--r--   0 marcp      (501) staff       (20)    10860 2024-04-01 02:42:14.000000 devopsdriver-0.1.32/devopsdriver/settings.py
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-01 03:27:04.119382 devopsdriver-0.1.32/devopsdriver.egg-info/
--rw-r--r--   0 marcp      (501) staff       (20)     4738 2024-04-01 03:27:04.000000 devopsdriver-0.1.32/devopsdriver.egg-info/PKG-INFO
--rw-r--r--   0 marcp      (501) staff       (20)      284 2024-04-01 03:27:04.000000 devopsdriver-0.1.32/devopsdriver.egg-info/SOURCES.txt
--rw-r--r--   0 marcp      (501) staff       (20)        1 2024-04-01 03:27:04.000000 devopsdriver-0.1.32/devopsdriver.egg-info/dependency_links.txt
--rw-r--r--   0 marcp      (501) staff       (20)       14 2024-04-01 03:27:04.000000 devopsdriver-0.1.32/devopsdriver.egg-info/requires.txt
--rw-r--r--   0 marcp      (501) staff       (20)       13 2024-04-01 03:27:04.000000 devopsdriver-0.1.32/devopsdriver.egg-info/top_level.txt
--rw-r--r--   0 marcp      (501) staff       (20)     1205 2024-04-01 02:18:29.000000 devopsdriver-0.1.32/pyproject.toml
--rw-r--r--   0 marcp      (501) staff       (20)       38 2024-04-01 03:27:04.119875 devopsdriver-0.1.32/setup.cfg
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-01 03:27:04.119188 devopsdriver-0.1.32/tests/
--rw-r--r--   0 marcp      (501) staff       (20)    10889 2024-04-01 02:42:56.000000 devopsdriver-0.1.32/tests/test_settings.py
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-02 00:28:54.710596 devopsdriver-0.1.34/
+-rw-r--r--   0 marcp      (501) staff       (20)     1211 2024-03-30 20:53:59.000000 devopsdriver-0.1.34/LICENSE
+-rw-r--r--   0 marcp      (501) staff       (20)     4927 2024-04-02 00:28:54.710327 devopsdriver-0.1.34/PKG-INFO
+-rw-r--r--   0 marcp      (501) staff       (20)     2429 2024-04-02 00:28:23.000000 devopsdriver-0.1.34/README.md
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-02 00:28:54.708654 devopsdriver-0.1.34/devopsdriver/
+-rw-r--r--   0 marcp      (501) staff       (20)       87 2024-04-02 00:28:09.000000 devopsdriver-0.1.34/devopsdriver/__init__.py
+-rw-r--r--   0 marcp      (501) staff       (20)    12690 2024-04-02 00:17:57.000000 devopsdriver-0.1.34/devopsdriver/settings.py
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-02 00:28:54.710075 devopsdriver-0.1.34/devopsdriver.egg-info/
+-rw-r--r--   0 marcp      (501) staff       (20)     4927 2024-04-02 00:28:54.000000 devopsdriver-0.1.34/devopsdriver.egg-info/PKG-INFO
+-rw-r--r--   0 marcp      (501) staff       (20)      284 2024-04-02 00:28:54.000000 devopsdriver-0.1.34/devopsdriver.egg-info/SOURCES.txt
+-rw-r--r--   0 marcp      (501) staff       (20)        1 2024-04-02 00:28:54.000000 devopsdriver-0.1.34/devopsdriver.egg-info/dependency_links.txt
+-rw-r--r--   0 marcp      (501) staff       (20)       30 2024-04-02 00:28:54.000000 devopsdriver-0.1.34/devopsdriver.egg-info/requires.txt
+-rw-r--r--   0 marcp      (501) staff       (20)       13 2024-04-02 00:28:54.000000 devopsdriver-0.1.34/devopsdriver.egg-info/top_level.txt
+-rw-r--r--   0 marcp      (501) staff       (20)     1226 2024-04-02 00:17:57.000000 devopsdriver-0.1.34/pyproject.toml
+-rw-r--r--   0 marcp      (501) staff       (20)       38 2024-04-02 00:28:54.710653 devopsdriver-0.1.34/setup.cfg
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-02 00:28:54.709614 devopsdriver-0.1.34/tests/
+-rw-r--r--   0 marcp      (501) staff       (20)    12527 2024-04-02 00:17:57.000000 devopsdriver-0.1.34/tests/test_settings.py
```

### Comparing `devopsdriver-0.1.32/LICENSE` & `devopsdriver-0.1.34/LICENSE`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.32/PKG-INFO` & `devopsdriver-0.1.34/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devopsdriver
-Version: 0.1.32
+Version: 0.1.34
 Summary: DevOps tools
 Author-email: Marc Page <marcallenpage@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -39,20 +39,22 @@
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development
-Requires-Python: >=3.12
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyYAML==6.0.1
+Requires-Dist: keyring==25.0.0
 
 ![status sheild](https://img.shields.io/static/v1?label=status&message=starting...&color=inactive&style=plastic)
+[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.34&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.34/)
 [![GitHub](https://img.shields.io/github/license/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver?tab=Unlicense-1-ov-file#readme)
 [![commit sheild](https://img.shields.io/github/last-commit/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![activity sheild](https://img.shields.io/github/commit-activity/m/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![GitHub top language](https://img.shields.io/github/languages/top/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver)
 [![size sheild](https://img.shields.io/github/languages/code-size/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver)
 
 [![example workflow](https://github.com/marcpage/devops-driver/actions/workflows/pr.yml/badge.svg)](https://github.com/marcpage/devops-driver/actions/workflows/pr.yml)
```

### Comparing `devopsdriver-0.1.32/README.md` & `devopsdriver-0.1.34/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 ![status sheild](https://img.shields.io/static/v1?label=status&message=starting...&color=inactive&style=plastic)
+[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.34&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.34/)
 [![GitHub](https://img.shields.io/github/license/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver?tab=Unlicense-1-ov-file#readme)
 [![commit sheild](https://img.shields.io/github/last-commit/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![activity sheild](https://img.shields.io/github/commit-activity/m/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![GitHub top language](https://img.shields.io/github/languages/top/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver)
 [![size sheild](https://img.shields.io/github/languages/code-size/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver)
 
 [![example workflow](https://github.com/marcpage/devops-driver/actions/workflows/pr.yml/badge.svg)](https://github.com/marcpage/devops-driver/actions/workflows/pr.yml)
```

### Comparing `devopsdriver-0.1.32/devopsdriver/settings.py` & `devopsdriver-0.1.34/devopsdriver/settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -78,25 +78,29 @@
 
 from json import load
 from os.path import dirname, basename, splitext, join
 from os import environ as os_environ, makedirs as os_makedirs
 from re import compile as regex
 from platform import system as os_system
 from sys import argv as sys_argv
+from getpass import getpass as os_getpass
 
 from yaml import safe_load
-
+from keyring import get_password, set_password
 
 # for testing
 ENVIRON = os_environ
 ARGV = sys_argv
 SYSTEM = os_system
 MAKEDIRS = os_makedirs
 SHARED = "devopsdriver"
 PRINT = print
+GET_PASSWORD = get_password
+SET_PASSWORD = set_password
+GET_PASS = os_getpass
 
 
 def load_json(path: str) -> dict:
     """Load a dictionary from a JSON file
 
     Args:
         path (str): Path to JSON file
@@ -150,54 +154,66 @@
         self.overrides = settings
         directories = [dirname(file), *directories, Settings.__preferences_dir()]
         search_info = Settings.__all_paths(file, directories)
         self.search_files = [join(d, n + e) for e, n, d, _ in search_info]
         self.settings = Settings.__find_all_settings(search_info)
         self.opts = {}
         self.environ = {}
+        self.secrets = {}
+
+    def __bypass(self, key: str, name: str, store: dict):
+        if name is None:
+            for setting_key, store_name in self.settings.get(key, {}).items():
+                store[setting_key] = store_name
+            return self
+
+        store[key] = name
+        return self
+
+    def key(self, key: str, name: str = None):
+        """Sets a keychain name to map to a settings value.
+
+        Args:
+            key (str): The settings key it maps to, dotted for inside dictionary
+            name (str): Name of the keychain key
+                            If name is not specified, the key is a settings value
+                            to lookup up the mappings for keys to switches
+
+        Returns:
+            Settings: Returns self so you can chain calls
+        """
+        return self.__bypass(key, name, self.secrets)
 
     def cli(self, key: str, name: str = None):
         """Sets a command line switch to map to a settings value.
 
         Args:
             key (str): The settings key it maps to, dotted for inside dictionary
             name (str): Name of the command line switch, eg '-p' or '--path'
                             If name is not specified, the key is a settings value
                             to lookup up the mappings for keys to switches
 
         Returns:
             Settings: Returns self so you can chain calls
         """
-        if name is None:
-            for setting_key, env_name in self.settings.get(key, {}).items():
-                self.opts[setting_key] = env_name
-            return self
-
-        self.opts[key] = name
-        return self
+        return self.__bypass(key, name, self.opts)
 
     def env(self, key: str, name: str = None):
         """Sets an environment variable to map to a settings value.
 
         Args:
             key (str): The settings key it maps to, dotted for inside dictionary
             name (str): Name of the environment variable
                             If name is not specified, the key is a settings value
                             to lookup up the mappings for keys to environment names
 
         Returns:
             Settings: Returns self so you can chain calls
         """
-        if name is None:
-            for setting_key, cli_name in self.settings.get(key, {}).items():
-                self.environ[setting_key] = cli_name
-            return self
-
-        self.environ[key] = name
-        return self
+        return self.__bypass(key, name, self.environ)
 
     @staticmethod
     def __patch_instance(key: str) -> str:
         for env_key, value in ENVIRON.items():
             if env_key.lower() == key.lower():
                 return value
 
@@ -208,14 +224,31 @@
         if isinstance(value, str):
             return Settings.ENV_VAR_PATTERN.sub(
                 lambda m: Settings.__patch_instance(m.group(1)), value
             )
 
         return value
 
+    @staticmethod
+    def split_key(key: str) -> tuple[str, str]:
+        """Splits a keychain name into service and name
+
+        Args:
+            key (str): If there is a / then it is service/name
+                        otherwise it is "system"/name
+
+        Returns:
+            tuple[str, str]: The service and name
+        """
+        parts = key.split("/", 1)
+        assert len(parts) in {1, 2}, parts
+        service = parts[0] if len(parts) == 2 else "system"
+        secret_name = parts[1] if len(parts) == 2 else parts[0]
+        return (service, secret_name)
+
     def __lookup(self, key: str, check: bool, default: any = None) -> any:
         # Settings passed in override everything
         if key in self.overrides:
             return True if check else self.overrides[key]
 
         # Settings on the command line take next precedence
         if key in self.opts:
@@ -225,14 +258,21 @@
 
         # Settings in the environment are next
         if key in self.environ:
             for e_key in ENVIRON:
                 if e_key.lower() == self.environ[key].lower():
                     return True if check else ENVIRON[e_key]
 
+        # Settings in the keychain are next
+        if key in self.secrets:
+            value = GET_PASSWORD(*Settings.split_key(self.secrets[key]))
+
+            if value is not None:
+                return True if check else value
+
         # Last check the files for settings
         keys = key.split(".")
         level = self.settings
 
         for key_part in keys[:-1]:
             level = level.get(key_part, {})
 
@@ -314,15 +354,27 @@
             Settings.__merge(settings, contents)
 
         return settings
 
 
 def main() -> None:
     """Get settings values"""
-    settings = Settings(__file__, dirname(dirname(__file__)))
+    settings = Settings(__file__, dirname(dirname(__file__))).key("secrets")
+
+    args = list(ARGV[1:])
+
+    if "--set_secrets" in args:
+        args.remove("--set_secrets")
+
+        for secret, key in settings.secrets.items():
+            if not settings.has(secret):
+                value = GET_PASS(f"{secret} ({key}): ")
+
+                if value:
+                    SET_PASSWORD(*Settings.split_key(key), value)
 
-    for arg in ARGV[1:]:
+    for arg in args:
         PRINT(settings.get(arg))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `devopsdriver-0.1.32/devopsdriver.egg-info/PKG-INFO` & `devopsdriver-0.1.34/devopsdriver.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devopsdriver
-Version: 0.1.32
+Version: 0.1.34
 Summary: DevOps tools
 Author-email: Marc Page <marcallenpage@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -39,20 +39,22 @@
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development
-Requires-Python: >=3.12
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyYAML==6.0.1
+Requires-Dist: keyring==25.0.0
 
 ![status sheild](https://img.shields.io/static/v1?label=status&message=starting...&color=inactive&style=plastic)
+[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.34&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.34/)
 [![GitHub](https://img.shields.io/github/license/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver?tab=Unlicense-1-ov-file#readme)
 [![commit sheild](https://img.shields.io/github/last-commit/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![activity sheild](https://img.shields.io/github/commit-activity/m/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![GitHub top language](https://img.shields.io/github/languages/top/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver)
 [![size sheild](https://img.shields.io/github/languages/code-size/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver)
 
 [![example workflow](https://github.com/marcpage/devops-driver/actions/workflows/pr.yml/badge.svg)](https://github.com/marcpage/devops-driver/actions/workflows/pr.yml)
```

### Comparing `devopsdriver-0.1.32/pyproject.toml` & `devopsdriver-0.1.34/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [project]
 name = "devopsdriver"
 description = "DevOps tools"
 readme = "README.md"
 license = {file = "LICENSE"}
 dynamic = ["version"]
-requires-python = ">= 3.12"
+requires-python = ">= 3.10"
 dependencies = [
   "PyYAML==6.0.1",
+  "keyring==25.0.0",
 ]
 keywords = ["azure", "devops", "jira", "confluence", "email", "pipelines", "tools"]
 classifiers=[
     "Development Status :: 1 - Planning",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Programming Language :: Python",
```

### Comparing `devopsdriver-0.1.32/tests/test_settings.py` & `devopsdriver-0.1.34/tests/test_settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 
 def __setup_settings(os: str = "Linux", shared: str = "test", **pref_dirs) -> None:
     settings.ENVIRON = {}
     settings.ARGV = []
     settings.SYSTEM = lambda: os
     settings.SHARED = shared
     settings.PRINT = lambda s: s
+    settings.GET_PASSWORD = lambda s, n: f"{s}:{n}"
+    settings.GET_PASS = lambda p: p
+    settings.SET_PASSWORD = lambda s, n, p: f"{s} {n} {p}"
     # settings.MAKEDIRS = lambda p: p
     # settings.Settings.FORMATS = None
     settings.Settings.PREF_DIR = pref_dirs
 
 
 def ensure(directory: str) -> str:
     """Ensures that a directory exists before using
@@ -288,12 +291,53 @@
     with TemporaryDirectory() as working_dir:
         __setup_settings(shared="test", Linux=join(working_dir, "Linux"))
         settings.ARGV = ["ignore", "test"]
         __write(join(working_dir, "Linux", "test.yml"), test=3)
         settings.main()
 
 
+def test_secret():
+    """test os secret storage"""
+    with TemporaryDirectory() as working_dir:
+        base_dir = join(working_dir, "base")
+        passwords = {"system": {"john": "setec astronomy"}}
+        __setup_settings(
+            os="Linux",
+            shared="test",
+            Linux=join(base_dir, "Linux"),
+            Darwin=join(base_dir, "macOS"),
+            Windows=join(base_dir, "Windows"),
+        )
+        settings.GET_PASSWORD = lambda s, e: passwords.get(s, {}).get(e, None)
+        __write(join(base_dir, "main.yml"), password="main")
+        opts = settings.Settings(join(base_dir, "main.py")).key(
+            "password", "system/john"
+        )
+        assert opts["password"] == "setec astronomy", opts["password"]
+
+
+def test_main_set_secret():
+    """test the main entry point when settings keychain secrets"""
+
+    def set_password(s, n, p):
+        assert s == "azure" and n == "token" and p == "setec astronomy", f"{s} {n} {p}"
+
+    with TemporaryDirectory() as working_dir:
+        __setup_settings(shared="test", Linux=join(working_dir, "Linux"))
+        settings.ARGV = ["ignore", "--set_secrets"]
+        settings.GET_PASSWORD = lambda s, n: None
+        settings.GET_PASS = lambda p: "setec astronomy"
+        settings.SET_PASSWORD = set_password
+        __write(
+            join(working_dir, "Linux", "test.yml"),
+            secrets={"azure.token": "azure/token"},
+        )
+        settings.main()
+
+
 if __name__ == "__main__":
+    test_main_set_secret()
+    test_secret()
     test_main()
     test_environ_values()
     test_cli_env_in_yaml()
     test_basic()
```

