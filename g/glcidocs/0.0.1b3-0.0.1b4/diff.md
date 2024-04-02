# Comparing `tmp/glcidocs-0.0.1b3.tar.gz` & `tmp/glcidocs-0.0.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glcidocs-0.0.1b3.tar", last modified: Mon Apr  1 18:59:26 2024, max compression
+gzip compressed data, was "glcidocs-0.0.1b4.tar", last modified: Tue Apr  2 21:34:13 2024, max compression
```

## Comparing `glcidocs-0.0.1b3.tar` & `glcidocs-0.0.1b4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 18:59:26.808100 glcidocs-0.0.1b3/
--rw-rw-rw-   0        0        0     1092 2024-03-29 11:49:25.000000 glcidocs-0.0.1b3/LICENSE
--rw-rw-rw-   0        0        0       25 2024-04-01 16:26:26.000000 glcidocs-0.0.1b3/MANIFEST.in
--rw-rw-rw-   0        0        0     3801 2024-04-01 18:59:26.808100 glcidocs-0.0.1b3/PKG-INFO
--rw-rw-rw-   0        0        0     3225 2024-04-01 16:26:26.000000 glcidocs-0.0.1b3/README.md
--rw-rw-rw-   0        0        0       88 2024-04-01 16:26:26.000000 glcidocs-0.0.1b3/pyproject.toml
--rw-rw-rw-   0        0        0      804 2024-04-01 18:59:26.808100 glcidocs-0.0.1b3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-01 18:59:26.776858 glcidocs-0.0.1b3/src/
-drwxrwxrwx   0        0        0        0 2024-04-01 18:59:26.792487 glcidocs-0.0.1b3/src/glcidocs/
--rw-rw-rw-   0        0        0     1545 2024-04-01 18:52:08.000000 glcidocs-0.0.1b3/src/glcidocs/__init__.py
--rw-rw-rw-   0        0        0      492 2024-04-01 18:52:01.000000 glcidocs-0.0.1b3/src/glcidocs/__main__.py
--rw-rw-rw-   0        0        0     2105 2024-04-01 16:26:26.000000 glcidocs-0.0.1b3/src/glcidocs/docsgen.py
--rw-rw-rw-   0        0        0       86 2024-04-01 16:26:26.000000 glcidocs-0.0.1b3/src/glcidocs/errors.py
--rw-rw-rw-   0        0        0     3796 2024-04-01 18:54:18.000000 glcidocs-0.0.1b3/src/glcidocs/pipelineparser.py
-drwxrwxrwx   0        0        0        0 2024-04-01 18:59:26.808100 glcidocs-0.0.1b3/src/glcidocs.egg-info/
--rw-rw-rw-   0        0        0     3801 2024-04-01 18:59:26.000000 glcidocs-0.0.1b3/src/glcidocs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2024-04-01 18:59:26.000000 glcidocs-0.0.1b3/src/glcidocs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 18:59:26.000000 glcidocs-0.0.1b3/src/glcidocs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-01 16:26:53.000000 glcidocs-0.0.1b3/src/glcidocs.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2024-04-01 18:59:26.000000 glcidocs-0.0.1b3/src/glcidocs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-01 18:59:26.000000 glcidocs-0.0.1b3/src/glcidocs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 21:34:13.711354 glcidocs-0.0.1b4/
+-rw-rw-rw-   0        0        0     1092 2024-03-29 11:49:25.000000 glcidocs-0.0.1b4/LICENSE
+-rw-rw-rw-   0        0        0       25 2024-04-01 16:26:26.000000 glcidocs-0.0.1b4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3801 2024-04-02 21:34:13.711354 glcidocs-0.0.1b4/PKG-INFO
+-rw-rw-rw-   0        0        0     3225 2024-04-01 16:26:26.000000 glcidocs-0.0.1b4/README.md
+-rw-rw-rw-   0        0        0       88 2024-04-01 16:26:26.000000 glcidocs-0.0.1b4/pyproject.toml
+-rw-rw-rw-   0        0        0      804 2024-04-02 21:34:13.726975 glcidocs-0.0.1b4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-02 21:34:13.680136 glcidocs-0.0.1b4/src/
+drwxrwxrwx   0        0        0        0 2024-04-02 21:34:13.711354 glcidocs-0.0.1b4/src/glcidocs/
+-rw-rw-rw-   0        0        0     1545 2024-04-02 21:33:48.000000 glcidocs-0.0.1b4/src/glcidocs/__init__.py
+-rw-rw-rw-   0        0        0      492 2024-04-01 18:52:01.000000 glcidocs-0.0.1b4/src/glcidocs/__main__.py
+-rw-rw-rw-   0        0        0     2105 2024-04-01 16:26:26.000000 glcidocs-0.0.1b4/src/glcidocs/docsgen.py
+-rw-rw-rw-   0        0        0       86 2024-04-01 16:26:26.000000 glcidocs-0.0.1b4/src/glcidocs/errors.py
+-rw-rw-rw-   0        0        0     4067 2024-04-02 21:32:51.000000 glcidocs-0.0.1b4/src/glcidocs/pipelineparser.py
+drwxrwxrwx   0        0        0        0 2024-04-02 21:34:13.711354 glcidocs-0.0.1b4/src/glcidocs.egg-info/
+-rw-rw-rw-   0        0        0     3801 2024-04-02 21:34:13.000000 glcidocs-0.0.1b4/src/glcidocs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2024-04-02 21:34:13.000000 glcidocs-0.0.1b4/src/glcidocs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 21:34:13.000000 glcidocs-0.0.1b4/src/glcidocs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-01 16:26:53.000000 glcidocs-0.0.1b4/src/glcidocs.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2024-04-02 21:34:13.000000 glcidocs-0.0.1b4/src/glcidocs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-02 21:34:13.000000 glcidocs-0.0.1b4/src/glcidocs.egg-info/top_level.txt
```

### Comparing `glcidocs-0.0.1b3/LICENSE` & `glcidocs-0.0.1b4/LICENSE`

 * *Files identical despite different names*

### Comparing `glcidocs-0.0.1b3/PKG-INFO` & `glcidocs-0.0.1b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glcidocs
-Version: 0.0.1b3
+Version: 0.0.1b4
 Summary: Simple generator of gitlab ci file documentation
 Home-page: https://github.com/martin356/gitlab-ci-docs
 Author: Martin Mudroch
 Author-email: martin.mudroch@proton.me
 License: MIT
 Keywords: gitlab,pipeline,documentation,ci/cd,gitlab-ci
 Classifier: Programming Language :: Python :: 3
```

### Comparing `glcidocs-0.0.1b3/README.md` & `glcidocs-0.0.1b4/README.md`

 * *Files identical despite different names*

### Comparing `glcidocs-0.0.1b3/setup.cfg` & `glcidocs-0.0.1b4/setup.cfg`

 * *Files identical despite different names*

### Comparing `glcidocs-0.0.1b3/src/glcidocs/__init__.py` & `glcidocs-0.0.1b4/src/glcidocs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 from pathlib import Path
 from typing import List
 from glcidocs.pipelineparser import CiFileParser
 from glcidocs.docsgen import HTMLBuilder
 
 
-__version__ = '0.0.1-beta.3'
+__version__ = '0.0.1-beta.4'
 
 
 def read_doc_file(file_path: str|Path) -> List[str]:
     with open(file_path, 'r') as f:
         return [line for line in f]
```

### Comparing `glcidocs-0.0.1b3/src/glcidocs/docsgen.py` & `glcidocs-0.0.1b4/src/glcidocs/docsgen.py`

 * *Files identical despite different names*

### Comparing `glcidocs-0.0.1b3/src/glcidocs/pipelineparser.py` & `glcidocs-0.0.1b4/src/glcidocs/pipelineparser.py`

 * *Files 9% similar despite different names*

```diff
@@ -74,17 +74,17 @@
         self._pipeline_name = ''
         self._condition = rule['if']
         self._variables = [
             Variable(
                 name=key,
                 value=rule['variables'][key],
                 comment=c[2].value if (c := rule['variables'].ca.items.get(key, None)) else ''
-            ) for key in rule['variables'] if key != '_PIPELINE_NAME'
+            ) for key in rule.get('variables', {}) if key != '_PIPELINE_NAME'
         ]
-        self._pipeline_name = rule['variables'].get('_PIPELINE_NAME', '')
+        self._pipeline_name = rule.get('variables').get('_PIPELINE_NAME', '')
 
     @property
     def condition(self) -> str:
         return self._condition
 
     @property
     def variables(self) -> List[Variable]:
@@ -93,17 +93,23 @@
     @property
     def pipeline_name(self) -> str:
         return self._pipeline_name
 
 
 class Workflow:
 
+    _regex_pipeline_source = '\$CI_PIPELINE_SOURCE\s==\s[\'"]?(web|pipeline|api|trigger)[\'"]?'
+
+    @classmethod
+    def _include_rule(cls, rule_if: str) -> bool:
+        return bool(re.search(cls._regex_pipeline_source, rule_if))
+
     def __init__(self, workflow: Dict):
-        self._pipeline_name = workflow.get('PIPELINE_NAME', None)
-        self._rules = [Rule(r) for r in workflow['rules']]
+        self._pipeline_name = workflow.get('name', '')
+        self._rules = [Rule(r) for r in workflow['rules'] if self._include_rule(r['if'])]
 
     @property
     def rules(self) -> List[Rule]:
         return self._rules
 
     @property
     def pipeline_name(self) -> str:
```

### Comparing `glcidocs-0.0.1b3/src/glcidocs.egg-info/PKG-INFO` & `glcidocs-0.0.1b4/src/glcidocs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glcidocs
-Version: 0.0.1b3
+Version: 0.0.1b4
 Summary: Simple generator of gitlab ci file documentation
 Home-page: https://github.com/martin356/gitlab-ci-docs
 Author: Martin Mudroch
 Author-email: martin.mudroch@proton.me
 License: MIT
 Keywords: gitlab,pipeline,documentation,ci/cd,gitlab-ci
 Classifier: Programming Language :: Python :: 3
```

