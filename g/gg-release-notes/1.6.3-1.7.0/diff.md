# Comparing `tmp/gg-release-notes-1.6.3.tar.gz` & `tmp/gg-release-notes-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gg-release-notes-1.6.3.tar", last modified: Tue Apr  2 08:53:49 2024, max compression
+gzip compressed data, was "gg-release-notes-1.7.0.tar", last modified: Tue Apr  2 09:08:45 2024, max compression
```

## Comparing `gg-release-notes-1.6.3.tar` & `gg-release-notes-1.7.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:53:49.235497 gg-release-notes-1.6.3/
--rw-rw-r--   0 rogier    (1000) rogier    (1000)     1066 2023-06-30 08:34:34.000000 gg-release-notes-1.6.3/LICENSE
--rw-rw-r--   0 rogier    (1000) rogier    (1000)     2947 2024-04-02 08:53:49.235497 gg-release-notes-1.6.3/PKG-INFO
--rw-rw-r--   0 rogier    (1000) rogier    (1000)     2593 2023-06-30 08:34:34.000000 gg-release-notes-1.6.3/README.md
--rw-rw-r--   0 rogier    (1000) rogier    (1000)       38 2024-04-02 08:53:49.235497 gg-release-notes-1.6.3/setup.cfg
--rw-rw-r--   0 rogier    (1000) rogier    (1000)      981 2024-04-02 08:53:27.000000 gg-release-notes-1.6.3/setup.py
-drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:53:49.235497 gg-release-notes-1.6.3/src/
-drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:53:49.235497 gg-release-notes-1.6.3/src/gg_release_notes/
--rw-rw-r--   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:36:47.000000 gg-release-notes-1.6.3/src/gg_release_notes/__init__.py
-drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:53:49.235497 gg-release-notes-1.6.3/src/gg_release_notes/config/
--rw-rw-r--   0 rogier    (1000) rogier    (1000)        0 2023-06-30 08:34:34.000000 gg-release-notes-1.6.3/src/gg_release_notes/config/__init__.py
--rw-rw-r--   0 rogier    (1000) rogier    (1000)      323 2024-04-02 08:49:26.000000 gg-release-notes-1.6.3/src/gg_release_notes/config/env_config.py
--rw-rw-r--   0 rogier    (1000) rogier    (1000)      596 2024-04-02 08:18:52.000000 gg-release-notes-1.6.3/src/gg_release_notes/config/github_config.py
--rw-rw-r--   0 rogier    (1000) rogier    (1000)     1520 2024-04-02 08:18:52.000000 gg-release-notes-1.6.3/src/gg_release_notes/config/prompt_config.py
--rw-rw-r--   0 rogier    (1000) rogier    (1000)     5004 2024-04-02 08:23:10.000000 gg-release-notes-1.6.3/src/gg_release_notes/generate_release_notes.py
--rw-rw-r--   0 rogier    (1000) rogier    (1000)     3815 2023-06-30 08:34:34.000000 gg-release-notes-1.6.3/src/gg_release_notes/pull_request.py
--rw-rw-r--   0 rogier    (1000) rogier    (1000)     4666 2024-04-02 08:18:53.000000 gg-release-notes-1.6.3/src/gg_release_notes/upload.py
-drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:53:49.235497 gg-release-notes-1.6.3/src/gg_release_notes/utils/
--rw-rw-r--   0 rogier    (1000) rogier    (1000)        0 2023-06-30 08:34:34.000000 gg-release-notes-1.6.3/src/gg_release_notes/utils/__init__.py
--rw-rw-r--   0 rogier    (1000) rogier    (1000)      422 2023-06-30 08:34:34.000000 gg-release-notes-1.6.3/src/gg_release_notes/utils/encode_bs64.py
--rw-rw-r--   0 rogier    (1000) rogier    (1000)     1842 2024-04-02 08:18:53.000000 gg-release-notes-1.6.3/src/gg_release_notes/version.py
-drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:53:49.235497 gg-release-notes-1.6.3/src/gg_release_notes.egg-info/
--rw-rw-r--   0 rogier    (1000) rogier    (1000)     2947 2024-04-02 08:53:49.000000 gg-release-notes-1.6.3/src/gg_release_notes.egg-info/PKG-INFO
--rw-rw-r--   0 rogier    (1000) rogier    (1000)      678 2024-04-02 08:53:49.000000 gg-release-notes-1.6.3/src/gg_release_notes.egg-info/SOURCES.txt
--rw-rw-r--   0 rogier    (1000) rogier    (1000)        1 2024-04-02 08:53:49.000000 gg-release-notes-1.6.3/src/gg_release_notes.egg-info/dependency_links.txt
--rw-rw-r--   0 rogier    (1000) rogier    (1000)      190 2024-04-02 08:53:49.000000 gg-release-notes-1.6.3/src/gg_release_notes.egg-info/requires.txt
--rw-rw-r--   0 rogier    (1000) rogier    (1000)       17 2024-04-02 08:53:49.000000 gg-release-notes-1.6.3/src/gg_release_notes.egg-info/top_level.txt
+drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 09:08:45.876325 gg-release-notes-1.7.0/
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)     1066 2023-06-30 08:34:34.000000 gg-release-notes-1.7.0/LICENSE
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)     2947 2024-04-02 09:08:45.876325 gg-release-notes-1.7.0/PKG-INFO
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)     2593 2023-06-30 08:34:34.000000 gg-release-notes-1.7.0/README.md
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)       38 2024-04-02 09:08:45.876325 gg-release-notes-1.7.0/setup.cfg
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)      981 2024-04-02 09:08:04.000000 gg-release-notes-1.7.0/setup.py
+drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 09:08:45.876325 gg-release-notes-1.7.0/src/
+drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 09:08:45.876325 gg-release-notes-1.7.0/src/gg_release_notes/
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:36:47.000000 gg-release-notes-1.7.0/src/gg_release_notes/__init__.py
+drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 09:08:45.876325 gg-release-notes-1.7.0/src/gg_release_notes/config/
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)        0 2023-06-30 08:34:34.000000 gg-release-notes-1.7.0/src/gg_release_notes/config/__init__.py
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)      323 2024-04-02 08:58:14.000000 gg-release-notes-1.7.0/src/gg_release_notes/config/env_config.py
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)      596 2024-04-02 08:18:52.000000 gg-release-notes-1.7.0/src/gg_release_notes/config/github_config.py
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)     1520 2024-04-02 08:18:52.000000 gg-release-notes-1.7.0/src/gg_release_notes/config/prompt_config.py
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)     5091 2024-04-02 09:07:48.000000 gg-release-notes-1.7.0/src/gg_release_notes/generate_release_notes.py
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)     3815 2023-06-30 08:34:34.000000 gg-release-notes-1.7.0/src/gg_release_notes/pull_request.py
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)     4666 2024-04-02 08:18:53.000000 gg-release-notes-1.7.0/src/gg_release_notes/upload.py
+drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 09:08:45.876325 gg-release-notes-1.7.0/src/gg_release_notes/utils/
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)        0 2023-06-30 08:34:34.000000 gg-release-notes-1.7.0/src/gg_release_notes/utils/__init__.py
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)      422 2023-06-30 08:34:34.000000 gg-release-notes-1.7.0/src/gg_release_notes/utils/encode_bs64.py
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)     1842 2024-04-02 08:18:53.000000 gg-release-notes-1.7.0/src/gg_release_notes/version.py
+drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 09:08:45.876325 gg-release-notes-1.7.0/src/gg_release_notes.egg-info/
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)     2947 2024-04-02 09:08:45.000000 gg-release-notes-1.7.0/src/gg_release_notes.egg-info/PKG-INFO
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)      678 2024-04-02 09:08:45.000000 gg-release-notes-1.7.0/src/gg_release_notes.egg-info/SOURCES.txt
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)        1 2024-04-02 09:08:45.000000 gg-release-notes-1.7.0/src/gg_release_notes.egg-info/dependency_links.txt
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)      190 2024-04-02 09:08:45.000000 gg-release-notes-1.7.0/src/gg_release_notes.egg-info/requires.txt
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)       17 2024-04-02 09:08:45.000000 gg-release-notes-1.7.0/src/gg_release_notes.egg-info/top_level.txt
```

### Comparing `gg-release-notes-1.6.3/LICENSE` & `gg-release-notes-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gg-release-notes-1.6.3/PKG-INFO` & `gg-release-notes-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gg-release-notes
-Version: 1.6.3
+Version: 1.7.0
 Summary: Python Interface for generating release notes for Github Actions
 Home-page: https://github.com/DataWiz40/gg-release-notes/
 Author: DataWiz40
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `gg-release-notes-1.6.3/README.md` & `gg-release-notes-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `gg-release-notes-1.6.3/setup.py` & `gg-release-notes-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 with open("./requirements-test.txt") as extra_requirements:
     EXTRA_REQUIRED = extra_requirements.read().split("\n")
 
 
 setup(
     name="gg-release-notes",
-    version="1.6.3",
+    version="1.7.0",
     description="Python Interface for generating release notes for Github Actions",
     url="https://github.com/DataWiz40/gg-release-notes/",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="DataWiz40",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
```

### Comparing `gg-release-notes-1.6.3/src/gg_release_notes/config/github_config.py` & `gg-release-notes-1.7.0/src/gg_release_notes/config/github_config.py`

 * *Files identical despite different names*

### Comparing `gg-release-notes-1.6.3/src/gg_release_notes/config/prompt_config.py` & `gg-release-notes-1.7.0/src/gg_release_notes/config/prompt_config.py`

 * *Files identical despite different names*

### Comparing `gg-release-notes-1.6.3/src/gg_release_notes/generate_release_notes.py` & `gg-release-notes-1.7.0/src/gg_release_notes/generate_release_notes.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,16 +17,17 @@
         **text_generation_params,
     ):
         self.env_config = env_config
         self.prompt_config = prompt_config
         self.prod_release_pr = prod_release_pr
         self.token_limit = token_limit
         self.text_genration_params = text_generation_params
-        openai.api_key = env_config.OPENAI_API_KEY
-        openai.organization = env_config.OPENAI_API_ORG
+        self.openai_client = openai.OpenAI(
+            api_key=env_config.OPENAI_API_KEY, organization=env_config.OPENAI_API_ORG
+        )
 
     def generate_release_notes(self, prompt: str) -> Any:
         """Generates release notes based on the issues and PR's in the Prod Release PR.
 
         Args:
             prompt (str): The prompt to use for the openai API
             prod_release_pr_number (str): The PR number of the prod release PR
@@ -37,15 +38,15 @@
         combined_release_notes = []
         batched_prompt, prompt_issues_descriptions = self._create_prompt_batches(5)
         for batch in batched_prompt:
             try:
                 print(f"Generating Prod Release for: \n{batch}")
                 # Assemble github titles for prompt
                 max_tokens = self.token_limit - len(prompt)
-                response = openai.chat.completions.create(
+                response = self.openai_client.chat.completions.create(
                     model=self.prompt_config.model,
                     messages=[
                         {"role": "system", "content": prompt},
                         {
                             "role": "user",
                             "content": "Generate release notes for the following PRs: \n"
                             + "\n".join(batch),
@@ -54,15 +55,17 @@
                     prompt=prompt,
                     max_tokens=max_tokens,
                     temperature=0.7,
                     n=1,
                     **self.text_genration_params,
                 )
                 combined_release_notes.append(
-                    response.get("choices", [{}])[0].get("message", {}).get("content", "NO RESPONSE")
+                    response.get("choices", [{}])[0]
+                    .get("message", {})
+                    .get("content", "NO RESPONSE")
                 )
             except Exception as e:
                 print(e)
                 continue
 
         response = (
             "\n\n"
```

### Comparing `gg-release-notes-1.6.3/src/gg_release_notes/pull_request.py` & `gg-release-notes-1.7.0/src/gg_release_notes/pull_request.py`

 * *Files identical despite different names*

### Comparing `gg-release-notes-1.6.3/src/gg_release_notes/upload.py` & `gg-release-notes-1.7.0/src/gg_release_notes/upload.py`

 * *Files identical despite different names*

### Comparing `gg-release-notes-1.6.3/src/gg_release_notes/version.py` & `gg-release-notes-1.7.0/src/gg_release_notes/version.py`

 * *Files identical despite different names*

### Comparing `gg-release-notes-1.6.3/src/gg_release_notes.egg-info/PKG-INFO` & `gg-release-notes-1.7.0/src/gg_release_notes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gg-release-notes
-Version: 1.6.3
+Version: 1.7.0
 Summary: Python Interface for generating release notes for Github Actions
 Home-page: https://github.com/DataWiz40/gg-release-notes/
 Author: DataWiz40
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `gg-release-notes-1.6.3/src/gg_release_notes.egg-info/SOURCES.txt` & `gg-release-notes-1.7.0/src/gg_release_notes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

