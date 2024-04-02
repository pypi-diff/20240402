# Comparing `tmp/pyviewer-1.3.8.tar.gz` & `tmp/pyviewer-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyviewer-1.3.8.tar", last modified: Wed Nov  8 12:15:26 2023, max compression
+gzip compressed data, was "pyviewer-1.3.9.tar", last modified: Mon Feb 12 10:28:44 2024, max compression
```

## Comparing `pyviewer-1.3.8.tar` & `pyviewer-1.3.9.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 12:15:26.884104 pyviewer-1.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)    20879 2023-11-08 12:15:19.000000 pyviewer-1.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2023-11-08 12:15:26.884104 pyviewer-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      967 2023-11-08 12:15:19.000000 pyviewer-1.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 12:15:26.884104 pyviewer-1.3.8/pyviewer/
--rw-r--r--   0 runner    (1001) docker     (127)  3423528 2023-11-08 12:15:19.000000 pyviewer-1.3.8/pyviewer/MPLUSRounded1c-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      333 2023-11-08 12:15:19.000000 pyviewer-1.3.8/pyviewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2023-11-08 12:15:19.000000 pyviewer-1.3.8/pyviewer/easy_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)    24765 2023-11-08 12:15:19.000000 pyviewer-1.3.8/pyviewer/gl_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)    24300 2023-11-08 12:15:19.000000 pyviewer-1.3.8/pyviewer/imgui_themes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5020 2023-11-08 12:15:19.000000 pyviewer-1.3.8/pyviewer/params.py
--rw-r--r--   0 runner    (1001) docker     (127)    71936 2023-11-08 12:15:19.000000 pyviewer-1.3.8/pyviewer/roboto_mono.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    10298 2023-11-08 12:15:19.000000 pyviewer-1.3.8/pyviewer/single_image_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10399 2023-11-08 12:15:19.000000 pyviewer-1.3.8/pyviewer/toolbar_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)    20168 2023-11-08 12:15:19.000000 pyviewer-1.3.8/pyviewer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 12:15:26.884104 pyviewer-1.3.8/pyviewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2023-11-08 12:15:26.000000 pyviewer-1.3.8/pyviewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      431 2023-11-08 12:15:26.000000 pyviewer-1.3.8/pyviewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-08 12:15:26.000000 pyviewer-1.3.8/pyviewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-11-08 12:15:26.000000 pyviewer-1.3.8/pyviewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-08 12:15:26.000000 pyviewer-1.3.8/pyviewer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-08 12:15:26.884104 pyviewer-1.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2023-11-08 12:15:19.000000 pyviewer-1.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:28:44.057263 pyviewer-1.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    20879 2024-02-12 10:28:37.000000 pyviewer-1.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-02-12 10:28:44.053263 pyviewer-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-02-12 10:28:37.000000 pyviewer-1.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:28:44.053263 pyviewer-1.3.9/pyviewer/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-02-12 10:28:37.000000 pyviewer-1.3.9/pyviewer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:28:44.053263 pyviewer-1.3.9/pyviewer/custom_ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-02-12 10:28:37.000000 pyviewer-1.3.9/pyviewer/custom_ops/cuda_gl_interop.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-02-12 10:28:37.000000 pyviewer-1.3.9/pyviewer/custom_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-12 10:28:37.000000 pyviewer-1.3.9/pyviewer/easy_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25802 2024-02-12 10:28:37.000000 pyviewer-1.3.9/pyviewer/gl_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24300 2024-02-12 10:28:37.000000 pyviewer-1.3.9/pyviewer/imgui_themes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-02-12 10:28:37.000000 pyviewer-1.3.9/pyviewer/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10332 2024-02-12 10:28:37.000000 pyviewer-1.3.9/pyviewer/single_image_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10646 2024-02-12 10:28:37.000000 pyviewer-1.3.9/pyviewer/toolbar_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20168 2024-02-12 10:28:37.000000 pyviewer-1.3.9/pyviewer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:28:44.053263 pyviewer-1.3.9/pyviewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-02-12 10:28:44.000000 pyviewer-1.3.9/pyviewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-02-12 10:28:44.000000 pyviewer-1.3.9/pyviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 10:28:44.000000 pyviewer-1.3.9/pyviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-12 10:28:44.000000 pyviewer-1.3.9/pyviewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-12 10:28:44.000000 pyviewer-1.3.9/pyviewer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 10:28:44.057263 pyviewer-1.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-02-12 10:28:37.000000 pyviewer-1.3.9/setup.py
```

### Comparing `pyviewer-1.3.8/LICENSE` & `pyviewer-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyviewer-1.3.8/PKG-INFO` & `pyviewer-1.3.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pyviewer
-Version: 1.3.8
+Version: 1.3.9
 Summary: Interactyive python viewers
 Home-page: https://github.com/harskish/pyviewer
 Author: Erik Härkönen
 Author-email: erik.harkonen@hotmail.com
 License: CC BY-NC-SA 4.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: glfw>2.0.0
 Requires-Dist: numpy
 Requires-Dist: pyopengl>3.0.0
 Requires-Dist: pyplotgui
 Requires-Dist: light-process==0.0.7
+Requires-Dist: ninja
 
 # PyViewer
 
 ![Toolbar Viewer](https://github.com/harskish/pyviewer/raw/master/docs/screenshot.jpg)
 
 Pyviewer is a python library for easily visualizing NumPy arrays and PyTorch tensors.
 
@@ -26,15 +27,15 @@
 
 A viewer for showing single fullscreen images without other UI elements. Runs in a ***separate process*** and remains interactive even if the main process is suspended (e.g. in a debugger). Great for interactively looking at intermediate values of complex ML/CG/CV pipelines.
 
 ### toolbar_viewer.py
 A viewer that shows ImGui UI elemets on the left, and a large image on the right. Runs in the main process, but supports visualizing torch tensors directly from GPU memory (unlike single_image_viewer).
 
 ## Other features
-* Bundles a custom build of PyImGui with plotting support (via ImPlot)
+* Bundles a [custom build](https://github.com/harskish/pyplotgui) of PyImGui with plotting support (via ImPlot)
 * Dynamically rescalable user interface
 * Window resizing to integer multiple of content resolution
 
 ## Installation
 `pip install pyviewer`
 
 ## Usage
```

### Comparing `pyviewer-1.3.8/README.md` & `pyviewer-1.3.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 A viewer for showing single fullscreen images without other UI elements. Runs in a ***separate process*** and remains interactive even if the main process is suspended (e.g. in a debugger). Great for interactively looking at intermediate values of complex ML/CG/CV pipelines.
 
 ### toolbar_viewer.py
 A viewer that shows ImGui UI elemets on the left, and a large image on the right. Runs in the main process, but supports visualizing torch tensors directly from GPU memory (unlike single_image_viewer).
 
 ## Other features
-* Bundles a custom build of PyImGui with plotting support (via ImPlot)
+* Bundles a [custom build](https://github.com/harskish/pyplotgui) of PyImGui with plotting support (via ImPlot)
 * Dynamically rescalable user interface
 * Window resizing to integer multiple of content resolution
 
 ## Installation
 `pip install pyviewer`
 
 ## Usage
```

### Comparing `pyviewer-1.3.8/pyviewer/gl_viewer.py` & `pyviewer-1.3.9/pyviewer/gl_viewer.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,25 +37,48 @@
     import pycuda
     import pycuda.gl as cuda_gl
     import pycuda.tools
     has_pycuda = True
 except Exception:
     pass
 
+# CUDA-GL copy via PyTorch extension
+pt_plugin = None
+try:
+    from . import custom_ops
+    pt_plugin = custom_ops.get_plugin('cuda_gl_interop', 'cuda_gl_interop.cpp', Path(__file__).parent / './custom_ops')
+except Exception:
+    pass
+
+class PTExtMapper:
+    tex: int
+    resource: int # uint64_t
+    
+    def __init__(self, tex) -> None:
+        self.tex = tex
+        self.resource = pt_plugin.register(tex)
+    
+    def unregister(self) -> None:
+        pt_plugin.unregister(self.resource)
+
+    def upload(self, ptr: int, W: int, H: int, N: int) -> None:
+        pt_plugin.upload(ptr, W, H, N, self.resource) # map, copy, unmap
+
 class _texture:
     '''
     This class maps torch tensors to gl textures without a CPU roundtrip.
     '''
     def __init__(self, min_mag_filter=gl.GL_LINEAR):
+        # Can be shared between py and c++
         self.tex = gl.glGenTextures(1)
         gl.glBindTexture(gl.GL_TEXTURE_2D, self.tex) # need to bind to modify
         # sets repeat and filtering parameters; change the second value of any tuple to change the value
         for params in ((gl.GL_TEXTURE_WRAP_S, gl.GL_REPEAT), (gl.GL_TEXTURE_WRAP_T, gl.GL_REPEAT), (gl.GL_TEXTURE_MIN_FILTER, min_mag_filter), (gl.GL_TEXTURE_MAG_FILTER, min_mag_filter)):
             gl.glTexParameteri(gl.GL_TEXTURE_2D, *params)
-        self.mapper = None
+        self.mapper = None  # pycuda mapper or torch extension cudaGraphicsResource_t
         self.is_fp = True
         self.shape = [0,0]
 
     # be sure to del textures if you create a forget them often (python doesn't necessarily call del on garbage collect)
     def __del__(self):
         gl.glDeleteTextures(1, [self.tex])
         if self.mapper is not None:
@@ -113,29 +136,29 @@
 
     def upload_torch(self, img):
         assert img.device.type == "cuda", "Please provide a CUDA tensor"
         assert img.ndim == 3, "Please provide a HWC tensor"
         assert img.shape[2] < min(img.shape[0], img.shape[1]), "Please provide a HWC tensor"
         assert img.dtype in [torch.float32, torch.uint8], 'Only fp32 and u8 supported'
 
-        if not has_pycuda:
+        if not has_pycuda and pt_plugin is None:
             return self.upload_np(img.detach().cpu().numpy())
         
         # OpenGL stores RGBA-strided data always
         # Must add alpha for gpu memcopy to work
         if img.shape[2] == 3:
             alpha = 255 if img.dtype == torch.uint8 else 1.0
             img = torch.cat((img, alpha*torch.ones_like(img[:, :, :1])), dim=-1)
 
         img = img.contiguous()
         self.upload_ptr(img.data_ptr(), img.shape, img.dtype.is_floating_point)
 
     # Copy from cuda pointer
     def upload_ptr(self, ptr, shape, is_fp32):
-        assert has_pycuda, 'PyCUDA-GL not available, cannot upload using raw pointer'
+        assert has_pycuda or pt_plugin is not None, 'PyCUDA-GL or PT plugin needed for pointer upload'
         has_alpha = shape[-1] == 4
 
         # reallocate if shape changed or data type changed from np to torch
         if shape[0] != self.shape[0] or shape[1] != self.shape[1] or self.is_fp != is_fp32 or self.mapper is None:
             self.shape = shape
             self.is_fp = is_fp32
             if self.mapper is not None:
@@ -161,41 +184,46 @@
 
             # Incoming channel format and dtype
             incoming_fmt = gl.GL_RGBA if has_alpha else gl.GL_RGB
             incoming_dtype = gl.GL_FLOAT if is_fp32 else gl.GL_UNSIGNED_BYTE # fp32 or u8
 
             gl.glTexImage2D(gl.GL_TEXTURE_2D, 0, internal_fmt, shape[1], shape[0], 0, incoming_fmt, incoming_dtype, None)
             gl.glBindTexture(gl.GL_TEXTURE_2D, 0)
-            self.mapper = cuda_gl.RegisteredImage(int(self.tex), gl.GL_TEXTURE_2D, pycuda.gl.graphics_map_flags.WRITE_DISCARD)
+            if has_pycuda:
+                self.mapper = cuda_gl.RegisteredImage(int(self.tex), gl.GL_TEXTURE_2D, pycuda.gl.graphics_map_flags.WRITE_DISCARD)
+            else:
+                self.mapper = PTExtMapper(int(self.tex))
         
-        # map texture to cuda ptr
-        tex_data = self.mapper.map()
-        tex_arr = tex_data.array(0, 0)
-
         # Cast to python integer type
         ptr_int = int(ptr)
         assert ptr_int == ptr, 'Device pointer overflow'
 
         N = 4 if is_fp32 else 1
         H, W, C = shape
         assert C == 4, 'Input data must be RGBA' # OpenGL always stores alpha channel
-        
-        # copy from torch tensor to mapped gl texture (avoid cpu roundtrip)
-        # https://documen.tician.de/pycuda/driver.html#pycuda.driver.Memcpy2D
-        cpy = pycuda.driver.Memcpy2D()
-        cpy.set_src_device(ptr_int)
-        cpy.set_dst_array(tex_arr)
-        cpy.width_in_bytes = W*C*N  # Number of bytes to copy for each row in the transfer
-        cpy.src_pitch = W*C*N       # Size of a row in bytes at the origin of the copy
-        cpy.dst_pitch = W*C*N       # Size of a row in bytes at the destination of the copy
-        cpy.height = H
-        cpy(aligned=False)
 
-        # cleanup
-        tex_data.unmap()
+        if has_pycuda:
+            # map texture to cuda ptr
+            tex_data = self.mapper.map()
+            tex_arr = tex_data.array(0, 0)
+            
+            # copy from torch tensor to mapped gl texture (avoid cpu roundtrip)
+            # https://documen.tician.de/pycuda/driver.html#pycuda.driver.Memcpy2D
+            cpy = pycuda.driver.Memcpy2D()
+            cpy.set_src_device(ptr_int)
+            cpy.set_dst_array(tex_arr)
+            cpy.width_in_bytes = W*C*N  # Number of bytes to copy for each row in the transfer
+            cpy.src_pitch = W*C*N       # Size of a row in bytes at the origin of the copy
+            cpy.dst_pitch = W*C*N       # Size of a row in bytes at the destination of the copy
+            cpy.height = H
+            cpy(aligned=False)
+            tex_data.unmap()
+        else:
+            self.mapper.upload(ptr_int, W, H, C*N)
+
         cuda_synchronize()
 
 class _editable:
     def __init__(self, name, ui_code = '', run_code = ''):
         self.name = name
         self.ui_code = ui_code if len(ui_code)>0 else 'imgui.begin(\'Test\')\nimgui.text(\'Example\')#your code here!\nimgui.end()'
         self.tentative_ui_code = self.ui_code
@@ -245,16 +273,16 @@
         
         fname = inifile or "".join(c for c in title.lower() if c.isalnum())
         self._inifile = Path(fname).with_suffix('.ini')
 
         if not glfw.init():
             raise RuntimeError('GLFW init failed')
 
-        if not has_pycuda:
-            print('PyCUDA with GL support not available, images will be uploaded from RAM.')
+        if not has_pycuda and pt_plugin is None:
+            print('Neither PyCUDA-GL nor Torch+CUDA available, images will be uploaded from RAM.')
         
         try:
             with open(self._inifile, 'r') as file:
                 self._width, self._height = [int(i) for i in file.readline().split()]
                 self.window_pos = [int(i) for i in file.readline().split()]
                 start_maximized = int(file.readline().rstrip())
                 self.ui_scale = float(file.readline().rstrip())
```

### Comparing `pyviewer-1.3.8/pyviewer/imgui_themes.py` & `pyviewer-1.3.9/pyviewer/imgui_themes.py`

 * *Files identical despite different names*

### Comparing `pyviewer-1.3.8/pyviewer/params.py` & `pyviewer-1.3.9/pyviewer/params.py`

 * *Files identical despite different names*

### Comparing `pyviewer-1.3.8/pyviewer/single_image_viewer.py` & `pyviewer-1.3.9/pyviewer/single_image_viewer.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,11 +269,12 @@
 # No-op if already open, therwise (re)start
 def show_window():
     # Elif to avoid immediate restart if first init
     if inst is None:
         init('SIV')
     elif not inst.started.value:
         inst.restart()
+        inst.paused.value = False
 
 def draw(*, img_hwc=None, img_chw=None, ignore_pause=False):
     init('SIV') # no-op if init already performed
     inst.draw(img_hwc, img_chw, ignore_pause)
```

### Comparing `pyviewer-1.3.8/pyviewer/toolbar_viewer.py` & `pyviewer-1.3.9/pyviewer/toolbar_viewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,17 @@
         cW, cH = [int(r-l) for l,r in zip(rmin, rmax)]
         
         # Compute size of image that fills smaller dimension
         # Bottom area for integer scaling buttons taken into account
         aspect = self.img_shape[2] / self.img_shape[1]
         out_width = min(cW, aspect*(cH - BOTTOM_PAD))
         self.content_size_px = (int(out_width), int(out_width / aspect))
+
+        # Draw UI elements before image
+        self.draw_pre()
         
         # Create imgui.image from provided data
         tex_in = v._images.get(self.output_key)
         if tex_in:
             canvas_size = (cW, cH - BOTTOM_PAD)
             tex = self.pan_handler.draw_to_canvas(tex_in.tex, *self.content_size_px, *canvas_size, self.pan_enabled)
             imgui.image(tex, *canvas_size)
@@ -243,14 +246,20 @@
     def draw_toolbar(self):
         pass
 
     # Draw extra UI elements below output image
     def draw_output_extra(self):
         if self._user_pad_bottom > 0:
             raise RuntimeError('Not implemented')
+    
+    # Draw UI elements before main image is drawn
+    # Can be (ab)used to draw only plots by never
+    # returning an image form compute()
+    def draw_pre(self):
+        pass
 
     # Draw overlays using main window draw list
     def draw_overlays(self, draw_list):
         pass
 
     def draw_menu(self):
         pass
```

### Comparing `pyviewer-1.3.8/pyviewer/utils.py` & `pyviewer-1.3.9/pyviewer/utils.py`

 * *Files identical despite different names*

### Comparing `pyviewer-1.3.8/pyviewer.egg-info/PKG-INFO` & `pyviewer-1.3.9/pyviewer.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pyviewer
-Version: 1.3.8
+Version: 1.3.9
 Summary: Interactyive python viewers
 Home-page: https://github.com/harskish/pyviewer
 Author: Erik Härkönen
 Author-email: erik.harkonen@hotmail.com
 License: CC BY-NC-SA 4.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: glfw>2.0.0
 Requires-Dist: numpy
 Requires-Dist: pyopengl>3.0.0
 Requires-Dist: pyplotgui
 Requires-Dist: light-process==0.0.7
+Requires-Dist: ninja
 
 # PyViewer
 
 ![Toolbar Viewer](https://github.com/harskish/pyviewer/raw/master/docs/screenshot.jpg)
 
 Pyviewer is a python library for easily visualizing NumPy arrays and PyTorch tensors.
 
@@ -26,15 +27,15 @@
 
 A viewer for showing single fullscreen images without other UI elements. Runs in a ***separate process*** and remains interactive even if the main process is suspended (e.g. in a debugger). Great for interactively looking at intermediate values of complex ML/CG/CV pipelines.
 
 ### toolbar_viewer.py
 A viewer that shows ImGui UI elemets on the left, and a large image on the right. Runs in the main process, but supports visualizing torch tensors directly from GPU memory (unlike single_image_viewer).
 
 ## Other features
-* Bundles a custom build of PyImGui with plotting support (via ImPlot)
+* Bundles a [custom build](https://github.com/harskish/pyplotgui) of PyImGui with plotting support (via ImPlot)
 * Dynamically rescalable user interface
 * Window resizing to integer multiple of content resolution
 
 ## Installation
 `pip install pyviewer`
 
 ## Usage
```

### Comparing `pyviewer-1.3.8/setup.py` & `pyviewer-1.3.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,30 +10,32 @@
 
 # Workflow:
 # Increment version number (together with other changes)
 # git commit
 # git tag -a "vX.X.X" -m "vX.X.X"  (only annotated tags show up in GitHub)
 # git push --follow-tags
 setup(name='pyviewer',
-    version='1.3.8',
+    version='1.3.9',
     description='Interactyive python viewers',
     author='Erik Härkönen',
     author_email='erik.harkonen@hotmail.com',
     url='https://github.com/harskish/pyviewer',
     packages=['pyviewer'], # name of importable thing
     setup_requires=['wheel'],
     install_requires=[
         'glfw>2.0.0',
         'numpy',
         'pyopengl>3.0.0',
         'pyplotgui',  # custom imgui+implot package
         'light-process==0.0.7',
+        'ninja', # for custom OP
     ],
     include_package_data=True,
     package_data={
-        '': ['*.ttf'] # embedded fonts
+        '': ['*.ttf'], # embedded fonts
+        '': ['custom_ops/*.cpp'], # custom CUDA op
     },
     long_description=Path('README.md').read_text()
         .replace('docs/screenshot.jpg', 'https://github.com/harskish/pyviewer/raw/master/docs/screenshot.jpg'),
     long_description_content_type="text/markdown",
     license='CC BY-NC-SA 4.0',
 )
```

