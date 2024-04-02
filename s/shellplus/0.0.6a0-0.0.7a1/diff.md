# Comparing `tmp/shellplus-0.0.6a0.tar.gz` & `tmp/shellplus-0.0.7a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellplus-0.0.6a0.tar", last modified: Sun Jan 28 12:54:47 2024, max compression
+gzip compressed data, was "shellplus-0.0.7a1.tar", last modified: Tue Apr  2 09:53:04 2024, max compression
```

## Comparing `shellplus-0.0.6a0.tar` & `shellplus-0.0.7a1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-01-28 12:54:47.334581 shellplus-0.0.6a0/
--rw-rw-rw-   0        0        0     1077 2024-01-28 12:54:47.333580 shellplus-0.0.6a0/PKG-INFO
--rw-rw-rw-   0        0        0      775 2024-01-26 16:03:46.000000 shellplus-0.0.6a0/README.md
--rw-rw-rw-   0        0        0       42 2024-01-28 12:54:47.334581 shellplus-0.0.6a0/setup.cfg
--rw-rw-rw-   0        0        0      714 2024-01-28 12:49:12.000000 shellplus-0.0.6a0/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-28 12:54:47.323461 shellplus-0.0.6a0/shellplus/
--rw-rw-rw-   0        0        0        0 2024-01-26 10:57:43.000000 shellplus-0.0.6a0/shellplus/__init__.py
--rw-rw-rw-   0        0        0      705 2024-01-26 15:26:13.000000 shellplus-0.0.6a0/shellplus/colors1.py
--rw-rw-rw-   0        0        0      653 2024-01-28 12:43:30.000000 shellplus-0.0.6a0/shellplus/styles.py
-drwxrwxrwx   0        0        0        0 2024-01-28 12:54:47.332577 shellplus-0.0.6a0/shellplus.egg-info/
--rw-rw-rw-   0        0        0     1077 2024-01-28 12:54:47.000000 shellplus-0.0.6a0/shellplus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2024-01-28 12:54:47.000000 shellplus-0.0.6a0/shellplus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-28 12:54:47.000000 shellplus-0.0.6a0/shellplus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-01-28 12:54:47.000000 shellplus-0.0.6a0/shellplus.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-01-28 12:54:47.000000 shellplus-0.0.6a0/shellplus.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 09:53:04.341572 shellplus-0.0.7a1/
+-rw-rw-rw-   0        0        0     1077 2024-04-02 09:53:04.339570 shellplus-0.0.7a1/PKG-INFO
+-rw-rw-rw-   0        0        0      775 2024-01-26 16:03:46.000000 shellplus-0.0.7a1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-02 09:53:04.341572 shellplus-0.0.7a1/setup.cfg
+-rw-rw-rw-   0        0        0      780 2024-04-02 09:52:47.000000 shellplus-0.0.7a1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 09:53:04.329785 shellplus-0.0.7a1/shellplus/
+-rw-rw-rw-   0        0        0        0 2024-01-26 10:57:43.000000 shellplus-0.0.7a1/shellplus/__init__.py
+-rw-rw-rw-   0        0        0      743 2024-04-02 09:16:37.000000 shellplus-0.0.7a1/shellplus/colors1.py
+-rw-rw-rw-   0        0        0     1060 2024-04-02 09:11:30.000000 shellplus-0.0.7a1/shellplus/styles.py
+drwxrwxrwx   0        0        0        0 2024-04-02 09:53:04.338568 shellplus-0.0.7a1/shellplus.egg-info/
+-rw-rw-rw-   0        0        0     1077 2024-04-02 09:53:04.000000 shellplus-0.0.7a1/shellplus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2024-04-02 09:53:04.000000 shellplus-0.0.7a1/shellplus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 09:53:04.000000 shellplus-0.0.7a1/shellplus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-02 09:53:04.000000 shellplus-0.0.7a1/shellplus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-02 09:53:04.000000 shellplus-0.0.7a1/shellplus.egg-info/top_level.txt
```

### Comparing `shellplus-0.0.6a0/PKG-INFO` & `shellplus-0.0.7a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellplus
-Version: 0.0.6a0
+Version: 0.0.7a1
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: Public Domain
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Requires-Dist: rich
```

### Comparing `shellplus-0.0.6a0/README.md` & `shellplus-0.0.7a1/README.md`

 * *Files identical despite different names*

### Comparing `shellplus-0.0.6a0/setup.py` & `shellplus-0.0.7a1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 
 # Read the contents of your README file
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='shellplus',
-    version='0.0.6a',
+    version='0.0.7a01',
     packages=find_packages(),
     install_requires=[
         'rich',  # Add any other dependencies here
     ],
+    setup_requires=['wheel'],  # Add 'wheel' to setup_requires
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: Public Domain',
         'Programming Language :: Python :: 3.11',
     ],
     # Add the long_description field
```

### Comparing `shellplus-0.0.6a0/shellplus/colors1.py` & `shellplus-0.0.7a1/shellplus/colors1.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
     'gum pink': color('#f8369d'),
     'bubblegum': color('#f8369d'),
 
     'green apple': color('#b3e52a'),
     'sour apple': color('#b3e52a'),
     'greenyellow': color('#b3e52a'),
+    'yellowgreen': color('#b3e52a'),
 
     'diva': color('#ccace3'),
 
     'navy': color('#020563'),
 
     'dark teal': color('#55aa88'),
     'dteal': color('#55aa88')
```

### Comparing `shellplus-0.0.6a0/shellplus.egg-info/PKG-INFO` & `shellplus-0.0.7a1/shellplus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellplus
-Version: 0.0.6a0
+Version: 0.0.7a1
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: Public Domain
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Requires-Dist: rich
```

