# Comparing `tmp/han2kip-0.1.1.tar.gz` & `tmp/han2kip-0.1.2.tar.gz`

## Comparing `han2kip-0.1.1.tar` & `han2kip-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 han2kip-0.1.1/han2kip/__init__.py
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 han2kip-0.1.1/han2kip/kip_converter.py
--rw-r--r--   0        0        0   901007 2020-02-02 00:00:00.000000 han2kip-0.1.1/han2kip/data/dict.txt
--rw-r--r--   0        0        0  2312337 2020-02-02 00:00:00.000000 han2kip-0.1.1/han2kip/data/words.json
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 han2kip-0.1.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 han2kip-0.1.1/LICENSE
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 han2kip-0.1.1/README.md
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 han2kip-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 han2kip-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 han2kip-0.1.2/han2kip/__init__.py
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 han2kip-0.1.2/han2kip/kip_converter.py
+-rw-r--r--   0        0        0   901007 2020-02-02 00:00:00.000000 han2kip-0.1.2/han2kip/data/dict.txt
+-rw-r--r--   0        0        0  2312337 2020-02-02 00:00:00.000000 han2kip-0.1.2/han2kip/data/words.json
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 han2kip-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 han2kip-0.1.2/LICENSE
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 han2kip-0.1.2/README.md
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 han2kip-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 han2kip-0.1.2/PKG-INFO
```

### Comparing `han2kip-0.1.1/han2kip/kip_converter.py` & `han2kip-0.1.2/han2kip/kip_converter.py`

 * *Files identical despite different names*

### Comparing `han2kip-0.1.1/han2kip/data/dict.txt` & `han2kip-0.1.2/han2kip/data/dict.txt`

 * *Files identical despite different names*

### Comparing `han2kip-0.1.1/han2kip/data/words.json` & `han2kip-0.1.2/han2kip/data/words.json`

 * *Files identical despite different names*

### Comparing `han2kip-0.1.1/.gitignore` & `han2kip-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `han2kip-0.1.1/LICENSE` & `han2kip-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `han2kip-0.1.1/README.md` & `han2kip-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `han2kip-0.1.1/pyproject.toml` & `han2kip-0.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 00000000: 5b62 7569 6c64 2d73 7973 7465 6d5d 0d0a  [build-system]..
 00000010: 7265 7175 6972 6573 203d 205b 2268 6174  requires = ["hat
 00000020: 6368 6c69 6e67 225d 0d0a 6275 696c 642d  chling"]..build-
 00000030: 6261 636b 656e 6420 3d20 2268 6174 6368  backend = "hatch
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 6861 6e32 6b69 7022 0d0a 7665 7273   "han2kip"..vers
-00000070: 696f 6e20 3d20 2230 2e31 2e31 220d 0a61  ion = "0.1.1"..a
+00000070: 696f 6e20 3d20 2230 2e31 2e32 220d 0a61  ion = "0.1.2"..a
 00000080: 7574 686f 7273 203d 205b 0d0a 2020 7b20  uthors = [..  { 
 00000090: 6e61 6d65 3d22 e69e 97e6 80a1 e890 b122  name="........."
-000000a0: 2c20 656d 6169 6c3d 2271 7731 3233 3435  , email="qw12345
-000000b0: 3535 3434 4067 6d61 696c 2e63 6f6d 227d  5544@gmail.com"}
-000000c0: 2c20 7b20 6e61 6d65 3d22 e69e 97e6 9f8f  , { name="......
-000000d0: e5bb b722 2c20 656d 6169 6c3d 2262 6f74  ...", email="bot
-000000e0: 696e 686f 6c6d 6573 4067 6d61 696c 2e63  inholmes@gmail.c
-000000f0: 6f6d 227d 0d0a 5d0d 0a64 6573 6372 6970  om"}..]..descrip
-00000100: 7469 6f6e 203d 2022 6861 6e32 6b69 7020  tion = "han2kip 
-00000110: 6973 2061 2070 6163 6b61 6765 2066 6f72  is a package for
-00000120: 2063 6f6e 7665 7274 696e 6720 5461 6977   converting Taiw
-00000130: 616e 6573 6520 486f 6b6b 6965 6e20 4861  anese Hokkien Ha
-00000140: 6e7a 6920 746f 2069 7473 2070 686f 6e65  nzi to its phone
-00000150: 7469 6320 7265 7072 6573 656e 7461 7469  tic representati
-00000160: 6f6e 2e22 0d0a 7265 6164 6d65 203d 2022  on."..readme = "
-00000170: 5245 4144 4d45 2e6d 6422 0d0a 6c69 6365  README.md"..lice
-00000180: 6e73 6520 3d20 7b20 6669 6c65 3d22 4c49  nse = { file="LI
-00000190: 4345 4e53 4522 207d 0d0a 636c 6173 7369  CENSE" }..classi
-000001a0: 6669 6572 7320 3d20 5b0d 0a20 2020 2022  fiers = [..    "
-000001b0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000001c0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000001d0: 3a20 3322 2c0d 0a20 2020 2022 4c69 6365  : 3",..    "Lice
-000001e0: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
-000001f0: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
-00000200: 7365 222c 0d0a 2020 2020 224f 7065 7261  se",..    "Opera
-00000210: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
-00000220: 5320 496e 6465 7065 6e64 656e 7422 2c0d  S Independent",.
-00000230: 0a5d 0d0a 6465 7065 6e64 656e 6369 6573  .]..dependencies
-00000240: 203d 205b 0d0a 2020 2020 2020 2020 226a   = [..        "j
-00000250: 6965 6261 3e3d 302e 3432 2e31 222c 0d0a  ieba>=0.42.1",..
-00000260: 2020 2020 5d0d 0a0d 0a5b 7072 6f6a 6563      ]....[projec
-00000270: 742e 7572 6c73 5d0d 0a22 486f 6d65 7061  t.urls].."Homepa
-00000280: 6765 2220 3d20 2268 7474 7073 3a2f 2f67  ge" = "https://g
-00000290: 6974 6875 622e 636f 6d2f 6a75 6c69 616f  ithub.com/juliao
-000002a0: 756f 2f68 616e 326b 6970 22              uo/han2kip"
+000000a0: 207d 2c20 0d0a 2020 7b20 6e61 6d65 3d22   }, ..  { name="
+000000b0: e69e 97e6 9f8f e5bb b722 207d 2c0d 0a5d  ........." },..]
+000000c0: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
+000000d0: 2268 616e 326b 6970 2069 7320 6120 7061  "han2kip is a pa
+000000e0: 636b 6167 6520 666f 7220 636f 6e76 6572  ckage for conver
+000000f0: 7469 6e67 2054 6169 7761 6e65 7365 2048  ting Taiwanese H
+00000100: 6f6b 6b69 656e 2048 616e 7a69 2074 6f20  okkien Hanzi to 
+00000110: 6974 7320 7068 6f6e 6574 6963 2072 6570  its phonetic rep
+00000120: 7265 7365 6e74 6174 696f 6e2e 220d 0a72  resentation."..r
+00000130: 6561 646d 6520 3d20 2252 4541 444d 452e  eadme = "README.
+00000140: 6d64 220d 0a6c 6963 656e 7365 203d 207b  md"..license = {
+00000150: 2066 696c 653d 224c 4943 454e 5345 2220   file="LICENSE" 
+00000160: 7d0d 0a63 6c61 7373 6966 6965 7273 203d  }..classifiers =
+00000170: 205b 0d0a 2020 2020 2250 726f 6772 616d   [..    "Program
+00000180: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000190: 2050 7974 686f 6e20 3a3a 2033 222c 0d0a   Python :: 3",..
+000001a0: 2020 2020 224c 6963 656e 7365 203a 3a20      "License :: 
+000001b0: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
+000001c0: 4d49 5420 4c69 6365 6e73 6522 2c0d 0a20  MIT License",.. 
+000001d0: 2020 2022 4f70 6572 6174 696e 6720 5379     "Operating Sy
+000001e0: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
+000001f0: 656e 6465 6e74 222c 0d0a 5d0d 0a64 6570  endent",..]..dep
+00000200: 656e 6465 6e63 6965 7320 3d20 5b0d 0a20  endencies = [.. 
+00000210: 2020 2020 2020 2022 6a69 6562 613e 3d30         "jieba>=0
+00000220: 2e34 322e 3122 2c0d 0a20 2020 205d 0d0a  .42.1",..    ]..
+00000230: 0d0a 5b70 726f 6a65 6374 2e75 726c 735d  ..[project.urls]
+00000240: 0d0a 2248 6f6d 6570 6167 6522 203d 2022  .."Homepage" = "
+00000250: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000260: 6f6d 2f6a 756c 6961 6f75 6f2f 6861 6e32  om/juliaouo/han2
+00000270: 6b69 7022                                kip"
```

### Comparing `han2kip-0.1.1/PKG-INFO` & `han2kip-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.3
 Name: han2kip
-Version: 0.1.1
+Version: 0.1.2
 Summary: han2kip is a package for converting Taiwanese Hokkien Hanzi to its phonetic representation.
 Project-URL: Homepage, https://github.com/juliaouo/han2kip
-Author-email: 林怡萱 <qw123455544@gmail.com>, 林柏廷 <botinholmes@gmail.com>
+Author: 林怡萱, 林柏廷
 License: MIT License
         
         Copyright (c) 2024 juliaouo
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

