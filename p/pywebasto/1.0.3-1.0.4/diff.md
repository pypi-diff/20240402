# Comparing `tmp/pywebasto-1.0.3.tar.gz` & `tmp/pywebasto-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywebasto-1.0.3.tar", max compression
+gzip compressed data, was "pywebasto-1.0.4.tar", max compression
```

## Comparing `pywebasto-1.0.3.tar` & `pywebasto-1.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2024-03-29 11:18:21.102101 pywebasto-1.0.3/LICENSE
--rw-r--r--   0        0        0       55 2024-03-29 11:18:21.102101 pywebasto-1.0.3/README.md
--rw-r--r--   0        0        0      582 2024-03-29 11:18:31.578253 pywebasto-1.0.3/pyproject.toml
--rw-r--r--   0        0        0    16426 2024-03-29 11:18:21.102101 pywebasto-1.0.3/pywebasto/__init__.py
--rw-r--r--   0        0        0      314 2024-03-29 11:18:21.102101 pywebasto-1.0.3/pywebasto/consts.py
--rw-r--r--   0        0        0      447 2024-03-29 11:18:21.102101 pywebasto-1.0.3/pywebasto/enums.py
--rw-r--r--   0        0        0      205 2024-03-29 11:18:21.102101 pywebasto-1.0.3/pywebasto/exceptions.py
--rw-r--r--   0        0        0      833 1970-01-01 00:00:00.000000 pywebasto-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-02 07:50:54.806967 pywebasto-1.0.4/LICENSE
+-rw-r--r--   0        0        0       55 2024-04-02 07:50:54.806967 pywebasto-1.0.4/README.md
+-rw-r--r--   0        0        0      582 2024-04-02 07:51:06.874885 pywebasto-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0    16559 2024-04-02 07:50:54.806967 pywebasto-1.0.4/pywebasto/__init__.py
+-rw-r--r--   0        0        0      314 2024-04-02 07:50:54.806967 pywebasto-1.0.4/pywebasto/consts.py
+-rw-r--r--   0        0        0      447 2024-04-02 07:50:54.806967 pywebasto-1.0.4/pywebasto/enums.py
+-rw-r--r--   0        0        0      205 2024-04-02 07:50:54.806967 pywebasto-1.0.4/pywebasto/exceptions.py
+-rw-r--r--   0        0        0      833 1970-01-01 00:00:00.000000 pywebasto-1.0.4/PKG-INFO
```

### Comparing `pywebasto-1.0.3/LICENSE` & `pywebasto-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pywebasto-1.0.3/pyproject.toml` & `pywebasto-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pywebasto"
-version = "v1.0.3"
+version = "v1.0.4"
 description = "API library for Webasto ThermoConnect devices"
 authors = ["Malene Trab <malene@trab.dk>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
```

### Comparing `pywebasto-1.0.3/pywebasto/__init__.py` & `pywebasto-1.0.4/pywebasto/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,15 +171,19 @@
                     self._heading = fwd_bearing
 
                 if distance > 0:
                     time_diff = (
                         self._cur_time - self._prev_time
                     ).total_seconds() / 3600
                     if time_diff > 0:
-                        self._speed = distance / time_diff
+                        self._speed = (distance / 1000) / time_diff
+                    else:
+                        self._speed = 0
+                else:
+                    self._speed = 0
 
         if self._last_data["temperature"][-1] == "C":
             self._iscelcius = True
 
         for output in self._last_data["outputs"]:
             if output["line"] == "OUTH" or output["line"] == "OUTV":
                 self._output_main = output
```

### Comparing `pywebasto-1.0.3/PKG-INFO` & `pywebasto-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywebasto
-Version: 1.0.3
+Version: 1.0.4
 Summary: API library for Webasto ThermoConnect devices
 License: MIT
 Author: Malene Trab
 Author-email: malene@trab.dk
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

