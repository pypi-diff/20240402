# Comparing `tmp/pyDSA_core-1.4.0.tar.gz` & `tmp/pyDSA_core-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyDSA_core-1.4.0.tar", last modified: Sat Sep 19 10:32:44 2020, max compression
+gzip compressed data, was "pyDSA_core-1.4.1.tar", last modified: Tue Apr  2 19:44:00 2024, max compression
```

## Comparing `pyDSA_core-1.4.0.tar` & `pyDSA_core-1.4.1.tar`

### file list

```diff
@@ -1,23 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-19 10:32:44.209221 pyDSA_core-1.4.0/
--rw-r--r--   0 root         (0) root         (0)     2449 2020-09-19 10:32:44.209221 pyDSA_core-1.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1325 2019-04-28 09:03:54.000000 pyDSA_core-1.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-19 10:32:44.199221 pyDSA_core-1.4.0/pyDSA_core/
--rw-r--r--   0 root         (0) root         (0)     3012 2019-11-04 00:10:36.000000 pyDSA_core-1.4.0/pyDSA_core/YL_fitting.py
--rw-r--r--   0 root         (0) root         (0)      749 2019-05-21 18:28:58.000000 pyDSA_core-1.4.0/pyDSA_core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5755 2020-08-09 09:47:11.000000 pyDSA_core-1.4.0/pyDSA_core/baseline.py
--rw-r--r--   0 root         (0) root         (0)    27621 2019-11-04 00:10:37.000000 pyDSA_core-1.4.0/pyDSA_core/dropedges.py
--rw-r--r--   0 root         (0) root         (0)    40504 2019-11-04 00:10:37.000000 pyDSA_core-1.4.0/pyDSA_core/dropfit.py
--rw-r--r--   0 root         (0) root         (0)    17801 2019-11-04 00:26:33.000000 pyDSA_core-1.4.0/pyDSA_core/helpers.py
--rw-r--r--   0 root         (0) root         (0)    38192 2020-08-09 09:47:12.000000 pyDSA_core-1.4.0/pyDSA_core/image.py
--rw-r--r--   0 root         (0) root         (0)    13738 2019-05-21 18:33:47.000000 pyDSA_core-1.4.0/pyDSA_core/temporaldropedges.py
--rw-r--r--   0 root         (0) root         (0)    22843 2019-05-21 18:33:47.000000 pyDSA_core-1.4.0/pyDSA_core/temporalfits.py
--rw-r--r--   0 root         (0) root         (0)    14673 2019-05-21 18:33:47.000000 pyDSA_core-1.4.0/pyDSA_core/temporalimages.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-19 10:32:44.209221 pyDSA_core-1.4.0/pyDSA_core.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2449 2020-09-19 10:32:44.000000 pyDSA_core-1.4.0/pyDSA_core.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      467 2020-09-19 10:32:44.000000 pyDSA_core-1.4.0/pyDSA_core.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-09-19 10:32:44.000000 pyDSA_core-1.4.0/pyDSA_core.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2019-11-04 00:02:52.000000 pyDSA_core-1.4.0/pyDSA_core.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       86 2020-09-19 10:32:44.000000 pyDSA_core-1.4.0/pyDSA_core.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2020-09-19 10:32:44.000000 pyDSA_core-1.4.0/pyDSA_core.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2020-09-19 10:32:44.209221 pyDSA_core-1.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1749 2020-09-19 10:31:48.000000 pyDSA_core-1.4.0/setup.py
+drwxr-xr-x   0 glaunay   (1000) glaunay   (1000)        0 2024-04-02 19:44:00.437492 pyDSA_core-1.4.1/
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)    35147 2019-03-26 23:55:49.000000 pyDSA_core-1.4.1/LICENSE
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)     2198 2024-04-02 19:44:00.437492 pyDSA_core-1.4.1/PKG-INFO
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)     1325 2019-04-28 09:03:54.000000 pyDSA_core-1.4.1/README.md
+drwxr-xr-x   0 glaunay   (1000) glaunay   (1000)        0 2024-04-02 19:44:00.434159 pyDSA_core-1.4.1/pyDSA_core/
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)     3012 2019-11-04 00:10:36.000000 pyDSA_core-1.4.1/pyDSA_core/YL_fitting.py
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)      749 2019-05-21 18:28:58.000000 pyDSA_core-1.4.1/pyDSA_core/__init__.py
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)     5755 2020-08-09 09:47:11.000000 pyDSA_core-1.4.1/pyDSA_core/baseline.py
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)    27621 2022-06-03 18:24:43.000000 pyDSA_core-1.4.1/pyDSA_core/dropedges.py
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)    40504 2019-11-04 00:10:37.000000 pyDSA_core-1.4.1/pyDSA_core/dropfit.py
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)    17801 2021-03-22 00:47:07.000000 pyDSA_core-1.4.1/pyDSA_core/helpers.py
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)    38192 2020-08-09 09:47:12.000000 pyDSA_core-1.4.1/pyDSA_core/image.py
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)    13738 2019-05-21 18:33:47.000000 pyDSA_core-1.4.1/pyDSA_core/temporaldropedges.py
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)    22843 2019-05-21 18:33:47.000000 pyDSA_core-1.4.1/pyDSA_core/temporalfits.py
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)    14673 2019-05-21 18:33:47.000000 pyDSA_core-1.4.1/pyDSA_core/temporalimages.py
+drwxr-xr-x   0 glaunay   (1000) glaunay   (1000)        0 2024-04-02 19:44:00.437492 pyDSA_core-1.4.1/pyDSA_core.egg-info/
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)     2198 2024-04-02 19:44:00.000000 pyDSA_core-1.4.1/pyDSA_core.egg-info/PKG-INFO
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)      615 2024-04-02 19:44:00.000000 pyDSA_core-1.4.1/pyDSA_core.egg-info/SOURCES.txt
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)        1 2024-04-02 19:44:00.000000 pyDSA_core-1.4.1/pyDSA_core.egg-info/dependency_links.txt
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)        1 2019-11-04 00:02:52.000000 pyDSA_core-1.4.1/pyDSA_core.egg-info/not-zip-safe
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)       86 2024-04-02 19:44:00.000000 pyDSA_core-1.4.1/pyDSA_core.egg-info/requires.txt
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)       11 2024-04-02 19:44:00.000000 pyDSA_core-1.4.1/pyDSA_core.egg-info/top_level.txt
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)       38 2024-04-02 19:44:00.437492 pyDSA_core-1.4.1/setup.cfg
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)     1749 2024-04-02 19:43:28.000000 pyDSA_core-1.4.1/setup.py
+drwxr-xr-x   0 glaunay   (1000) glaunay   (1000)        0 2024-04-02 19:44:00.437492 pyDSA_core-1.4.1/tests/
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)     3614 2019-05-21 18:32:52.000000 pyDSA_core-1.4.1/tests/test_baseline.py
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)     3984 2019-05-21 18:32:52.000000 pyDSA_core-1.4.1/tests/test_dropedges.py
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)     2714 2019-05-21 18:32:52.000000 pyDSA_core-1.4.1/tests/test_dropfit.py
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)     7537 2019-05-21 18:32:52.000000 pyDSA_core-1.4.1/tests/test_helpers.py
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)     5204 2019-05-21 18:32:52.000000 pyDSA_core-1.4.1/tests/test_image.py
+-rw-r--r--   0 glaunay   (1000) glaunay   (1000)     2446 2019-05-21 18:32:52.000000 pyDSA_core-1.4.1/tests/test_temporalimages.py
```

### Comparing `pyDSA_core-1.4.0/PKG-INFO` & `pyDSA_core-1.4.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,77 @@
 Metadata-Version: 2.1
 Name: pyDSA_core
-Version: 1.4.0
+Version: 1.4.1
 Summary: Python Drop Shape Analyzer
 Home-page: https://framagit.org/gabylaunay/pyDSA_core
 Author: Gaby Launay
 Author-email: gaby.launay@protonmail.com
-License: UNKNOWN
-Description: <div align="center">
-          <img width=500px" src="https://framagit.org/gabylaunay/pyDSA_core/raw/master/branding/pyDSA_logo_python_text.svg"><br><br>
-        </div>
-        
-        # PyDSA_core: python3 package for drop shape analysis.
-        
-        ## Features
-        
-        PyDSA_core allow to import videos and images of droplets and to get their properties, including
-        
-          - Drop edges positions
-          - Contact angles
-          - Contact angle hysteresis
-          - Radius
-          - Volume
-          - Triple point positions (for SLIPS surfaces)
-          - ...
-        
-        A Graphical interface is also available [here](https://framagit.org/gabylaunay/pyDSA_gui).
-        
-        A tutorial is available [here](https://gabylaunay.github.io/Python-cookbook/).
-        
-        ## Dependencies
-        
-        pyDSA_core relies on matplotlib, numpy, scipy, IMTreatment and OpenCV.
-        
-        ## Installation
-        
-        ``pip install pydsa_core``
-        
-        To update pyDSA_core, use:
-        
-        ``pip install -U pydsa_core``
-        
-        ## Citing this software
-        
-        If PyDSA_core have been usefull for you, please consider citing it:
-        ```
-        Launay G. PyDSA: Drop shape analysis in Python, 2018-, https://framagit.org/gabylaunay/pyDSA_core [Online; accessed <today>].
-        ```
-        
-        bibtex entry:
-        ``` bibtex
-        @Misc{launay_pydsa_2018,
-          author =    {Gaby Launay},
-          title =     {{PyDSA}: Drop shape analysis in {Python}},
-          year =      {2018--},
-          url = "https://framagit.org/gabylaunay/pyDSA_core",
-          note = {[Online; accessed <today>]}
-        }
-        
-        ```
-        
 Keywords: DSA drop shape contact angle hysteresis
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: opencv-python-headless
+Requires-Dist: scipy
+Requires-Dist: imageio
+Requires-Dist: scikit-image
+Requires-Dist: IMTreatment>=1.3.5
+
+<div align="center">
+  <img width=500px" src="https://framagit.org/gabylaunay/pyDSA_core/raw/master/branding/pyDSA_logo_python_text.svg"><br><br>
+</div>
+
+# PyDSA_core: python3 package for drop shape analysis.
+
+## Features
+
+PyDSA_core allow to import videos and images of droplets and to get their properties, including
+
+  - Drop edges positions
+  - Contact angles
+  - Contact angle hysteresis
+  - Radius
+  - Volume
+  - Triple point positions (for SLIPS surfaces)
+  - ...
+
+A Graphical interface is also available [here](https://framagit.org/gabylaunay/pyDSA_gui).
+
+A tutorial is available [here](https://gabylaunay.github.io/Python-cookbook/).
+
+## Dependencies
+
+pyDSA_core relies on matplotlib, numpy, scipy, IMTreatment and OpenCV.
+
+## Installation
+
+``pip install pydsa_core``
+
+To update pyDSA_core, use:
+
+``pip install -U pydsa_core``
+
+## Citing this software
+
+If PyDSA_core have been usefull for you, please consider citing it:
+```
+Launay G. PyDSA: Drop shape analysis in Python, 2018-, https://framagit.org/gabylaunay/pyDSA_core [Online; accessed <today>].
+```
+
+bibtex entry:
+``` bibtex
+@Misc{launay_pydsa_2018,
+  author =    {Gaby Launay},
+  title =     {{PyDSA}: Drop shape analysis in {Python}},
+  year =      {2018--},
+  url = "https://framagit.org/gabylaunay/pyDSA_core",
+  note = {[Online; accessed <today>]}
+}
+
+```
```

### Comparing `pyDSA_core-1.4.0/README.md` & `pyDSA_core-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pyDSA_core-1.4.0/pyDSA_core/YL_fitting.py` & `pyDSA_core-1.4.1/pyDSA_core/YL_fitting.py`

 * *Files identical despite different names*

### Comparing `pyDSA_core-1.4.0/pyDSA_core/__init__.py` & `pyDSA_core-1.4.1/pyDSA_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyDSA_core-1.4.0/pyDSA_core/baseline.py` & `pyDSA_core-1.4.1/pyDSA_core/baseline.py`

 * *Files identical despite different names*

### Comparing `pyDSA_core-1.4.0/pyDSA_core/dropedges.py` & `pyDSA_core-1.4.1/pyDSA_core/dropedges.py`

 * *Files identical despite different names*

### Comparing `pyDSA_core-1.4.0/pyDSA_core/dropfit.py` & `pyDSA_core-1.4.1/pyDSA_core/dropfit.py`

 * *Files identical despite different names*

### Comparing `pyDSA_core-1.4.0/pyDSA_core/helpers.py` & `pyDSA_core-1.4.1/pyDSA_core/helpers.py`

 * *Files identical despite different names*

### Comparing `pyDSA_core-1.4.0/pyDSA_core/image.py` & `pyDSA_core-1.4.1/pyDSA_core/image.py`

 * *Files identical despite different names*

### Comparing `pyDSA_core-1.4.0/pyDSA_core/temporaldropedges.py` & `pyDSA_core-1.4.1/pyDSA_core/temporaldropedges.py`

 * *Files identical despite different names*

### Comparing `pyDSA_core-1.4.0/pyDSA_core/temporalfits.py` & `pyDSA_core-1.4.1/pyDSA_core/temporalfits.py`

 * *Files identical despite different names*

### Comparing `pyDSA_core-1.4.0/pyDSA_core/temporalimages.py` & `pyDSA_core-1.4.1/pyDSA_core/temporalimages.py`

 * *Files identical despite different names*

### Comparing `pyDSA_core-1.4.0/pyDSA_core.egg-info/PKG-INFO` & `pyDSA_core-1.4.1/pyDSA_core.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,71 +1,77 @@
 Metadata-Version: 2.1
-Name: pyDSA-core
-Version: 1.4.0
+Name: pyDSA_core
+Version: 1.4.1
 Summary: Python Drop Shape Analyzer
 Home-page: https://framagit.org/gabylaunay/pyDSA_core
 Author: Gaby Launay
 Author-email: gaby.launay@protonmail.com
-License: UNKNOWN
-Description: <div align="center">
-          <img width=500px" src="https://framagit.org/gabylaunay/pyDSA_core/raw/master/branding/pyDSA_logo_python_text.svg"><br><br>
-        </div>
-        
-        # PyDSA_core: python3 package for drop shape analysis.
-        
-        ## Features
-        
-        PyDSA_core allow to import videos and images of droplets and to get their properties, including
-        
-          - Drop edges positions
-          - Contact angles
-          - Contact angle hysteresis
-          - Radius
-          - Volume
-          - Triple point positions (for SLIPS surfaces)
-          - ...
-        
-        A Graphical interface is also available [here](https://framagit.org/gabylaunay/pyDSA_gui).
-        
-        A tutorial is available [here](https://gabylaunay.github.io/Python-cookbook/).
-        
-        ## Dependencies
-        
-        pyDSA_core relies on matplotlib, numpy, scipy, IMTreatment and OpenCV.
-        
-        ## Installation
-        
-        ``pip install pydsa_core``
-        
-        To update pyDSA_core, use:
-        
-        ``pip install -U pydsa_core``
-        
-        ## Citing this software
-        
-        If PyDSA_core have been usefull for you, please consider citing it:
-        ```
-        Launay G. PyDSA: Drop shape analysis in Python, 2018-, https://framagit.org/gabylaunay/pyDSA_core [Online; accessed <today>].
-        ```
-        
-        bibtex entry:
-        ``` bibtex
-        @Misc{launay_pydsa_2018,
-          author =    {Gaby Launay},
-          title =     {{PyDSA}: Drop shape analysis in {Python}},
-          year =      {2018--},
-          url = "https://framagit.org/gabylaunay/pyDSA_core",
-          note = {[Online; accessed <today>]}
-        }
-        
-        ```
-        
 Keywords: DSA drop shape contact angle hysteresis
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: opencv-python-headless
+Requires-Dist: scipy
+Requires-Dist: imageio
+Requires-Dist: scikit-image
+Requires-Dist: IMTreatment>=1.3.5
+
+<div align="center">
+  <img width=500px" src="https://framagit.org/gabylaunay/pyDSA_core/raw/master/branding/pyDSA_logo_python_text.svg"><br><br>
+</div>
+
+# PyDSA_core: python3 package for drop shape analysis.
+
+## Features
+
+PyDSA_core allow to import videos and images of droplets and to get their properties, including
+
+  - Drop edges positions
+  - Contact angles
+  - Contact angle hysteresis
+  - Radius
+  - Volume
+  - Triple point positions (for SLIPS surfaces)
+  - ...
+
+A Graphical interface is also available [here](https://framagit.org/gabylaunay/pyDSA_gui).
+
+A tutorial is available [here](https://gabylaunay.github.io/Python-cookbook/).
+
+## Dependencies
+
+pyDSA_core relies on matplotlib, numpy, scipy, IMTreatment and OpenCV.
+
+## Installation
+
+``pip install pydsa_core``
+
+To update pyDSA_core, use:
+
+``pip install -U pydsa_core``
+
+## Citing this software
+
+If PyDSA_core have been usefull for you, please consider citing it:
+```
+Launay G. PyDSA: Drop shape analysis in Python, 2018-, https://framagit.org/gabylaunay/pyDSA_core [Online; accessed <today>].
+```
+
+bibtex entry:
+``` bibtex
+@Misc{launay_pydsa_2018,
+  author =    {Gaby Launay},
+  title =     {{PyDSA}: Drop shape analysis in {Python}},
+  year =      {2018--},
+  url = "https://framagit.org/gabylaunay/pyDSA_core",
+  note = {[Online; accessed <today>]}
+}
+
+```
```

### Comparing `pyDSA_core-1.4.0/setup.py` & `pyDSA_core-1.4.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), "r") as fh:
     long_description = fh.read()
 
 setup(
     name='pyDSA_core',
-    version='1.4.0',
+    version='1.4.1',
     description='Python Drop Shape Analyzer',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://framagit.org/gabylaunay/pyDSA_core',
     author='Gaby Launay',
     author_email='gaby.launay@protonmail.com',
     classifiers=[
@@ -39,13 +39,13 @@
         'Natural Language :: English',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Operating System :: POSIX :: Linux',
     ],
     keywords='DSA drop shape contact angle hysteresis',
     packages=find_packages(exclude=['contrib', 'docs', 'tests', 'samples']),
     install_requires=['numpy', 'matplotlib', 'opencv-python-headless', 'scipy',
-                      'imageio', 'scikit-image', 'IMTreatment==1.2.0'],
+                      'imageio', 'scikit-image', 'IMTreatment>=1.3.5'],
     extras_require={},
     setup_requires=['pytest-runner'],
     tests_require=['pytest'],
     zip_safe=False,
 )
```

