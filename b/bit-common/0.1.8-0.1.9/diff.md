# Comparing `tmp/bit_common-0.1.8.tar.gz` & `tmp/bit_common-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bit_common-0.1.8.tar", max compression
+gzip compressed data, was "bit_common-0.1.9.tar", max compression
```

## Comparing `bit_common-0.1.8.tar` & `bit_common-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1385 2024-03-22 23:31:16.439317 bit_common-0.1.8/README.md
--rw-r--r--   0        0        0        0 2024-03-26 16:26:56.207758 bit_common-0.1.8/bit/__init__.py
--rw-r--r--   0        0        0     1632 2024-03-26 21:37:25.770757 bit_common-0.1.8/bit/controller.py
--rw-r--r--   0        0        0      388 2024-03-26 20:39:50.846638 bit_common-0.1.8/bit/middleware.py
--rw-r--r--   0        0        0     6591 2024-03-26 20:41:10.671124 bit_common-0.1.8/bit/model.py
--rw-r--r--   0        0        0     2369 2024-03-26 21:50:42.914649 bit_common-0.1.8/bit/protocol.py
--rw-r--r--   0        0        0        0 2024-03-26 20:45:59.857611 bit_common-0.1.8/bit/py.typed
--rw-r--r--   0        0        0        0 2024-03-26 16:24:14.359356 bit_common-0.1.8/bit/type/__init__.py
--rw-r--r--   0        0        0     6124 2024-03-28 16:30:19.172825 bit_common-0.1.8/bit/type/base.py
--rw-r--r--   0        0        0     2512 2024-03-22 17:33:58.201946 bit_common-0.1.8/bit/type/bitarray.py
--rw-r--r--   0        0        0     1341 2024-03-26 20:50:15.568290 bit_common-0.1.8/bit/type/endian.py
--rw-r--r--   0        0        0     5541 2024-03-26 20:02:05.853515 bit_common-0.1.8/bit/type/integer.py
--rw-r--r--   0        0        0      997 2024-03-28 15:50:23.893007 bit_common-0.1.8/bit/type/network.py
--rw-r--r--   0        0        0     3677 2024-03-26 20:03:49.710103 bit_common-0.1.8/bit/type/string.py
--rw-r--r--   0        0        0      994 2024-03-28 16:30:25.006483 bit_common-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1801 1970-01-01 00:00:00.000000 bit_common-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1390 2024-03-30 20:24:43.009557 bit_common-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2024-03-26 16:26:56.207758 bit_common-0.1.9/bit/__init__.py
+-rw-r--r--   0        0        0     1632 2024-03-26 21:37:25.770757 bit_common-0.1.9/bit/controller.py
+-rw-r--r--   0        0        0      388 2024-03-26 20:39:50.846638 bit_common-0.1.9/bit/middleware.py
+-rw-r--r--   0        0        0     6591 2024-03-26 20:41:10.671124 bit_common-0.1.9/bit/model.py
+-rw-r--r--   0        0        0     2386 2024-03-30 20:19:20.353414 bit_common-0.1.9/bit/protocol.py
+-rw-r--r--   0        0        0        0 2024-03-26 20:45:59.857611 bit_common-0.1.9/bit/py.typed
+-rw-r--r--   0        0        0      536 2024-03-30 20:23:13.942067 bit_common-0.1.9/bit/type/__init__.py
+-rw-r--r--   0        0        0     6124 2024-03-28 16:30:19.172825 bit_common-0.1.9/bit/type/base.py
+-rw-r--r--   0        0        0     2512 2024-03-22 17:33:58.201946 bit_common-0.1.9/bit/type/bitarray.py
+-rw-r--r--   0        0        0     1341 2024-03-26 20:50:15.568290 bit_common-0.1.9/bit/type/endian.py
+-rw-r--r--   0        0        0     5541 2024-03-26 20:02:05.853515 bit_common-0.1.9/bit/type/integer.py
+-rw-r--r--   0        0        0     1199 2024-03-29 22:48:24.865677 bit_common-0.1.9/bit/type/network.py
+-rw-r--r--   0        0        0     3849 2024-03-29 22:51:37.683057 bit_common-0.1.9/bit/type/string.py
+-rw-r--r--   0        0        0     1028 2024-03-30 20:24:57.060388 bit_common-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1806 1970-01-01 00:00:00.000000 bit_common-0.1.9/PKG-INFO
```

### Comparing `bit_common-0.1.8/README.md` & `bit_common-0.1.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ### Usage
 
 Here are some examples of how you can use `bit-common`.
 
 #### Converting data to bits
 
 ```python
-from bit import int8, UTF8StringWithPrefix
+from bit.type import int8, UTF8StringWithPrefix
 
 # Converting data to bits
 data = int8(3)
 bits = data.to_bits()
 print(bits)  # Output: [1, 1, 0, 0, 0, 0, 0, 0]
 
 # Converting bits to data
```

### Comparing `bit_common-0.1.8/bit/controller.py` & `bit_common-0.1.9/bit/controller.py`

 * *Files identical despite different names*

### Comparing `bit_common-0.1.8/bit/model.py` & `bit_common-0.1.9/bit/model.py`

 * *Files identical despite different names*

### Comparing `bit_common-0.1.8/bit/protocol.py` & `bit_common-0.1.9/bit/protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
         self.transport = cast(asyncio.Transport, self.transport)
 
         result = await self.handle_data(data)
 
         if result is not None:
             self.transport.write(result)
 
+    @create_task
     async def datagram_received(self, data: bytes, addr: Any) -> None:
         """Called when some datagram is received."""
 
         self.transport = cast(asyncio.DatagramTransport, self.transport)
 
         result = await self.handle_data(data)
```

### Comparing `bit_common-0.1.8/bit/type/base.py` & `bit_common-0.1.9/bit/type/base.py`

 * *Files identical despite different names*

### Comparing `bit_common-0.1.8/bit/type/bitarray.py` & `bit_common-0.1.9/bit/type/bitarray.py`

 * *Files identical despite different names*

### Comparing `bit_common-0.1.8/bit/type/endian.py` & `bit_common-0.1.9/bit/type/endian.py`

 * *Files identical despite different names*

### Comparing `bit_common-0.1.8/bit/type/integer.py` & `bit_common-0.1.9/bit/type/integer.py`

 * *Files identical despite different names*

### Comparing `bit_common-0.1.8/bit/type/network.py` & `bit_common-0.1.9/bit/type/network.py`

 * *Files 24% similar despite different names*

```diff
@@ -25,22 +25,30 @@
     ) -> int:
 
         if isinstance(value, str):
             return int(cls.EXTRA(value))
 
         return super()._validate(value, info)
 
-    def __str__(self):
+    def __repr__(self):
         return str(self.EXTRA(self.value))
 
 
 class IPv6Address(IPv4Address):
     LENGTH = 128
     EXTRA: ClassVar[type] = ipaddress.IPv6Address
 
 
 class IPv4Mask(IPv4Address):
     pass
 
 
 class IPv6Mask(IPv6Address):
     pass
+
+
+class MACAddress(UnsignedInteger):
+    LENGTH = 48
+
+    def __repr__(self):
+        hex_data = f"{self.value:012x}"
+        return ":".join([hex_data[i : i + 2] for i in range(0, len(hex_data), 2)])
```

### Comparing `bit_common-0.1.8/bit/type/string.py` & `bit_common-0.1.9/bit/type/string.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,14 +75,19 @@
 
         elif isinstance(value, bytes):
             value = value.decode(cls.ENCODING)
 
         if not isinstance(value, str):
             raise ValueError(f"Expected str, got {type(value)}.")
 
+        try:
+            value.encode(cls.ENCODING)
+        except UnicodeEncodeError:
+            raise ValueError(f"Invalid value {value} for {cls.ENCODING} encoding.")
+
         return value
 
     @classmethod
     def __get_pydantic_core_schema__(
         cls, *args: P.args, **kwargs: P.kwargs
     ) -> core_schema.PlainValidatorFunctionSchema:
         return core_schema.with_info_plain_validator_function(cls.validate)
```

### Comparing `bit_common-0.1.8/pyproject.toml` & `bit_common-0.1.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bit-common"
-version = "0.1.8"
+version = "0.1.9"
 description = "Bit common types and utilities."
 authors = ["Yury Sokov <me@yurzs.dev>"]
 readme = "README.md"
 packages = [
     { include = "bit", from = "." },
     { include = "bit/py.typed", from = "." },
 ]
@@ -41,10 +41,11 @@
 
 [tool.autoflake]
 remove-all-unused-imports = true
 remove-duplicate-keys = true
 remove-unused-variables = true
 in-place = true
 recursive = true
+ignore-init-module-imports = true
 
 [tool.pytest]
 asyncio-mode = true
```

### Comparing `bit_common-0.1.8/PKG-INFO` & `bit_common-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bit-common
-Version: 0.1.8
+Version: 0.1.9
 Summary: Bit common types and utilities.
 License: MIT
 Author: Yury Sokov
 Author-email: me@yurzs.dev
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -37,15 +37,15 @@
 ### Usage
 
 Here are some examples of how you can use `bit-common`.
 
 #### Converting data to bits
 
 ```python
-from bit import int8, UTF8StringWithPrefix
+from bit.type import int8, UTF8StringWithPrefix
 
 # Converting data to bits
 data = int8(3)
 bits = data.to_bits()
 print(bits)  # Output: [1, 1, 0, 0, 0, 0, 0, 0]
 
 # Converting bits to data
```

