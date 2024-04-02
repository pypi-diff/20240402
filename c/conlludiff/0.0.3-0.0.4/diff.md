# Comparing `tmp/conlludiff-0.0.3.tar.gz` & `tmp/conlludiff-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conlludiff-0.0.3.tar", last modified: Thu Mar 28 11:14:44 2024, max compression
+gzip compressed data, was "conlludiff-0.0.4.tar", last modified: Tue Apr  2 08:11:44 2024, max compression
```

## Comparing `conlludiff-0.0.3.tar` & `conlludiff-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-03-28 11:14:44.669266 conlludiff-0.0.3/
--rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)    11357 2024-03-27 11:54:24.000000 conlludiff-0.0.3/LICENSE
--rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-03-27 11:54:24.000000 conlludiff-0.0.3/MANIFEST.in
--rw-r--r--   0 prupnik  (1977552579) prupnik  (1977552579)    29553 2024-03-28 11:14:44.669266 conlludiff-0.0.3/PKG-INFO
--rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)    15787 2024-03-28 11:11:28.000000 conlludiff-0.0.3/README.md
--rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     1062 2024-03-28 11:12:41.000000 conlludiff-0.0.3/pyproject.toml
--rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)       38 2024-03-28 11:14:44.670266 conlludiff-0.0.3/setup.cfg
-drwxrwxr-x   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-03-28 11:14:44.518263 conlludiff-0.0.3/src/
-drwxrwxr-x   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-03-28 11:14:44.623265 conlludiff-0.0.3/src/conlludiff/
--rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)       28 2024-03-27 12:20:04.000000 conlludiff-0.0.3/src/conlludiff/__init__.py
--rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     4245 2024-03-27 11:54:24.000000 conlludiff-0.0.3/src/conlludiff/__main__.py
--rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     7486 2024-03-27 12:20:10.000000 conlludiff-0.0.3/src/conlludiff/differ.py
-drwxrwxr-x   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-03-28 11:14:44.667266 conlludiff-0.0.3/src/conlludiff.egg-info/
--rw-r--r--   0 prupnik  (1977552579) prupnik  (1977552579)    29553 2024-03-28 11:14:44.000000 conlludiff-0.0.3/src/conlludiff.egg-info/PKG-INFO
--rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)      362 2024-03-28 11:14:44.000000 conlludiff-0.0.3/src/conlludiff.egg-info/SOURCES.txt
--rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)        1 2024-03-28 11:14:44.000000 conlludiff-0.0.3/src/conlludiff.egg-info/dependency_links.txt
--rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)       70 2024-03-28 11:14:44.000000 conlludiff-0.0.3/src/conlludiff.egg-info/requires.txt
--rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)       16 2024-03-28 11:14:44.000000 conlludiff-0.0.3/src/conlludiff.egg-info/top_level.txt
-drwxrwxr-x   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-03-28 11:14:44.626265 conlludiff-0.0.3/src/docs/
--rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     1527 2024-03-27 11:54:25.000000 conlludiff-0.0.3/src/docs/conf.py
-drwxrwxr-x   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-03-28 11:14:44.663266 conlludiff-0.0.3/tests/
--rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     1635 2024-03-27 11:54:25.000000 conlludiff-0.0.3/tests/test_expected_behaviour.py
+drwxrwxr-x   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-02 08:11:44.768902 conlludiff-0.0.4/
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)    11357 2024-03-27 11:54:24.000000 conlludiff-0.0.4/LICENSE
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-03-27 11:54:24.000000 conlludiff-0.0.4/MANIFEST.in
+-rw-r--r--   0 prupnik  (1977552579) prupnik  (1977552579)    29556 2024-04-02 08:11:44.767902 conlludiff-0.0.4/PKG-INFO
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)    15790 2024-03-28 14:07:26.000000 conlludiff-0.0.4/README.md
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     1062 2024-04-02 08:10:24.000000 conlludiff-0.0.4/pyproject.toml
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)       38 2024-04-02 08:11:44.768902 conlludiff-0.0.4/setup.cfg
+drwxrwxr-x   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-02 08:11:44.702901 conlludiff-0.0.4/src/
+drwxrwxr-x   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-02 08:11:44.705901 conlludiff-0.0.4/src/conlludiff/
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)       28 2024-03-27 12:20:04.000000 conlludiff-0.0.4/src/conlludiff/__init__.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     4673 2024-04-02 08:05:15.000000 conlludiff-0.0.4/src/conlludiff/__main__.py
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     8038 2024-04-02 08:05:15.000000 conlludiff-0.0.4/src/conlludiff/differ.py
+drwxrwxr-x   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-02 08:11:44.766902 conlludiff-0.0.4/src/conlludiff.egg-info/
+-rw-r--r--   0 prupnik  (1977552579) prupnik  (1977552579)    29556 2024-04-02 08:11:44.000000 conlludiff-0.0.4/src/conlludiff.egg-info/PKG-INFO
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)      362 2024-04-02 08:11:44.000000 conlludiff-0.0.4/src/conlludiff.egg-info/SOURCES.txt
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)        1 2024-04-02 08:11:44.000000 conlludiff-0.0.4/src/conlludiff.egg-info/dependency_links.txt
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)       70 2024-04-02 08:11:44.000000 conlludiff-0.0.4/src/conlludiff.egg-info/requires.txt
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)       16 2024-04-02 08:11:44.000000 conlludiff-0.0.4/src/conlludiff.egg-info/top_level.txt
+drwxrwxr-x   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-02 08:11:44.707901 conlludiff-0.0.4/src/docs/
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     1527 2024-03-27 11:54:25.000000 conlludiff-0.0.4/src/docs/conf.py
+drwxrwxr-x   0 prupnik  (1977552579) prupnik  (1977552579)        0 2024-04-02 08:11:44.765902 conlludiff-0.0.4/tests/
+-rw-rw-r--   0 prupnik  (1977552579) prupnik  (1977552579)     1123 2024-04-02 08:05:15.000000 conlludiff-0.0.4/tests/test_expected_behaviour.py
```

### Comparing `conlludiff-0.0.3/LICENSE` & `conlludiff-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `conlludiff-0.0.3/PKG-INFO` & `conlludiff-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conlludiff
-Version: 0.0.3
+Version: 0.0.4
 Summary: Analyze two CONLLU files
 Author-email: Peter Rupnik <rupnikpeter@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -234,15 +234,15 @@
 
 ```
 pip install conlludiff
 ```
 
 ## CLI use
 
-Run as `python conlludiff <json>`.
+Run as `python -m conlludiff <json>`.
 
 The tool is configured through a JSON configuration file (example in `config_files/ssj_sst_upos.json`) where the user defines:
 - `file1` - The conllu file containing the first language sample
 - `file2` - The conllu file containing the second language sample
 - `event` - The linguistic feature the comparison is to be based on, optional events are form, lemma, upos, xpos, upos+feats, feat (each feature separately), feats (all features of a word merged), deprel, deprel+head_deprel
 - `filter` - The minimum p-value of the chi-square test for the entry to be filtered from the results
 - `fields` - A list of fields to be retained in the output (list of available values is listed below)
```

### Comparing `conlludiff-0.0.3/README.md` & `conlludiff-0.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 ```
 pip install conlludiff
 ```
 
 ## CLI use
 
-Run as `python conlludiff <json>`.
+Run as `python -m conlludiff <json>`.
 
 The tool is configured through a JSON configuration file (example in `config_files/ssj_sst_upos.json`) where the user defines:
 - `file1` - The conllu file containing the first language sample
 - `file2` - The conllu file containing the second language sample
 - `event` - The linguistic feature the comparison is to be based on, optional events are form, lemma, upos, xpos, upos+feats, feat (each feature separately), feats (all features of a word merged), deprel, deprel+head_deprel
 - `filter` - The minimum p-value of the chi-square test for the entry to be filtered from the results
 - `fields` - A list of fields to be retained in the output (list of available values is listed below)
```

### Comparing `conlludiff-0.0.3/pyproject.toml` & `conlludiff-0.0.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "conlludiff"
-version = "0.0.3"
+version = "0.0.4"
 description = "Analyze two CONLLU files"
 readme = "README.md"
 authors = [{ name = "Peter Rupnik", email = "rupnikpeter@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
@@ -26,15 +26,15 @@
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest", "sphinx"]
 
 [project.urls]
 Homepage = "https://github.com/clarinsi/conllu-diff"
 
 
 [tool.bumpver]
-current_version = "0.0.3"
+current_version = "0.0.4"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `conlludiff-0.0.3/src/conlludiff/__main__.py` & `conlludiff-0.0.4/src/conlludiff/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,27 @@
-from conllu import parse_incr, parse
-import sys
-from scipy.stats import chi2_contingency
 import argparse
+import csv
 import importlib
+import logging
+import sys
+from collections import Counter
+from math import log, sqrt
+
+import numpy as np
+from conllu import parse, parse_incr
+from scipy.stats import chi2_contingency
 
 parser = argparse.ArgumentParser(description="")
 parser.add_argument("config", metavar="c", type=str, help="JSON configuration file")
 args = parser.parse_args()
 import json
 
 # from types import SimpleNamespace
 # config=json.load(open(args.config),object_hook=lambda d: SimpleNamespace(**d))
 config = json.load(open(args.config))
-from collections import Counter
-from math import sqrt, log
 
 predefined_events = {
     "form": lambda x: x["token"]["form"],
     "lemma": lambda x: x["token"]["lemma"],
     "upos": lambda x: x["token"]["upos"],
     "xpos": lambda x: x["token"]["xpos"],
     "upos+feats": lambda x: x["token"]["upos"]
@@ -89,49 +93,60 @@
     e2 = c2 * (f1 + f2) / (c1 + c2)
     try:
         return 2 * ((f1 * log(f1 / e1)) + (f2 * log(f2 / e2)))
     except:
         return
 
 
+invalid_counter = 0
 results = []
 for event in set(events1).union(set(events2)):
     f1 = events1.get(event, 0)
     f2 = events2.get(event, 0)
-    # try:
     test = chi2_contingency(((f1, c1 - f1), (f2, c2 - f2)))
-    # except:
-    #    continue
     or_result, or_direction = odds_ratio(f1, c1, f2, c2)
-    results.append(
-        {
-            "event": event,
-            "chisq": test[0],
-            "chisq_p": test[1],
-            "cramers_v": sqrt(test[0] / (c1 + c2)),
-            "odds_ratio": or_result,
-            "odds_ratio_direction": or_direction,
-            "llr": llr(f1, c1, f2, c2),
-            "contingency": ((f1, c1 - f1), (f2, c2 - f2)),
-        }
+    expected_f = list(np.append(*test.expected_freq))
+
+    # check if all expected frequencies are above 5
+    if any(y < 5 for y in expected_f):
+        invalid_counter += 1
+    else:
+        results.append(
+            {
+                "event": event,
+                "chisq": test[0],
+                "chisq_p": test[1],
+                "cramers_v": sqrt(test[0] / (c1 + c2)),
+                "odds_ratio": or_result,
+                "odds_ratio_direction": or_direction,
+                "llr": llr(f1, c1, f2, c2),
+                "contingency": ((f1, c1 - f1), (f2, c2 - f2)),
+            }
+        )
+
+if invalid_counter:
+    logging.warning(
+        f"{invalid_counter} events were not recorded since one or more expected values were "
+        f"less than 5"
     )
+
 # adam's wilcoxon
 # difference in relative frequency
 # craig's zetta (might need substructure
 # multiple feature extractors? a vs b
 
+# filter results
 if "filter" in config:
     results = [e for e in results if e["chisq_p"] < float(config["filter"])]
 if config["order"] in results[0]:
     results = sorted(
         results,
         key=lambda x: (x[config["order"]], x["event"]),
         reverse=config["reverse"],
     )
-import csv
 
 if config["output"] == "stdout":
     csvfile = sys.stdout
 else:
     csvfile = open(config["output"], "w")
 writer = csv.DictWriter(
     csvfile, config["fields"], delimiter="\t", extrasaction="ignore"
```

### Comparing `conlludiff-0.0.3/src/conlludiff/differ.py` & `conlludiff-0.0.4/src/conlludiff/differ.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import csv
 import sys
 from pathlib import Path
 from collections import Counter
 from conllu import parse_incr, parse
 from scipy.stats import chi2_contingency
 from math import sqrt, log, inf
-
+import logging
+import numpy as np
 
 predefined_events = {
     "form": lambda x: x["token"]["form"],
     "lemma": lambda x: x["token"]["lemma"],
     "upos": lambda x: x["token"]["upos"],
     "xpos": lambda x: x["token"]["xpos"],
     "upos+feats": lambda x: (
@@ -95,28 +96,30 @@
             "file2": file2,
             "event": event,
             "filter": filter,
             "fields": fields,
             "order": order,
             "reverse": reverse,
         }
+        if filter == None:
+            del self.config["filter"]
         self._run()
 
     def to_tsv(self, path: str | Path):
         """Export the results to tsv file
 
         Args:
             path (str | Path): Path to which results will be written
         """
         Path(path).write_text(self.results_string)
 
     def _run(self):
         config = self.config
-        if not config["filter"]:
-            config["filter"] = inf
+        # if not config["filter"]:
+        #     config["filter"] = inf
         if config["event"] in predefined_events:
             config["event_function"] = predefined_events[config["event"]]
         else:
             config["event_function"] = eval(config["event"])
 
         events1 = []
         with open(config["file1"], "r") as f:
@@ -162,48 +165,58 @@
             e1 = c1 * (f1 + f2) / (c1 + c2)
             e2 = c2 * (f1 + f2) / (c1 + c2)
             try:
                 return 2 * ((f1 * log(f1 / e1)) + (f2 * log(f2 / e2)))
             except:
                 return
 
+        invalid_counter = 0
         results = []
         for event in set(events1).union(set(events2)):
             f1 = events1.get(event, 0)
             f2 = events2.get(event, 0)
             # try:
             test = chi2_contingency(((f1, c1 - f1), (f2, c2 - f2)))
             # except:
             #    continue
             or_result, or_direction = odds_ratio(f1, c1, f2, c2)
-            results.append(
-                {
-                    "event": event,
-                    "chisq": test[0],
-                    "chisq_p": test[1],
-                    "cramers_v": sqrt(test[0] / (c1 + c2)),
-                    "odds_ratio": or_result,
-                    "odds_ratio_direction": or_direction,
-                    "llr": llr(f1, c1, f2, c2),
-                    "contingency": ((f1, c1 - f1), (f2, c2 - f2)),
-                }
+            expected_f = list(np.append(*test.expected_freq))
+            if any(y < 5 for y in expected_f):
+                invalid_counter += 1
+            else:
+                results.append(
+                    {
+                        "event": event,
+                        "chisq": test[0],
+                        "chisq_p": test[1],
+                        "cramers_v": sqrt(test[0] / (c1 + c2)),
+                        "odds_ratio": or_result,
+                        "odds_ratio_direction": or_direction,
+                        "llr": llr(f1, c1, f2, c2),
+                        "contingency": ((f1, c1 - f1), (f2, c2 - f2)),
+                    }
+                )
+        if invalid_counter:
+            logging.warning(
+                f"{invalid_counter} events were not recorded since {invalid_counter} values "
+                f"occured less than 5 times"
             )
         # adam's wilcoxon
         # difference in relative frequency
         # craig's zetta (might need substructure
         # multiple feature extractors? a vs b
 
-        if "filter" in config:
-            results = [e for e in results if e["chisq_p"] < float(config["filter"])]
         if config["order"] in results[0]:
             results = sorted(
                 results,
                 key=lambda x: (x[config["order"]], x["event"]),
                 reverse=config["reverse"],
             )
+        if "filter" in config:
+            results = [e for e in results if e["chisq_p"] < float(config["filter"])]
         self.results = [{f: i.get(f) for f in config["fields"]} for i in results]
         from contextlib import redirect_stdout
         import io
 
         f = io.StringIO()
         with redirect_stdout(f):
             writer = csv.DictWriter(
```

### Comparing `conlludiff-0.0.3/src/conlludiff.egg-info/PKG-INFO` & `conlludiff-0.0.4/src/conlludiff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conlludiff
-Version: 0.0.3
+Version: 0.0.4
 Summary: Analyze two CONLLU files
 Author-email: Peter Rupnik <rupnikpeter@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -234,15 +234,15 @@
 
 ```
 pip install conlludiff
 ```
 
 ## CLI use
 
-Run as `python conlludiff <json>`.
+Run as `python -m conlludiff <json>`.
 
 The tool is configured through a JSON configuration file (example in `config_files/ssj_sst_upos.json`) where the user defines:
 - `file1` - The conllu file containing the first language sample
 - `file2` - The conllu file containing the second language sample
 - `event` - The linguistic feature the comparison is to be based on, optional events are form, lemma, upos, xpos, upos+feats, feat (each feature separately), feats (all features of a word merged), deprel, deprel+head_deprel
 - `filter` - The minimum p-value of the chi-square test for the entry to be filtered from the results
 - `fields` - A list of fields to be retained in the output (list of available values is listed below)
```

### Comparing `conlludiff-0.0.3/src/docs/conf.py` & `conlludiff-0.0.4/src/docs/conf.py`

 * *Files identical despite different names*

