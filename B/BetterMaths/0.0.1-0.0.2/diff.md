# Comparing `tmp/bettermaths-0.0.1.tar.gz` & `tmp/bettermaths-0.0.2.tar.gz`

## Comparing `bettermaths-0.0.1.tar` & `bettermaths-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,20 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bettermaths-0.0.1/src/BetterMaths/__init__.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 bettermaths-0.0.1/src/BetterMaths/geometry.py
--rw-r--r--   0        0        0    14719 2020-02-02 00:00:00.000000 bettermaths-0.0.1/src/BetterMaths/main.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 bettermaths-0.0.1/src/BetterMaths/probability.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 bettermaths-0.0.1/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 bettermaths-0.0.1/LICENSE
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 bettermaths-0.0.1/README.md
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 bettermaths-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 bettermaths-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 bettermaths-0.0.2/generate.py
+-rw-r--r--   0        0        0    37790 2020-02-02 00:00:00.000000 bettermaths-0.0.2/images/banner.png
+-rw-r--r--   0        0        0    21551 2020-02-02 00:00:00.000000 bettermaths-0.0.2/images/logo transparent.png
+-rw-r--r--   0        0        0    26707 2020-02-02 00:00:00.000000 bettermaths-0.0.2/images/logo.png
+-rw-r--r--   0        0        0    23333 2020-02-02 00:00:00.000000 bettermaths-0.0.2/images/wiki/equation-page.png
+-rw-r--r--   0        0        0    22228 2020-02-02 00:00:00.000000 bettermaths-0.0.2/images/wiki/geometry-page.png
+-rw-r--r--   0        0        0    19633 2020-02-02 00:00:00.000000 bettermaths-0.0.2/images/wiki/home-page.png
+-rw-r--r--   0        0        0    23092 2020-02-02 00:00:00.000000 bettermaths-0.0.2/images/wiki/probabilities-page.png
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 bettermaths-0.0.2/src/BetterMaths/__init__.py
+-rw-r--r--   0        0        0    21932 2020-02-02 00:00:00.000000 bettermaths-0.0.2/src/BetterMaths/main.py
+-rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 bettermaths-0.0.2/src/BetterMaths/main.pyi
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bettermaths-0.0.2/src/BetterMaths/geometry/__init__.py
+-rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 bettermaths-0.0.2/src/BetterMaths/geometry/main.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bettermaths-0.0.2/src/BetterMaths/probability/__init__.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 bettermaths-0.0.2/src/BetterMaths/probability/main.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bettermaths-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 bettermaths-0.0.2/LICENSE
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 bettermaths-0.0.2/README.md
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 bettermaths-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 bettermaths-0.0.2/PKG-INFO
```

### Comparing `bettermaths-0.0.1/LICENSE` & `bettermaths-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bettermaths-0.0.1/README.md` & `bettermaths-0.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ![alt text](images/banner.png "Title")
 
 
-[![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/)
+[![MIT License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
 > [!WARNING]
 > This module is in beta phase
 
-#### See the [Wiki](https://github.com/Dhaiven/BetterMath/wiki) for documentations
+#### See the [Wiki](https://github.com/Dhaiven/BetterMaths/wiki) for documentations
 
 ## Contribution
-BetterMath accepts community contributions!
+BetterMaths accepts community contributions!
 
 ## Authors
-  - <img src="https://www.github.com/Dhaiven.png" width="3%" height="3%" border-radius=100% />  [@Dhaiven](https://www.github.com/Dhaiven) for code
-  - <img src="https://www.github.com/algorythmTTV.png" width="3%" height="3%" border-radius=100% />  [@algorythmTTV](https://www.github.com/algorythmTTV) for images and site
+  - <img src="https://www.github.com/Dhaiven.png" width="3%" height="3%"/> [@Dhaiven](https://www.github.com/Dhaiven) for code
+  - <img src="https://www.github.com/algorythmTTV.png" width="3%" height="3%"/> [@algorythmTTV](https://www.github.com/algorythmTTV) for images and site
```

### Comparing `bettermaths-0.0.1/pyproject.toml` & `bettermaths-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "BetterMaths"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Dhaiven", email="bettermath.get.help@gmail.com" },
   { name="algorythmTTV", email="bettermath.get.help@gmail.com" },
 ]
 description = "Python mathematics made easier"
 readme = "README.md"
 requires-python = ">=3.4"
@@ -25,9 +25,9 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 keywords = ["math", "mathematics", "better", "easier", "simple", "easy"]
 
 [project.urls]
 Homepage = "https://dhaiven.github.io/"
-Documentation = "https://dhaiven.github.io/BetterMath/wiki"
-Repository = "https://github.com/Dhaiven/BetterMath"
+Documentation = "https://dhaiven.github.io/BetterMaths/wiki"
+Repository = "https://github.com/Dhaiven/BetterMaths"
```

### Comparing `bettermaths-0.0.1/PKG-INFO` & `bettermaths-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.3
 Name: BetterMaths
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python mathematics made easier
 Project-URL: Homepage, https://dhaiven.github.io/
-Project-URL: Documentation, https://dhaiven.github.io/BetterMath/wiki
-Project-URL: Repository, https://github.com/Dhaiven/BetterMath
+Project-URL: Documentation, https://dhaiven.github.io/BetterMaths/wiki
+Project-URL: Repository, https://github.com/Dhaiven/BetterMaths
 Author-email: Dhaiven <bettermath.get.help@gmail.com>, algorythmTTV <bettermath.get.help@gmail.com>
 License-File: LICENSE
 Keywords: better,easier,easy,math,mathematics,simple
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
@@ -21,19 +21,19 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 
 ![alt text](images/banner.png "Title")
 
 
-[![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/)
+[![MIT License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
 > [!WARNING]
 > This module is in beta phase
 
-#### See the [Wiki](https://github.com/Dhaiven/BetterMath/wiki) for documentations
+#### See the [Wiki](https://github.com/Dhaiven/BetterMaths/wiki) for documentations
 
 ## Contribution
-BetterMath accepts community contributions!
+BetterMaths accepts community contributions!
 
 ## Authors
-  - <img src="https://www.github.com/Dhaiven.png" width="3%" height="3%" border-radius=100% />  [@Dhaiven](https://www.github.com/Dhaiven) for code
-  - <img src="https://www.github.com/algorythmTTV.png" width="3%" height="3%" border-radius=100% />  [@algorythmTTV](https://www.github.com/algorythmTTV) for images and site
+  - <img src="https://www.github.com/Dhaiven.png" width="3%" height="3%"/> [@Dhaiven](https://www.github.com/Dhaiven) for code
+  - <img src="https://www.github.com/algorythmTTV.png" width="3%" height="3%"/> [@algorythmTTV](https://www.github.com/algorythmTTV) for images and site
```

