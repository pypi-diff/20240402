# Comparing `tmp/v2share-0.1.0a4.tar.gz` & `tmp/v2share-0.1.0a5.tar.gz`

## Comparing `v2share-0.1.0a4.tar` & `v2share-0.1.0a5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 v2share-0.1.0a4/requirements.txt
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 v2share-0.1.0a4/.github/workflows/python-tests.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 v2share-0.1.0a4/tests/__init__.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 v2share-0.1.0a4/tests/test_config.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 v2share-0.1.0a4/v2share/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 v2share-0.1.0a4/v2share/_version.py
--rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 v2share-0.1.0a4/v2share/clash.py
--rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 v2share-0.1.0a4/v2share/clashmeta.py
--rw-r--r--   0        0        0     4260 2020-02-02 00:00:00.000000 v2share-0.1.0a4/v2share/data.py
--rw-r--r--   0        0        0     6759 2020-02-02 00:00:00.000000 v2share-0.1.0a4/v2share/singbox.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 v2share-0.1.0a4/v2share/templates/clash.yml
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 v2share-0.1.0a4/v2share/templates/singbox.json
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 v2share-0.1.0a4/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 v2share-0.1.0a4/README.md
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 v2share-0.1.0a4/pyproject.toml
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 v2share-0.1.0a4/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 v2share-0.1.0a5/requirements.txt
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 v2share-0.1.0a5/.github/workflows/python-tests.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 v2share-0.1.0a5/tests/__init__.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 v2share-0.1.0a5/tests/test_config.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 v2share-0.1.0a5/v2share/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 v2share-0.1.0a5/v2share/_version.py
+-rw-r--r--   0        0        0     4052 2020-02-02 00:00:00.000000 v2share-0.1.0a5/v2share/clash.py
+-rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 v2share-0.1.0a5/v2share/clashmeta.py
+-rw-r--r--   0        0        0     4260 2020-02-02 00:00:00.000000 v2share-0.1.0a5/v2share/data.py
+-rw-r--r--   0        0        0     6759 2020-02-02 00:00:00.000000 v2share-0.1.0a5/v2share/singbox.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 v2share-0.1.0a5/v2share/templates/clash.yml
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 v2share-0.1.0a5/v2share/templates/singbox.json
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 v2share-0.1.0a5/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 v2share-0.1.0a5/README.md
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 v2share-0.1.0a5/pyproject.toml
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 v2share-0.1.0a5/PKG-INFO
```

### Comparing `v2share-0.1.0a4/.github/workflows/python-tests.yml` & `v2share-0.1.0a5/.github/workflows/python-tests.yml`

 * *Files identical despite different names*

### Comparing `v2share-0.1.0a4/tests/test_config.py` & `v2share-0.1.0a5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `v2share-0.1.0a4/v2share/clash.py` & `v2share-0.1.0a5/v2share/clash.py`

 * *Files 5% similar despite different names*

```diff
@@ -119,15 +119,15 @@
             path=config.path,
             udp=True,
             alpn=config.alpn,
             ais=config.allow_insecure,
         )
 
         if config.protocol == "vmess":
-            node["uuid"] = config.uuid
+            node["uuid"] = str(config.uuid)
             node["alterId"] = 0
             node["cipher"] = "auto"
             self.data["proxies"].append(node)
             self.proxy_remarks.append(config.remark)
         elif config.protocol == "trojan":
             node["password"] = config.password
             self.data["proxies"].append(node)
```

### Comparing `v2share-0.1.0a4/v2share/clashmeta.py` & `v2share-0.1.0a5/v2share/clashmeta.py`

 * *Files 13% similar despite different names*

```diff
@@ -59,22 +59,22 @@
             fp=config.fingerprint,
             pbk=config.reality_pbk,
             sid=config.reality_sid,
             ais=config.allow_insecure,
         )
 
         if config.protocol == "vmess":
-            node["uuid"] = config.uuid
+            node["uuid"] = str(config.uuid)
             node["alterId"] = 0
             node["cipher"] = "auto"
             self.data["proxies"].append(node)
             self.proxy_remarks.append(config.remark)
 
         if config.protocol == "vless":
-            node["uuid"] = config.uuid
+            node["uuid"] = str(config.uuid)
 
             if (
                 config.transport_type in ("tcp", "kcp")
                 and config.header_type != "http"
             ):
                 node["flow"] = config.flow
```

### Comparing `v2share-0.1.0a4/v2share/data.py` & `v2share-0.1.0a5/v2share/data.py`

 * *Files identical despite different names*

### Comparing `v2share-0.1.0a4/v2share/singbox.py` & `v2share-0.1.0a5/v2share/singbox.py`

 * *Files identical despite different names*

### Comparing `v2share-0.1.0a4/v2share/templates/singbox.json` & `v2share-0.1.0a5/v2share/templates/singbox.json`

 * *Files identical despite different names*

### Comparing `v2share-0.1.0a4/.gitignore` & `v2share-0.1.0a5/.gitignore`

 * *Files identical despite different names*

### Comparing `v2share-0.1.0a4/pyproject.toml` & `v2share-0.1.0a5/pyproject.toml`

 * *Files identical despite different names*

