# Comparing `tmp/pipxu-1.3.tar.gz` & `tmp/pipxu-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipxu-1.3.tar", last modified: Mon Apr  1 06:25:53 2024, max compression
+gzip compressed data, was "pipxu-1.4.tar", last modified: Tue Apr  2 01:19:18 2024, max compression
```

## Comparing `pipxu-1.3.tar` & `pipxu-1.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-01 06:25:53.509425 pipxu-1.3/
--rw-r--r--   0 mark      (1000) mark      (1000)       74 2023-09-17 09:50:08.000000 pipxu-1.3/.flake8
--rw-r--r--   0 mark      (1000) mark      (1000)       60 2024-02-24 11:57:27.000000 pipxu-1.3/.gitignore
--rw-r--r--   0 mark      (1000) mark      (1000)      441 2024-03-29 00:15:14.000000 pipxu-1.3/Makefile
--rw-r--r--   0 mark      (1000) mark      (1000)    15012 2024-04-01 06:25:53.509425 pipxu-1.3/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)    14489 2024-04-01 05:18:50.000000 pipxu-1.3/README.md
--rwxr-xr-x   0 mark      (1000) mark      (1000)      258 2024-03-29 22:26:39.000000 pipxu-1.3/bootstrap.sh
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-01 06:25:53.506092 pipxu-1.3/pipxu/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2024-03-29 00:15:14.000000 pipxu-1.3/pipxu/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)      126 2024-03-29 00:15:14.000000 pipxu-1.3/pipxu/__main__.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-01 06:25:53.509425 pipxu-1.3/pipxu/commands/
--rw-r--r--   0 mark      (1000) mark      (1000)     1190 2024-04-01 06:20:51.000000 pipxu-1.3/pipxu/commands/inject.py
--rw-r--r--   0 mark      (1000) mark      (1000)     4309 2024-04-01 06:20:46.000000 pipxu-1.3/pipxu/commands/install.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1368 2024-04-01 06:19:23.000000 pipxu-1.3/pipxu/commands/list.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1079 2024-04-01 06:21:00.000000 pipxu-1.3/pipxu/commands/reinstall-all.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2189 2024-04-01 06:21:09.000000 pipxu-1.3/pipxu/commands/reinstall.py
--rw-r--r--   0 mark      (1000) mark      (1000)      945 2024-04-01 06:19:39.000000 pipxu-1.3/pipxu/commands/runpip.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1190 2024-04-01 06:21:15.000000 pipxu-1.3/pipxu/commands/uninject.py
--rw-r--r--   0 mark      (1000) mark      (1000)      765 2024-04-01 06:19:47.000000 pipxu-1.3/pipxu/commands/uninstall-all.py
--rw-r--r--   0 mark      (1000) mark      (1000)      899 2024-04-01 06:19:51.000000 pipxu-1.3/pipxu/commands/uninstall.py
--rw-r--r--   0 mark      (1000) mark      (1000)      739 2024-04-01 06:21:22.000000 pipxu-1.3/pipxu/commands/upgrade-all.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1394 2024-04-01 06:21:28.000000 pipxu-1.3/pipxu/commands/upgrade.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1579 2024-04-01 06:20:09.000000 pipxu-1.3/pipxu/commands/version.py
--rw-r--r--   0 mark      (1000) mark      (1000)     5646 2024-04-01 06:11:46.000000 pipxu-1.3/pipxu/pipxu.py
--rw-r--r--   0 mark      (1000) mark      (1000)      780 2024-03-29 00:15:14.000000 pipxu-1.3/pipxu/run.py
--rw-r--r--   0 mark      (1000) mark      (1000)     9675 2024-04-01 03:05:25.000000 pipxu-1.3/pipxu/utils.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-01 06:25:53.509425 pipxu-1.3/pipxu.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)    15012 2024-04-01 06:25:53.000000 pipxu-1.3/pipxu.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      648 2024-04-01 06:25:53.000000 pipxu-1.3/pipxu.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2024-04-01 06:25:53.000000 pipxu-1.3/pipxu.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       43 2024-04-01 06:25:53.000000 pipxu-1.3/pipxu.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       68 2024-04-01 06:25:53.000000 pipxu-1.3/pipxu.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        6 2024-04-01 06:25:53.000000 pipxu-1.3/pipxu.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)     1042 2024-03-29 05:04:28.000000 pipxu-1.3/pyproject.toml
--rw-r--r--   0 mark      (1000) mark      (1000)       38 2024-04-01 06:25:53.509425 pipxu-1.3/setup.cfg
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-02 01:19:18.885772 pipxu-1.4/
+-rw-r--r--   0 mark      (1000) mark      (1000)       74 2023-09-17 09:50:08.000000 pipxu-1.4/.flake8
+-rw-r--r--   0 mark      (1000) mark      (1000)       60 2024-02-24 11:57:27.000000 pipxu-1.4/.gitignore
+-rw-r--r--   0 mark      (1000) mark      (1000)      441 2024-03-29 00:15:14.000000 pipxu-1.4/Makefile
+-rw-r--r--   0 mark      (1000) mark      (1000)    14459 2024-04-02 01:19:18.885772 pipxu-1.4/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)    13936 2024-04-02 01:08:56.000000 pipxu-1.4/README.md
+-rwxr-xr-x   0 mark      (1000) mark      (1000)      258 2024-03-29 22:26:39.000000 pipxu-1.4/bootstrap.sh
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-02 01:19:18.885772 pipxu-1.4/pipxu/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2024-03-29 00:15:14.000000 pipxu-1.4/pipxu/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      126 2024-03-29 00:15:14.000000 pipxu-1.4/pipxu/__main__.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-02 01:19:18.885772 pipxu-1.4/pipxu/commands/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1175 2024-04-02 01:11:43.000000 pipxu-1.4/pipxu/commands/inject.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     4305 2024-04-02 01:08:36.000000 pipxu-1.4/pipxu/commands/install.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1369 2024-04-02 01:11:56.000000 pipxu-1.4/pipxu/commands/list.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1097 2024-04-02 01:12:02.000000 pipxu-1.4/pipxu/commands/reinstall-all.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2166 2024-04-02 01:12:09.000000 pipxu-1.4/pipxu/commands/reinstall.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      957 2024-04-02 01:12:18.000000 pipxu-1.4/pipxu/commands/runpip.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1175 2024-04-02 01:12:24.000000 pipxu-1.4/pipxu/commands/uninject.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      763 2024-04-02 01:12:29.000000 pipxu-1.4/pipxu/commands/uninstall-all.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      875 2024-04-02 01:12:35.000000 pipxu-1.4/pipxu/commands/uninstall.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      757 2024-04-02 01:12:41.000000 pipxu-1.4/pipxu/commands/upgrade-all.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1368 2024-04-02 01:12:46.000000 pipxu-1.4/pipxu/commands/upgrade.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1595 2024-04-02 01:12:52.000000 pipxu-1.4/pipxu/commands/version.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     5646 2024-04-02 01:13:11.000000 pipxu-1.4/pipxu/pipxu.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      780 2024-04-02 01:13:16.000000 pipxu-1.4/pipxu/run.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     9670 2024-04-02 01:13:23.000000 pipxu-1.4/pipxu/utils.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-02 01:19:18.885772 pipxu-1.4/pipxu.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)    14459 2024-04-02 01:19:18.000000 pipxu-1.4/pipxu.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      648 2024-04-02 01:19:18.000000 pipxu-1.4/pipxu.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2024-04-02 01:19:18.000000 pipxu-1.4/pipxu.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       43 2024-04-02 01:19:18.000000 pipxu-1.4/pipxu.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       68 2024-04-02 01:19:18.000000 pipxu-1.4/pipxu.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        6 2024-04-02 01:19:18.000000 pipxu-1.4/pipxu.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)     1042 2024-03-29 05:04:28.000000 pipxu-1.4/pyproject.toml
+-rw-r--r--   0 mark      (1000) mark      (1000)       38 2024-04-02 01:19:18.885772 pipxu-1.4/setup.cfg
```

### Comparing `pipxu-1.3/PKG-INFO` & `pipxu-1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipxu
-Version: 1.3
+Version: 1.4
 Summary: Install and Run Python Applications in Isolated Environments using UV
 Author-email: Mark Blakeney <mark.blakeney@bullet-systems.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/bulletmark/pipxu
 Keywords: pipx,pip,uv,venv,virtualenv
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -63,49 +63,45 @@
   --man-dir MAN_DIR     specify PIPXU_MAN_DIR
   --default-python DEFAULT_PYTHON
                         path to default python executable, default="python3"
   -V, --version         just print pipxu version and exit
 
 Commands:
   {inject,install,list,reinstall-all,reinstall,runpip,uninject,uninstall-all,uninstall,upgrade-all,upgrade,version}
-    inject              Install extra packages into an application's virtual
-                        environment.
+    inject              Install extra packages into an application.
     install             Install a Python application using an isolated virtual
                         environment.
-    list                List Python applications installed by this tool.
-    reinstall-all       Reinstall all packages and their executables.
-    reinstall           Reinstall a package and it's executables.
+    list                List all applications installed by this tool.
+    reinstall-all       Reinstall all applications.
+    reinstall           Reinstall an application.
     runpip              Run pip with given arguments on virtual environment
-                        for the given package.
-    uninject            Uninstall extra packages from an application's virtual
-                        environment.
-    uninstall-all       Uninstall all Python applications and their virtual
-                        environments.
-    uninstall           Uninstall a Python application and it's virtual
-                        environment
-    upgrade-all         Upgrade all packages and their executables.
-    upgrade             Upgrade a package and it's executables.
-    version             List installed package versions.
+                        for the given application.
+    uninject            Uninstall extra packages from an application.
+    uninstall-all       Uninstall all applications.
+    uninstall           Uninstall an application.
+    upgrade-all         Upgrade all applications.
+    upgrade             Upgrade an application.
+    version             List installed application versions.
 
 Note you can set default starting global options in $HOME/.config/pipxu-
 flags.conf.
 ```
 
 Type `pipxu <command> -h` to see specific help/usage for any
 individual command:
 
 ### Command `inject`
 
 ```
 usage: pipxu inject [-h] [-v] package extras [extras ...]
 
-Install extra packages into an application's virtual environment.
+Install extra packages into an application.
 
 positional arguments:
-  package        existing package name
+  package        existing application name
   extras         extra package name[s] to inject/install
 
 options:
   -h, --help     show this help message and exit
   -v, --verbose  give more output
 ```
 
@@ -114,74 +110,74 @@
 ```
 usage: pipxu install [-h] [-p PYTHON | -P PYENV] [-f] [-e] [-d] [-v]
                            package [package ...]
 
 Install a Python application using an isolated virtual environment.
 
 positional arguments:
-  package               package[s] to install
+  package               application[s] to install
 
 options:
   -h, --help            show this help message and exit
   -p PYTHON, --python PYTHON
                         specify explicit python executable path
   -P PYENV, --pyenv PYENV
                         pyenv python version to use, i.e. from `pyenv
                         versions`, e.g. "3.9".
   -f, --force           recreate any existing venv
-  -e, --editable        install package[s] in editable mode
+  -e, --editable        install application[s] in editable mode
   -d, --include-deps    include executables from dependencies
   -v, --verbose         give more output
 ```
 
 ### Command `list`
 
 ```
 usage: pipxu list [-h] [--json] [package ...]
 
-List Python applications installed by this tool.
+List all applications installed by this tool.
 
 positional arguments:
-  package     list the given package[s] only
+  package     list the given application[s] only
 
 options:
   -h, --help  show this help message and exit
   --json      output json instead
 ```
 
 ### Command `reinstall-all`
 
 ```
 usage: pipxu reinstall-all [-h] [-p PYTHON | -P PYENV] [-v]
                                  [-s [SKIP ...]]
 
-Reinstall all packages and their executables.
+Reinstall all applications.
 
 options:
   -h, --help            show this help message and exit
   -p PYTHON, --python PYTHON
                         specify explicit python executable path
   -P PYENV, --pyenv PYENV
                         pyenv python version to use, i.e. from `pyenv
                         versions`, e.g. "3.9".
   -v, --verbose         give more output
   -s [SKIP ...], --skip [SKIP ...]
-                        skip these packages, e.g. package1 package2
+                        skip these applications, e.g. "-s package1 package2"
 ```
 
 ### Command `reinstall`
 
 ```
 usage: pipxu reinstall [-h] [-p PYTHON | -P PYENV] [-v]
                              package [package ...]
 
-Reinstall a package and it's executables.
+Reinstall an application.
 
 positional arguments:
-  package               package name[s] to upgrade
+  package               application[s] to reinstall
 
 options:
   -h, --help            show this help message and exit
   -p PYTHON, --python PYTHON
                         specify explicit python executable path
   -P PYENV, --pyenv PYENV
                         pyenv python version to use, i.e. from `pyenv
@@ -190,107 +186,107 @@
 ```
 
 ### Command `runpip`
 
 ```
 usage: pipxu runpip [-h] package [args ...]
 
-Run pip with given arguments on virtual environment for the given package.
+Run pip with given arguments on virtual environment for the given application.
 
 positional arguments:
-  package     existing package name
+  package     existing application name
   args        arguments to pass to uv pip. should start with "--".
 
 options:
   -h, --help  show this help message and exit
 ```
 
 ### Command `uninject`
 
 ```
 usage: pipxu uninject [-h] [-v] package extras [extras ...]
 
-Uninstall extra packages from an application's virtual environment.
+Uninstall extra packages from an application.
 
 positional arguments:
-  package        existing package name
+  package        existing application name
   extras         extra package name[s] to uninstall
 
 options:
   -h, --help     show this help message and exit
   -v, --verbose  give more output
 ```
 
 ### Command `uninstall-all`
 
 ```
 usage: pipxu uninstall-all [-h] [-v] [-s [SKIP ...]]
 
-Uninstall all Python applications and their virtual environments.
+Uninstall all applications.
 
 options:
   -h, --help            show this help message and exit
   -v, --verbose         give more output
   -s [SKIP ...], --skip [SKIP ...]
-                        skip these packages, e.g. package1 package2
+                        skip these applications, e.g. "-s package1 package2"
 ```
 
 ### Command `uninstall`
 
 ```
 usage: pipxu uninstall [-h] [-v] package [package ...]
 
-Uninstall a Python application and it's virtual environment
+Uninstall an application.
 
 positional arguments:
-  package        package name[s] to uninstall
+  package        application[s] to uninstall
 
 options:
   -h, --help     show this help message and exit
   -v, --verbose  give more output
 ```
 
 ### Command `upgrade-all`
 
 ```
 usage: pipxu upgrade-all [-h] [-v] [-s [SKIP ...]]
 
-Upgrade all packages and their executables.
+Upgrade all applications.
 
 options:
   -h, --help            show this help message and exit
   -v, --verbose         give more output
   -s [SKIP ...], --skip [SKIP ...]
-                        skip these packages, e.g. package1 package2
+                        skip these applications, e.g. "-s package1 package2"
 ```
 
 ### Command `upgrade`
 
 ```
 usage: pipxu upgrade [-h] [-v] package [package ...]
 
-Upgrade a package and it's executables.
+Upgrade an application.
 
 positional arguments:
-  package        package name[s] to upgrade
+  package        application[s] to upgrade
 
 options:
   -h, --help     show this help message and exit
   -v, --verbose  give more output
 ```
 
 ### Command `version`
 
 ```
 usage: pipxu version [-h] [package]
 
-List installed package versions.
+List installed application versions.
 
 positional arguments:
-  package     report specific package and dependent package versions
+  package     report specific application and dependent package versions
 
 options:
   -h, --help  show this help message and exit
 ```
 
 ## Installation and Upgrade
 
@@ -362,18 +358,14 @@
    .` or `pipxu inject . pudb`. I.e. `pipxu` automatically determines
    the package name associated with the current directory. Note that
    `pipx` accepts "`.`" for the install command, but not for any others.
 
 3. If run as root or with `sudo`, `pipxu` installs applications to a
    global location.
 
-At the time of initial release, the `pipxu` application comprises 736
-lines of Python code whereas the `pipx` application is 4300 lines of
-Python code.
-
 ## Environment Variables
 
 Type `pipxu` without any arguments to see usage and the current
 environment. The environment is printed at the bottom of the screen
 output as follows:
 
 E.g. run as my user "mark":
```

### Comparing `pipxu-1.3/README.md` & `pipxu-1.4/pipxu.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: pipxu
+Version: 1.4
+Summary: Install and Run Python Applications in Isolated Environments using UV
+Author-email: Mark Blakeney <mark.blakeney@bullet-systems.net>
+License: GPLv3
+Project-URL: Homepage, https://github.com/bulletmark/pipxu
+Keywords: pipx,pip,uv,venv,virtualenv
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Requires-Dist: filelock
+Requires-Dist: platformdirs
+Requires-Dist: importlib-metadata; python_version < "3.8"
+
 ## PIPXU - Install and Run Python Applications in Isolated Environments using UV
 [![PyPi](https://img.shields.io/pypi/v/pipxu)](https://pypi.org/project/pipxu/)
 [![AUR](https://img.shields.io/aur/version/pipxu)](https://aur.archlinux.org/packages/pipxu/)
 
 [`pipxu`][pipxu] installs Python applications, i.e. a Python packages
 which have one or more executable programs, into independent isolated
 virtual environments on your system. Each package and it's dependencies
@@ -48,49 +63,45 @@
   --man-dir MAN_DIR     specify PIPXU_MAN_DIR
   --default-python DEFAULT_PYTHON
                         path to default python executable, default="python3"
   -V, --version         just print pipxu version and exit
 
 Commands:
   {inject,install,list,reinstall-all,reinstall,runpip,uninject,uninstall-all,uninstall,upgrade-all,upgrade,version}
-    inject              Install extra packages into an application's virtual
-                        environment.
+    inject              Install extra packages into an application.
     install             Install a Python application using an isolated virtual
                         environment.
-    list                List Python applications installed by this tool.
-    reinstall-all       Reinstall all packages and their executables.
-    reinstall           Reinstall a package and it's executables.
+    list                List all applications installed by this tool.
+    reinstall-all       Reinstall all applications.
+    reinstall           Reinstall an application.
     runpip              Run pip with given arguments on virtual environment
-                        for the given package.
-    uninject            Uninstall extra packages from an application's virtual
-                        environment.
-    uninstall-all       Uninstall all Python applications and their virtual
-                        environments.
-    uninstall           Uninstall a Python application and it's virtual
-                        environment
-    upgrade-all         Upgrade all packages and their executables.
-    upgrade             Upgrade a package and it's executables.
-    version             List installed package versions.
+                        for the given application.
+    uninject            Uninstall extra packages from an application.
+    uninstall-all       Uninstall all applications.
+    uninstall           Uninstall an application.
+    upgrade-all         Upgrade all applications.
+    upgrade             Upgrade an application.
+    version             List installed application versions.
 
 Note you can set default starting global options in $HOME/.config/pipxu-
 flags.conf.
 ```
 
 Type `pipxu <command> -h` to see specific help/usage for any
 individual command:
 
 ### Command `inject`
 
 ```
 usage: pipxu inject [-h] [-v] package extras [extras ...]
 
-Install extra packages into an application's virtual environment.
+Install extra packages into an application.
 
 positional arguments:
-  package        existing package name
+  package        existing application name
   extras         extra package name[s] to inject/install
 
 options:
   -h, --help     show this help message and exit
   -v, --verbose  give more output
 ```
 
@@ -99,74 +110,74 @@
 ```
 usage: pipxu install [-h] [-p PYTHON | -P PYENV] [-f] [-e] [-d] [-v]
                            package [package ...]
 
 Install a Python application using an isolated virtual environment.
 
 positional arguments:
-  package               package[s] to install
+  package               application[s] to install
 
 options:
   -h, --help            show this help message and exit
   -p PYTHON, --python PYTHON
                         specify explicit python executable path
   -P PYENV, --pyenv PYENV
                         pyenv python version to use, i.e. from `pyenv
                         versions`, e.g. "3.9".
   -f, --force           recreate any existing venv
-  -e, --editable        install package[s] in editable mode
+  -e, --editable        install application[s] in editable mode
   -d, --include-deps    include executables from dependencies
   -v, --verbose         give more output
 ```
 
 ### Command `list`
 
 ```
 usage: pipxu list [-h] [--json] [package ...]
 
-List Python applications installed by this tool.
+List all applications installed by this tool.
 
 positional arguments:
-  package     list the given package[s] only
+  package     list the given application[s] only
 
 options:
   -h, --help  show this help message and exit
   --json      output json instead
 ```
 
 ### Command `reinstall-all`
 
 ```
 usage: pipxu reinstall-all [-h] [-p PYTHON | -P PYENV] [-v]
                                  [-s [SKIP ...]]
 
-Reinstall all packages and their executables.
+Reinstall all applications.
 
 options:
   -h, --help            show this help message and exit
   -p PYTHON, --python PYTHON
                         specify explicit python executable path
   -P PYENV, --pyenv PYENV
                         pyenv python version to use, i.e. from `pyenv
                         versions`, e.g. "3.9".
   -v, --verbose         give more output
   -s [SKIP ...], --skip [SKIP ...]
-                        skip these packages, e.g. package1 package2
+                        skip these applications, e.g. "-s package1 package2"
 ```
 
 ### Command `reinstall`
 
 ```
 usage: pipxu reinstall [-h] [-p PYTHON | -P PYENV] [-v]
                              package [package ...]
 
-Reinstall a package and it's executables.
+Reinstall an application.
 
 positional arguments:
-  package               package name[s] to upgrade
+  package               application[s] to reinstall
 
 options:
   -h, --help            show this help message and exit
   -p PYTHON, --python PYTHON
                         specify explicit python executable path
   -P PYENV, --pyenv PYENV
                         pyenv python version to use, i.e. from `pyenv
@@ -175,107 +186,107 @@
 ```
 
 ### Command `runpip`
 
 ```
 usage: pipxu runpip [-h] package [args ...]
 
-Run pip with given arguments on virtual environment for the given package.
+Run pip with given arguments on virtual environment for the given application.
 
 positional arguments:
-  package     existing package name
+  package     existing application name
   args        arguments to pass to uv pip. should start with "--".
 
 options:
   -h, --help  show this help message and exit
 ```
 
 ### Command `uninject`
 
 ```
 usage: pipxu uninject [-h] [-v] package extras [extras ...]
 
-Uninstall extra packages from an application's virtual environment.
+Uninstall extra packages from an application.
 
 positional arguments:
-  package        existing package name
+  package        existing application name
   extras         extra package name[s] to uninstall
 
 options:
   -h, --help     show this help message and exit
   -v, --verbose  give more output
 ```
 
 ### Command `uninstall-all`
 
 ```
 usage: pipxu uninstall-all [-h] [-v] [-s [SKIP ...]]
 
-Uninstall all Python applications and their virtual environments.
+Uninstall all applications.
 
 options:
   -h, --help            show this help message and exit
   -v, --verbose         give more output
   -s [SKIP ...], --skip [SKIP ...]
-                        skip these packages, e.g. package1 package2
+                        skip these applications, e.g. "-s package1 package2"
 ```
 
 ### Command `uninstall`
 
 ```
 usage: pipxu uninstall [-h] [-v] package [package ...]
 
-Uninstall a Python application and it's virtual environment
+Uninstall an application.
 
 positional arguments:
-  package        package name[s] to uninstall
+  package        application[s] to uninstall
 
 options:
   -h, --help     show this help message and exit
   -v, --verbose  give more output
 ```
 
 ### Command `upgrade-all`
 
 ```
 usage: pipxu upgrade-all [-h] [-v] [-s [SKIP ...]]
 
-Upgrade all packages and their executables.
+Upgrade all applications.
 
 options:
   -h, --help            show this help message and exit
   -v, --verbose         give more output
   -s [SKIP ...], --skip [SKIP ...]
-                        skip these packages, e.g. package1 package2
+                        skip these applications, e.g. "-s package1 package2"
 ```
 
 ### Command `upgrade`
 
 ```
 usage: pipxu upgrade [-h] [-v] package [package ...]
 
-Upgrade a package and it's executables.
+Upgrade an application.
 
 positional arguments:
-  package        package name[s] to upgrade
+  package        application[s] to upgrade
 
 options:
   -h, --help     show this help message and exit
   -v, --verbose  give more output
 ```
 
 ### Command `version`
 
 ```
 usage: pipxu version [-h] [package]
 
-List installed package versions.
+List installed application versions.
 
 positional arguments:
-  package     report specific package and dependent package versions
+  package     report specific application and dependent package versions
 
 options:
   -h, --help  show this help message and exit
 ```
 
 ## Installation and Upgrade
 
@@ -347,18 +358,14 @@
    .` or `pipxu inject . pudb`. I.e. `pipxu` automatically determines
    the package name associated with the current directory. Note that
    `pipx` accepts "`.`" for the install command, but not for any others.
 
 3. If run as root or with `sudo`, `pipxu` installs applications to a
    global location.
 
-At the time of initial release, the `pipxu` application comprises 736
-lines of Python code whereas the `pipx` application is 4300 lines of
-Python code.
-
 ## Environment Variables
 
 Type `pipxu` without any arguments to see usage and the current
 environment. The environment is printed at the bottom of the screen
 output as follows:
 
 E.g. run as my user "mark":
```

### Comparing `pipxu-1.3/pipxu/commands/inject.py` & `pipxu-1.4/pipxu/commands/inject.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # Author: Mark Blakeney, Feb 2024.
-'Install extra packages into an application\'s virtual environment.'
+'Install extra packages into an application.'
 from __future__ import annotations
 
 from argparse import ArgumentParser, Namespace
 from typing import Optional
 
 from .. import utils
 
 def init(parser: ArgumentParser) -> None:
     'Called to add command arguments to parser at init'
     parser.add_argument('-v', '--verbose', action='store_true',
                         help='give more output')
     parser.add_argument('package',
-                        help='existing package name')
+                        help='existing application name')
     parser.add_argument('extras', nargs='+',
                         help='extra package name[s] to inject/install')
 
 def main(args: Namespace) -> Optional[str]:
     'Called to action this command'
     pkgname, vdir = utils.get_package_from_arg(args.package, args)
     if not vdir:
-        return f'Package {pkgname} is not installed.'
+        return f'Application {pkgname} is not installed.'
 
     pip_args = utils.make_args((args.verbose, '-v'))
     extras = ' '.join(f'"{a}"' for a in args.extras)
     if not utils.piprun(vdir, f'install{pip_args} {extras}'):
         return f'Error: failed to install "{extras}" to {pkgname}'
 
     return utils.add_or_remove_pkg(vdir, pkgname, args.extras, args, add=True)
```

### Comparing `pipxu-1.3/pipxu/commands/install.py` & `pipxu-1.4/pipxu/commands/install.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 from platformdirs import user_runtime_path
 
 from .. import utils
 from ..run import run
 
 MAX_VDIRS = 1_000_000
 
-def get_next_vdir(vdirbase: Path, maxn) -> Optional[Path]:
+def get_next_vdir(vdirbase: Path) -> Optional[Path]:
     'Return the first available venv directory'
     vdirs = set(int(f.name) for f in vdirbase.iterdir())
-    for n in range(1, maxn + 1):
+    for n in range(1, MAX_VDIRS + 1):
         if n not in vdirs:
             return vdirbase / str(n)
 
     return None
 
 def init(parser: ArgumentParser) -> None:
     'Called to add command arguments to parser at init'
@@ -30,35 +30,35 @@
                         help='specify explicit python executable path')
     xgroup.add_argument('-P', '--pyenv',
                         help='pyenv python version to use, '
                         'i.e. from `pyenv versions`, e.g. "3.9".')
     parser.add_argument('-f', '--force', action='store_true',
                         help='recreate any existing venv')
     parser.add_argument('-e', '--editable', action='store_true',
-                        help='install package[s] in editable mode')
+                        help='install application[s] in editable mode')
     parser.add_argument('-d', '--include-deps', action='store_true',
                         help='include executables from dependencies')
     parser.add_argument('-v', '--verbose', action='store_true',
                         help='give more output')
     parser.add_argument('package', nargs='+',
-                        help='package[s] to install')
+                        help='application[s] to install')
 
 def main(args: Namespace) -> Optional[str]:
     'Called to action this command'
     pyexe = utils.get_python(args)
     venv_args = utils.make_args((args.verbose, '-v'), (not args.verbose, '-q'),
                                 (bool(pyexe), f'--python={pyexe}'))
     pip_args = utils.make_args((args.verbose, '-v'), (args.editable, '-e'))
 
     lockfile = user_runtime_path() / f'{args._prog}.lock'
     vdirbase = args._venvs_dir
     for pkg in args.package:
         # Use a lock file in case we are running multiple installs in parallel
         with FileLock(lockfile):
-            vdir = get_next_vdir(vdirbase, MAX_VDIRS)
+            vdir = get_next_vdir(vdirbase)
             if not vdir:
                 return f'Error: Too many vdirs (>{MAX_VDIRS}) in {vdirbase}'
 
             # Create the vdir
             if not run(f'uv venv{venv_args} {vdir}'):
                 utils.rm_vdir(vdir, args)
                 return f'Error: failed to create {vdir} for {pkg}.'
```

### Comparing `pipxu-1.3/pipxu/commands/list.py` & `pipxu-1.4/pipxu/commands/list.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Author: Mark Blakeney, Feb 2024.
-'List Python applications installed by this tool.'
+'List all applications installed by this tool.'
 from __future__ import annotations
 
 import json
 from argparse import ArgumentParser, Namespace
 from typing import Optional
 
 from .. import utils
@@ -13,15 +13,15 @@
     return f'"{value}"' if isinstance(value, str) else value
 
 def init(parser: ArgumentParser) -> None:
     'Called to add command arguments to parser at init'
     parser.add_argument('--json', action='store_true',
                         help='output json instead')
     parser.add_argument('package', nargs='*',
-                        help='list the given package[s] only')
+                        help='list the given application[s] only')
 
 def main(args: Namespace) -> Optional[str]:
     'Called to action this command'
     pkgs = set(utils.get_package_from_arg(p, args)[0] for p in args.package)
     json_out = {}
     for pdir in sorted(args._packages_dir.iterdir()):
         pkgname = pdir.name
```

### Comparing `pipxu-1.3/pipxu/commands/reinstall-all.py` & `pipxu-1.4/pipxu/commands/reinstall-all.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Author: Mark Blakeney, Feb 2024.
-'Reinstall all packages and their executables.'
+'Reinstall all applications.'
 from __future__ import annotations
 
 from argparse import ArgumentParser, Namespace
 from typing import Optional
 
 from .. import utils
 from . import reinstall
@@ -15,13 +15,14 @@
                         help='specify explicit python executable path')
     xgroup.add_argument('-P', '--pyenv',
                         help='pyenv python version to use, '
                         'i.e. from `pyenv versions`, e.g. "3.9".')
     parser.add_argument('-v', '--verbose', action='store_true',
                         help='give more output')
     parser.add_argument('-s', '--skip', nargs='*',
-                        help='skip these packages, e.g. package1 package2')
+                        help='skip these applications, '
+                        'e.g. "-s package1 package2"')
 
 def main(args: Namespace) -> Optional[str]:
     'Called to action this command'
     args.package = utils.get_all_package_names(args)
     return reinstall.main(args)
```

### Comparing `pipxu-1.3/pipxu/commands/reinstall.py` & `pipxu-1.4/pipxu/commands/reinstall.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Author: Mark Blakeney, Feb 2024.
-'Reinstall a package and it\'s executables.'
+'Reinstall an application.'
 from __future__ import annotations
 
-from argparse import ArgumentParser, Namespace
-from typing import Optional
 import shutil
 import tempfile
+from argparse import ArgumentParser, Namespace
 from pathlib import Path
+from typing import Optional
 
 from .. import utils
 from ..run import run
 
 def init(parser: ArgumentParser) -> None:
     'Called to add command arguments to parser at init'
     xgroup = parser.add_mutually_exclusive_group()
@@ -18,26 +18,26 @@
                         help='specify explicit python executable path')
     xgroup.add_argument('-P', '--pyenv',
                         help='pyenv python version to use, '
                         'i.e. from `pyenv versions`, e.g. "3.9".')
     parser.add_argument('-v', '--verbose', action='store_true',
                         help='give more output')
     parser.add_argument('package', nargs='+',
-                        help='package name[s] to upgrade')
+                        help='application[s] to reinstall')
 
 def main(args: Namespace) -> Optional[str]:
     'Called to action this command'
     pyexe = utils.get_python(args)
     venv_args = utils.make_args((args.verbose, '-v'), (not args.verbose, '-q'),
                                 (bool(pyexe), f'--python={pyexe}'))
     pip_args = utils.make_args((args.verbose, '-v'))
     for pkgname in args.package:
         pkgname, vdir = utils.get_package_from_arg(pkgname, args)
         if not vdir:
-            return f'package {pkgname} is not installed.'
+            return f'Application {pkgname} is not installed.'
 
         data = utils.get_json(vdir, args) or {}
 
         with tempfile.TemporaryDirectory() as tdir:
             tfile = Path(tdir, args._freeze_file)
             shutil.copyfile(vdir / args._freeze_file, tfile)
 
@@ -50,10 +50,10 @@
                 utils.rm_vdir(vdir, args)
                 return f'Error: failed to resync {pkgname}'
 
         err = utils.make_links(vdir, pkgname, args, data)
         if err:
             return err
 
-        print(f'Reinstall of {pkgname} completed.')
+        print(f'{pkgname} reinstalled.')
 
     return None
```

### Comparing `pipxu-1.3/pipxu/commands/runpip.py` & `pipxu-1.4/pipxu/commands/runpip.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Author: Mark Blakeney, Feb 2024.
-'Run pip with given arguments on virtual environment for the given package.'
+'Run pip with given arguments on virtual environment for the given application.'
 from __future__ import annotations
 
 from argparse import ArgumentParser, Namespace
 from typing import Optional
 
 from .. import utils
 
 def init(parser: ArgumentParser) -> None:
     'Called to add command arguments to parser at init'
     parser.add_argument('package',
-                        help='existing package name')
+                        help='existing application name')
     parser.add_argument('args', nargs='*',
                         help='arguments to pass to uv pip. '
                         'should start with "--".')
 
 def main(args: Namespace) -> Optional[str]:
     'Called to action this command'
     pkgname, vdir = utils.get_package_from_arg(args.package, args)
     if not vdir:
-        return f'Package {pkgname} is not installed.'
+        return f'Application {pkgname} is not installed.'
 
     if not utils.piprun(vdir, ' '.join(args.args), quiet=True):
         return f'Error: failed to run pip for {pkgname}'
     return None
```

### Comparing `pipxu-1.3/pipxu/commands/uninject.py` & `pipxu-1.4/pipxu/commands/uninject.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # Author: Mark Blakeney, Feb 2024.
-'Uninstall extra packages from an application\'s virtual environment.'
+'Uninstall extra packages from an application.'
 from __future__ import annotations
 
 from argparse import ArgumentParser, Namespace
 from typing import Optional
 
 from .. import utils
 
 def init(parser: ArgumentParser) -> None:
     'Called to add command arguments to parser at init'
     parser.add_argument('-v', '--verbose', action='store_true',
                         help='give more output')
     parser.add_argument('package',
-                        help='existing package name')
+                        help='existing application name')
     parser.add_argument('extras', nargs='+',
                         help='extra package name[s] to uninstall')
 
 def main(args: Namespace) -> Optional[str]:
     'Called to action this command'
     pkgname, vdir = utils.get_package_from_arg(args.package, args)
     if not vdir:
-        return f'package {pkgname} is not installed.'
+        return f'Application {pkgname} is not installed.'
 
     pip_args = utils.make_args((args.verbose, '-v'))
     extras = ' '.join(f'"{a}"' for a in args.extras)
     if not utils.piprun(vdir, f'uninstall{pip_args} {extras}'):
         return f'Error: failed to uninstall {extras} to {pkgname}'
 
     return utils.add_or_remove_pkg(vdir, pkgname, args.extras, args, add=False)
```

### Comparing `pipxu-1.3/pipxu/commands/uninstall-all.py` & `pipxu-1.4/pipxu/commands/uninstall-all.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # Author: Mark Blakeney, Feb 2024.
-'Uninstall all Python applications and their virtual environments.'
+'Uninstall all applications.'
 from __future__ import annotations
 
 from argparse import ArgumentParser, Namespace
 from typing import Optional
 
 from .. import utils
 from . import uninstall
 
 def init(parser: ArgumentParser) -> None:
     'Called to add command arguments to parser at init'
     parser.add_argument('-v', '--verbose', action='store_true',
                         help='give more output')
     parser.add_argument('-s', '--skip', nargs='*',
-                        help='skip these packages, e.g. package1 package2')
+                        help='skip these applications, '
+                        'e.g. "-s package1 package2"')
 
 def main(args: Namespace) -> Optional[str]:
     'Called to action this command'
     args.package = utils.get_all_package_names(args)
     return uninstall.main(args)
```

### Comparing `pipxu-1.3/pipxu/commands/uninstall.py` & `pipxu-1.4/pipxu/commands/uninstall.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Author: Mark Blakeney, Feb 2024.
-'Uninstall a Python application and it\'s virtual environment'
+'Uninstall an application.'
 from __future__ import annotations
 
 from argparse import ArgumentParser, Namespace
 from typing import Optional
 
 from .. import utils
 
 def init(parser: ArgumentParser) -> None:
     'Called to add command arguments to parser at init'
     parser.add_argument('-v', '--verbose', action='store_true',
                         help='give more output')
     parser.add_argument('package', nargs='+',
-                        help='package name[s] to uninstall')
+                        help='application[s] to uninstall')
 
 def main(args: Namespace) -> Optional[str]:
     'Called to action this command'
     for pkgname in args.package:
         pkgname, vdir = utils.get_package_from_arg(pkgname, args)
         if not vdir or not utils.rm_package(pkgname, args):
-            return f'{pkgname} is not installed.'
+            return f'Application {pkgname} is not installed.'
 
         print(f'{pkgname} uninstalled.')
 
     return None
```

### Comparing `pipxu-1.3/pipxu/commands/upgrade.py` & `pipxu-1.4/pipxu/commands/upgrade.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # Author: Mark Blakeney, Feb 2024.
-'Upgrade a package and it\'s executables.'
+'Upgrade an application.'
 from __future__ import annotations
 
 from argparse import ArgumentParser, Namespace
 from typing import Optional
 
 from .. import utils
 
 def init(parser: ArgumentParser) -> None:
     'Called to add command arguments to parser at init'
     parser.add_argument('-v', '--verbose', action='store_true',
                         help='give more output')
     parser.add_argument('package', nargs='+',
-                        help='package name[s] to upgrade')
+                        help='application[s] to upgrade')
 
 def main(args: Namespace) -> Optional[str]:
     'Called to action this command'
     pip_args = utils.make_args((args.verbose, '-v'), (True, '-U'))
     for pkgname in args.package:
         pkgname, vdir = utils.get_package_from_arg(pkgname, args)
         if not vdir:
-            return f'package {pkgname} is not installed.'
+            return f'Application {pkgname} is not installed.'
 
         data = utils.get_json(vdir, args) or {}
         editpath = data.get('editpath')
         pkg = f'-e {editpath}' if editpath else pkgname
         extras = ' '.join(data.get('injected', []))
         if not utils.piprun(vdir, f'install --reinstall'
                             f'{pip_args} {pkg} {extras}'):
             return f'Error: failed to {args.name} {pkgname}'
 
         err = utils.make_links(vdir, pkgname, args, data)
         if err:
             return err
 
-        print(f'Upgrade of {pkgname} completed.')
+        print(f'{pkgname} upgraded.')
 
     return None
```

### Comparing `pipxu-1.3/pipxu/commands/version.py` & `pipxu-1.4/pipxu/commands/version.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # Author: Mark Blakeney, Feb 2024.
-'List installed package versions.'
+'List installed application versions.'
 from __future__ import annotations
 
 from argparse import ArgumentParser, Namespace
 from typing import Optional
 
 from .. import utils
 
 def init(parser: ArgumentParser) -> None:
     'Called to add command arguments to parser at init'
     parser.add_argument('package', nargs='?',
-                        help='report specific package and dependent '
+                        help='report specific application and dependent '
                         'package versions')
 
 def main(args: Namespace) -> Optional[str]:
     'Called to action this command'
     def display(pkgname, version):
         ver, loc = version
         if loc:
             ver += f' @ {loc}'
         print(f'{pkgname}=={ver}')
 
     if args.package:
         pkgname, vdir = utils.get_package_from_arg(args.package, args)
         if not vdir:
-            return f'Package {pkgname} not found.'
+            return f'Application {pkgname} not found.'
 
         versions = utils.get_versions(args._packages_dir / pkgname)
         if not versions:
-            return f'Package {pkgname} versions not found.'
+            return f'Application {pkgname} versions not found.'
 
         # Reorder version dict to put pkgname first
         if pkgname in versions:
             sversions = {pkgname: versions[pkgname]}
             del versions[pkgname]
             sversions.update(versions)
             versions = sversions
```

### Comparing `pipxu-1.3/pipxu/pipxu.py` & `pipxu-1.4/pipxu/pipxu.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 import shlex
 import sys
 from pathlib import Path
 from typing import Optional
 
 import platformdirs
 
-from .run import run
 from . import utils
+from .run import run
 
 DEFUV = 'uv'
 DEFPY = 'python3'
 
 # Some constants
 MOD = Path(__file__)
 PROG = MOD.stem
```

### Comparing `pipxu-1.3/pipxu/run.py` & `pipxu-1.4/pipxu/run.py`

 * *Files identical despite different names*

### Comparing `pipxu-1.3/pipxu/utils.py` & `pipxu-1.4/pipxu/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -220,36 +220,38 @@
                 break
         else:
             return name, None
 
     path = (args._packages_dir / name).resolve()
     return name, (path if path.exists() else None)
 
+def rm_path(path: Path) -> None:
+    'Remove the given path'
+    print(f'Purging stray {path}', file=sys.stderr)
+    if path.is_dir():
+        shutil.rmtree(path)
+    else:
+        path.unlink()
+
 def purge_old_venvs(args: Namespace) -> None:
     'Clean out any old virtual environments and package names'
-    valids = set(f.resolve().name for f in args._packages_dir.iterdir())
-    vdirs = set(f.name for f in args._venvs_dir.iterdir())
-
-    # Remove any venvs that are not in the packages directory
-    for vdir in (vdirs - valids):
-        tgt = args._venvs_dir / vdir
-        print(f'Purging stray venv {tgt}', file=sys.stderr)
-        if tgt.is_dir():
-            rm_vdir(args._venvs_dir / vdir, args)
+    # Remove any packages that do not point to a dir in the venvs directory
+    valids_venvs = set()
+    for pkg in args._packages_dir.iterdir():
+        vdir = pkg.resolve()
+        if vdir.parent != args._venvs_dir or not vdir.is_dir() \
+                or not vdir.name.isdigit():
+            rm_path(pkg)
         else:
-            tgt.unlink()
+            valids_venvs.add(vdir.name)
 
-    # Remove any packages that are not in the venvs directory
-    for pkg in (valids - vdirs):
-        tgt = args._packages_dir / pkg
-        print(f'Purging stray package link {tgt}', file=sys.stderr)
-        if tgt.is_dir():
-            shutil.rmtree(tgt)
-        else:
-            tgt.unlink()
+    # Remove any venvs that are not in the packages directory
+    for vdir in args._venvs_dir.iterdir():
+        if vdir.name not in valids_venvs:
+            rm_path(vdir)
 
 def get_all_package_names(args: Namespace) -> list[str]:
     'Return a sorted list of all package names'
     return sorted(set(f.name for f in args._packages_dir.iterdir())
                   - set(args.skip or []))
 
 def get_python(args: Namespace) -> str:
```

### Comparing `pipxu-1.3/pipxu.egg-info/PKG-INFO` & `pipxu-1.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: pipxu
-Version: 1.3
-Summary: Install and Run Python Applications in Isolated Environments using UV
-Author-email: Mark Blakeney <mark.blakeney@bullet-systems.net>
-License: GPLv3
-Project-URL: Homepage, https://github.com/bulletmark/pipxu
-Keywords: pipx,pip,uv,venv,virtualenv
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Requires-Dist: filelock
-Requires-Dist: platformdirs
-Requires-Dist: importlib-metadata; python_version < "3.8"
-
 ## PIPXU - Install and Run Python Applications in Isolated Environments using UV
 [![PyPi](https://img.shields.io/pypi/v/pipxu)](https://pypi.org/project/pipxu/)
 [![AUR](https://img.shields.io/aur/version/pipxu)](https://aur.archlinux.org/packages/pipxu/)
 
 [`pipxu`][pipxu] installs Python applications, i.e. a Python packages
 which have one or more executable programs, into independent isolated
 virtual environments on your system. Each package and it's dependencies
@@ -63,49 +48,45 @@
   --man-dir MAN_DIR     specify PIPXU_MAN_DIR
   --default-python DEFAULT_PYTHON
                         path to default python executable, default="python3"
   -V, --version         just print pipxu version and exit
 
 Commands:
   {inject,install,list,reinstall-all,reinstall,runpip,uninject,uninstall-all,uninstall,upgrade-all,upgrade,version}
-    inject              Install extra packages into an application's virtual
-                        environment.
+    inject              Install extra packages into an application.
     install             Install a Python application using an isolated virtual
                         environment.
-    list                List Python applications installed by this tool.
-    reinstall-all       Reinstall all packages and their executables.
-    reinstall           Reinstall a package and it's executables.
+    list                List all applications installed by this tool.
+    reinstall-all       Reinstall all applications.
+    reinstall           Reinstall an application.
     runpip              Run pip with given arguments on virtual environment
-                        for the given package.
-    uninject            Uninstall extra packages from an application's virtual
-                        environment.
-    uninstall-all       Uninstall all Python applications and their virtual
-                        environments.
-    uninstall           Uninstall a Python application and it's virtual
-                        environment
-    upgrade-all         Upgrade all packages and their executables.
-    upgrade             Upgrade a package and it's executables.
-    version             List installed package versions.
+                        for the given application.
+    uninject            Uninstall extra packages from an application.
+    uninstall-all       Uninstall all applications.
+    uninstall           Uninstall an application.
+    upgrade-all         Upgrade all applications.
+    upgrade             Upgrade an application.
+    version             List installed application versions.
 
 Note you can set default starting global options in $HOME/.config/pipxu-
 flags.conf.
 ```
 
 Type `pipxu <command> -h` to see specific help/usage for any
 individual command:
 
 ### Command `inject`
 
 ```
 usage: pipxu inject [-h] [-v] package extras [extras ...]
 
-Install extra packages into an application's virtual environment.
+Install extra packages into an application.
 
 positional arguments:
-  package        existing package name
+  package        existing application name
   extras         extra package name[s] to inject/install
 
 options:
   -h, --help     show this help message and exit
   -v, --verbose  give more output
 ```
 
@@ -114,74 +95,74 @@
 ```
 usage: pipxu install [-h] [-p PYTHON | -P PYENV] [-f] [-e] [-d] [-v]
                            package [package ...]
 
 Install a Python application using an isolated virtual environment.
 
 positional arguments:
-  package               package[s] to install
+  package               application[s] to install
 
 options:
   -h, --help            show this help message and exit
   -p PYTHON, --python PYTHON
                         specify explicit python executable path
   -P PYENV, --pyenv PYENV
                         pyenv python version to use, i.e. from `pyenv
                         versions`, e.g. "3.9".
   -f, --force           recreate any existing venv
-  -e, --editable        install package[s] in editable mode
+  -e, --editable        install application[s] in editable mode
   -d, --include-deps    include executables from dependencies
   -v, --verbose         give more output
 ```
 
 ### Command `list`
 
 ```
 usage: pipxu list [-h] [--json] [package ...]
 
-List Python applications installed by this tool.
+List all applications installed by this tool.
 
 positional arguments:
-  package     list the given package[s] only
+  package     list the given application[s] only
 
 options:
   -h, --help  show this help message and exit
   --json      output json instead
 ```
 
 ### Command `reinstall-all`
 
 ```
 usage: pipxu reinstall-all [-h] [-p PYTHON | -P PYENV] [-v]
                                  [-s [SKIP ...]]
 
-Reinstall all packages and their executables.
+Reinstall all applications.
 
 options:
   -h, --help            show this help message and exit
   -p PYTHON, --python PYTHON
                         specify explicit python executable path
   -P PYENV, --pyenv PYENV
                         pyenv python version to use, i.e. from `pyenv
                         versions`, e.g. "3.9".
   -v, --verbose         give more output
   -s [SKIP ...], --skip [SKIP ...]
-                        skip these packages, e.g. package1 package2
+                        skip these applications, e.g. "-s package1 package2"
 ```
 
 ### Command `reinstall`
 
 ```
 usage: pipxu reinstall [-h] [-p PYTHON | -P PYENV] [-v]
                              package [package ...]
 
-Reinstall a package and it's executables.
+Reinstall an application.
 
 positional arguments:
-  package               package name[s] to upgrade
+  package               application[s] to reinstall
 
 options:
   -h, --help            show this help message and exit
   -p PYTHON, --python PYTHON
                         specify explicit python executable path
   -P PYENV, --pyenv PYENV
                         pyenv python version to use, i.e. from `pyenv
@@ -190,107 +171,107 @@
 ```
 
 ### Command `runpip`
 
 ```
 usage: pipxu runpip [-h] package [args ...]
 
-Run pip with given arguments on virtual environment for the given package.
+Run pip with given arguments on virtual environment for the given application.
 
 positional arguments:
-  package     existing package name
+  package     existing application name
   args        arguments to pass to uv pip. should start with "--".
 
 options:
   -h, --help  show this help message and exit
 ```
 
 ### Command `uninject`
 
 ```
 usage: pipxu uninject [-h] [-v] package extras [extras ...]
 
-Uninstall extra packages from an application's virtual environment.
+Uninstall extra packages from an application.
 
 positional arguments:
-  package        existing package name
+  package        existing application name
   extras         extra package name[s] to uninstall
 
 options:
   -h, --help     show this help message and exit
   -v, --verbose  give more output
 ```
 
 ### Command `uninstall-all`
 
 ```
 usage: pipxu uninstall-all [-h] [-v] [-s [SKIP ...]]
 
-Uninstall all Python applications and their virtual environments.
+Uninstall all applications.
 
 options:
   -h, --help            show this help message and exit
   -v, --verbose         give more output
   -s [SKIP ...], --skip [SKIP ...]
-                        skip these packages, e.g. package1 package2
+                        skip these applications, e.g. "-s package1 package2"
 ```
 
 ### Command `uninstall`
 
 ```
 usage: pipxu uninstall [-h] [-v] package [package ...]
 
-Uninstall a Python application and it's virtual environment
+Uninstall an application.
 
 positional arguments:
-  package        package name[s] to uninstall
+  package        application[s] to uninstall
 
 options:
   -h, --help     show this help message and exit
   -v, --verbose  give more output
 ```
 
 ### Command `upgrade-all`
 
 ```
 usage: pipxu upgrade-all [-h] [-v] [-s [SKIP ...]]
 
-Upgrade all packages and their executables.
+Upgrade all applications.
 
 options:
   -h, --help            show this help message and exit
   -v, --verbose         give more output
   -s [SKIP ...], --skip [SKIP ...]
-                        skip these packages, e.g. package1 package2
+                        skip these applications, e.g. "-s package1 package2"
 ```
 
 ### Command `upgrade`
 
 ```
 usage: pipxu upgrade [-h] [-v] package [package ...]
 
-Upgrade a package and it's executables.
+Upgrade an application.
 
 positional arguments:
-  package        package name[s] to upgrade
+  package        application[s] to upgrade
 
 options:
   -h, --help     show this help message and exit
   -v, --verbose  give more output
 ```
 
 ### Command `version`
 
 ```
 usage: pipxu version [-h] [package]
 
-List installed package versions.
+List installed application versions.
 
 positional arguments:
-  package     report specific package and dependent package versions
+  package     report specific application and dependent package versions
 
 options:
   -h, --help  show this help message and exit
 ```
 
 ## Installation and Upgrade
 
@@ -362,18 +343,14 @@
    .` or `pipxu inject . pudb`. I.e. `pipxu` automatically determines
    the package name associated with the current directory. Note that
    `pipx` accepts "`.`" for the install command, but not for any others.
 
 3. If run as root or with `sudo`, `pipxu` installs applications to a
    global location.
 
-At the time of initial release, the `pipxu` application comprises 736
-lines of Python code whereas the `pipx` application is 4300 lines of
-Python code.
-
 ## Environment Variables
 
 Type `pipxu` without any arguments to see usage and the current
 environment. The environment is printed at the bottom of the screen
 output as follows:
 
 E.g. run as my user "mark":
```

### Comparing `pipxu-1.3/pipxu.egg-info/SOURCES.txt` & `pipxu-1.4/pipxu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pipxu-1.3/pyproject.toml` & `pipxu-1.4/pyproject.toml`

 * *Files identical despite different names*

