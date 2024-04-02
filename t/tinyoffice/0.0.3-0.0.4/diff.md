# Comparing `tmp/tinyoffice-0.0.3.tar.gz` & `tmp/tinyoffice-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyoffice-0.0.3.tar", last modified: Mon Apr  1 13:56:46 2024, max compression
+gzip compressed data, was "tinyoffice-0.0.4.tar", last modified: Tue Apr  2 15:24:46 2024, max compression
```

## Comparing `tinyoffice-0.0.3.tar` & `tinyoffice-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-04-01 13:56:46.424853 tinyoffice-0.0.3/
--rw-r--r--   0 sam        (501) staff       (20)     1864 2024-04-01 01:59:02.000000 tinyoffice-0.0.3/.gitignore
--rw-r--r--   0 sam        (501) staff       (20)     1072 2024-03-31 12:26:00.000000 tinyoffice-0.0.3/LICENSE
--rw-r--r--   0 sam        (501) staff       (20)     2748 2024-04-01 13:56:46.424625 tinyoffice-0.0.3/PKG-INFO
--rw-r--r--   0 sam        (501) staff       (20)     2230 2024-04-01 13:55:05.000000 tinyoffice-0.0.3/README.md
--rw-r--r--   0 sam        (501) staff       (20)      692 2024-04-01 13:56:39.000000 tinyoffice-0.0.3/pyproject.toml
--rw-r--r--   0 sam        (501) staff       (20)       38 2024-04-01 13:56:46.424930 tinyoffice-0.0.3/setup.cfg
-drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-04-01 13:56:46.423608 tinyoffice-0.0.3/tinyoffice/
--rw-r--r--   0 sam        (501) staff       (20)        0 2024-03-31 12:26:00.000000 tinyoffice-0.0.3/tinyoffice/__init__.py
--rw-r--r--   0 sam        (501) staff       (20)     5694 2024-04-01 01:59:29.000000 tinyoffice-0.0.3/tinyoffice/__main__.py
--rw-r--r--   0 sam        (501) staff       (20)    22375 2024-04-01 13:53:53.000000 tinyoffice-0.0.3/tinyoffice/tinyoffice.py
-drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-04-01 13:56:46.424382 tinyoffice-0.0.3/tinyoffice.egg-info/
--rw-r--r--   0 sam        (501) staff       (20)     2748 2024-04-01 13:56:46.000000 tinyoffice-0.0.3/tinyoffice.egg-info/PKG-INFO
--rw-r--r--   0 sam        (501) staff       (20)      283 2024-04-01 13:56:46.000000 tinyoffice-0.0.3/tinyoffice.egg-info/SOURCES.txt
--rw-r--r--   0 sam        (501) staff       (20)        1 2024-04-01 13:56:46.000000 tinyoffice-0.0.3/tinyoffice.egg-info/dependency_links.txt
--rw-r--r--   0 sam        (501) staff       (20)        7 2024-04-01 13:56:46.000000 tinyoffice-0.0.3/tinyoffice.egg-info/requires.txt
--rw-r--r--   0 sam        (501) staff       (20)       21 2024-04-01 13:56:46.000000 tinyoffice-0.0.3/tinyoffice.egg-info/top_level.txt
+drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-04-02 15:24:46.259314 tinyoffice-0.0.4/
+-rw-r--r--   0 sam        (501) staff       (20)     1864 2024-04-01 01:59:02.000000 tinyoffice-0.0.4/.gitignore
+-rw-r--r--   0 sam        (501) staff       (20)     1072 2024-03-31 12:26:00.000000 tinyoffice-0.0.4/LICENSE
+-rw-r--r--   0 sam        (501) staff       (20)     2748 2024-04-02 15:24:46.259107 tinyoffice-0.0.4/PKG-INFO
+-rw-r--r--   0 sam        (501) staff       (20)     2230 2024-04-01 13:55:05.000000 tinyoffice-0.0.4/README.md
+-rw-r--r--   0 sam        (501) staff       (20)      692 2024-04-02 15:24:33.000000 tinyoffice-0.0.4/pyproject.toml
+-rw-r--r--   0 sam        (501) staff       (20)       38 2024-04-02 15:24:46.259352 tinyoffice-0.0.4/setup.cfg
+drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-04-02 15:24:46.257815 tinyoffice-0.0.4/tinyoffice/
+-rw-r--r--   0 sam        (501) staff       (20)        0 2024-03-31 12:26:00.000000 tinyoffice-0.0.4/tinyoffice/__init__.py
+-rw-r--r--   0 sam        (501) staff       (20)     5694 2024-04-02 15:22:26.000000 tinyoffice-0.0.4/tinyoffice/__main__.py
+-rw-r--r--   0 sam        (501) staff       (20)    23487 2024-04-02 15:23:46.000000 tinyoffice-0.0.4/tinyoffice/tinyoffice.py
+drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-04-02 15:24:46.258853 tinyoffice-0.0.4/tinyoffice.egg-info/
+-rw-r--r--   0 sam        (501) staff       (20)     2748 2024-04-02 15:24:46.000000 tinyoffice-0.0.4/tinyoffice.egg-info/PKG-INFO
+-rw-r--r--   0 sam        (501) staff       (20)      283 2024-04-02 15:24:46.000000 tinyoffice-0.0.4/tinyoffice.egg-info/SOURCES.txt
+-rw-r--r--   0 sam        (501) staff       (20)        1 2024-04-02 15:24:46.000000 tinyoffice-0.0.4/tinyoffice.egg-info/dependency_links.txt
+-rw-r--r--   0 sam        (501) staff       (20)        7 2024-04-02 15:24:46.000000 tinyoffice-0.0.4/tinyoffice.egg-info/requires.txt
+-rw-r--r--   0 sam        (501) staff       (20)       21 2024-04-02 15:24:46.000000 tinyoffice-0.0.4/tinyoffice.egg-info/top_level.txt
```

### Comparing `tinyoffice-0.0.3/.gitignore` & `tinyoffice-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `tinyoffice-0.0.3/LICENSE` & `tinyoffice-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyoffice-0.0.3/PKG-INFO` & `tinyoffice-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyoffice
-Version: 0.0.3
+Version: 0.0.4
 Summary: Make your Office files tiny!
 Author-email: Samuel Woodward <sam@woodward.fyi>
 Project-URL: Homepage, https://github.com/PyWoody/tinyoffice
 Keywords: office,compress,convert,image,Word,Excel,Powerpoint
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tinyoffice-0.0.3/README.md` & `tinyoffice-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `tinyoffice-0.0.3/pyproject.toml` & `tinyoffice-0.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 keywords = ["office", "compress", "convert", "image", "Word", "Excel", "Powerpoint"]
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-version = "0.0.3"
+version = "0.0.4"
 dependencies = ["Pillow"]
 
 [project.urls]
 Homepage = "https://github.com/PyWoody/tinyoffice"
 
 [tool.setuptools.packages.find]
 exclude = ["data"]
```

### Comparing `tinyoffice-0.0.3/tinyoffice/__main__.py` & `tinyoffice-0.0.4/tinyoffice/__main__.py`

 * *Files identical despite different names*

### Comparing `tinyoffice-0.0.3/tinyoffice/tinyoffice.py` & `tinyoffice-0.0.4/tinyoffice/tinyoffice.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,19 +110,29 @@
         image_extensions = {
             ext for ext, func in registered_extensions.items()
             if func in Image.SAVE
             if func in Image.OPEN
         }
     with ProcessPoolExecutor() as executor:
         for root, dirs, files in os.walk(cwd):
+            if output in root:
+                continue
+            outpath_created = False
             for f in files:
                 if os.path.splitext(f)[1].lower() in types:
                     fpath = os.path.join(root, f)
-                    outpath = os.path.join(output, f)
+                    outpath = os.path.join(
+                        output, os.path.relpath(root, start=cwd), f
+                    )
                     if overwrite or not os.path.isfile(outpath):
+                        if not outpath_created:
+                            os.makedirs(
+                                os.path.dirname(outpath), exist_ok=True
+                            )
+                            outpath_created = True
                         future = executor.submit(
                             process,
                             fpath,
                             output=outpath,
                             convert=convert,
                             image_extensions=image_extensions,
                             jpeg_quality=jpeg_quality,
@@ -438,50 +448,51 @@
 
 def printer(future, verbosity=Verbosity.NORMAL):
     try:
         result = future.result()
     except Exception as e:
         print(e)
     else:
+        plural_errors = '' if len(result.errors) == 1 else 's'
         if verbosity is Verbosity.LOW:
             if result.num_images_compressed:
                 print(
-                    f'Compressed {result.filename}. '
-                    f'{len(result.errors):,} Error(s) encountered.'
+                    f'Compressed {result.filename!r}. '
+                    f'{len(result.errors):,} Error{plural_errors} encountered.'
                 )
         elif verbosity is Verbosity.NORMAL:
             if result.num_images_compressed:
                 print(
-                    f'Filename: {result.filename}.'
+                    f'Filename: {result.filename!r}.'
                     '\n'
                     f'Results: '
                     f'{result.num_images_compressed:,} compressed, '
                     f'{result.num_images_converted:,} converted, '
                     f'{result.num_images_skipped:,} skipped'
                     '\n'
                     f'Errors: {len(result.errors):,}'
                 )
             else:
                 print(
-                    f'No compressed images for {result.filename}. '
-                    f'{len(result.errors):,} Error(s) encountered.'
+                    f'No images compressed for {result.filename!r}. '
+                    f'{len(result.errors):,} Error{plural_errors} encountered.'
                 )
         elif verbosity is Verbosity.HIGH:
-            errors = "\n\t".join(result.errors) if result.errors else 'None!'
+            errors = ", ".join(result.errors) if result.errors else 'None!'
             print(
                 ''.join(
                     [
-                        f'Filename: {result.filename}.',
+                        f'Filename: {result.filename!r}.',
                         '\n',
                         'Results: ',
                         f'\n\t{result.num_images_compressed:,} compressed',
                         f'\n\t{result.num_images_converted:,} converted',
                         f'\n\t{result.num_images_skipped:,} skipped',
                         '\n',
-                        f'Errors: {errors}'
+                        f'Errors:\n\t{errors}'
                     ]
                 )
             )
 
 
 def totaler(output_record, future):
     try:
@@ -504,22 +515,27 @@
             output_record['images_converted'] += result.num_images_converted
             output_record['total_bytes'] += result.start_size
             output_record['total_bytes_compressed'] += result.compressed_size
             output_record['image_errors'].extend(result.errors)
 
 
 def print_total(record, verbosity):
-    if verbosity is not Verbosity.NONE:
-        print('\n\n')
+    print('\n\n')
+    plural_files = '' if len(record['compressed_files']) == 1 else 's'
+    plural_imgs = '' if record['images_compressed'] == 1 else 's'
+    plural_converted = '' if record['images_converted'] == 1 else 's'
+    plural_img_errs = '' if record['image_errors'] == 1 else 's'
+    plural_errs = '' if len(record['errors']) == 1 else 's'
     if verbosity is Verbosity.LOW:
         print(
             f'Compressed {len(record["compressed_files"]):,} '
-            f'document(s) with {len(record["image_errors"]):,} '
-            'image(s) that could not be converted and '
-            f'{len(record["errors"]):,} document(s) '
+            f'document{plural_files} with '
+            f'{len(record["image_errors"]):,} '
+            f'image{plural_img_errs} that could not be converted and '
+            f'{len(record["errors"]):,} document{plural_errs} '
             'that failed.'
         )
     elif verbosity is Verbosity.NORMAL:
         if record['total_bytes_compressed'] > 0:
             gb = 1024 * 1024 * 1024
             mb = 1024 * 1024
             kb = 1024
@@ -531,27 +547,30 @@
             elif total_cmp > kb:
                 savings = f'{total_cmp / kb:.2f} KB'
             else:
                 if total_cmp < 1:
                     total_cmp = '<1'
                 savings = f'{total_cmp} bytes'
             output = f'Compressed {len(record["compressed_files"]):,} '
-            output += 'document(s)\n'
-            output += f'\n{record["images_compressed"]:,} '
-            output += 'image(s) were '
+            output += f'document{plural_files}\n'
+            output += f'{record["images_compressed"]:,} '
+            output += f'image{plural_imgs} were '
             output += f'compressed for a savings of {savings}'
             output += '\n'
             if record['images_converted'] > 0:
                 output += f'{record["images_converted"]:,} '
-                output += 'image(s) were converted from TIFF to JPG\n'
+                output += f'image{plural_converted} were '
+                output += 'converted from TIFF to JPG\n'
             if record['image_errors']:
                 output += f'{len(record["image_errors"]):,} '
-                output += 'image(s) could not be converted or compressed\n'
+                output += f'image{plural_img_errs} could not be '
+                output += 'converted or compressed\n'
             if record['errors']:
-                output += f'{len(record["errors"]):,} document(s) '
+                output += f'{len(record["errors"]):,} '
+                output += f'document{plural_errs} '
                 output += 'could not be compressed due to error'
         else:
             output = 'No images were compressed'
         print(output)
     elif verbosity is Verbosity.HIGH:
         if record['total_bytes_compressed'] > 0:
             gb = 1024 * 1024 * 1024
@@ -565,26 +584,28 @@
             elif total_cmp > kb:
                 savings = f'{total_cmp / kb:.2f} KB'
             else:
                 if total_cmp < 1:
                     total_cmp = '<1'
                 savings = f'{total_cmp} bytes'
             output = f'Compressed {len(record["compressed_files"]):,} '
-            output += 'document(s):\n\t'
+            output += f'document{plural_files}:\n\t'
             output += '\n\t'.join(record['compressed_files'])
             output += f'\n{record["images_compressed"]:,} '
-            output += 'image(s) were '
+            output += f'image{plural_imgs} were '
             output += f'compressed for a savings of {savings}'
             output += '\n'
             if record['images_converted'] > 0:
                 output += f'{record["images_converted"]:,} '
-                output += 'image(s) were converted from TIFF to JPG\n'
+                output += f'image{plural_converted} were converted '
+                output += 'from TIFF to JPG\n'
             if record['image_errors']:
                 output += f'{len(record["image_errors"]):,} '
-                output += 'image(s) could not be converted or compressed\n'
+                output += f'image{plural_img_errs} could not be '
+                output += 'converted or compressed\n'
             if record['errors']:
                 output += 'ERRORS:\n\t'
                 output += '\n\t'.join(record["errors"])
             else:
                 output += 'No errors received!'
         else:
             output = 'No images were compressed'
```

### Comparing `tinyoffice-0.0.3/tinyoffice.egg-info/PKG-INFO` & `tinyoffice-0.0.4/tinyoffice.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyoffice
-Version: 0.0.3
+Version: 0.0.4
 Summary: Make your Office files tiny!
 Author-email: Samuel Woodward <sam@woodward.fyi>
 Project-URL: Homepage, https://github.com/PyWoody/tinyoffice
 Keywords: office,compress,convert,image,Word,Excel,Powerpoint
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

