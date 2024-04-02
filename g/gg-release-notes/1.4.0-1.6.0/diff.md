# Comparing `tmp/gg-release-notes-1.4.0.tar.gz` & `tmp/gg-release-notes-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gg-release-notes-1.4.0.tar", last modified: Tue Mar 26 12:45:55 2024, max compression
+gzip compressed data, was "gg-release-notes-1.6.0.tar", last modified: Tue Apr  2 08:37:01 2024, max compression
```

## Comparing `gg-release-notes-1.4.0.tar` & `gg-release-notes-1.6.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-03-26 12:45:55.232220 gg-release-notes-1.4.0/
--rw-rw-r--   0 rogier    (1000) rogier    (1000)     1066 2023-06-30 08:34:34.000000 gg-release-notes-1.4.0/LICENSE
--rw-rw-r--   0 rogier    (1000) rogier    (1000)     2947 2024-03-26 12:45:55.232220 gg-release-notes-1.4.0/PKG-INFO
--rw-rw-r--   0 rogier    (1000) rogier    (1000)     2593 2023-06-30 08:34:34.000000 gg-release-notes-1.4.0/README.md
--rw-rw-r--   0 rogier    (1000) rogier    (1000)       38 2024-03-26 12:45:55.232220 gg-release-notes-1.4.0/setup.cfg
--rw-rw-r--   0 rogier    (1000) rogier    (1000)     1121 2023-06-30 08:34:34.000000 gg-release-notes-1.4.0/setup.py
-drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-03-26 12:45:55.232220 gg-release-notes-1.4.0/src/
-drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-03-26 12:45:55.232220 gg-release-notes-1.4.0/src/gg_release_notes/
--rw-rw-r--   0 rogier    (1000) rogier    (1000)       21 2024-03-26 12:40:56.000000 gg-release-notes-1.4.0/src/gg_release_notes/__init__.py
-drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-03-26 12:45:55.232220 gg-release-notes-1.4.0/src/gg_release_notes/config/
--rw-rw-r--   0 rogier    (1000) rogier    (1000)        0 2023-06-30 08:34:34.000000 gg-release-notes-1.4.0/src/gg_release_notes/config/__init__.py
--rw-rw-r--   0 rogier    (1000) rogier    (1000)      306 2023-06-30 08:34:34.000000 gg-release-notes-1.4.0/src/gg_release_notes/config/env_config.py
--rw-rw-r--   0 rogier    (1000) rogier    (1000)      549 2023-06-30 08:34:34.000000 gg-release-notes-1.4.0/src/gg_release_notes/config/github_config.py
--rw-rw-r--   0 rogier    (1000) rogier    (1000)     1506 2024-03-26 11:07:42.000000 gg-release-notes-1.4.0/src/gg_release_notes/config/prompt_config.py
--rw-rw-r--   0 rogier    (1000) rogier    (1000)     4619 2024-03-26 12:36:32.000000 gg-release-notes-1.4.0/src/gg_release_notes/generate_release_notes.py
--rw-rw-r--   0 rogier    (1000) rogier    (1000)     3815 2023-06-30 08:34:34.000000 gg-release-notes-1.4.0/src/gg_release_notes/pull_request.py
--rw-rw-r--   0 rogier    (1000) rogier    (1000)     4678 2023-06-30 08:34:34.000000 gg-release-notes-1.4.0/src/gg_release_notes/upload.py
-drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-03-26 12:45:55.232220 gg-release-notes-1.4.0/src/gg_release_notes/utils/
--rw-rw-r--   0 rogier    (1000) rogier    (1000)        0 2023-06-30 08:34:34.000000 gg-release-notes-1.4.0/src/gg_release_notes/utils/__init__.py
--rw-rw-r--   0 rogier    (1000) rogier    (1000)      422 2023-06-30 08:34:34.000000 gg-release-notes-1.4.0/src/gg_release_notes/utils/encode_bs64.py
--rw-rw-r--   0 rogier    (1000) rogier    (1000)     1862 2023-06-30 08:34:34.000000 gg-release-notes-1.4.0/src/gg_release_notes/version.py
-drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-03-26 12:45:55.232220 gg-release-notes-1.4.0/src/gg_release_notes.egg-info/
--rw-rw-r--   0 rogier    (1000) rogier    (1000)     2947 2024-03-26 12:45:55.000000 gg-release-notes-1.4.0/src/gg_release_notes.egg-info/PKG-INFO
--rw-rw-r--   0 rogier    (1000) rogier    (1000)      678 2024-03-26 12:45:55.000000 gg-release-notes-1.4.0/src/gg_release_notes.egg-info/SOURCES.txt
--rw-rw-r--   0 rogier    (1000) rogier    (1000)        1 2024-03-26 12:45:55.000000 gg-release-notes-1.4.0/src/gg_release_notes.egg-info/dependency_links.txt
--rw-rw-r--   0 rogier    (1000) rogier    (1000)      165 2024-03-26 12:45:55.000000 gg-release-notes-1.4.0/src/gg_release_notes.egg-info/requires.txt
--rw-rw-r--   0 rogier    (1000) rogier    (1000)       17 2024-03-26 12:45:55.000000 gg-release-notes-1.4.0/src/gg_release_notes.egg-info/top_level.txt
+drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:37:01.440134 gg-release-notes-1.6.0/
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)     1066 2023-06-30 08:34:34.000000 gg-release-notes-1.6.0/LICENSE
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)     2947 2024-04-02 08:37:01.440134 gg-release-notes-1.6.0/PKG-INFO
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)     2593 2023-06-30 08:34:34.000000 gg-release-notes-1.6.0/README.md
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)       38 2024-04-02 08:37:01.440134 gg-release-notes-1.6.0/setup.cfg
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)      981 2024-04-02 08:36:44.000000 gg-release-notes-1.6.0/setup.py
+drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:37:01.440134 gg-release-notes-1.6.0/src/
+drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:37:01.440134 gg-release-notes-1.6.0/src/gg_release_notes/
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:36:47.000000 gg-release-notes-1.6.0/src/gg_release_notes/__init__.py
+drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:37:01.440134 gg-release-notes-1.6.0/src/gg_release_notes/config/
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)        0 2023-06-30 08:34:34.000000 gg-release-notes-1.6.0/src/gg_release_notes/config/__init__.py
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)      306 2023-06-30 08:34:34.000000 gg-release-notes-1.6.0/src/gg_release_notes/config/env_config.py
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)      596 2024-04-02 08:18:52.000000 gg-release-notes-1.6.0/src/gg_release_notes/config/github_config.py
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)     1520 2024-04-02 08:18:52.000000 gg-release-notes-1.6.0/src/gg_release_notes/config/prompt_config.py
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)     5004 2024-04-02 08:23:10.000000 gg-release-notes-1.6.0/src/gg_release_notes/generate_release_notes.py
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)     3815 2023-06-30 08:34:34.000000 gg-release-notes-1.6.0/src/gg_release_notes/pull_request.py
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)     4666 2024-04-02 08:18:53.000000 gg-release-notes-1.6.0/src/gg_release_notes/upload.py
+drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:37:01.440134 gg-release-notes-1.6.0/src/gg_release_notes/utils/
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)        0 2023-06-30 08:34:34.000000 gg-release-notes-1.6.0/src/gg_release_notes/utils/__init__.py
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)      422 2023-06-30 08:34:34.000000 gg-release-notes-1.6.0/src/gg_release_notes/utils/encode_bs64.py
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)     1842 2024-04-02 08:18:53.000000 gg-release-notes-1.6.0/src/gg_release_notes/version.py
+drwxrwxr-x   0 rogier    (1000) rogier    (1000)        0 2024-04-02 08:37:01.440134 gg-release-notes-1.6.0/src/gg_release_notes.egg-info/
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)     2947 2024-04-02 08:37:01.000000 gg-release-notes-1.6.0/src/gg_release_notes.egg-info/PKG-INFO
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)      678 2024-04-02 08:37:01.000000 gg-release-notes-1.6.0/src/gg_release_notes.egg-info/SOURCES.txt
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)        1 2024-04-02 08:37:01.000000 gg-release-notes-1.6.0/src/gg_release_notes.egg-info/dependency_links.txt
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)      187 2024-04-02 08:37:01.000000 gg-release-notes-1.6.0/src/gg_release_notes.egg-info/requires.txt
+-rw-rw-r--   0 rogier    (1000) rogier    (1000)       17 2024-04-02 08:37:01.000000 gg-release-notes-1.6.0/src/gg_release_notes.egg-info/top_level.txt
```

### Comparing `gg-release-notes-1.4.0/LICENSE` & `gg-release-notes-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gg-release-notes-1.4.0/PKG-INFO` & `gg-release-notes-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gg-release-notes
-Version: 1.4.0
+Version: 1.6.0
 Summary: Python Interface for generating release notes for Github Actions
 Home-page: https://github.com/DataWiz40/gg-release-notes/
 Author: DataWiz40
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `gg-release-notes-1.4.0/README.md` & `gg-release-notes-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `gg-release-notes-1.4.0/setup.py` & `gg-release-notes-1.6.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 """Python setup.py for project_name package"""
 import os
 from setuptools import find_packages, setup
 
 
-with open('./README.md', 'r', encoding='utf-8') as fh:
+with open("./README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 print(os.getcwd())
 
 # What packages are required for this module to be executed?
 with open("./requirements.txt") as requirements:
     REQUIRED = requirements.read().split("\n")
 
 with open("./requirements-test.txt") as extra_requirements:
     EXTRA_REQUIRED = extra_requirements.read().split("\n")
 
-with open("./src/gg_release_notes/__init__.py") as f:
-    release_notes_version = f.read().split("=")[1].strip().strip("'")
-
 
 setup(
     name="gg-release-notes",
-    version=release_notes_version,
+    version="1.6.0",
     description="Python Interface for generating release notes for Github Actions",
     url="https://github.com/DataWiz40/gg-release-notes/",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="DataWiz40",
-    package_dir={'': 'src'},
-    packages=find_packages(where='src'),
-    python_requires='>=3.6',
+    package_dir={"": "src"},
+    packages=find_packages(where="src"),
+    python_requires=">=3.6",
     install_requires=REQUIRED,
-    extras_require={"test": EXTRA_REQUIRED },
+    extras_require={"test": EXTRA_REQUIRED},
 )
```

### Comparing `gg-release-notes-1.4.0/src/gg_release_notes/config/github_config.py` & `gg-release-notes-1.6.0/src/gg_release_notes/config/github_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,21 @@
 
 from gg_release_notes.config.env_config import EnvConfig
 
 
 class GithubAPIConfig:
     """Wrapper for Github API"""
 
-    def __init__(self, owner: str, repository: str, env_config: EnvConfig, github_prod_release_label: str = "prod-release"):
+    def __init__(
+        self,
+        owner: str,
+        repository: str,
+        env_config: EnvConfig,
+        github_prod_release_label: str = "prod-release",
+    ):
         self.owner = owner
         self.repository = repository
         self.github_api = GhApi(
             owner=owner,
             repo=repository,
             token=env_config.ENV_GITHUB_API_TOKEN,
         )
```

### Comparing `gg-release-notes-1.4.0/src/gg_release_notes/config/prompt_config.py` & `gg-release-notes-1.6.0/src/gg_release_notes/config/prompt_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from gg_release_notes.version import ReleaseVersion
 from gg_release_notes.config.github_config import GithubAPIConfig
 
 
 class PromptConfig:
     """Prompt configuration used for the GPT generation"""
 
-    def __init__(self, github_config: GithubAPIConfig, model: str = "gpt-4-0125-preview"):
+    def __init__(
+        self, github_config: GithubAPIConfig, model: str = "gpt-4-0125-preview"
+    ):
         """s
 
         Args:
             github_config (GithubAPIConfig): Github configuration
         """
         self.github_config = github_config
         self.release_version = ReleaseVersion(github_config)
```

### Comparing `gg-release-notes-1.4.0/src/gg_release_notes/generate_release_notes.py` & `gg-release-notes-1.6.0/src/gg_release_notes/generate_release_notes.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 class ReleaseNotes:
     def __init__(
         self,
         env_config: EnvConfig,
         prompt_config: PromptConfig,
         prod_release_pr: ProdReleasePR,
-        token_limit: int = 2000,
+        token_limit: int = 10000,
         **text_generation_params,
     ):
         self.env_config = env_config
         self.prompt_config = prompt_config
         self.prod_release_pr = prod_release_pr
         self.token_limit = token_limit
         self.text_genration_params = text_generation_params
@@ -36,25 +36,34 @@
 
         combined_release_notes = []
         batched_prompt, prompt_issues_descriptions = self._create_prompt_batches(5)
         for batch in batched_prompt:
             try:
                 print(f"Generating Prod Release for: \n{batch}")
                 # Assemble github titles for prompt
-                prompt = f"{prompt} {','.join(batch)}"
                 max_tokens = self.token_limit - len(prompt)
-                response = openai.Completion.create(
+                response = openai.chat.completions.create(
                     model=self.prompt_config.model,
+                    messages=[
+                        {"role": "system", "content": prompt},
+                        {
+                            "role": "user",
+                            "content": "Generate release notes for the following PRs: \n"
+                            + "\n".join(batch),
+                        },
+                    ],
                     prompt=prompt,
                     max_tokens=max_tokens,
                     temperature=0.7,
                     n=1,
                     **self.text_genration_params,
                 )
-                combined_release_notes.append(response.get("choices")[0].get("text"))
+                combined_release_notes.append(
+                    response.get("choices", [{}])[0].get("message", {}).get("content", "NO RESPONSE")
+                )
             except Exception as e:
                 print(e)
                 continue
 
         response = (
             "\n\n"
             + self.prompt_config.release_notes_start_text
```

### Comparing `gg-release-notes-1.4.0/src/gg_release_notes/pull_request.py` & `gg-release-notes-1.6.0/src/gg_release_notes/pull_request.py`

 * *Files identical despite different names*

### Comparing `gg-release-notes-1.4.0/src/gg_release_notes/upload.py` & `gg-release-notes-1.6.0/src/gg_release_notes/upload.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         )
         return update_req
 
     def make_github_release(self, versioning_type: Optional[str]):
         """Creates a release in Github using Github API."""
         if not versioning_type:
             versioning_type = str(self.prod_release_pr.requested_new_version_type())
-            
+
         new_version = self.prod_release_version.increment_version(
             self.prod_release_version.current_version, versioning_type=versioning_type
         )
         self.github_api.repos.create_release(
             tag_name=new_version,
             name=self.release_title,
             body=self.release_payload.get("body", ""),
```

### Comparing `gg-release-notes-1.4.0/src/gg_release_notes/version.py` & `gg-release-notes-1.6.0/src/gg_release_notes/version.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,29 +28,29 @@
         """Gets the current version number of the release."""
         try:
             release_req = self.github_api.repos.get_latest_release()
             version = release_req.get("tag_name", "1.0.0")
         except:
             # No release exists yet
             version = "1.0.0"
-        
+
         return str(version)
 
     def increment_version(
         self, current_version: str, versioning_type: Optional[str]
     ) -> str:
         """Increments the version number of the current release."""
         print(f"Current version: {current_version}")
         # Remove the 'v' from the version number
         if current_version.startswith("v."):
             current_version = current_version[2:]
-            
-        version_parts = list(map(int, current_version.split('.')))
-        if str(versioning_type).lower() == 'major':
+
+        version_parts = list(map(int, current_version.split(".")))
+        if str(versioning_type).lower() == "major":
             version_parts[0] += 1
             version_parts[1], version_parts[2] = 0, 0
-        elif str(versioning_type).lower() == 'minor':
+        elif str(versioning_type).lower() == "minor":
             version_parts[1] += 1
             version_parts[2] = 0
         else:
             version_parts[2] += 1
-        return '.'.join(map(str, version_parts))
+        return ".".join(map(str, version_parts))
```

### Comparing `gg-release-notes-1.4.0/src/gg_release_notes.egg-info/PKG-INFO` & `gg-release-notes-1.6.0/src/gg_release_notes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gg-release-notes
-Version: 1.4.0
+Version: 1.6.0
 Summary: Python Interface for generating release notes for Github Actions
 Home-page: https://github.com/DataWiz40/gg-release-notes/
 Author: DataWiz40
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `gg-release-notes-1.4.0/src/gg_release_notes.egg-info/SOURCES.txt` & `gg-release-notes-1.6.0/src/gg_release_notes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

