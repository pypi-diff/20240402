# Comparing `tmp/SecuMas-0.0.1.3.tar.gz` & `tmp/SecuMas-0.0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SecuMas-0.0.1.3.tar", last modified: Fri Mar 15 15:49:36 2024, max compression
+gzip compressed data, was "SecuMas-0.0.1.4.tar", last modified: Tue Apr  2 08:02:03 2024, max compression
```

## Comparing `SecuMas-0.0.1.3.tar` & `SecuMas-0.0.1.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 deolekar   (501) staff       (20)        0 2024-03-15 15:49:36.226194 SecuMas-0.0.1.3/
--rw-r--r--   0 deolekar   (501) staff       (20)     1054 2024-03-14 14:41:48.000000 SecuMas-0.0.1.3/LICENSE
--rw-r--r--   0 deolekar   (501) staff       (20)     2182 2024-03-15 15:49:36.225546 SecuMas-0.0.1.3/PKG-INFO
--rw-rw-r--   0 deolekar   (501) staff       (20)     1091 2024-03-15 15:42:35.000000 SecuMas-0.0.1.3/README.md
-drwxr-xr-x   0 deolekar   (501) staff       (20)        0 2024-03-15 15:49:36.222582 SecuMas-0.0.1.3/SecuMas/
--rw-rw-r--   0 deolekar   (501) staff       (20)       95 2024-03-14 21:57:54.000000 SecuMas-0.0.1.3/SecuMas/__init__.py
--rw-r--r--   0 deolekar   (501) staff       (20)     1342 2024-03-15 10:16:07.000000 SecuMas-0.0.1.3/SecuMas/cusip.py
--rw-r--r--   0 deolekar   (501) staff       (20)     1424 2024-03-14 14:20:37.000000 SecuMas-0.0.1.3/SecuMas/isin.py
--rw-rw-r--   0 deolekar   (501) staff       (20)       34 2024-03-14 14:33:47.000000 SecuMas-0.0.1.3/SecuMas/main.py
-drwxr-xr-x   0 deolekar   (501) staff       (20)        0 2024-03-15 15:49:36.224985 SecuMas-0.0.1.3/SecuMas.egg-info/
--rw-r--r--   0 deolekar   (501) staff       (20)     2182 2024-03-15 15:49:36.000000 SecuMas-0.0.1.3/SecuMas.egg-info/PKG-INFO
--rw-r--r--   0 deolekar   (501) staff       (20)      219 2024-03-15 15:49:36.000000 SecuMas-0.0.1.3/SecuMas.egg-info/SOURCES.txt
--rw-r--r--   0 deolekar   (501) staff       (20)        1 2024-03-15 15:49:36.000000 SecuMas-0.0.1.3/SecuMas.egg-info/dependency_links.txt
--rw-r--r--   0 deolekar   (501) staff       (20)        8 2024-03-15 15:49:36.000000 SecuMas-0.0.1.3/SecuMas.egg-info/top_level.txt
--rw-r--r--   0 deolekar   (501) staff       (20)       38 2024-03-15 15:49:36.226339 SecuMas-0.0.1.3/setup.cfg
--rw-rw-r--   0 deolekar   (501) staff       (20)     1423 2024-03-15 15:49:32.000000 SecuMas-0.0.1.3/setup.py
+drwxr-xr-x   0 deolekar   (501) staff       (20)        0 2024-04-02 08:02:03.406991 SecuMas-0.0.1.4/
+-rw-r--r--   0 deolekar   (501) staff       (20)     1054 2024-03-14 14:41:48.000000 SecuMas-0.0.1.4/LICENSE
+-rw-r--r--   0 deolekar   (501) staff       (20)     2594 2024-04-02 08:02:03.406576 SecuMas-0.0.1.4/PKG-INFO
+-rw-rw-r--   0 deolekar   (501) staff       (20)     1160 2024-03-17 22:23:14.000000 SecuMas-0.0.1.4/README.md
+drwxr-xr-x   0 deolekar   (501) staff       (20)        0 2024-04-02 08:02:03.405007 SecuMas-0.0.1.4/SecuMas/
+-rw-rw-r--   0 deolekar   (501) staff       (20)      131 2024-03-16 22:38:39.000000 SecuMas-0.0.1.4/SecuMas/__init__.py
+-rw-r--r--   0 deolekar   (501) staff       (20)     1342 2024-04-02 07:44:47.000000 SecuMas-0.0.1.4/SecuMas/cusip.py
+-rw-r--r--   0 deolekar   (501) staff       (20)     1340 2024-04-02 07:44:34.000000 SecuMas-0.0.1.4/SecuMas/isin.py
+-rw-rw-r--   0 deolekar   (501) staff       (20)       34 2024-03-14 14:33:47.000000 SecuMas-0.0.1.4/SecuMas/main.py
+-rw-r--r--   0 deolekar   (501) staff       (20)     1160 2024-04-02 07:44:55.000000 SecuMas-0.0.1.4/SecuMas/sedol.py
+drwxr-xr-x   0 deolekar   (501) staff       (20)        0 2024-04-02 08:02:03.406112 SecuMas-0.0.1.4/SecuMas.egg-info/
+-rw-r--r--   0 deolekar   (501) staff       (20)     2594 2024-04-02 08:02:03.000000 SecuMas-0.0.1.4/SecuMas.egg-info/PKG-INFO
+-rw-r--r--   0 deolekar   (501) staff       (20)      236 2024-04-02 08:02:03.000000 SecuMas-0.0.1.4/SecuMas.egg-info/SOURCES.txt
+-rw-r--r--   0 deolekar   (501) staff       (20)        1 2024-04-02 08:02:03.000000 SecuMas-0.0.1.4/SecuMas.egg-info/dependency_links.txt
+-rw-r--r--   0 deolekar   (501) staff       (20)        8 2024-04-02 08:02:03.000000 SecuMas-0.0.1.4/SecuMas.egg-info/top_level.txt
+-rw-r--r--   0 deolekar   (501) staff       (20)       38 2024-04-02 08:02:03.407183 SecuMas-0.0.1.4/setup.cfg
+-rw-rw-r--   0 deolekar   (501) staff       (20)     1423 2024-03-15 17:11:03.000000 SecuMas-0.0.1.4/setup.py
```

### Comparing `SecuMas-0.0.1.3/LICENSE` & `SecuMas-0.0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `SecuMas-0.0.1.3/PKG-INFO` & `SecuMas-0.0.1.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,62 @@
 Metadata-Version: 2.1
 Name: SecuMas
-Version: 0.0.1.3
+Version: 0.0.1.4
 Summary: An application build for Securities Master platform
 Home-page: https://secumas.dev
 Author: A Deolekar
 Author-email: sher.buk@gmail.com
 License: MIT License
 Project-URL: Documentation, https://secumas.dev/
 Project-URL: Source, https://github.com/deolekar/SecuMas
+Description: # Introduction
+        
+        This Repo is for Securities Master Python custom package built.
+        
+        ```batch
+        pip install SecuMas
+        ```
+        
+        Examples:
+        
+        ```python
+        import SecuMas
+        
+        ''' Validate (ISIN)'''
+        print (SecuMas.isin.validate('IN8081309367'))
+        
+        ''' Generate Dummy ISINs (development usecase)'''
+        print (SecuMas.isin.dummy(5))
+        
+        ```
+        
+        # Package documentation
+        
+        > [Documentation](https://www.secumas.dev/)
+        
+        # Code contributions
+        
+        > [Check ToDo](https://github.com/deolekar/MMjs/blob/main/ToDo.txt)
+        
+        Improvements to SecuMas are most welcome. Integrating contributions will be done on a best-effort basis and can be made easier if the following are considered:
+        
+        Contributions are made as GitHub pull requests.
+        
+        Submitted contributions will often be reformatted and sometimes restructured for consistency with other parts.
+        
+        Contributions will be acknowledged in the release notes.
+        
+        Contributions should add or update a copyright statement if you feel the contribution is significant.
+        
+        All contribution should be made with compatible applicable copyright.
+        
+        It is not needed to modify the README.md, it will be updated on release.
+        
+        All code should be well tested and achieve 100% code coverage.
+        
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
@@ -20,51 +65,7 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 2 - Pre-Alpha
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Introduction
-
-This Repo is for Securities Master Python custom package built.
-
-```batch
-pip install SecuMas
-```
-
-Examples:
-
-```python
-import SecuMas
-
-''' Validate (ISIN)'''
-print (SecuMas.isin.validate('IN8081309367'))
-
-''' Generate Dummy ISINs (development usecase)'''
-print (SecuMas.isin.dummy(5))
-
-```
-
-# Package documentation
-
-> [Documentation](https://www.secumas.dev/)
-
-# Code contributions
-
-Improvements to SecuMas are most welcome. Integrating contributions will be done on a best-effort basis and can be made easier if the following are considered:
-
-Contributions are made as GitHub pull requests.
-
-Submitted contributions will often be reformatted and sometimes restructured for consistency with other parts.
-
-Contributions will be acknowledged in the release notes.
-
-Contributions should add or update a copyright statement if you feel the contribution is significant.
-
-All contribution should be made with compatible applicable copyright.
-
-It is not needed to modify the README.md, it will be updated on release.
-
-All code should be well tested and achieve 100% code coverage.
```

### Comparing `SecuMas-0.0.1.3/README.md` & `SecuMas-0.0.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 
 # Package documentation
 
 > [Documentation](https://www.secumas.dev/)
 
 # Code contributions
 
+> [Check ToDo](https://github.com/deolekar/MMjs/blob/main/ToDo.txt)
+
 Improvements to SecuMas are most welcome. Integrating contributions will be done on a best-effort basis and can be made easier if the following are considered:
 
 Contributions are made as GitHub pull requests.
 
 Submitted contributions will often be reformatted and sometimes restructured for consistency with other parts.
 
 Contributions will be acknowledged in the release notes.
```

### Comparing `SecuMas-0.0.1.3/SecuMas/cusip.py` & `SecuMas-0.0.1.4/SecuMas/cusip.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     """Calculate the check digit of CUSIP."""
     # convert to numeric first, then sum individual digits
     identifier = ''.join(
         str((1, 2)[i % 2] * _characterSet.index(n)) for i, n in enumerate(identifier))
     return str((10 - sum(int(n) for n in identifier)) % 10)
 
 def validate(identifier):
-    """Check if CUSIP id valid. This checks the length and check digit."""
+    """Check if CUSIP is valid. This checks the length and check digit."""
     identifier = stripe(identifier)
     if not all(x in _characterSet for x in identifier):
         return 'Invalid Format'
     if len(identifier) != 9:
         return 'Incorrect Length'
     """if identifier[:2] not in _country_codes:
         raise InvalidComponent()"""
```

### Comparing `SecuMas-0.0.1.3/SecuMas/isin.py` & `SecuMas-0.0.1.4/SecuMas/isin.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,22 +12,20 @@
     # convert to numeric first, then double some, then sum individual digits
     identifier = ''.join(str(_characterSet.index(n)) for n in identifier)
     identifier = ''.join(
         str((2, 1)[i % 2] * int(n)) for i, n in enumerate(reversed(identifier)))
     return str((10 - sum(int(n) for n in identifier)) % 10)
 
 def validate(identifier):
-    """Check if ISIN id valid. This checks the length and check digit."""
+    """Check if ISIN is valid. This checks the length and check digit."""
     identifier = stripe(identifier)
     if not all(x in _characterSet for x in identifier):
         return 'Invalid Format'
     if len(identifier) != 12:
         return 'Incorrect Length'
-    """if identifier[:2] not in _country_codes:
-        raise InvalidComponent()"""
     if get_check_digit(identifier[:-1]) != identifier[-1]:
         return 'Incorrect Checkdigit'
     return identifier
 
 def dummy(number):
     """Generate dummy ISINs."""
     isins = []
```

### Comparing `SecuMas-0.0.1.3/SecuMas.egg-info/PKG-INFO` & `SecuMas-0.0.1.4/SecuMas.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,62 @@
 Metadata-Version: 2.1
 Name: SecuMas
-Version: 0.0.1.3
+Version: 0.0.1.4
 Summary: An application build for Securities Master platform
 Home-page: https://secumas.dev
 Author: A Deolekar
 Author-email: sher.buk@gmail.com
 License: MIT License
 Project-URL: Documentation, https://secumas.dev/
 Project-URL: Source, https://github.com/deolekar/SecuMas
+Description: # Introduction
+        
+        This Repo is for Securities Master Python custom package built.
+        
+        ```batch
+        pip install SecuMas
+        ```
+        
+        Examples:
+        
+        ```python
+        import SecuMas
+        
+        ''' Validate (ISIN)'''
+        print (SecuMas.isin.validate('IN8081309367'))
+        
+        ''' Generate Dummy ISINs (development usecase)'''
+        print (SecuMas.isin.dummy(5))
+        
+        ```
+        
+        # Package documentation
+        
+        > [Documentation](https://www.secumas.dev/)
+        
+        # Code contributions
+        
+        > [Check ToDo](https://github.com/deolekar/MMjs/blob/main/ToDo.txt)
+        
+        Improvements to SecuMas are most welcome. Integrating contributions will be done on a best-effort basis and can be made easier if the following are considered:
+        
+        Contributions are made as GitHub pull requests.
+        
+        Submitted contributions will often be reformatted and sometimes restructured for consistency with other parts.
+        
+        Contributions will be acknowledged in the release notes.
+        
+        Contributions should add or update a copyright statement if you feel the contribution is significant.
+        
+        All contribution should be made with compatible applicable copyright.
+        
+        It is not needed to modify the README.md, it will be updated on release.
+        
+        All code should be well tested and achieve 100% code coverage.
+        
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
@@ -20,51 +65,7 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 2 - Pre-Alpha
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Introduction
-
-This Repo is for Securities Master Python custom package built.
-
-```batch
-pip install SecuMas
-```
-
-Examples:
-
-```python
-import SecuMas
-
-''' Validate (ISIN)'''
-print (SecuMas.isin.validate('IN8081309367'))
-
-''' Generate Dummy ISINs (development usecase)'''
-print (SecuMas.isin.dummy(5))
-
-```
-
-# Package documentation
-
-> [Documentation](https://www.secumas.dev/)
-
-# Code contributions
-
-Improvements to SecuMas are most welcome. Integrating contributions will be done on a best-effort basis and can be made easier if the following are considered:
-
-Contributions are made as GitHub pull requests.
-
-Submitted contributions will often be reformatted and sometimes restructured for consistency with other parts.
-
-Contributions will be acknowledged in the release notes.
-
-Contributions should add or update a copyright statement if you feel the contribution is significant.
-
-All contribution should be made with compatible applicable copyright.
-
-It is not needed to modify the README.md, it will be updated on release.
-
-All code should be well tested and achieve 100% code coverage.
```

### Comparing `SecuMas-0.0.1.3/setup.py` & `SecuMas-0.0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name="SecuMas",
-    version="0.0.1.3",
+    version="0.0.1.4",
     author="A Deolekar",
     author_email="sher.buk@gmail.com",
     url="https://secumas.dev",
     description="An application build for Securities Master platform",
     readme = "README.md",
     packages=find_packages(),
     classifiers=[
```

