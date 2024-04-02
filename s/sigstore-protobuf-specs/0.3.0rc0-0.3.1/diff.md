# Comparing `tmp/sigstore_protobuf_specs-0.3.0rc0.tar.gz` & `tmp/sigstore_protobuf_specs-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigstore_protobuf_specs-0.3.0rc0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sigstore_protobuf_specs-0.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sigstore_protobuf_specs-0.3.0rc0.tar` & `sigstore_protobuf_specs-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    11358 2024-01-18 02:28:05.480022 sigstore_protobuf_specs-0.3.0rc0/LICENSE
--rw-r--r--   0        0        0      216 2024-01-18 02:28:05.480022 sigstore_protobuf_specs-0.3.0rc0/README.md
--rw-r--r--   0        0        0     1194 2024-01-18 02:28:05.480022 sigstore_protobuf_specs-0.3.0rc0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-18 02:28:05.480022 sigstore_protobuf_specs-0.3.0rc0/sigstore_protobuf_specs/__init__.py
--rw-r--r--   0        0        0        0 2024-01-18 02:28:05.480022 sigstore_protobuf_specs-0.3.0rc0/sigstore_protobuf_specs/dev/__init__.py
--rw-r--r--   0        0        0        0 2024-01-18 02:28:05.480022 sigstore_protobuf_specs-0.3.0rc0/sigstore_protobuf_specs/dev/sigstore/__init__.py
--rw-r--r--   0        0        0        0 2024-01-18 02:28:05.480022 sigstore_protobuf_specs-0.3.0rc0/sigstore_protobuf_specs/dev/sigstore/bundle/__init__.py
--rw-r--r--   0        0        0     4429 2024-01-18 02:28:05.480022 sigstore_protobuf_specs-0.3.0rc0/sigstore_protobuf_specs/dev/sigstore/bundle/v1/__init__.py
--rw-r--r--   0        0        0        0 2024-01-18 02:28:05.480022 sigstore_protobuf_specs-0.3.0rc0/sigstore_protobuf_specs/dev/sigstore/common/__init__.py
--rw-r--r--   0        0        0     8332 2024-01-18 02:28:05.480022 sigstore_protobuf_specs-0.3.0rc0/sigstore_protobuf_specs/dev/sigstore/common/v1/__init__.py
--rw-r--r--   0        0        0        0 2024-01-18 02:28:05.480022 sigstore_protobuf_specs-0.3.0rc0/sigstore_protobuf_specs/dev/sigstore/events/__init__.py
--rw-r--r--   0        0        0     1763 2024-01-18 02:28:05.484022 sigstore_protobuf_specs-0.3.0rc0/sigstore_protobuf_specs/dev/sigstore/events/v1/__init__.py
--rw-r--r--   0        0        0        0 2024-01-18 02:28:05.484022 sigstore_protobuf_specs-0.3.0rc0/sigstore_protobuf_specs/dev/sigstore/rekor/__init__.py
--rw-r--r--   0        0        0     6355 2024-01-18 02:28:05.484022 sigstore_protobuf_specs-0.3.0rc0/sigstore_protobuf_specs/dev/sigstore/rekor/v1/__init__.py
--rw-r--r--   0        0        0        0 2024-01-18 02:28:05.484022 sigstore_protobuf_specs-0.3.0rc0/sigstore_protobuf_specs/dev/sigstore/trustroot/__init__.py
--rw-r--r--   0        0        0     4879 2024-01-18 02:28:05.484022 sigstore_protobuf_specs-0.3.0rc0/sigstore_protobuf_specs/dev/sigstore/trustroot/v1/__init__.py
--rw-r--r--   0        0        0        0 2024-01-18 02:28:05.484022 sigstore_protobuf_specs-0.3.0rc0/sigstore_protobuf_specs/dev/sigstore/verification/__init__.py
--rw-r--r--   0        0        0     7370 2024-01-18 02:28:05.484022 sigstore_protobuf_specs-0.3.0rc0/sigstore_protobuf_specs/dev/sigstore/verification/v1/__init__.py
--rw-r--r--   0        0        0        0 2024-01-18 02:28:05.484022 sigstore_protobuf_specs-0.3.0rc0/sigstore_protobuf_specs/google/__init__.py
--rw-r--r--   0        0        0     2114 2024-01-18 02:28:05.484022 sigstore_protobuf_specs-0.3.0rc0/sigstore_protobuf_specs/google/api/__init__.py
--rw-r--r--   0        0        0        0 2024-01-18 02:28:05.484022 sigstore_protobuf_specs-0.3.0rc0/sigstore_protobuf_specs/io/__init__.py
--rw-r--r--   0        0        0     1450 2024-01-18 02:28:05.484022 sigstore_protobuf_specs-0.3.0rc0/sigstore_protobuf_specs/io/intoto/__init__.py
--rw-r--r--   0        0        0     1369 1970-01-01 00:00:00.000000 sigstore_protobuf_specs-0.3.0rc0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-04-02 17:45:06.452222 sigstore_protobuf_specs-0.3.1/LICENSE
+-rw-r--r--   0        0        0      216 2024-04-02 17:45:06.452222 sigstore_protobuf_specs-0.3.1/README.md
+-rw-r--r--   0        0        0     1191 2024-04-02 17:45:06.452222 sigstore_protobuf_specs-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-02 17:45:06.452222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 17:45:06.452222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 17:45:06.452222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/sigstore/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 17:45:06.452222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/sigstore/bundle/__init__.py
+-rw-r--r--   0        0        0     4571 2024-04-02 17:45:06.452222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/sigstore/bundle/v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 17:45:06.452222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/sigstore/common/__init__.py
+-rw-r--r--   0        0        0     9042 2024-04-02 17:45:06.452222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/sigstore/common/v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 17:45:06.452222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/sigstore/events/__init__.py
+-rw-r--r--   0        0        0     1763 2024-04-02 17:45:06.452222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/sigstore/events/v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 17:45:06.452222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/sigstore/rekor/__init__.py
+-rw-r--r--   0        0        0     6380 2024-04-02 17:45:06.452222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/sigstore/rekor/v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 17:45:06.456222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/sigstore/trustroot/__init__.py
+-rw-r--r--   0        0        0     8142 2024-04-02 17:45:06.456222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/sigstore/trustroot/v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 17:45:06.456222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/sigstore/verification/__init__.py
+-rw-r--r--   0        0        0     7370 2024-04-02 17:45:06.456222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/sigstore/verification/v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 17:45:06.456222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/google/__init__.py
+-rw-r--r--   0        0        0     2114 2024-04-02 17:45:06.456222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/google/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 17:45:06.456222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/io/__init__.py
+-rw-r--r--   0        0        0     1450 2024-04-02 17:45:06.456222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/io/intoto/__init__.py
+-rw-r--r--   0        0        0     1366 1970-01-01 00:00:00.000000 sigstore_protobuf_specs-0.3.1/PKG-INFO
```

### Comparing `sigstore_protobuf_specs-0.3.0rc0/LICENSE` & `sigstore_protobuf_specs-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sigstore_protobuf_specs-0.3.0rc0/pyproject.toml` & `sigstore_protobuf_specs-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "sigstore-protobuf-specs"
-version = "0.3.0rc0"
+version = "0.3.1"
 description = "A library for serializing and deserializing Sigstore messages"
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [
   { name = "Sigstore Authors", email = "sigstore-dev@googlegroups.com" },
 ]
 classifiers = [
```

### Comparing `sigstore_protobuf_specs-0.3.0rc0/sigstore_protobuf_specs/dev/sigstore/bundle/v1/__init__.py` & `sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/sigstore/bundle/v1/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,17 +76,19 @@
     """
 
 
 @dataclass(eq=False, repr=False)
 class Bundle(betterproto.Message):
     media_type: str = betterproto.string_field(1)
     """
-    MUST be application/vnd.dev.sigstore.bundle+json;version=0.1 or
-    application/vnd.dev.sigstore.bundle+json;version=0.2 or
-    application/vnd.dev.sigstore.bundle+json;version=0.3 when encoded as JSON.
+    MUST be application/vnd.dev.sigstore.bundle.v0.3+json when when encoded as
+    JSON. Clients must to be able to accept media type using the previously
+    defined formats: * application/vnd.dev.sigstore.bundle+json;version=0.1 *
+    application/vnd.dev.sigstore.bundle+json;version=0.2 *
+    application/vnd.dev.sigstore.bundle+json;version=0.3
     """
 
     verification_material: "VerificationMaterial" = betterproto.message_field(2)
     """
     When a signer is identified by a X.509 certificate, a verifier MUST verify
     that the signature was computed at the time the certificate was valid as
     described in the Sigstore client spec: "Verification using a Bundle". <http
```

### Comparing `sigstore_protobuf_specs-0.3.0rc0/sigstore_protobuf_specs/dev/sigstore/common/v1/__init__.py` & `sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/sigstore/common/v1/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,53 +30,65 @@
     SHA3_256 = 4
     SHA3_384 = 5
 
 
 class PublicKeyDetails(betterproto.Enum):
     """
     Details of a specific public key, capturing the the key encoding method,
-    and signature algorithm. To avoid the possibility of contradicting formats
-    such as PKCS1 with ED25519 the valid permutations are listed as a linear
-    set instead of a cartesian set (i.e one combined variable instead of two,
-    one for encoding and one for the signature algorithm).
+    and signature algorithm. PublicKeyDetails captures the public key/hash
+    algorithm combinations recommended in the Sigstore ecosystem. This is
+    modelled as a linear set as we want to provide a small number of
+    opinionated options instead of allowing every possible permutation. Any
+    changes to this enum MUST be reflected in the algorithm registry. See:
+    docs/algorithm-registry.md To avoid the possibility of contradicting
+    formats such as PKCS1 with ED25519 the valid permutations are listed as a
+    linear set instead of a cartesian set (i.e one combined variable instead of
+    two, one for encoding and one for the signature algorithm).
     """
 
     PUBLIC_KEY_DETAILS_UNSPECIFIED = 0
     PKCS1_RSA_PKCS1V5 = 1
     """RSA"""
 
     PKCS1_RSA_PSS = 2
     PKIX_RSA_PKCS1V5 = 3
     PKIX_RSA_PSS = 4
-    PKIX_ECDSA_P256_SHA_256 = 5
-    """ECDSA"""
+    PKIX_RSA_PKCS1V15_2048_SHA256 = 9
+    """RSA public key in PKIX format, PKCS#1v1.5 signature"""
 
+    PKIX_RSA_PKCS1V15_3072_SHA256 = 10
+    PKIX_RSA_PKCS1V15_4096_SHA256 = 11
+    PKIX_RSA_PSS_2048_SHA256 = 16
+    """RSA public key in PKIX format, RSASSA-PSS signature"""
+
+    PKIX_RSA_PSS_3072_SHA256 = 17
+    PKIX_RSA_PSS_4096_SHA256 = 18
     PKIX_ECDSA_P256_HMAC_SHA_256 = 6
+    """ECDSA"""
+
+    PKIX_ECDSA_P256_SHA_256 = 5
+    PKIX_ECDSA_P384_SHA_384 = 12
+    PKIX_ECDSA_P521_SHA_512 = 13
     PKIX_ED25519 = 7
     """Ed 25519"""
 
-
-class KnownSignatureAlgorithm(betterproto.Enum):
+    PKIX_ED25519_PH = 8
+    LMS_SHA256 = 14
     """
-    KnownSignatureAlgorithm captures the public key/hash algorithm combinations
-    recommended in the Sigstore ecosystem. This is modelled as a linear set as
-    we want to provide a small number of opinionated options instead of
-    allowing every possible permutation. Any changes to this enum MUST be
-    reflected in the algorithm registry. See: docs/algorithm-registry.md
+    LMS and LM-OTS These keys and signatures may be used by private Sigstore
+    deployments, but are not currently supported by the public good instance.
+    USER WARNING: LMS and LM-OTS are both stateful signature schemes. Using
+    them correctly requires discretion and careful consideration to ensure that
+    individual secret keys are not used more than once. In addition, LM-OTS is
+    a single-use scheme, meaning that it MUST NOT be used for more than one
+    signature per LM-OTS key. If you cannot maintain these invariants, you MUST
+    NOT use these schemes.
     """
 
-    KNOWN_SIGNATURE_ALGORITHM_UNSPECIFIED = 0
-    RSA_SIGN_PKCS1_2048_SHA256 = 1
-    RSA_SIGN_PKCS1_3072_SHA256 = 2
-    RSA_SIGN_PKCS1_4096_SHA256 = 3
-    ECDSA_SHA2_256_NISTP256 = 4
-    ECDSA_SHA2_384_NISTP384 = 5
-    ECDSA_SHA2_512_NISTP521 = 6
-    ED25519 = 7
-    ED25519_PH = 8
+    LMOTS_SHA256 = 15
 
 
 class SubjectAlternativeNameType(betterproto.Enum):
     SUBJECT_ALTERNATIVE_NAME_TYPE_UNSPECIFIED = 0
     EMAIL = 1
     URI = 2
     OTHER_NAME = 3
```

### Comparing `sigstore_protobuf_specs-0.3.0rc0/sigstore_protobuf_specs/dev/sigstore/events/v1/__init__.py` & `sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/sigstore/events/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore_protobuf_specs-0.3.0rc0/sigstore_protobuf_specs/dev/sigstore/rekor/v1/__init__.py` & `sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/sigstore/rekor/v1/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,22 +24,22 @@
     version: str = betterproto.string_field(2)
     """The specific api version of the type."""
 
 
 @dataclass(eq=False, repr=False)
 class Checkpoint(betterproto.Message):
     """
-    The checkpoint contains a signature of the tree head (root hash), size of
-    the tree, the transparency log's unique identifier (log ID), hostname and
-    the current time. The result is a string, the format is described here
-    https://github.com/transparency-dev/formats/blob/main/log/README.md The
-    details are here https://github.com/sigstore/rekor/blob/a6e58f72b6b18cc06ce
-    fe61808efd562b9726330/pkg/util/signed_note.go#L114 The signature has the
-    same format as InclusionPromise.signed_entry_timestamp. See below for more
-    details.
+    The checkpoint MUST contain a signature of the tree head (root hash), size
+    of the tree and the transparency log's unique identifier (log ID). It MAY
+    also be followed by any optional data. The result is a string,  the format
+    is described here https://github.com/transparency-
+    dev/formats/blob/main/log/README.md The details are here https://github.com
+    /sigstore/rekor/blob/a6e58f72b6b18cc06cefe61808efd562b9726330/pkg/util/sign
+    ed_note.go#L114 The signature has the same format as
+    InclusionPromise.signed_entry_timestamp. See below for more details.
     """
 
     envelope: str = betterproto.string_field(1)
 
 
 @dataclass(eq=False, repr=False)
 class InclusionProof(betterproto.Message):
```

### Comparing `sigstore_protobuf_specs-0.3.0rc0/sigstore_protobuf_specs/dev/sigstore/verification/v1/__init__.py` & `sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/sigstore/verification/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore_protobuf_specs-0.3.0rc0/sigstore_protobuf_specs/google/api/__init__.py` & `sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/google/api/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore_protobuf_specs-0.3.0rc0/sigstore_protobuf_specs/io/intoto/__init__.py` & `sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/io/intoto/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore_protobuf_specs-0.3.0rc0/PKG-INFO` & `sigstore_protobuf_specs-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigstore-protobuf-specs
-Version: 0.3.0rc0
+Version: 0.3.1
 Summary: A library for serializing and deserializing Sigstore messages
 Author-email: Sigstore Authors <sigstore-dev@googlegroups.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
```

