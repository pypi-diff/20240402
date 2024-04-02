# Comparing `tmp/space_packet_parser-4.2.0rc2.tar.gz` & `tmp/space_packet_parser-4.2.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "space_packet_parser-4.2.0rc2.tar", max compression
+gzip compressed data, was "space_packet_parser-4.2.0rc3.tar", max compression
```

## Comparing `space_packet_parser-4.2.0rc2.tar` & `space_packet_parser-4.2.0rc3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1891 2024-03-06 16:54:13.972484 space_packet_parser-4.2.0rc2/CITATION.cff
--rw-r--r--   0        0        0     1485 2023-03-10 14:38:01.516115 space_packet_parser-4.2.0rc2/LICENSE.txt
--rw-r--r--   0        0        0      928 2023-08-25 16:27:42.967679 space_packet_parser-4.2.0rc2/README.md
--rw-r--r--   0        0        0     1523 2024-03-14 05:02:14.741412 space_packet_parser-4.2.0rc2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-10 14:37:59.135790 space_packet_parser-4.2.0rc2/space_packet_parser/__init__.py
--rw-r--r--   0        0        0    11212 2023-03-14 19:05:53.865522 space_packet_parser-4.2.0rc2/space_packet_parser/csvdef.py
--rw-r--r--   0        0        0    28202 2024-03-14 04:57:44.972800 space_packet_parser-4.2.0rc2/space_packet_parser/parser.py
--rw-r--r--   0        0        0   107227 2024-03-14 04:57:44.973186 space_packet_parser-4.2.0rc2/space_packet_parser/xtcedef.py
--rw-r--r--   0        0        0     2080 1970-01-01 00:00:00.000000 space_packet_parser-4.2.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     1891 2024-03-06 16:54:13.972484 space_packet_parser-4.2.0rc3/CITATION.cff
+-rw-r--r--   0        0        0     1485 2023-03-10 14:38:01.516115 space_packet_parser-4.2.0rc3/LICENSE.txt
+-rw-r--r--   0        0        0      928 2023-08-25 16:27:42.967679 space_packet_parser-4.2.0rc3/README.md
+-rw-r--r--   0        0        0     1523 2024-03-18 19:26:12.546493 space_packet_parser-4.2.0rc3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-10 14:37:59.135790 space_packet_parser-4.2.0rc3/space_packet_parser/__init__.py
+-rw-r--r--   0        0        0    11212 2023-03-14 19:05:53.865522 space_packet_parser-4.2.0rc3/space_packet_parser/csvdef.py
+-rw-r--r--   0        0        0    28202 2024-03-14 04:57:44.972800 space_packet_parser-4.2.0rc3/space_packet_parser/parser.py
+-rw-r--r--   0        0        0   107402 2024-03-14 06:54:28.728965 space_packet_parser-4.2.0rc3/space_packet_parser/xtcedef.py
+-rw-r--r--   0        0        0     2080 1970-01-01 00:00:00.000000 space_packet_parser-4.2.0rc3/PKG-INFO
```

### Comparing `space_packet_parser-4.2.0rc2/CITATION.cff` & `space_packet_parser-4.2.0rc3/CITATION.cff`

 * *Files identical despite different names*

### Comparing `space_packet_parser-4.2.0rc2/LICENSE.txt` & `space_packet_parser-4.2.0rc3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `space_packet_parser-4.2.0rc2/README.md` & `space_packet_parser-4.2.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `space_packet_parser-4.2.0rc2/pyproject.toml` & `space_packet_parser-4.2.0rc3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "space_packet_parser"
-version = "4.2.0rc2"
+version = "4.2.0rc3"
 description = "A CCSDS telemetry packet decoding library based on the XTCE packet format description standard."
 license = "BSD-3-Clause"
 readme = "README.md"
 include = ["LICENSE.txt", "CITATION.cff"]
 authors = [
     "Gavin Medley <gavin.medley@lasp.colorado.edu>",
     "Michael Chambliss <michael.chambliss@lasp.colorado.edu>",
```

### Comparing `space_packet_parser-4.2.0rc2/space_packet_parser/csvdef.py` & `space_packet_parser-4.2.0rc3/space_packet_parser/csvdef.py`

 * *Files identical despite different names*

### Comparing `space_packet_parser-4.2.0rc2/space_packet_parser/parser.py` & `space_packet_parser-4.2.0rc3/space_packet_parser/parser.py`

 * *Files identical despite different names*

### Comparing `space_packet_parser-4.2.0rc2/space_packet_parser/xtcedef.py` & `space_packet_parser-4.2.0rc3/space_packet_parser/xtcedef.py`

 * *Files 0% similar despite different names*

```diff
@@ -860,18 +860,20 @@
         context_match_element = element.find('xtce:ContextMatch', ns)
         if context_match_element.find('xtce:ComparisonList', ns) is not None:
             return [Comparison.from_match_criteria_xml_element(el, ns)
                     for el in context_match_element.findall('xtce:ComparisonList/xtce:Comparison', ns)]
         if context_match_element.find('xtce:Comparison', ns) is not None:
             return [Comparison.from_match_criteria_xml_element(
                 context_match_element.find('xtce:Comparison', ns), ns)]
-        # TODO: Implement handling of BooleanExpression
-        raise NotImplementedError("ContextCalibrator doesn't contain Comparison on ComparisonList. This probably"
-                                  "means the match criteria is an unsupported type (BooleanExpression or "
-                                  "CustomAlgorithm).")
+        if context_match_element.find('xtce:BooleanExpression', ns) is not None:
+            return [BooleanExpression.from_match_criteria_xml_element(
+                context_match_element.find('xtce:BooleanExpression', ns), ns)]
+        raise NotImplementedError("ContextCalibrator doesn't contain Comparison, ComparisonList, or BooleanExpression. "
+                                  "This probably means the match criteria is an unsupported type "
+                                  "(CustomAlgorithm).")
 
     @classmethod
     def from_context_calibrator_xml_element(cls, element: ElementTree.Element, ns: dict):
         """Create a ContextCalibrator object from an <xtce:ContextCalibrator> XML element
 
         Parameters
         ----------
```

### Comparing `space_packet_parser-4.2.0rc2/PKG-INFO` & `space_packet_parser-4.2.0rc3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: space_packet_parser
-Version: 4.2.0rc2
+Version: 4.2.0rc3
 Summary: A CCSDS telemetry packet decoding library based on the XTCE packet format description standard.
 Home-page: https://space-packet-parser.readthedocs.io
 License: BSD-3-Clause
 Keywords: ccsds,xtce,space data systems,space packet protocol,packet parsing,lasp,university of colorado,data processing,data extraction,data manipulation,data transformation,data encoding,data decoding,packet inspection,binary data,python
 Author: Gavin Medley
 Author-email: gavin.medley@lasp.colorado.edu
 Maintainer: Gavin Medley
```

