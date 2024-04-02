# Comparing `tmp/pygm-1.0.tar.gz` & `tmp/pygm-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygm-1.0.tar", last modified: Thu Mar 28 18:46:58 2024, max compression
+gzip compressed data, was "pygm-1.0.1.tar", last modified: Tue Apr  2 16:07:40 2024, max compression
```

## Comparing `pygm-1.0.tar` & `pygm-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 giorgio    (501) staff       (20)        0 2024-03-28 18:46:58.316919 pygm-1.0/
--rw-r--r--   0 giorgio    (501) staff       (20)    11357 2020-07-14 07:41:04.000000 pygm-1.0/LICENSE
--rw-r--r--   0 giorgio    (501) staff       (20)      100 2024-03-28 11:26:02.000000 pygm-1.0/MANIFEST.in
-drwxr-xr-x   0 giorgio    (501) staff       (20)        0 2024-03-28 18:46:58.311662 pygm-1.0/PGM-index/
-drwxr-xr-x   0 giorgio    (501) staff       (20)        0 2024-03-28 18:46:58.311716 pygm-1.0/PGM-index/include/
-drwxr-xr-x   0 giorgio    (501) staff       (20)        0 2024-03-28 18:46:58.313041 pygm-1.0/PGM-index/include/pgm/
--rw-r--r--   0 giorgio    (501) staff       (20)    11650 2024-03-27 14:33:41.000000 pygm-1.0/PGM-index/include/pgm/pgm_index.hpp
--rw-r--r--   0 giorgio    (501) staff       (20)    11633 2024-03-27 14:33:41.000000 pygm-1.0/PGM-index/include/pgm/piecewise_linear_model.hpp
--rw-r--r--   0 giorgio    (501) staff       (20)     6886 2024-03-28 18:46:58.316224 pygm-1.0/PKG-INFO
--rw-r--r--   0 giorgio    (501) staff       (20)     5090 2024-03-27 18:47:41.000000 pygm-1.0/README.md
-drwxr-xr-x   0 giorgio    (501) staff       (20)        0 2024-03-28 18:46:58.314391 pygm-1.0/pygm/
--rw-r--r--   0 giorgio    (501) staff       (20)      226 2024-03-28 18:38:22.000000 pygm-1.0/pygm/__init__.py
--rw-r--r--   0 giorgio    (501) staff       (20)    20013 2024-03-28 12:29:41.000000 pygm-1.0/pygm/pygm.cpp
--rw-r--r--   0 giorgio    (501) staff       (20)    10399 2024-03-28 08:42:43.000000 pygm-1.0/pygm/sortedcontainer.py
--rw-r--r--   0 giorgio    (501) staff       (20)     6885 2024-03-28 08:54:06.000000 pygm-1.0/pygm/sortedlist.py
--rw-r--r--   0 giorgio    (501) staff       (20)     9927 2024-03-28 08:54:23.000000 pygm-1.0/pygm/sortedset.py
-drwxr-xr-x   0 giorgio    (501) staff       (20)        0 2024-03-28 18:46:58.315984 pygm-1.0/pygm.egg-info/
--rw-r--r--   0 giorgio    (501) staff       (20)     6886 2024-03-28 18:46:58.000000 pygm-1.0/pygm.egg-info/PKG-INFO
--rw-r--r--   0 giorgio    (501) staff       (20)      405 2024-03-28 18:46:58.000000 pygm-1.0/pygm.egg-info/SOURCES.txt
--rw-r--r--   0 giorgio    (501) staff       (20)        1 2024-03-28 18:46:58.000000 pygm-1.0/pygm.egg-info/dependency_links.txt
--rw-r--r--   0 giorgio    (501) staff       (20)        1 2020-07-10 18:32:05.000000 pygm-1.0/pygm.egg-info/not-zip-safe
--rw-r--r--   0 giorgio    (501) staff       (20)        5 2024-03-28 18:46:58.000000 pygm-1.0/pygm.egg-info/top_level.txt
--rw-r--r--   0 giorgio    (501) staff       (20)       38 2024-03-28 18:46:58.316970 pygm-1.0/setup.cfg
--rw-r--r--   0 giorgio    (501) staff       (20)     5017 2024-03-28 18:46:49.000000 pygm-1.0/setup.py
-drwxr-xr-x   0 giorgio    (501) staff       (20)        0 2024-03-28 18:46:58.315662 pygm-1.0/tests/
--rw-r--r--   0 giorgio    (501) staff       (20)     6028 2024-03-28 06:59:51.000000 pygm-1.0/tests/test_sorted_list.py
--rw-r--r--   0 giorgio    (501) staff       (20)     5816 2020-07-12 19:42:40.000000 pygm-1.0/tests/test_sorted_set.py
+drwxr-xr-x   0 giorgio    (501) staff       (20)        0 2024-04-02 16:07:40.877800 pygm-1.0.1/
+-rw-r--r--   0 giorgio    (501) staff       (20)    11357 2020-07-14 07:41:04.000000 pygm-1.0.1/LICENSE
+-rw-r--r--   0 giorgio    (501) staff       (20)      100 2024-03-28 11:26:02.000000 pygm-1.0.1/MANIFEST.in
+drwxr-xr-x   0 giorgio    (501) staff       (20)        0 2024-04-02 16:07:40.871023 pygm-1.0.1/PGM-index/
+drwxr-xr-x   0 giorgio    (501) staff       (20)        0 2024-04-02 16:07:40.871080 pygm-1.0.1/PGM-index/include/
+drwxr-xr-x   0 giorgio    (501) staff       (20)        0 2024-04-02 16:07:40.872761 pygm-1.0.1/PGM-index/include/pgm/
+-rw-r--r--   0 giorgio    (501) staff       (20)    11650 2024-03-27 14:33:41.000000 pygm-1.0.1/PGM-index/include/pgm/pgm_index.hpp
+-rw-r--r--   0 giorgio    (501) staff       (20)    11633 2024-03-27 14:33:41.000000 pygm-1.0.1/PGM-index/include/pgm/piecewise_linear_model.hpp
+-rw-r--r--   0 giorgio    (501) staff       (20)     7053 2024-04-02 16:07:40.877100 pygm-1.0.1/PKG-INFO
+-rw-r--r--   0 giorgio    (501) staff       (20)     5090 2024-03-27 18:47:41.000000 pygm-1.0.1/README.md
+drwxr-xr-x   0 giorgio    (501) staff       (20)        0 2024-04-02 16:07:40.874537 pygm-1.0.1/pygm/
+-rw-r--r--   0 giorgio    (501) staff       (20)      228 2024-04-02 14:20:42.000000 pygm-1.0.1/pygm/__init__.py
+-rw-r--r--   0 giorgio    (501) staff       (20)    19804 2024-04-02 14:14:50.000000 pygm-1.0.1/pygm/pygm.cpp
+-rw-r--r--   0 giorgio    (501) staff       (20)    10399 2024-03-28 08:42:43.000000 pygm-1.0.1/pygm/sortedcontainer.py
+-rw-r--r--   0 giorgio    (501) staff       (20)     6885 2024-03-28 08:54:06.000000 pygm-1.0.1/pygm/sortedlist.py
+-rw-r--r--   0 giorgio    (501) staff       (20)     9927 2024-03-28 08:54:23.000000 pygm-1.0.1/pygm/sortedset.py
+drwxr-xr-x   0 giorgio    (501) staff       (20)        0 2024-04-02 16:07:40.876817 pygm-1.0.1/pygm.egg-info/
+-rw-r--r--   0 giorgio    (501) staff       (20)     7053 2024-04-02 16:07:40.000000 pygm-1.0.1/pygm.egg-info/PKG-INFO
+-rw-r--r--   0 giorgio    (501) staff       (20)      405 2024-04-02 16:07:40.000000 pygm-1.0.1/pygm.egg-info/SOURCES.txt
+-rw-r--r--   0 giorgio    (501) staff       (20)        1 2024-04-02 16:07:40.000000 pygm-1.0.1/pygm.egg-info/dependency_links.txt
+-rw-r--r--   0 giorgio    (501) staff       (20)        1 2020-07-10 18:32:05.000000 pygm-1.0.1/pygm.egg-info/not-zip-safe
+-rw-r--r--   0 giorgio    (501) staff       (20)        5 2024-04-02 16:07:40.000000 pygm-1.0.1/pygm.egg-info/top_level.txt
+-rw-r--r--   0 giorgio    (501) staff       (20)       38 2024-04-02 16:07:40.877864 pygm-1.0.1/setup.cfg
+-rw-r--r--   0 giorgio    (501) staff       (20)     5181 2024-04-02 14:19:13.000000 pygm-1.0.1/setup.py
+drwxr-xr-x   0 giorgio    (501) staff       (20)        0 2024-04-02 16:07:40.876349 pygm-1.0.1/tests/
+-rw-r--r--   0 giorgio    (501) staff       (20)     6028 2024-03-28 06:59:51.000000 pygm-1.0.1/tests/test_sorted_list.py
+-rw-r--r--   0 giorgio    (501) staff       (20)     5816 2020-07-12 19:42:40.000000 pygm-1.0.1/tests/test_sorted_set.py
```

### Comparing `pygm-1.0/LICENSE` & `pygm-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygm-1.0/PGM-index/include/pgm/pgm_index.hpp` & `pygm-1.0.1/PGM-index/include/pgm/pgm_index.hpp`

 * *Files identical despite different names*

### Comparing `pygm-1.0/PGM-index/include/pgm/piecewise_linear_model.hpp` & `pygm-1.0.1/PGM-index/include/pgm/piecewise_linear_model.hpp`

 * *Files identical despite different names*

### Comparing `pygm-1.0/PKG-INFO` & `pygm-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: pygm
-Version: 1.0
+Version: 1.0.1
 Summary: Sorted containers with state-of-the-art query performance and compressed memory usage
 Home-page: https://pgm.di.unipi.it/
 Author: Giorgio Vinciguerra
 Author-email: i@gvdev.com
 License: Apache-2.0
 Project-URL: Documentation, https://pgm.di.unipi.it/docs/python-reference/
 Project-URL: Source, https://github.com/gvinciguerra/PyGM/
 Project-URL: Tracker, https://github.com/gvinciguerra/PyGM/issues
 Keywords: tree list array btree b+tree vector skiplist container sortedlist sorted set query index data structure
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development
 Classifier: Topic :: System
```

#### html2text {}

```diff
@@ -1,31 +1,33 @@
-Metadata-Version: 2.1 Name: pygm Version: 1.0 Summary: Sorted containers with
+Metadata-Version: 2.1 Name: pygm Version: 1.0.1 Summary: Sorted containers with
 state-of-the-art query performance and compressed memory usage Home-page:
 https://pgm.di.unipi.it/ Author: Giorgio Vinciguerra Author-email: i@gvdev.com
 License: Apache-2.0 Project-URL: Documentation, https://pgm.di.unipi.it/docs/
 python-reference/ Project-URL: Source, https://github.com/gvinciguerra/PyGM/
 Project-URL: Tracker, https://github.com/gvinciguerra/PyGM/issues Keywords:
 tree list array btree b+tree vector skiplist container sortedlist sorted set
 query index data structure Classifier: License :: OSI Approved :: Apache
-Software License Classifier: Development Status :: 3 - Alpha Classifier:
-Intended Audience :: Developers Classifier: Intended Audience :: Information
-Technology Classifier: Intended Audience :: Science/Research Classifier:
-Natural Language :: English Classifier: Programming Language :: C++ Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.3 Classifier: Programming Language :: Python :: 3.4 Classifier:
-Programming Language :: Python :: 3.5 Classifier: Programming Language ::
-Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Topic :: Database Classifier: Topic :: Scientific/
-Engineering Classifier: Topic :: Scientific/Engineering :: Artificial
-Intelligence Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Topic :: Scientific/Engineering :: Information Analysis Classifier:
-Topic :: Software Development Classifier: Topic :: System Classifier: Topic ::
-System :: Archiving :: Compression Classifier: Topic :: Utilities Description-
-Content-Type: text/markdown License-File: LICENSE
+Software License Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
+Information Technology Classifier: Intended Audience :: Science/Research
+Classifier: Natural Language :: English Classifier: Programming Language :: C++
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.3 Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5 Classifier: Programming
+Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Classifier: Topic :: Database Classifier: Topic ::
+Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
+Artificial Intelligence Classifier: Topic :: Scientific/Engineering :: Bio-
+Informatics Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Software Development Classifier: Topic :: System
+Classifier: Topic :: System :: Archiving :: Compression Classifier: Topic ::
+Utilities Description-Content-Type: text/markdown License-File: LICENSE
                                     [pygm]
 PyGM is a Python library that enables fast query operations on sorted lists of
 numbers (like integers and floats) with a tiny memory overhead. Internally, it
 features the _P_G_M_-_i_n_d_e_x, a state-of-the-art learned data structure that robustly
         scales to billions of elements in just a few tens of megabytes.
    _[_B_u_i_l_d_ _s_t_a_t_u_s_]_[_C_o_d_e_ _c_o_v_e_r_a_g_e_]_[_P_y_P_I_]_[_L_i_c_e_n_s_e_]_[_G_i_t_H_u_b_ _s_t_a_r_s_]_[_G_i_t_H_u_b_ _f_o_r_k_s_]
 ## Quick start Install with pip: ```bash pip install pygm ``` PyGM supports
```

### Comparing `pygm-1.0/README.md` & `pygm-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pygm-1.0/pygm/pygm.cpp` & `pygm-1.0.1/pygm/pygm.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -268,33 +268,27 @@
             throw std::invalid_argument("level can't be < 0");
         if (level_num >= this->height())
             throw std::invalid_argument("level can't be >= index height");
 
         return this->levels_offsets[level_num + 1] - this->levels_offsets[level_num] - 1;
     }
 
-    std::unordered_map<std::string, double> segment(size_t level_num, size_t segment_num) {
+    py::dict segment(size_t level_num, size_t segment_num) {
         if (level_num >= this->height())
             throw std::invalid_argument("level can't be >= index height");
         if (segment_num >= num_segments(level_num))
             throw std::invalid_argument("segment can't be >= number of segments in level");
 
-        std::unordered_map<std::string, double> segment;
-        segment["epsilon"] = level_num == 0 ? get_epsilon() : get_epsilon_recursive();
-
-        auto segment_it = this->segments.begin() + this->levels_offsets[level_num];
-        for (int sn = segment_num; sn > 0; --sn) {
-            ++segment_it;
-        }
-
-        segment["key"] = segment_it->key;
-        segment["slope"] = segment_it->slope;
-        segment["intercept"] = segment_it->intercept;
-
-        return segment;
+        auto &s = this->segments[this->levels_offsets[level_num] + segment_num];
+        py::dict out;
+        out["key"] = s.key;
+        out["slope"] = s.slope;
+        out["intercept"] = s.intercept;
+        out["epsilon"] = level_num == 0 ? get_epsilon() : get_epsilon_recursive();
+        return out;
     }
 
     K operator[](size_t i) const { return data[i]; }
 
     size_t size() const { return data.size(); }
 
     size_t get_epsilon() const { return epsilon; }
```

### Comparing `pygm-1.0/pygm/sortedcontainer.py` & `pygm-1.0.1/pygm/sortedcontainer.py`

 * *Files identical despite different names*

### Comparing `pygm-1.0/pygm/sortedlist.py` & `pygm-1.0.1/pygm/sortedlist.py`

 * *Files identical despite different names*

### Comparing `pygm-1.0/pygm/sortedset.py` & `pygm-1.0.1/pygm/sortedset.py`

 * *Files identical despite different names*

### Comparing `pygm-1.0/pygm.egg-info/PKG-INFO` & `pygm-1.0.1/pygm.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: pygm
-Version: 1.0
+Version: 1.0.1
 Summary: Sorted containers with state-of-the-art query performance and compressed memory usage
 Home-page: https://pgm.di.unipi.it/
 Author: Giorgio Vinciguerra
 Author-email: i@gvdev.com
 License: Apache-2.0
 Project-URL: Documentation, https://pgm.di.unipi.it/docs/python-reference/
 Project-URL: Source, https://github.com/gvinciguerra/PyGM/
 Project-URL: Tracker, https://github.com/gvinciguerra/PyGM/issues
 Keywords: tree list array btree b+tree vector skiplist container sortedlist sorted set query index data structure
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development
 Classifier: Topic :: System
```

#### html2text {}

```diff
@@ -1,31 +1,33 @@
-Metadata-Version: 2.1 Name: pygm Version: 1.0 Summary: Sorted containers with
+Metadata-Version: 2.1 Name: pygm Version: 1.0.1 Summary: Sorted containers with
 state-of-the-art query performance and compressed memory usage Home-page:
 https://pgm.di.unipi.it/ Author: Giorgio Vinciguerra Author-email: i@gvdev.com
 License: Apache-2.0 Project-URL: Documentation, https://pgm.di.unipi.it/docs/
 python-reference/ Project-URL: Source, https://github.com/gvinciguerra/PyGM/
 Project-URL: Tracker, https://github.com/gvinciguerra/PyGM/issues Keywords:
 tree list array btree b+tree vector skiplist container sortedlist sorted set
 query index data structure Classifier: License :: OSI Approved :: Apache
-Software License Classifier: Development Status :: 3 - Alpha Classifier:
-Intended Audience :: Developers Classifier: Intended Audience :: Information
-Technology Classifier: Intended Audience :: Science/Research Classifier:
-Natural Language :: English Classifier: Programming Language :: C++ Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.3 Classifier: Programming Language :: Python :: 3.4 Classifier:
-Programming Language :: Python :: 3.5 Classifier: Programming Language ::
-Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Topic :: Database Classifier: Topic :: Scientific/
-Engineering Classifier: Topic :: Scientific/Engineering :: Artificial
-Intelligence Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Topic :: Scientific/Engineering :: Information Analysis Classifier:
-Topic :: Software Development Classifier: Topic :: System Classifier: Topic ::
-System :: Archiving :: Compression Classifier: Topic :: Utilities Description-
-Content-Type: text/markdown License-File: LICENSE
+Software License Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
+Information Technology Classifier: Intended Audience :: Science/Research
+Classifier: Natural Language :: English Classifier: Programming Language :: C++
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.3 Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5 Classifier: Programming
+Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Classifier: Topic :: Database Classifier: Topic ::
+Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
+Artificial Intelligence Classifier: Topic :: Scientific/Engineering :: Bio-
+Informatics Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Software Development Classifier: Topic :: System
+Classifier: Topic :: System :: Archiving :: Compression Classifier: Topic ::
+Utilities Description-Content-Type: text/markdown License-File: LICENSE
                                     [pygm]
 PyGM is a Python library that enables fast query operations on sorted lists of
 numbers (like integers and floats) with a tiny memory overhead. Internally, it
 features the _P_G_M_-_i_n_d_e_x, a state-of-the-art learned data structure that robustly
         scales to billions of elements in just a few tens of megabytes.
    _[_B_u_i_l_d_ _s_t_a_t_u_s_]_[_C_o_d_e_ _c_o_v_e_r_a_g_e_]_[_P_y_P_I_]_[_L_i_c_e_n_s_e_]_[_G_i_t_H_u_b_ _s_t_a_r_s_]_[_G_i_t_H_u_b_ _f_o_r_k_s_]
 ## Quick start Install with pip: ```bash pip install pygm ``` PyGM supports
```

### Comparing `pygm-1.0/setup.py` & `pygm-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import subprocess
 import sys
 import tempfile
 
 import setuptools
 from setuptools.command.build_ext import build_ext
 
-__version__ = '1.0'
+__version__ = '1.0.1'
 
 
 class get_pybind_include(object):
     """Helper class to determine the pybind11 include path."""
 
     def __str__(self):
         import pybind11
@@ -113,28 +113,31 @@
     ext_modules=ext_modules,
     packages=setuptools.find_packages(),
     setup_requires=['pybind11>=2.5.0'],
     cmdclass={'build_ext': BuildExt},
     zip_safe=False,
     classifiers=[
         'License :: OSI Approved :: Apache Software License',
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Information Technology',
         'Intended Audience :: Science/Research',
         'Natural Language :: English',
         'Programming Language :: C++',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Topic :: Database',
         'Topic :: Scientific/Engineering',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Scientific/Engineering :: Bio-Informatics',
         'Topic :: Scientific/Engineering :: Information Analysis',
         'Topic :: Software Development',
         'Topic :: System',
```

### Comparing `pygm-1.0/tests/test_sorted_list.py` & `pygm-1.0.1/tests/test_sorted_list.py`

 * *Files identical despite different names*

### Comparing `pygm-1.0/tests/test_sorted_set.py` & `pygm-1.0.1/tests/test_sorted_set.py`

 * *Files identical despite different names*

