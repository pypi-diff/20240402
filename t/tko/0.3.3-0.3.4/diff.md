# Comparing `tmp/tko-0.3.3.tar.gz` & `tmp/tko-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tko-0.3.3.tar", last modified: Sat Mar 23 01:42:05 2024, max compression
+gzip compressed data, was "tko-0.3.4.tar", last modified: Tue Apr  2 11:34:04 2024, max compression
```

## Comparing `tko-0.3.3.tar` & `tko-0.3.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-03-23 01:42:05.939944 tko-0.3.3/
--rw-r--r--   0 lion      (1000) lion      (1000)     1043 2023-08-02 17:52:17.000000 tko-0.3.3/LICENSE
--rw-r--r--   0 lion      (1000) lion      (1000)      191 2023-08-02 17:33:10.000000 tko-0.3.3/MANIFEST.in
--rw-r--r--   0 lion      (1000) lion      (1000)     6765 2024-03-23 01:42:05.939944 tko-0.3.3/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)     5911 2024-03-23 01:30:54.000000 tko-0.3.3/Readme.md
--rw-r--r--   0 lion      (1000) lion      (1000)     2923 2024-03-22 23:28:19.000000 tko-0.3.3/changelog.md
--rw-r--r--   0 lion      (1000) lion      (1000)      298 2023-08-02 17:36:39.000000 tko-0.3.3/requirements.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-03-23 01:42:05.939944 tko-0.3.3/setup.cfg
--rw-r--r--   0 lion      (1000) lion      (1000)     3969 2024-03-23 01:41:44.000000 tko-0.3.3/setup.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-03-23 01:42:05.923277 tko-0.3.3/src/
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-03-23 01:42:05.933277 tko-0.3.3/src/tko/
--rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-03-22 22:07:27.000000 tko-0.3.3/src/tko/__init__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     9191 2024-03-20 21:10:58.000000 tko-0.3.3/src/tko/__main__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     4771 2024-03-22 23:27:23.000000 tko-0.3.3/src/tko/actions.py
--rw-r--r--   0 lion      (1000) lion      (1000)     4367 2024-03-20 21:10:58.000000 tko-0.3.3/src/tko/basic.py
--rw-r--r--   0 lion      (1000) lion      (1000)    10034 2023-10-19 13:10:37.000000 tko-0.3.3/src/tko/diff.py
--rw-r--r--   0 lion      (1000) lion      (1000)     7521 2024-03-21 14:49:39.000000 tko-0.3.3/src/tko/down.py
--rw-r--r--   0 lion      (1000) lion      (1000)     5166 2024-03-23 01:38:05.000000 tko-0.3.3/src/tko/filter.py
--rw-r--r--   0 lion      (1000) lion      (1000)     5747 2023-10-07 23:37:00.000000 tko-0.3.3/src/tko/format.py
--rw-r--r--   0 lion      (1000) lion      (1000)     2727 2024-03-13 17:39:00.000000 tko-0.3.3/src/tko/guide.py
--rw-r--r--   0 lion      (1000) lion      (1000)     8186 2024-03-22 22:49:12.000000 tko-0.3.3/src/tko/loader.py
--rw-r--r--   0 lion      (1000) lion      (1000)     2567 2023-08-03 03:39:13.000000 tko-0.3.3/src/tko/pattern.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1803 2023-10-19 18:36:35.000000 tko-0.3.3/src/tko/runner.py
--rw-r--r--   0 lion      (1000) lion      (1000)     5609 2024-03-20 21:47:04.000000 tko-0.3.3/src/tko/settings.py
--rw-r--r--   0 lion      (1000) lion      (1000)     4426 2024-03-22 11:32:02.000000 tko-0.3.3/src/tko/solver.py
--rw-r--r--   0 lion      (1000) lion      (1000)     7124 2024-03-22 22:37:53.000000 tko-0.3.3/src/tko/wdir.py
--rw-r--r--   0 lion      (1000) lion      (1000)     3177 2024-03-22 23:26:27.000000 tko-0.3.3/src/tko/writer.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-03-23 01:42:05.936610 tko-0.3.3/src/tko.egg-info/
--rw-r--r--   0 lion      (1000) lion      (1000)     6765 2024-03-23 01:42:05.000000 tko-0.3.3/src/tko.egg-info/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)      554 2024-03-23 01:42:05.000000 tko-0.3.3/src/tko.egg-info/SOURCES.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-03-23 01:42:05.000000 tko-0.3.3/src/tko.egg-info/dependency_links.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       47 2024-03-23 01:42:05.000000 tko-0.3.3/src/tko.egg-info/entry_points.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       59 2024-03-23 01:42:05.000000 tko-0.3.3/src/tko.egg-info/requires.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        4 2024-03-23 01:42:05.000000 tko-0.3.3/src/tko.egg-info/top_level.txt
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-02 11:34:04.686540 tko-0.3.4/
+-rw-r--r--   0 lion      (1000) lion      (1000)     1043 2023-08-02 17:52:17.000000 tko-0.3.4/LICENSE
+-rw-r--r--   0 lion      (1000) lion      (1000)      191 2023-08-02 17:33:10.000000 tko-0.3.4/MANIFEST.in
+-rw-r--r--   0 lion      (1000) lion      (1000)     6765 2024-04-02 11:34:04.686540 tko-0.3.4/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)     5911 2024-04-02 11:33:20.000000 tko-0.3.4/Readme.md
+-rw-r--r--   0 lion      (1000) lion      (1000)     2959 2024-04-02 11:33:20.000000 tko-0.3.4/changelog.md
+-rw-r--r--   0 lion      (1000) lion      (1000)      298 2023-08-02 17:36:39.000000 tko-0.3.4/requirements.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-04-02 11:34:04.689873 tko-0.3.4/setup.cfg
+-rw-r--r--   0 lion      (1000) lion      (1000)     3969 2024-04-02 11:33:20.000000 tko-0.3.4/setup.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-02 11:34:04.673206 tko-0.3.4/src/
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-02 11:34:04.683206 tko-0.3.4/src/tko/
+-rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-04-02 11:33:20.000000 tko-0.3.4/src/tko/__init__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     9191 2024-03-20 21:10:58.000000 tko-0.3.4/src/tko/__main__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     4771 2024-04-02 11:33:20.000000 tko-0.3.4/src/tko/actions.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     4367 2024-03-20 21:10:58.000000 tko-0.3.4/src/tko/basic.py
+-rw-r--r--   0 lion      (1000) lion      (1000)    10034 2023-10-19 13:10:37.000000 tko-0.3.4/src/tko/diff.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     7521 2024-03-21 14:49:39.000000 tko-0.3.4/src/tko/down.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     5166 2024-04-02 11:33:20.000000 tko-0.3.4/src/tko/filter.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     5747 2023-10-07 23:37:00.000000 tko-0.3.4/src/tko/format.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     2727 2024-03-13 17:39:00.000000 tko-0.3.4/src/tko/guide.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     8097 2024-04-02 11:33:20.000000 tko-0.3.4/src/tko/loader.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     2567 2023-08-03 03:39:13.000000 tko-0.3.4/src/tko/pattern.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     1803 2023-10-19 18:36:35.000000 tko-0.3.4/src/tko/runner.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     5609 2024-03-20 21:47:04.000000 tko-0.3.4/src/tko/settings.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     4426 2024-03-22 11:32:02.000000 tko-0.3.4/src/tko/solver.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     7124 2024-04-02 11:33:20.000000 tko-0.3.4/src/tko/wdir.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     3177 2024-04-02 11:33:20.000000 tko-0.3.4/src/tko/writer.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-02 11:34:04.686540 tko-0.3.4/src/tko.egg-info/
+-rw-r--r--   0 lion      (1000) lion      (1000)     6765 2024-04-02 11:34:04.000000 tko-0.3.4/src/tko.egg-info/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)      554 2024-04-02 11:34:04.000000 tko-0.3.4/src/tko.egg-info/SOURCES.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-04-02 11:34:04.000000 tko-0.3.4/src/tko.egg-info/dependency_links.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       47 2024-04-02 11:34:04.000000 tko-0.3.4/src/tko.egg-info/entry_points.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       59 2024-04-02 11:34:04.000000 tko-0.3.4/src/tko.egg-info/requires.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        4 2024-04-02 11:34:04.000000 tko-0.3.4/src/tko.egg-info/top_level.txt
```

### Comparing `tko-0.3.3/LICENSE` & `tko-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tko-0.3.3/PKG-INFO` & `tko-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tko
-Version: 0.3.3
+Version: 0.3.4
 Summary: tko: Test Kit Operations
 Home-page: https://github.com/senapk/tko
 Author: David Sena Oliveira
 Author-email: sena@ufc.br
 Project-URL: Bug Reports, https://github.com/senapk/tko/issues
 Project-URL: Source, https://github.com/senapk/tko/
 Keywords: programming,learning
```

### Comparing `tko-0.3.3/Readme.md` & `tko-0.3.4/Readme.md`

 * *Files identical despite different names*

### Comparing `tko-0.3.3/changelog.md` & `tko-0.3.4/changelog.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Changelog
 
+- 0.3.4:
+  - cio mode update parser
 - 0.3.3:
   - improved filter mode for fun
   - fixed bud in grade reduction show for build a .tio file
 - 0.3.2:
   - search for "public static void main" in multi file java solvers
   - search for file without "export" in multi file typescript solvers
 - 0.3.1:
```

### Comparing `tko-0.3.3/setup.py` & `tko-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.3/src/tko/__main__.py` & `tko-0.3.4/src/tko/__main__.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.3/src/tko/actions.py` & `tko-0.3.4/src/tko/actions.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.3/src/tko/basic.py` & `tko-0.3.4/src/tko/basic.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.3/src/tko/diff.py` & `tko-0.3.4/src/tko/diff.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.3/src/tko/down.py` & `tko-0.3.4/src/tko/down.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.3/src/tko/filter.py` & `tko-0.3.4/src/tko/filter.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.3/src/tko/format.py` & `tko-0.3.4/src/tko/format.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.3/src/tko/guide.py` & `tko-0.3.4/src/tko/guide.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.3/src/tko/loader.py` & `tko-0.3.4/src/tko/loader.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import annotations
-from typing import List, Tuple, Optional
+from typing import List, Tuple, Optional, Dict
 import re
 import os
 
 from .basic import Unit
 from .pattern import PatternLoader
 
 
@@ -101,58 +101,50 @@
         pass
 
     @staticmethod
     def parse_cio(text, source, crude_mode=False):
         unit_list = []
         text = "\n" + text
 
-        for test_case in text.split("\n#__case")[1:]:
-            unit = Unit()
-            unit.source = source
-            unit.output = test_case
-            unit_list.append(unit)
+        pattern = r'```.*?\n(.*?)```' # get only inside code blocks
+        code = re.findall(pattern, text, re.MULTILINE | re.DOTALL)
+        # join all code blocks found
+        text = "\n" + "\n".join(code)
+
+        pieces: List[Dict[str, List[str], List[str]]] = [] # header, input, output
+
+        open_case = False
+        for line in text.split("\n"):
+            if line.startswith("#__case") or line.startswith("#TEST_CASE"):
+                pieces.append({"header": line, "input": [], "output": []})
+                open_case = True
+            elif open_case:
+                pieces[-1]["output"].append(line)
+                if line.startswith("$end"):
+                    open_case = False
+
+        # concatenando testes contínuos e finalizando testes sem $end
+        for i in range(len(pieces)):
+            output = pieces[i]["output"]
+            if output[-1] != "$end" and i < len(pieces) - 1:
+                pieces[i + 1]["output"] = output + pieces[i + 1]["output"]
+                output.append("$end")
+
+        # removendo linhas vazias e criando input das linhas com $
+        for piece in pieces:
+            piece["input"]  = [line[1:] for line in piece["output"] if line.startswith("$")]
+            piece["output"] = [line for line in piece["output"] if line != "" and not line.startswith("#")]
+
+        for piece in pieces:
+            case = " ".join(piece["header"].split(" ")[1:])
+            input = "\n".join(piece["input"]) + "\n"
+            output = "\n".join(piece["output"])
+            unit_list.append(Unit(case, input, output, None, source))
 
         for unit in unit_list:
-            test = unit.output
-            if "\n$end" in test:
-                test = test.split("\n$end")[0] + "\n$end"
-
-            lines = test.split("\n")
-            tags = lines[0].strip().split(" ")
-            if tags[-1].endswith("%"):
-                unit.grade = int(tags[-1][0:-1])
-                del tags[-1]
-            else:
-                unit.grade = None
-            unit.case = " ".join(tags)
-            unit.output = "\n".join(lines[1:])
-
-        # concatenando testes contínuos
-        for i in range(len(unit_list)):
-            unit = unit_list[i]
-            if "\n$end" not in unit.output and (i < len(unit_list) - 1):
-                unit_list[i + 1].output = unit.output + '\n' + unit_list[i + 1].output
-                unit.output = unit.output + "\n$end\n"
-
-        for unit in unit_list:
-            lines = unit.output.split('\n')
-            unit.output = ""
-            unit.input = ""
-            # filtrando linhas vazias e comentários
-            for line in lines:
-                if crude_mode:  #
-                    unit.output += line + '\n'
-                    if line == "" or line.startswith("$") or line.startswith("#"):
-                        unit.input += line + '\n'
-                else:
-                    if line != "" and not line.startswith("#"):
-                        unit.output += line + '\n'
-                        if line.startswith("$"):
-                            unit.input += line[1:] + '\n'
-        for unit in unit_list:
             unit.fromCio = True
 
         return unit_list
 
     @staticmethod
     def parse_tio(text: str, source: str = "") -> List[Unit]:
```

### Comparing `tko-0.3.3/src/tko/pattern.py` & `tko-0.3.4/src/tko/pattern.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.3/src/tko/runner.py` & `tko-0.3.4/src/tko/runner.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.3/src/tko/settings.py` & `tko-0.3.4/src/tko/settings.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.3/src/tko/solver.py` & `tko-0.3.4/src/tko/solver.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.3/src/tko/wdir.py` & `tko-0.3.4/src/tko/wdir.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.3/src/tko/writer.py` & `tko-0.3.4/src/tko/writer.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.3/src/tko.egg-info/PKG-INFO` & `tko-0.3.4/src/tko.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tko
-Version: 0.3.3
+Version: 0.3.4
 Summary: tko: Test Kit Operations
 Home-page: https://github.com/senapk/tko
 Author: David Sena Oliveira
 Author-email: sena@ufc.br
 Project-URL: Bug Reports, https://github.com/senapk/tko/issues
 Project-URL: Source, https://github.com/senapk/tko/
 Keywords: programming,learning
```

### Comparing `tko-0.3.3/src/tko.egg-info/SOURCES.txt` & `tko-0.3.4/src/tko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

