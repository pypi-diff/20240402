# Comparing `tmp/zz-pix-0.0.5.tar.gz` & `tmp/zz-pix-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zz-pix-0.0.5.tar", last modified: Mon Apr  1 22:28:00 2024, max compression
+gzip compressed data, was "zz-pix-0.0.6.tar", last modified: Tue Apr  2 12:16:23 2024, max compression
```

## Comparing `zz-pix-0.0.5.tar` & `zz-pix-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 22:28:00.835146 zz-pix-0.0.5/
--rw-rw-rw-   0        0        0    11541 2024-03-29 15:51:16.000000 zz-pix-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     3601 2024-04-01 22:28:00.834147 zz-pix-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-01 22:28:00.822374 zz-pix-0.0.5/pix/
--rw-rw-rw-   0        0        0        0 2024-03-29 15:51:16.000000 zz-pix-0.0.5/pix/__init__.py
--rw-rw-rw-   0        0        0     2837 2024-04-01 22:27:14.000000 zz-pix-0.0.5/pix/blip.py
--rw-rw-rw-   0        0        0     4579 2024-04-01 21:55:54.000000 zz-pix-0.0.5/pix/cli_parser.py
--rw-rw-rw-   0        0        0     2856 2024-03-29 15:51:16.000000 zz-pix-0.0.5/pix/converter.py
--rw-rw-rw-   0        0        0     3852 2024-03-29 15:51:16.000000 zz-pix-0.0.5/pix/croper.py
--rw-rw-rw-   0        0        0     4431 2024-04-01 22:03:29.000000 zz-pix-0.0.5/pix/main.py
--rw-rw-rw-   0        0        0      182 2024-04-01 22:27:53.000000 zz-pix-0.0.5/pix/manifest.json
--rw-rw-rw-   0        0        0      588 2024-03-30 18:15:25.000000 zz-pix-0.0.5/pix/prune.py
--rw-rw-rw-   0        0        0     1580 2024-03-29 15:51:16.000000 zz-pix-0.0.5/pix/resizer.py
--rw-rw-rw-   0        0        0      706 2024-03-29 18:51:50.000000 zz-pix-0.0.5/pix/utils.py
--rw-rw-rw-   0        0        0       42 2024-04-01 22:28:00.835146 zz-pix-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1789 2024-04-01 18:25:17.000000 zz-pix-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-01 22:28:00.834147 zz-pix-0.0.5/zz_pix.egg-info/
--rw-rw-rw-   0        0        0     3601 2024-04-01 22:28:00.000000 zz-pix-0.0.5/zz_pix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2024-04-01 22:28:00.000000 zz-pix-0.0.5/zz_pix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 22:28:00.000000 zz-pix-0.0.5/zz_pix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-04-01 22:28:00.000000 zz-pix-0.0.5/zz_pix.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       90 2024-04-01 22:28:00.000000 zz-pix-0.0.5/zz_pix.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-01 22:28:00.000000 zz-pix-0.0.5/zz_pix.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 12:16:23.298185 zz-pix-0.0.6/
+-rw-rw-rw-   0        0        0    11541 2024-03-29 15:51:16.000000 zz-pix-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     6703 2024-04-02 12:16:23.298185 zz-pix-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-02 12:16:23.285631 zz-pix-0.0.6/pix/
+-rw-rw-rw-   0        0        0        0 2024-03-29 15:51:16.000000 zz-pix-0.0.6/pix/__init__.py
+-rw-rw-rw-   0        0        0     4614 2024-04-02 11:30:53.000000 zz-pix-0.0.6/pix/caption.py
+-rw-rw-rw-   0        0        0     4497 2024-04-02 11:53:42.000000 zz-pix-0.0.6/pix/cli_parser.py
+-rw-rw-rw-   0        0        0     2856 2024-03-29 15:51:16.000000 zz-pix-0.0.6/pix/converter.py
+-rw-rw-rw-   0        0        0     3852 2024-03-29 15:51:16.000000 zz-pix-0.0.6/pix/croper.py
+-rw-rw-rw-   0        0        0     4456 2024-04-02 12:14:29.000000 zz-pix-0.0.6/pix/main.py
+-rw-rw-rw-   0        0        0      182 2024-04-02 11:48:56.000000 zz-pix-0.0.6/pix/manifest.json
+-rw-rw-rw-   0        0        0      588 2024-03-30 18:15:25.000000 zz-pix-0.0.6/pix/prune.py
+-rw-rw-rw-   0        0        0     1580 2024-03-29 15:51:16.000000 zz-pix-0.0.6/pix/resizer.py
+-rw-rw-rw-   0        0        0      706 2024-03-29 18:51:50.000000 zz-pix-0.0.6/pix/utils.py
+-rw-rw-rw-   0        0        0       42 2024-04-02 12:16:23.298185 zz-pix-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1789 2024-04-01 18:25:17.000000 zz-pix-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:16:23.297186 zz-pix-0.0.6/zz_pix.egg-info/
+-rw-rw-rw-   0        0        0     6703 2024-04-02 12:16:23.000000 zz-pix-0.0.6/zz_pix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2024-04-02 12:16:23.000000 zz-pix-0.0.6/zz_pix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 12:16:23.000000 zz-pix-0.0.6/zz_pix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-04-02 12:16:23.000000 zz-pix-0.0.6/zz_pix.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       90 2024-04-02 12:16:23.000000 zz-pix-0.0.6/zz_pix.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-02 12:16:23.000000 zz-pix-0.0.6/zz_pix.egg-info/top_level.txt
```

### Comparing `zz-pix-0.0.5/LICENSE` & `zz-pix-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `zz-pix-0.0.5/pix/cli_parser.py` & `zz-pix-0.0.6/pix/cli_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,23 +44,22 @@
     # prune command
     prune_parser = subparser.add_parser("prune", help="Remove images smaller than specified resolution")
     prune_parser.add_argument("input", type=str, help="Input image or directory")
     prune_parser.add_argument("-r", "--resolution", type=str, help="Minimum resolution as WxH. Images smaller than this will be removed.")
     prune_parser.add_argument("--dry-run", action="store_true", help="Perform a dry run without deleting files.")
 
     # blip command
-    blip_parser = subparser.add_parser("blip", help="Blip caption on images")
+    blip_parser = subparser.add_parser("caption", help="Caption on images")
     blip_parser.add_argument("input", type=str, help="Input image or directory")
-    blip_parser.add_argument("--json", type=str, help="export JSON file containing captions")
-    blip_parser.add_argument("--token", type=int, help="Max token length for captioning", default=32)
-    blip_parser.add_argument("--batch", type=int, help="Batch size for captioning", default=8)
-    blip_parser.add_argument("--temperature", type=float, help="Temperature for captioning", default=0.8)
+    blip_parser.add_argument("-t", "--token", type=int, help="Max token length for captioning", default=32)
+    blip_parser.add_argument("-b", "--batch", type=int, help="Batch size for captioning", default=1)
+    blip_parser.add_argument("-p", "--prompt", type=str, help="Prompt for captioning")
+    blip_parser.add_argument("--temperature", type=float, help="Temperature for captioning", default=1.0)
     blip_parser.add_argument("--seed", type=int, help="Seed for reproducibility")
-    blip_parser.add_argument("--prompt", type=str, help="Prompt for captioning")
     blip_parser.add_argument("--large", action="store_true", help="Use the large model")
     blip_parser.add_argument("--cpu", action="store_true", help="Use CPU instead of GPU")
-    blip_parser.add_argument("--question", action="store_true", help="QA mode for captioning")
     blip_parser.add_argument("--metadata", action="store_true", help="Write caption as metadata for image")
     blip_parser.add_argument("--blip2", action="store_true", help="Use Blip2 model for captioning")
+    blip_parser.add_argument("--verbose", action="store_true", help="Print verbose output")
 
     return parser
 # fmt: on
```

### Comparing `zz-pix-0.0.5/pix/converter.py` & `zz-pix-0.0.6/pix/converter.py`

 * *Files identical despite different names*

### Comparing `zz-pix-0.0.5/pix/croper.py` & `zz-pix-0.0.6/pix/croper.py`

 * *Files identical despite different names*

### Comparing `zz-pix-0.0.5/pix/main.py` & `zz-pix-0.0.6/pix/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -88,36 +88,36 @@
         prune.prune_image(file_input, args.resolution, args.dry_run)
     elif file_input.is_dir():
         prune.prune_images(file_input, args.resolution, args.dry_run)
     else:
         raise FileNotFoundError(f"`{args.input}` not found.")
 
 
-def blip_cmd(args):
-    from pix.blip import Blip
+def caption_cmd(args):
+    from pix.caption import Blip
 
     file_input = pathlib.Path(args.input).absolute()
     if file_input.is_dir():
         file_input = file_input.joinpath("*.*")
     inputs = glob.glob(str(file_input))  # wildcard
     # filter out non-image files
     inputs = [i for i in inputs if utils.is_file_supported(i)]
 
     blip = Blip(args.large, args.cpu, args.blip2)
 
     caption_dicts = blip.caption_image(
-        inputs, args.token, args.seed, args.temperature, args.batch, args.prompt, args.question
+        inputs, args.token, args.seed, args.temperature, args.batch, args.prompt
     )
     for image, caption_dict in zip(inputs, caption_dicts):
         caption = caption_dict[0]["generated_text"]
         if args.metadata:
             with pyexiv2.Image(image) as img:
                 img.modify_exif({"Exif.Image.XPComment": caption})
-
-        print(f"\n{image} - {caption}")
+        if args.verbose:
+            print(f"\n{image} - {caption}")
 
 
 def main():
     try:
         parser = cli_parser.get_parser()
         args = parser.parse_args()
         if args.command is None:
@@ -137,16 +137,16 @@
             crop_cmd(args)
 
         # Prune command
         elif args.command == "prune":
             prune_cmd(args)
 
         # Blip command
-        elif args.command == "blip":
-            blip_cmd(args)
+        elif args.command == "caption":
+            caption_cmd(args)
 
         print("Done!")
     except FileNotFoundError as e:
         print("File not found:", e)
         exit(1)
     except FileExistsError as e:
         print(e)
```

### Comparing `zz-pix-0.0.5/pix/prune.py` & `zz-pix-0.0.6/pix/prune.py`

 * *Files identical despite different names*

### Comparing `zz-pix-0.0.5/pix/resizer.py` & `zz-pix-0.0.6/pix/resizer.py`

 * *Files identical despite different names*

### Comparing `zz-pix-0.0.5/pix/utils.py` & `zz-pix-0.0.6/pix/utils.py`

 * *Files identical despite different names*

### Comparing `zz-pix-0.0.5/setup.py` & `zz-pix-0.0.6/setup.py`

 * *Files identical despite different names*

