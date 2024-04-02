# Comparing `tmp/monkey.crawler-2.0.0.dev6.tar.gz` & `tmp/monkey.crawler-2.0.0.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monkey.crawler-2.0.0.dev6.tar", last modified: Wed Nov 29 06:54:25 2023, max compression
+gzip compressed data, was "monkey.crawler-2.0.0.dev7.tar", last modified: Tue Apr  2 14:34:43 2024, max compression
```

## Comparing `monkey.crawler-2.0.0.dev6.tar` & `monkey.crawler-2.0.0.dev7.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-11-29 06:54:25.740352 monkey.crawler-2.0.0.dev6/
--rw-rw-rw-   0        0        0    11556 2023-05-16 05:14:05.000000 monkey.crawler-2.0.0.dev6/LICENSE.txt
--rw-rw-rw-   0        0        0       60 2023-05-16 05:14:05.000000 monkey.crawler-2.0.0.dev6/MANIFEST.in
--rw-rw-rw-   0        0        0      855 2023-11-29 06:54:25.737361 monkey.crawler-2.0.0.dev6/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-05-16 05:14:05.000000 monkey.crawler-2.0.0.dev6/README.rst
-drwxrwxrwx   0        0        0        0 2023-11-29 06:54:25.559324 monkey.crawler-2.0.0.dev6/monkey/
--rw-rw-rw-   0        0        0       84 2023-05-16 05:14:05.000000 monkey.crawler-2.0.0.dev6/monkey/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-29 06:54:25.626596 monkey.crawler-2.0.0.dev6/monkey/crawler/
--rw-rw-rw-   0        0        0       84 2023-05-16 05:14:05.000000 monkey.crawler-2.0.0.dev6/monkey/crawler/__init__.py
--rw-rw-rw-   0        0        0     1177 2023-05-16 05:14:05.000000 monkey.crawler-2.0.0.dev6/monkey/crawler/crawler.py
-drwxrwxrwx   0        0        0        0 2023-11-29 06:54:25.654724 monkey.crawler-2.0.0.dev6/monkey/crawler/crawlers/
--rw-rw-rw-   0        0        0       84 2023-05-16 05:14:05.000000 monkey.crawler-2.0.0.dev6/monkey/crawler/crawlers/__init__.py
--rw-rw-rw-   0        0        0     1191 2023-05-16 05:14:05.000000 monkey.crawler-2.0.0.dev6/monkey/crawler/crawlers/csv.py
--rw-rw-rw-   0        0        0     1108 2023-11-29 06:49:02.000000 monkey.crawler-2.0.0.dev6/monkey/crawler/crawlers/dir.py
--rw-rw-rw-   0        0        0     2814 2023-05-16 05:14:05.000000 monkey.crawler-2.0.0.dev6/monkey/crawler/crawlers/xml.py
-drwxrwxrwx   0        0        0        0 2023-11-29 06:54:25.710435 monkey.crawler-2.0.0.dev6/monkey/crawler/handlers/
--rw-rw-rw-   0        0        0       82 2023-05-16 05:14:05.000000 monkey.crawler-2.0.0.dev6/monkey/crawler/handlers/__init__.py
--rw-rw-rw-   0        0        0     4204 2023-11-29 06:49:02.000000 monkey.crawler-2.0.0.dev6/monkey/crawler/handlers/bulk.py
--rw-rw-rw-   0        0        0     3366 2023-05-31 10:36:15.000000 monkey.crawler-2.0.0.dev6/monkey/crawler/handlers/calc.py
--rw-rw-rw-   0        0        0     2025 2023-05-16 05:14:05.000000 monkey.crawler-2.0.0.dev6/monkey/crawler/handlers/composite.py
--rw-rw-rw-   0        0        0    12818 2023-05-16 05:14:05.000000 monkey.crawler-2.0.0.dev6/monkey/crawler/handlers/filter.py
--rw-rw-rw-   0        0        0     1962 2023-05-16 05:14:05.000000 monkey.crawler-2.0.0.dev6/monkey/crawler/handlers/format.py
--rw-rw-rw-   0        0        0     2169 2023-11-29 06:49:02.000000 monkey.crawler-2.0.0.dev6/monkey/crawler/handlers/project.py
--rw-rw-rw-   0        0        0     8402 2023-11-29 06:49:02.000000 monkey.crawler-2.0.0.dev6/monkey/crawler/handlers/transform.py
--rw-rw-rw-   0        0        0     1835 2023-05-16 05:14:05.000000 monkey.crawler-2.0.0.dev6/monkey/crawler/op_codes.py
--rw-rw-rw-   0        0        0     6275 2023-06-01 06:27:23.000000 monkey.crawler-2.0.0.dev6/monkey/crawler/pipeline.py
--rw-rw-rw-   0        0        0     2885 2023-05-16 05:14:05.000000 monkey.crawler-2.0.0.dev6/monkey/crawler/processor.py
-drwxrwxrwx   0        0        0        0 2023-11-29 06:54:25.727412 monkey.crawler-2.0.0.dev6/monkey/crawler/processors/
--rw-rw-rw-   0        0        0       82 2023-05-16 05:14:05.000000 monkey.crawler-2.0.0.dev6/monkey/crawler/processors/__init__.py
--rw-rw-rw-   0        0        0     7670 2023-05-16 05:14:05.000000 monkey.crawler-2.0.0.dev6/monkey/crawler/processors/dump.py
-drwxrwxrwx   0        0        0        0 2023-11-29 06:54:25.734370 monkey.crawler-2.0.0.dev6/monkey.crawler.egg-info/
--rw-rw-rw-   0        0        0      855 2023-11-29 06:54:25.000000 monkey.crawler-2.0.0.dev6/monkey.crawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      844 2023-11-29 06:54:25.000000 monkey.crawler-2.0.0.dev6/monkey.crawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-29 06:54:25.000000 monkey.crawler-2.0.0.dev6/monkey.crawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-11-29 06:54:25.000000 monkey.crawler-2.0.0.dev6/monkey.crawler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-05-16 05:14:05.000000 monkey.crawler-2.0.0.dev6/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-11-29 06:54:25.741350 monkey.crawler-2.0.0.dev6/setup.cfg
--rw-rw-rw-   0        0        0     1302 2023-11-29 06:51:16.000000 monkey.crawler-2.0.0.dev6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 14:34:43.365784 monkey.crawler-2.0.0.dev7/
+-rw-rw-rw-   0        0        0    11556 2023-05-16 05:14:05.000000 monkey.crawler-2.0.0.dev7/LICENSE.txt
+-rw-rw-rw-   0        0        0       60 2023-05-16 05:14:05.000000 monkey.crawler-2.0.0.dev7/MANIFEST.in
+-rw-rw-rw-   0        0        0      855 2024-04-02 14:34:43.362789 monkey.crawler-2.0.0.dev7/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-05-16 05:14:05.000000 monkey.crawler-2.0.0.dev7/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-02 14:34:43.227157 monkey.crawler-2.0.0.dev7/monkey/
+-rw-rw-rw-   0        0        0       84 2023-05-16 05:14:05.000000 monkey.crawler-2.0.0.dev7/monkey/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 14:34:43.283004 monkey.crawler-2.0.0.dev7/monkey/crawler/
+-rw-rw-rw-   0        0        0       84 2023-05-16 05:14:05.000000 monkey.crawler-2.0.0.dev7/monkey/crawler/__init__.py
+-rw-rw-rw-   0        0        0     1177 2023-05-16 05:14:05.000000 monkey.crawler-2.0.0.dev7/monkey/crawler/crawler.py
+drwxrwxrwx   0        0        0        0 2024-04-02 14:34:43.300954 monkey.crawler-2.0.0.dev7/monkey/crawler/crawlers/
+-rw-rw-rw-   0        0        0       84 2023-05-16 05:14:05.000000 monkey.crawler-2.0.0.dev7/monkey/crawler/crawlers/__init__.py
+-rw-rw-rw-   0        0        0     1191 2023-05-16 05:14:05.000000 monkey.crawler-2.0.0.dev7/monkey/crawler/crawlers/csv.py
+-rw-rw-rw-   0        0        0     1108 2023-11-29 06:49:02.000000 monkey.crawler-2.0.0.dev7/monkey/crawler/crawlers/dir.py
+-rw-rw-rw-   0        0        0     2814 2023-05-16 05:14:05.000000 monkey.crawler-2.0.0.dev7/monkey/crawler/crawlers/xml.py
+drwxrwxrwx   0        0        0        0 2024-04-02 14:34:43.342843 monkey.crawler-2.0.0.dev7/monkey/crawler/handlers/
+-rw-rw-rw-   0        0        0       82 2023-05-16 05:14:05.000000 monkey.crawler-2.0.0.dev7/monkey/crawler/handlers/__init__.py
+-rw-rw-rw-   0        0        0     4204 2023-11-29 06:49:02.000000 monkey.crawler-2.0.0.dev7/monkey/crawler/handlers/bulk.py
+-rw-rw-rw-   0        0        0     3366 2023-05-31 10:36:15.000000 monkey.crawler-2.0.0.dev7/monkey/crawler/handlers/calc.py
+-rw-rw-rw-   0        0        0     2025 2023-05-16 05:14:05.000000 monkey.crawler-2.0.0.dev7/monkey/crawler/handlers/composite.py
+-rw-rw-rw-   0        0        0    12818 2023-05-16 05:14:05.000000 monkey.crawler-2.0.0.dev7/monkey/crawler/handlers/filter.py
+-rw-rw-rw-   0        0        0     1962 2023-05-16 05:14:05.000000 monkey.crawler-2.0.0.dev7/monkey/crawler/handlers/format.py
+-rw-rw-rw-   0        0        0     2169 2023-11-29 06:49:02.000000 monkey.crawler-2.0.0.dev7/monkey/crawler/handlers/project.py
+-rw-rw-rw-   0        0        0     9324 2024-04-02 14:33:38.000000 monkey.crawler-2.0.0.dev7/monkey/crawler/handlers/transform.py
+-rw-rw-rw-   0        0        0     1835 2023-05-16 05:14:05.000000 monkey.crawler-2.0.0.dev7/monkey/crawler/op_codes.py
+-rw-rw-rw-   0        0        0     6275 2023-06-01 06:27:23.000000 monkey.crawler-2.0.0.dev7/monkey/crawler/pipeline.py
+-rw-rw-rw-   0        0        0     2885 2023-05-16 05:14:05.000000 monkey.crawler-2.0.0.dev7/monkey/crawler/processor.py
+drwxrwxrwx   0        0        0        0 2024-04-02 14:34:43.352815 monkey.crawler-2.0.0.dev7/monkey/crawler/processors/
+-rw-rw-rw-   0        0        0       82 2023-05-16 05:14:05.000000 monkey.crawler-2.0.0.dev7/monkey/crawler/processors/__init__.py
+-rw-rw-rw-   0        0        0     7670 2023-05-16 05:14:05.000000 monkey.crawler-2.0.0.dev7/monkey/crawler/processors/dump.py
+drwxrwxrwx   0        0        0        0 2024-04-02 14:34:43.358802 monkey.crawler-2.0.0.dev7/monkey.crawler.egg-info/
+-rw-rw-rw-   0        0        0      855 2024-04-02 14:34:43.000000 monkey.crawler-2.0.0.dev7/monkey.crawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      844 2024-04-02 14:34:43.000000 monkey.crawler-2.0.0.dev7/monkey.crawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 14:34:43.000000 monkey.crawler-2.0.0.dev7/monkey.crawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-02 14:34:43.000000 monkey.crawler-2.0.0.dev7/monkey.crawler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-05-16 05:14:05.000000 monkey.crawler-2.0.0.dev7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 14:34:43.366780 monkey.crawler-2.0.0.dev7/setup.cfg
+-rw-rw-rw-   0        0        0     1302 2024-04-02 14:33:38.000000 monkey.crawler-2.0.0.dev7/setup.py
```

### Comparing `monkey.crawler-2.0.0.dev6/LICENSE.txt` & `monkey.crawler-2.0.0.dev7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `monkey.crawler-2.0.0.dev6/PKG-INFO` & `monkey.crawler-2.0.0.dev7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monkey.crawler
-Version: 2.0.0.dev6
+Version: 2.0.0.dev7
 Summary: Small framework to crawl misc data sources and process records.
 Home-page: https://bitbucket.org/monkeytechnologies/monkey-crawler
 Author: Xavier ROY
 Author-email: xavier@regbuddy.eu
 License: Apache License, Version 2.0
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 1 - Planning
```

### Comparing `monkey.crawler-2.0.0.dev6/monkey/crawler/crawler.py` & `monkey.crawler-2.0.0.dev7/monkey/crawler/crawler.py`

 * *Files identical despite different names*

### Comparing `monkey.crawler-2.0.0.dev6/monkey/crawler/crawlers/csv.py` & `monkey.crawler-2.0.0.dev7/monkey/crawler/crawlers/csv.py`

 * *Files identical despite different names*

### Comparing `monkey.crawler-2.0.0.dev6/monkey/crawler/crawlers/dir.py` & `monkey.crawler-2.0.0.dev7/monkey/crawler/crawlers/dir.py`

 * *Files identical despite different names*

### Comparing `monkey.crawler-2.0.0.dev6/monkey/crawler/crawlers/xml.py` & `monkey.crawler-2.0.0.dev7/monkey/crawler/crawlers/xml.py`

 * *Files identical despite different names*

### Comparing `monkey.crawler-2.0.0.dev6/monkey/crawler/handlers/bulk.py` & `monkey.crawler-2.0.0.dev7/monkey/crawler/handlers/bulk.py`

 * *Files identical despite different names*

### Comparing `monkey.crawler-2.0.0.dev6/monkey/crawler/handlers/calc.py` & `monkey.crawler-2.0.0.dev7/monkey/crawler/handlers/calc.py`

 * *Files identical despite different names*

### Comparing `monkey.crawler-2.0.0.dev6/monkey/crawler/handlers/composite.py` & `monkey.crawler-2.0.0.dev7/monkey/crawler/handlers/composite.py`

 * *Files identical despite different names*

### Comparing `monkey.crawler-2.0.0.dev6/monkey/crawler/handlers/filter.py` & `monkey.crawler-2.0.0.dev7/monkey/crawler/handlers/filter.py`

 * *Files identical despite different names*

### Comparing `monkey.crawler-2.0.0.dev6/monkey/crawler/handlers/format.py` & `monkey.crawler-2.0.0.dev7/monkey/crawler/handlers/format.py`

 * *Files identical despite different names*

### Comparing `monkey.crawler-2.0.0.dev6/monkey/crawler/handlers/project.py` & `monkey.crawler-2.0.0.dev7/monkey/crawler/handlers/project.py`

 * *Files identical despite different names*

### Comparing `monkey.crawler-2.0.0.dev6/monkey/crawler/handlers/transform.py` & `monkey.crawler-2.0.0.dev7/monkey/crawler/handlers/transform.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,14 +101,38 @@
         """
         if value is not None and len(value) > 0:
             return datetime.strptime(value, self.format_spec)
         else:
             return None
 
 
+class DatetimeFormatter(Transformer):
+    """Converts the value of the specified field into datetime representation string.
+        See: 'Format codes
+        <https://docs.python.org/fr/3/library/datetime.html?highlight=datetime#strftime-strptime-behavior>'_
+        """
+    def __init__(self, format_spec: str = '%Y-%m-%dT%H:%M:%S'):
+        """Initializes the transformer
+        :param format_spec: the format specification. If not specified, the format operation applies ISO 8601 format
+        'YYYY-MM-DDTHH:MM:SS'.
+        """
+        super().__init__()
+        self.format_spec = format_spec
+
+    def transform(self, value):
+        """Performs the format operation
+        :param value: the value to format
+        :return: the formatted value
+        """
+        if isinstance(value, datetime):
+            return value.strptime(self.format_spec)
+        else:
+            return None
+
+
 class E164Formatter(Transformer):
     """Converts specified field value as a string representation of a phone number in E.164 format
     """
 
     def __init__(self, default_country_code: int = None):
         """Initializes the transformer
         :param default_country_code: the country code (dial code) to use by default if provided value does not represent
```

### Comparing `monkey.crawler-2.0.0.dev6/monkey/crawler/op_codes.py` & `monkey.crawler-2.0.0.dev7/monkey/crawler/op_codes.py`

 * *Files identical despite different names*

### Comparing `monkey.crawler-2.0.0.dev6/monkey/crawler/pipeline.py` & `monkey.crawler-2.0.0.dev7/monkey/crawler/pipeline.py`

 * *Files identical despite different names*

### Comparing `monkey.crawler-2.0.0.dev6/monkey/crawler/processor.py` & `monkey.crawler-2.0.0.dev7/monkey/crawler/processor.py`

 * *Files identical despite different names*

### Comparing `monkey.crawler-2.0.0.dev6/monkey/crawler/processors/dump.py` & `monkey.crawler-2.0.0.dev7/monkey/crawler/processors/dump.py`

 * *Files identical despite different names*

### Comparing `monkey.crawler-2.0.0.dev6/monkey.crawler.egg-info/PKG-INFO` & `monkey.crawler-2.0.0.dev7/monkey.crawler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monkey.crawler
-Version: 2.0.0.dev6
+Version: 2.0.0.dev7
 Summary: Small framework to crawl misc data sources and process records.
 Home-page: https://bitbucket.org/monkeytechnologies/monkey-crawler
 Author: Xavier ROY
 Author-email: xavier@regbuddy.eu
 License: Apache License, Version 2.0
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 1 - Planning
```

### Comparing `monkey.crawler-2.0.0.dev6/monkey.crawler.egg-info/SOURCES.txt` & `monkey.crawler-2.0.0.dev7/monkey.crawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `monkey.crawler-2.0.0.dev6/setup.py` & `monkey.crawler-2.0.0.dev7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import os
 from setuptools import setup, find_packages
 
 __name__ = 'monkey.crawler'
-__version__ = '2.0.0.dev6'
+__version__ = '2.0.0.dev7'
 __author__ = 'Xavier ROY'
 __author_email__ = 'xavier@regbuddy.eu'
 
 project_dir = os.path.dirname(os.path.realpath(__file__))
 requirement_file_path = project_dir + '/requirements.txt'
 requirements = []
 if os.path.isfile(requirement_file_path):
```

