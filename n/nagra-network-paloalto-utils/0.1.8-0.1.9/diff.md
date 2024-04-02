# Comparing `tmp/nagra_network_paloalto_utils-0.1.8.tar.gz` & `tmp/nagra_network_paloalto_utils-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nagra_network_paloalto_utils-0.1.8.tar", max compression
+gzip compressed data, was "nagra_network_paloalto_utils-0.1.9.tar", max compression
```

## Comparing `nagra_network_paloalto_utils-0.1.8.tar` & `nagra_network_paloalto_utils-0.1.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0       37 2023-12-12 10:51:18.074169 nagra_network_paloalto_utils-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-12-15 17:18:47.633258 nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/__init__.py
--rw-r--r--   0        0        0      335 2023-12-12 10:51:18.074169 nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/__main__.py
--rw-r--r--   0        0        0     1484 2023-12-13 10:15:42.581231 nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/commands/__init__.py
--rw-r--r--   0        0        0      759 2023-12-12 10:51:18.074169 nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/commands/git_writer.py
--rw-r--r--   0        0        0      674 2023-12-15 16:47:07.749416 nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/commands/panorama/__init__.py
--rw-r--r--   0        0        0      343 2023-12-12 10:51:18.074169 nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/commands/panorama/objects/__init__.py
--rw-r--r--   0        0        0     4455 2023-12-12 10:51:18.078169 nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/commands/panorama/objects/addresses.py
--rw-r--r--   0        0        0      962 2023-12-12 10:51:18.078169 nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/commands/panorama/objects/applications.py
--rw-r--r--   0        0        0     2494 2023-12-12 10:51:18.078169 nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/commands/panorama/objects/services.py
--rw-r--r--   0        0        0     2294 2023-12-12 10:51:18.078169 nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/commands/panorama/objects/tags.py
--rw-r--r--   0        0        0     3501 2023-12-15 17:18:47.393257 nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/commands/panorama/panorama.py
--rw-r--r--   0        0        0      145 2023-12-12 10:51:18.078169 nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/commands/terraform/__init__.py
--rw-r--r--   0        0        0     1070 2023-12-13 10:15:42.581231 nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/commands/terraform/object_deletion_checker.py
--rw-r--r--   0        0        0      191 2023-12-12 10:51:18.078169 nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/commands/yaml/__init__.py
--rw-r--r--   0        0        0     2730 2023-12-12 10:51:18.078169 nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/commands/yaml/checks.py
--rw-r--r--   0        0        0     1402 2023-12-12 10:51:18.082169 nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/commands/yaml/indexes.py
--rw-r--r--   0        0        0        0 2023-12-15 17:18:47.637258 nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/utils/__init__.py
--rw-r--r--   0        0        0     3396 2023-12-12 10:51:18.082169 nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/utils/addresses.py
--rw-r--r--   0        0        0     3568 2023-12-13 10:15:42.581231 nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/utils/addresses_remove.py
--rw-r--r--   0        0        0     1265 2023-12-12 10:51:18.082169 nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/utils/applications.py
--rw-r--r--   0        0        0     1631 2023-12-13 10:40:40.435465 nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/utils/checks.py
--rw-r--r--   0        0        0        0 2023-12-15 17:18:47.637258 nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/utils/common/__init__.py
--rw-r--r--   0        0        0     1877 2023-12-15 16:47:07.753416 nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/utils/common/utils.py
--rw-r--r--   0        0        0     1823 2023-12-12 10:51:18.086169 nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/utils/common/yamlizer.py
--rw-r--r--   0        0        0      352 2023-12-12 10:51:18.086169 nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/utils/constants.py
--rw-r--r--   0        0        0     2826 2023-12-12 10:51:18.086169 nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/utils/git_writer.py
--rw-r--r--   0        0        0     1516 2023-12-12 10:51:18.086169 nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/utils/indexes.py
--rw-r--r--   0        0        0     4187 2023-12-13 16:45:54.977765 nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/utils/locking_panorama.py
--rw-r--r--   0        0        0     2389 2023-12-12 10:51:18.086169 nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/utils/object_deletion_checker.py
--rw-r--r--   0        0        0     9185 2023-12-15 17:18:47.393257 nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/utils/panorama.py
--rw-r--r--   0        0        0     1679 2023-12-12 10:51:18.090169 nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/utils/rules_getter.py
--rw-r--r--   0        0        0     1982 2023-12-12 10:51:18.090169 nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/utils/services.py
--rw-r--r--   0        0        0     1012 2023-12-12 10:51:18.090169 nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/utils/tags.py
--rw-r--r--   0        0        0      770 2023-12-15 17:18:47.393257 nagra_network_paloalto_utils-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      918 1970-01-01 00:00:00.000000 nagra_network_paloalto_utils-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       37 2023-12-12 10:51:18.074169 nagra_network_paloalto_utils-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-12-15 18:36:47.090040 nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/__init__.py
+-rw-r--r--   0        0        0      335 2023-12-12 10:51:18.074169 nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/__main__.py
+-rw-r--r--   0        0        0     1484 2023-12-13 10:15:42.581231 nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/commands/__init__.py
+-rw-r--r--   0        0        0      759 2023-12-12 10:51:18.074169 nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/commands/git_writer.py
+-rw-r--r--   0        0        0      674 2023-12-15 16:47:07.749416 nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/commands/panorama/__init__.py
+-rw-r--r--   0        0        0      343 2023-12-12 10:51:18.074169 nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/commands/panorama/objects/__init__.py
+-rw-r--r--   0        0        0     4455 2023-12-12 10:51:18.078169 nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/commands/panorama/objects/addresses.py
+-rw-r--r--   0        0        0      962 2023-12-12 10:51:18.078169 nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/commands/panorama/objects/applications.py
+-rw-r--r--   0        0        0     2494 2023-12-12 10:51:18.078169 nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/commands/panorama/objects/services.py
+-rw-r--r--   0        0        0     2294 2023-12-12 10:51:18.078169 nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/commands/panorama/objects/tags.py
+-rw-r--r--   0        0        0     3470 2023-12-15 18:36:46.886040 nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/commands/panorama/panorama.py
+-rw-r--r--   0        0        0      145 2023-12-12 10:51:18.078169 nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/commands/terraform/__init__.py
+-rw-r--r--   0        0        0     1070 2023-12-13 10:15:42.581231 nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/commands/terraform/object_deletion_checker.py
+-rw-r--r--   0        0        0      191 2023-12-12 10:51:18.078169 nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/commands/yaml/__init__.py
+-rw-r--r--   0        0        0     2730 2023-12-12 10:51:18.078169 nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/commands/yaml/checks.py
+-rw-r--r--   0        0        0     1402 2023-12-12 10:51:18.082169 nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/commands/yaml/indexes.py
+-rw-r--r--   0        0        0        0 2023-12-15 18:36:47.094040 nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/utils/__init__.py
+-rw-r--r--   0        0        0     3396 2023-12-12 10:51:18.082169 nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/utils/addresses.py
+-rw-r--r--   0        0        0     3568 2023-12-13 10:15:42.581231 nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/utils/addresses_remove.py
+-rw-r--r--   0        0        0     1265 2023-12-12 10:51:18.082169 nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/utils/applications.py
+-rw-r--r--   0        0        0     1631 2023-12-13 10:40:40.435465 nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/utils/checks.py
+-rw-r--r--   0        0        0        0 2023-12-15 18:36:47.094040 nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/utils/common/__init__.py
+-rw-r--r--   0        0        0     1877 2023-12-15 16:47:07.753416 nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/utils/common/utils.py
+-rw-r--r--   0        0        0     1823 2023-12-12 10:51:18.086169 nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/utils/common/yamlizer.py
+-rw-r--r--   0        0        0      352 2023-12-12 10:51:18.086169 nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/utils/constants.py
+-rw-r--r--   0        0        0     2826 2023-12-12 10:51:18.086169 nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/utils/git_writer.py
+-rw-r--r--   0        0        0     1516 2023-12-12 10:51:18.086169 nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/utils/indexes.py
+-rw-r--r--   0        0        0     4187 2023-12-13 16:45:54.977765 nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/utils/locking_panorama.py
+-rw-r--r--   0        0        0     2389 2023-12-12 10:51:18.086169 nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/utils/object_deletion_checker.py
+-rw-r--r--   0        0        0     9223 2023-12-15 18:36:46.886040 nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/utils/panorama.py
+-rw-r--r--   0        0        0     1679 2023-12-12 10:51:18.090169 nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/utils/rules_getter.py
+-rw-r--r--   0        0        0     1982 2023-12-12 10:51:18.090169 nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/utils/services.py
+-rw-r--r--   0        0        0     1012 2023-12-12 10:51:18.090169 nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/utils/tags.py
+-rw-r--r--   0        0        0      743 2023-12-15 18:36:46.890040 nagra_network_paloalto_utils-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 nagra_network_paloalto_utils-0.1.9/PKG-INFO
```

### Comparing `nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/commands/__init__.py` & `nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/commands/git_writer.py` & `nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/commands/git_writer.py`

 * *Files identical despite different names*

### Comparing `nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/commands/panorama/__init__.py` & `nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/commands/panorama/__init__.py`

 * *Files identical despite different names*

### Comparing `nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/commands/panorama/objects/addresses.py` & `nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/commands/panorama/objects/addresses.py`

 * *Files identical despite different names*

### Comparing `nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/commands/panorama/objects/applications.py` & `nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/commands/panorama/objects/applications.py`

 * *Files identical despite different names*

### Comparing `nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/commands/panorama/objects/services.py` & `nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/commands/panorama/objects/services.py`

 * *Files identical despite different names*

### Comparing `nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/commands/panorama/objects/tags.py` & `nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/commands/panorama/objects/tags.py`

 * *Files identical despite different names*

### Comparing `nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/commands/panorama/panorama.py` & `nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/commands/panorama/panorama.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,14 @@
         obj.CI_COMMIT_SHA,
     )
 
     res = commit(
         obj.URL,
         obj.API_KEY,
         commiter_name,
-        commit_type="partial",
         description=description,
     )
     if res in ("fail", "error"):
         log.error(
             "Error. This is most likely because someone else is performing maintenance on the firewall."
             " You will need to manually commit-all",
         )
```

### Comparing `nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/commands/terraform/object_deletion_checker.py` & `nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/commands/terraform/object_deletion_checker.py`

 * *Files identical despite different names*

### Comparing `nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/commands/yaml/checks.py` & `nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/commands/yaml/checks.py`

 * *Files identical despite different names*

### Comparing `nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/commands/yaml/indexes.py` & `nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/commands/yaml/indexes.py`

 * *Files identical despite different names*

### Comparing `nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/utils/addresses.py` & `nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/utils/addresses.py`

 * *Files identical despite different names*

### Comparing `nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/utils/addresses_remove.py` & `nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/utils/addresses_remove.py`

 * *Files identical despite different names*

### Comparing `nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/utils/applications.py` & `nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/utils/applications.py`

 * *Files identical despite different names*

### Comparing `nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/utils/checks.py` & `nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/utils/checks.py`

 * *Files identical despite different names*

### Comparing `nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/utils/common/utils.py` & `nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/utils/common/utils.py`

 * *Files identical despite different names*

### Comparing `nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/utils/common/yamlizer.py` & `nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/utils/common/yamlizer.py`

 * *Files identical despite different names*

### Comparing `nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/utils/git_writer.py` & `nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/utils/git_writer.py`

 * *Files identical despite different names*

### Comparing `nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/utils/indexes.py` & `nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/utils/indexes.py`

 * *Files identical despite different names*

### Comparing `nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/utils/locking_panorama.py` & `nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/utils/locking_panorama.py`

 * *Files identical despite different names*

### Comparing `nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/utils/object_deletion_checker.py` & `nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/utils/object_deletion_checker.py`

 * *Files identical despite different names*

### Comparing `nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/utils/panorama.py` & `nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/utils/panorama.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,32 +82,30 @@
     return True
 
 
 def commit(
     url,
     api_key,
     admin: str,
-    commit_type="normal",
     description="Terraform pipeline auto commit",
     verify=False,
     timeout=None,
 ) -> str:
     """
     Commit on the panorama
     :param admin: admin name under which to commit
     :param commit_type: the type of commit
     :return: error, fail, success, unchanged or timeout
     """
     api = XMLApi(url, api_key, verify=verify)
     # Check if there are changes pending to commit
-    if commit_type != "all":
-        res = api.pending_changes().xpath(".//result/text()")[0]
-        if res == "no":
-            log.info("No change to commit")
-            return "unchanged"
+    res = api.pending_changes().xpath(".//result/text()")[0]
+    if res == "no":
+        log.info("No change to commit")
+        return "unchanged"
     description_tag = f"<description>{description}</description>"
     cmd = (
         "<commit><partial>"
         "<device-and-network>excluded</device-and-network>"
         "<shared-object>excluded</shared-object>"
         f"<admin><member>{admin}</member></admin>"
         f"{description_tag}"
@@ -122,14 +120,16 @@
         line = commit_response["result"]["msg"]["line"]
         log.info(
             f"""Success: {line}""",
         )
         job_id = commit_response["result"]["job"]
     except Exception as e:
         log.warning(e)
+        if "No edits" in str(e):
+            return "unchanged"
         return "error"
     # TODO: Code should always return a value
     try:
         delta_seconds = 20
         max_retry = 15
         # Loop to check the job status every 20 seconds until the job
         # is completed, or up to 5 minutes (15 retries)
@@ -145,28 +145,28 @@
             # If job is still pending, continue loop
             if result == "PEND":
                 job_progress = job["progress"]
                 log.info(
                     f"Job pending: {job_progress}% completed",
                 )
                 continue
-            if result == "FAIL":
-                log.error(f"Commit FAILED: {details}")
-                return "fail"
             if result == "OK":
                 log.info(f"Commit SUCCEED: {details}")
                 return "success"
+            if result == "FAIL":
+                log.error(f"Commit FAILED: {details}")
+                return "fail"
             log.error(f"ERROR: Received unexpected result '{result}'")
             return "error"
         log.warning(
             f"Commit pending for {delta_seconds * max_retry // 60} minutes - stopping script"
         )
         return "timeout"
     except Exception as e:
-        log.error(e)
+        log.error(f"Error while waiting for job completion: {e}")
         return "unchanged"
 
 
 def check_pending_on_devices(
     devices: list,
     api_key,
     url,
```

### Comparing `nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/utils/rules_getter.py` & `nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/utils/rules_getter.py`

 * *Files identical despite different names*

### Comparing `nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/utils/services.py` & `nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/utils/services.py`

 * *Files identical despite different names*

### Comparing `nagra_network_paloalto_utils-0.1.8/nagra_network_paloalto_utils/utils/tags.py` & `nagra_network_paloalto_utils-0.1.9/nagra_network_paloalto_utils/utils/tags.py`

 * *Files identical despite different names*

### Comparing `nagra_network_paloalto_utils-0.1.8/pyproject.toml` & `nagra_network_paloalto_utils-0.1.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [tool.poetry]
 name = "nagra_network_paloalto_utils"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["David Gallay <david.gallay@nagra.com>"]
 readme = "README.md"
 packages = [{include = "nagra_network_paloalto_utils", from="."}]
 
 [tool.poetry.scripts]
 paloalto_utils = "nagra_network_paloalto_utils.__main__:main"
 pautils = "nagra_network_paloalto_utils.__main__:main"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pyyaml = ">=0.2.5"
-pan-os-python = ">=1.2.0"
 gitpython = ">=0.3.6"
 colorama = ">=0.4.4"
 urllib3 = ">=1.26.4"
 ruamel-yaml = ">=0.17.21"
 xmltodict = ">=0.13.0"
 click = "^8.1.7"
 nagra-panorama-api = "^0.1.12"
```

### Comparing `nagra_network_paloalto_utils-0.1.8/PKG-INFO` & `nagra_network_paloalto_utils-0.1.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: nagra_network_paloalto_utils
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: David Gallay
 Author-email: david.gallay@nagra.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: colorama (>=0.4.4)
 Requires-Dist: gitpython (>=0.3.6)
 Requires-Dist: glom (>=23.4.0,<24.0.0)
 Requires-Dist: nagra-panorama-api (>=0.1.12,<0.2.0)
-Requires-Dist: pan-os-python (>=1.2.0)
 Requires-Dist: pyyaml (>=0.2.5)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: ruamel-yaml (>=0.17.21)
 Requires-Dist: urllib3 (>=1.26.4)
 Requires-Dist: xmltodict (>=0.13.0)
 Description-Content-Type: text/markdown
```

