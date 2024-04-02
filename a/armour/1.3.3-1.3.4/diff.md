# Comparing `tmp/armour-1.3.3-py2.py3-none-any.whl.zip` & `tmp/armour-1.3.4-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 26473 bytes, number of entries: 19
--rw-r--r--  2.0 unx      231 b- defN 24-Feb-29 20:50 armour/__init__.py
--rw-r--r--  2.0 unx     7372 b- defN 23-Oct-14 20:41 armour/crypt.py
+Zip file size: 26329 bytes, number of entries: 19
+-rw-r--r--  2.0 unx      231 b- defN 24-Apr-02 12:09 armour/__init__.py
+-rw-r--r--  2.0 unx     6977 b- defN 24-Apr-02 12:12 armour/crypt.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Aug-15 17:45 armour/py.typed
 -rw-r--r--  2.0 unx      202 b- defN 23-Oct-14 15:53 armour/gen/__init__.py
 -rw-r--r--  2.0 unx     2971 b- defN 23-Oct-27 22:51 armour/gen/gen.py
 -rw-r--r--  2.0 unx     5858 b- defN 24-Feb-29 20:36 armour/gen/info.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Oct-14 16:32 armour/gen/py.typed
 -rw-r--r--  2.0 unx      205 b- defN 23-Oct-13 19:24 armour/pdb/__init__.py
 -rw-r--r--  2.0 unx     9719 b- defN 23-Oct-28 14:50 armour/pdb/entries.py
 -rw-r--r--  2.0 unx     2215 b- defN 23-Oct-28 14:44 armour/pdb/exc.py
 -rw-r--r--  2.0 unx     8613 b- defN 23-Oct-14 22:23 armour/pdb/header.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Oct-13 21:55 armour/pdb/py.typed
 -rw-r--r--  2.0 unx      686 b- defN 23-Oct-13 19:19 armour/pdb/s.py
--rw-------  2.0 unx    35113 b- defN 24-Feb-29 20:52 armour-1.3.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     3096 b- defN 24-Feb-29 20:52 armour-1.3.3.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 24-Feb-29 20:52 armour-1.3.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Feb-29 20:52 armour-1.3.3.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Oct-12 19:58 armour-1.3.3.dist-info/zip-safe
--rw-rw-r--  2.0 unx     1433 b- defN 24-Feb-29 20:52 armour-1.3.3.dist-info/RECORD
-19 files, 77832 bytes uncompressed, 24161 bytes compressed:  69.0%
+-rw-------  2.0 unx    35091 b- defN 24-Apr-02 12:13 armour-1.3.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3116 b- defN 24-Apr-02 12:13 armour-1.3.4.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-Apr-02 12:13 armour-1.3.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-02 12:13 armour-1.3.4.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Oct-12 19:58 armour-1.3.4.dist-info/zip-safe
+-rw-rw-r--  2.0 unx     1433 b- defN 24-Apr-02 12:13 armour-1.3.4.dist-info/RECORD
+19 files, 77435 bytes uncompressed, 24017 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -33,26 +33,26 @@
 
 Filename: armour/pdb/py.typed
 Comment: 
 
 Filename: armour/pdb/s.py
 Comment: 
 
-Filename: armour-1.3.3.dist-info/LICENSE
+Filename: armour-1.3.4.dist-info/LICENSE
 Comment: 
 
-Filename: armour-1.3.3.dist-info/METADATA
+Filename: armour-1.3.4.dist-info/METADATA
 Comment: 
 
-Filename: armour-1.3.3.dist-info/WHEEL
+Filename: armour-1.3.4.dist-info/WHEEL
 Comment: 
 
-Filename: armour-1.3.3.dist-info/top_level.txt
+Filename: armour-1.3.4.dist-info/top_level.txt
 Comment: 
 
-Filename: armour-1.3.3.dist-info/zip-safe
+Filename: armour-1.3.4.dist-info/zip-safe
 Comment: 
 
-Filename: armour-1.3.3.dist-info/RECORD
+Filename: armour-1.3.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## armour/__init__.py

```diff
@@ -2,10 +2,10 @@
 # -*- coding: utf-8 -*-
 """armour"""
 
 from typing import Final, Tuple
 
 from . import crypt, gen, pdb
 
-__version__: Final[str] = "1.3.3"
+__version__: Final[str] = "1.3.4"
 
 __all__: Final[Tuple[str, ...]] = "__version__", "crypt", "gen", "pdb"
```

## armour/crypt.py

```diff
@@ -2,14 +2,15 @@
 # -*- coding: utf-8 -*-
 """cryptography algorithms"""
 
 import base64
 import secrets
 import typing
 
+import crc4
 import zstd
 from cryptography.fernet import Fernet
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes, hmac, padding
 from cryptography.hazmat.primitives.ciphers import (Cipher, CipherContext, algorithms,
                                                     modes)
 from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
@@ -260,52 +261,30 @@
 
     return data
 
 
 # -- rc4 encryption --
 
 
-def crypt_rc4(data: bytes, key: bytes) -> bytes:
-    """rc4 crypto"""
-
-    S = list(range(256))
-    j: int = 0
-    out: bytearray = bytearray()
-
-    for i in range(256):
-        j = (j + S[i] + key[i % len(key)]) % 256
-        S[i], S[j] = S[j], S[i]
-
-    i = j = 0
-
-    for byte in data:
-        i = (i + 1) % 256
-        j = (j + S[i]) % 256
-        S[i], S[j] = S[j], S[i]
-        out.append(byte ^ S[(S[i] + S[j]) % 256])
-
-    return bytes(out)
-
-
 def encrypt_rc4(
     data: bytes,
     isec_crypto_passes: int,
     password: bytes,
     salt: bytes,
     hash_salt_len: int,
 ) -> bytes:
     """encrypt rc4"""
 
     rsalt: bytes = RAND.randbytes(hash_salt_len + 13)
     key: bytes = hash_algo(0, rsalt + password + salt)
 
     for _ in range(isec_crypto_passes):
-        data = crypt_rc4(data=RAND.randbytes(5) + data + RAND.randbytes(5), key=key)
+        data = crc4.rc4(RAND.randbytes(5) + data + RAND.randbytes(5), key)  # type: ignore
 
-    return rsalt + data
+    return rsalt + data  # type: ignore
 
 
 def decrypt_rc4(
     data: bytes,
     isec_crypto_passes: int,
     password: bytes,
     salt: bytes,
@@ -317,10 +296,10 @@
 
     rsalt: bytes = data[:hash_salt_len]
     data = data[hash_salt_len:]
 
     key: bytes = hash_algo(0, rsalt + password + salt)
 
     for _ in range(isec_crypto_passes):
-        data = crypt_rc4(data=data, key=key)[5:-5]
+        data = crc4.rc4(data, key)[5:-5]  # type: ignore
 
-    return data
+    return data  # type: ignore
```

## Comparing `armour-1.3.3.dist-info/LICENSE` & `armour-1.3.4.dist-info/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -628,15 +628,15 @@
 
   To do so, attach the following notices to the program.  It is safest
 to attach them to the start of each source file to most effectively
 state the exclusion of warranty; and each file should have at least
 the "copyright" line and a pointer to where the full notice is found.
 
     armour
-    Copyright (C) 2022  Ari Archer <ari.web.xyz@gmail.com>
+    Copyright (C) 2024  Ari Archer <ari@ari.lt>
 
     This program is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
 
     This program is distributed in the hope that it will be useful,
@@ -648,15 +648,15 @@
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 Also add information on how to contact you by electronic and paper mail.
 
   If the program does terminal interaction, make it output a short
 notice like this when it starts in an interactive mode:
 
-    armour  Copyright (C) 2023  Ari Archer <ari.web.xyz@gmail.com>
+    armour  Copyright (C) 2024  Ari Archer <ari@ari.lt>
     This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
     This is free software, and you are welcome to redistribute it
     under certain conditions; type `show c' for details.
 
 The hypothetical commands `show w' and `show c' should show the appropriate
 parts of the General Public License.  Of course, your program's commands
 might be different; for a GUI interface, you would use an "about box".
```

## Comparing `armour-1.3.3.dist-info/METADATA` & `armour-1.3.4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: armour
-Version: 1.3.3
+Version: 1.3.4
 Summary: password securing, management and generation tools
 Home-page: https://ari-web.xyz/gh/armour
 Author: Ari Archer
 Author-email: ari.web.xyz@gmail.com
 License: GPLv3+
 Project-URL: Bug Tracker, https://ari-web.xyz/gh/armour/issues
 Project-URL: Documentation, https://ari-web.xyz/gh/armour/tree/main/doc
@@ -26,14 +26,15 @@
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cryptography
 Requires-Dist: zstd
+Requires-Dist: crc4
 
 # armour
 
 > password securing, management and generation tools
 
 # userland tools
```

## Comparing `armour-1.3.3.dist-info/RECORD` & `armour-1.3.4.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-armour/__init__.py,sha256=dKfEoe6YRJe3NPoANZ4aWwJldJ3wvyeHqykkjTlRoM8,231
-armour/crypt.py,sha256=a9itmUz1Ijfdwpw_sx6AEO62aMYGDG55jU2FXiw8kiE,7372
+armour/__init__.py,sha256=VcRJmdrT5yrwx1zeySjw8PxQEOE0h6UxsHSClXOfe2Y,231
+armour/crypt.py,sha256=RufAWRJDAHch8vBszNZ-JrD-e74wf1jm7kI1FXPdjhc,6977
 armour/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 armour/gen/__init__.py,sha256=g__Jyu19SmE_utDu3XnkSS2tLX2-hFHd80008Hoyv80,202
 armour/gen/gen.py,sha256=a8sInpUWf6V5NTF2sSN-km3oKNPnUQgcwFvf8Cohfxo,2971
 armour/gen/info.py,sha256=LPY7GRYUm3s98IHcREcW8WWuAGTyBOcFMK0YdWnFiuw,5858
 armour/gen/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 armour/pdb/__init__.py,sha256=P0BNCB3OB5XUp3FHnBzyBrIG3jiIKFjsnGGGTyV7lBQ,205
 armour/pdb/entries.py,sha256=r37VKdwgrleiqz99KSHlk-1a7HGV08lbhU-LvgrV6Rw,9719
 armour/pdb/exc.py,sha256=QM7BZS0mdzZhnkXkhbt3WGfb46th9Iw7kV5KzQ3Os2E,2215
 armour/pdb/header.py,sha256=JtMRP9v3QXlojePXAIJ3rn_gXLCqS-WdoK8vEdW-2X0,8613
 armour/pdb/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 armour/pdb/s.py,sha256=wjAMynYTsrlCiGzKNhybw-gbg490B0Dn3Lx-sX9TGHI,686
-armour-1.3.3.dist-info/LICENSE,sha256=DRm2JRnhh3CJd-sIBDhAtAt9Kv7eYnFr8ndxf364qHM,35113
-armour-1.3.3.dist-info/METADATA,sha256=bHsxZu1gyAtToliOARlTzql-KeaOH2HrlrXaWFCSkMw,3096
-armour-1.3.3.dist-info/WHEEL,sha256=-G_t0oGuE7UD0DrSpVZnq1hHMBV9DD2XkS5v7XpmTnk,110
-armour-1.3.3.dist-info/top_level.txt,sha256=0bjBbmw8imNlTF9u5h8nlDNKpXxFV8_k9COygQp8_Fc,7
-armour-1.3.3.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-armour-1.3.3.dist-info/RECORD,,
+armour-1.3.4.dist-info/LICENSE,sha256=YKQLGtM_eE0NBGEmij6uEkS-5mz1_-u-DksxNW0OCr8,35091
+armour-1.3.4.dist-info/METADATA,sha256=UOdFZvr-_DLv_BgdoVNSapvsOmZ_jwA0lNsplCIQHD4,3116
+armour-1.3.4.dist-info/WHEEL,sha256=DZajD4pwLWue70CAfc7YaxT1wLUciNBvN_TTcvXpltE,110
+armour-1.3.4.dist-info/top_level.txt,sha256=0bjBbmw8imNlTF9u5h8nlDNKpXxFV8_k9COygQp8_Fc,7
+armour-1.3.4.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+armour-1.3.4.dist-info/RECORD,,
```

