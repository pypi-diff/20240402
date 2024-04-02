# Comparing `tmp/alita_tools-0.0.2.tar.gz` & `tmp/alita_tools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alita_tools-0.0.2.tar", last modified: Tue Apr  2 11:56:23 2024, max compression
+gzip compressed data, was "alita_tools-0.0.3.tar", last modified: Tue Apr  2 15:17:30 2024, max compression
```

## Comparing `alita_tools-0.0.2.tar` & `alita_tools-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,30 @@
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-02 11:56:23.690000 alita_tools-0.0.2/
--rwx------   0 arozumenko   (501) staff       (20)    11357 2024-03-30 06:45:53.000000 alita_tools-0.0.2/LICENSE
--rwx------   0 arozumenko   (501) staff       (20)      968 2024-04-02 11:56:23.750000 alita_tools-0.0.2/PKG-INFO
--rwx------   0 arozumenko   (501) staff       (20)      102 2024-03-30 06:45:53.000000 alita_tools-0.0.2/README.md
--rwx------   0 arozumenko   (501) staff       (20)      809 2024-04-02 06:52:15.000000 alita_tools-0.0.2/pyproject.toml
--rwx------   0 arozumenko   (501) staff       (20)      138 2024-04-01 06:54:04.000000 alita_tools-0.0.2/requirements.txt
--rwx------   0 arozumenko   (501) staff       (20)       38 2024-04-02 11:56:23.750000 alita_tools-0.0.2/setup.cfg
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-02 11:56:23.690000 alita_tools-0.0.2/src/
--rwx------   0 arozumenko   (501) staff       (20)        0 2024-03-30 17:59:06.000000 alita_tools-0.0.2/src/__init__.py
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-02 11:56:23.690000 alita_tools-0.0.2/src/alita_tools/
--rwx------   0 arozumenko   (501) staff       (20)        0 2024-03-30 06:51:51.000000 alita_tools-0.0.2/src/alita_tools/__init__.py
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-02 11:56:23.700000 alita_tools-0.0.2/src/alita_tools/confluence/
--rwx------   0 arozumenko   (501) staff       (20)     1083 2024-04-02 06:51:21.000000 alita_tools-0.0.2/src/alita_tools/confluence/__init__.py
--rwx------   0 arozumenko   (501) staff       (20)    10955 2024-04-02 06:41:36.000000 alita_tools-0.0.2/src/alita_tools/confluence/api_wrapper.py
--rwx------   0 arozumenko   (501) staff       (20)      794 2024-04-02 06:48:47.000000 alita_tools-0.0.2/src/alita_tools/confluence/tool.py
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-02 11:56:23.700000 alita_tools-0.0.2/src/alita_tools/github/
--rwx------   0 arozumenko   (501) staff       (20)      979 2024-04-02 06:55:08.000000 alita_tools-0.0.2/src/alita_tools/github/__init__.py
--rwx------   0 arozumenko   (501) staff       (20)    14849 2024-04-02 11:56:06.000000 alita_tools-0.0.2/src/alita_tools/github/api_wrapper.py
--rwx------   0 arozumenko   (501) staff       (20)      907 2024-04-02 11:15:34.000000 alita_tools-0.0.2/src/alita_tools/github/tool.py
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-02 11:56:23.690000 alita_tools-0.0.2/src/alita_tools.egg-info/
--rwx------   0 arozumenko   (501) staff       (20)      968 2024-04-02 11:56:23.000000 alita_tools-0.0.2/src/alita_tools.egg-info/PKG-INFO
--rwx------   0 arozumenko   (501) staff       (20)      507 2024-04-02 11:56:23.000000 alita_tools-0.0.2/src/alita_tools.egg-info/SOURCES.txt
--rwx------   0 arozumenko   (501) staff       (20)        1 2024-04-02 11:56:23.000000 alita_tools-0.0.2/src/alita_tools.egg-info/dependency_links.txt
--rwx------   0 arozumenko   (501) staff       (20)      139 2024-04-02 11:56:23.000000 alita_tools-0.0.2/src/alita_tools.egg-info/requires.txt
--rwx------   0 arozumenko   (501) staff       (20)       21 2024-04-02 11:56:23.000000 alita_tools-0.0.2/src/alita_tools.egg-info/top_level.txt
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-02 15:17:29.890000 alita_tools-0.0.3/
+-rwx------   0 arozumenko   (501) staff       (20)    11357 2024-03-30 06:45:53.000000 alita_tools-0.0.3/LICENSE
+-rwx------   0 arozumenko   (501) staff       (20)      968 2024-04-02 15:17:29.990000 alita_tools-0.0.3/PKG-INFO
+-rwx------   0 arozumenko   (501) staff       (20)      102 2024-03-30 06:45:53.000000 alita_tools-0.0.3/README.md
+-rwx------   0 arozumenko   (501) staff       (20)      809 2024-04-02 15:17:20.000000 alita_tools-0.0.3/pyproject.toml
+-rwx------   0 arozumenko   (501) staff       (20)      138 2024-04-01 06:54:04.000000 alita_tools-0.0.3/requirements.txt
+-rwx------   0 arozumenko   (501) staff       (20)       38 2024-04-02 15:17:30.000000 alita_tools-0.0.3/setup.cfg
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-02 15:17:29.890000 alita_tools-0.0.3/src/
+-rwx------   0 arozumenko   (501) staff       (20)        0 2024-03-30 17:59:06.000000 alita_tools-0.0.3/src/__init__.py
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-02 15:17:29.890000 alita_tools-0.0.3/src/alita_tools/
+-rwx------   0 arozumenko   (501) staff       (20)        0 2024-03-30 06:51:51.000000 alita_tools-0.0.3/src/alita_tools/__init__.py
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-02 15:17:29.890000 alita_tools-0.0.3/src/alita_tools/base/
+-rwx------   0 arozumenko   (501) staff       (20)        0 2024-04-02 14:42:43.000000 alita_tools-0.0.3/src/alita_tools/base/__init__.py
+-rwx------   0 arozumenko   (501) staff       (20)      719 2024-04-02 15:17:01.000000 alita_tools-0.0.3/src/alita_tools/base/tool.py
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-02 15:17:29.900000 alita_tools-0.0.3/src/alita_tools/confluence/
+-rwx------   0 arozumenko   (501) staff       (20)     1077 2024-04-02 14:44:26.000000 alita_tools-0.0.3/src/alita_tools/confluence/__init__.py
+-rwx------   0 arozumenko   (501) staff       (20)    10955 2024-04-02 06:41:36.000000 alita_tools-0.0.3/src/alita_tools/confluence/api_wrapper.py
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-02 15:17:29.900000 alita_tools-0.0.3/src/alita_tools/github/
+-rwx------   0 arozumenko   (501) staff       (20)      979 2024-04-02 06:55:08.000000 alita_tools-0.0.3/src/alita_tools/github/__init__.py
+-rwx------   0 arozumenko   (501) staff       (20)    14849 2024-04-02 14:45:38.000000 alita_tools-0.0.3/src/alita_tools/github/api_wrapper.py
+-rwx------   0 arozumenko   (501) staff       (20)      907 2024-04-02 11:15:34.000000 alita_tools-0.0.3/src/alita_tools/github/tool.py
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-02 15:17:29.900000 alita_tools-0.0.3/src/alita_tools/jira/
+-rwx------   0 arozumenko   (501) staff       (20)     1059 2024-04-02 14:44:32.000000 alita_tools-0.0.3/src/alita_tools/jira/__init__.py
+-rwx------   0 arozumenko   (501) staff       (20)    11386 2024-04-02 14:42:10.000000 alita_tools-0.0.3/src/alita_tools/jira/api_wrapper.py
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-02 15:17:29.890000 alita_tools-0.0.3/src/alita_tools.egg-info/
+-rwx------   0 arozumenko   (501) staff       (20)      968 2024-04-02 15:17:29.000000 alita_tools-0.0.3/src/alita_tools.egg-info/PKG-INFO
+-rwx------   0 arozumenko   (501) staff       (20)      603 2024-04-02 15:17:29.000000 alita_tools-0.0.3/src/alita_tools.egg-info/SOURCES.txt
+-rwx------   0 arozumenko   (501) staff       (20)        1 2024-04-02 15:17:29.000000 alita_tools-0.0.3/src/alita_tools.egg-info/dependency_links.txt
+-rwx------   0 arozumenko   (501) staff       (20)      139 2024-04-02 15:17:29.000000 alita_tools-0.0.3/src/alita_tools.egg-info/requires.txt
+-rwx------   0 arozumenko   (501) staff       (20)       21 2024-04-02 15:17:29.000000 alita_tools-0.0.3/src/alita_tools.egg-info/top_level.txt
```

### Comparing `alita_tools-0.0.2/LICENSE` & `alita_tools-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alita_tools-0.0.2/PKG-INFO` & `alita_tools-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alita_tools
-Version: 0.0.2
+Version: 0.0.3
 Summary: Default set of tools and toolkits available within ProjectAlita and CodeMie applications.
 Author-email: Artem Rozumenko <support@projectalita.ai>, Vadym Vlasenko <vadym_vlasenko@epam.com>
 Project-URL: Homepage, https://projectalita.ai
 Project-URL: Issues, https://github.com/ProjectAlita/application-tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `alita_tools-0.0.2/pyproject.toml` & `alita_tools-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alita_tools"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Artem Rozumenko", email="support@projectalita.ai" },
   { name="Vadym Vlasenko", email="vadym_vlasenko@epam.com"}
 ]
 description = "Default set of tools and toolkits available within ProjectAlita and CodeMie applications."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `alita_tools-0.0.2/src/alita_tools/confluence/__init__.py` & `alita_tools-0.0.3/src/alita_tools/confluence/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import Optional, List
 from langchain_core.pydantic_v1 import root_validator
 from langchain_community.agent_toolkits.base import BaseToolkit
 from .api_wrapper import ConfluenceAPIWrapper
 from langchain_core.tools import BaseTool
-from .tool import ConfluenceAction
+from ..base.tool import BaseAction
 
 
 class ConfluenceTookit(BaseToolkit):
     tools: List[BaseTool] = []
     
     @classmethod
     def get_toolkit(cls, selected_tools: list[str] = [], **kwargs):
         confluence_api_wrapper = ConfluenceAPIWrapper(**kwargs)
         available_tools = confluence_api_wrapper.get_available_tools()
         tools = []
         for tool in available_tools:
             if selected_tools:
                 if tool["name"] not in selected_tools:
                     continue
-            tools.append(ConfluenceAction(
+            tools.append(BaseAction(
                 api_wrapper=confluence_api_wrapper,
                 name=tool["name"],
                 description=tool["description"],
                 args_schema=tool["args_schema"]
             ))
         return cls(tools=tools)
```

### Comparing `alita_tools-0.0.2/src/alita_tools/confluence/api_wrapper.py` & `alita_tools-0.0.3/src/alita_tools/confluence/api_wrapper.py`

 * *Files identical despite different names*

### Comparing `alita_tools-0.0.2/src/alita_tools/github/__init__.py` & `alita_tools-0.0.3/src/alita_tools/github/__init__.py`

 * *Files identical despite different names*

### Comparing `alita_tools-0.0.2/src/alita_tools/github/api_wrapper.py` & `alita_tools-0.0.3/src/alita_tools/github/api_wrapper.py`

 * *Files identical despite different names*

### Comparing `alita_tools-0.0.2/src/alita_tools/github/tool.py` & `alita_tools-0.0.3/src/alita_tools/github/tool.py`

 * *Files identical despite different names*

### Comparing `alita_tools-0.0.2/src/alita_tools.egg-info/PKG-INFO` & `alita_tools-0.0.3/src/alita_tools.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alita_tools
-Version: 0.0.2
+Version: 0.0.3
 Summary: Default set of tools and toolkits available within ProjectAlita and CodeMie applications.
 Author-email: Artem Rozumenko <support@projectalita.ai>, Vadym Vlasenko <vadym_vlasenko@epam.com>
 Project-URL: Homepage, https://projectalita.ai
 Project-URL: Issues, https://github.com/ProjectAlita/application-tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

