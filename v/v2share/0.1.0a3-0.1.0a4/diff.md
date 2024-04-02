# Comparing `tmp/v2share-0.1.0a3.tar.gz` & `tmp/v2share-0.1.0a4.tar.gz`

## Comparing `v2share-0.1.0a3.tar` & `v2share-0.1.0a4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 v2share-0.1.0a3/requirements.txt
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 v2share-0.1.0a3/.github/workflows/python-tests.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 v2share-0.1.0a3/tests/__init__.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 v2share-0.1.0a3/tests/test_config.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 v2share-0.1.0a3/v2share/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 v2share-0.1.0a3/v2share/_version.py
--rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 v2share-0.1.0a3/v2share/clash.py
--rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 v2share-0.1.0a3/v2share/clashmeta.py
--rw-r--r--   0        0        0     4260 2020-02-02 00:00:00.000000 v2share-0.1.0a3/v2share/data.py
--rw-r--r--   0        0        0     6754 2020-02-02 00:00:00.000000 v2share-0.1.0a3/v2share/singbox.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 v2share-0.1.0a3/v2share/templates/clash.yml
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 v2share-0.1.0a3/v2share/templates/singbox.json
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 v2share-0.1.0a3/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 v2share-0.1.0a3/README.md
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 v2share-0.1.0a3/pyproject.toml
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 v2share-0.1.0a3/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 v2share-0.1.0a4/requirements.txt
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 v2share-0.1.0a4/.github/workflows/python-tests.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 v2share-0.1.0a4/tests/__init__.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 v2share-0.1.0a4/tests/test_config.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 v2share-0.1.0a4/v2share/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 v2share-0.1.0a4/v2share/_version.py
+-rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 v2share-0.1.0a4/v2share/clash.py
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 v2share-0.1.0a4/v2share/clashmeta.py
+-rw-r--r--   0        0        0     4260 2020-02-02 00:00:00.000000 v2share-0.1.0a4/v2share/data.py
+-rw-r--r--   0        0        0     6759 2020-02-02 00:00:00.000000 v2share-0.1.0a4/v2share/singbox.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 v2share-0.1.0a4/v2share/templates/clash.yml
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 v2share-0.1.0a4/v2share/templates/singbox.json
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 v2share-0.1.0a4/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 v2share-0.1.0a4/README.md
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 v2share-0.1.0a4/pyproject.toml
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 v2share-0.1.0a4/PKG-INFO
```

### Comparing `v2share-0.1.0a3/.github/workflows/python-tests.yml` & `v2share-0.1.0a4/.github/workflows/python-tests.yml`

 * *Files identical despite different names*

### Comparing `v2share-0.1.0a3/tests/test_config.py` & `v2share-0.1.0a4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `v2share-0.1.0a3/v2share/clash.py` & `v2share-0.1.0a4/v2share/clash.py`

 * *Files identical despite different names*

### Comparing `v2share-0.1.0a3/v2share/clashmeta.py` & `v2share-0.1.0a4/v2share/clashmeta.py`

 * *Files identical despite different names*

### Comparing `v2share-0.1.0a3/v2share/data.py` & `v2share-0.1.0a4/v2share/data.py`

 * *Files identical despite different names*

### Comparing `v2share-0.1.0a3/v2share/singbox.py` & `v2share-0.1.0a4/v2share/singbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,15 +194,15 @@
                 sid=config.reality_sid,
                 header_type=config.header_type,
                 headers={},
                 ais=config.allow_insecure,
             )
 
             if config.protocol in ["vless", "vmess"]:
-                outbound["uuid"] = config.uuid
+                outbound["uuid"] = str(config.uuid)
 
             elif config.protocol == "trojan":
                 outbound["password"] = config.password
 
             elif config.protocol == "shadowsocks":
                 outbound["password"] = config.password
                 outbound["method"] = config.shadowsocks_method
```

### Comparing `v2share-0.1.0a3/v2share/templates/singbox.json` & `v2share-0.1.0a4/v2share/templates/singbox.json`

 * *Files identical despite different names*

### Comparing `v2share-0.1.0a3/.gitignore` & `v2share-0.1.0a4/.gitignore`

 * *Files identical despite different names*

### Comparing `v2share-0.1.0a3/pyproject.toml` & `v2share-0.1.0a4/pyproject.toml`

 * *Files identical despite different names*

