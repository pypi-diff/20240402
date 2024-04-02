# Comparing `tmp/moby_distribution-0.5.9.tar.gz` & `tmp/moby_distribution-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moby_distribution-0.5.9.tar", max compression
+gzip compressed data, was "moby_distribution-0.6.0.tar", max compression
```

## Comparing `moby_distribution-0.5.9.tar` & `moby_distribution-0.6.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    11357 2024-01-26 09:36:29.551053 moby_distribution-0.5.9/LICENSE
--rw-r--r--   0        0        0     7006 2024-01-26 09:36:29.551053 moby_distribution-0.5.9/README.md
--rw-r--r--   0        0        0      895 2024-01-26 09:36:29.551053 moby_distribution-0.5.9/moby_distribution/__init__.py
--rw-r--r--   0        0        0        0 2024-01-26 09:36:29.551053 moby_distribution-0.5.9/moby_distribution/registry/__init__.py
--rw-r--r--   0        0        0     5582 2024-01-26 09:36:29.555053 moby_distribution-0.5.9/moby_distribution/registry/auth.py
--rw-r--r--   0        0        0     7160 2024-01-26 09:36:29.555053 moby_distribution-0.5.9/moby_distribution/registry/client.py
--rw-r--r--   0        0        0      917 2024-01-26 09:36:29.555053 moby_distribution-0.5.9/moby_distribution/registry/exceptions.py
--rw-r--r--   0        0        0      752 2024-01-26 09:36:29.555053 moby_distribution-0.5.9/moby_distribution/registry/resources/__init__.py
--rw-r--r--   0        0        0    11137 2024-01-26 09:36:29.555053 moby_distribution-0.5.9/moby_distribution/registry/resources/blobs.py
--rw-r--r--   0        0        0    14480 2024-01-26 09:36:29.555053 moby_distribution-0.5.9/moby_distribution/registry/resources/image.py
--rw-r--r--   0        0        0     4875 2024-01-26 09:36:29.555053 moby_distribution-0.5.9/moby_distribution/registry/resources/manifests.py
--rw-r--r--   0        0        0     1033 2024-01-26 09:36:29.555053 moby_distribution-0.5.9/moby_distribution/registry/resources/tags.py
--rw-r--r--   0        0        0     3972 2024-01-26 09:36:29.555053 moby_distribution-0.5.9/moby_distribution/registry/utils.py
--rw-r--r--   0        0        0        0 2024-01-26 09:36:29.555053 moby_distribution-0.5.9/moby_distribution/spec/__init__.py
--rw-r--r--   0        0        0     1140 2024-01-26 09:36:29.555053 moby_distribution-0.5.9/moby_distribution/spec/auth.py
--rw-r--r--   0        0        0     1070 2024-01-26 09:36:29.555053 moby_distribution-0.5.9/moby_distribution/spec/base.py
--rw-r--r--   0        0        0     2798 2024-01-26 09:36:29.555053 moby_distribution-0.5.9/moby_distribution/spec/endpoint.py
--rw-r--r--   0        0        0     3757 2024-01-26 09:36:29.555053 moby_distribution-0.5.9/moby_distribution/spec/image_json.py
--rw-r--r--   0        0        0     4594 2024-01-26 09:36:29.555053 moby_distribution-0.5.9/moby_distribution/spec/manifest.py
--rw-r--r--   0        0        0      914 2024-01-26 09:36:29.555053 moby_distribution-0.5.9/pyproject.toml
--rw-r--r--   0        0        0     8027 1970-01-01 00:00:00.000000 moby_distribution-0.5.9/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/LICENSE
+-rw-r--r--   0        0        0     7006 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/README.md
+-rw-r--r--   0        0        0      895 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/moby_distribution/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/moby_distribution/registry/__init__.py
+-rw-r--r--   0        0        0     5910 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/moby_distribution/registry/auth.py
+-rw-r--r--   0        0        0     7598 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/moby_distribution/registry/client.py
+-rw-r--r--   0        0        0      917 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/moby_distribution/registry/exceptions.py
+-rw-r--r--   0        0        0      752 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/moby_distribution/registry/resources/__init__.py
+-rw-r--r--   0        0        0    11137 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/moby_distribution/registry/resources/blobs.py
+-rw-r--r--   0        0        0    14792 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/moby_distribution/registry/resources/image.py
+-rw-r--r--   0        0        0     4875 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/moby_distribution/registry/resources/manifests.py
+-rw-r--r--   0        0        0     1033 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/moby_distribution/registry/resources/tags.py
+-rw-r--r--   0        0        0     3972 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/moby_distribution/registry/utils.py
+-rw-r--r--   0        0        0        0 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/moby_distribution/spec/__init__.py
+-rw-r--r--   0        0        0     1140 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/moby_distribution/spec/auth.py
+-rw-r--r--   0        0        0     1070 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/moby_distribution/spec/base.py
+-rw-r--r--   0        0        0     4204 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/moby_distribution/spec/endpoint.py
+-rw-r--r--   0        0        0     3757 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/moby_distribution/spec/image_json.py
+-rw-r--r--   0        0        0     4594 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/moby_distribution/spec/manifest.py
+-rw-r--r--   0        0        0      914 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     8027 1970-01-01 00:00:00.000000 moby_distribution-0.6.0/PKG-INFO
```

### Comparing `moby_distribution-0.5.9/LICENSE` & `moby_distribution-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.5.9/README.md` & `moby_distribution-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.5.9/moby_distribution/__init__.py` & `moby_distribution-0.6.0/moby_distribution/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from moby_distribution.registry.resources.image import ImageRef, LayerRef
 from moby_distribution.registry.resources.manifests import ManifestRef
 from moby_distribution.registry.resources.tags import Tags
 from moby_distribution.spec.endpoint import OFFICIAL_ENDPOINT, APIEndpoint
 from moby_distribution.spec.image_json import ImageJSON
 from moby_distribution.spec.manifest import ManifestSchema1, ManifestSchema2, OCIManifestSchema1
 
-__version__ = "0.5.9"
+__version__ = "0.6.0"
 __ALL__ = [
     "DockerRegistryV2Client",
     "Blob",
     "ManifestRef",
     "Tags",
     "APIEndpoint",
     "ManifestSchema1",
```

### Comparing `moby_distribution-0.5.9/moby_distribution/registry/auth.py` & `moby_distribution-0.6.0/moby_distribution/registry/auth.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 import logging
 from typing import Any, Dict, Optional
 
 import requests
 from www_authenticate import parse
 
 from moby_distribution.registry.exceptions import AuthFailed
+from moby_distribution.registry.utils import TypeTimeout
 from moby_distribution.spec.auth import TokenResponse
 
-AUTH_TIMEOUT = 60 * 3
+AUTH_TIMEOUT = 30
 logger = logging.getLogger(__name__)
 
 
 class AuthorizationProvider:
     def provide(self) -> str:
         """Provide the 'Authorization' used in HTTP Headers
 
@@ -31,15 +32,17 @@
 
     @property
     def www_authenticate(self):
         if self._www_authenticate is None:
             self._www_authenticate = parse(self._raw_www_authenticate)
         return self._www_authenticate
 
-    def authenticate(self, username: Optional[str] = None, password: Optional[str] = None) -> AuthorizationProvider:
+    def authenticate(
+        self, username: Optional[str] = None, password: Optional[str] = None, *, timeout: TypeTimeout = AUTH_TIMEOUT
+    ) -> AuthorizationProvider:
         raise NotImplementedError
 
     @property
     def raw_www_authenticate(self) -> str:
         return self._raw_www_authenticate
 
 
@@ -69,15 +72,17 @@
             return f"{self.token_type} {self.token_response.access_token}"
         raise ValueError("Missing Token")
 
 
 class HTTPBasicAuthentication(BaseAuthentication):
     """`HTTP Basic Authentication` Authenticator"""
 
-    def authenticate(self, username: Optional[str] = None, password: Optional[str] = None) -> AuthorizationProvider:
+    def authenticate(
+        self, username: Optional[str] = None, password: Optional[str] = None, *, timeout: TypeTimeout = AUTH_TIMEOUT
+    ) -> AuthorizationProvider:
         if username is None or password is None:
             raise AuthFailed(
                 message="请提供用户名和密码",
                 status_code=400,
                 response=None,
             )
         return BasicAuthAuthorizationProvider(username, password)
@@ -104,15 +109,17 @@
         for key in self.REQUIRE_KEYS:
             assert key in self.bearer
 
         self.backend = self.bearer["realm"]
         self.service = self.bearer["service"]
         self.scope = self.bearer.get("scope", None)
 
-    def authenticate(self, username: Optional[str] = None, password: Optional[str] = None) -> AuthorizationProvider:
+    def authenticate(
+        self, username: Optional[str] = None, password: Optional[str] = None, *, timeout: TypeTimeout = AUTH_TIMEOUT
+    ) -> AuthorizationProvider:
         """Authenticate to the registry.
         If no username and password provided, will authenticate as the anonymous user.
 
         :param username: User name to authenticate as.
         :param password: User's password.
         :return:
         """
@@ -126,26 +133,30 @@
         if username and password:
             auth = base64.b64encode(f"{username}:{password}".encode()).decode()
             headers["Authorization"] = f"Basic {auth}"
         elif any([username, password]) and not all([username, password]):
             logger.warning("请同时提供 username 和 password!")
 
         logger.info("sending authentication request to authorization service<%s>", self.backend)
-        resp = requests.get(self.backend, headers=headers, params=params, timeout=AUTH_TIMEOUT)
+        resp = requests.get(self.backend, headers=headers, params=params, timeout=timeout)
         if resp.status_code != 200:
             raise AuthFailed(
                 message="用户凭证校验失败, 请检查用户信息和操作权限",
                 status_code=resp.status_code,
                 response=resp,
             )
         return TokenAuthorizationProvider(TokenResponse(**resp.json()))
 
 
 class UniversalAuthentication(BaseAuthentication):
     """An Auto auth backend, which will auto auth by `scheme` provided by www_authenticate"""
 
-    def authenticate(self, username: Optional[str] = None, password: Optional[str] = None) -> AuthorizationProvider:
+    def authenticate(
+        self, username: Optional[str] = None, password: Optional[str] = None, *, timeout: TypeTimeout = AUTH_TIMEOUT
+    ) -> AuthorizationProvider:
         if "basic" in self.www_authenticate:
-            return HTTPBasicAuthentication(self.raw_www_authenticate).authenticate(username, password)
+            return HTTPBasicAuthentication(self.raw_www_authenticate).authenticate(username, password, timeout=timeout)
         elif "bearer" in self.www_authenticate:
-            return DockerRegistryTokenAuthentication(self.raw_www_authenticate).authenticate(username, password)
+            return DockerRegistryTokenAuthentication(self.raw_www_authenticate).authenticate(
+                username, password, timeout=timeout
+            )
         raise NotImplementedError("未支持的认证方式")
```

### Comparing `moby_distribution-0.5.9/moby_distribution/registry/client.py` & `moby_distribution-0.6.0/moby_distribution/registry/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,56 +25,63 @@
     def from_api_endpoint(
         cls,
         api_endpoint: APIEndpoint = OFFICIAL_ENDPOINT,
         username: Optional[str] = None,
         password: Optional[str] = None,
         authenticator_class: Type[BaseAuthentication] = UniversalAuthentication,
         default_timeout: TypeTimeout = 60 * 10,
-        https_detect_timeout: float = 10,
+        https_detect_timeout: float = 30,
+        auth_timeout: TypeTimeout = 30,
     ):
         https_scheme = "https://"
         http_scheme = "http://"
         enable_https, certificate_valid = api_endpoint.is_secure_repository(timeout=https_detect_timeout)
         if enable_https:
             client = cls(
                 api_base_url=f"{https_scheme}{api_endpoint.api_base_url}",
                 username=username,
                 password=password,
                 verify_certificate=certificate_valid,
                 authenticator_class=authenticator_class,
                 default_timeout=default_timeout,
+                auth_timeout=auth_timeout,
             )
             if certificate_valid or client.ping():
                 return client
         return cls(
             api_base_url=f"{http_scheme}{api_endpoint.api_base_url}",
             username=username,
             password=password,
             verify_certificate=False,
             authenticator_class=authenticator_class,
             default_timeout=default_timeout,
+            auth_timeout=auth_timeout,
         )
 
     def __init__(
         self,
         api_base_url: str,
         username: Optional[str] = None,
         password: Optional[str] = None,
         verify_certificate: bool = True,
         authenticator_class: Type[BaseAuthentication] = UniversalAuthentication,
         default_timeout: TypeTimeout = 60 * 10,
+        auth_timeout: TypeTimeout = 30,
     ):
         if default_timeout is not None and not isinstance(default_timeout, tuple) and isinf(default_timeout):
             raise ValueError("default_timeout should not be infinity.")
+        if auth_timeout is not None and not isinstance(auth_timeout, tuple) and isinf(auth_timeout):
+            raise ValueError("auth_timeout should not be infinity.")
         if api_base_url.endswith("/"):
             api_base_url = api_base_url.rstrip("/")
         self.api_base_url = api_base_url
         self.session = requests.session()
         self.session.verify = verify_certificate
         self.default_timeout = default_timeout
+        self.auth_timeout = auth_timeout
 
         self.username = username
         self.password = password
         self.authenticator_class = authenticator_class
         self._authed: Optional[AuthorizationProvider] = None
 
     def ping(self) -> bool:
@@ -137,15 +144,17 @@
         except Exception:
             curl = "<unknown>"
 
         if resp.status_code == 401:
             if auto_auth:
                 www_authenticate = resp.headers["www-authenticate"]
                 auth = self.authenticator_class(www_authenticate)
-                self._authed = auth.authenticate(username=self.username, password=self.password)
+                self._authed = auth.authenticate(
+                    username=self.username, password=self.password, timeout=self.auth_timeout
+                )
                 raise exceptions.RetryAgain
 
             logger.debug("Requesting %s, but PermissionDeny, Equivalent curl command: %s", url, curl)
             raise exceptions.PermissionDeny
 
         if resp.status_code == 403:
             if auto_auth and self._authed is None and self.ping():
```

### Comparing `moby_distribution-0.5.9/moby_distribution/registry/exceptions.py` & `moby_distribution-0.6.0/moby_distribution/registry/exceptions.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.5.9/moby_distribution/registry/resources/__init__.py` & `moby_distribution-0.6.0/moby_distribution/registry/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.5.9/moby_distribution/registry/resources/blobs.py` & `moby_distribution-0.6.0/moby_distribution/registry/resources/blobs.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.5.9/moby_distribution/registry/resources/image.py` & `moby_distribution-0.6.0/moby_distribution/registry/resources/image.py`

 * *Files 3% similar despite different names*

```diff
@@ -128,14 +128,15 @@
                 to_repo = named.name
 
             if to_reference is None:
                 to_reference = named.tag or "latest"
 
             layers = []
             for layer in manifest.Layers:
+                # gzip it for smaller size
                 gzipped_filepath = workplace / (layer + ".gz")
                 with (workplace / layer).open(mode="rb") as fh, gzip.open(gzipped_filepath, mode="wb") as compressed:
                     shutil.copyfileobj(fh, compressed)
 
                 # The gzipped file can only be obtained after the compressed object is closed
                 # (because the gzip context information has not yet been written).
                 gzipped_signer = HashSignWrapper()
@@ -222,55 +223,61 @@
         """
         if not layer.exists and not layer.local_path:
             raise ValueError("Unknown layer")
 
         uncompressed_tarball_signer = HashSignWrapper()
         # Add local layer
         if layer.local_path:
-            # Step 1: calculate the sha256 sum for the gzipped_tarball
-            gzipped_signer = HashSignWrapper()
+            # Step 1: calculate the sha256 sum for the tarball file
+            raw_tarball_signer = HashSignWrapper()
             with layer.local_path.open(mode="rb") as gzipped:
-                shutil.copyfileobj(gzipped, gzipped_signer)
-                size = gzipped_signer.tell()
+                shutil.copyfileobj(gzipped, raw_tarball_signer)
+                size = raw_tarball_signer.tell()
 
             # Step 2: calculate the sha256 sum for the uncompressed_tarball
-            with gzip.open(filename=layer.local_path) as uncompressed:
-                shutil.copyfileobj(uncompressed, uncompressed_tarball_signer)
+            # for gzipped tarball, we need decompress first
+            try:
+                with gzip.open(filename=layer.local_path) as uncompressed:
+                    shutil.copyfileobj(uncompressed, uncompressed_tarball_signer)
+            except OSError:
+                uncompressed_tarball_signer = raw_tarball_signer
 
-            if layer.digest and layer.digest != gzipped_signer.digest():
+            if layer.digest and layer.digest != raw_tarball_signer.digest():
                 raise ValueError(
                     "Wrong digest, layer.digest<'%s'> != signer.digest<'%s'>",
                     layer.digest,
-                    gzipped_signer.digest(),
+                    raw_tarball_signer.digest(),
                 )
 
-            layer.digest = gzipped_signer.digest()
+            layer.digest = raw_tarball_signer.digest()
             layer.repo = self.repo
             layer.size = size
 
         # Add remote layer if the layer is exists in registry
         else:
             with generate_temp_dir() as temp_dir:
                 # Step 1: calculate the sha256 sum for the gzipped_tarball
                 with (temp_dir / "blob").open(mode="wb") as fh:
-                    gzipped_signer = HashSignWrapper(fh=fh)
-                    Blob(repo=layer.repo, digest=layer.digest, fileobj=gzipped_signer, client=self.client).download()
-                    size = gzipped_signer.tell()
+                    raw_tarball_signer = HashSignWrapper(fh=fh)
+                    Blob(
+                        repo=layer.repo, digest=layer.digest, fileobj=raw_tarball_signer, client=self.client
+                    ).download()
+                    size = raw_tarball_signer.tell()
 
                 # Step 2: calculate the sha256 sum for the uncompressed_tarball
                 with gzip.open(filename=(temp_dir / "blob")) as uncompressed:
                     shutil.copyfileobj(uncompressed, uncompressed_tarball_signer)
 
             if layer.size != size:
                 raise ValueError("Wrong Size, layer.size<'%d'> != signer.size<'%d'>", layer.size, size)
-            if layer.digest != gzipped_signer.digest():
+            if layer.digest != raw_tarball_signer.digest():
                 raise ValueError(
                     "Wrong digest, layer.digest<'%s'> != signer.digest<'%s'>",
                     layer.digest,
-                    gzipped_signer.digest(),
+                    raw_tarball_signer.digest(),
                 )
 
         self._dirty = True
         self._append_diff_ids.append(uncompressed_tarball_signer.digest())
         self._append_historys.append(
             history
             or History(
@@ -279,15 +286,15 @@
                 created=default_created(),
                 empty_layer=False,
             )
         )
         self.layers.append(layer)
 
         return DockerManifestLayerDescriptor(
-            digest=gzipped_signer.digest(),
+            digest=raw_tarball_signer.digest(),
             size=size,
         )
 
     @property
     def image_json(self) -> ImageJSON:
         base = ImageJSON(**json.loads(self._initial_config))
         if not self._dirty:
```

### Comparing `moby_distribution-0.5.9/moby_distribution/registry/resources/manifests.py` & `moby_distribution-0.6.0/moby_distribution/registry/resources/manifests.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.5.9/moby_distribution/registry/resources/tags.py` & `moby_distribution-0.6.0/moby_distribution/registry/resources/tags.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.5.9/moby_distribution/registry/utils.py` & `moby_distribution-0.6.0/moby_distribution/registry/utils.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.5.9/moby_distribution/spec/auth.py` & `moby_distribution-0.6.0/moby_distribution/spec/auth.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.5.9/moby_distribution/spec/base.py` & `moby_distribution-0.6.0/moby_distribution/spec/base.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.5.9/moby_distribution/spec/endpoint.py` & `moby_distribution-0.6.0/moby_distribution/spec/endpoint.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,68 @@
 import re
 import socket
 import ssl
+from functools import wraps
 from typing import Optional, Pattern, Tuple
 
-from pydantic import BaseModel
+from pydantic import VERSION, BaseModel
+
+_endpoint_status_cache = {
+    # well-known endpoints
+    "registry.hub.docker.com": (True, True),
+    "index.docker.io": (True, True),
+    "quay.io": (True, True),
+}
+
+
+def cache_endpoint_status(func):
+    @wraps(func)
+    def is_secure_repository(self, *, timeout: Optional[float] = None):
+        if self.url in _endpoint_status_cache:
+            return _endpoint_status_cache[self.url]
+        _endpoint_status_cache[self.url] = func(self, timeout=timeout)
+        return _endpoint_status_cache[self.url]
+
+    return is_secure_repository
+
+
+class cached_property:
+    """
+    Decorator that converts a method with a single self argument into
+    a property cached on the instance.
+    """
+
+    # NOTE: implementation borrowed from Django.
+    # NOTE: we use fget, fset and fdel attributes to mimic @property.
+    fset = fdel = None
+
+    def __init__(self, fget):
+        self.fget = fget
+        self.__doc__ = getattr(fget, '__doc__')
+
+    def __get__(self, instance, type=None):
+        if instance is None:
+            return self
+        res = instance.__dict__[self.fget.__name__] = self.fget(instance)
+        return res
 
 
 class APIEndpoint(BaseModel):
     version: int = 2
     url: str
     official: bool = False
 
+    class Config:
+        arbitrary_types_allowed = True
+        if VERSION.startswith("1."):
+            keep_untouched = (cached_property,)
+        else:
+            ignored_types = (cached_property,)
+
+    @cache_endpoint_status
     def is_secure_repository(self, *, timeout: Optional[float] = None) -> Tuple[bool, bool]:
         """Detect if the repository is secure
 
         returns Tuple[bool, bool], the first one mean if the server support https?,
                                     the second one mean if the ssl certificate is valid?
         """
         match = url_regex().match(self.url)
@@ -37,15 +85,15 @@
             return False, False
         except socket.timeout:
             raise
         except OSError:
             return False, False
         return True, True
 
-    @property
+    @cached_property
     def api_base_url(self) -> str:
         match = url_regex().match(self.url)
         if not match:
             raise ValueError("Invalid Url")
 
         parts = match.groupdict()
         hostname = parts["domain"] or parts["ipv4"] or parts["ipv6"]
```

### Comparing `moby_distribution-0.5.9/moby_distribution/spec/image_json.py` & `moby_distribution-0.6.0/moby_distribution/spec/image_json.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.5.9/moby_distribution/spec/manifest.py` & `moby_distribution-0.6.0/moby_distribution/spec/manifest.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.5.9/pyproject.toml` & `moby_distribution-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "moby-distribution"
-version = "0.5.9"
+version = "0.6.0"
 description = "Yet another moby(docker) distribution implement by python."
 authors = ["shabbywu <shabbywu@qq.com>"]
 license = "Apache-2.0"
 
 readme = "README.md"
 repository = "https://github.com/shabbywu/distribution"
 homepage = "https://github.com/shabbywu/distribution"
```

### Comparing `moby_distribution-0.5.9/PKG-INFO` & `moby_distribution-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moby-distribution
-Version: 0.5.9
+Version: 0.6.0
 Summary: Yet another moby(docker) distribution implement by python.
 Home-page: https://github.com/shabbywu/distribution
 License: Apache-2.0
 Author: shabbywu
 Author-email: shabbywu@qq.com
 Requires-Python: >=3.6.2,<4
 Classifier: License :: OSI Approved :: Apache Software License
```

