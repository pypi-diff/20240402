# Comparing `tmp/strings_repository-0.1.0.tar.gz` & `tmp/strings_repository-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strings_repository-0.1.0.tar", last modified: Wed Nov  8 07:13:29 2023, max compression
+gzip compressed data, was "strings_repository-0.2.0.tar", last modified: Tue Apr  2 09:50:25 2024, max compression
```

## Comparing `strings_repository-0.1.0.tar` & `strings_repository-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 heretrix   (501) staff       (20)        0 2023-11-08 07:13:29.499928 strings_repository-0.1.0/
--rw-r--r--   0 heretrix   (501) staff       (20)     1065 2023-11-06 09:55:10.000000 strings_repository-0.1.0/LICENSE
--rw-r--r--   0 heretrix   (501) staff       (20)      718 2023-11-08 07:13:29.499534 strings_repository-0.1.0/PKG-INFO
--rw-r--r--   0 heretrix   (501) staff       (20)      944 2023-11-08 07:06:39.000000 strings_repository-0.1.0/README.md
-drwxr-xr-x   0 heretrix   (501) staff       (20)        0 2023-11-08 07:13:29.488320 strings_repository-0.1.0/bin/
--rwxr-xr-x   0 heretrix   (501) staff       (20)       68 2023-11-06 11:01:29.000000 strings_repository-0.1.0/bin/strings_repository
--rw-r--r--   0 heretrix   (501) staff       (20)       38 2023-11-08 07:13:29.500731 strings_repository-0.1.0/setup.cfg
--rw-r--r--   0 heretrix   (501) staff       (20)     1055 2023-11-08 07:12:07.000000 strings_repository-0.1.0/setup.py
-drwxr-xr-x   0 heretrix   (501) staff       (20)        0 2023-11-08 07:13:29.490128 strings_repository-0.1.0/strings_repository/
--rw-r--r--   0 heretrix   (501) staff       (20)        0 2023-11-06 10:18:52.000000 strings_repository-0.1.0/strings_repository/__init__.py
--rw-r--r--   0 heretrix   (501) staff       (20)      103 2023-11-06 10:20:38.000000 strings_repository-0.1.0/strings_repository/__main__.py
--rw-r--r--   0 heretrix   (501) staff       (20)     1685 2023-11-08 06:40:05.000000 strings_repository-0.1.0/strings_repository/cli.py
--rw-r--r--   0 heretrix   (501) staff       (20)     2271 2023-11-08 06:42:29.000000 strings_repository-0.1.0/strings_repository/strings_repository.py
-drwxr-xr-x   0 heretrix   (501) staff       (20)        0 2023-11-08 07:13:29.498871 strings_repository-0.1.0/strings_repository.egg-info/
--rw-r--r--   0 heretrix   (501) staff       (20)      718 2023-11-08 07:13:29.000000 strings_repository-0.1.0/strings_repository.egg-info/PKG-INFO
--rw-r--r--   0 heretrix   (501) staff       (20)      397 2023-11-08 07:13:29.000000 strings_repository-0.1.0/strings_repository.egg-info/SOURCES.txt
--rw-r--r--   0 heretrix   (501) staff       (20)        1 2023-11-08 07:13:29.000000 strings_repository-0.1.0/strings_repository.egg-info/dependency_links.txt
--rw-r--r--   0 heretrix   (501) staff       (20)       22 2023-11-08 07:13:29.000000 strings_repository-0.1.0/strings_repository.egg-info/requires.txt
--rw-r--r--   0 heretrix   (501) staff       (20)       19 2023-11-08 07:13:29.000000 strings_repository-0.1.0/strings_repository.egg-info/top_level.txt
+drwxr-xr-x   0 heretrix   (501) staff       (20)        0 2024-04-02 09:50:25.496626 strings_repository-0.2.0/
+-rw-r--r--   0 heretrix   (501) staff       (20)     1065 2023-11-06 09:55:10.000000 strings_repository-0.2.0/LICENSE
+-rw-r--r--   0 heretrix   (501) staff       (20)      718 2024-04-02 09:50:25.496408 strings_repository-0.2.0/PKG-INFO
+-rw-r--r--   0 heretrix   (501) staff       (20)     1002 2023-11-08 07:32:43.000000 strings_repository-0.2.0/README.md
+drwxr-xr-x   0 heretrix   (501) staff       (20)        0 2024-04-02 09:50:25.480074 strings_repository-0.2.0/bin/
+-rwxr-xr-x   0 heretrix   (501) staff       (20)       68 2023-11-06 11:01:29.000000 strings_repository-0.2.0/bin/strings_repository
+-rw-r--r--   0 heretrix   (501) staff       (20)       79 2024-04-02 09:50:25.498450 strings_repository-0.2.0/setup.cfg
+-rw-r--r--   0 heretrix   (501) staff       (20)     1055 2024-04-02 09:13:36.000000 strings_repository-0.2.0/setup.py
+drwxr-xr-x   0 heretrix   (501) staff       (20)        0 2024-04-02 09:50:25.488869 strings_repository-0.2.0/strings_repository/
+-rw-r--r--   0 heretrix   (501) staff       (20)        0 2023-11-06 10:18:52.000000 strings_repository-0.2.0/strings_repository/__init__.py
+-rw-r--r--   0 heretrix   (501) staff       (20)      103 2023-11-06 10:20:38.000000 strings_repository-0.2.0/strings_repository/__main__.py
+-rw-r--r--   0 heretrix   (501) staff       (20)     1685 2024-03-12 11:29:59.000000 strings_repository-0.2.0/strings_repository/cli.py
+-rw-r--r--   0 heretrix   (501) staff       (20)     2371 2024-04-02 09:12:38.000000 strings_repository-0.2.0/strings_repository/strings_repository.py
+drwxr-xr-x   0 heretrix   (501) staff       (20)        0 2024-04-02 09:50:25.495902 strings_repository-0.2.0/strings_repository.egg-info/
+-rw-r--r--   0 heretrix   (501) staff       (20)      718 2024-04-02 09:50:25.000000 strings_repository-0.2.0/strings_repository.egg-info/PKG-INFO
+-rw-r--r--   0 heretrix   (501) staff       (20)      397 2024-04-02 09:50:25.000000 strings_repository-0.2.0/strings_repository.egg-info/SOURCES.txt
+-rw-r--r--   0 heretrix   (501) staff       (20)        1 2024-04-02 09:50:25.000000 strings_repository-0.2.0/strings_repository.egg-info/dependency_links.txt
+-rw-r--r--   0 heretrix   (501) staff       (20)       22 2024-04-02 09:50:25.000000 strings_repository-0.2.0/strings_repository.egg-info/requires.txt
+-rw-r--r--   0 heretrix   (501) staff       (20)       19 2024-04-02 09:50:25.000000 strings_repository-0.2.0/strings_repository.egg-info/top_level.txt
```

### Comparing `strings_repository-0.1.0/LICENSE` & `strings_repository-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `strings_repository-0.1.0/PKG-INFO` & `strings_repository-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strings_repository
-Version: 0.1.0
+Version: 0.2.0
 Summary: Simple commandline tool for pulling data from strings repository (https://github.com/HereTrix/strings_repository)
 Home-page: https://github.com/HereTrix/strings_repository_cli
 Download-URL: https://github.com/HereTrix/strings_repository_cli/archive/refs/tags/0.1.0.tar.gz
 Author: HereTrix
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `strings_repository-0.1.0/README.md` & `strings_repository-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 
 Overview
 --------
 Application utilize `strings_repository.yaml` file for configuration. It is possible to use custom environment variable to store access token or put it directly into file. Environment variable usage is highly recommended.
 
 Installation
 -------
+Install via `pip install strings_repository` 
 
-Clone repository and launch `pip install .`
+or manually clone repository and launch `pip install .`
 
 Usage
 -------
 To create configuration file run `strings_repository init` command and follow instructions.
 
 Alternatively you can create `strings_repository.yaml` file manually.
 Example:
```

### Comparing `strings_repository-0.1.0/setup.py` & `strings_repository-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='strings_repository',
-    version='0.1.0',
+    version='0.2.0',
     description='Simple commandline tool for pulling data from strings repository (https://github.com/HereTrix/strings_repository)',
     url='https://github.com/HereTrix/strings_repository_cli',
     download_url='https://github.com/HereTrix/strings_repository_cli/archive/refs/tags/0.1.0.tar.gz',
     author='HereTrix',
     license='MIT',
     packages=['strings_repository'],
     install_requires=[
```

### Comparing `strings_repository-0.1.0/strings_repository/cli.py` & `strings_repository-0.2.0/strings_repository/cli.py`

 * *Files identical despite different names*

### Comparing `strings_repository-0.1.0/strings_repository/strings_repository.py` & `strings_repository-0.2.0/strings_repository/strings_repository.py`

 * *Files 11% similar despite different names*

```diff
@@ -65,30 +65,35 @@
         if tags:
             data['tags'] = tags
 
         langs = config_data.get(LANGUAGES_KEY)
         if langs:
             data['codes'] = langs
 
+        print('Fetching data...')
+
         url = config_data[HOST_KEY] + '/api/plugin/export'
         response = requests.post(
             url=url,
             data=data,
             headers={
                 'Access-Token': api_key
             },
         )
 
+        print('Unpacking...')
+
         with tempfile.NamedTemporaryFile(delete=True) as tmp:
             tmp.write(response.content)
             tmp.seek(0)
 
             config_path = config_data[PATH_KEY]
             working_dir = os.getcwd()
             path = os.path.join(working_dir, config_path)
 
             unzip = zipfile.ZipFile(tmp)
             unzip.extractall(path)
+            print('Completed...')
 
 
 if __name__ == "__main__":
     App.pull()
```

### Comparing `strings_repository-0.1.0/strings_repository.egg-info/PKG-INFO` & `strings_repository-0.2.0/strings_repository.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: strings-repository
-Version: 0.1.0
+Name: strings_repository
+Version: 0.2.0
 Summary: Simple commandline tool for pulling data from strings repository (https://github.com/HereTrix/strings_repository)
 Home-page: https://github.com/HereTrix/strings_repository_cli
 Download-URL: https://github.com/HereTrix/strings_repository_cli/archive/refs/tags/0.1.0.tar.gz
 Author: HereTrix
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

