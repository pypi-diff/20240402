# Comparing `tmp/alita_tools-0.0.1.tar.gz` & `tmp/alita_tools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alita_tools-0.0.1.tar", last modified: Mon Apr  1 11:57:48 2024, max compression
+gzip compressed data, was "alita_tools-0.0.2.tar", last modified: Tue Apr  2 11:56:23 2024, max compression
```

## Comparing `alita_tools-0.0.1.tar` & `alita_tools-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-01 11:57:48.030000 alita_tools-0.0.1/
--rwx------   0 arozumenko   (501) staff       (20)    11357 2024-03-30 06:45:53.000000 alita_tools-0.0.1/LICENSE
--rwx------   0 arozumenko   (501) staff       (20)      968 2024-04-01 11:57:48.060000 alita_tools-0.0.1/PKG-INFO
--rwx------   0 arozumenko   (501) staff       (20)      102 2024-03-30 06:45:53.000000 alita_tools-0.0.1/README.md
--rwx------   0 arozumenko   (501) staff       (20)      809 2024-04-01 11:57:37.000000 alita_tools-0.0.1/pyproject.toml
--rwx------   0 arozumenko   (501) staff       (20)      138 2024-04-01 06:54:04.000000 alita_tools-0.0.1/requirements.txt
--rwx------   0 arozumenko   (501) staff       (20)       38 2024-04-01 11:57:48.070000 alita_tools-0.0.1/setup.cfg
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-01 11:57:48.030000 alita_tools-0.0.1/src/
--rwx------   0 arozumenko   (501) staff       (20)        0 2024-03-30 17:59:06.000000 alita_tools-0.0.1/src/__init__.py
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-01 11:57:48.030000 alita_tools-0.0.1/src/alita_tools/
--rwx------   0 arozumenko   (501) staff       (20)        0 2024-03-30 06:51:51.000000 alita_tools-0.0.1/src/alita_tools/__init__.py
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-01 11:57:48.030000 alita_tools-0.0.1/src/alita_tools/confluence/
--rwx------   0 arozumenko   (501) staff       (20)     1080 2024-04-01 07:44:04.000000 alita_tools-0.0.1/src/alita_tools/confluence/__init__.py
--rwx------   0 arozumenko   (501) staff       (20)    10523 2024-04-01 08:00:31.000000 alita_tools-0.0.1/src/alita_tools/confluence/api_wrapper.py
--rwx------   0 arozumenko   (501) staff       (20)      794 2024-04-01 07:42:41.000000 alita_tools-0.0.1/src/alita_tools/confluence/tool.py
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-01 11:57:48.040000 alita_tools-0.0.1/src/alita_tools/github/
--rwx------   0 arozumenko   (501) staff       (20)      807 2024-03-31 13:10:58.000000 alita_tools-0.0.1/src/alita_tools/github/__init__.py
--rwx------   0 arozumenko   (501) staff       (20)     3404 2024-03-31 13:14:48.000000 alita_tools-0.0.1/src/alita_tools/github/api_wrapper.py
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-01 11:57:48.030000 alita_tools-0.0.1/src/alita_tools.egg-info/
--rwx------   0 arozumenko   (501) staff       (20)      968 2024-04-01 11:57:48.000000 alita_tools-0.0.1/src/alita_tools.egg-info/PKG-INFO
--rwx------   0 arozumenko   (501) staff       (20)      476 2024-04-01 11:57:48.000000 alita_tools-0.0.1/src/alita_tools.egg-info/SOURCES.txt
--rwx------   0 arozumenko   (501) staff       (20)        1 2024-04-01 11:57:48.000000 alita_tools-0.0.1/src/alita_tools.egg-info/dependency_links.txt
--rwx------   0 arozumenko   (501) staff       (20)      139 2024-04-01 11:57:48.000000 alita_tools-0.0.1/src/alita_tools.egg-info/requires.txt
--rwx------   0 arozumenko   (501) staff       (20)       21 2024-04-01 11:57:48.000000 alita_tools-0.0.1/src/alita_tools.egg-info/top_level.txt
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-02 11:56:23.690000 alita_tools-0.0.2/
+-rwx------   0 arozumenko   (501) staff       (20)    11357 2024-03-30 06:45:53.000000 alita_tools-0.0.2/LICENSE
+-rwx------   0 arozumenko   (501) staff       (20)      968 2024-04-02 11:56:23.750000 alita_tools-0.0.2/PKG-INFO
+-rwx------   0 arozumenko   (501) staff       (20)      102 2024-03-30 06:45:53.000000 alita_tools-0.0.2/README.md
+-rwx------   0 arozumenko   (501) staff       (20)      809 2024-04-02 06:52:15.000000 alita_tools-0.0.2/pyproject.toml
+-rwx------   0 arozumenko   (501) staff       (20)      138 2024-04-01 06:54:04.000000 alita_tools-0.0.2/requirements.txt
+-rwx------   0 arozumenko   (501) staff       (20)       38 2024-04-02 11:56:23.750000 alita_tools-0.0.2/setup.cfg
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-02 11:56:23.690000 alita_tools-0.0.2/src/
+-rwx------   0 arozumenko   (501) staff       (20)        0 2024-03-30 17:59:06.000000 alita_tools-0.0.2/src/__init__.py
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-02 11:56:23.690000 alita_tools-0.0.2/src/alita_tools/
+-rwx------   0 arozumenko   (501) staff       (20)        0 2024-03-30 06:51:51.000000 alita_tools-0.0.2/src/alita_tools/__init__.py
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-02 11:56:23.700000 alita_tools-0.0.2/src/alita_tools/confluence/
+-rwx------   0 arozumenko   (501) staff       (20)     1083 2024-04-02 06:51:21.000000 alita_tools-0.0.2/src/alita_tools/confluence/__init__.py
+-rwx------   0 arozumenko   (501) staff       (20)    10955 2024-04-02 06:41:36.000000 alita_tools-0.0.2/src/alita_tools/confluence/api_wrapper.py
+-rwx------   0 arozumenko   (501) staff       (20)      794 2024-04-02 06:48:47.000000 alita_tools-0.0.2/src/alita_tools/confluence/tool.py
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-02 11:56:23.700000 alita_tools-0.0.2/src/alita_tools/github/
+-rwx------   0 arozumenko   (501) staff       (20)      979 2024-04-02 06:55:08.000000 alita_tools-0.0.2/src/alita_tools/github/__init__.py
+-rwx------   0 arozumenko   (501) staff       (20)    14849 2024-04-02 11:56:06.000000 alita_tools-0.0.2/src/alita_tools/github/api_wrapper.py
+-rwx------   0 arozumenko   (501) staff       (20)      907 2024-04-02 11:15:34.000000 alita_tools-0.0.2/src/alita_tools/github/tool.py
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-02 11:56:23.690000 alita_tools-0.0.2/src/alita_tools.egg-info/
+-rwx------   0 arozumenko   (501) staff       (20)      968 2024-04-02 11:56:23.000000 alita_tools-0.0.2/src/alita_tools.egg-info/PKG-INFO
+-rwx------   0 arozumenko   (501) staff       (20)      507 2024-04-02 11:56:23.000000 alita_tools-0.0.2/src/alita_tools.egg-info/SOURCES.txt
+-rwx------   0 arozumenko   (501) staff       (20)        1 2024-04-02 11:56:23.000000 alita_tools-0.0.2/src/alita_tools.egg-info/dependency_links.txt
+-rwx------   0 arozumenko   (501) staff       (20)      139 2024-04-02 11:56:23.000000 alita_tools-0.0.2/src/alita_tools.egg-info/requires.txt
+-rwx------   0 arozumenko   (501) staff       (20)       21 2024-04-02 11:56:23.000000 alita_tools-0.0.2/src/alita_tools.egg-info/top_level.txt
```

### Comparing `alita_tools-0.0.1/LICENSE` & `alita_tools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alita_tools-0.0.1/PKG-INFO` & `alita_tools-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alita_tools
-Version: 0.0.1
+Version: 0.0.2
 Summary: Default set of tools and toolkits available within ProjectAlita and CodeMie applications.
 Author-email: Artem Rozumenko <support@projectalita.ai>, Vadym Vlasenko <vadym_vlasenko@epam.com>
 Project-URL: Homepage, https://projectalita.ai
 Project-URL: Issues, https://github.com/ProjectAlita/application-tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `alita_tools-0.0.1/pyproject.toml` & `alita_tools-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alita_tools"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Artem Rozumenko", email="support@projectalita.ai" },
   { name="Vadym Vlasenko", email="vadym_vlasenko@epam.com"}
 ]
 description = "Default set of tools and toolkits available within ProjectAlita and CodeMie applications."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `alita_tools-0.0.1/src/alita_tools/confluence/__init__.py` & `alita_tools-0.0.2/src/alita_tools/confluence/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     @classmethod
     def get_toolkit(cls, selected_tools: list[str] = [], **kwargs):
         confluence_api_wrapper = ConfluenceAPIWrapper(**kwargs)
         available_tools = confluence_api_wrapper.get_available_tools()
         tools = []
         for tool in available_tools:
             if selected_tools:
-                if tool.name not in selected_tools:
+                if tool["name"] not in selected_tools:
                     continue
             tools.append(ConfluenceAction(
                 api_wrapper=confluence_api_wrapper,
                 name=tool["name"],
                 description=tool["description"],
                 args_schema=tool["args_schema"]
             ))
```

### Comparing `alita_tools-0.0.1/src/alita_tools/confluence/api_wrapper.py` & `alita_tools-0.0.2/src/alita_tools/confluence/api_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,27 +253,37 @@
 
         return texts
     
     def get_available_tools(self):
         return [
             {
                 "name": "create_page",
+                "ref": self.create_page,
                 "description": self.create_page.__doc__,
                 "args_schema": createPage,
             },
             {
                 "name": "page_exists",
+                "ref": self.page_exists,
                 "description": self.page_exists.__doc__,
                 "args_schema": pageExists,
             },
             {
                 "name": "get_pages_with_label",
+                "ref": self.get_pages_with_label,
                 "description": self.get_pages_with_label.__doc__,
                 "args_schema": getPagesWithLabel,
             },
             {
                 "name": "search_pages",
+                "ref": self.search_pages,
                 "description": self.search_pages.__doc__,
                 "args_schema": searchPages,
             }
         ]
-        
+    
+    def run(self, mode: str, *args: Any, **kwargs: Any):
+        for tool in self.get_available_tools():
+            if tool["name"] == mode:
+                return tool["ref"](*args, **kwargs)
+        else:
+            raise ValueError(f"Unknown mode: {mode}")
```

### Comparing `alita_tools-0.0.1/src/alita_tools/confluence/tool.py` & `alita_tools-0.0.2/src/alita_tools/confluence/tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,8 +19,8 @@
     def _run(
         self,
         *args: Any,
         run_manager: Optional[CallbackManagerForToolRun] = None,
         **kwargs: Any,
     ) -> str:
         """Use the Confluence API to run an operation."""
-        return self.api_wrapper.run(self.mode, *args, **kwargs)
+        return self.api_wrapper.run(self.name, *args, **kwargs)
```

### Comparing `alita_tools-0.0.1/src/alita_tools.egg-info/PKG-INFO` & `alita_tools-0.0.2/src/alita_tools.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alita_tools
-Version: 0.0.1
+Version: 0.0.2
 Summary: Default set of tools and toolkits available within ProjectAlita and CodeMie applications.
 Author-email: Artem Rozumenko <support@projectalita.ai>, Vadym Vlasenko <vadym_vlasenko@epam.com>
 Project-URL: Homepage, https://projectalita.ai
 Project-URL: Issues, https://github.com/ProjectAlita/application-tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

