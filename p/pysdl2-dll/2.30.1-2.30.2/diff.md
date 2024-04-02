# Comparing `tmp/pysdl2-dll-2.30.1.tar.gz` & `tmp/pysdl2-dll-2.30.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysdl2-dll-2.30.1.tar", last modified: Mon Apr  1 03:14:17 2024, max compression
+gzip compressed data, was "pysdl2-dll-2.30.2.tar", last modified: Tue Apr  2 14:00:53 2024, max compression
```

## Comparing `pysdl2-dll-2.30.1.tar` & `pysdl2-dll-2.30.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 03:14:17.992820 pysdl2-dll-2.30.1/
--rw-r--r--   0 root         (0) root         (0)    16725 2024-04-01 03:14:16.000000 pysdl2-dll-2.30.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       34 2024-04-01 03:14:16.000000 pysdl2-dll-2.30.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3938 2024-04-01 03:14:17.992820 pysdl2-dll-2.30.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3165 2024-04-01 03:14:16.000000 pysdl2-dll-2.30.1/README.md
--rw-r--r--   0 root         (0) root         (0)    19649 2024-04-01 03:14:16.000000 pysdl2-dll-2.30.1/getdlls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 03:14:17.992820 pysdl2-dll-2.30.1/pysdl2_dll.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3938 2024-04-01 03:14:17.000000 pysdl2-dll-2.30.1/pysdl2_dll.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      261 2024-04-01 03:14:17.000000 pysdl2-dll-2.30.1/pysdl2_dll.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-01 03:14:17.000000 pysdl2-dll-2.30.1/pysdl2_dll.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-01 03:14:17.000000 pysdl2-dll-2.30.1/pysdl2_dll.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 03:14:17.992820 pysdl2-dll-2.30.1/sdl2dll/
--rw-r--r--   0 root         (0) root         (0)      419 2024-04-01 03:14:16.000000 pysdl2-dll-2.30.1/sdl2dll/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 03:14:17.992820 pysdl2-dll-2.30.1/sdl2dll/dll/
--rw-r--r--   0 root         (0) root         (0)       36 2024-04-01 03:14:17.000000 pysdl2-dll-2.30.1/sdl2dll/dll/.unsupported
--rw-r--r--   0 root         (0) root         (0)     2567 2024-04-01 03:14:16.000000 pysdl2-dll-2.30.1/sdl2dll/initcheck.py
--rw-r--r--   0 root         (0) root         (0)      116 2024-04-01 03:14:17.992820 pysdl2-dll-2.30.1/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     2534 2024-04-01 03:14:16.000000 pysdl2-dll-2.30.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 14:00:53.479080 pysdl2-dll-2.30.2/
+-rw-r--r--   0 root         (0) root         (0)    16725 2024-04-02 14:00:52.000000 pysdl2-dll-2.30.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       34 2024-04-02 14:00:52.000000 pysdl2-dll-2.30.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3938 2024-04-02 14:00:53.479080 pysdl2-dll-2.30.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3165 2024-04-02 14:00:52.000000 pysdl2-dll-2.30.2/README.md
+-rw-r--r--   0 root         (0) root         (0)    19649 2024-04-02 14:00:52.000000 pysdl2-dll-2.30.2/getdlls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 14:00:53.478079 pysdl2-dll-2.30.2/pysdl2_dll.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3938 2024-04-02 14:00:53.000000 pysdl2-dll-2.30.2/pysdl2_dll.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      261 2024-04-02 14:00:53.000000 pysdl2-dll-2.30.2/pysdl2_dll.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 14:00:53.000000 pysdl2-dll-2.30.2/pysdl2_dll.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-02 14:00:53.000000 pysdl2-dll-2.30.2/pysdl2_dll.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 14:00:53.479080 pysdl2-dll-2.30.2/sdl2dll/
+-rw-r--r--   0 root         (0) root         (0)      419 2024-04-02 14:00:52.000000 pysdl2-dll-2.30.2/sdl2dll/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 14:00:53.479080 pysdl2-dll-2.30.2/sdl2dll/dll/
+-rw-r--r--   0 root         (0) root         (0)       36 2024-04-02 14:00:53.000000 pysdl2-dll-2.30.2/sdl2dll/dll/.unsupported
+-rw-r--r--   0 root         (0) root         (0)     2567 2024-04-02 14:00:52.000000 pysdl2-dll-2.30.2/sdl2dll/initcheck.py
+-rw-r--r--   0 root         (0) root         (0)      116 2024-04-02 14:00:53.479080 pysdl2-dll-2.30.2/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     2534 2024-04-02 14:00:52.000000 pysdl2-dll-2.30.2/setup.py
```

### Comparing `pysdl2-dll-2.30.1/LICENSE` & `pysdl2-dll-2.30.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pysdl2-dll-2.30.1/PKG-INFO` & `pysdl2-dll-2.30.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysdl2-dll
-Version: 2.30.1
+Version: 2.30.2
 Summary: Pre-built SDL2 binaries for PySDL2
 Home-page: https://github.com/a-hurst/pysdl2-dll
 Author: Austin Hurst
 Author-email: mynameisaustinhurst@gmail.com
 License: Mozilla Public License Version 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
@@ -27,15 +27,15 @@
 
 It uses the official SDL2, SDL2\_mixer, SDL2\_ttf, and SDL2\_image binaries for macOS and Windows, as well as [unofficial SDL2\_gfx binaries](https://github.com/a-hurst/sdl2gfx-builds) for the same platforms. For Linux, the SDL2 binaries and their dependencies are all built from source using the official Python [manylinux](https://github.com/pypa/manylinux) images for maximum compatibility.
 
 The latest release includes the following versions of the SDL2 binaries:
 
 SDL2 | SDL2\_ttf | SDL2\_mixer | SDL2\_image | SDL2\_gfx
 --- | --- | --- | --- | ---
-2.30.1 | 2.22.0 | 2.8.0 | 2.8.2 | 1.0.4
+2.30.2 | 2.22.0 | 2.8.0 | 2.8.2 | 1.0.4
 
 
 ## Installation
 
 You can install the latest version of pysdl2-dll via pip:
 
 ```bash
```

### Comparing `pysdl2-dll-2.30.1/README.md` & `pysdl2-dll-2.30.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 It uses the official SDL2, SDL2\_mixer, SDL2\_ttf, and SDL2\_image binaries for macOS and Windows, as well as [unofficial SDL2\_gfx binaries](https://github.com/a-hurst/sdl2gfx-builds) for the same platforms. For Linux, the SDL2 binaries and their dependencies are all built from source using the official Python [manylinux](https://github.com/pypa/manylinux) images for maximum compatibility.
 
 The latest release includes the following versions of the SDL2 binaries:
 
 SDL2 | SDL2\_ttf | SDL2\_mixer | SDL2\_image | SDL2\_gfx
 --- | --- | --- | --- | ---
-2.30.1 | 2.22.0 | 2.8.0 | 2.8.2 | 1.0.4
+2.30.2 | 2.22.0 | 2.8.0 | 2.8.2 | 1.0.4
 
 
 ## Installation
 
 You can install the latest version of pysdl2-dll via pip:
 
 ```bash
```

### Comparing `pysdl2-dll-2.30.1/getdlls.py` & `pysdl2-dll-2.30.2/getdlls.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 except ImportError:
     from urllib2 import urlopen # Python 2
 
 
 libraries = ['SDL2', 'SDL2_mixer', 'SDL2_ttf', 'SDL2_image', 'SDL2_gfx']
 
 libversions = {
-    'SDL2': '2.30.1',
+    'SDL2': '2.30.2',
     'SDL2_mixer': '2.8.0',
     'SDL2_ttf': '2.22.0',
     'SDL2_image': '2.8.2',
     'SDL2_gfx': '1.0.4'
 }
 
 url_fmt = 'https://github.com/libsdl-org/SDL{LIB}/releases/download/release-{0}/SDL2{LIB}-{0}{1}'
```

### Comparing `pysdl2-dll-2.30.1/pysdl2_dll.egg-info/PKG-INFO` & `pysdl2-dll-2.30.2/pysdl2_dll.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysdl2-dll
-Version: 2.30.1
+Version: 2.30.2
 Summary: Pre-built SDL2 binaries for PySDL2
 Home-page: https://github.com/a-hurst/pysdl2-dll
 Author: Austin Hurst
 Author-email: mynameisaustinhurst@gmail.com
 License: Mozilla Public License Version 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
@@ -27,15 +27,15 @@
 
 It uses the official SDL2, SDL2\_mixer, SDL2\_ttf, and SDL2\_image binaries for macOS and Windows, as well as [unofficial SDL2\_gfx binaries](https://github.com/a-hurst/sdl2gfx-builds) for the same platforms. For Linux, the SDL2 binaries and their dependencies are all built from source using the official Python [manylinux](https://github.com/pypa/manylinux) images for maximum compatibility.
 
 The latest release includes the following versions of the SDL2 binaries:
 
 SDL2 | SDL2\_ttf | SDL2\_mixer | SDL2\_image | SDL2\_gfx
 --- | --- | --- | --- | ---
-2.30.1 | 2.22.0 | 2.8.0 | 2.8.2 | 1.0.4
+2.30.2 | 2.22.0 | 2.8.0 | 2.8.2 | 1.0.4
 
 
 ## Installation
 
 You can install the latest version of pysdl2-dll via pip:
 
 ```bash
```

### Comparing `pysdl2-dll-2.30.1/sdl2dll/initcheck.py` & `pysdl2-dll-2.30.2/sdl2dll/initcheck.py`

 * *Files identical despite different names*

### Comparing `pysdl2-dll-2.30.1/setup.py` & `pysdl2-dll-2.30.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 # Install the package
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
 	name='pysdl2-dll',
-	version='2.30.1',
+	version='2.30.2',
 	author='Austin Hurst',
 	author_email='mynameisaustinhurst@gmail.com',
     license='Mozilla Public License Version 2.0',
     description='Pre-built SDL2 binaries for PySDL2',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/a-hurst/pysdl2-dll',
```

