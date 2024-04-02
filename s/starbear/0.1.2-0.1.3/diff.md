# Comparing `tmp/starbear-0.1.2.tar.gz` & `tmp/starbear-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starbear-0.1.2.tar", max compression
+gzip compressed data, was "starbear-0.1.3.tar", max compression
```

## Comparing `starbear-0.1.2.tar` & `starbear-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      804 2024-03-22 19:26:19.860706 starbear-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      314 2024-02-29 00:44:16.645421 starbear-0.1.2/starbear/__init__.py
--rw-r--r--   0        0        0      276 2023-12-18 19:59:00.300414 starbear-0.1.2/starbear/bearlib-template.html
--rw-r--r--   0        0        0    23797 2024-03-22 19:25:15.416712 starbear-0.1.2/starbear/bearlib.js
--rw-r--r--   0        0        0     1049 2024-02-02 19:46:01.148155 starbear-0.1.2/starbear/bearstyle.css
--rw-r--r--   0        0        0     2206 2024-02-29 00:50:48.026310 starbear-0.1.2/starbear/constructors.py
--rw-r--r--   0        0        0      322 2024-02-12 21:08:30.565978 starbear-0.1.2/starbear/page-template.html
--rw-r--r--   0        0        0    10202 2024-02-01 21:21:51.768382 starbear-0.1.2/starbear/page.py
--rw-r--r--   0        0        0     2264 2024-02-01 21:13:07.770061 starbear-0.1.2/starbear/ref.py
--rw-r--r--   0        0        0     7708 2024-02-01 21:14:06.522289 starbear-0.1.2/starbear/repr.py
--rw-r--r--   0        0        0    18401 2024-02-29 01:06:30.383219 starbear-0.1.2/starbear/serve.py
--rw-r--r--   0        0        0     4117 2024-01-19 16:02:41.325613 starbear-0.1.2/starbear/templating.py
--rw-r--r--   0        0        0     4819 2024-02-02 19:44:20.515869 starbear-0.1.2/starbear/utils.py
--rw-r--r--   0        0        0       18 2024-03-22 19:26:19.881235 starbear-0.1.2/starbear/version.py
--rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 starbear-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      804 2024-04-02 15:08:35.685190 starbear-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      314 2024-02-29 00:44:16.645421 starbear-0.1.3/starbear/__init__.py
+-rw-r--r--   0        0        0      276 2023-12-18 19:59:00.300414 starbear-0.1.3/starbear/bearlib-template.html
+-rw-r--r--   0        0        0    23868 2024-03-28 03:45:42.824944 starbear-0.1.3/starbear/bearlib.js
+-rw-r--r--   0        0        0     1049 2024-02-02 19:46:01.148155 starbear-0.1.3/starbear/bearstyle.css
+-rw-r--r--   0        0        0     2206 2024-02-29 00:50:48.026310 starbear-0.1.3/starbear/constructors.py
+-rw-r--r--   0        0        0      322 2024-02-12 21:08:30.565978 starbear-0.1.3/starbear/page-template.html
+-rw-r--r--   0        0        0    10202 2024-02-01 21:21:51.768382 starbear-0.1.3/starbear/page.py
+-rw-r--r--   0        0        0     2264 2024-02-01 21:13:07.770061 starbear-0.1.3/starbear/ref.py
+-rw-r--r--   0        0        0     7708 2024-02-01 21:14:06.522289 starbear-0.1.3/starbear/repr.py
+-rw-r--r--   0        0        0    18401 2024-02-29 01:06:30.383219 starbear-0.1.3/starbear/serve.py
+-rw-r--r--   0        0        0     4117 2024-01-19 16:02:41.325613 starbear-0.1.3/starbear/templating.py
+-rw-r--r--   0        0        0     4819 2024-02-02 19:44:20.515869 starbear-0.1.3/starbear/utils.py
+-rw-r--r--   0        0        0       18 2024-04-02 15:08:35.705934 starbear-0.1.3/starbear/version.py
+-rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 starbear-0.1.3/PKG-INFO
```

### Comparing `starbear-0.1.2/pyproject.toml` & `starbear-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "starbear"
-version = "0.1.2"
+version = "0.1.3"
 description = "Framework for easy small local web apps or programs"
 authors = ["Olivier Breuleux <breuleux@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 uvicorn = ">=0.17.6"
```

### Comparing `starbear-0.1.2/starbear/bearlib.js` & `starbear-0.1.3/starbear/bearlib.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -68,14 +68,16 @@
             for (let [k, v] of Object.entries(form)) {
                 let key = null;
                 if (isNaN(k)) {
                     key = k;
                 } else if (v.name) {
                     key = v.name;
                     v = form[key];
+                } else {
+                    continue;
                 }
                 let current = this.data;
                 let subkeys = key.split(".");
                 let zipped = subkeys.map((k, i) => [k, subkeys[i + 1]]);
                 let [lastkey, _] = zipped.pop();
                 for (let [subkey, nxt] of zipped) {
                     if (isNaN(nxt)) {
```

### Comparing `starbear-0.1.2/starbear/bearstyle.css` & `starbear-0.1.3/starbear/bearstyle.css`

 * *Files identical despite different names*

### Comparing `starbear-0.1.2/starbear/constructors.py` & `starbear-0.1.3/starbear/constructors.py`

 * *Files identical despite different names*

### Comparing `starbear-0.1.2/starbear/page.py` & `starbear-0.1.3/starbear/page.py`

 * *Files identical despite different names*

### Comparing `starbear-0.1.2/starbear/ref.py` & `starbear-0.1.3/starbear/ref.py`

 * *Files identical despite different names*

### Comparing `starbear-0.1.2/starbear/repr.py` & `starbear-0.1.3/starbear/repr.py`

 * *Files identical despite different names*

### Comparing `starbear-0.1.2/starbear/serve.py` & `starbear-0.1.3/starbear/serve.py`

 * *Files identical despite different names*

### Comparing `starbear-0.1.2/starbear/templating.py` & `starbear-0.1.3/starbear/templating.py`

 * *Files identical despite different names*

### Comparing `starbear-0.1.2/starbear/utils.py` & `starbear-0.1.3/starbear/utils.py`

 * *Files identical despite different names*

### Comparing `starbear-0.1.2/PKG-INFO` & `starbear-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starbear
-Version: 0.1.2
+Version: 0.1.3
 Summary: Framework for easy small local web apps or programs
 License: MIT
 Author: Olivier Breuleux
 Author-email: breuleux@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

