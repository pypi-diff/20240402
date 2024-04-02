# Comparing `tmp/didcomm_messaging-0.1.0a3.tar.gz` & `tmp/didcomm_messaging-0.1.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "didcomm_messaging-0.1.0a3.tar", last modified: Mon Jan  8 22:02:58 2024, max compression
+gzip compressed data, was "didcomm_messaging-0.1.0a4.tar", last modified: Wed Jan 24 19:48:03 2024, max compression
```

## Comparing `didcomm_messaging-0.1.0a3.tar` & `didcomm_messaging-0.1.0a4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    11357 2024-01-08 22:02:38.808870 didcomm_messaging-0.1.0a3/LICENSE
--rw-r--r--   0        0        0     3592 2024-01-08 22:02:38.808870 didcomm_messaging-0.1.0a3/README.md
--rw-r--r--   0        0        0     3329 2024-01-08 22:02:38.812870 didcomm_messaging-0.1.0a3/didcomm_messaging/__init__.py
--rw-r--r--   0        0        0      221 2024-01-08 22:02:38.812870 didcomm_messaging-0.1.0a3/didcomm_messaging/crypto/__init__.py
--rw-r--r--   0        0        0       52 2024-01-08 22:02:38.812870 didcomm_messaging-0.1.0a3/didcomm_messaging/crypto/backend/__init__.py
--rw-r--r--   0        0        0    14000 2024-01-08 22:02:38.812870 didcomm_messaging-0.1.0a3/didcomm_messaging/crypto/backend/askar.py
--rw-r--r--   0        0        0     7510 2024-01-08 22:02:38.812870 didcomm_messaging-0.1.0a3/didcomm_messaging/crypto/backend/authlib.py
--rw-r--r--   0        0        0      646 2024-01-08 22:02:38.812870 didcomm_messaging-0.1.0a3/didcomm_messaging/crypto/backend/basic.py
--rw-r--r--   0        0        0     4085 2024-01-08 22:02:38.812870 didcomm_messaging-0.1.0a3/didcomm_messaging/crypto/base.py
--rw-r--r--   0        0        0    15151 2024-01-08 22:02:38.812870 didcomm_messaging-0.1.0a3/didcomm_messaging/crypto/jwe.py
--rw-r--r--   0        0        0       42 2024-01-08 22:02:38.812870 didcomm_messaging-0.1.0a3/didcomm_messaging/multiformats/__init__.py
--rw-r--r--   0        0        0     3880 2024-01-08 22:02:38.812870 didcomm_messaging-0.1.0a3/didcomm_messaging/multiformats/multibase.py
--rw-r--r--   0        0        0     2109 2024-01-08 22:02:38.812870 didcomm_messaging-0.1.0a3/didcomm_messaging/multiformats/multicodec.py
--rw-r--r--   0        0        0     6753 2024-01-08 22:02:38.812870 didcomm_messaging-0.1.0a3/didcomm_messaging/packaging.py
--rw-r--r--   0        0        0     2487 2024-01-08 22:02:38.812870 didcomm_messaging-0.1.0a3/didcomm_messaging/resolver/__init__.py
--rw-r--r--   0        0        0     1227 2024-01-08 22:02:38.812870 didcomm_messaging-0.1.0a3/didcomm_messaging/resolver/peer.py
--rw-r--r--   0        0        0     5339 2024-01-08 22:02:38.812870 didcomm_messaging-0.1.0a3/didcomm_messaging/routing.py
--rw-r--r--   0        0        0     1589 2024-01-08 22:02:58.033075 didcomm_messaging-0.1.0a3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-08 22:02:38.812870 didcomm_messaging-0.1.0a3/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-01-08 22:02:38.812870 didcomm_messaging-0.1.0a3/tests/crypto/__init__.py
--rw-r--r--   0        0        0     6607 2024-01-08 22:02:38.812870 didcomm_messaging-0.1.0a3/tests/crypto/test_askar.py
--rw-r--r--   0        0        0     3154 2024-01-08 22:02:38.812870 didcomm_messaging-0.1.0a3/tests/crypto/test_askar_x_authlib.py
--rw-r--r--   0        0        0     2124 2024-01-08 22:02:38.812870 didcomm_messaging-0.1.0a3/tests/crypto/test_authlib.py
--rw-r--r--   0        0        0      740 2024-01-08 22:02:38.812870 didcomm_messaging-0.1.0a3/tests/test_didresolver.py
--rw-r--r--   0        0        0     2020 2024-01-08 22:02:38.812870 didcomm_messaging-0.1.0a3/tests/test_packaging.py
--rw-r--r--   0        0        0      771 2024-01-08 22:02:38.812870 didcomm_messaging-0.1.0a3/tests/test_secrets.py
--rw-r--r--   0        0        0     4314 1970-01-01 00:00:00.000000 didcomm_messaging-0.1.0a3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/LICENSE
+-rw-r--r--   0        0        0     3592 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/README.md
+-rw-r--r--   0        0        0     3329 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/didcomm_messaging/__init__.py
+-rw-r--r--   0        0        0      221 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/didcomm_messaging/crypto/__init__.py
+-rw-r--r--   0        0        0       52 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/didcomm_messaging/crypto/backend/__init__.py
+-rw-r--r--   0        0        0    14000 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/didcomm_messaging/crypto/backend/askar.py
+-rw-r--r--   0        0        0     7510 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/didcomm_messaging/crypto/backend/authlib.py
+-rw-r--r--   0        0        0      646 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/didcomm_messaging/crypto/backend/basic.py
+-rw-r--r--   0        0        0     4085 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/didcomm_messaging/crypto/base.py
+-rw-r--r--   0        0        0    15151 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/didcomm_messaging/crypto/jwe.py
+-rw-r--r--   0        0        0       42 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/didcomm_messaging/multiformats/__init__.py
+-rw-r--r--   0        0        0     3880 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/didcomm_messaging/multiformats/multibase.py
+-rw-r--r--   0        0        0     2264 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/didcomm_messaging/multiformats/multicodec.py
+-rw-r--r--   0        0        0     6753 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/didcomm_messaging/packaging.py
+-rw-r--r--   0        0        0     2487 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/didcomm_messaging/resolver/__init__.py
+-rw-r--r--   0        0        0     1227 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/didcomm_messaging/resolver/peer.py
+-rw-r--r--   0        0        0     5339 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/didcomm_messaging/routing.py
+-rw-r--r--   0        0        0     1589 2024-01-24 19:48:03.577793 didcomm_messaging-0.1.0a4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/tests/crypto/__init__.py
+-rw-r--r--   0        0        0     6607 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/tests/crypto/test_askar.py
+-rw-r--r--   0        0        0     3154 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/tests/crypto/test_askar_x_authlib.py
+-rw-r--r--   0        0        0     2124 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/tests/crypto/test_authlib.py
+-rw-r--r--   0        0        0      740 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/tests/test_didresolver.py
+-rw-r--r--   0        0        0     2020 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/tests/test_packaging.py
+-rw-r--r--   0        0        0      771 2024-01-24 19:47:42.929722 didcomm_messaging-0.1.0a4/tests/test_secrets.py
+-rw-r--r--   0        0        0     4314 1970-01-01 00:00:00.000000 didcomm_messaging-0.1.0a4/PKG-INFO
```

### Comparing `didcomm_messaging-0.1.0a3/LICENSE` & `didcomm_messaging-0.1.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.0a3/README.md` & `didcomm_messaging-0.1.0a4/README.md`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.0a3/didcomm_messaging/__init__.py` & `didcomm_messaging-0.1.0a4/didcomm_messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.0a3/didcomm_messaging/crypto/backend/askar.py` & `didcomm_messaging-0.1.0a4/didcomm_messaging/crypto/backend/askar.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.0a3/didcomm_messaging/crypto/backend/authlib.py` & `didcomm_messaging-0.1.0a4/didcomm_messaging/crypto/backend/authlib.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.0a3/didcomm_messaging/crypto/backend/basic.py` & `didcomm_messaging-0.1.0a4/didcomm_messaging/crypto/backend/basic.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.0a3/didcomm_messaging/crypto/base.py` & `didcomm_messaging-0.1.0a4/didcomm_messaging/crypto/base.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.0a3/didcomm_messaging/crypto/jwe.py` & `didcomm_messaging-0.1.0a4/didcomm_messaging/crypto/jwe.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.0a3/didcomm_messaging/multiformats/multibase.py` & `didcomm_messaging-0.1.0a4/didcomm_messaging/multiformats/multibase.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.0a3/didcomm_messaging/multiformats/multicodec.py` & `didcomm_messaging-0.1.0a4/didcomm_messaging/multiformats/multicodec.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,17 @@
     code: bytes
 
 
 class SupportedCodecs(Enum):
     """Enumeration of supported multicodecs."""
 
     ed25519_pub = Multicodec("ed25519-pub", b"\xed\x01")
+    ed25519_priv = Multicodec("ed25519-priv", b"\x80\x26")
     x25519_pub = Multicodec("x25519-pub", b"\xec\x01")
+    x25519_priv = Multicodec("x25519-priv", b"\x82\x26")
     bls12381g1 = Multicodec("bls12_381-g1-pub", b"\xea\x01")
     bls12381g2 = Multicodec("bls12_381-g2-pub", b"\xeb\x01")
     bls12381g1g2 = Multicodec("bls12_381-g1g2-pub", b"\xee\x01")
     secp256k1_pub = Multicodec("secp256k1-pub", b"\xe7\x01")
 
     @classmethod
     def by_name(cls, name: str) -> Multicodec:
@@ -36,15 +38,17 @@
             if data.startswith(codec.value.code):
                 return codec.value
         raise ValueError("Unsupported multicodec")
 
 
 MulticodecStr = Literal[
     "ed25519-pub",
+    "ed25519-priv",
     "x25519-pub",
+    "x25519-priv",
     "bls12_381-g1-pub",
     "bls12_381-g2-pub",
     "bls12_381-g1g2-pub",
     "secp256k1-pub",
 ]
```

### Comparing `didcomm_messaging-0.1.0a3/didcomm_messaging/packaging.py` & `didcomm_messaging-0.1.0a4/didcomm_messaging/packaging.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.0a3/didcomm_messaging/resolver/__init__.py` & `didcomm_messaging-0.1.0a4/didcomm_messaging/resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.0a3/didcomm_messaging/resolver/peer.py` & `didcomm_messaging-0.1.0a4/didcomm_messaging/resolver/peer.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.0a3/didcomm_messaging/routing.py` & `didcomm_messaging-0.1.0a4/didcomm_messaging/routing.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.0a3/pyproject.toml` & `didcomm_messaging-0.1.0a4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "didcomm-messaging"
-version = "0.1.0a3"
+version = "0.1.0a4"
 description = "DIDComm Messaging implemented with swappable backends."
 authors = [
     { name = "Daniel Bluhm", email = "dbluhm@pm.me" },
     { name = "Colton Wolkins", email = "colton@indicio.tech" },
     { name = "Micah Peltier", email = "micah@indicio.tech" },
 ]
 dependencies = [
```

### Comparing `didcomm_messaging-0.1.0a3/tests/crypto/test_askar.py` & `didcomm_messaging-0.1.0a4/tests/crypto/test_askar.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.0a3/tests/crypto/test_askar_x_authlib.py` & `didcomm_messaging-0.1.0a4/tests/crypto/test_askar_x_authlib.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.0a3/tests/crypto/test_authlib.py` & `didcomm_messaging-0.1.0a4/tests/crypto/test_authlib.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.0a3/tests/test_didresolver.py` & `didcomm_messaging-0.1.0a4/tests/test_didresolver.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.0a3/tests/test_packaging.py` & `didcomm_messaging-0.1.0a4/tests/test_packaging.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.0a3/tests/test_secrets.py` & `didcomm_messaging-0.1.0a4/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.0a3/PKG-INFO` & `didcomm_messaging-0.1.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: didcomm-messaging
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: DIDComm Messaging implemented with swappable backends.
 Author-Email: Daniel Bluhm <dbluhm@pm.me>, Colton Wolkins <colton@indicio.tech>, Micah Peltier <micah@indicio.tech>
 License: Apache-2.0
 Requires-Python: >=3.9
 Requires-Dist: base58>=2.1.1
 Requires-Dist: pydid>=0.4.2
 Requires-Dist: aries-askar>=0.2.9; extra == "askar"
```

