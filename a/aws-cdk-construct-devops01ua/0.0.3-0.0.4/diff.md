# Comparing `tmp/aws_cdk_construct_devops01ua-0.0.3.tar.gz` & `tmp/aws_cdk_construct_devops01ua-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_cdk_construct_devops01ua-0.0.3.tar", last modified: Tue Apr  2 15:59:40 2024, max compression
+gzip compressed data, was "aws_cdk_construct_devops01ua-0.0.4.tar", last modified: Tue Apr  2 16:06:11 2024, max compression
```

## Comparing `aws_cdk_construct_devops01ua-0.0.3.tar` & `aws_cdk_construct_devops01ua-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxr-xr-x   0 ahrechanychenko   (501) staff       (20)        0 2024-04-02 15:59:40.579388 aws_cdk_construct_devops01ua-0.0.3/
--rw-r--r--   0 ahrechanychenko   (501) staff       (20)     1579 2024-04-02 15:59:40.578770 aws_cdk_construct_devops01ua-0.0.3/PKG-INFO
--rw-r--r--   0 ahrechanychenko   (501) staff       (20)      898 2024-04-02 15:34:46.000000 aws_cdk_construct_devops01ua-0.0.3/README.md
-drwxr-xr-x   0 ahrechanychenko   (501) staff       (20)        0 2024-04-02 15:59:40.578239 aws_cdk_construct_devops01ua-0.0.3/aws_cdk_construct_devops01ua.egg-info/
--rw-r--r--   0 ahrechanychenko   (501) staff       (20)     1579 2024-04-02 15:59:40.000000 aws_cdk_construct_devops01ua-0.0.3/aws_cdk_construct_devops01ua.egg-info/PKG-INFO
--rw-r--r--   0 ahrechanychenko   (501) staff       (20)      277 2024-04-02 15:59:40.000000 aws_cdk_construct_devops01ua-0.0.3/aws_cdk_construct_devops01ua.egg-info/SOURCES.txt
--rw-r--r--   0 ahrechanychenko   (501) staff       (20)        1 2024-04-02 15:59:40.000000 aws_cdk_construct_devops01ua-0.0.3/aws_cdk_construct_devops01ua.egg-info/dependency_links.txt
--rw-r--r--   0 ahrechanychenko   (501) staff       (20)       38 2024-04-02 15:59:40.000000 aws_cdk_construct_devops01ua-0.0.3/aws_cdk_construct_devops01ua.egg-info/requires.txt
--rw-r--r--   0 ahrechanychenko   (501) staff       (20)        1 2024-04-02 15:59:40.000000 aws_cdk_construct_devops01ua-0.0.3/aws_cdk_construct_devops01ua.egg-info/top_level.txt
--rw-r--r--   0 ahrechanychenko   (501) staff       (20)       38 2024-04-02 15:59:40.579456 aws_cdk_construct_devops01ua-0.0.3/setup.cfg
--rw-r--r--   0 ahrechanychenko   (501) staff       (20)      953 2024-04-02 15:59:05.000000 aws_cdk_construct_devops01ua-0.0.3/setup.py
+drwxr-xr-x   0 ahrechanychenko   (501) staff       (20)        0 2024-04-02 16:06:11.909496 aws_cdk_construct_devops01ua-0.0.4/
+-rw-r--r--   0 ahrechanychenko   (501) staff       (20)     1579 2024-04-02 16:06:11.908717 aws_cdk_construct_devops01ua-0.0.4/PKG-INFO
+-rw-r--r--   0 ahrechanychenko   (501) staff       (20)      898 2024-04-02 15:34:46.000000 aws_cdk_construct_devops01ua-0.0.4/README.md
+drwxr-xr-x   0 ahrechanychenko   (501) staff       (20)        0 2024-04-02 16:06:11.908212 aws_cdk_construct_devops01ua-0.0.4/aws_cdk_construct_devops01ua.egg-info/
+-rw-r--r--   0 ahrechanychenko   (501) staff       (20)     1579 2024-04-02 16:06:11.000000 aws_cdk_construct_devops01ua-0.0.4/aws_cdk_construct_devops01ua.egg-info/PKG-INFO
+-rw-r--r--   0 ahrechanychenko   (501) staff       (20)      311 2024-04-02 16:06:11.000000 aws_cdk_construct_devops01ua-0.0.4/aws_cdk_construct_devops01ua.egg-info/SOURCES.txt
+-rw-r--r--   0 ahrechanychenko   (501) staff       (20)        1 2024-04-02 16:06:11.000000 aws_cdk_construct_devops01ua-0.0.4/aws_cdk_construct_devops01ua.egg-info/dependency_links.txt
+-rw-r--r--   0 ahrechanychenko   (501) staff       (20)       38 2024-04-02 16:06:11.000000 aws_cdk_construct_devops01ua-0.0.4/aws_cdk_construct_devops01ua.egg-info/requires.txt
+-rw-r--r--   0 ahrechanychenko   (501) staff       (20)        4 2024-04-02 16:06:11.000000 aws_cdk_construct_devops01ua-0.0.4/aws_cdk_construct_devops01ua.egg-info/top_level.txt
+-rw-r--r--   0 ahrechanychenko   (501) staff       (20)       38 2024-04-02 16:06:11.909552 aws_cdk_construct_devops01ua-0.0.4/setup.cfg
+-rw-r--r--   0 ahrechanychenko   (501) staff       (20)      953 2024-04-02 16:06:06.000000 aws_cdk_construct_devops01ua-0.0.4/setup.py
+drwxr-xr-x   0 ahrechanychenko   (501) staff       (20)        0 2024-04-02 16:06:11.907434 aws_cdk_construct_devops01ua-0.0.4/vpc/
+-rw-r--r--   0 ahrechanychenko   (501) staff       (20)        0 2024-04-02 16:05:07.000000 aws_cdk_construct_devops01ua-0.0.4/vpc/__init__.py
+-rw-r--r--   0 ahrechanychenko   (501) staff       (20)     2185 2024-04-02 15:25:22.000000 aws_cdk_construct_devops01ua-0.0.4/vpc/constructs.py
```

### Comparing `aws_cdk_construct_devops01ua-0.0.3/PKG-INFO` & `aws_cdk_construct_devops01ua-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws_cdk_construct_devops01ua
-Version: 0.0.3
+Version: 0.0.4
 Summary: Sample of custom AWS CDK construct for demo purposes
 Author: Artem Hrechanychenko
 Author-email: devops01ua@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `aws_cdk_construct_devops01ua-0.0.3/README.md` & `aws_cdk_construct_devops01ua-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `aws_cdk_construct_devops01ua-0.0.3/aws_cdk_construct_devops01ua.egg-info/PKG-INFO` & `aws_cdk_construct_devops01ua-0.0.4/aws_cdk_construct_devops01ua.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws_cdk_construct_devops01ua
-Version: 0.0.3
+Version: 0.0.4
 Summary: Sample of custom AWS CDK construct for demo purposes
 Author: Artem Hrechanychenko
 Author-email: devops01ua@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `aws_cdk_construct_devops01ua-0.0.3/setup.py` & `aws_cdk_construct_devops01ua-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='aws_cdk_construct_devops01ua',  # Replace with your package name
-    version='0.0.3',  # Replace with your package version
+    version='0.0.4',  # Replace with your package version
     author='Artem Hrechanychenko',
     author_email='devops01ua@gmail.com',
     description='Sample of custom AWS CDK construct for demo purposes',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

