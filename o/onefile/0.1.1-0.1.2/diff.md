# Comparing `tmp/onefile-0.1.1.tar.gz` & `tmp/onefile-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onefile-0.1.1.tar", max compression
+gzip compressed data, was "onefile-0.1.2.tar", max compression
```

## Comparing `onefile-0.1.1.tar` & `onefile-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0     1084 2024-03-21 14:26:35.830740 onefile-0.1.1/LICENSE
--rw-r--r--   0        0        0      218 2024-03-21 14:26:35.830740 onefile-0.1.1/README.md
--rw-r--r--   0        0        0      343 2024-03-21 14:26:35.830740 onefile-0.1.1/onefile/__init__.py
--rw-r--r--   0        0        0    11952 2024-03-21 14:26:35.830740 onefile-0.1.1/onefile/junit.py
--rw-r--r--   0        0        0      374 2024-03-21 14:26:35.830740 onefile-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      824 1970-01-01 00:00:00.000000 onefile-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2024-04-02 15:22:22.177219 onefile-0.1.2/LICENSE
+-rw-r--r--   0        0        0      673 2024-04-02 15:22:22.177219 onefile-0.1.2/README.md
+-rw-r--r--   0        0        0      343 2024-04-02 15:22:22.177219 onefile-0.1.2/onefile/__init__.py
+-rw-r--r--   0        0        0    12216 2024-04-02 15:22:22.177219 onefile-0.1.2/onefile/junit.py
+-rw-r--r--   0        0        0    15890 2024-04-02 15:22:22.177219 onefile-0.1.2/onefile/report_html.py
+-rw-r--r--   0        0        0    10895 2024-04-02 15:22:22.177219 onefile-0.1.2/onefile/template.html
+-rw-r--r--   0        0        0      392 2024-04-02 15:22:22.177219 onefile-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1318 1970-01-01 00:00:00.000000 onefile-0.1.2/PKG-INFO
```

### Comparing `onefile-0.1.1/LICENSE` & `onefile-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `onefile-0.1.1/onefile/junit.py` & `onefile-0.1.2/onefile/junit.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 class Message:
     def __init__(self, message: str, text: Optional[str] = None):
         self.message: str = message
         self.text: str = text
 
     def __repr__(self):
         return (
-            f"{self.__class__.__name__}(message='{self.message}', text='{self.text}')"
+            f"{self.__class__.__name__}(message='{self.message}', "
+            f"text='{self.text}')"
         )
 
 
 class Error(Message):
     pass
 
 
@@ -31,15 +32,16 @@
 class Skipped(Message):
     def __init__(self, skip_type: str, message: str, text: str):
         super().__init__(message, text)
         self.type = skip_type
 
     def __repr__(self):
         return (
-            f"Skipped(message='{self.message}', type='{self.type}', text='{self.text})"
+            f"Skipped(message='{self.message}', type='{self.type}', "
+            f"text='{self.text})"
         )
 
 
 class TestCase:
     def __init__(
         self,
         classname: str = "",
@@ -60,16 +62,16 @@
         self.failure = failure
         self.skipped = skipped
 
     def __repr__(self):
         return (
             f"TestCase(classname='{self.classname}', name='{self.name}', "
             f"file='{self.file}', line='{self.line}', "
-            f"time='{self.time}', error='{self.error}', failure='{self.failure}', "
-            f"skipped='{self.skipped}')"
+            f"time='{self.time}', error='{self.error}', "
+            f"failure='{self.failure}', skipped='{self.skipped}')"
         )
 
 
 class TestSuite:
     def __init__(
         self,
         name: str = "",
@@ -94,15 +96,16 @@
     def add_test_case(self, test_case: TestCase) -> None:
         self.test_cases.append(test_case)
 
     def __repr__(self):
         return (
             f"TestSuite(name='{self.name}', errors={self.errors}, "
             f"failures={self.failures}, skipped={self.skipped}, "
-            f"tests={self.tests}, time={self.time}, timestamp='{self.timestamp}', "
+            f"tests={self.tests}, time={self.time}, "
+            f"timestamp='{self.timestamp}', "
             f"hostname='{self.hostname}', testcases={self.test_cases})"
         )
 
 
 class TestSuites:
     def __init__(self):
         self.test_suites: list[TestSuite] = []
@@ -138,23 +141,29 @@
             )
 
             for test_case_elem in test_suite_elem:
                 error, failure, skipped = None, None, None
 
                 if (error_elem := test_case_elem.find("error")) is not None:
                     error = Error(
-                        message=error_elem.get("message", ""), text=error_elem.text
+                        message=error_elem.get("message", ""),
+                        text=error_elem.text,
                     )
 
-                if (failure_elem := test_case_elem.find("failure")) is not None:
+                if (
+                    failure_elem := test_case_elem.find("failure")
+                ) is not None:
                     failure = Failure(
-                        message=failure_elem.get("message", ""), text=failure_elem.text
+                        message=failure_elem.get("message", ""),
+                        text=failure_elem.text,
                     )
 
-                if (skipped_elem := test_case_elem.find("skipped")) is not None:
+                if (
+                    skipped_elem := test_case_elem.find("skipped")
+                ) is not None:
                     skipped = Skipped(
                         skip_type=skipped_elem.get("type", ""),
                         message=skipped_elem.get("message", ""),
                         text=skipped_elem.text,
                     )
 
                 test_case = TestCase(
@@ -203,19 +212,23 @@
                     if tc.classname == loaded_testcase.classname
                     and tc.name == loaded_testcase.name
                 ),
                 None,
             )
 
             if existing_tc_index is not None:
-                logging.debug(f"Test case found!")
+                logging.debug("Test case found!")
                 if is_test_suite_timestamp_updated:
                     logging.debug("Test suite timestamp is updated!")
-                    logging.debug("Update final test suite errors, failures, skipped")
-                    existing_tc = final_test_suite.test_cases[existing_tc_index]
+                    logging.debug(
+                        "Update final test suite errors, failures, skipped"
+                    )
+                    existing_tc = final_test_suite.test_cases[
+                        existing_tc_index
+                    ]
 
                     if loaded_testcase.error and not existing_tc.error:
                         logging.debug("Increase errors attribute!")
                         final_test_suite.errors += 1
                     elif not loaded_testcase.error and existing_tc.error:
                         logging.debug("Decrease errors attribute!")
                         final_test_suite.errors -= 1
@@ -237,15 +250,15 @@
                     existing_tc.time = loaded_testcase.time
                     existing_tc.error = loaded_testcase.error
                     existing_tc.failure = loaded_testcase.failure
                     existing_tc.skipped = loaded_testcase.skipped
                 else:
                     logging.debug("Test suite timestamp is NOT updated!")
             else:
-                logging.debug(f"Test case NOT found!")
+                logging.debug("Test case NOT found!")
                 if loaded_testcase.error:
                     final_test_suite.errors += 1
                 if loaded_testcase.failure:
                     final_test_suite.failures += 1
                 if loaded_testcase.skipped:
                     final_test_suite.skipped += 1
                 final_test_suite.tests += 1
```

### Comparing `onefile-0.1.1/PKG-INFO` & `onefile-0.1.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,42 @@
 Metadata-Version: 2.1
 Name: onefile
-Version: 0.1.1
+Version: 0.1.2
 Summary: Merge multiple files into one!
 License: MIT
 Author: Andras Santa
 Author-email: andras.santa@zyte.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: lxml (>=5.1.0,<6.0.0)
+Requires-Dist: parsel (>=1.8.1,<2.0.0)
 Requires-Dist: pytest (>=8.0.0,<9.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # onefile
 Merge multiples files into one!
 
 Current supported files to merge:
 
-- junit.xml
+- junit.xml (Ref.: [JUnitXML file](https://docs.pytest.org/en/7.1.x/how-to/output.html#creating-junitxml-format-files))
+- report.html (Ref.: [self-contained HTML report file](https://pytest-html.readthedocs.io/en/latest/user_guide.html#enhancing-reports))
 
-Example:
+Example for junit.xml file merge:
 
 ```
 from onefile.junit import merge_junit_files
 
 merge_junit_files(["junit_1.xml", "junit_2.xml", "junit_3.xml"])
 ```
+
+Example for report.html file merge:
+
+```
+from onefile.report_html import merge_report_html_files
+
+merge_junit_files(["report_html_1.xml", "report_html_2.xml", "report_html_3.xml"])
+```
```

