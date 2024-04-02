# Comparing `tmp/py-domain-driven-design-1.0.0a1.tar.gz` & `tmp/py-domain-driven-design-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/py-domain-driven-design-1.0.0a1.tar", last modified: Mon Mar  4 07:30:21 2024, max compression
+gzip compressed data, was "dist/py-domain-driven-design-1.0.0a2.tar", last modified: Tue Apr  2 05:02:18 2024, max compression
```

## Comparing `py-domain-driven-design-1.0.0a1.tar` & `py-domain-driven-design-1.0.0a2.tar`

### file list

```diff
@@ -1,12 +1,35 @@
-drwxr-xr-x   0 david      (501) staff       (20)        0 2024-03-04 07:30:21.000000 py-domain-driven-design-1.0.0a1/
--rw-r--r--   0 david      (501) staff       (20)    35149 2021-03-14 15:00:54.000000 py-domain-driven-design-1.0.0a1/LICENSE
--rw-r--r--   0 david      (501) staff       (20)     2600 2024-03-04 07:30:21.000000 py-domain-driven-design-1.0.0a1/PKG-INFO
--rw-r--r--   0 david      (501) staff       (20)     1505 2024-03-04 07:28:31.000000 py-domain-driven-design-1.0.0a1/README.md
--rw-r--r--   0 david      (501) staff       (20)       38 2024-03-04 07:30:21.000000 py-domain-driven-design-1.0.0a1/setup.cfg
--rw-r--r--   0 david      (501) staff       (20)     1587 2024-03-04 07:27:59.000000 py-domain-driven-design-1.0.0a1/setup.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2024-03-04 07:30:21.000000 py-domain-driven-design-1.0.0a1/src/
-drwxr-xr-x   0 david      (501) staff       (20)        0 2024-03-04 07:30:21.000000 py-domain-driven-design-1.0.0a1/src/py_domain_driven_design.egg-info/
--rw-r--r--   0 david      (501) staff       (20)     2600 2024-03-04 07:30:20.000000 py-domain-driven-design-1.0.0a1/src/py_domain_driven_design.egg-info/PKG-INFO
--rw-r--r--   0 david      (501) staff       (20)      230 2024-03-04 07:30:20.000000 py-domain-driven-design-1.0.0a1/src/py_domain_driven_design.egg-info/SOURCES.txt
--rw-r--r--   0 david      (501) staff       (20)        1 2024-03-04 07:30:20.000000 py-domain-driven-design-1.0.0a1/src/py_domain_driven_design.egg-info/dependency_links.txt
--rw-r--r--   0 david      (501) staff       (20)        1 2024-03-04 07:30:20.000000 py-domain-driven-design-1.0.0a1/src/py_domain_driven_design.egg-info/top_level.txt
+drwxr-xr-x   0 david      (501) staff       (20)        0 2024-04-02 05:02:18.000000 py-domain-driven-design-1.0.0a2/
+-rw-r--r--   0 david      (501) staff       (20)    35149 2021-03-14 15:00:54.000000 py-domain-driven-design-1.0.0a2/LICENSE
+-rw-r--r--   0 david      (501) staff       (20)     6263 2024-04-02 05:02:18.000000 py-domain-driven-design-1.0.0a2/PKG-INFO
+-rw-r--r--   0 david      (501) staff       (20)     5172 2024-04-02 04:52:43.000000 py-domain-driven-design-1.0.0a2/README.md
+-rw-r--r--   0 david      (501) staff       (20)       38 2024-04-02 05:02:18.000000 py-domain-driven-design-1.0.0a2/setup.cfg
+-rw-r--r--   0 david      (501) staff       (20)     1607 2024-04-02 05:01:08.000000 py-domain-driven-design-1.0.0a2/setup.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2024-04-02 05:02:18.000000 py-domain-driven-design-1.0.0a2/src/
+drwxr-xr-x   0 david      (501) staff       (20)        0 2024-04-02 05:02:18.000000 py-domain-driven-design-1.0.0a2/src/ddd/
+-rw-r--r--   0 david      (501) staff       (20)        0 2020-11-30 11:28:04.000000 py-domain-driven-design-1.0.0a2/src/ddd/__init__.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2024-04-02 05:02:18.000000 py-domain-driven-design-1.0.0a2/src/ddd/domain/
+-rw-r--r--   0 david      (501) staff       (20)        0 2020-11-30 11:28:04.000000 py-domain-driven-design-1.0.0a2/src/ddd/domain/__init__.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2024-04-02 05:02:18.000000 py-domain-driven-design-1.0.0a2/src/ddd/domain/model/
+-rw-r--r--   0 david      (501) staff       (20)        0 2020-11-30 11:28:04.000000 py-domain-driven-design-1.0.0a2/src/ddd/domain/model/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)       83 2024-03-31 06:46:53.000000 py-domain-driven-design-1.0.0a2/src/ddd/domain/model/aggregate_root.py
+-rw-r--r--   0 david      (501) staff       (20)       23 2024-03-31 05:38:14.000000 py-domain-driven-design-1.0.0a2/src/ddd/domain/model/entity.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2024-04-02 05:02:18.000000 py-domain-driven-design-1.0.0a2/src/ddd/domain/model/exceptions/
+-rw-r--r--   0 david      (501) staff       (20)        0 2020-11-30 11:28:04.000000 py-domain-driven-design-1.0.0a2/src/ddd/domain/model/exceptions/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)       51 2024-04-01 06:21:10.000000 py-domain-driven-design-1.0.0a2/src/ddd/domain/model/exceptions/entity_not_found_exception.py
+-rw-r--r--   0 david      (501) staff       (20)       28 2024-03-31 05:38:11.000000 py-domain-driven-design-1.0.0a2/src/ddd/domain/model/value_object.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2024-04-02 05:02:18.000000 py-domain-driven-design-1.0.0a2/src/ddd/infrastructure/
+-rw-r--r--   0 david      (501) staff       (20)        0 2020-11-30 11:28:04.000000 py-domain-driven-design-1.0.0a2/src/ddd/infrastructure/__init__.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2024-04-02 05:02:18.000000 py-domain-driven-design-1.0.0a2/src/ddd/infrastructure/repository/
+-rw-r--r--   0 david      (501) staff       (20)        0 2020-11-30 11:28:04.000000 py-domain-driven-design-1.0.0a2/src/ddd/infrastructure/repository/__init__.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2024-04-02 05:02:18.000000 py-domain-driven-design-1.0.0a2/src/ddd/infrastructure/repository/datastore/
+-rw-r--r--   0 david      (501) staff       (20)        0 2020-11-30 11:28:04.000000 py-domain-driven-design-1.0.0a2/src/ddd/infrastructure/repository/datastore/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)     1737 2024-04-01 07:25:46.000000 py-domain-driven-design-1.0.0a2/src/ddd/infrastructure/repository/datastore/datastore_repository_base.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2024-04-02 05:02:18.000000 py-domain-driven-design-1.0.0a2/src/ddd/infrastructure/repository/in_memory/
+-rw-r--r--   0 david      (501) staff       (20)        0 2020-11-30 11:28:04.000000 py-domain-driven-design-1.0.0a2/src/ddd/infrastructure/repository/in_memory/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)     1242 2024-04-01 07:25:46.000000 py-domain-driven-design-1.0.0a2/src/ddd/infrastructure/repository/in_memory/in_memory_repository_base.py
+-rw-r--r--   0 david      (501) staff       (20)      404 2024-03-31 07:31:52.000000 py-domain-driven-design-1.0.0a2/src/ddd/infrastructure/repository/irepository.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2024-04-02 05:02:18.000000 py-domain-driven-design-1.0.0a2/src/py_domain_driven_design.egg-info/
+-rw-r--r--   0 david      (501) staff       (20)     6263 2024-04-02 05:02:18.000000 py-domain-driven-design-1.0.0a2/src/py_domain_driven_design.egg-info/PKG-INFO
+-rw-r--r--   0 david      (501) staff       (20)      911 2024-04-02 05:02:18.000000 py-domain-driven-design-1.0.0a2/src/py_domain_driven_design.egg-info/SOURCES.txt
+-rw-r--r--   0 david      (501) staff       (20)        1 2024-04-02 05:02:18.000000 py-domain-driven-design-1.0.0a2/src/py_domain_driven_design.egg-info/dependency_links.txt
+-rw-r--r--   0 david      (501) staff       (20)        4 2024-04-02 05:02:18.000000 py-domain-driven-design-1.0.0a2/src/py_domain_driven_design.egg-info/top_level.txt
```

### Comparing `py-domain-driven-design-1.0.0a1/LICENSE` & `py-domain-driven-design-1.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `py-domain-driven-design-1.0.0a1/setup.py` & `py-domain-driven-design-1.0.0a2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 from setuptools import find_packages
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
-    name='py-domain-driven-design',
-    version='1.0.0-alpha.1',
-    author='David Runemalm, 2024',
-    author_email='david.runemalm@gmail.com',
-    description=
-    'A py-domain-driven-design_AND_TYPE for Python.',
+    name="py-domain-driven-design",
+    version="1.0.0-alpha.2",
+    author="David Runemalm, 2024",
+    author_email="david.runemalm@gmail.com",
+    description="A domain-driven design library for Python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url='https://github.com/runemalm/py-domain-driven-design',
+    url="https://github.com/runemalm/py-domain-driven-design",
     project_urls={
         "Documentation": "https://py-domain-driven-design.readthedocs.io/en/latest/",
         "Bug Tracker": "https://github.com/runemalm/py-domain-driven-design/issues",
     },
-    package_dir={'': 'src'},
-    packages = find_packages(
-        where = 'src',
-        include = ['ddd*', ],
-        exclude = ['tests*', ]
+    package_dir={"": "src"},
+    packages=find_packages(
+        where="src",
+        include=[
+            "ddd*",
+        ],
+        exclude=[
+            "tests*",
+        ],
     ),
-    license='GNU General Public License v3.0',
-    install_requires=[
-
-    ],
+    license="GNU General Public License v3.0",
+    install_requires=[],
     tests_require=[
-        'pytest',
+        "pytest",
     ],
-    python_requires='>=3.7',
+    python_requires=">=3.7",
     classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Programming Language :: Python :: 3.12',
-        'Topic :: Software Development :: Libraries :: Python Modules',
+        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
+        "Topic :: Software Development :: Libraries :: Python Modules",
     ],
 )
```

