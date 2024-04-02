# Comparing `tmp/llsd-1.2.3.tar.gz` & `tmp/llsd-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llsd-1.2.3.tar", last modified: Thu Sep  7 20:22:47 2023, max compression
+gzip compressed data, was "llsd-1.2.4.tar", last modified: Tue Apr  2 06:37:48 2024, max compression
```

## Comparing `llsd-1.2.3.tar` & `llsd-1.2.4.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-07 20:22:47.732035 llsd-1.2.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-07 20:22:47.728035 llsd-1.2.3/.github/
--rw-r--r--   0 root         (0) root         (0)      114 2023-09-07 20:21:37.000000 llsd-1.2.3/.github/dependabot.yaml
--rw-r--r--   0 root         (0) root         (0)      349 2023-09-07 20:21:37.000000 llsd-1.2.3/.github/release.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-07 20:22:47.728035 llsd-1.2.3/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      898 2023-09-07 20:21:37.000000 llsd-1.2.3/.github/workflows/bench.yaml
--rw-r--r--   0 root         (0) root         (0)     2222 2023-09-07 20:21:37.000000 llsd-1.2.3/.github/workflows/ci.yaml
--rw-r--r--   0 root         (0) root         (0)      854 2023-09-07 20:21:37.000000 llsd-1.2.3/.github/workflows/cla.yaml
--rw-r--r--   0 root         (0) root         (0)     5250 2023-09-07 20:21:37.000000 llsd-1.2.3/.gitignore
--rw-r--r--   0 root         (0) root         (0)      447 2023-09-07 20:21:37.000000 llsd-1.2.3/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)       94 2023-09-07 20:21:37.000000 llsd-1.2.3/CREDITS.md
--rw-r--r--   0 root         (0) root         (0)     1065 2023-09-07 20:21:37.000000 llsd-1.2.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2086 2023-09-07 20:22:47.732035 llsd-1.2.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1308 2023-09-07 20:21:37.000000 llsd-1.2.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-07 20:22:47.728035 llsd-1.2.3/llsd/
--rw-r--r--   0 root         (0) root         (0)     3336 2023-09-07 20:21:37.000000 llsd-1.2.3/llsd/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19685 2023-09-07 20:21:37.000000 llsd-1.2.3/llsd/base.py
--rw-r--r--   0 root         (0) root         (0)     2306 2023-09-07 20:21:37.000000 llsd-1.2.3/llsd/fastest_elementtree.py
--rw-r--r--   0 root         (0) root         (0)     9579 2023-09-07 20:21:37.000000 llsd-1.2.3/llsd/serde_binary.py
--rw-r--r--   0 root         (0) root         (0)    18404 2023-09-07 20:21:37.000000 llsd-1.2.3/llsd/serde_notation.py
--rw-r--r--   0 root         (0) root         (0)    11628 2023-09-07 20:21:37.000000 llsd-1.2.3/llsd/serde_xml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-07 20:22:47.728035 llsd-1.2.3/llsd.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2086 2023-09-07 20:22:47.000000 llsd-1.2.3/llsd.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      532 2023-09-07 20:22:47.000000 llsd-1.2.3/llsd.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-07 20:22:47.000000 llsd-1.2.3/llsd.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-09-07 20:22:47.000000 llsd-1.2.3/llsd.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-09-07 20:22:47.000000 llsd-1.2.3/llsd.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-09-07 20:22:47.732035 llsd-1.2.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1171 2023-09-07 20:21:37.000000 llsd-1.2.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-07 20:22:47.728035 llsd-1.2.3/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-07 20:21:37.000000 llsd-1.2.3/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5288 2023-09-07 20:21:37.000000 llsd-1.2.3/tests/bench.py
--rw-r--r--   0 root         (0) root         (0)    17339 2023-09-07 20:21:37.000000 llsd-1.2.3/tests/fuzz.py
--rw-r--r--   0 root         (0) root         (0)    66168 2023-09-07 20:21:37.000000 llsd-1.2.3/tests/llsd_test.py
--rw-r--r--   0 root         (0) root         (0)      190 2023-09-07 20:21:37.000000 llsd-1.2.3/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 06:37:48.738875 llsd-1.2.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 06:37:48.730875 llsd-1.2.4/.github/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-04-02 06:36:50.000000 llsd-1.2.4/.github/dependabot.yaml
+-rw-r--r--   0 root         (0) root         (0)      349 2024-04-02 06:36:50.000000 llsd-1.2.4/.github/release.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 06:37:48.730875 llsd-1.2.4/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      898 2024-04-02 06:36:50.000000 llsd-1.2.4/.github/workflows/bench.yaml
+-rw-r--r--   0 root         (0) root         (0)     2351 2024-04-02 06:36:50.000000 llsd-1.2.4/.github/workflows/ci.yaml
+-rw-r--r--   0 root         (0) root         (0)      854 2024-04-02 06:36:50.000000 llsd-1.2.4/.github/workflows/cla.yaml
+-rw-r--r--   0 root         (0) root         (0)     5250 2024-04-02 06:36:50.000000 llsd-1.2.4/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      447 2024-04-02 06:36:50.000000 llsd-1.2.4/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)       94 2024-04-02 06:36:50.000000 llsd-1.2.4/CREDITS.md
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-04-02 06:36:50.000000 llsd-1.2.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2086 2024-04-02 06:37:48.738875 llsd-1.2.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1308 2024-04-02 06:36:50.000000 llsd-1.2.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 06:37:48.734875 llsd-1.2.4/llsd/
+-rw-r--r--   0 root         (0) root         (0)     3336 2024-04-02 06:36:50.000000 llsd-1.2.4/llsd/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19685 2024-04-02 06:36:50.000000 llsd-1.2.4/llsd/base.py
+-rw-r--r--   0 root         (0) root         (0)     2306 2024-04-02 06:36:50.000000 llsd-1.2.4/llsd/fastest_elementtree.py
+-rw-r--r--   0 root         (0) root         (0)     9579 2024-04-02 06:36:50.000000 llsd-1.2.4/llsd/serde_binary.py
+-rw-r--r--   0 root         (0) root         (0)    18404 2024-04-02 06:36:50.000000 llsd-1.2.4/llsd/serde_notation.py
+-rw-r--r--   0 root         (0) root         (0)    11663 2024-04-02 06:36:50.000000 llsd-1.2.4/llsd/serde_xml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 06:37:48.734875 llsd-1.2.4/llsd.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2086 2024-04-02 06:37:48.000000 llsd-1.2.4/llsd.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      568 2024-04-02 06:37:48.000000 llsd-1.2.4/llsd.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 06:37:48.000000 llsd-1.2.4/llsd.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2024-04-02 06:37:48.000000 llsd-1.2.4/llsd.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-02 06:37:48.000000 llsd-1.2.4/llsd.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 06:37:48.738875 llsd-1.2.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-04-02 06:36:50.000000 llsd-1.2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 06:37:48.734875 llsd-1.2.4/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 06:36:50.000000 llsd-1.2.4/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5288 2024-04-02 06:36:50.000000 llsd-1.2.4/tests/bench.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 06:37:48.734875 llsd-1.2.4/tests/fixtures/
+-rw-r--r--   0 root         (0) root         (0)   150300 2024-04-02 06:36:50.000000 llsd-1.2.4/tests/fixtures/viewer-autobuild.xml
+-rw-r--r--   0 root         (0) root         (0)    17339 2024-04-02 06:36:50.000000 llsd-1.2.4/tests/fuzz.py
+-rw-r--r--   0 root         (0) root         (0)    67105 2024-04-02 06:36:50.000000 llsd-1.2.4/tests/llsd_test.py
+-rw-r--r--   0 root         (0) root         (0)      195 2024-04-02 06:36:50.000000 llsd-1.2.4/tox.ini
```

### Comparing `llsd-1.2.3/.github/workflows/bench.yaml` & `llsd-1.2.4/.github/workflows/bench.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,17 @@
   deployments: write
 
 jobs:
   benchmark:
     name: Run benchmarks 
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: "3.10"
 
       - name: Run benchmarks
         run: |
           pip install .[dev] 
           pytest tests/bench.py --benchmark-json benchmark.json
```

### Comparing `llsd-1.2.3/.github/workflows/ci.yaml` & `llsd-1.2.4/.github/workflows/ci.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -7,22 +7,26 @@
     tags: [v*.*.*]
 
 jobs:
   build:
     name: Test & Build
     strategy:
       matrix:
-        python-version: ['2.7', '3.7', '3.8', '3.10']
+        python-version: ['3.7', '3.8', '3.10']
+        image-variant: ['']
+        include:
+          - python-version: '2.7'
+            image-variant: '-buster'
     runs-on: [ubuntu-latest]
     container:
-      image: "python:${{ matrix.python-version }}-buster"
+      image: "python:${{ matrix.python-version }}${{ matrix.image-variant }}"
     env:
       PYTHON: ${{ matrix.python-version }}
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0 # fetch all history for setuptools_scm to be able to read tags
 
       - name: Install python dependencies
         run: |
           apt-get update
           apt-get -y install sudo
@@ -40,37 +44,37 @@
           TOXENV: ${{ steps.pyenv.outputs.value }}
         run: tox
 
       - name: Build python package
         run: python -m build
 
       - name: Upload coverage
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
         if: matrix.python-version == '3.10'
         with:
           token: ${{ secrets.CODECOV_TOKEN }}
           env_vars: PYTHON
           fail_ci_if_error: true
           files: .coverage.${{ steps.pyenv.outputs.value }}.xml
 
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         if: matrix.python-version == '2.7' || matrix.python-version == '3.8'
         with:
           name: dist-${{ matrix.python-version }}
           path: dist
 
   publish:
     name: Publish to PyPI
     needs: build
     runs-on: [ubuntu-latest]
     permissions:
       id-token: write
     if: github.event_name != 'pull_request'
     steps:
-      - uses: actions/download-artifact@v3
+      - uses: actions/download-artifact@v4
 
       - name: Organize files for upload
         run: |
           mkdir dist
           mv dist-3.8/* dist/
           mv dist-2.7/*.whl dist/
```

### Comparing `llsd-1.2.3/.github/workflows/cla.yaml` & `llsd-1.2.4/.github/workflows/cla.yaml`

 * *Files identical despite different names*

### Comparing `llsd-1.2.3/.gitignore` & `llsd-1.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `llsd-1.2.3/LICENSE` & `llsd-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `llsd-1.2.3/PKG-INFO` & `llsd-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llsd
-Version: 1.2.3
+Version: 1.2.4
 Summary: Linden Lab Structured Data (LLSD) serialization library
 Home-page: https://github.com/secondlife/python-llsd
 Author: Linden Research, Inc.
 Author-email: opensource-dev@lists.secondlife.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `llsd-1.2.3/README.md` & `llsd-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `llsd-1.2.3/llsd/__init__.py` & `llsd-1.2.4/llsd/__init__.py`

 * *Files identical despite different names*

### Comparing `llsd-1.2.3/llsd/base.py` & `llsd-1.2.4/llsd/base.py`

 * *Files identical despite different names*

### Comparing `llsd-1.2.3/llsd/fastest_elementtree.py` & `llsd-1.2.4/llsd/fastest_elementtree.py`

 * *Files identical despite different names*

### Comparing `llsd-1.2.3/llsd/serde_binary.py` & `llsd-1.2.4/llsd/serde_binary.py`

 * *Files identical despite different names*

### Comparing `llsd-1.2.3/llsd/serde_notation.py` & `llsd-1.2.4/llsd/serde_notation.py`

 * *Files identical despite different names*

### Comparing `llsd-1.2.3/llsd/serde_xml.py` & `llsd-1.2.4/llsd/serde_xml.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,14 +115,15 @@
     def _ARRAY(self, v):
         self.stream.writelines([b'<array>', self._eol])
         self._depth += 1
         for item in v:
             self._indent()
             self._generate(item)
         self._depth -= 1
+        self._indent()
         self.stream.writelines([b'</array>', self._eol])
     def _MAP(self, v):
         self.stream.writelines([b'<map>', self._eol])
         self._depth += 1
         for key, value in v.items():
             self._indent()
             if PY2:     # pragma: no cover
@@ -158,15 +159,15 @@
         """
         Serialize a python object to self.stream as application/llsd+xml.
         :param something: A python object (typically a dict) to be serialized.
         """
         self.stream.writelines([b'<?xml version="1.0" ?>', self._eol,
                                 b'<llsd>', self._eol])
         self._generate(something)
-        self.stream.write(b'</llsd>')
+        self.stream.write(b'</llsd>' + self._eol)
 
 
 class LLSDXMLPrettyFormatter(LLSDXMLFormatter):
     """
     Class which implements 'pretty' LLSD XML serialization..
 
     See http://wiki.secondlife.com/wiki/LLSD#XML_Serialization
```

### Comparing `llsd-1.2.3/llsd.egg-info/PKG-INFO` & `llsd-1.2.4/llsd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llsd
-Version: 1.2.3
+Version: 1.2.4
 Summary: Linden Lab Structured Data (LLSD) serialization library
 Home-page: https://github.com/secondlife/python-llsd
 Author: Linden Research, Inc.
 Author-email: opensource-dev@lists.secondlife.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `llsd-1.2.3/llsd.egg-info/SOURCES.txt` & `llsd-1.2.4/llsd.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -20,8 +20,9 @@
 llsd.egg-info/SOURCES.txt
 llsd.egg-info/dependency_links.txt
 llsd.egg-info/requires.txt
 llsd.egg-info/top_level.txt
 tests/__init__.py
 tests/bench.py
 tests/fuzz.py
-tests/llsd_test.py
+tests/llsd_test.py
+tests/fixtures/viewer-autobuild.xml
```

### Comparing `llsd-1.2.3/setup.py` & `llsd-1.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `llsd-1.2.3/tests/bench.py` & `llsd-1.2.4/tests/bench.py`

 * *Files identical despite different names*

### Comparing `llsd-1.2.3/tests/fuzz.py` & `llsd-1.2.4/tests/fuzz.py`

 * *Files identical despite different names*

### Comparing `llsd-1.2.3/tests/llsd_test.py` & `llsd-1.2.4/tests/llsd_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,22 +8,25 @@
 from itertools import islice
 import pprint
 import re
 import struct
 import time
 import unittest
 import uuid
+from os import path
 
 import pytest
 
 import llsd
-from llsd.base import PY2, is_integer, is_string, is_unicode, MAX_FORMAT_DEPTH, MAX_PARSE_DEPTH
+from llsd.base import PY2, is_integer, is_string, is_unicode, MAX_FORMAT_DEPTH
 from llsd.serde_xml import remove_invalid_xml_bytes
 from tests.fuzz import LLSDFuzzer
 
+FIXTURES_DIR = path.join(path.dirname(__file__), 'fixtures')
+
 
 class Foo(object):
     """
     Simple Mock Class used for testing.
     """
     pass
 
@@ -1401,14 +1404,23 @@
                                   base64_binary_xml)
 
         blank_binary_xml = b"""<?xml version="1.0" ?><llsd><binary /></llsd>"""
 
         python_binary = llsd.binary(b'');
 
         self.assertXMLRoundtrip(python_binary, blank_binary_xml)
+    
+    @pytest.mark.skipif(PY2, reason="Object order between python 2 and 3 differs")
+    def testViewerAutobuildRoundTrip(self):
+        """Test that llsd does not muck up the viewer autobuild"""
+        with open(path.join(FIXTURES_DIR, "viewer-autobuild.xml"), "rb") as f:
+            autobuild_bytes = f.read()
+            autobuild_parsed = llsd.parse_xml(autobuild_bytes)
+        assert autobuild_bytes.decode("utf8") == llsd.format_pretty_xml(autobuild_parsed).decode("utf8")
+        
 
     def testXMLOfAllTypes(self):
         """
         Test parse_xml with complex xml data which contains all types xml element.
         Maps to test scenarios module:llsd:test#65
         """
         xml_of_all_types = b"""<?xml version="1.0" encoding="UTF-8"?>
@@ -1499,14 +1511,33 @@
 
         This maps to test scenarios module:llsd:test#75
         """
         python_object = {'id': ['string1', 123, {'name': 123}]}
 
         output_xml = llsd.format_pretty_xml(python_object)
 
+        with open("foo.llsd.xml", "wb") as f:
+            f.write(output_xml)
+
+        self.assertEqual(output_xml.decode("utf8"), """<?xml version="1.0" ?>
+<llsd>
+<map>
+    <key>id</key>
+    <array>
+      <string>string1</string>
+      <integer>123</integer>
+      <map>
+        <key>name</key>
+        <integer>123</integer>
+      </map>
+    </array>
+  </map>
+</llsd>
+""")
+
         # check whether the output_xml contains whitespaces and new line character
         whitespaces_count = output_xml.count(b' ')
         newline_count = output_xml.count(b'\n')
 
         self.assertTrue(whitespaces_count > 50)
         self.assertTrue(newline_count > 10)
 
@@ -1940,7 +1971,9 @@
     def test_uuid_map_key(self):
         '''
         LLSD Map keys are supposed to be strings; convert a map with a uuid key
         '''
         llsdmap=llsd.LLSD({uuid.UUID(int=0) : 'uuid'})
         self.assertEqual(llsd.format_xml(llsdmap), b'<?xml version="1.0" ?><llsd><map><key>00000000-0000-0000-0000-000000000000</key><string>uuid</string></map></llsd>')
         self.assertEqual(llsd.format_notation(llsdmap), b"{'00000000-0000-0000-0000-000000000000':'uuid'}")
+
+
```

