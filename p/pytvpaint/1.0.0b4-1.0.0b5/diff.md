# Comparing `tmp/pytvpaint-1.0.0b4.tar.gz` & `tmp/pytvpaint-1.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytvpaint-1.0.0b4.tar", max compression
+gzip compressed data, was "pytvpaint-1.0.0b5.tar", max compression
```

## Comparing `pytvpaint-1.0.0b4.tar` & `pytvpaint-1.0.0b5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1070 2024-03-28 15:34:10.487100 pytvpaint-1.0.0b4/LICENSE.md
--rw-r--r--   0        0        0     3515 2024-03-28 15:34:10.487100 pytvpaint-1.0.0b4/README.md
--rw-r--r--   0        0        0     2229 2024-03-28 15:34:10.495100 pytvpaint-1.0.0b4/pyproject.toml
--rw-r--r--   0        0        0     1233 2024-03-28 15:34:10.495100 pytvpaint-1.0.0b4/pytvpaint/__init__.py
--rw-r--r--   0        0        0     8570 2024-03-28 15:34:10.495100 pytvpaint-1.0.0b4/pytvpaint/camera.py
--rw-r--r--   0        0        0    32489 2024-03-28 15:34:10.495100 pytvpaint-1.0.0b4/pytvpaint/clip.py
--rw-r--r--   0        0        0      573 2024-03-28 15:34:10.495100 pytvpaint-1.0.0b4/pytvpaint/george/__init__.py
--rw-r--r--   0        0        0     4888 2024-03-28 15:34:10.495100 pytvpaint-1.0.0b4/pytvpaint/george/client/__init__.py
--rw-r--r--   0        0        0     9747 2024-03-28 15:34:10.495100 pytvpaint-1.0.0b4/pytvpaint/george/client/parse.py
--rw-r--r--   0        0        0     5389 2024-03-28 15:34:10.495100 pytvpaint-1.0.0b4/pytvpaint/george/client/rpc.py
--rw-r--r--   0        0        0      687 2024-03-28 15:34:10.495100 pytvpaint-1.0.0b4/pytvpaint/george/exceptions.py
--rw-r--r--   0        0        0    28188 2024-03-28 15:34:10.495100 pytvpaint-1.0.0b4/pytvpaint/george/grg_base.py
--rw-r--r--   0        0        0     2719 2024-03-28 15:34:10.495100 pytvpaint-1.0.0b4/pytvpaint/george/grg_camera.py
--rw-r--r--   0        0        0    19243 2024-03-28 15:34:10.495100 pytvpaint-1.0.0b4/pytvpaint/george/grg_clip.py
--rw-r--r--   0        0        0    31138 2024-03-28 15:34:10.495100 pytvpaint-1.0.0b4/pytvpaint/george/grg_layer.py
--rw-r--r--   0        0        0    14738 2024-03-28 15:34:10.495100 pytvpaint-1.0.0b4/pytvpaint/george/grg_project.py
--rw-r--r--   0        0        0     1189 2024-03-28 15:34:10.495100 pytvpaint-1.0.0b4/pytvpaint/george/grg_scene.py
--rw-r--r--   0        0        0    36492 2024-03-28 15:34:10.495100 pytvpaint-1.0.0b4/pytvpaint/layer.py
--rw-r--r--   0        0        0    22578 2024-03-28 15:34:10.495100 pytvpaint-1.0.0b4/pytvpaint/project.py
--rw-r--r--   0        0        0        0 2024-03-28 15:34:10.495100 pytvpaint-1.0.0b4/pytvpaint/py.typed
--rw-r--r--   0        0        0     4278 2024-03-28 15:34:10.495100 pytvpaint-1.0.0b4/pytvpaint/scene.py
--rw-r--r--   0        0        0     8662 2024-03-28 15:34:10.495100 pytvpaint-1.0.0b4/pytvpaint/sound.py
--rw-r--r--   0        0        0    17075 2024-03-28 15:34:10.495100 pytvpaint-1.0.0b4/pytvpaint/utils.py
--rw-r--r--   0        0        0     4420 1970-01-01 00:00:00.000000 pytvpaint-1.0.0b4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-02 14:46:10.861198 pytvpaint-1.0.0b5/LICENSE.md
+-rw-r--r--   0        0        0     3515 2024-04-02 14:46:10.861198 pytvpaint-1.0.0b5/README.md
+-rw-r--r--   0        0        0     2229 2024-04-02 14:46:10.869198 pytvpaint-1.0.0b5/pyproject.toml
+-rw-r--r--   0        0        0     1233 2024-04-02 14:46:10.869198 pytvpaint-1.0.0b5/pytvpaint/__init__.py
+-rw-r--r--   0        0        0     8570 2024-04-02 14:46:10.869198 pytvpaint-1.0.0b5/pytvpaint/camera.py
+-rw-r--r--   0        0        0    32489 2024-04-02 14:46:10.869198 pytvpaint-1.0.0b5/pytvpaint/clip.py
+-rw-r--r--   0        0        0      573 2024-04-02 14:46:10.869198 pytvpaint-1.0.0b5/pytvpaint/george/__init__.py
+-rw-r--r--   0        0        0     4890 2024-04-02 14:46:10.869198 pytvpaint-1.0.0b5/pytvpaint/george/client/__init__.py
+-rw-r--r--   0        0        0     9747 2024-04-02 14:46:10.869198 pytvpaint-1.0.0b5/pytvpaint/george/client/parse.py
+-rw-r--r--   0        0        0     5389 2024-04-02 14:46:10.869198 pytvpaint-1.0.0b5/pytvpaint/george/client/rpc.py
+-rw-r--r--   0        0        0      687 2024-04-02 14:46:10.869198 pytvpaint-1.0.0b5/pytvpaint/george/exceptions.py
+-rw-r--r--   0        0        0    28188 2024-04-02 14:46:10.869198 pytvpaint-1.0.0b5/pytvpaint/george/grg_base.py
+-rw-r--r--   0        0        0     2719 2024-04-02 14:46:10.869198 pytvpaint-1.0.0b5/pytvpaint/george/grg_camera.py
+-rw-r--r--   0        0        0    19243 2024-04-02 14:46:10.869198 pytvpaint-1.0.0b5/pytvpaint/george/grg_clip.py
+-rw-r--r--   0        0        0    31138 2024-04-02 14:46:10.869198 pytvpaint-1.0.0b5/pytvpaint/george/grg_layer.py
+-rw-r--r--   0        0        0    14902 2024-04-02 14:46:10.869198 pytvpaint-1.0.0b5/pytvpaint/george/grg_project.py
+-rw-r--r--   0        0        0     1189 2024-04-02 14:46:10.869198 pytvpaint-1.0.0b5/pytvpaint/george/grg_scene.py
+-rw-r--r--   0        0        0    36492 2024-04-02 14:46:10.869198 pytvpaint-1.0.0b5/pytvpaint/layer.py
+-rw-r--r--   0        0        0    22500 2024-04-02 14:46:10.869198 pytvpaint-1.0.0b5/pytvpaint/project.py
+-rw-r--r--   0        0        0        0 2024-04-02 14:46:10.869198 pytvpaint-1.0.0b5/pytvpaint/py.typed
+-rw-r--r--   0        0        0     4278 2024-04-02 14:46:10.869198 pytvpaint-1.0.0b5/pytvpaint/scene.py
+-rw-r--r--   0        0        0     8662 2024-04-02 14:46:10.869198 pytvpaint-1.0.0b5/pytvpaint/sound.py
+-rw-r--r--   0        0        0    17075 2024-04-02 14:46:10.869198 pytvpaint-1.0.0b5/pytvpaint/utils.py
+-rw-r--r--   0        0        0     4420 1970-01-01 00:00:00.000000 pytvpaint-1.0.0b5/PKG-INFO
```

### Comparing `pytvpaint-1.0.0b4/LICENSE.md` & `pytvpaint-1.0.0b5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b4/README.md` & `pytvpaint-1.0.0b5/README.md`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b4/pyproject.toml` & `pytvpaint-1.0.0b5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytvpaint"
-version = "1.0.0b4"
+version = "1.0.0b5"
 description = "Python scripting for TVPaint"
 authors = [
     "Brunch Studio Developers <dev@brunchstudio.tv>",
     "Radouane Lahmidi <rlahmidi@brunchstudio.tv>",
     "Joseph Henry <jhenry@brunchstudio.tv>",
 ]
 license = "MIT"
```

### Comparing `pytvpaint-1.0.0b4/pytvpaint/__init__.py` & `pytvpaint-1.0.0b5/pytvpaint/__init__.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b4/pytvpaint/camera.py` & `pytvpaint-1.0.0b5/pytvpaint/camera.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b4/pytvpaint/clip.py` & `pytvpaint-1.0.0b5/pytvpaint/clip.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b4/pytvpaint/george/__init__.py` & `pytvpaint-1.0.0b5/pytvpaint/george/__init__.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b4/pytvpaint/george/client/__init__.py` & `pytvpaint-1.0.0b5/pytvpaint/george/client/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,45 +20,47 @@
 
 
 def _connect_client(
     host: str = "ws://localhost", port: int = 3000, timeout: int = 60
 ) -> JSONRPCClient:
     host = os.getenv("PYTVPAINT_WS_HOST", host)
     port = int(os.getenv("PYTVPAINT_WS_PORT", port))
-    startup_connect = bool(os.getenv("PYTVPAINT_WS_STARTUP_CONNECT", 1))
+    startup_connect = bool(int(os.getenv("PYTVPAINT_WS_STARTUP_CONNECT", 1)))
     timeout = int(os.getenv("PYTVPAINT_WS_TIMEOUT", timeout))
 
-    if timeout == 0:
-        timeout = -1
-
     rpc_client = JSONRPCClient(f"{host}:{port}", timeout)
 
+    if not startup_connect:
+        return rpc_client
+
     start_time = time()
     wait_duration = 5
     connection_successful = False
 
-    while startup_connect and ((time() - start_time) < timeout):
+    while True:
+        if timeout and (time() - start_time) > timeout:
+            break
         with contextlib.suppress(ConnectionRefusedError):
             rpc_client.connect()
             connection_successful = True
             break
 
         log.warning(f"Connection refused, trying again in {wait_duration} seconds...")
         sleep(wait_duration)
 
-    if startup_connect and not connection_successful:
+    if not connection_successful:
         # Connection could not be established after timeout
         if rpc_client.is_connected:
             rpc_client.disconnect()
 
         raise ConnectionRefusedError(
             "Could not establish connection with a tvpaint instance before timeout !"
         )
 
-    if startup_connect and connection_successful:
+    if connection_successful:
         log.info(f"Connected to TVPaint on port {port}")
 
     return rpc_client
 
 
 rpc_client = _connect_client()
```

### Comparing `pytvpaint-1.0.0b4/pytvpaint/george/client/parse.py` & `pytvpaint-1.0.0b5/pytvpaint/george/client/parse.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b4/pytvpaint/george/client/rpc.py` & `pytvpaint-1.0.0b5/pytvpaint/george/client/rpc.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b4/pytvpaint/george/exceptions.py` & `pytvpaint-1.0.0b5/pytvpaint/george/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b4/pytvpaint/george/grg_base.py` & `pytvpaint-1.0.0b5/pytvpaint/george/grg_base.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b4/pytvpaint/george/grg_camera.py` & `pytvpaint-1.0.0b5/pytvpaint/george/grg_camera.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b4/pytvpaint/george/grg_clip.py` & `pytvpaint-1.0.0b5/pytvpaint/george/grg_clip.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b4/pytvpaint/george/grg_layer.py` & `pytvpaint-1.0.0b5/pytvpaint/george/grg_layer.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b4/pytvpaint/george/grg_project.py` & `pytvpaint-1.0.0b5/pytvpaint/george/grg_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,20 @@
     return BackgroundMode.COLOR, RGBColor(*map(int, values))
 
 
 def tv_background_set(
     mode: BackgroundMode,
     color: tuple[RGBColor, RGBColor] | RGBColor | None = None,
 ) -> None:
-    """Set the background mode of the project."""
+    """Set the background mode of the project.
+
+    Args:
+        mode: color mode (None, checker or one color)
+        color: None for None mode, RBGColor for one color, and tuple of RGBColors for checker
+    """
     args = []
 
     if mode == BackgroundMode.CHECK and isinstance(color, tuple):
         c1, c2 = color
         args = [c1.r, c1.g, c1.b, c2.r, c2.g, c2.b]
     elif mode == BackgroundMode.COLOR and isinstance(color, RGBColor):
         args = [color.r, color.g, color.b]
```

### Comparing `pytvpaint-1.0.0b4/pytvpaint/george/grg_scene.py` & `pytvpaint-1.0.0b5/pytvpaint/george/grg_scene.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b4/pytvpaint/layer.py` & `pytvpaint-1.0.0b5/pytvpaint/layer.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b4/pytvpaint/project.py` & `pytvpaint-1.0.0b5/pytvpaint/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,16 +262,15 @@
 
     @background_colors.setter
     @set_as_current
     def background_colors(
         self,
         colors: tuple[george.RGBColor, george.RGBColor] | george.RGBColor,
     ) -> None:
-        colors_args = colors if isinstance(colors, tuple) else [colors]
-        george.tv_background_set(self.background_mode, *colors_args)
+        george.tv_background_set(self.background_mode, colors)
 
     @set_as_current
     def clear_background(self) -> None:
         """Clear the background color and set it to None."""
         self.background_mode = george.BackgroundMode.NONE
         self.background_colors = (
             george.RGBColor(255, 255, 255),
```

### Comparing `pytvpaint-1.0.0b4/pytvpaint/scene.py` & `pytvpaint-1.0.0b5/pytvpaint/scene.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b4/pytvpaint/sound.py` & `pytvpaint-1.0.0b5/pytvpaint/sound.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b4/pytvpaint/utils.py` & `pytvpaint-1.0.0b5/pytvpaint/utils.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b4/PKG-INFO` & `pytvpaint-1.0.0b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytvpaint
-Version: 1.0.0b4
+Version: 1.0.0b5
 Summary: Python scripting for TVPaint
 Home-page: https://github.com/brunchstudio/pytvpaint
 License: MIT
 Keywords: tvpaint,brunch,tvp,george
 Author: Brunch Studio Developers
 Author-email: dev@brunchstudio.tv
 Requires-Python: >=3.9
```

