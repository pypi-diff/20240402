# Comparing `tmp/zz-pix-0.0.3.tar.gz` & `tmp/zz-pix-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zz-pix-0.0.3.tar", last modified: Sat Mar 30 19:07:04 2024, max compression
+gzip compressed data, was "zz-pix-0.0.4.tar", last modified: Mon Apr  1 22:08:32 2024, max compression
```

## Comparing `zz-pix-0.0.3.tar` & `zz-pix-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-03-30 19:07:04.824689 zz-pix-0.0.3/
--rw-rw-rw-   0        0        0    11541 2024-03-29 15:51:16.000000 zz-pix-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     3399 2024-03-30 19:07:04.824689 zz-pix-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-30 19:07:04.816395 zz-pix-0.0.3/pix/
--rw-rw-rw-   0        0        0        0 2024-03-29 15:51:16.000000 zz-pix-0.0.3/pix/__init__.py
--rw-rw-rw-   0        0        0     3341 2024-03-30 17:59:52.000000 zz-pix-0.0.3/pix/cli_parser.py
--rw-rw-rw-   0        0        0     2856 2024-03-29 15:51:16.000000 zz-pix-0.0.3/pix/converter.py
--rw-rw-rw-   0        0        0     3852 2024-03-29 15:51:16.000000 zz-pix-0.0.3/pix/croper.py
--rw-rw-rw-   0        0        0     3484 2024-03-30 18:07:27.000000 zz-pix-0.0.3/pix/main.py
--rw-rw-rw-   0        0        0      182 2024-03-30 19:06:35.000000 zz-pix-0.0.3/pix/manifest.json
--rw-rw-rw-   0        0        0      588 2024-03-30 18:15:25.000000 zz-pix-0.0.3/pix/prune.py
--rw-rw-rw-   0        0        0     1580 2024-03-29 15:51:16.000000 zz-pix-0.0.3/pix/resizer.py
--rw-rw-rw-   0        0        0      706 2024-03-29 18:51:50.000000 zz-pix-0.0.3/pix/utils.py
--rw-rw-rw-   0        0        0       42 2024-03-30 19:07:04.824689 zz-pix-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1654 2024-03-30 19:00:22.000000 zz-pix-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-30 19:07:04.824689 zz-pix-0.0.3/zz_pix.egg-info/
--rw-rw-rw-   0        0        0     3399 2024-03-30 19:07:04.000000 zz-pix-0.0.3/zz_pix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      334 2024-03-30 19:07:04.000000 zz-pix-0.0.3/zz_pix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-30 19:07:04.000000 zz-pix-0.0.3/zz_pix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-03-30 19:07:04.000000 zz-pix-0.0.3/zz_pix.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       38 2024-03-30 19:07:04.000000 zz-pix-0.0.3/zz_pix.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-03-30 19:07:04.000000 zz-pix-0.0.3/zz_pix.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 22:08:32.113780 zz-pix-0.0.4/
+-rw-rw-rw-   0        0        0    11541 2024-03-29 15:51:16.000000 zz-pix-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     3601 2024-04-01 22:08:32.112278 zz-pix-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-01 22:08:32.102768 zz-pix-0.0.4/pix/
+-rw-rw-rw-   0        0        0        0 2024-03-29 15:51:16.000000 zz-pix-0.0.4/pix/__init__.py
+-rw-rw-rw-   0        0        0     2661 2024-04-01 21:55:37.000000 zz-pix-0.0.4/pix/blip.py
+-rw-rw-rw-   0        0        0     4579 2024-04-01 21:55:54.000000 zz-pix-0.0.4/pix/cli_parser.py
+-rw-rw-rw-   0        0        0     2856 2024-03-29 15:51:16.000000 zz-pix-0.0.4/pix/converter.py
+-rw-rw-rw-   0        0        0     3852 2024-03-29 15:51:16.000000 zz-pix-0.0.4/pix/croper.py
+-rw-rw-rw-   0        0        0     4431 2024-04-01 22:03:29.000000 zz-pix-0.0.4/pix/main.py
+-rw-rw-rw-   0        0        0      182 2024-04-01 16:45:01.000000 zz-pix-0.0.4/pix/manifest.json
+-rw-rw-rw-   0        0        0      588 2024-03-30 18:15:25.000000 zz-pix-0.0.4/pix/prune.py
+-rw-rw-rw-   0        0        0     1580 2024-03-29 15:51:16.000000 zz-pix-0.0.4/pix/resizer.py
+-rw-rw-rw-   0        0        0      706 2024-03-29 18:51:50.000000 zz-pix-0.0.4/pix/utils.py
+-rw-rw-rw-   0        0        0       42 2024-04-01 22:08:32.113780 zz-pix-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1789 2024-04-01 18:25:17.000000 zz-pix-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 22:08:32.112278 zz-pix-0.0.4/zz_pix.egg-info/
+-rw-rw-rw-   0        0        0     3601 2024-04-01 22:08:32.000000 zz-pix-0.0.4/zz_pix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2024-04-01 22:08:32.000000 zz-pix-0.0.4/zz_pix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 22:08:32.000000 zz-pix-0.0.4/zz_pix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-04-01 22:08:32.000000 zz-pix-0.0.4/zz_pix.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       90 2024-04-01 22:08:32.000000 zz-pix-0.0.4/zz_pix.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-01 22:08:32.000000 zz-pix-0.0.4/zz_pix.egg-info/top_level.txt
```

### Comparing `zz-pix-0.0.3/LICENSE` & `zz-pix-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zz-pix-0.0.3/PKG-INFO` & `zz-pix-0.0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zz-pix
-Version: 0.0.3
+Version: 0.0.4
 Summary: CLI tool for image manipulation
 Home-page: https://github.com/sean1832/pix
 Author: Zeke Zhang
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,14 +18,21 @@
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Multimedia :: Graphics :: Graphics Conversion
 Classifier: Topic :: Multimedia :: Graphics :: Editors
 Classifier: Topic :: Multimedia :: Graphics :: Editors :: Raster-Based
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pillow
+Requires-Dist: pillow-avif-plugin
+Requires-Dist: pillow-heif
+Requires-Dist: transformers>=4.39.2
+Requires-Dist: torch>=2.2.2
+Requires-Dist: termcolor
+Requires-Dist: pyexiv2
 
 # PIX
 a simple image manipulation tool for the terminal
 
 ## Features
 - [x] Resize
 - [x] Crop
```

### Comparing `zz-pix-0.0.3/pix/converter.py` & `zz-pix-0.0.4/pix/converter.py`

 * *Files identical despite different names*

### Comparing `zz-pix-0.0.3/pix/croper.py` & `zz-pix-0.0.4/pix/croper.py`

 * *Files identical despite different names*

### Comparing `zz-pix-0.0.3/pix/main.py` & `zz-pix-0.0.4/pix/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+import glob
 import pathlib
 import traceback
 
-from pix import cli_parser, converter, croper, prune, resizer
+import pyexiv2
+
+from pix import cli_parser, converter, croper, prune, resizer, utils
 
 
 def get_io_paths(args):
     file_input = pathlib.Path(args.input)
     file_output = pathlib.Path(args.output)
     return file_input, file_output
 
@@ -45,17 +48,15 @@
             file_input,
             file_output,
             args.size,
             args.scale,
             args.overwrite,
         )
     elif file_input.is_dir():
-        resizer.resize_images(
-            file_input, file_output, args.size, args.scale, args.overwrite
-        )
+        resizer.resize_images(file_input, file_output, args.size, args.scale, args.overwrite)
     else:
         raise FileNotFoundError(f"`{args.input}` not found.")
 
 
 def crop_cmd(args):
     file_input, file_output = get_io_paths(args)
     if file_input.is_file():
@@ -87,14 +88,38 @@
         prune.prune_image(file_input, args.resolution, args.dry_run)
     elif file_input.is_dir():
         prune.prune_images(file_input, args.resolution, args.dry_run)
     else:
         raise FileNotFoundError(f"`{args.input}` not found.")
 
 
+def blip_cmd(args):
+    from pix.blip import Blip
+
+    file_input = pathlib.Path(args.input).absolute()
+    if file_input.is_dir():
+        file_input = file_input.joinpath("*.*")
+    inputs = glob.glob(str(file_input))  # wildcard
+    # filter out non-image files
+    inputs = [i for i in inputs if utils.is_file_supported(i)]
+
+    blip = Blip(args.large, args.cpu, args.blip2)
+
+    caption_dicts = blip.caption_image(
+        inputs, args.token, args.seed, args.temperature, args.batch, args.prompt, args.question
+    )
+    for image, caption_dict in zip(inputs, caption_dicts):
+        caption = caption_dict[0]["generated_text"]
+        if args.metadata:
+            with pyexiv2.Image(image) as img:
+                img.modify_exif({"Exif.Image.XPComment": caption})
+
+        print(f"\n{image} - {caption}")
+
+
 def main():
     try:
         parser = cli_parser.get_parser()
         args = parser.parse_args()
         if args.command is None:
             parser.print_help()
             return
@@ -110,14 +135,19 @@
         # Crop command
         elif args.command == "crop":
             crop_cmd(args)
 
         # Prune command
         elif args.command == "prune":
             prune_cmd(args)
+
+        # Blip command
+        elif args.command == "blip":
+            blip_cmd(args)
+
         print("Done!")
     except FileNotFoundError as e:
         print("File not found:", e)
         exit(1)
     except FileExistsError as e:
         print(e)
         exit(1)
```

### Comparing `zz-pix-0.0.3/pix/prune.py` & `zz-pix-0.0.4/pix/prune.py`

 * *Files identical despite different names*

### Comparing `zz-pix-0.0.3/pix/resizer.py` & `zz-pix-0.0.4/pix/resizer.py`

 * *Files identical despite different names*

### Comparing `zz-pix-0.0.3/pix/utils.py` & `zz-pix-0.0.4/pix/utils.py`

 * *Files identical despite different names*

### Comparing `zz-pix-0.0.3/setup.py` & `zz-pix-0.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,15 +16,23 @@
     packages=find_packages(),
     include_package_data=True,
     package_data={
         "": [
             "manifest.json",
         ]
     },
-    install_requires=["pillow", "pillow-avif-plugin", "pillow-heif"],
+    install_requires=[
+        "pillow",
+        "pillow-avif-plugin",
+        "pillow-heif",
+        "transformers>=4.39.2",
+        "torch>=2.2.2",
+        "termcolor",
+        "pyexiv2",
+    ],
     entry_points={
         "console_scripts": [
             "pix = pix.main:main",
         ],
     },
     python_requires=">=3.9",
     # https://pypi.org/classifiers/
```

### Comparing `zz-pix-0.0.3/zz_pix.egg-info/PKG-INFO` & `zz-pix-0.0.4/zz_pix.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zz-pix
-Version: 0.0.3
+Version: 0.0.4
 Summary: CLI tool for image manipulation
 Home-page: https://github.com/sean1832/pix
 Author: Zeke Zhang
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,14 +18,21 @@
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Multimedia :: Graphics :: Graphics Conversion
 Classifier: Topic :: Multimedia :: Graphics :: Editors
 Classifier: Topic :: Multimedia :: Graphics :: Editors :: Raster-Based
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pillow
+Requires-Dist: pillow-avif-plugin
+Requires-Dist: pillow-heif
+Requires-Dist: transformers>=4.39.2
+Requires-Dist: torch>=2.2.2
+Requires-Dist: termcolor
+Requires-Dist: pyexiv2
 
 # PIX
 a simple image manipulation tool for the terminal
 
 ## Features
 - [x] Resize
 - [x] Crop
```

