# Comparing `tmp/tempren-1.0.0.tar.gz` & `tmp/tempren-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tempren-1.0.0.tar", max compression
+gzip compressed data, was "tempren-1.0.1.tar", max compression
```

## Comparing `tempren-1.0.0.tar` & `tempren-1.0.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    32473 2023-10-23 19:29:34.440568 tempren-1.0.0/LICENSE
--rw-r--r--   0        0        0     5282 2023-10-23 19:29:34.440568 tempren-1.0.0/README.md
--rw-r--r--   0        0        0     1801 2023-10-23 19:29:34.440568 tempren-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-10-23 19:29:34.440568 tempren-1.0.0/tempren/__init__.py
--rw-r--r--   0        0        0     3807 2023-10-23 19:29:34.440568 tempren-1.0.0/tempren/adhoc.py
--rw-r--r--   0        0        0     2797 2023-10-23 19:29:34.440568 tempren-1.0.0/tempren/alias.py
--rwxr-xr-x   0        0        0    22434 2023-10-23 19:29:34.440568 tempren-1.0.0/tempren/cli.py
--rw-r--r--   0        0        0     2518 2023-10-23 19:29:34.440568 tempren-1.0.0/tempren/discovery.py
--rw-r--r--   0        0        0      431 2023-10-23 19:29:34.440568 tempren-1.0.0/tempren/evaluation.py
--rw-r--r--   0        0        0      995 2023-10-23 19:29:34.440568 tempren-1.0.0/tempren/exceptions.py
--rw-r--r--   0        0        0     3067 2023-10-23 19:29:34.440568 tempren-1.0.0/tempren/factories.py
--rw-r--r--   0        0        0     3207 2023-10-23 19:29:34.440568 tempren-1.0.0/tempren/file_filters.py
--rw-r--r--   0        0        0     1689 2023-10-23 19:29:34.440568 tempren-1.0.0/tempren/file_sorters.py
--rw-r--r--   0        0        0     6573 2023-10-23 19:29:34.440568 tempren-1.0.0/tempren/filesystem.py
--rw-r--r--   0        0        0    13693 2023-10-23 19:29:34.440568 tempren-1.0.0/tempren/pipeline.py
--rw-r--r--   0        0        0     4239 2023-10-23 19:29:34.444568 tempren-1.0.0/tempren/primitives.py
--rw-r--r--   0        0        0        0 2023-10-23 19:29:34.444568 tempren-1.0.0/tempren/tags/__init__.py
--rw-r--r--   0        0        0     3017 2023-10-23 19:29:34.444568 tempren-1.0.0/tempren/tags/audio.py
--rw-r--r--   0        0        0    14814 2023-10-23 19:29:34.444568 tempren-1.0.0/tempren/tags/core.py
--rw-r--r--   0        0        0     1245 2023-10-23 19:29:34.444568 tempren-1.0.0/tempren/tags/filesystem.py
--rw-r--r--   0        0        0     2975 2023-10-23 19:29:34.444568 tempren-1.0.0/tempren/tags/gpx.py
--rw-r--r--   0        0        0     1835 2023-10-23 19:29:34.444568 tempren-1.0.0/tempren/tags/hash.py
--rw-r--r--   0        0        0     5806 2023-10-23 19:29:34.444568 tempren-1.0.0/tempren/tags/image.py
--rw-r--r--   0        0        0     6539 2023-10-23 19:29:34.444568 tempren-1.0.0/tempren/tags/text.py
--rw-r--r--   0        0        0     3055 2023-10-23 19:29:34.444568 tempren-1.0.0/tempren/tags/video.py
--rw-r--r--   0        0        0        0 2023-10-23 19:29:34.444568 tempren-1.0.0/tempren/template/__init__.py
--rw-r--r--   0        0        0     3143 2023-10-23 19:29:34.444568 tempren-1.0.0/tempren/template/ast.py
--rw-r--r--   0        0        0     3682 2023-10-23 19:29:34.444568 tempren-1.0.0/tempren/template/compiler.py
--rw-r--r--   0        0        0     1182 2023-10-23 19:29:34.444568 tempren-1.0.0/tempren/template/exceptions.py
--rw-r--r--   0        0        0     1202 2023-10-23 19:29:34.444568 tempren-1.0.0/tempren/template/generators.py
--rw-r--r--   0        0        0     1064 2023-10-23 19:29:34.444568 tempren-1.0.0/tempren/template/grammar/TagTemplateLexer.g4
--rw-r--r--   0        0        0     6080 2023-10-23 19:29:34.444568 tempren-1.0.0/tempren/template/grammar/TagTemplateLexer.interp
--rw-r--r--   0        0        0    20134 2023-10-23 19:29:34.444568 tempren-1.0.0/tempren/template/grammar/TagTemplateLexer.py
--rw-r--r--   0        0        0      326 2023-10-23 19:29:34.444568 tempren-1.0.0/tempren/template/grammar/TagTemplateLexer.tokens
--rw-r--r--   0        0        0     1184 2023-10-23 19:29:34.444568 tempren-1.0.0/tempren/template/grammar/TagTemplateParser.g4
--rw-r--r--   0        0        0     4296 2023-10-23 19:29:34.444568 tempren-1.0.0/tempren/template/grammar/TagTemplateParser.interp
--rw-r--r--   0        0        0    38985 2023-10-23 19:29:34.444568 tempren-1.0.0/tempren/template/grammar/TagTemplateParser.py
--rw-r--r--   0        0        0      326 2023-10-23 19:29:34.444568 tempren-1.0.0/tempren/template/grammar/TagTemplateParser.tokens
--rw-r--r--   0        0        0     1786 2023-10-23 19:29:34.444568 tempren-1.0.0/tempren/template/grammar/TagTemplateParserVisitor.py
--rw-r--r--   0        0        0        0 2023-10-23 19:29:34.444568 tempren-1.0.0/tempren/template/grammar/__init__.py
--rwxr-xr-x   0        0        0      261 2023-10-23 19:29:34.444568 tempren-1.0.0/tempren/template/grammar/generate.sh
--rwxr-xr-x   0        0        0      266 2023-10-23 19:29:34.444568 tempren-1.0.0/tempren/template/grammar/generate_for_grun.sh
--rw-r--r--   0        0        0     8213 2023-10-23 19:29:34.444568 tempren-1.0.0/tempren/template/parser.py
--rw-r--r--   0        0        0     6740 2023-10-23 19:29:34.444568 tempren-1.0.0/tempren/template/registry.py
--rw-r--r--   0        0        0     6920 1970-01-01 00:00:00.000000 tempren-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    32473 2024-04-02 18:39:02.617130 tempren-1.0.1/LICENSE
+-rw-r--r--   0        0        0     5282 2024-04-02 18:39:02.617130 tempren-1.0.1/README.md
+-rw-r--r--   0        0        0     1799 2024-04-02 18:39:02.617130 tempren-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/__init__.py
+-rw-r--r--   0        0        0     3807 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/adhoc.py
+-rw-r--r--   0        0        0     2797 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/alias.py
+-rwxr-xr-x   0        0        0    22434 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/cli.py
+-rw-r--r--   0        0        0     2518 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/discovery.py
+-rw-r--r--   0        0        0      431 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/evaluation.py
+-rw-r--r--   0        0        0      995 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/exceptions.py
+-rw-r--r--   0        0        0     3067 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/factories.py
+-rw-r--r--   0        0        0     3207 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/file_filters.py
+-rw-r--r--   0        0        0     1689 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/file_sorters.py
+-rw-r--r--   0        0        0     6573 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/filesystem.py
+-rw-r--r--   0        0        0    13693 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/pipeline.py
+-rw-r--r--   0        0        0     4239 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/primitives.py
+-rw-r--r--   0        0        0        0 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/tags/__init__.py
+-rw-r--r--   0        0        0     3017 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/tags/audio.py
+-rw-r--r--   0        0        0    14814 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/tags/core.py
+-rw-r--r--   0        0        0     1245 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/tags/filesystem.py
+-rw-r--r--   0        0        0     2975 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/tags/gpx.py
+-rw-r--r--   0        0        0     1835 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/tags/hash.py
+-rw-r--r--   0        0        0     5816 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/tags/image.py
+-rw-r--r--   0        0        0     6539 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/tags/text.py
+-rw-r--r--   0        0        0     3055 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/tags/video.py
+-rw-r--r--   0        0        0        0 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/__init__.py
+-rw-r--r--   0        0        0     3143 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/ast.py
+-rw-r--r--   0        0        0     3682 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/compiler.py
+-rw-r--r--   0        0        0     1182 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/exceptions.py
+-rw-r--r--   0        0        0     1202 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/generators.py
+-rw-r--r--   0        0        0     1064 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/grammar/TagTemplateLexer.g4
+-rw-r--r--   0        0        0     6080 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/grammar/TagTemplateLexer.interp
+-rw-r--r--   0        0        0    20134 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/grammar/TagTemplateLexer.py
+-rw-r--r--   0        0        0      326 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/grammar/TagTemplateLexer.tokens
+-rw-r--r--   0        0        0     1184 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/grammar/TagTemplateParser.g4
+-rw-r--r--   0        0        0     4296 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/grammar/TagTemplateParser.interp
+-rw-r--r--   0        0        0    38985 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/grammar/TagTemplateParser.py
+-rw-r--r--   0        0        0      326 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/grammar/TagTemplateParser.tokens
+-rw-r--r--   0        0        0     1786 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/grammar/TagTemplateParserVisitor.py
+-rw-r--r--   0        0        0        0 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/grammar/__init__.py
+-rwxr-xr-x   0        0        0      261 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/grammar/generate.sh
+-rwxr-xr-x   0        0        0      266 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/grammar/generate_for_grun.sh
+-rw-r--r--   0        0        0     8213 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/parser.py
+-rw-r--r--   0        0        0     6740 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/registry.py
+-rw-r--r--   0        0        0     6971 1970-01-01 00:00:00.000000 tempren-1.0.1/PKG-INFO
```

### Comparing `tempren-1.0.0/LICENSE` & `tempren-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tempren-1.0.0/README.md` & `tempren-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `tempren-1.0.0/pyproject.toml` & `tempren-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tempren"
-version = "1.0.0"
+version = "1.0.1"
 description = "Template-based renaming utility"
 readme = "README.md"
 license = "GPL-3.0-or-later"
 authors = ["Paweł Żukowski <p.z.idlecode@gmail.com>"]
 homepage = "https://github.com/idle-code/tempren"
 keywords = ["batch-renaming", "cli", "filename"]
 classifiers = [
@@ -33,18 +33,18 @@
 piexif = "^1.1.3"
 pymediainfo = {version = "^6.0.1", optional = true}
 isodate = "^0.6.1"
 gpxpy = "1.5.0"
 Pint = "^0.21.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.4.0"
+pytest = "^7.4.4"
 pytest-cov = "^4.1"
 coverage = "^7.2.7"
-pre-commit = "^3.3.3"
+pre-commit = "^3.5"
 mypy = "^1.4.1"
 pylint = "^3.0.2"
 
 [tool.poetry.extras]
 video = ["pymediainfo"]
 
 [tool.poetry.scripts]
```

### Comparing `tempren-1.0.0/tempren/adhoc.py` & `tempren-1.0.1/tempren/adhoc.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.0/tempren/alias.py` & `tempren-1.0.1/tempren/alias.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.0/tempren/cli.py` & `tempren-1.0.1/tempren/cli.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.0/tempren/discovery.py` & `tempren-1.0.1/tempren/discovery.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.0/tempren/exceptions.py` & `tempren-1.0.1/tempren/exceptions.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.0/tempren/factories.py` & `tempren-1.0.1/tempren/factories.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.0/tempren/file_filters.py` & `tempren-1.0.1/tempren/file_filters.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.0/tempren/file_sorters.py` & `tempren-1.0.1/tempren/file_sorters.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.0/tempren/filesystem.py` & `tempren-1.0.1/tempren/filesystem.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.0/tempren/pipeline.py` & `tempren-1.0.1/tempren/pipeline.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.0/tempren/primitives.py` & `tempren-1.0.1/tempren/primitives.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.0/tempren/tags/audio.py` & `tempren-1.0.1/tempren/tags/audio.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.0/tempren/tags/core.py` & `tempren-1.0.1/tempren/tags/core.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.0/tempren/tags/filesystem.py` & `tempren-1.0.1/tempren/tags/filesystem.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.0/tempren/tags/gpx.py` & `tempren-1.0.1/tempren/tags/gpx.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.0/tempren/tags/hash.py` & `tempren-1.0.1/tempren/tags/hash.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.0/tempren/tags/image.py` & `tempren-1.0.1/tempren/tags/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 from fractions import Fraction
 from typing import Any, Iterator, Optional, Tuple
 
 import piexif
 import PIL
 from piexif import TAGS
 from piexif import TYPES as TAG_TYPES
-from PIL import Image
+from PIL.Image import Image
 
 from tempren.alias import TagAlias
 from tempren.exceptions import FileNotSupportedError, MissingMetadataError
 from tempren.primitives import File, Tag
 
 
 class PillowTagBase(Tag, ABC):
     """Base for tags extracting metadata from images using Pillow library"""
 
     require_context = False
 
     def process(self, file: File, context: Optional[str]) -> Any:
         try:
-            with Image.open(file.absolute_path) as img:
+            with PIL.Image.open(file.absolute_path) as img:
                 return self.extract_metadata(img)
         except PIL.UnidentifiedImageError:
             raise FileNotSupportedError()
 
     @abstractmethod
     def extract_metadata(self, image: Image) -> Any:
         raise NotImplementedError()
```

### Comparing `tempren-1.0.0/tempren/tags/text.py` & `tempren-1.0.1/tempren/tags/text.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.0/tempren/tags/video.py` & `tempren-1.0.1/tempren/tags/video.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.0/tempren/template/ast.py` & `tempren-1.0.1/tempren/template/ast.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.0/tempren/template/compiler.py` & `tempren-1.0.1/tempren/template/compiler.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.0/tempren/template/exceptions.py` & `tempren-1.0.1/tempren/template/exceptions.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.0/tempren/template/generators.py` & `tempren-1.0.1/tempren/template/generators.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.0/tempren/template/grammar/TagTemplateLexer.g4` & `tempren-1.0.1/tempren/template/grammar/TagTemplateLexer.g4`

 * *Files identical despite different names*

### Comparing `tempren-1.0.0/tempren/template/grammar/TagTemplateLexer.interp` & `tempren-1.0.1/tempren/template/grammar/TagTemplateLexer.interp`

 * *Files identical despite different names*

### Comparing `tempren-1.0.0/tempren/template/grammar/TagTemplateLexer.py` & `tempren-1.0.1/tempren/template/grammar/TagTemplateLexer.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.0/tempren/template/grammar/TagTemplateParser.g4` & `tempren-1.0.1/tempren/template/grammar/TagTemplateParser.g4`

 * *Files identical despite different names*

### Comparing `tempren-1.0.0/tempren/template/grammar/TagTemplateParser.interp` & `tempren-1.0.1/tempren/template/grammar/TagTemplateParser.interp`

 * *Files identical despite different names*

### Comparing `tempren-1.0.0/tempren/template/grammar/TagTemplateParser.py` & `tempren-1.0.1/tempren/template/grammar/TagTemplateParser.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.0/tempren/template/grammar/TagTemplateParserVisitor.py` & `tempren-1.0.1/tempren/template/grammar/TagTemplateParserVisitor.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.0/tempren/template/parser.py` & `tempren-1.0.1/tempren/template/parser.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.0/tempren/template/registry.py` & `tempren-1.0.1/tempren/template/registry.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.0/PKG-INFO` & `tempren-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tempren
-Version: 1.0.0
+Version: 1.0.1
 Summary: Template-based renaming utility
 Home-page: https://github.com/idle-code/tempren
 License: GPL-3.0-or-later
 Keywords: batch-renaming,cli,filename
 Author: Paweł Żukowski
 Author-email: p.z.idlecode@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -18,14 +18,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Filesystems
 Classifier: Topic :: Utilities
 Provides-Extra: video
 Requires-Dist: Pillow (>=10.0.0,<11.0.0)
 Requires-Dist: Pint (>=0.21.0,<0.22.0)
 Requires-Dist: Unidecode (>=1.3.6,<2.0.0)
 Requires-Dist: antlr4-python3-runtime (==4.13.1)
```

