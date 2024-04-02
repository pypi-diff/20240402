# Comparing `tmp/pyaogmaneo-2.3.9.tar.gz` & `tmp/pyaogmaneo-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaogmaneo-2.3.9.tar", last modified: Sat Jan 20 18:53:41 2024, max compression
+gzip compressed data, was "pyaogmaneo-2.4.0.tar", last modified: Tue Apr  2 17:13:30 2024, max compression
```

## Comparing `pyaogmaneo-2.3.9.tar` & `pyaogmaneo-2.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2024-01-20 18:53:41.468998 pyaogmaneo-2.3.9/
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2024-01-20 18:53:41.468998 pyaogmaneo-2.3.9/CMake/
--rw-r--r--   0 ericl     (1000) ericl     (1001)     1250 2024-01-20 17:52:41.000000 pyaogmaneo-2.3.9/CMake/FindAOgmaNeo.cmake
--rw-r--r--   0 ericl     (1000) ericl     (1001)     2620 2024-01-20 18:51:16.000000 pyaogmaneo-2.3.9/CMakeLists.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)    17842 2022-12-03 02:07:03.000000 pyaogmaneo-2.3.9/LICENSE.md
--rw-r--r--   0 ericl     (1000) ericl     (1001)       64 2022-12-03 02:07:03.000000 pyaogmaneo-2.3.9/MANIFEST.in
--rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2024-01-20 18:53:41.468998 pyaogmaneo-2.3.9/PKG-INFO
--rw-r--r--   0 ericl     (1000) ericl     (1001)     2415 2024-01-20 17:52:41.000000 pyaogmaneo-2.3.9/README.md
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2024-01-20 18:53:41.468998 pyaogmaneo-2.3.9/pyaogmaneo.egg-info/
--rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2024-01-20 18:53:41.000000 pyaogmaneo-2.3.9/pyaogmaneo.egg-info/PKG-INFO
--rw-r--r--   0 ericl     (1000) ericl     (1001)      505 2024-01-20 18:53:41.000000 pyaogmaneo-2.3.9/pyaogmaneo.egg-info/SOURCES.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2024-01-20 18:53:41.000000 pyaogmaneo-2.3.9/pyaogmaneo.egg-info/dependency_links.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2023-06-29 17:53:40.000000 pyaogmaneo-2.3.9/pyaogmaneo.egg-info/not-zip-safe
--rw-r--r--   0 ericl     (1000) ericl     (1001)       11 2024-01-20 18:53:41.000000 pyaogmaneo-2.3.9/pyaogmaneo.egg-info/top_level.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)      101 2023-01-13 01:36:37.000000 pyaogmaneo-2.3.9/pyproject.toml
--rw-r--r--   0 ericl     (1000) ericl     (1001)       38 2024-01-20 18:53:41.468998 pyaogmaneo-2.3.9/setup.cfg
--rw-r--r--   0 ericl     (1000) ericl     (1001)     4204 2024-01-20 18:52:22.000000 pyaogmaneo-2.3.9/setup.py
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2024-01-20 18:53:41.468998 pyaogmaneo-2.3.9/source/
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2024-01-20 18:53:41.468998 pyaogmaneo-2.3.9/source/pyaogmaneo/
--rw-r--r--   0 ericl     (1000) ericl     (1001)     1153 2024-01-20 17:52:41.000000 pyaogmaneo-2.3.9/source/pyaogmaneo/py_helpers.cpp
--rw-r--r--   0 ericl     (1000) ericl     (1001)     1953 2024-01-20 17:52:41.000000 pyaogmaneo-2.3.9/source/pyaogmaneo/py_helpers.h
--rw-r--r--   0 ericl     (1000) ericl     (1001)    12600 2024-01-20 17:52:41.000000 pyaogmaneo-2.3.9/source/pyaogmaneo/py_hierarchy.cpp
--rw-r--r--   0 ericl     (1000) ericl     (1001)     7095 2024-01-20 17:52:41.000000 pyaogmaneo-2.3.9/source/pyaogmaneo/py_hierarchy.h
--rw-r--r--   0 ericl     (1000) ericl     (1001)     7846 2024-01-20 17:52:41.000000 pyaogmaneo-2.3.9/source/pyaogmaneo/py_image_encoder.cpp
--rw-r--r--   0 ericl     (1000) ericl     (1001)     3209 2024-01-20 17:52:41.000000 pyaogmaneo-2.3.9/source/pyaogmaneo/py_image_encoder.h
--rw-r--r--   0 ericl     (1000) ericl     (1001)    11526 2024-01-20 18:13:26.000000 pyaogmaneo-2.3.9/source/pyaogmaneo/py_module.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:13:30.332402 pyaogmaneo-2.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:13:30.328402 pyaogmaneo-2.4.0/CMake/
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-02 17:13:20.000000 pyaogmaneo-2.4.0/CMake/FindAOgmaNeo.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-02 17:13:20.000000 pyaogmaneo-2.4.0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17842 2024-04-02 17:13:20.000000 pyaogmaneo-2.4.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-02 17:13:20.000000 pyaogmaneo-2.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-02 17:13:30.332402 pyaogmaneo-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-02 17:13:20.000000 pyaogmaneo-2.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:13:30.332402 pyaogmaneo-2.4.0/pyaogmaneo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-02 17:13:30.000000 pyaogmaneo-2.4.0/pyaogmaneo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-02 17:13:30.000000 pyaogmaneo-2.4.0/pyaogmaneo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 17:13:30.000000 pyaogmaneo-2.4.0/pyaogmaneo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 17:13:30.000000 pyaogmaneo-2.4.0/pyaogmaneo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 17:13:30.000000 pyaogmaneo-2.4.0/pyaogmaneo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-02 17:13:20.000000 pyaogmaneo-2.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 17:13:30.332402 pyaogmaneo-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-02 17:13:20.000000 pyaogmaneo-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:13:30.328402 pyaogmaneo-2.4.0/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:13:30.328402 pyaogmaneo-2.4.0/source/pyaogmaneo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-02 17:13:20.000000 pyaogmaneo-2.4.0/source/pyaogmaneo/py_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-02 17:13:20.000000 pyaogmaneo-2.4.0/source/pyaogmaneo/py_helpers.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12446 2024-04-02 17:13:20.000000 pyaogmaneo-2.4.0/source/pyaogmaneo/py_hierarchy.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-04-02 17:13:20.000000 pyaogmaneo-2.4.0/source/pyaogmaneo/py_hierarchy.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-04-02 17:13:20.000000 pyaogmaneo-2.4.0/source/pyaogmaneo/py_image_encoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-02 17:13:20.000000 pyaogmaneo-2.4.0/source/pyaogmaneo/py_image_encoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11200 2024-04-02 17:13:20.000000 pyaogmaneo-2.4.0/source/pyaogmaneo/py_module.cpp
```

### Comparing `pyaogmaneo-2.3.9/CMake/FindAOgmaNeo.cmake` & `pyaogmaneo-2.4.0/CMake/FindAOgmaNeo.cmake`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.3.9/CMakeLists.txt` & `pyaogmaneo-2.4.0/CMakeLists.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #  PyAOgmaNeo
 #  Copyright(c) 2020-2024 Ogma Intelligent Systems Corp. All rights reserved.
 #
 #  This copy of PyAOgmaNeo is licensed to you under the terms described
 #  in the PYAOGMANEO_LICENSE.md file included in this distribution.
 # ----------------------------------------------------------------------------
 
-cmake_minimum_required(VERSION 3.13)
+cmake_minimum_required(VERSION 3.24)
 
 project(pyaogmaneo)
 
 include(FetchContent)
 
 list(APPEND CMAKE_MODULE_PATH "${CMAKE_CURRENT_SOURCE_DIR}/CMake/")
 
@@ -32,37 +32,27 @@
     find_package(AOgmaNeo)
 else()
     message(STATUS "Not using system installation of AOgmaNeo, will download from repository")
 
     FetchContent_Declare(
         AOgmaNeo
         GIT_REPOSITORY https://github.com/ogmacorp/AOgmaNeo.git
-        GIT_TAG 38bae0ea80670dae6c89a0b4f495a58b763421ba
+        GIT_TAG ac704b11ade55184b8b59c6831b7a0a121940767
     )
 
-    FetchContent_GetProperties(AOgmaNeo)
-
-    if(NOT AOgmaNeo_POPULATED)
-        FetchContent_Populate(AOgmaNeo)
-        add_subdirectory(${aogmaneo_SOURCE_DIR} ${aogmaneo_BINARY_DIR})
-    endif()
+    FetchContent_MakeAvailable(AOgmaNeo)
 endif()
 
 FetchContent_Declare(
     pybind11
     GIT_REPOSITORY https://github.com/pybind/pybind11
     GIT_TAG origin/master 
 )
 
-FetchContent_GetProperties(pybind11)
-
-if(NOT pybind11_POPULATED)
-    FetchContent_Populate(pybind11)
-    add_subdirectory(${pybind11_SOURCE_DIR} ${pybind11_BINARY_DIR})
-endif()
+FetchContent_MakeAvailable(pybind11)
 
 include_directories(${AOgmaNeo_SOURCE_DIR}/source)
 
 find_package(OpenMP REQUIRED)
 
 set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} ${OpenMP_CXX_FLAGS}")
 
@@ -76,17 +66,14 @@
 set(PYAOGMANEO_SRC
     "source/pyaogmaneo/py_module.cpp"
     "source/pyaogmaneo/py_helpers.cpp"
     "source/pyaogmaneo/py_hierarchy.cpp"
     "source/pyaogmaneo/py_image_encoder.cpp"
 )
 
-find_package(Python COMPONENTS Interpreter Development)
-find_package(pybind11 CONFIG)
-
 pybind11_add_module(pyaogmaneo ${PYAOGMANEO_SRC})
 
 if(USE_SYSTEM_AOGMANEO)
     message(STATUS ${AOGMANEO_LIBRARIES})
     target_link_libraries(pyaogmaneo PUBLIC ${AOGMANEO_LIBRARIES} ${OpenMP_CXX_FLAGS})
 else()
     target_link_libraries(pyaogmaneo PUBLIC AOgmaNeo ${OpenMP_CXX_FLAGS})
```

### Comparing `pyaogmaneo-2.3.9/LICENSE.md` & `pyaogmaneo-2.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.3.9/PKG-INFO` & `pyaogmaneo-2.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaogmaneo
-Version: 2.3.9
+Version: 2.4.0
 Summary: Python bindings for the AOgmaNeo library
 Home-page: https://ogmacorp.com/
 Author: Ogma Intelligent Systems Corp
 Author-email: info@ogmacorp.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pyaogmaneo-2.3.9/README.md` & `pyaogmaneo-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.3.9/pyaogmaneo.egg-info/PKG-INFO` & `pyaogmaneo-2.4.0/pyaogmaneo.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaogmaneo
-Version: 2.3.9
+Version: 2.4.0
 Summary: Python bindings for the AOgmaNeo library
 Home-page: https://ogmacorp.com/
 Author: Ogma Intelligent Systems Corp
 Author-email: info@ogmacorp.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pyaogmaneo-2.3.9/setup.py` & `pyaogmaneo-2.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,16 @@
     def build_extension(self, ext):
         extdir = os.path.abspath(os.path.dirname(self.get_ext_fullpath(ext.name)))
 
         if not extdir.endswith(os.path.sep):
             extdir += os.path.sep
 
         cmake_args = [ '-DCMAKE_LIBRARY_OUTPUT_DIRECTORY=' + extdir,
-                       '-DUSE_SYSTEM_AOGMANEO=' + ('On' if use_system_aogmaneo else 'Off') ]
+                      '-DPYBIND11_FINDPYTHON=ON',
+                      '-DUSE_SYSTEM_AOGMANEO=' + ('On' if use_system_aogmaneo else 'Off') ]
 
         cfg = 'Debug' if self.debug else 'Release'
         build_args = [ '--config', cfg ]
 
         if platform.system() == "Windows":
             cmake_args += [ '-DCMAKE_LIBRARY_OUTPUT_DIRECTORY_{}={}'.format(cfg.upper(), extdir) ]
 
@@ -83,15 +84,15 @@
             os.makedirs(self.build_temp)
 
         subprocess.check_call([ 'cmake', ext.sourcedir ] + cmake_args, cwd=self.build_temp, env=env)
         subprocess.check_call([ 'cmake', '--build', '.' ] + build_args, cwd=self.build_temp)
 
 setup(
     name="pyaogmaneo",
-    version="2.3.9",
+    version="2.4.0",
     description="Python bindings for the AOgmaNeo library",
     long_description='https://github.com/ogmacorp/PyAOgmaNeo',
     author='Ogma Intelligent Systems Corp',
     author_email='info@ogmacorp.com',
     url='https://ogmacorp.com/',
     license='Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License',
     classifiers=[
```

### Comparing `pyaogmaneo-2.3.9/source/pyaogmaneo/py_helpers.cpp` & `pyaogmaneo-2.4.0/source/pyaogmaneo/py_helpers.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.3.9/source/pyaogmaneo/py_helpers.h` & `pyaogmaneo-2.4.0/source/pyaogmaneo/py_helpers.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.3.9/source/pyaogmaneo/py_hierarchy.cpp` & `pyaogmaneo-2.4.0/source/pyaogmaneo/py_hierarchy.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -24,17 +24,14 @@
         throw std::runtime_error("error: num_dendrites_per_cell < 1 is not allowed!");
 
     if (up_radius < 0)
         throw std::runtime_error("error: up_radius < 0 is not allowed!");
 
     if (down_radius < 0)
         throw std::runtime_error("error: down_radius < 0 is not allowed!");
-
-    if (history_capacity < 2)
-        throw std::runtime_error("error: history_capacity < 2 is not allowed!");
 }
 
 void Layer_Desc::check_in_range() const {
     if (std::get<0>(hidden_size) < 1)
         throw std::runtime_error("error: hidden_size[0] < 1 is not allowed!");
 
     if (std::get<1>(hidden_size) < 1)
@@ -108,16 +105,15 @@
         io_descs[i].check_in_range();
 
         c_io_descs[i] = aon::Hierarchy::IO_Desc(
             aon::Int3(std::get<0>(io_descs[i].size), std::get<1>(io_descs[i].size), std::get<2>(io_descs[i].size)),
             static_cast<aon::IO_Type>(io_descs[i].type),
             io_descs[i].num_dendrites_per_cell,
             io_descs[i].up_radius,
-            io_descs[i].down_radius,
-            io_descs[i].history_capacity
+            io_descs[i].down_radius
         );
     }
     
     aon::Array<aon::Hierarchy::Layer_Desc> c_layer_descs(layer_descs.size());
 
     for (int l = 0; l < layer_descs.size(); l++) {
         layer_descs[l].check_in_range();
```

### Comparing `pyaogmaneo-2.3.9/source/pyaogmaneo/py_hierarchy.h` & `pyaogmaneo-2.4.0/source/pyaogmaneo/py_hierarchy.h`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 #include "py_helpers.h"
 #include <aogmaneo/hierarchy.h>
 
 namespace py = pybind11;
 
 namespace pyaon {
-const int hierarchy_magic = 6338803;
+const int hierarchy_magic = 9211838;
 
 enum IO_Type {
     none = 0,
     prediction = 1,
     action = 2
 };
 
@@ -27,31 +27,27 @@
     IO_Type type;
 
     int num_dendrites_per_cell;
 
     int up_radius;
     int down_radius;
 
-    int history_capacity;
-
     IO_Desc(
         const std::tuple<int, int, int> &size,
         IO_Type type,
         int num_dendrites_per_cell,
         int up_radius,
-        int down_radius,
-        int history_capacity
+        int down_radius
     )
     :
     size(size),
     type(type),
     num_dendrites_per_cell(num_dendrites_per_cell),
     up_radius(up_radius),
-    down_radius(down_radius),
-    history_capacity(history_capacity)
+    down_radius(down_radius)
     {}
 
     void check_in_range() const;
 };
 
 struct Layer_Desc {
     std::tuple<int, int, int> hidden_size;
@@ -271,22 +267,13 @@
 
         if (h.get_io_type(i) == aon::action)
             return h.get_actor(i).get_visible_layer_desc(0).radius;
         
         return h.get_decoder(l, i).get_visible_layer_desc(0).radius;
     }
 
-    int get_actor_history_capacity(
-        int i
-    ) const {
-        if (i < 0 || i >= h.get_num_io() || h.get_io_type(i) != aon::action)
-            throw std::runtime_error("error: " + std::to_string(i) + " is not a valid input index!");
-
-        return h.get_actor(i).get_history_capacity();
-    }
-
     void merge(
         const std::vector<Hierarchy*> &hierarchies,
         Merge_Mode mode
     );
 };
 }
```

### Comparing `pyaogmaneo-2.3.9/source/pyaogmaneo/py_image_encoder.cpp` & `pyaogmaneo-2.4.0/source/pyaogmaneo/py_image_encoder.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.3.9/source/pyaogmaneo/py_image_encoder.h` & `pyaogmaneo-2.4.0/source/pyaogmaneo/py_image_encoder.h`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 #include "py_helpers.h"
 #include <aogmaneo/image_encoder.h>
 
 namespace py = pybind11;
 
 namespace pyaon {
-const int image_encoder_magic = 5189334;
+const int image_encoder_magic = 7557115;
 
 struct Image_Visible_Layer_Desc {
     std::tuple<int, int, int> size;
 
     int radius;
 
     Image_Visible_Layer_Desc(
```

### Comparing `pyaogmaneo-2.3.9/source/pyaogmaneo/py_module.cpp` & `pyaogmaneo-2.4.0/source/pyaogmaneo/py_module.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -31,30 +31,27 @@
 
     py::class_<pyaon::IO_Desc>(m, "IODesc")
         .def(py::init<
                 std::tuple<int, int, int>,
                 pyaon::IO_Type,
                 int,
                 int,
-                int,
                 int
             >(),
             py::arg("size") = std::tuple<int, int, int>({ 4, 4, 16 }),
             py::arg("io_type") = pyaon::prediction,
             py::arg("num_dendrites_per_cell") = 4,
             py::arg("up_radius") = 2,
-            py::arg("down_radius") = 2,
-            py::arg("history_capacity") = 256
+            py::arg("down_radius") = 2
         )
         .def_readwrite("size", &pyaon::IO_Desc::size)
         .def_readwrite("io_type", &pyaon::IO_Desc::type)
         .def_readwrite("num_dendrites_per_cell", &pyaon::IO_Desc::num_dendrites_per_cell)
         .def_readwrite("up_radius", &pyaon::IO_Desc::up_radius)
         .def_readwrite("down_radius", &pyaon::IO_Desc::down_radius)
-        .def_readwrite("history_capacity", &pyaon::IO_Desc::history_capacity)
         .def("__copy__", 
             [](const pyaon::IO_Desc &other) {
                 return other;
             }
         )
         .def("__deepcopy__", 
             [](const pyaon::IO_Desc &other) {
@@ -95,32 +92,30 @@
             }
         );
 
     // bind params
     py::class_<aon::Encoder::Params>(m, "EncoderParams")
         .def(py::init<>())
         .def_readwrite("scale", &aon::Encoder::Params::scale)
-        .def_readwrite("lr", &aon::Encoder::Params::lr);
+        .def_readwrite("lr", &aon::Encoder::Params::lr)
+        .def_readwrite("early_stop_cells", &aon::Encoder::Params::early_stop_cells);
 
     py::class_<aon::Decoder::Params>(m, "DecoderParams")
         .def(py::init<>())
         .def_readwrite("scale", &aon::Decoder::Params::scale)
-        .def_readwrite("lr", &aon::Decoder::Params::lr)
-        .def_readwrite("leak", &aon::Decoder::Params::leak);
+        .def_readwrite("lr", &aon::Decoder::Params::lr);
 
     py::class_<aon::Actor::Params>(m, "ActorParams")
         .def(py::init<>())
         .def_readwrite("vlr", &aon::Actor::Params::vlr)
-        .def_readwrite("alr", &aon::Actor::Params::alr)
-        .def_readwrite("rate", &aon::Actor::Params::rate)
-        .def_readwrite("leak", &aon::Actor::Params::leak)
-        .def_readwrite("clip_coef", &aon::Actor::Params::clip_coef)
+        .def_readwrite("plr", &aon::Actor::Params::plr)
+        .def_readwrite("value_rate", &aon::Actor::Params::value_rate)
         .def_readwrite("discount", &aon::Actor::Params::discount)
-        .def_readwrite("min_steps", &aon::Actor::Params::min_steps)
-        .def_readwrite("history_iters", &aon::Actor::Params::history_iters);
+        .def_readwrite("trace_curve", &aon::Actor::Params::trace_curve)
+        .def_readwrite("trace_decay", &aon::Actor::Params::trace_decay);
 
     py::class_<aon::Hierarchy::Layer_Params>(m, "LayerParams")
         .def(py::init<>())
         .def_readwrite("encoder", &aon::Hierarchy::Layer_Params::encoder)
         .def_readwrite("decoder", &aon::Hierarchy::Layer_Params::decoder);
 
     py::class_<aon::Hierarchy::IO_Params>(m, "IOParams")
@@ -174,15 +169,14 @@
         .def("get_ticks", &pyaon::Hierarchy::get_ticks)
         .def("get_ticks_per_update", &pyaon::Hierarchy::get_ticks_per_update)
         .def("get_num_io", &pyaon::Hierarchy::get_num_io)
         .def("get_io_size", &pyaon::Hierarchy::get_io_size)
         .def("get_io_type", &pyaon::Hierarchy::get_io_type)
         .def("get_up_radius", &pyaon::Hierarchy::get_up_radius)
         .def("get_down_radius", &pyaon::Hierarchy::get_down_radius)
-        .def("get_actor_history_capacity", &pyaon::Hierarchy::get_actor_history_capacity)
         .def("merge", &pyaon::Hierarchy::merge)
         .def("__copy__", 
             [](const pyaon::Hierarchy &other) {
                 return other;
             }
         )
         .def("__deepcopy__",
```

