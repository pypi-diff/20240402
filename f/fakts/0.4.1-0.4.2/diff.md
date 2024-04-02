# Comparing `tmp/fakts-0.4.1.tar.gz` & `tmp/fakts-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fakts-0.4.1.tar", max compression
+gzip compressed data, was "fakts-0.4.2.tar", max compression
```

## Comparing `fakts-0.4.1.tar` & `fakts-0.4.2.tar`

### file list

```diff
@@ -1,51 +1,52 @@
--rw-r--r--   0        0        0     4166 2024-01-05 12:07:57.937529 fakts-0.4.1/README.md
--rw-r--r--   0        0        0      936 2024-01-05 12:07:57.941529 fakts-0.4.1/fakts/__init__.py
--rw-r--r--   0        0        0      348 2024-01-05 12:07:57.941529 fakts-0.4.1/fakts/cli/__init__.py
--rw-r--r--   0        0        0     4194 2024-01-05 12:07:57.941529 fakts-0.4.1/fakts/cli/advertise.py
--rw-r--r--   0        0        0     4314 2024-01-31 13:33:54.008647 fakts-0.4.1/fakts/cli/main.py
--rw-r--r--   0        0        0     1062 2024-01-05 12:07:57.941529 fakts-0.4.1/fakts/errors.py
--rw-r--r--   0        0        0    10083 2024-01-05 12:07:57.941529 fakts-0.4.1/fakts/fakts.py
--rw-r--r--   0        0        0     1474 2024-01-05 12:07:57.941529 fakts-0.4.1/fakts/grants/__init__.py
--rw-r--r--   0        0        0     3101 2024-01-05 12:07:57.941529 fakts-0.4.1/fakts/grants/env.py
--rw-r--r--   0        0        0      120 2024-01-05 12:07:57.941529 fakts-0.4.1/fakts/grants/errors.py
--rw-r--r--   0        0        0      117 2024-01-05 12:07:57.941529 fakts-0.4.1/fakts/grants/io/__init__.py
--rw-r--r--   0        0        0     4699 2024-01-05 12:07:57.941529 fakts-0.4.1/fakts/grants/io/qt/yaml.py
--rw-r--r--   0        0        0     1475 2024-01-05 12:07:57.941529 fakts-0.4.1/fakts/grants/io/toml.py
--rw-r--r--   0        0        0      752 2024-01-05 12:07:57.941529 fakts-0.4.1/fakts/grants/io/yaml.py
--rw-r--r--   0        0        0      285 2024-01-05 12:07:57.941529 fakts-0.4.1/fakts/grants/meta/__init__.py
--rw-r--r--   0        0        0     3710 2024-01-05 12:07:57.941529 fakts-0.4.1/fakts/grants/meta/cache.py
--rw-r--r--   0        0        0     1438 2024-01-05 12:07:57.941529 fakts-0.4.1/fakts/grants/meta/failsafe.py
--rw-r--r--   0        0        0     1746 2024-01-05 12:07:57.945529 fakts-0.4.1/fakts/grants/meta/parallel.py
--rw-r--r--   0        0        0      419 2024-01-05 12:07:57.945529 fakts-0.4.1/fakts/grants/remote/__init__.py
--rw-r--r--   0        0        0     2071 2024-01-05 12:07:57.945529 fakts-0.4.1/fakts/grants/remote/base.py
--rw-r--r--   0        0        0     1691 2024-01-05 12:07:57.945529 fakts-0.4.1/fakts/grants/remote/builders.py
--rw-r--r--   0        0        0      375 2024-01-05 12:07:57.945529 fakts-0.4.1/fakts/grants/remote/claimers/__init__.py
--rw-r--r--   0        0        0     2492 2024-01-05 12:07:57.945529 fakts-0.4.1/fakts/grants/remote/claimers/post.py
--rw-r--r--   0        0        0      696 2024-01-05 12:07:57.945529 fakts-0.4.1/fakts/grants/remote/claimers/static.py
--rw-r--r--   0        0        0      266 2024-01-05 12:07:57.945529 fakts-0.4.1/fakts/grants/remote/demanders/__init__.py
--rw-r--r--   0        0        0     5087 2024-01-05 12:07:57.945529 fakts-0.4.1/fakts/grants/remote/demanders/auto_save.py
--rw-r--r--   0        0        0     2628 2024-01-05 12:07:57.945529 fakts-0.4.1/fakts/grants/remote/demanders/cache.py
--rw-r--r--   0        0        0     8843 2024-01-05 12:07:57.945529 fakts-0.4.1/fakts/grants/remote/demanders/device_code.py
--rw-r--r--   0        0        0      137 2024-01-05 12:07:57.945529 fakts-0.4.1/fakts/grants/remote/demanders/qt/__init__.py
--rw-r--r--   0        0        0     1965 2024-01-05 12:07:57.945529 fakts-0.4.1/fakts/grants/remote/demanders/qt/auto_save_token_widget.py
--rw-r--r--   0        0        0     2582 2024-01-05 12:07:57.945529 fakts-0.4.1/fakts/grants/remote/demanders/qt/qt_settings_token_store.py
--rw-r--r--   0        0        0     3196 2024-01-05 12:07:57.945529 fakts-0.4.1/fakts/grants/remote/demanders/retrieve.py
--rw-r--r--   0        0        0     1596 2024-01-05 12:07:57.945529 fakts-0.4.1/fakts/grants/remote/demanders/static.py
--rw-r--r--   0        0        0     3253 2024-01-13 14:27:06.393039 fakts-0.4.1/fakts/grants/remote/demanders/utils.py
--rw-r--r--   0        0        0      459 2024-01-05 12:07:57.945529 fakts-0.4.1/fakts/grants/remote/discovery/__init__.py
--rw-r--r--   0        0        0     7036 2024-01-31 12:16:22.055310 fakts-0.4.1/fakts/grants/remote/discovery/advertised.py
--rw-r--r--   0        0        0     4877 2024-01-05 12:07:57.945529 fakts-0.4.1/fakts/grants/remote/discovery/auto_save.py
--rw-r--r--   0        0        0     2011 2024-01-05 12:07:57.945529 fakts-0.4.1/fakts/grants/remote/discovery/cache.py
--rw-r--r--   0        0        0      138 2024-01-05 12:07:57.945529 fakts-0.4.1/fakts/grants/remote/discovery/qt/__init__.py
--rw-r--r--   0        0        0     1952 2024-01-05 12:07:57.949529 fakts-0.4.1/fakts/grants/remote/discovery/qt/auto_save_endpoint_widget.py
--rw-r--r--   0        0        0     1352 2024-01-05 12:07:57.949529 fakts-0.4.1/fakts/grants/remote/discovery/qt/qt_settings_endpoint_store.py
--rw-r--r--   0        0        0    16040 2024-01-31 12:12:49.794226 fakts-0.4.1/fakts/grants/remote/discovery/qt/selectable_beacon.py
--rw-r--r--   0        0        0      833 2024-01-05 12:07:57.949529 fakts-0.4.1/fakts/grants/remote/discovery/static.py
--rw-r--r--   0        0        0     3931 2024-01-05 12:07:57.949529 fakts-0.4.1/fakts/grants/remote/discovery/utils.py
--rw-r--r--   0        0        0     2770 2024-01-05 12:07:57.949529 fakts-0.4.1/fakts/grants/remote/discovery/well_known.py
--rw-r--r--   0        0        0      504 2024-01-05 12:07:57.949529 fakts-0.4.1/fakts/grants/remote/errors.py
--rw-r--r--   0        0        0     3475 2024-01-05 12:07:57.949529 fakts-0.4.1/fakts/grants/remote/models.py
--rw-r--r--   0        0        0     2205 2024-01-05 12:07:57.949529 fakts-0.4.1/fakts/models.py
--rw-r--r--   0        0        0      681 2024-01-05 12:07:57.949529 fakts-0.4.1/fakts/utils.py
--rw-r--r--   0        0        0     2249 2024-02-07 14:35:40.616231 fakts-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     5149 1970-01-01 00:00:00.000000 fakts-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     4166 2024-04-02 09:59:45.253647 fakts-0.4.2/README.md
+-rw-r--r--   0        0        0      936 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/__init__.py
+-rw-r--r--   0        0        0      348 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/cli/__init__.py
+-rw-r--r--   0        0        0     4194 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/cli/advertise.py
+-rw-r--r--   0        0        0     4314 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/cli/main.py
+-rw-r--r--   0        0        0     1062 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/errors.py
+-rw-r--r--   0        0        0    10083 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/fakts.py
+-rw-r--r--   0        0        0     1474 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/__init__.py
+-rw-r--r--   0        0        0     3101 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/env.py
+-rw-r--r--   0        0        0      120 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/errors.py
+-rw-r--r--   0        0        0      117 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/io/__init__.py
+-rw-r--r--   0        0        0     4699 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/io/qt/yaml.py
+-rw-r--r--   0        0        0     1475 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/io/toml.py
+-rw-r--r--   0        0        0      752 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/io/yaml.py
+-rw-r--r--   0        0        0      285 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/meta/__init__.py
+-rw-r--r--   0        0        0     3710 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/meta/cache.py
+-rw-r--r--   0        0        0     1438 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/meta/failsafe.py
+-rw-r--r--   0        0        0     1746 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/meta/parallel.py
+-rw-r--r--   0        0        0      419 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/remote/__init__.py
+-rw-r--r--   0        0        0     2140 2024-04-02 10:33:11.408718 fakts-0.4.2/fakts/grants/remote/base.py
+-rw-r--r--   0        0        0     2074 2024-04-02 10:34:33.092560 fakts-0.4.2/fakts/grants/remote/builders.py
+-rw-r--r--   0        0        0      375 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/remote/claimers/__init__.py
+-rw-r--r--   0        0        0     2492 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/remote/claimers/post.py
+-rw-r--r--   0        0        0      696 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/remote/claimers/static.py
+-rw-r--r--   0        0        0      266 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/remote/demanders/__init__.py
+-rw-r--r--   0        0        0     5087 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/remote/demanders/auto_save.py
+-rw-r--r--   0        0        0     2628 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/remote/demanders/cache.py
+-rw-r--r--   0        0        0     8843 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/remote/demanders/device_code.py
+-rw-r--r--   0        0        0      137 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/remote/demanders/qt/__init__.py
+-rw-r--r--   0        0        0     1965 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/remote/demanders/qt/auto_save_token_widget.py
+-rw-r--r--   0        0        0     2582 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/remote/demanders/qt/qt_settings_token_store.py
+-rw-r--r--   0        0        0     3351 2024-04-02 10:20:11.850394 fakts-0.4.2/fakts/grants/remote/demanders/redeem.py
+-rw-r--r--   0        0        0     3196 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/remote/demanders/retrieve.py
+-rw-r--r--   0        0        0     1596 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/remote/demanders/static.py
+-rw-r--r--   0        0        0     3253 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/remote/demanders/utils.py
+-rw-r--r--   0        0        0      459 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/remote/discovery/__init__.py
+-rw-r--r--   0        0        0     7036 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/remote/discovery/advertised.py
+-rw-r--r--   0        0        0     4877 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/remote/discovery/auto_save.py
+-rw-r--r--   0        0        0     2011 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/remote/discovery/cache.py
+-rw-r--r--   0        0        0      138 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/remote/discovery/qt/__init__.py
+-rw-r--r--   0        0        0     1952 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/remote/discovery/qt/auto_save_endpoint_widget.py
+-rw-r--r--   0        0        0     1352 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/remote/discovery/qt/qt_settings_endpoint_store.py
+-rw-r--r--   0        0        0    16040 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/remote/discovery/qt/selectable_beacon.py
+-rw-r--r--   0        0        0      833 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/remote/discovery/static.py
+-rw-r--r--   0        0        0     3931 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/remote/discovery/utils.py
+-rw-r--r--   0        0        0     2770 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/remote/discovery/well_known.py
+-rw-r--r--   0        0        0      504 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/remote/errors.py
+-rw-r--r--   0        0        0     3475 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/grants/remote/models.py
+-rw-r--r--   0        0        0     2205 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/models.py
+-rw-r--r--   0        0        0      681 2024-04-02 09:59:45.253647 fakts-0.4.2/fakts/utils.py
+-rw-r--r--   0        0        0     2249 2024-04-02 13:27:55.262453 fakts-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     5200 1970-01-01 00:00:00.000000 fakts-0.4.2/PKG-INFO
```

### Comparing `fakts-0.4.1/README.md` & `fakts-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `fakts-0.4.1/fakts/__init__.py` & `fakts-0.4.2/fakts/__init__.py`

 * *Files identical despite different names*

### Comparing `fakts-0.4.1/fakts/cli/advertise.py` & `fakts-0.4.2/fakts/cli/advertise.py`

 * *Files identical despite different names*

### Comparing `fakts-0.4.1/fakts/cli/main.py` & `fakts-0.4.2/fakts/cli/main.py`

 * *Files identical despite different names*

### Comparing `fakts-0.4.1/fakts/errors.py` & `fakts-0.4.2/fakts/errors.py`

 * *Files identical despite different names*

### Comparing `fakts-0.4.1/fakts/fakts.py` & `fakts-0.4.2/fakts/fakts.py`

 * *Files identical despite different names*

### Comparing `fakts-0.4.1/fakts/grants/__init__.py` & `fakts-0.4.2/fakts/grants/__init__.py`

 * *Files identical despite different names*

### Comparing `fakts-0.4.1/fakts/grants/env.py` & `fakts-0.4.2/fakts/grants/env.py`

 * *Files identical despite different names*

### Comparing `fakts-0.4.1/fakts/grants/io/qt/yaml.py` & `fakts-0.4.2/fakts/grants/io/qt/yaml.py`

 * *Files identical despite different names*

### Comparing `fakts-0.4.1/fakts/grants/io/toml.py` & `fakts-0.4.2/fakts/grants/io/toml.py`

 * *Files identical despite different names*

### Comparing `fakts-0.4.1/fakts/grants/io/yaml.py` & `fakts-0.4.2/fakts/grants/io/yaml.py`

 * *Files identical despite different names*

### Comparing `fakts-0.4.1/fakts/grants/meta/cache.py` & `fakts-0.4.2/fakts/grants/meta/cache.py`

 * *Files identical despite different names*

### Comparing `fakts-0.4.1/fakts/grants/meta/failsafe.py` & `fakts-0.4.2/fakts/grants/meta/failsafe.py`

 * *Files identical despite different names*

### Comparing `fakts-0.4.1/fakts/grants/meta/parallel.py` & `fakts-0.4.2/fakts/grants/meta/parallel.py`

 * *Files identical despite different names*

### Comparing `fakts-0.4.1/fakts/grants/remote/base.py` & `fakts-0.4.2/fakts/grants/remote/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from fakts.grants.errors import GrantError
 from typing import Dict
 import logging
 from .models import Demander, Discovery, Claimer
 from fakts.models import FaktsRequest, FaktValue
-from pydantic import BaseModel
-
+from pydantic import BaseModel, Field
+from fakts.grants.remote.claimers.static import StaticClaimer
 logger = logging.getLogger(__name__)
 
 
 Token = str
 EndpointUrl = str
 
 
@@ -36,15 +36,15 @@
 
     discovery: Discovery
     """The discovery mechanism to use for finding the endpoint"""
 
     demander: Demander
     """The demander mechanism to use for demanding the token FROM the endpoint"""
 
-    claimer: Claimer
+    claimer: Claimer 
     """The claimer mechanism to use for claiming the token FROM the endpoint"""
 
     async def aload(self, request: FaktsRequest) -> Dict[str, FaktValue]:
         """Load the configuration
 
         This function will first discover the endpoint, then demand a token from it,
         and then claim the configuration from it.
```

### Comparing `fakts-0.4.1/fakts/grants/remote/builders.py` & `fakts-0.4.2/fakts/grants/remote/builders.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from fakts.grants.remote import RemoteGrant
 
 from fakts.grants.remote.claimers.static import StaticClaimer
 from fakts.grants.remote.discovery.static import StaticDiscovery
 from fakts.grants.remote.demanders.static import StaticDemander
+from fakts.grants.remote.demanders.redeem import RedeemDemander
 from fakts.grants.remote.claimers.post import ClaimEndpointClaimer
 from fakts.grants.remote.models import FaktsEndpoint, FaktValue
 from typing import Dict
 
 
 def build_remote_testing(value: Dict[str, FaktValue]) -> RemoteGrant:
     """Builds a remote grant for testing purposes
@@ -29,14 +30,23 @@
             endpoint=FaktsEndpoint(base_url="https://example.com")
         ),
         claimer=StaticClaimer(value=value),
         demander=StaticDemander(token="token"),  # type: ignore
     )
 
 
+def build_redeem_grant(url: str, manifest: Dict[str, FaktValue], redeem_token: str ) -> RemoteGrant:
+
+    return RemoteGrant(
+        discovery=StaticDiscovery(endpoint=FaktsEndpoint(base_url=url)),
+        claimer=ClaimEndpointClaimer(),
+        demander=RedeemDemander(manifest=manifest, token=redeem_token),
+    )
+
+
 def build_remote_testing_with_token(fakts_url: str, token: str) -> RemoteGrant:
     """Builds a remote grant for testing purposes
 
     This grant will use the given token to demand the configuration from fakts.
     This is great for testing purposes, or when an api token is known at compile time.
 
     Parameters
```

### Comparing `fakts-0.4.1/fakts/grants/remote/claimers/post.py` & `fakts-0.4.2/fakts/grants/remote/claimers/post.py`

 * *Files identical despite different names*

### Comparing `fakts-0.4.1/fakts/grants/remote/claimers/static.py` & `fakts-0.4.2/fakts/grants/remote/claimers/static.py`

 * *Files identical despite different names*

### Comparing `fakts-0.4.1/fakts/grants/remote/demanders/auto_save.py` & `fakts-0.4.2/fakts/grants/remote/demanders/auto_save.py`

 * *Files identical despite different names*

### Comparing `fakts-0.4.1/fakts/grants/remote/demanders/cache.py` & `fakts-0.4.2/fakts/grants/remote/demanders/cache.py`

 * *Files identical despite different names*

### Comparing `fakts-0.4.1/fakts/grants/remote/demanders/device_code.py` & `fakts-0.4.2/fakts/grants/remote/demanders/device_code.py`

 * *Files identical despite different names*

### Comparing `fakts-0.4.1/fakts/grants/remote/demanders/qt/auto_save_token_widget.py` & `fakts-0.4.2/fakts/grants/remote/demanders/qt/auto_save_token_widget.py`

 * *Files identical despite different names*

### Comparing `fakts-0.4.1/fakts/grants/remote/demanders/qt/qt_settings_token_store.py` & `fakts-0.4.2/fakts/grants/remote/demanders/qt/qt_settings_token_store.py`

 * *Files identical despite different names*

### Comparing `fakts-0.4.1/fakts/grants/remote/demanders/retrieve.py` & `fakts-0.4.2/fakts/grants/remote/demanders/retrieve.py`

 * *Files identical despite different names*

### Comparing `fakts-0.4.1/fakts/grants/remote/demanders/static.py` & `fakts-0.4.2/fakts/grants/remote/demanders/static.py`

 * *Files identical despite different names*

### Comparing `fakts-0.4.1/fakts/grants/remote/demanders/utils.py` & `fakts-0.4.2/fakts/grants/remote/demanders/utils.py`

 * *Files identical despite different names*

### Comparing `fakts-0.4.1/fakts/grants/remote/discovery/advertised.py` & `fakts-0.4.2/fakts/grants/remote/discovery/advertised.py`

 * *Files identical despite different names*

### Comparing `fakts-0.4.1/fakts/grants/remote/discovery/auto_save.py` & `fakts-0.4.2/fakts/grants/remote/discovery/auto_save.py`

 * *Files identical despite different names*

### Comparing `fakts-0.4.1/fakts/grants/remote/discovery/cache.py` & `fakts-0.4.2/fakts/grants/remote/discovery/cache.py`

 * *Files identical despite different names*

### Comparing `fakts-0.4.1/fakts/grants/remote/discovery/qt/auto_save_endpoint_widget.py` & `fakts-0.4.2/fakts/grants/remote/discovery/qt/auto_save_endpoint_widget.py`

 * *Files identical despite different names*

### Comparing `fakts-0.4.1/fakts/grants/remote/discovery/qt/qt_settings_endpoint_store.py` & `fakts-0.4.2/fakts/grants/remote/discovery/qt/qt_settings_endpoint_store.py`

 * *Files identical despite different names*

### Comparing `fakts-0.4.1/fakts/grants/remote/discovery/qt/selectable_beacon.py` & `fakts-0.4.2/fakts/grants/remote/discovery/qt/selectable_beacon.py`

 * *Files identical despite different names*

### Comparing `fakts-0.4.1/fakts/grants/remote/discovery/static.py` & `fakts-0.4.2/fakts/grants/remote/discovery/static.py`

 * *Files identical despite different names*

### Comparing `fakts-0.4.1/fakts/grants/remote/discovery/utils.py` & `fakts-0.4.2/fakts/grants/remote/discovery/utils.py`

 * *Files identical despite different names*

### Comparing `fakts-0.4.1/fakts/grants/remote/discovery/well_known.py` & `fakts-0.4.2/fakts/grants/remote/discovery/well_known.py`

 * *Files identical despite different names*

### Comparing `fakts-0.4.1/fakts/grants/remote/models.py` & `fakts-0.4.2/fakts/grants/remote/models.py`

 * *Files identical despite different names*

### Comparing `fakts-0.4.1/fakts/models.py` & `fakts-0.4.2/fakts/models.py`

 * *Files identical despite different names*

### Comparing `fakts-0.4.1/fakts/utils.py` & `fakts-0.4.2/fakts/utils.py`

 * *Files identical despite different names*

### Comparing `fakts-0.4.1/pyproject.toml` & `fakts-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fakts"
-version = "0.4.1"
+version = "0.4.2"
 description = "asynchronous configuration provider ( tailored to support dynamic client-server relations)"
 authors = ["jhnnsrs <jhnnsrs@gmail.com>"]
 license = "CC BY-NC 3.0"
 readme = "README.md"
 packages = [{ include = "fakts" }]
 
 [tool.poetry.dependencies]
```

### Comparing `fakts-0.4.1/PKG-INFO` & `fakts-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: fakts
-Version: 0.4.1
+Version: 0.4.2
 Summary: asynchronous configuration provider ( tailored to support dynamic client-server relations)
 License: CC BY-NC 3.0
 Author: jhnnsrs
 Author-email: jhnnsrs@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: cli
 Provides-Extra: remote
 Requires-Dist: PyYAML (>=6)
 Requires-Dist: QtPy (>=2.0.1,<3.0.0)
 Requires-Dist: aiohttp (>=3.8.2,<4.0.0) ; extra == "remote"
 Requires-Dist: certifi (>2021) ; extra == "remote"
 Requires-Dist: koil (>=0.3.5)
```

