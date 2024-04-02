# Comparing `tmp/tablecache-3.2.0.tar.gz` & `tmp/tablecache-4.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablecache-3.2.0.tar", last modified: Sat Dec  2 12:34:44 2023, max compression
+gzip compressed data, was "tablecache-4.0.0rc0.tar", last modified: Tue Apr  2 05:13:26 2024, max compression
```

## Comparing `tablecache-3.2.0.tar` & `tablecache-4.0.0rc0.tar`

### file list

```diff
@@ -1,31 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 12:34:44.220553 tablecache-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2023-12-02 12:34:33.000000 tablecache-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-02 12:34:33.000000 tablecache-3.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6349 2023-12-02 12:34:44.220553 tablecache-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5565 2023-12-02 12:34:33.000000 tablecache-3.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      177 2023-12-02 12:34:33.000000 tablecache-3.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 12:34:44.216553 tablecache-3.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-02 12:34:33.000000 tablecache-3.2.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-02 12:34:33.000000 tablecache-3.2.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-12-02 12:34:33.000000 tablecache-3.2.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-02 12:34:44.220553 tablecache-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2023-12-02 12:34:33.000000 tablecache-3.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 12:34:44.220553 tablecache-3.2.0/tablecache/
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2023-12-02 12:34:33.000000 tablecache-3.2.0/tablecache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11350 2023-12-02 12:34:33.000000 tablecache-3.2.0/tablecache/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     9297 2023-12-02 12:34:33.000000 tablecache-3.2.0/tablecache/codec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2023-12-02 12:34:33.000000 tablecache-3.2.0/tablecache/db.py
--rw-r--r--   0 runner    (1001) docker     (127)    18323 2023-12-02 12:34:33.000000 tablecache-3.2.0/tablecache/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     8089 2023-12-02 12:34:33.000000 tablecache-3.2.0/tablecache/subset.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2023-12-02 12:34:33.000000 tablecache-3.2.0/tablecache/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 12:34:44.220553 tablecache-3.2.0/tablecache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6349 2023-12-02 12:34:44.000000 tablecache-3.2.0/tablecache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      509 2023-12-02 12:34:44.000000 tablecache-3.2.0/tablecache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-02 12:34:44.000000 tablecache-3.2.0/tablecache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      182 2023-12-02 12:34:44.000000 tablecache-3.2.0/tablecache.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-02 12:34:44.000000 tablecache-3.2.0/tablecache.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 12:34:44.220553 tablecache-3.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    20636 2023-12-02 12:34:33.000000 tablecache-3.2.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    13607 2023-12-02 12:34:33.000000 tablecache-3.2.0/tests/test_codec.py
--rw-r--r--   0 runner    (1001) docker     (127)     8923 2023-12-02 12:34:33.000000 tablecache-3.2.0/tests/test_db.py
--rw-r--r--   0 runner    (1001) docker     (127)    28601 2023-12-02 12:34:33.000000 tablecache-3.2.0/tests/test_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 05:13:26.653800 tablecache-4.0.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-02 05:13:26.653800 tablecache-4.0.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 05:13:26.645800 tablecache-4.0.0rc0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/requirements/local.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/requirements/postgres.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/requirements/redis.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 05:13:26.653800 tablecache-4.0.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 05:13:26.645800 tablecache-4.0.0rc0/tablecache/
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/tablecache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24310 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/tablecache/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/tablecache/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/tablecache/index.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 05:13:26.645800 tablecache-4.0.0rc0/tablecache/local/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/tablecache/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14058 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/tablecache/local/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 05:13:26.645800 tablecache-4.0.0rc0/tablecache/postgres/
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/tablecache/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/tablecache/postgres/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 05:13:26.645800 tablecache-4.0.0rc0/tablecache/redis/
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/tablecache/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/tablecache/redis/codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35091 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/tablecache/redis/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/tablecache/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/tablecache/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 05:13:26.649800 tablecache-4.0.0rc0/tablecache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-02 05:13:26.000000 tablecache-4.0.0rc0/tablecache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-02 05:13:26.000000 tablecache-4.0.0rc0/tablecache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 05:13:26.000000 tablecache-4.0.0rc0/tablecache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-02 05:13:26.000000 tablecache-4.0.0rc0/tablecache.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 05:13:26.000000 tablecache-4.0.0rc0/tablecache.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 05:13:26.649800 tablecache-4.0.0rc0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    62150 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/tests/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16610 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/tests/test_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-04-02 05:13:23.000000 tablecache-4.0.0rc0/tests/test_storage.py
```

### Comparing `tablecache-3.2.0/LICENSE` & `tablecache-4.0.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `tablecache-3.2.0/tablecache/codec.py` & `tablecache-4.0.0rc0/tablecache/redis/codec.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,35 +26,51 @@
 
 class Codec[T](abc.ABC):
     """
     Abstract base for codecs.
 
     A codec can encode certain values to bytes, then decode those back to the
     original value.
-
-    If an input value for encoding or decoding is unsuitable in any way, a
-    ValueError is raised.
     """
+
     @abc.abstractmethod
     def encode(self, value: T) -> bytes:
+        """
+        Encode the value to bytes.
+
+        :param value: The value to encode.
+        :return: A representation of the input value as bytes.
+        :raise ValueError: If the input value is invalid and can't be encoded.
+        """
         raise NotImplementedError
 
     @abc.abstractmethod
     def decode(self, bs: bytes) -> T:
+        """
+        Decode the bytes to a value.
+
+        :param bs: A :py:class:`bytes` object containing an encoded value.
+        :return: The decoded value
+        :raise ValueError: If the input is invalid and can't be decoded.
+        """
         raise NotImplementedError
 
 
 class Nullable[T](Codec[t.Optional[T]]):
     """
     Wrapper codec that allows representing nullable values.
 
     Encodes optional values by using an inner codec for values, and a marker
     for None.
     """
+
     def __init__(self, value_codec: Codec[T]):
+        """
+        :param value_codec: Wrapped codec to encode and decode values.
+        """
         self._value_codec = value_codec
 
     @t.override
     def encode(self, value: t.Optional[T]) -> bytes:
         if value is None:
             return b'\x00'
         return b'\x01' + self._value_codec.encode(value)
@@ -70,15 +86,19 @@
     """
     Wrapper codec that allows representing arrays (i.e. lists).
 
     Encodes elements using an inner codec. The length of each element is
     encoded using a 16-bit unsigned integer, so elements must not be over 65535
     bytes long.
     """
+
     def __init__(self, value_codec: Codec[T]):
+        """
+        :param value_codec: Wrapped codec to encode and decode array values.
+        """
         self._value_codec = value_codec
         self._length_codec = UnsignedInt16Codec()
 
     @t.override
     def encode(self, values: list[T]) -> bytes:
         if not isinstance(values, list):
             raise ValueError('Value must be a list.')
@@ -115,15 +135,15 @@
             return False
         if bs == b'\x01':
             return True
         raise ValueError('Invalid bool representation.')
 
 
 class StringCodec(Codec[str]):
-    """Simple str<->bytest codec (UTF-8)."""
+    """Simple str<->bytes codec (UTF-8)."""
     @t.override
     def encode(self, value: str) -> bytes:
         if not isinstance(value, str):
             raise ValueError('Value is not a string.')
         return value.encode()
 
     @t.override
@@ -160,14 +180,15 @@
     @t.override
     def decode(self, bs: bytes) -> numbers.Real:
         return float(bs.decode())
 
 
 class EncodedNumberCodec[T: numbers.Number](Codec[T]):
     """Codec that encodes numbers to bytes directly."""
+
     def __init__(self, struct_format: str) -> None:
         self._struct_format = struct_format
 
     @t.override
     def encode(self, value: T) -> bytes:
         try:
             return struct.pack(self._struct_format, value)
@@ -229,31 +250,31 @@
 
 class EncodedFloatCodec(EncodedNumberCodec[numbers.Real]):
     """
     Codec that encodes floats to bytes directly.
 
     Infinities and NaNs are handled. Signalling NaNs mostly work, with the
     exception that the most significant bit of the signalling part is always 1
-    (i.e. single-precision NaNs always start with 7fc or ffc, and double
-    precision with 7ff8 or fff8).
+    (i.e. single-precision NaNs always start with ``7fc`` or ``ffc``, and
+    double precision with ``7ff8`` or ``fff8``).
     """
 
 
 class Float32Codec(EncodedFloatCodec):
     _min_value, = struct.unpack('>f', bytes.fromhex('ff7fffff'))
     _max_value, = struct.unpack('>f', bytes.fromhex('7f7fffff'))
 
     def __init__(self) -> None:
         super().__init__('>f')
 
     @t.override
     def encode(self, value: numbers.Real) -> bytes:
         encoded = super().encode(value)
-        if not math.isinf(value) and (value < self._min_value
-                                      or value > self._max_value):
+        if not math.isinf(value) and (value < self._min_value or
+                                      value > self._max_value):
             raise ValueError('Value is outside of float32 range.')
         return encoded
 
 
 class Float64Codec(EncodedFloatCodec):
     def __init__(self) -> None:
         super().__init__('>d')
@@ -279,14 +300,15 @@
     Encodes values as an epoch timestamp in a double precision float, so
     precision is limited to that value range.
 
     Only timezone-naive datetimes ones in timezone UTC can be encoded. Any
     other value results in a ValueError. Naive datetimes are treated as though
     they are UTC. When decoding datetimes in UTC are returned.
     """
+
     def __init__(self):
         self._float_codec = Float64Codec()
 
     @t.override
     def encode(self, value: datetime.datetime) -> bytes:
         if not isinstance(value, datetime.datetime):
             raise ValueError('Value is not a datetime.')
```

### Comparing `tablecache-3.2.0/tablecache/types.py` & `tablecache-4.0.0rc0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,26 @@
-# Copyright 2023 Marc Lehmann
+# tablecache
 
-# This file is part of tablecache.
-#
-# tablecache is free software: you can redistribute it and/or modify it under
-# the terms of the GNU Affero General Public License as published by the Free
-# Software Foundation, either version 3 of the License, or (at your option) any
-# later version.
-#
-# tablecache is distributed in the hope that it will be useful, but WITHOUT ANY
-# WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
-# A PARTICULAR PURPOSE. See the GNU Affero General Public License for more
-# details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with tablecache. If not, see <https://www.gnu.org/licenses/>.
+Simple cache for unwieldily joined relations.
 
-import collections.abc as ca
-import typing as t
+## Copyright and license
 
-type Record = ca.Mapping[str, t.Any]
-type Records = ca.AsyncIterator[Record]
+Copyright 2023, 2024 Marc Lehmann
+
+This file is part of tablecache.
+
+tablecache is free software: you can redistribute it and/or modify it under the
+terms of the GNU Affero General Public License as published by the Free
+Software Foundation, either version 3 of the License, or (at your option) any
+later version.
+
+tablecache is distributed in the hope that it will be useful, but WITHOUT ANY
+WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
+PARTICULAR PURPOSE. See the GNU Affero General Public License for more details.
+
+You should have received a copy of the GNU Affero General Public License along
+with tablecache. If not, see <https://www.gnu.org/licenses/>.
+
+## Documentation
+
+For documentation, please see
+[readthedocs](https://tablecache.readthedocs.io/).
```

