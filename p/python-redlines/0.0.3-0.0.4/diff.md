# Comparing `tmp/python_redlines-0.0.3.tar.gz` & `tmp/python_redlines-0.0.4.tar.gz`

## Comparing `python_redlines-0.0.3.tar` & `python_redlines-0.0.4.tar`

### file list

```diff
@@ -1,29 +1,5 @@
--rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 python_redlines-0.0.3/build_differ.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 python_redlines-0.0.3/extract_version.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 python_redlines-0.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 python_redlines-0.0.3/.idea/.gitignore
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 python_redlines-0.0.3/.idea/misc.xml
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 python_redlines-0.0.3/.idea/modules.xml
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 python_redlines-0.0.3/.idea/python-redlines.iml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 python_redlines-0.0.3/.idea/vcs.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 python_redlines-0.0.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 python_redlines-0.0.3/csproj/Program.cs
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 python_redlines-0.0.3/csproj/redlines.csproj
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 python_redlines-0.0.3/csproj/redlines.sln
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 python_redlines-0.0.3/docs/developer-guide.md
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 python_redlines-0.0.3/docs/quickstart.md
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 python_redlines-0.0.3/src/python_redlines/__about__.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 python_redlines-0.0.3/src/python_redlines/__init__.py
--rw-r--r--   0        0        0     4635 2020-02-02 00:00:00.000000 python_redlines-0.0.3/src/python_redlines/engines.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 python_redlines-0.0.3/src/python_redlines/bin/.gitignore
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 python_redlines-0.0.3/src/python_redlines/dist/.gitignore
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 python_redlines-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 python_redlines-0.0.3/tests/test_openxml_differ.py
--rw-r--r--   0        0        0    13779 2020-02-02 00:00:00.000000 python_redlines-0.0.3/tests/fixtures/expected_redline.docx
--rw-r--r--   0        0        0    14715 2020-02-02 00:00:00.000000 python_redlines-0.0.3/tests/fixtures/modified.docx
--rw-r--r--   0        0        0    13357 2020-02-02 00:00:00.000000 python_redlines-0.0.3/tests/fixtures/original.docx
--rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 python_redlines-0.0.3/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 python_redlines-0.0.3/LICENSE.md
--rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 python_redlines-0.0.3/README.md
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 python_redlines-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     8850 2020-02-02 00:00:00.000000 python_redlines-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 python_redlines-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 python_redlines-0.0.4/LICENSE.md
+-rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 python_redlines-0.0.4/README.md
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 python_redlines-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     8850 2020-02-02 00:00:00.000000 python_redlines-0.0.4/PKG-INFO
```

### Comparing `python_redlines-0.0.3/.gitignore` & `python_redlines-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `python_redlines-0.0.3/LICENSE.md` & `python_redlines-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `python_redlines-0.0.3/README.md` & `python_redlines-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `python_redlines-0.0.3/pyproject.toml` & `python_redlines-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,23 @@
 "dist" = "python_redlines/dist"
 
 [tool.hatch.build.targets.wheel]
 artifacts = [
   "*.zip",
   "*.tar.gz",
 ]
+[tool.hatch.build.targets.sdist]
+include = [
+  "python_redlines/dist",
+  "python_redlines/bin",
+]
+
+# Build hook to build the binaries for distribution...
+[tool.hatch.build.hooks.custom]
+path = "hatch_run_build_hook.py"
 
 [project]
 name = "python-redlines"
 dynamic = ["version"]
 description = ''
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `python_redlines-0.0.3/PKG-INFO` & `python_redlines-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: python-redlines
-Version: 0.0.3
+Version: 0.0.4
 Project-URL: Documentation, https://github.com/unknown/python-redlines#readme
 Project-URL: Issues, https://github.com/unknown/python-redlines/issues
 Project-URL: Source, https://github.com/unknown/python-redlines
 Author: John Scrudato IV
 License-Expression: MIT
 License-File: LICENSE.md
 Classifier: Development Status :: 4 - Beta
```

