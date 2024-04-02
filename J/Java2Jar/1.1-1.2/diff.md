# Comparing `tmp/Java2Jar-1.1.tar.gz` & `tmp/Java2Jar-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Java2Jar-1.1.tar", last modified: Tue Apr  2 11:50:56 2024, max compression
+gzip compressed data, was "Java2Jar-1.2.tar", last modified: Tue Apr  2 12:04:08 2024, max compression
```

## Comparing `Java2Jar-1.1.tar` & `Java2Jar-1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 11:50:56.051594 Java2Jar-1.1/
-drwxrwxrwx   0        0        0        0 2024-04-02 11:50:56.049585 Java2Jar-1.1/Java2Jar.egg-info/
--rw-rw-rw-   0        0        0      712 2024-04-02 11:50:55.000000 Java2Jar-1.1/Java2Jar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      166 2024-04-02 11:50:55.000000 Java2Jar-1.1/Java2Jar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 11:50:55.000000 Java2Jar-1.1/Java2Jar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 11:50:55.000000 Java2Jar-1.1/Java2Jar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      825 2024-03-31 10:49:35.000000 Java2Jar-1.1/Java2Jar.py
--rw-rw-rw-   0        0        0     1065 2024-03-31 11:10:25.000000 Java2Jar-1.1/LICENSE
--rw-rw-rw-   0        0        0      712 2024-04-02 11:50:56.051594 Java2Jar-1.1/PKG-INFO
--rw-rw-rw-   0        0        0      368 2024-04-02 10:19:48.000000 Java2Jar-1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-02 11:50:56.051594 Java2Jar-1.1/setup.cfg
--rw-rw-rw-   0        0        0      732 2024-04-02 10:31:21.000000 Java2Jar-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:04:08.109834 Java2Jar-1.2/
+drwxrwxrwx   0        0        0        0 2024-04-02 12:04:08.108834 Java2Jar-1.2/Java2Jar.egg-info/
+-rw-rw-rw-   0        0        0      712 2024-04-02 12:04:08.000000 Java2Jar-1.2/Java2Jar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      166 2024-04-02 12:04:08.000000 Java2Jar-1.2/Java2Jar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 12:04:08.000000 Java2Jar-1.2/Java2Jar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 12:04:08.000000 Java2Jar-1.2/Java2Jar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      825 2024-04-02 12:03:18.000000 Java2Jar-1.2/Java2Jar.py
+-rw-rw-rw-   0        0        0     1065 2024-03-31 11:10:25.000000 Java2Jar-1.2/LICENSE
+-rw-rw-rw-   0        0        0      712 2024-04-02 12:04:08.108834 Java2Jar-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      368 2024-04-02 10:19:48.000000 Java2Jar-1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-02 12:04:08.109834 Java2Jar-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      765 2024-04-02 12:03:32.000000 Java2Jar-1.2/setup.py
```

### Comparing `Java2Jar-1.1/Java2Jar.egg-info/PKG-INFO` & `Java2Jar-1.2/Java2Jar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Java2Jar
-Version: 1.1
+Version: 1.2
 Summary: A tool to convert Java files to JAR files
 Author: Soumalya Das
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `Java2Jar-1.1/Java2Jar.py` & `Java2Jar-1.2/Java2Jar.py`

 * *Files identical despite different names*

### Comparing `Java2Jar-1.1/LICENSE` & `Java2Jar-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Java2Jar-1.1/PKG-INFO` & `Java2Jar-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Java2Jar
-Version: 1.1
+Version: 1.2
 Summary: A tool to convert Java files to JAR files
 Author: Soumalya Das
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `Java2Jar-1.1/setup.py` & `Java2Jar-1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 # Read the contents of your README.md file
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='Java2Jar',
-    version='1.1',
+    version='1.2',
     packages=find_packages(),
-    scripts=['Java2Jar.py'],
+    scripts=['Java2Jar.py'],  # Notice the indentation here
     description='A tool to convert Java files to JAR files',
     author='Soumalya Das',
     long_description=long_description,  # Use the contents of your README.md file
     long_description_content_type='text/markdown',  # Set the content type of the long description
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
-)
+)
```

