# Comparing `tmp/sc_file-3.0.4.tar.gz` & `tmp/sc_file-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sc_file-3.0.4.tar", max compression
+gzip compressed data, was "sc_file-3.0.5.tar", max compression
```

## Comparing `sc_file-3.0.4.tar` & `sc_file-3.0.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1083 2023-01-22 13:34:34.609366 sc_file-3.0.4/LICENSE
--rw-r--r--   0        0        0      607 2024-03-26 21:28:59.417991 sc_file-3.0.4/pyproject.toml
--rw-r--r--   0        0        0     4912 2024-03-26 21:28:59.416992 sc_file-3.0.4/README.md
--rw-r--r--   0        0        0      158 2024-03-20 03:27:16.310140 sc_file-3.0.4/scfile/__init__.py
--rw-r--r--   0        0        0     1485 2024-03-20 03:27:16.311141 sc_file-3.0.4/scfile/__main__.py
--rw-r--r--   0        0        0     1192 2024-03-20 03:27:16.311141 sc_file-3.0.4/scfile/consts.py
--rw-r--r--   0        0        0     1124 2024-03-20 03:27:16.312140 sc_file-3.0.4/scfile/enums.py
--rw-r--r--   0        0        0      427 2024-03-20 03:27:16.312140 sc_file-3.0.4/scfile/exceptions/__init__.py
--rw-r--r--   0        0        0       84 2024-03-20 03:27:16.312140 sc_file-3.0.4/scfile/exceptions/base.py
--rw-r--r--   0        0        0     1408 2024-03-20 03:27:16.313140 sc_file-3.0.4/scfile/exceptions/basic.py
--rw-r--r--   0        0        0      641 2024-03-20 03:27:16.313140 sc_file-3.0.4/scfile/exceptions/decode.py
--rw-r--r--   0        0        0     1409 2024-03-20 03:27:16.313140 sc_file-3.0.4/scfile/exceptions/mcsa.py
--rw-r--r--   0        0        0      866 2024-03-20 03:27:16.314140 sc_file-3.0.4/scfile/exceptions/ol.py
--rw-r--r--   0        0        0        2 2024-03-20 03:27:16.314140 sc_file-3.0.4/scfile/file/__init__.py
--rw-r--r--   0        0        0      780 2024-03-20 03:27:16.314140 sc_file-3.0.4/scfile/file/base.py
--rw-r--r--   0        0        0      394 2024-03-25 13:19:34.701976 sc_file-3.0.4/scfile/file/data.py
--rw-r--r--   0        0        0     2162 2024-03-20 03:27:16.315140 sc_file-3.0.4/scfile/file/dds/encoder.py
--rw-r--r--   0        0        0     1124 2024-03-20 03:27:16.315140 sc_file-3.0.4/scfile/file/dds/structure.py
--rw-r--r--   0        0        0     3185 2024-03-26 21:28:59.417991 sc_file-3.0.4/scfile/file/decoder.py
--rw-r--r--   0        0        0     1840 2024-03-26 21:28:59.418992 sc_file-3.0.4/scfile/file/encoder.py
--rw-r--r--   0        0        0     7319 2024-03-26 21:28:59.418992 sc_file-3.0.4/scfile/file/mcsa/decoder.py
--rw-r--r--   0        0        0      682 2024-03-26 21:28:59.419991 sc_file-3.0.4/scfile/file/mcsa/flags.py
--rw-r--r--   0        0        0      153 2024-03-20 03:27:16.317139 sc_file-3.0.4/scfile/file/mcsa/versions.py
--rw-r--r--   0        0        0      611 2024-03-20 03:27:16.317139 sc_file-3.0.4/scfile/file/mic/decoder.py
--rw-r--r--   0        0        0     2284 2024-03-26 21:28:59.419991 sc_file-3.0.4/scfile/file/obj/encoder.py
--rw-r--r--   0        0        0      694 2024-03-20 03:27:16.318139 sc_file-3.0.4/scfile/file/ol/converter/base.py
--rw-r--r--   0        0        0      189 2024-03-20 03:27:16.318139 sc_file-3.0.4/scfile/file/ol/converter/bgra8.py
--rw-r--r--   0        0        0      244 2024-03-20 03:27:16.318139 sc_file-3.0.4/scfile/file/ol/converter/rgba32f.py
--rw-r--r--   0        0        0     3864 2024-03-26 21:28:59.419991 sc_file-3.0.4/scfile/file/ol/decoder.py
--rw-r--r--   0        0        0      144 2024-03-20 03:27:16.319140 sc_file-3.0.4/scfile/file/ol/formats.py
--rw-r--r--   0        0        0      295 2024-03-20 03:27:16.319140 sc_file-3.0.4/scfile/file/png/encoder.py
--rw-r--r--   0        0        0        0 2024-03-20 03:27:16.319140 sc_file-3.0.4/scfile/io/__init__.py
--rw-r--r--   0        0        0     1568 2024-03-20 03:27:16.320140 sc_file-3.0.4/scfile/io/base.py
--rw-r--r--   0        0        0      261 2024-03-20 03:27:16.320140 sc_file-3.0.4/scfile/io/binary.py
--rw-r--r--   0        0        0      610 2024-03-20 03:27:16.320140 sc_file-3.0.4/scfile/io/mcsa.py
--rw-r--r--   0        0        0      405 2024-03-20 03:27:16.321141 sc_file-3.0.4/scfile/io/ol.py
--rw-r--r--   0        0        0      122 2024-03-26 21:28:59.420991 sc_file-3.0.4/scfile/types.py
--rw-r--r--   0        0        0     3341 2024-03-20 03:27:16.322141 sc_file-3.0.4/scfile/utils/convert.py
--rw-r--r--   0        0        0     3025 2024-03-26 21:28:59.420991 sc_file-3.0.4/scfile/utils/model.py
--rw-r--r--   0        0        0     5933 1970-01-01 00:00:00.000000 sc_file-3.0.4/setup.py
--rw-r--r--   0        0        0     5236 1970-01-01 00:00:00.000000 sc_file-3.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-01-22 13:34:34.609366 sc_file-3.0.5/LICENSE
+-rw-r--r--   0        0        0      607 2024-04-02 04:05:44.387714 sc_file-3.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5066 2024-04-02 04:05:44.387714 sc_file-3.0.5/README.md
+-rw-r--r--   0        0        0      158 2024-03-20 03:27:16.310140 sc_file-3.0.5/scfile/__init__.py
+-rw-r--r--   0        0        0     1485 2024-04-02 04:00:34.370200 sc_file-3.0.5/scfile/__main__.py
+-rw-r--r--   0        0        0     1192 2024-03-20 03:27:16.311141 sc_file-3.0.5/scfile/consts.py
+-rw-r--r--   0        0        0     1124 2024-03-20 03:27:16.312140 sc_file-3.0.5/scfile/enums.py
+-rw-r--r--   0        0        0      427 2024-03-20 03:27:16.312140 sc_file-3.0.5/scfile/exceptions/__init__.py
+-rw-r--r--   0        0        0       84 2024-03-20 03:27:16.312140 sc_file-3.0.5/scfile/exceptions/base.py
+-rw-r--r--   0        0        0     1408 2024-03-20 03:27:16.313140 sc_file-3.0.5/scfile/exceptions/basic.py
+-rw-r--r--   0        0        0      641 2024-03-20 03:27:16.313140 sc_file-3.0.5/scfile/exceptions/decode.py
+-rw-r--r--   0        0        0     1409 2024-03-20 03:27:16.313140 sc_file-3.0.5/scfile/exceptions/mcsa.py
+-rw-r--r--   0        0        0      866 2024-03-20 03:27:16.314140 sc_file-3.0.5/scfile/exceptions/ol.py
+-rw-r--r--   0        0        0        2 2024-03-20 03:27:16.314140 sc_file-3.0.5/scfile/file/__init__.py
+-rw-r--r--   0        0        0      780 2024-03-20 03:27:16.314140 sc_file-3.0.5/scfile/file/base.py
+-rw-r--r--   0        0        0      394 2024-03-25 13:19:34.701976 sc_file-3.0.5/scfile/file/data.py
+-rw-r--r--   0        0        0     2162 2024-03-20 03:27:16.315140 sc_file-3.0.5/scfile/file/dds/encoder.py
+-rw-r--r--   0        0        0     1124 2024-03-20 03:27:16.315140 sc_file-3.0.5/scfile/file/dds/structure.py
+-rw-r--r--   0        0        0     3185 2024-03-26 21:28:59.417991 sc_file-3.0.5/scfile/file/decoder.py
+-rw-r--r--   0        0        0     1840 2024-03-26 21:28:59.418992 sc_file-3.0.5/scfile/file/encoder.py
+-rw-r--r--   0        0        0     7329 2024-04-02 04:05:44.388714 sc_file-3.0.5/scfile/file/mcsa/decoder.py
+-rw-r--r--   0        0        0      682 2024-03-26 21:28:59.419991 sc_file-3.0.5/scfile/file/mcsa/flags.py
+-rw-r--r--   0        0        0      153 2024-03-20 03:27:16.317139 sc_file-3.0.5/scfile/file/mcsa/versions.py
+-rw-r--r--   0        0        0      611 2024-03-20 03:27:16.317139 sc_file-3.0.5/scfile/file/mic/decoder.py
+-rw-r--r--   0        0        0     2284 2024-03-26 21:28:59.419991 sc_file-3.0.5/scfile/file/obj/encoder.py
+-rw-r--r--   0        0        0      694 2024-03-20 03:27:16.318139 sc_file-3.0.5/scfile/file/ol/converter/base.py
+-rw-r--r--   0        0        0      189 2024-03-20 03:27:16.318139 sc_file-3.0.5/scfile/file/ol/converter/bgra8.py
+-rw-r--r--   0        0        0      244 2024-03-20 03:27:16.318139 sc_file-3.0.5/scfile/file/ol/converter/rgba32f.py
+-rw-r--r--   0        0        0     3864 2024-03-26 21:28:59.419991 sc_file-3.0.5/scfile/file/ol/decoder.py
+-rw-r--r--   0        0        0      144 2024-03-20 03:27:16.319140 sc_file-3.0.5/scfile/file/ol/formats.py
+-rw-r--r--   0        0        0      295 2024-03-20 03:27:16.319140 sc_file-3.0.5/scfile/file/png/encoder.py
+-rw-r--r--   0        0        0        0 2024-03-20 03:27:16.319140 sc_file-3.0.5/scfile/io/__init__.py
+-rw-r--r--   0        0        0     1568 2024-03-20 03:27:16.320140 sc_file-3.0.5/scfile/io/base.py
+-rw-r--r--   0        0        0      261 2024-03-20 03:27:16.320140 sc_file-3.0.5/scfile/io/binary.py
+-rw-r--r--   0        0        0      610 2024-03-20 03:27:16.320140 sc_file-3.0.5/scfile/io/mcsa.py
+-rw-r--r--   0        0        0      405 2024-03-20 03:27:16.321141 sc_file-3.0.5/scfile/io/ol.py
+-rw-r--r--   0        0        0      122 2024-03-26 21:28:59.420991 sc_file-3.0.5/scfile/types.py
+-rw-r--r--   0        0        0     3341 2024-03-20 03:27:16.322141 sc_file-3.0.5/scfile/utils/convert.py
+-rw-r--r--   0        0        0     3025 2024-04-01 08:54:55.823781 sc_file-3.0.5/scfile/utils/model.py
+-rw-r--r--   0        0        0     6089 1970-01-01 00:00:00.000000 sc_file-3.0.5/setup.py
+-rw-r--r--   0        0        0     5385 1970-01-01 00:00:00.000000 sc_file-3.0.5/PKG-INFO
```

### Comparing `sc_file-3.0.4/LICENSE` & `sc_file-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.4/pyproject.toml` & `sc_file-3.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sc-file"
-version = "3.0.4"
+version = "3.0.5"
 description = "Utility & Library for decoding stalcraft assets"
 authors = ["onejeuu <bloodtrail@beber1k.ru>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "scfile" }]
 
 [tool.poetry.dependencies]
```

### Comparing `sc_file-3.0.4/README.md` & `sc_file-3.0.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 # SC FILE
 
 Utility and Library for decoding and converting stalcraft assets files, such as models and textures into well-known formats.
 
 You can use executable from [Releases](https://github.com/onejeuu/sc-file/releases) page.
 
+> [!IMPORTANT]
+> This utility is designed for artworks and etc \
+> There is not and will not be any encoding back into game formats
+
 > [!WARNING]
-> Do not use game assets directly.
-> You can get banned for any changes in game client.
+> Do not use game assets directly \
+> You can get banned for any changes in game client
 
 # 📁 Formats
 
 | Type    | Source format | Output format |
 | ------- | ------------- | ------------- |
 | Model   | .mcsa         | .obj          |
 | Texture | .ol           | .dds          |
@@ -22,22 +26,23 @@
 
 Texture formats unsupported: Cubemaps (hdri, sky)
 
 # 💻 CLI Utility
 
 ## Usage
 
-You can drag and drop one or multiple files to `scfile.exe`.
-
 From bash:
 
 ```bash
-scfile [OPTIONS] [FILES]...
+scfile [FILES]... [OPTIONS]
 ```
 
+> [!TIP]
+> You can just drag and drop one or multiple files onto `scfile.exe`
+
 ## Arguments
 
 - `FILES`: **List of file paths to be converted**. Multiple files should be separated by **spaces**. Accepts both full and relative paths. **Does not accept directory**.
 
 ## Options
 
 - `-O`, `--output`: **One path to output file or directory**. Can be specified multiple times for different output files or directories. If not specified, file will be saved in the same directory with a new suffix. You can specify multiple `FILES` and a single `--output` directory.
@@ -197,15 +202,15 @@
         obj.save_as("model_1.obj")
         obj.save_as("model_2.obj")
 ```
 
 # 🛠️ Build
 
 > [!IMPORTANT]
-> You will need [poetry](https://python-poetry.org) to do compilation.
+> You will need [poetry](https://python-poetry.org) to do compilation
 
 > [!TIP]
 > Before proceeding, it's recommended to create virtual environment
 >
 > ```bash
 > poetry shell
 > ```
```

### Comparing `sc_file-3.0.4/scfile/__main__.py` & `sc_file-3.0.5/scfile/__main__.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.4/scfile/consts.py` & `sc_file-3.0.5/scfile/consts.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.4/scfile/enums.py` & `sc_file-3.0.5/scfile/enums.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.4/scfile/exceptions/basic.py` & `sc_file-3.0.5/scfile/exceptions/basic.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.4/scfile/exceptions/decode.py` & `sc_file-3.0.5/scfile/exceptions/decode.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.4/scfile/exceptions/mcsa.py` & `sc_file-3.0.5/scfile/exceptions/mcsa.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.4/scfile/exceptions/ol.py` & `sc_file-3.0.5/scfile/exceptions/ol.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.4/scfile/file/base.py` & `sc_file-3.0.5/scfile/file/base.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.4/scfile/file/dds/encoder.py` & `sc_file-3.0.5/scfile/file/dds/encoder.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.4/scfile/file/dds/structure.py` & `sc_file-3.0.5/scfile/file/dds/structure.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.4/scfile/file/decoder.py` & `sc_file-3.0.5/scfile/file/decoder.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.4/scfile/file/encoder.py` & `sc_file-3.0.5/scfile/file/encoder.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.4/scfile/file/mcsa/decoder.py` & `sc_file-3.0.5/scfile/file/mcsa/decoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,17 +73,17 @@
             self.model.scale.texture = self.f.readb(F.F32)
 
         # ! unconfirmed
         if self.flags[Flag.NORMALS] and self.version >= 10.0:
             self.model.scale.normals = self.f.readb(F.F32)
 
     def _parse_meshes(self):
-        meshes_count = self.f.readb(F.U32)
+        self.meshes_count = self.f.readb(F.U32)
 
-        for _ in range(meshes_count):
+        for _ in range(self.meshes_count):
             self._parse_mesh()
 
     def _parse_mesh(self):
         self.mesh = Mesh()
 
         # Name & Material
         self.mesh.name = self.f.reads().decode()
```

### Comparing `sc_file-3.0.4/scfile/file/mcsa/flags.py` & `sc_file-3.0.5/scfile/file/mcsa/flags.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.4/scfile/file/mic/decoder.py` & `sc_file-3.0.5/scfile/file/mic/decoder.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.4/scfile/file/obj/encoder.py` & `sc_file-3.0.5/scfile/file/obj/encoder.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.4/scfile/file/ol/converter/base.py` & `sc_file-3.0.5/scfile/file/ol/converter/base.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.4/scfile/file/ol/decoder.py` & `sc_file-3.0.5/scfile/file/ol/decoder.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.4/scfile/io/base.py` & `sc_file-3.0.5/scfile/io/base.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.4/scfile/io/mcsa.py` & `sc_file-3.0.5/scfile/io/mcsa.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.4/scfile/utils/convert.py` & `sc_file-3.0.5/scfile/utils/convert.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.4/scfile/utils/model.py` & `sc_file-3.0.5/scfile/utils/model.py`

 * *Files identical despite different names*

### Comparing `sc_file-3.0.4/setup.py` & `sc_file-3.0.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,17 +25,17 @@
  'quicktex>=0.2.0,<0.3.0']
 
 entry_points = \
 {'console_scripts': ['build = build:build']}
 
 setup_kwargs = {
     'name': 'sc-file',
-    'version': '3.0.4',
+    'version': '3.0.5',
     'description': 'Utility & Library for decoding stalcraft assets',
-    'long_description': '# SC FILE\n\nUtility and Library for decoding and converting stalcraft assets files, such as models and textures into well-known formats.\n\nYou can use executable from [Releases](https://github.com/onejeuu/sc-file/releases) page.\n\n> [!WARNING]\n> Do not use game assets directly.\n> You can get banned for any changes in game client.\n\n# 📁 Formats\n\n| Type    | Source format | Output format |\n| ------- | ------------- | ------------- |\n| Model   | .mcsa         | .obj          |\n| Texture | .ol           | .dds          |\n| Image   | .mic          | .png          |\n\nModel versions supported: 7.0, 8.0, 10.0\n\nTexture formats supported: DXT1, DXT3, DXT5, RGBA8, BGRA8, RGBA32F, DXN_XY\n\nTexture formats unsupported: Cubemaps (hdri, sky)\n\n# 💻 CLI Utility\n\n## Usage\n\nYou can drag and drop one or multiple files to `scfile.exe`.\n\nFrom bash:\n\n```bash\nscfile [OPTIONS] [FILES]...\n```\n\n## Arguments\n\n- `FILES`: **List of file paths to be converted**. Multiple files should be separated by **spaces**. Accepts both full and relative paths. **Does not accept directory**.\n\n## Options\n\n- `-O`, `--output`: **One path to output file or directory**. Can be specified multiple times for different output files or directories. If not specified, file will be saved in the same directory with a new suffix. You can specify multiple `FILES` and a single `--output` directory.\n\n## Examples\n\n1. Convert a single file:\n\n   ```bash\n   scfile file.mcsa\n   ```\n\n   _Will be saved in the same directory with a new suffix._\n\n1. Convert a single file with a specified path or name:\n\n   ```bash\n   scfile file.mcsa --output path/to/file.obj\n   ```\n\n1. Convert multiple files to a specified directory:\n\n   ```bash\n   scfile file1.mcsa file2.mcsa --output path/to/dir\n   ```\n\n1. Convert multiple files with explicitly specified output files:\n\n   ```bash\n   scfile file1.mcsa file2.mcsa -O 1.obj -O 2.obj\n   ```\n\n   _If the count of `FILES` and `--output` is different, as many files as possible will be converted._\n\n1. Convert all `.mcsa` files in the current directory:\n\n   ```bash\n   scfile *.mcsa\n   ```\n\n   _In this case, `--output` accepts only a directory. Subdirectories are not included._\n\n1. Convert all `.mcsa` files with subdirectories to a specified directory:\n\n   ```bash\n   scfile **/*.mcsa -O path/to/dir\n   ```\n\n   _In this case, `--output` accepts only a directory. With `--output` specified, directory structure is not duplicated._\n\n# 📚 Library\n\n## Install\n\n### Pip\n\n```bash\npip install sc-file -U\n```\n\n### Manual\n\n```bash\ngit clone git@github.com:onejeuu/sc-file.git\n```\n\n```bash\ncd sc-file\n```\n\n```bash\npoetry install\n```\n\n## Usage\n\n### Simple\n\n```python\nfrom scfile import convert\n\n# Output path is optional.\n# Defaults to source path with new suffix.\nconvert.mcsa_to_obj("path/to/model.mcsa", "path/to/model.obj")\nconvert.ol_to_dds("path/to/texture.ol", "path/to/texture.dds")\nconvert.mic_to_png("path/to/image.mic", "path/to/image.png")\n\n# Or determinate it automatically\nconvert.auto("path/to/model.mcsa")\n```\n\n### Advanced\n\nDefault\n\n```python\nfrom scfile.file.data import ModelData\nfrom scfile.file.mcsa.decoder import McsaDecoder\nfrom scfile.file.obj.encoder import ObjEncoder\n\nmcsa = McsaDecoder("model.mcsa")\ndata: ModelData = mcsa.decode()\nmcsa.close() # ? Necessary to close\n\nobj = ObjEncoder(data)\nobj.encode().save("model.obj") # ? Encoder closes after saving\n```\n\nUse encoding content bytes\n\n```python\nobj = ObjEncoder(data)\nobj.encode()\n\nwith open("model.obj", "wb") as fp:\n    fp.write(obj.content)\n\nobj.close() # ? Necessary to close\n```\n\nUse convert methods\n\n```python\nmcsa = McsaDecoder("model.mcsa")\nmcsa.convert_to(ObjEncoder).save("model.obj")\nmcsa.close() # ? Necessary to close\n```\n\n```python\nmcsa = McsaDecoder("model.mcsa")\nmcsa.to_obj().save("model.obj")\nmcsa.close() # ? Necessary to close\n```\n\nUse context manager\n\n```python\nwith McsaDecoder("model.mcsa") as mcsa:\n    data: ModelData = mcsa.decode()\n\nwith ObjEncoder(data) as obj:\n    obj.encode().save("model.obj")\n```\n\nUse context manager + convert methods\n\n```python\nwith McsaDecoder("model.mcsa") as mcsa:\n    mcsa.to_obj().save("model.obj")\n```\n\nSave multiple copies\n\n```python\nwith McsaDecoder("model.mcsa") as mcsa:\n    with mcsa.to_obj() as obj:\n        obj.save_as("model_1.obj")\n        obj.save_as("model_2.obj")\n```\n\n# 🛠️ Build\n\n> [!IMPORTANT]\n> You will need [poetry](https://python-poetry.org) to do compilation.\n\n> [!TIP]\n> Before proceeding, it\'s recommended to create virtual environment\n>\n> ```bash\n> poetry shell\n> ```\n\nThen install dependencies:\n\n```bash\npoetry install\n```\n\nAnd run script to compile:\n\n```bash\npoetry run build\n```\n\nExecutable file will be created in `/dist` directory.\n',
+    'long_description': '# SC FILE\n\nUtility and Library for decoding and converting stalcraft assets files, such as models and textures into well-known formats.\n\nYou can use executable from [Releases](https://github.com/onejeuu/sc-file/releases) page.\n\n> [!IMPORTANT]\n> This utility is designed for artworks and etc \\\n> There is not and will not be any encoding back into game formats\n\n> [!WARNING]\n> Do not use game assets directly \\\n> You can get banned for any changes in game client\n\n# 📁 Formats\n\n| Type    | Source format | Output format |\n| ------- | ------------- | ------------- |\n| Model   | .mcsa         | .obj          |\n| Texture | .ol           | .dds          |\n| Image   | .mic          | .png          |\n\nModel versions supported: 7.0, 8.0, 10.0\n\nTexture formats supported: DXT1, DXT3, DXT5, RGBA8, BGRA8, RGBA32F, DXN_XY\n\nTexture formats unsupported: Cubemaps (hdri, sky)\n\n# 💻 CLI Utility\n\n## Usage\n\nFrom bash:\n\n```bash\nscfile [FILES]... [OPTIONS]\n```\n\n> [!TIP]\n> You can just drag and drop one or multiple files onto `scfile.exe`\n\n## Arguments\n\n- `FILES`: **List of file paths to be converted**. Multiple files should be separated by **spaces**. Accepts both full and relative paths. **Does not accept directory**.\n\n## Options\n\n- `-O`, `--output`: **One path to output file or directory**. Can be specified multiple times for different output files or directories. If not specified, file will be saved in the same directory with a new suffix. You can specify multiple `FILES` and a single `--output` directory.\n\n## Examples\n\n1. Convert a single file:\n\n   ```bash\n   scfile file.mcsa\n   ```\n\n   _Will be saved in the same directory with a new suffix._\n\n1. Convert a single file with a specified path or name:\n\n   ```bash\n   scfile file.mcsa --output path/to/file.obj\n   ```\n\n1. Convert multiple files to a specified directory:\n\n   ```bash\n   scfile file1.mcsa file2.mcsa --output path/to/dir\n   ```\n\n1. Convert multiple files with explicitly specified output files:\n\n   ```bash\n   scfile file1.mcsa file2.mcsa -O 1.obj -O 2.obj\n   ```\n\n   _If the count of `FILES` and `--output` is different, as many files as possible will be converted._\n\n1. Convert all `.mcsa` files in the current directory:\n\n   ```bash\n   scfile *.mcsa\n   ```\n\n   _In this case, `--output` accepts only a directory. Subdirectories are not included._\n\n1. Convert all `.mcsa` files with subdirectories to a specified directory:\n\n   ```bash\n   scfile **/*.mcsa -O path/to/dir\n   ```\n\n   _In this case, `--output` accepts only a directory. With `--output` specified, directory structure is not duplicated._\n\n# 📚 Library\n\n## Install\n\n### Pip\n\n```bash\npip install sc-file -U\n```\n\n### Manual\n\n```bash\ngit clone git@github.com:onejeuu/sc-file.git\n```\n\n```bash\ncd sc-file\n```\n\n```bash\npoetry install\n```\n\n## Usage\n\n### Simple\n\n```python\nfrom scfile import convert\n\n# Output path is optional.\n# Defaults to source path with new suffix.\nconvert.mcsa_to_obj("path/to/model.mcsa", "path/to/model.obj")\nconvert.ol_to_dds("path/to/texture.ol", "path/to/texture.dds")\nconvert.mic_to_png("path/to/image.mic", "path/to/image.png")\n\n# Or determinate it automatically\nconvert.auto("path/to/model.mcsa")\n```\n\n### Advanced\n\nDefault\n\n```python\nfrom scfile.file.data import ModelData\nfrom scfile.file.mcsa.decoder import McsaDecoder\nfrom scfile.file.obj.encoder import ObjEncoder\n\nmcsa = McsaDecoder("model.mcsa")\ndata: ModelData = mcsa.decode()\nmcsa.close() # ? Necessary to close\n\nobj = ObjEncoder(data)\nobj.encode().save("model.obj") # ? Encoder closes after saving\n```\n\nUse encoding content bytes\n\n```python\nobj = ObjEncoder(data)\nobj.encode()\n\nwith open("model.obj", "wb") as fp:\n    fp.write(obj.content)\n\nobj.close() # ? Necessary to close\n```\n\nUse convert methods\n\n```python\nmcsa = McsaDecoder("model.mcsa")\nmcsa.convert_to(ObjEncoder).save("model.obj")\nmcsa.close() # ? Necessary to close\n```\n\n```python\nmcsa = McsaDecoder("model.mcsa")\nmcsa.to_obj().save("model.obj")\nmcsa.close() # ? Necessary to close\n```\n\nUse context manager\n\n```python\nwith McsaDecoder("model.mcsa") as mcsa:\n    data: ModelData = mcsa.decode()\n\nwith ObjEncoder(data) as obj:\n    obj.encode().save("model.obj")\n```\n\nUse context manager + convert methods\n\n```python\nwith McsaDecoder("model.mcsa") as mcsa:\n    mcsa.to_obj().save("model.obj")\n```\n\nSave multiple copies\n\n```python\nwith McsaDecoder("model.mcsa") as mcsa:\n    with mcsa.to_obj() as obj:\n        obj.save_as("model_1.obj")\n        obj.save_as("model_2.obj")\n```\n\n# 🛠️ Build\n\n> [!IMPORTANT]\n> You will need [poetry](https://python-poetry.org) to do compilation\n\n> [!TIP]\n> Before proceeding, it\'s recommended to create virtual environment\n>\n> ```bash\n> poetry shell\n> ```\n\nThen install dependencies:\n\n```bash\npoetry install\n```\n\nAnd run script to compile:\n\n```bash\npoetry run build\n```\n\nExecutable file will be created in `/dist` directory.\n',
     'author': 'onejeuu',
     'author_email': 'bloodtrail@beber1k.ru',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `sc_file-3.0.4/PKG-INFO` & `sc_file-3.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sc-file
-Version: 3.0.4
+Version: 3.0.5
 Summary: Utility & Library for decoding stalcraft assets
 License: MIT
 Author: onejeuu
 Author-email: bloodtrail@beber1k.ru
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -17,17 +17,21 @@
 
 # SC FILE
 
 Utility and Library for decoding and converting stalcraft assets files, such as models and textures into well-known formats.
 
 You can use executable from [Releases](https://github.com/onejeuu/sc-file/releases) page.
 
+> [!IMPORTANT]
+> This utility is designed for artworks and etc \
+> There is not and will not be any encoding back into game formats
+
 > [!WARNING]
-> Do not use game assets directly.
-> You can get banned for any changes in game client.
+> Do not use game assets directly \
+> You can get banned for any changes in game client
 
 # 📁 Formats
 
 | Type    | Source format | Output format |
 | ------- | ------------- | ------------- |
 | Model   | .mcsa         | .obj          |
 | Texture | .ol           | .dds          |
@@ -39,22 +43,23 @@
 
 Texture formats unsupported: Cubemaps (hdri, sky)
 
 # 💻 CLI Utility
 
 ## Usage
 
-You can drag and drop one or multiple files to `scfile.exe`.
-
 From bash:
 
 ```bash
-scfile [OPTIONS] [FILES]...
+scfile [FILES]... [OPTIONS]
 ```
 
+> [!TIP]
+> You can just drag and drop one or multiple files onto `scfile.exe`
+
 ## Arguments
 
 - `FILES`: **List of file paths to be converted**. Multiple files should be separated by **spaces**. Accepts both full and relative paths. **Does not accept directory**.
 
 ## Options
 
 - `-O`, `--output`: **One path to output file or directory**. Can be specified multiple times for different output files or directories. If not specified, file will be saved in the same directory with a new suffix. You can specify multiple `FILES` and a single `--output` directory.
@@ -214,15 +219,15 @@
         obj.save_as("model_1.obj")
         obj.save_as("model_2.obj")
 ```
 
 # 🛠️ Build
 
 > [!IMPORTANT]
-> You will need [poetry](https://python-poetry.org) to do compilation.
+> You will need [poetry](https://python-poetry.org) to do compilation
 
 > [!TIP]
 > Before proceeding, it's recommended to create virtual environment
 >
 > ```bash
 > poetry shell
 > ```
```

