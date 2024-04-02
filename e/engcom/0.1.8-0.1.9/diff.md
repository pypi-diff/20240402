# Comparing `tmp/engcom-0.1.8.tar.gz` & `tmp/engcom-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "engcom-0.1.8.tar", max compression
+gzip compressed data, was "engcom-0.1.9.tar", max compression
```

## Comparing `engcom-0.1.8.tar` & `engcom-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1083 2024-02-04 07:35:08.420431 engcom-0.1.8/LICENSE
--rw-r--r--   0        0        0      100 2024-02-04 07:35:08.420499 engcom-0.1.8/README.md
--rw-r--r--   0        0        0       46 2024-03-03 08:40:07.786163 engcom-0.1.8/engcom/__init__.py
--rw-r--r--   0        0        0     7498 2024-02-29 08:59:54.327790 engcom-0.1.8/engcom/data.py
--rw-r--r--   0        0        0    40584 2024-03-05 22:41:20.309322 engcom-0.1.8/engcom/filter.lua
--rw-r--r--   0        0        0      441 2024-03-01 08:14:12.068615 engcom-0.1.8/engcom/models.py
--rw-r--r--   0        0        0    18292 2024-02-05 09:24:31.701712 engcom-0.1.8/engcom/pandoc_reference.docx
--rw-r--r--   0        0        0     7282 2024-03-05 09:44:33.272576 engcom-0.1.8/engcom/publication.py
--rw-r--r--   0        0        0      999 2024-03-02 17:43:52.808428 engcom-0.1.8/engcom/publish.py
--rw-r--r--   0        0        0     1203 2024-03-05 09:35:57.944699 engcom-0.1.8/engcom/show.py
--rw-r--r--   0        0        0     6379 2024-03-03 09:12:01.708555 engcom-0.1.8/engcom/tufte.py
--rw-r--r--   0        0        0      622 2024-03-05 22:43:04.172444 engcom-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      977 1970-01-01 00:00:00.000000 engcom-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-02-04 07:35:08.420431 engcom-0.1.9/LICENSE
+-rw-r--r--   0        0        0      100 2024-02-04 07:35:08.420499 engcom-0.1.9/README.md
+-rw-r--r--   0        0        0       46 2024-03-03 08:40:07.786163 engcom-0.1.9/engcom/__init__.py
+-rw-r--r--   0        0        0     7498 2024-02-29 08:59:54.327790 engcom-0.1.9/engcom/data.py
+-rw-r--r--   0        0        0    40510 2024-03-06 00:27:03.781358 engcom-0.1.9/engcom/filter.lua
+-rw-r--r--   0        0        0      441 2024-03-01 08:14:12.068615 engcom-0.1.9/engcom/models.py
+-rw-r--r--   0        0        0    18292 2024-02-05 09:24:31.701712 engcom-0.1.9/engcom/pandoc_reference.docx
+-rw-r--r--   0        0        0     7282 2024-03-05 09:44:33.272576 engcom-0.1.9/engcom/publication.py
+-rw-r--r--   0        0        0      999 2024-03-02 17:43:52.808428 engcom-0.1.9/engcom/publish.py
+-rw-r--r--   0        0        0     1203 2024-03-05 09:35:57.944699 engcom-0.1.9/engcom/show.py
+-rw-r--r--   0        0        0     6379 2024-03-03 09:12:01.708555 engcom-0.1.9/engcom/tufte.py
+-rw-r--r--   0        0        0      622 2024-03-06 00:28:59.650860 engcom-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      977 1970-01-01 00:00:00.000000 engcom-0.1.9/PKG-INFO
```

### Comparing `engcom-0.1.8/LICENSE` & `engcom-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `engcom-0.1.8/engcom/data.py` & `engcom-0.1.9/engcom/data.py`

 * *Files identical despite different names*

### Comparing `engcom-0.1.8/engcom/filter.lua` & `engcom-0.1.9/engcom/filter.lua`

 * *Files 1% similar despite different names*

```diff
@@ -817,20 +817,16 @@
       width = ""
     else
       width = pandoc.utils.stringify(width)
       width = "width=" .. width
     end
     -- reset \graphicslist{}
     graphics_list_reset = "\\gdef\\graphicslist{}%\n"
-    -- see if standalone
-    if el.classes:includes('standalone') then
-      graphics_command = "\\noindent\\includestandalone["
-    else
-      graphics_command = "\\includegraphics["
-    end
+    -- graphics command
+    graphics_command = "\\begin{tikzpicture}%\n\\node[inner sep=0pt] {\\input{"..src.."}};%\n\\end{tikzpicture}%"
     -- get figcaption options
     figcaption_keys = {"color","format","credit","permission","reprint","territory","language","edition","fair","publicity","size","permissioncomment","layoutcomment"}
     options = "["
     i = 0
     for key, value in pairs(el.attr.attributes) do
       if has_value(figcaption_keys,key) then -- for markdown
         if i==0 then
@@ -864,15 +860,15 @@
         "\\centering\n"
       fig_end = "\\end{figure}\n"
       nofloat_text = "float"
     end
     -- construct latex figure
     fig_tex = graphics_list_reset ..
       fig_begin ..
-      graphics_command..width .."]{"..src.."}\n"..
+      graphics_command.."\n"..
       "\\caption{"..caption.."}\n"..
       "\\label{"..el.attr.identifier.."}\n".. 
       fig_end
     return pandoc.RawInline('latex', fig_tex)
   elseif FORMAT:match 'html' then
     -- deal with filename stuff
     local stripped = string.gsub(src,"common-rtcbook/",'')
```

### Comparing `engcom-0.1.8/engcom/pandoc_reference.docx` & `engcom-0.1.9/engcom/pandoc_reference.docx`

 * *Files identical despite different names*

### Comparing `engcom-0.1.8/engcom/publication.py` & `engcom-0.1.9/engcom/publication.py`

 * *Files identical despite different names*

### Comparing `engcom-0.1.8/engcom/publish.py` & `engcom-0.1.9/engcom/publish.py`

 * *Files identical despite different names*

### Comparing `engcom-0.1.8/engcom/show.py` & `engcom-0.1.9/engcom/show.py`

 * *Files identical despite different names*

### Comparing `engcom-0.1.8/engcom/tufte.py` & `engcom-0.1.9/engcom/tufte.py`

 * *Files identical despite different names*

### Comparing `engcom-0.1.8/pyproject.toml` & `engcom-0.1.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "engcom"
-version = "0.1.8"
+version = "0.1.9"
 description = "Miscellaneous tools for engineering computing"
 authors = ["Rico Picone <rpicone@stmartin.edu>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.11"
```

### Comparing `engcom-0.1.8/PKG-INFO` & `engcom-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: engcom
-Version: 0.1.8
+Version: 0.1.9
 Summary: Miscellaneous tools for engineering computing
 License: MIT
 Author: Rico Picone
 Author-email: rpicone@stmartin.edu
 Requires-Python: >=3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

