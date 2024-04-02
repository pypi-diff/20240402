# Comparing `tmp/robotframework_reportmodifier-0.1.9.tar.gz` & `tmp/robotframework_reportmodifier-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_reportmodifier-0.1.9.tar", max compression
+gzip compressed data, was "robotframework_reportmodifier-0.2.0.tar", max compression
```

## Comparing `robotframework_reportmodifier-0.1.9.tar` & `robotframework_reportmodifier-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35801 2024-02-12 08:28:04.348570 robotframework_reportmodifier-0.1.9/LICENSE
--rw-r--r--   0        0        0     2560 2024-02-12 10:15:29.877308 robotframework_reportmodifier-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     4704 2024-02-06 11:27:56.446152 robotframework_reportmodifier-0.1.9/README.md
--rw-r--r--   0        0        0       44 2024-02-05 21:56:41.563296 robotframework_reportmodifier-0.1.9/src/reportmodifier/__init__.py
--rw-r--r--   0        0        0       21 2024-02-05 21:56:41.564295 robotframework_reportmodifier-0.1.9/src/reportmodifier/__version__.py
--rw-r--r--   0        0        0     1572 2024-02-05 21:56:41.565293 robotframework_reportmodifier-0.1.9/src/reportmodifier/_file_tools.py
--rw-r--r--   0        0        0     5790 2024-02-12 07:29:37.883742 robotframework_reportmodifier-0.1.9/src/reportmodifier/_report_configuration.py
--rw-r--r--   0        0        0     1713 2024-02-12 07:30:39.491570 robotframework_reportmodifier-0.1.9/src/reportmodifier/ReportModifier.py
--rw-r--r--   0        0        0    11010 2024-02-12 07:31:01.985745 robotframework_reportmodifier-0.1.9/src/reportmodifier/ReportModifierVisitor.py
--rw-r--r--   0        0        0       74 2024-02-05 21:56:41.558294 robotframework_reportmodifier-0.1.9/src/ReportModifierListener/__init__.py
--rw-r--r--   0        0        0      815 2024-02-12 09:34:13.815807 robotframework_reportmodifier-0.1.9/src/ReportModifierListener/ReportModifierListener.py
--rw-r--r--   0        0        0     5269 1970-01-01 00:00:00.000000 robotframework_reportmodifier-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0    35801 2024-02-12 08:28:04.348570 robotframework_reportmodifier-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2032 2024-03-28 08:50:33.654585 robotframework_reportmodifier-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4848 2024-03-28 08:21:54.396809 robotframework_reportmodifier-0.2.0/README.md
+-rw-r--r--   0        0        0       44 2024-03-28 08:26:32.278869 robotframework_reportmodifier-0.2.0/src/reportmodifier/__init__.py
+-rw-r--r--   0        0        0       22 2024-03-18 14:55:57.436001 robotframework_reportmodifier-0.2.0/src/reportmodifier/__version__.py
+-rw-r--r--   0        0        0     1664 2024-03-26 08:36:58.839614 robotframework_reportmodifier-0.2.0/src/reportmodifier/_file_tools.py
+-rw-r--r--   0        0        0     5981 2024-03-26 12:34:37.585293 robotframework_reportmodifier-0.2.0/src/reportmodifier/_report_configuration.py
+-rw-r--r--   0        0        0     6905 2024-03-28 08:46:21.576313 robotframework_reportmodifier-0.2.0/src/reportmodifier/ReportModifier.py
+-rw-r--r--   0        0        0    11922 2024-03-28 08:42:48.616199 robotframework_reportmodifier-0.2.0/src/reportmodifier/ReportModifierVisitor.py
+-rw-r--r--   0        0        0       79 2024-03-18 15:11:07.246558 robotframework_reportmodifier-0.2.0/src/ReportModifierListener/__init__.py
+-rw-r--r--   0        0        0      879 2024-03-27 07:28:27.461714 robotframework_reportmodifier-0.2.0/src/ReportModifierListener/ReportModifierListener.py
+-rw-r--r--   0        0        0     5482 1970-01-01 00:00:00.000000 robotframework_reportmodifier-0.2.0/PKG-INFO
```

### Comparing `robotframework_reportmodifier-0.1.9/LICENSE` & `robotframework_reportmodifier-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_reportmodifier-0.1.9/pyproject.toml` & `robotframework_reportmodifier-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,160 +1,127 @@
 00000000: 5b74 6f6f 6c2e 706f 6574 7279 5d0d 0a6e  [tool.poetry]..n
 00000010: 616d 6520 3d20 2272 6f62 6f74 6672 616d  ame = "robotfram
 00000020: 6577 6f72 6b2d 7265 706f 7274 6d6f 6469  ework-reportmodi
 00000030: 6669 6572 220d 0a76 6572 7369 6f6e 203d  fier"..version =
-00000040: 2022 302e 312e 3922 0d0a 6465 7363 7269   "0.1.9"..descri
+00000040: 2022 302e 322e 3022 0d0a 6465 7363 7269   "0.2.0"..descri
 00000050: 7074 696f 6e20 3d20 2246 696c 7465 7220  ption = "Filter 
 00000060: 7265 706f 7274 2063 6f6e 7465 6e74 2e22  report content."
 00000070: 0d0a 6175 7468 6f72 7320 3d20 5b22 4d61  ..authors = ["Ma
 00000080: 7474 6869 6173 2047 756e 7468 6572 203c  tthias Gunther <
 00000090: 6d61 7474 6869 6173 6775 6e74 6865 7240  matthiasgunther@
-000000a0: 676d 6169 6c2e 636f 6d3e 225d 0d0a 7265  gmail.com>"]..re
-000000b0: 6164 6d65 203d 2022 5245 4144 4d45 2e6d  adme = "README.m
-000000c0: 6422 0d0a 7061 636b 6167 6573 203d 205b  d"..packages = [
-000000d0: 0d0a 2020 2020 7b20 696e 636c 7564 6520  ..    { include 
-000000e0: 3d20 2272 6570 6f72 746d 6f64 6966 6965  = "reportmodifie
-000000f0: 7222 2c20 6672 6f6d 203d 2022 7372 6322  r", from = "src"
-00000100: 207d 2c0d 0a20 2020 207b 2069 6e63 6c75   },..    { inclu
-00000110: 6465 203d 2022 5265 706f 7274 4d6f 6469  de = "ReportModi
-00000120: 6669 6572 4c69 7374 656e 6572 222c 2066  fierListener", f
-00000130: 726f 6d20 3d20 2273 7263 2220 7d0d 0a20  rom = "src" }.. 
-00000140: 205d 0d0a 0d0a 5b62 7569 6c64 2d73 7973   ]....[build-sys
-00000150: 7465 6d5d 0d0a 7265 7175 6972 6573 203d  tem]..requires =
-00000160: 205b 2270 6f65 7472 792d 636f 7265 225d   ["poetry-core"]
-00000170: 0d0a 6275 696c 642d 6261 636b 656e 6420  ..build-backend 
-00000180: 3d20 2270 6f65 7472 792e 636f 7265 2e6d  = "poetry.core.m
-00000190: 6173 6f6e 7279 2e61 7069 220d 0a0d 0a5b  asonry.api"....[
-000001a0: 7072 6f6a 6563 742e 7572 6c73 5d0d 0a48  project.urls]..H
-000001b0: 6f6d 6570 6167 6520 3d20 2268 7474 7073  omepage = "https
-000001c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4d61  ://github.com/Ma
-000001d0: 726b 6574 5371 7561 7265 2f72 6f62 6f74  rketSquare/robot
-000001e0: 6672 616d 6577 6f72 6b2d 7265 706f 7274  framework-report
-000001f0: 6d6f 6469 6669 6572 220d 0a49 7373 7565  modifier"..Issue
-00000200: 7320 3d20 2268 7474 7073 3a2f 2f67 6974  s = "https://git
-00000210: 6875 622e 636f 6d2f 4d61 726b 6574 5371  hub.com/MarketSq
-00000220: 7561 7265 2f72 6f62 6f74 6672 616d 6577  uare/robotframew
-00000230: 6f72 6b2d 7265 706f 7274 6d6f 6469 6669  ork-reportmodifi
-00000240: 6572 2f69 7373 7565 7322 0d0a 0d0a 5b74  er/issues"....[t
-00000250: 6f6f 6c2e 706f 6574 7279 2e64 6570 656e  ool.poetry.depen
-00000260: 6465 6e63 6965 735d 0d0a 7079 7468 6f6e  dencies]..python
-00000270: 203d 2022 5e33 2e38 220d 0a72 6f62 6f74   = "^3.8"..robot
-00000280: 6672 616d 6577 6f72 6b20 3d20 223e 3d34  framework = ">=4
-00000290: 2e31 220d 0a70 7964 616e 7469 6320 3d20  .1"..pydantic = 
-000002a0: 225e 312e 3130 2e34 220d 0a72 756c 652d  "^1.10.4"..rule-
-000002b0: 656e 6769 6e65 203d 2022 5e33 2e35 2e30  engine = "^3.5.0
-000002c0: 220d 0a0d 0a5b 746f 6f6c 2e70 6f65 7472  "....[tool.poetr
-000002d0: 792e 6772 6f75 702e 636f 6e66 6967 2e64  y.group.config.d
-000002e0: 6570 656e 6465 6e63 6965 735d 0d0a 5079  ependencies]..Py
-000002f0: 5941 4d4c 203d 2022 5e36 2e30 220d 0a70  YAML = "^6.0"..p
-00000300: 6174 686c 6962 203d 2022 5e31 2e30 2e31  athlib = "^1.0.1
-00000310: 220d 0a72 6567 6578 203d 2022 5e32 3032  "..regex = "^202
-00000320: 332e 3130 2e33 220d 0a0d 0a5b 746f 6f6c  3.10.3"....[tool
-00000330: 2e70 6f65 7472 792e 6772 6f75 702e 6465  .poetry.group.de
-00000340: 762e 6465 7065 6e64 656e 6369 6573 5d0d  v.dependencies].
-00000350: 0a72 6f62 6f74 6672 616d 6577 6f72 6b20  .robotframework 
-00000360: 3d20 225e 342e 3122 0d0a 7275 6666 203d  = "^4.1"..ruff =
-00000370: 2022 2a22 0d0a 6d79 7079 203d 2022 2a22   "*"..mypy = "*"
-00000380: 0d0a 626c 6163 6b20 3d20 222a 220d 0a0d  ..black = "*"...
-00000390: 0a5b 746f 6f6c 2e62 6c61 636b 5d0d 0a6c  .[tool.black]..l
-000003a0: 696e 652d 6c65 6e67 7468 203d 2031 3230  ine-length = 120
-000003b0: 0d0a 7461 7267 6574 2d76 6572 7369 6f6e  ..target-version
-000003c0: 203d 205b 2770 7933 3827 5d0d 0a65 7863   = ['py38']..exc
-000003d0: 6c75 6465 203d 2027 2727 0d0a 280d 0a20  lude = '''..(.. 
-000003e0: 202f 280d 0a20 2020 2020 205c 2e65 6767   /(..      \.egg
-000003f0: 7320 2020 2020 2020 2020 2320 6578 636c  s         # excl
-00000400: 7564 6520 6120 6665 7720 636f 6d6d 6f6e  ude a few common
-00000410: 2064 6972 6563 746f 7269 6573 2069 6e20   directories in 
-00000420: 7468 650d 0a20 2020 207c 205c 2e67 6974  the..    | \.git
-00000430: 2020 2020 2020 2020 2020 2320 726f 6f74            # root
-00000440: 206f 6620 7468 6520 7072 6f6a 6563 740d   of the project.
-00000450: 0a20 2020 207c 205c 2e6d 7970 795f 6361  .    | \.mypy_ca
-00000460: 6368 650d 0a20 2020 207c 205c 2e74 6f78  che..    | \.tox
-00000470: 0d0a 2020 2020 7c20 5c2e 7665 6e76 0d0a  ..    | \.venv..
-00000480: 2020 2020 7c20 6275 696c 640d 0a20 2020      | build..   
-00000490: 207c 2064 6973 740d 0a20 2020 207c 206f   | dist..    | o
-000004a0: 7574 0d0a 2020 2020 7c20 706c 6179 6772  ut..    | playgr
-000004b0: 6f75 6e64 0d0a 2020 292f 0d0a 290d 0a27  ound..  )/..)..'
-000004c0: 2727 0d0a 0d0a 5b74 6f6f 6c2e 7275 6666  ''....[tool.ruff
-000004d0: 5d0d 0a6c 696e 652d 6c65 6e67 7468 203d  ]..line-length =
-000004e0: 2031 3230 0d0a 7461 7267 6574 2d76 6572   120..target-ver
-000004f0: 7369 6f6e 203d 2022 7079 3338 220d 0a65  sion = "py38"..e
-00000500: 7863 6c75 6465 203d 205b 0d0a 2020 222e  xclude = [..  ".
-00000510: 627a 7222 2c0d 0a20 2022 2e64 6972 656e  bzr",..  ".diren
-00000520: 7622 2c0d 0a20 2022 2e65 6767 7322 2c0d  v",..  ".eggs",.
-00000530: 0a20 2022 2e67 6974 222c 0d0a 2020 222e  .  ".git",..  ".
-00000540: 6867 222c 0d0a 2020 222e 6d79 7079 5f63  hg",..  ".mypy_c
-00000550: 6163 6865 222c 0d0a 2020 222e 6e6f 7822  ache",..  ".nox"
-00000560: 2c0d 0a20 2022 2e70 616e 7473 2e64 222c  ,..  ".pants.d",
-00000570: 0d0a 2020 222e 7275 6666 5f63 6163 6865  ..  ".ruff_cache
-00000580: 222c 0d0a 2020 222e 7376 6e22 2c0d 0a20  ",..  ".svn",.. 
-00000590: 2022 2e74 6f78 222c 0d0a 2020 222e 7665   ".tox",..  ".ve
-000005a0: 6e76 222c 0d0a 2020 225f 5f70 7970 6163  nv",..  "__pypac
-000005b0: 6b61 6765 735f 5f22 2c0d 0a20 2022 5f62  kages__",..  "_b
-000005c0: 7569 6c64 222c 0d0a 2020 2262 7563 6b2d  uild",..  "buck-
-000005d0: 6f75 7422 2c0d 0a20 2022 6275 696c 6422  out",..  "build"
-000005e0: 2c0d 0a20 2022 6469 7374 222c 0d0a 2020  ,..  "dist",..  
-000005f0: 226e 6f64 655f 6d6f 6475 6c65 7322 2c0d  "node_modules",.
-00000600: 0a20 2022 7665 6e76 222c 0d0a 2020 222e  .  "venv",..  ".
-00000610: 6861 7463 6822 2c0d 0a5d 0d0a 6967 6e6f  hatch",..]..igno
-00000620: 7265 203d 205b 2245 3734 3122 2c20 224e  re = ["E741", "N
-00000630: 3830 3522 5d0d 0a73 656c 6563 7420 3d20  805"]..select = 
-00000640: 5b0d 0a20 2022 4522 2c0d 0a20 2022 4622  [..  "E",..  "F"
-00000650: 2c0d 0a20 2022 5722 2c0d 0a20 2022 4922  ,..  "W",..  "I"
-00000660: 2c0d 0a20 2022 4e22 2c0d 0a20 2023 2255  ,..  "N",..  #"U
-00000670: 5022 2c0d 0a20 2022 5954 5422 2c0d 0a20  P",..  "YTT",.. 
-00000680: 2023 2241 4e4e 222c 0d0a 2020 2322 424c   #"ANN",..  #"BL
-00000690: 4522 2c0d 0a20 2023 2242 222c 0d0a 2020  E",..  #"B",..  
-000006a0: 2322 4122 0d0a 2020 2322 434f 4d22 0d0a  #"A"..  #"COM"..
-000006b0: 2020 2320 2243 3422 2c20 2320 544f 444f    # "C4", # TODO
-000006c0: 2065 6e61 626c 6520 7468 6973 0d0a 2020   enable this..  
-000006d0: 2244 545a 222c 0d0a 2020 2254 3130 222c  "DTZ",..  "T10",
-000006e0: 0d0a 2020 2320 2245 4d22 2c0d 0a20 2022  ..  # "EM",..  "
-000006f0: 4953 4322 2c0d 0a20 2022 4722 2c0d 0a20  ISC",..  "G",.. 
-00000700: 2023 2249 4e50 222c 0d0a 2020 2250 4945   #"INP",..  "PIE
-00000710: 222c 0d0a 2020 2320 2254 3230 222c 0d0a  ",..  # "T20",..
-00000720: 2020 2250 5422 2c0d 0a20 2022 5122 2c0d    "PT",..  "Q",.
-00000730: 0a20 2022 5245 5422 2c0d 0a20 2023 2022  .  "RET",..  # "
-00000740: 5349 4d22 2c20 2320 544f 444f 2065 6e61  SIM", # TODO ena
-00000750: 626c 6520 7468 6973 0d0a 2020 2322 5449  ble this..  #"TI
-00000760: 4422 2c0d 0a20 2023 2254 4348 222c 0d0a  D",..  #"TCH",..
-00000770: 2020 2322 4152 4722 2c0d 0a20 2023 2250    #"ARG",..  #"P
-00000780: 5448 222c 2023 2054 4f44 4f20 656e 6162  TH", # TODO enab
-00000790: 6c65 2074 6869 730d 0a5d 0d0a 0d0a 5b74  le this..]....[t
-000007a0: 6f6f 6c2e 7275 6666 2e70 6572 2d66 696c  ool.ruff.per-fil
-000007b0: 652d 6967 6e6f 7265 735d 0d0a 225f 5f69  e-ignores].."__i
-000007c0: 6e69 745f 5f2e 7079 2220 3d20 5b22 4634  nit__.py" = ["F4
-000007d0: 3031 225d 0d0a 0d0a 0d0a 5b74 6f6f 6c2e  01"]......[tool.
-000007e0: 6d79 7079 5d0d 0a23 204d 7950 7920 636f  mypy]..# MyPy co
-000007f0: 6e66 6967 0d0a 2320 4669 6c65 2072 6566  nfig..# File ref
-00000800: 6572 656e 6365 2068 6572 6520 2d20 6874  erence here - ht
-00000810: 7470 3a2f 2f6d 7970 792e 7265 6164 7468  tp://mypy.readth
-00000820: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-00000830: 7374 2f63 6f6e 6669 675f 6669 6c65 2e68  st/config_file.h
-00000840: 746d 6c23 636f 6e66 6967 2d66 696c 650d  tml#config-file.
-00000850: 0a70 7974 686f 6e5f 7665 7273 696f 6e20  .python_version 
-00000860: 3d20 332e 380d 0a77 6172 6e5f 7265 6475  = 3.8..warn_redu
-00000870: 6e64 616e 745f 6361 7374 7320 3d20 7472  ndant_casts = tr
-00000880: 7565 0d0a 7761 726e 5f75 6e75 7365 645f  ue..warn_unused_
-00000890: 6967 6e6f 7265 7320 3d20 7472 7565 0d0a  ignores = true..
-000008a0: 7761 726e 5f72 6574 7572 6e5f 616e 7920  warn_return_any 
-000008b0: 3d20 7472 7565 0d0a 7761 726e 5f75 6e75  = true..warn_unu
-000008c0: 7365 645f 636f 6e66 6967 7320 3d20 7472  sed_configs = tr
-000008d0: 7565 0d0a 7374 7269 6374 203d 2074 7275  ue..strict = tru
-000008e0: 650d 0a64 6973 616c 6c6f 775f 7375 6263  e..disallow_subc
-000008f0: 6c61 7373 696e 675f 616e 7920 3d20 6661  lassing_any = fa
-00000900: 6c73 650d 0a23 6967 6e6f 7265 5f6d 6973  lse..#ignore_mis
-00000910: 7369 6e67 5f69 6d70 6f72 7473 203d 2074  sing_imports = t
-00000920: 7275 650d 0a65 7863 6c75 6465 203d 205b  rue..exclude = [
-00000930: 0d0a 2020 225c 5c2e 6d79 7079 5f63 6163  ..  "\\.mypy_cac
-00000940: 6865 222c 0d0a 2020 225c 5c2e 7665 6e76  he",..  "\\.venv
-00000950: 222c 0d0a 2020 2262 7569 6c64 222c 0d0a  ",..  "build",..
-00000960: 2020 2264 6973 7422 2c0d 0a20 2022 6f75    "dist",..  "ou
-00000970: 7422 2c0d 0a20 2022 706c 6179 6772 6f75  t",..  "playgrou
-00000980: 6e64 222c 0d0a 2020 2273 6372 6970 7473  nd",..  "scripts
-00000990: 222c 0d0a 5d0d 0a0d 0a5b 5b74 6f6f 6c2e  ",..]....[[tool.
-000009a0: 6d79 7079 2e6f 7665 7272 6964 6573 5d5d  mypy.overrides]]
-000009b0: 0d0a 6d6f 6475 6c65 203d 205b 2272 6f62  ..module = ["rob
-000009c0: 6f74 2e2a 222c 2022 726f 626f 7469 6479  ot.*", "robotidy
-000009d0: 2e2a 222c 2022 726f 626f 636f 702e 2a22  .*", "robocop.*"
-000009e0: 5d0d 0a69 676e 6f72 655f 6d69 7373 696e  ]..ignore_missin
-000009f0: 675f 696d 706f 7274 7320 3d20 7472 7565  g_imports = true
+000000a0: 676d 6169 6c2e 636f 6d3e 225d 0d0a 686f  gmail.com>"]..ho
+000000b0: 6d65 7061 6765 203d 2022 6874 7470 733a  mepage = "https:
+000000c0: 2f2f 6769 7468 7562 2e63 6f6d 2f4d 6172  //github.com/Mar
+000000d0: 6b65 7453 7175 6172 652f 726f 626f 7466  ketSquare/robotf
+000000e0: 7261 6d65 776f 726b 2d72 6570 6f72 746d  ramework-reportm
+000000f0: 6f64 6966 6965 7222 0d0a 7265 6164 6d65  odifier"..readme
+00000100: 203d 2022 5245 4144 4d45 2e6d 6422 0d0a   = "README.md"..
+00000110: 7061 636b 6167 6573 203d 205b 0d0a 2020  packages = [..  
+00000120: 2020 7b20 696e 636c 7564 6520 3d20 2272    { include = "r
+00000130: 6570 6f72 746d 6f64 6966 6965 7222 2c20  eportmodifier", 
+00000140: 6672 6f6d 203d 2022 7372 6322 207d 2c0d  from = "src" },.
+00000150: 0a20 2020 207b 2069 6e63 6c75 6465 203d  .    { include =
+00000160: 2022 5265 706f 7274 4d6f 6469 6669 6572   "ReportModifier
+00000170: 4c69 7374 656e 6572 222c 2066 726f 6d20  Listener", from 
+00000180: 3d20 2273 7263 2220 7d0d 0a20 205d 0d0a  = "src" }..  ]..
+00000190: 0d0a 5b62 7569 6c64 2d73 7973 7465 6d5d  ..[build-system]
+000001a0: 0d0a 7265 7175 6972 6573 203d 205b 2270  ..requires = ["p
+000001b0: 6f65 7472 792d 636f 7265 225d 0d0a 6275  oetry-core"]..bu
+000001c0: 696c 642d 6261 636b 656e 6420 3d20 2270  ild-backend = "p
+000001d0: 6f65 7472 792e 636f 7265 2e6d 6173 6f6e  oetry.core.mason
+000001e0: 7279 2e61 7069 220d 0a0d 0a5b 746f 6f6c  ry.api"....[tool
+000001f0: 2e70 6f65 7472 792e 6465 7065 6e64 656e  .poetry.dependen
+00000200: 6369 6573 5d0d 0a70 7974 686f 6e20 3d20  cies]..python = 
+00000210: 225e 332e 3822 0d0a 726f 626f 7466 7261  "^3.8"..robotfra
+00000220: 6d65 776f 726b 203d 2022 5e36 2e31 220d  mework = "^6.1".
+00000230: 0a70 7964 616e 7469 6320 3d20 225e 312e  .pydantic = "^1.
+00000240: 3130 2e34 220d 0a72 756c 652d 656e 6769  10.4"..rule-engi
+00000250: 6e65 203d 2022 5e34 220d 0a0d 0a5b 746f  ne = "^4"....[to
+00000260: 6f6c 2e70 6f65 7472 792e 6772 6f75 702e  ol.poetry.group.
+00000270: 636f 6e66 6967 2e64 6570 656e 6465 6e63  config.dependenc
+00000280: 6965 735d 0d0a 5079 5941 4d4c 203d 2022  ies]..PyYAML = "
+00000290: 5e36 2e30 220d 0a70 6174 686c 6962 203d  ^6.0"..pathlib =
+000002a0: 2022 5e31 2e30 2e31 220d 0a72 6567 6578   "^1.0.1"..regex
+000002b0: 203d 2022 5e32 3032 332e 3130 2e33 220d   = "^2023.10.3".
+000002c0: 0a0d 0a5b 746f 6f6c 2e70 6f65 7472 792e  ...[tool.poetry.
+000002d0: 6772 6f75 702e 6465 762e 6465 7065 6e64  group.dev.depend
+000002e0: 656e 6369 6573 5d0d 0a72 6f62 6f74 6672  encies]..robotfr
+000002f0: 616d 6577 6f72 6b20 3d20 225e 362e 3122  amework = "^6.1"
+00000300: 0d0a 7275 6666 203d 2022 2a22 0d0a 6d79  ..ruff = "*"..my
+00000310: 7079 203d 2022 2a22 0d0a 626c 6163 6b20  py = "*"..black 
+00000320: 3d20 222a 220d 0a0d 0a5b 746f 6f6c 2e72  = "*"....[tool.r
+00000330: 7566 665d 0d0a 6c69 6e65 2d6c 656e 6774  uff]..line-lengt
+00000340: 6820 3d20 3132 300d 0a74 6172 6765 742d  h = 120..target-
+00000350: 7665 7273 696f 6e20 3d20 2270 7933 3822  version = "py38"
+00000360: 0d0a 6578 636c 7564 6520 3d20 5b0d 0a20  ..exclude = [.. 
+00000370: 2022 2e76 7363 6f64 6522 2c0d 0a20 2022   ".vscode",..  "
+00000380: 5c5c 2e76 656e 7622 2c0d 0a20 2022 2e67  \\.venv",..  ".g
+00000390: 6974 222c 0d0a 2020 222e 6d79 7079 5f63  it",..  ".mypy_c
+000003a0: 6163 6865 222c 0d0a 2020 222e 7275 6666  ache",..  ".ruff
+000003b0: 5f63 6163 6865 222c 0d0a 2020 225f 6275  _cache",..  "_bu
+000003c0: 696c 6422 2c0d 0a20 2022 6275 636b 2d6f  ild",..  "buck-o
+000003d0: 7574 222c 0d0a 2020 2262 7569 6c64 222c  ut",..  "build",
+000003e0: 0d0a 2020 2264 6973 7422 2c0d 0a20 2022  ..  "dist",..  "
+000003f0: 7461 736b 732e 7079 220d 0a5d 0d0a 0d0a  tasks.py"..]....
+00000400: 5b74 6f6f 6c2e 7275 6666 2e6c 696e 745d  [tool.ruff.lint]
+00000410: 2020 2320 4669 6c65 2072 6566 6572 656e    # File referen
+00000420: 6365 2068 6572 6520 2d20 6874 7470 733a  ce here - https:
+00000430: 2f2f 646f 6373 2e61 7374 7261 6c2e 7368  //docs.astral.sh
+00000440: 2f72 7566 662f 7275 6c65 732f 0d0a 6578  /ruff/rules/..ex
+00000450: 7465 6e64 2d73 656c 6563 7420 3d20 5b22  tend-select = ["
+00000460: 4535 3031 225d 0d0a 6967 6e6f 7265 203d  E501"]..ignore =
+00000470: 205b 2245 3734 3122 2c20 224e 3830 3522   ["E741", "N805"
+00000480: 2c20 2250 5430 3039 222c 2022 5245 5435  , "PT009", "RET5
+00000490: 3033 225d 0d0a 7365 6c65 6374 203d 205b  03"]..select = [
+000004a0: 0d0a 2020 2245 222c 0d0a 2020 2246 222c  ..  "E",..  "F",
+000004b0: 0d0a 2020 2257 222c 0d0a 2020 2249 222c  ..  "W",..  "I",
+000004c0: 0d0a 2020 224e 222c 0d0a 2020 2255 5022  ..  "N",..  "UP"
+000004d0: 2c0d 0a20 2022 5954 5422 2c0d 0a20 2022  ,..  "YTT",..  "
+000004e0: 424c 4522 2c0d 0a20 2022 4222 2c0d 0a20  BLE",..  "B",.. 
+000004f0: 2022 4122 2c0d 0a20 2022 4334 222c 0d0a   "A",..  "C4",..
+00000500: 2020 2244 545a 222c 0d0a 2020 2254 3130    "DTZ",..  "T10
+00000510: 222c 0d0a 2020 2245 4d22 2c0d 0a20 2022  ",..  "EM",..  "
+00000520: 4722 2c0d 0a20 2022 494e 5022 2c0d 0a20  G",..  "INP",.. 
+00000530: 2022 5049 4522 2c0d 0a20 2022 5432 3022   "PIE",..  "T20"
+00000540: 2c0d 0a20 2022 5054 222c 0d0a 2020 2251  ,..  "PT",..  "Q
+00000550: 222c 0d0a 2020 2252 4554 222c 0d0a 2020  ",..  "RET",..  
+00000560: 2254 4944 222c 0d0a 2020 2254 4348 222c  "TID",..  "TCH",
+00000570: 0d0a 2020 2241 5247 222c 0d0a 2020 2250  ..  "ARG",..  "P
+00000580: 5448 220d 0a5d 0d0a 0d0a 5b74 6f6f 6c2e  TH"..]....[tool.
+00000590: 7275 6666 2e6c 696e 742e 7065 722d 6669  ruff.lint.per-fi
+000005a0: 6c65 2d69 676e 6f72 6573 5d0d 0a22 5f5f  le-ignores].."__
+000005b0: 696e 6974 5f5f 2e70 7922 203d 205b 2246  init__.py" = ["F
+000005c0: 3430 3122 5d0d 0a0d 0a0d 0a5b 746f 6f6c  401"]......[tool
+000005d0: 2e6d 7970 795d 0d0a 2320 4d79 5079 2063  .mypy]..# MyPy c
+000005e0: 6f6e 6669 670d 0a23 2046 696c 6520 7265  onfig..# File re
+000005f0: 6665 7265 6e63 6520 6865 7265 202d 2068  ference here - h
+00000600: 7474 703a 2f2f 6d79 7079 2e72 6561 6474  ttp://mypy.readt
+00000610: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
+00000620: 6573 742f 636f 6e66 6967 5f66 696c 652e  est/config_file.
+00000630: 6874 6d6c 2363 6f6e 6669 672d 6669 6c65  html#config-file
+00000640: 0d0a 7079 7468 6f6e 5f76 6572 7369 6f6e  ..python_version
+00000650: 203d 2033 2e38 0d0a 7761 726e 5f72 6564   = 3.8..warn_red
+00000660: 756e 6461 6e74 5f63 6173 7473 203d 2074  undant_casts = t
+00000670: 7275 650d 0a77 6172 6e5f 756e 7573 6564  rue..warn_unused
+00000680: 5f69 676e 6f72 6573 203d 2074 7275 650d  _ignores = true.
+00000690: 0a77 6172 6e5f 7265 7475 726e 5f61 6e79  .warn_return_any
+000006a0: 203d 2074 7275 650d 0a77 6172 6e5f 756e   = true..warn_un
+000006b0: 7573 6564 5f63 6f6e 6669 6773 203d 2074  used_configs = t
+000006c0: 7275 650d 0a73 7472 6963 7420 3d20 7472  rue..strict = tr
+000006d0: 7565 0d0a 6469 7361 6c6c 6f77 5f73 7562  ue..disallow_sub
+000006e0: 636c 6173 7369 6e67 5f61 6e79 203d 2066  classing_any = f
+000006f0: 616c 7365 0d0a 2369 676e 6f72 655f 6d69  alse..#ignore_mi
+00000700: 7373 696e 675f 696d 706f 7274 7320 3d20  ssing_imports = 
+00000710: 7472 7565 0d0a 6578 636c 7564 6520 3d20  true..exclude = 
+00000720: 5b0d 0a20 2022 5c5c 2e6d 7970 795f 6361  [..  "\\.mypy_ca
+00000730: 6368 6522 2c0d 0a20 2022 5c5c 2e76 656e  che",..  "\\.ven
+00000740: 7622 2c0d 0a20 2022 6275 696c 6422 2c0d  v",..  "build",.
+00000750: 0a20 2022 6469 7374 222c 0d0a 2020 226f  .  "dist",..  "o
+00000760: 7574 222c 0d0a 2020 2270 6c61 7967 726f  ut",..  "playgro
+00000770: 756e 6422 2c0d 0a20 2022 7363 7269 7074  und",..  "script
+00000780: 7322 0d0a 5d0d 0a0d 0a5b 5b74 6f6f 6c2e  s"..]....[[tool.
+00000790: 6d79 7079 2e6f 7665 7272 6964 6573 5d5d  mypy.overrides]]
+000007a0: 0d0a 6d6f 6475 6c65 203d 205b 2272 6f62  ..module = ["rob
+000007b0: 6f74 2e2a 222c 2022 726f 626f 7469 6479  ot.*", "robotidy
+000007c0: 2e2a 222c 2022 726f 626f 636f 702e 2a22  .*", "robocop.*"
+000007d0: 5d0d 0a69 676e 6f72 655f 6d69 7373 696e  ]..ignore_missin
+000007e0: 675f 696d 706f 7274 7320 3d20 7472 7565  g_imports = true
```

### Comparing `robotframework_reportmodifier-0.1.9/README.md` & `robotframework_reportmodifier-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -44,21 +44,22 @@
  - Second Level Keyword. Third Level Keyword    → All logged contents of the keyword *Second Level Keyword. Third Level Keyword* are included, regardless of how often this call was made in the test case.
 ```
 
 **Option "messages"**
 
 Filtering based on message content.
 
-The message configuration collects logs that contain a specific text or correspond to a specific regular expression. It means, the message is valid as soos as defined text is found in the message or the regular expression has any foundings. For the definition of the RegEx pattern, we recommend an online test, e.g. on regex.com. Characters such as $ must be escaped with a backslash (\).
+The message configuration collects logs that contain a specific text or correspond to a specific regular expression. It means, the message is valid as soon as defined text is found in the message or the regular expression has any foundings. For the definition of the RegEx pattern, we recommend an online test, e.g. on regex.com. Characters such as $ must be escaped with a backslash (\). You can specify text, pattern of status.
 Examples: 
 ```shell
 message = "Starting test case with a custom log."
 messages:
  - text: custom                → Log is relevant because message contains the word "custom" 
  - pattern: Starting .* log    → Log is relevant because regex.findall("Starting .* log", "message", regex.IGNORECASE) returns at least one hit
+ - status: FAIL | PASS | SKIP  → Log is relevant if the message level is equal to predefined status
 ```
 
 **Option "ignored_messages"**
 
 Removal of unwanted content that was taken along by previous configuration, e.g.:
 
 message 1 = "Starting test case with a custom log."
```

### Comparing `robotframework_reportmodifier-0.1.9/src/reportmodifier/_file_tools.py` & `robotframework_reportmodifier-0.2.0/src/reportmodifier/_file_tools.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import os
+from pathlib import Path
+from typing import Dict, Union
 
 
-def get_files_in_folder(top_level_dir, condition_callback=None, recursive=True):
-    """ Similar to the a bit overloaded function list_files_in_folder(). The result is basically the same: A dict with
+def get_files_in_folder(top_level_dir: Union[str, Path], condition_callback=None, recursive=True) -> Dict:
+    """Similar to the a bit overloaded function list_files_in_folder(). The result is basically the same: A dict with
     the base file name as key and the full file path as value. But this function eliminates an unpleasant flaw of
     list_files_in_folder(), if its argument name_as_key is True: It lists truly ALL files. If a file appears in
     multiple sub-directories with the same name, list_files_in_folder() lists it only once, any other appearance is
     being ignored. This function lists those files anyway by prefixing the base file with the sub-directory name.
     Example: There are two files:
-        D:\temp\1.txt
-        D:\temp\subdir\1.txt
-    list_files_in_folder(r'D:\temp', name_as_key=True) returns {'1.txt': 'D:\temp\subdir\1.txt'}
-    get_files_in_folder(r'D:\temp') returns {'1.txt': 'D:\temp\1.txt', 'subdir\1.txt': 'D:\temp\subdir\1.txt'}
+        D:/temp/1.txt
+        D:/temp/subdir/1.txt
+    list_files_in_folder(r'D:\temp', name_as_key=True) returns {'1.txt': 'D:/temp/subdir/1.txt'}
+    get_files_in_folder(r'D:\temp') returns {'1.txt': 'D:\temp\1.txt', 'subdir\1.txt': 'D:/temp/subdir/1.txt'}
     Another feature of this function is to define a condition which is a callback function to check the file for
     validity. This callback function must take one parameter 'path' and must return True or False.
     """
-    result = dict()
-    for root, dirs, files in os.walk(top_level_dir):
+    result = {}
+    for root, _, files in os.walk(top_level_dir):
         for f in files:
-            path = os.path.join(root, f)
+            path = os.path.join(root, f)  # noqa: PTH118
             if condition_callback is None or condition_callback(path):
                 result[os.path.relpath(path, top_level_dir)] = os.path.normpath(path)
         if not recursive:
             return result
     return result
```

### Comparing `robotframework_reportmodifier-0.1.9/src/reportmodifier/_report_configuration.py` & `robotframework_reportmodifier-0.2.0/src/reportmodifier/_report_configuration.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,85 +14,83 @@
         self.__keyword_names_as_info = None
         self.__keyword_as_structure = None
 
     def __config(self) -> Dict:
         if self.__path is None:
             self.__yaml_config = {}
             return self.__yaml_config
-        assert Path(self.__path).exists(
-        ) is True, f"Configuration path does not exist! {self.__path}"
+        assert Path(self.__path).exists() is True, f"Configuration path does not exist! {self.__path}"
         if self.__yaml_config is None:
-            self.__yaml_config = yaml.safe_load(
-                Path(self.__path).read_text(encoding="utf-8"))
+            self.__yaml_config = yaml.safe_load(Path(self.__path).read_text(encoding="utf-8"))
         return self.__yaml_config
 
     @property
     def keyword_as_structure(self) -> List:
         if self.__keyword_as_structure is None:
             self.__keyword_as_structure = []
-            keywords = self.__config().get('keyword_as_structure')
+            keywords = self.__config().get("keyword_as_structure")
             if keywords is not None:
-                self.__keyword_as_structure = [
-                    KeywordAsStructure(c) for c in list(keywords)]
+                self.__keyword_as_structure = [KeywordAsStructure(c) for c in list(keywords)]
         return self.__keyword_as_structure
 
     @property
     def keywords(self) -> List:
         if self.__keywords is None:
             self.__keywords = []
-            if self.__config().get('keywords') is not None:
-                self.__keywords = [KeywordConfig(c) for c in list(
-                    self.__config().get('keywords'))]
+            if self.__config().get("keywords") is not None:
+                self.__keywords = [KeywordConfig(c) for c in list(self.__config().get("keywords"))]
         return self.__keywords
 
     @property
     def keyword_names(self) -> List:
         return [k.name for k in self.keywords]
 
     def _message_configs(self) -> List:
         if self.__messages is None:
-            self.__messages = list()
-            if 'messages' in list(self.__config()):
-                self.__messages = [MessageConfig(
-                    c) for c in list(self.__config()['messages'])]
+            self.__messages = []
+            if "messages" in list(self.__config()):
+                self.__messages = [MessageConfig(c) for c in list(self.__config()["messages"])]
         return self.__messages
 
     @property
     def message_pattern(self) -> List:
-        return list(set([k.pattern for k in self._message_configs() if k.pattern is not None]))
+        return list({k.pattern for k in self._message_configs() if k.pattern is not None})
 
     @property
     def message_text(self) -> List:
-        self.message_pattern
-        return list(set([k.text for k in self._message_configs() if k.text is not None]))
+        self.message_pattern  # noqa: B018
+        return list({k.text for k in self._message_configs() if k.text is not None})
+
+    @property
+    def message_status(self) -> List:
+        self.message_pattern  # noqa: B018
+        return list({k.status for k in self._message_configs() if k.status is not None})
 
     def _ignored_message_configs(self) -> List:
         if self.__ignored_messages is None:
-            self.__ignored_messages = list()
-            if 'ignored_messages' in list(self.__config()):
-                self.__ignored_messages = [MessageConfig(
-                    c) for c in list(self.__config()['ignored_messages'])]
+            self.__ignored_messages = []
+            if "ignored_messages" in list(self.__config()):
+                self.__ignored_messages = [MessageConfig(c) for c in list(self.__config()["ignored_messages"])]
         return self.__ignored_messages
 
     @property
     def ignored_message_pattern(self) -> List:
         return [k.pattern for k in self._ignored_message_configs() if k.pattern is not None]
 
     @property
     def ignored_messages(self) -> List:
-        self.ignored_message_pattern
+        self.ignored_message_pattern  # noqa: B018
         return [c.text for c in self._ignored_message_configs() if c.text is not None]
 
     @property
     def names_as_info(self) -> List:
         if self.__keyword_names_as_info is None:
-            self.__keyword_names_as_info = list()
-            if 'keyword_name_as_info' in list(self.__config()):
-                self.__keyword_names_as_info = [NameAsInfo(c) for c in list(
-                    self.__config()['keyword_name_as_info'])]
+            self.__keyword_names_as_info = []
+            if "keyword_name_as_info" in list(self.__config()):
+                self.__keyword_names_as_info = [NameAsInfo(c) for c in list(self.__config()["keyword_name_as_info"])]
         return [k.name for k in self.__keyword_names_as_info]
 
 
 class KeywordConfig:
     def __init__(self, config: Union[str, Dict]) -> None:
         self.__config = config
 
@@ -101,73 +99,78 @@
         if isinstance(self.__config, str):
             result = self.__config.split("[")[0].strip()
             if "." not in result:
                 result = result.strip()
             else:
                 result = result.split(".")[-1]
         elif isinstance(self.__config, dict):
-            result = self.__config.get('name')
+            result = self.__config.get("name")
         return result
 
     @property
     def path(self) -> str:
         if isinstance(self.__config, dict):
-            return self.__config.get('path')
-        path = self.__config.split('[')[0].strip()
-        path_parts = path.split('.')
+            return self.__config.get("path")
+        path = self.__config.split("[")[0].strip()
+        path_parts = path.split(".")
         if len(path_parts) > 1:
             return path
 
     @property
     def index(self) -> Union[List, None]:
         if isinstance(self.__config, dict):
-            i = self.__config.get('index')
+            i = self.__config.get("index")
             if i and not isinstance(i, list):
                 i = [i]
             return i
-        parts = self.__config.split('[')
+        parts = self.__config.split("[")
         if len(parts) > 1:
-            return [int(i) for i in parts[-1].replace(']', '').split(',')]
+            return [int(i) for i in parts[-1].replace("]", "").split(",")]
 
     @property
     def set(self):
         if isinstance(self.__config, dict):
-            return self.__config.get('set')
+            return self.__config.get("set")
         return False
 
 
 class MessageConfig:
     def __init__(self, config) -> None:
         self.__config = config
 
     @property
     def pattern(self):
         if isinstance(self.__config, dict):
-            return self.__config.get('pattern')
+            return self.__config.get("pattern")
         return self.__config
 
     @property
     def text(self):
         if isinstance(self.__config, dict):
-            return self.__config.get('text')
+            return self.__config.get("text")
+
+    @property
+    def status(self):
+        if isinstance(self.__config, dict):
+            return self.__config.get("status")
 
 
 class NameAsInfo:
     def __init__(self, config) -> None:
         self.__config = config
 
     @property
     def name(self):
         if isinstance(self.__config, dict):
-            return self.__config.get('name')
+            return self.__config.get("name")
         return self.__config
 
 
 class KeywordAsStructure:
     def __init__(self, config) -> None:
         self.__config = config
 
     @property
     def name(self):
         if isinstance(self.__config, dict):
-            return self.__config.get('name')
+            return self.__config.get("name")
         return self.__config
```

### Comparing `robotframework_reportmodifier-0.1.9/src/reportmodifier/ReportModifierVisitor.py` & `robotframework_reportmodifier-0.2.0/src/reportmodifier/ReportModifierVisitor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# noqa: N999
 from collections import defaultdict
 from copy import deepcopy
 from pathlib import Path
 
 import regex
 from robot.api import logger
 from robot.model import TestSuite
@@ -14,24 +15,25 @@
 class ReportModifierVisitor(ResultVisitor):
     def __init__(self) -> None:
         super().__init__()
         self.report_configuration = ReportConfiguration(None)
         self.basic_configuration = ReportConfiguration(None)
         self.__report_name = None
         self.__keyword_calls = defaultdict(int)
-        self._relevant_keyword_calls = list()
+        self._relevant_keyword_calls = []
         self._relevant_messages = defaultdict(list)
         self._keyword = None
+        self._keyword_path = ""
         self.__root = None
-        self._tests = list()
+        self._tests = []
 
     @property
     def report_name(self):
         if self.__report_name is None:
-            return 'custom_log'
+            return "custom_log"
         return self.__report_name
 
     @report_name.setter
     def report_name(self, name):
         self.__report_name = name
 
     def start_suite(self, suite: TestSuite) -> bool | None:
@@ -46,31 +48,35 @@
             suite.tests.clear()
             suite.tests = self._tests
         if suite.has_teardown:
             suite.teardown = None
 
     def start_test(self, test: TestCase):
         self._relevant_messages = defaultdict(list)
-        self._relevant_keyword_calls = list()
+        self._relevant_keyword_calls = []
         self.report_configuration = ReportConfiguration(None)
         for tag in test.tags:
-            if tag.startswith(('fb_report:', 'report:')):
-                report_configuration = tag.split('report:')[-1].strip()
+            if tag.startswith(("fb_report:", "report:")):
+                report_configuration = tag.split("report:")[-1].strip()
                 test_path = Path(test.source)
-                test_dir = Path(*test_path.parts[0:test_path.parts.index('tests')+1])
+                test_dir = Path(*test_path.parts[0 : test_path.parts.index("tests") + 1])
                 configuration_path = get_files_in_folder(
                     top_level_dir=test_dir,
-                    condition_callback=lambda p: Path(p).stem.lower() == report_configuration.split('.yaml')[0].lower() and Path(p).suffix == '.yaml',
-                    recursive=True)
+                    condition_callback=lambda p: Path(p).stem.lower() == report_configuration.split(".yaml")[0].lower()  # noqa: B023
+                    and Path(p).suffix == ".yaml",
+                    recursive=True,
+                )
                 if not configuration_path:
-                    logger.error(f'Could not find custon log configuration "{report_configuration}" of test  {test.name}')
+                    logger.error(
+                        f'Could not find custon log configuration "{report_configuration}" of test  {test.name}',
+                    )
                     return False
                 path = list(configuration_path.values())[0]
-                logger.info(f'Found log configuration of fest: {test.name}: {tag} {path}')
-                if report_configuration.lower() == 'basic_config':
+                logger.info(f"Found log configuration of fest: {test.name}: {tag} {path}")
+                if report_configuration.lower() == "basic_config":
                     self.basic_configuration = ReportConfiguration(path)
                 else:
                     self.report_configuration = ReportConfiguration(path)
                     if self.__report_name is None:
                         self.__report_name = report_configuration
                 break
 
@@ -84,167 +90,202 @@
                     keyword.args = []
                     keyword.body = messages
                     test.body.append(keyword)
                 else:
                     test.body += messages
             test.setup = None
             test.teardown = None
-            logger.debug(f'Relevant keywords: {self._relevant_keyword_calls}')
+            logger.debug(f"Relevant keywords: {self._relevant_keyword_calls}")
         self._tests.append(deepcopy(test))
 
     def start_keyword(self, keyword: Keyword):
         if self.report_configuration or self.basic_configuration:
-            logger.debug(f'Checking {keyword.kwname} --> {keyword.libname} --> {keyword.parent.name}')
+            logger.debug(f"Checking {keyword.kwname} --> {keyword.libname} --> {keyword.parent.name}")
             self.__keyword_calls[keyword.kwname] += 1
             if _keyword_name_for_structure_is_relevant(
-                    keyword.kwname, [k.name for k in self.report_configuration.keyword_as_structure]):
+                keyword.kwname,
+                [k.name for k in self.report_configuration.keyword_as_structure],
+            ):
                 self._keyword = keyword
-            if _keyword_name_as_info_is_relevant(keyword,
-                                                 self.report_configuration,
-                                                 self.basic_configuration):
+                self._keyword_path = _get_keyword_call_path(keyword)
+            if _keyword_name_as_info_is_relevant(keyword, self.report_configuration, self.basic_configuration):
                 msg = f'<b><mark style="background:powderblue">{keyword.name.strip()}</mark></b>\n{keyword.doc.strip()}'
-                message = Message(msg, level='INFO', html=True, timestamp=keyword.starttime)
+                message = Message(msg, level="INFO", html=True, timestamp=keyword.starttime)
                 self._relevant_messages[self._keyword].append(message)
                 self._relevant_keyword_calls.append(_get_keyword_call_path(keyword))
-            if _all_keyword_messages_are_relevant(keyword,
-                                                  self.__keyword_calls[keyword.kwname],
-                                                  self._relevant_messages[self._keyword],
-                                                  self.report_configuration,
-                                                  self.basic_configuration):
-                logger.debug(f'Found relevant keyword {keyword.kwname}')
+            if _all_keyword_messages_are_relevant(
+                keyword,
+                self.__keyword_calls[keyword.kwname],
+                self._relevant_messages[self._keyword],
+                self.report_configuration,
+                self.basic_configuration,
+            ):
+                logger.debug(f"Found relevant keyword {keyword.kwname}")
                 last_message = _get_last_message(self._relevant_messages[self._keyword])
-                submessages = list()
+                submessages = []
                 submessages = _get_all_submessages(keyword.body, submessages)
-                relevant_messages = [m for m in keyword.messages + submessages if
-                                     not _message_shall_be_ignored(m.message,
-                                                                   self.report_configuration,
-                                                                   self.basic_configuration,
-                                                                   last_message)]
+                relevant_messages = [
+                    m
+                    for m in keyword.messages + submessages
+                    if not _message_shall_be_ignored(
+                        m.message,
+                        self.report_configuration,
+                        self.basic_configuration,
+                        last_message,
+                    )
+                ]
                 if relevant_messages:
                     self._relevant_messages[self._keyword] += relevant_messages
                     self._relevant_keyword_calls.append(_get_keyword_call_path(keyword))
 
-    def end_keyword(self, keyword: Keyword):
-        self._keyword = None
+    def end_keyword(self, keyword: Keyword):  # noqa: ARG002
+        if self._keyword and self._keyword_path not in _get_keyword_call_path(keyword):
+            self._keyword = None
 
     def start_message(self, msg: Message):
         if self.report_configuration or self.basic_configuration:
             last_message = _get_last_message(self._relevant_messages[self._keyword])
-            if _message_content_is_relevant(msg.message,
-                                            self.report_configuration,
-                                            self.basic_configuration,
-                                            last_message):
+            if _message_content_is_relevant(
+                msg.message,
+                self.report_configuration,
+                self.basic_configuration,
+                last_message,
+            ):
+                self._relevant_messages[self._keyword].append(msg)
+                self._relevant_keyword_calls.append(_get_keyword_call_path(msg.parent))
+            if _message_status_is_relevant(
+                msg.level, self.report_configuration.message_status + self.basic_configuration.message_status
+            ):
                 self._relevant_messages[self._keyword].append(msg)
                 self._relevant_keyword_calls.append(_get_keyword_call_path(msg.parent))
 
     def end_message(self, msg: Message):
         pass
 
 
 def _get_all_submessages(keywords__, submessages_):
     for keyword in keywords__:
         if not isinstance(keyword, Keyword):
             continue
-        submessages_ += [l for l in keyword.messages]
+        submessages_ += list(keyword.messages)
         if keyword.body:
             _get_all_submessages(keyword.body, submessages_)
     return submessages_
 
 
 def _get_last_message(messages):
     if messages:
         return messages[-1].message
     return ""
 
 
 def _keyword_name_for_structure_is_relevant(keyword_name: str, accepted_names: list) -> bool:
-    return keyword_name.lower().strip() in [k.lower().strip() for k in accepted_names]
+    for accepted_name in accepted_names:
+        pattern = f"^{accepted_name}"
+        if regex.findall(pattern, keyword_name, regex.I):
+            return True
+    return False
 
 
 def _check_name_relevance(keyword_name, keywords) -> list:
     return list(filter(lambda k: k.name is None or k.name.lower() == keyword_name.lower(), keywords))
 
 
 def _get_keyword_call_path(keyword):
     # first instance needs to be a keyword not a warn or error of report summary
     if not isinstance(keyword, Keyword):
-        return ''
+        return ""
     path = [keyword.kwname]
     k = keyword
     while k.parent:
         k = k.parent
         if isinstance(k, Keyword):
             path.append(k.kwname)
         if isinstance(k, TestCase):
             path.append(k.name)
             break
 
     keyword_path = ".".join(reversed(path))
-    return keyword_path
+    return keyword_path  # noqa: RET504
 
 
 def _check_path_relevance(keyword, keywords):
-    """ returns keywords which 
-    - path is a part of given keyword path or 
-    - path is None """
+    """returns keywords which
+    - path is a part of given keyword path or
+    - path is None"""
     keyword_path = _get_keyword_call_path(keyword)
     return [k for k in keywords if k.path is None or k.path.lower() in keyword_path.lower()]
 
 
 def _check_index_relevance(call_index, keywords):
     return list(filter(lambda k: k.index is None or call_index in k.index, keywords))
 
 
 def _keyword_name_as_info_is_relevant(keyword, report_configuration, basic_configuration):
     keyword_path = _get_keyword_call_path(keyword)
-    for name_as_info in report_configuration.names_as_info+basic_configuration.names_as_info:
-        if keyword_path.lower().endswith(name_as_info.lower()):
+    for name_as_info in report_configuration.names_as_info + basic_configuration.names_as_info:
+        pattern = f"{name_as_info}$"
+        if regex.findall(pattern, keyword_path, regex.I):
             return True
     return False
 
 
 def _all_keyword_messages_are_relevant(keyword, call_index, report_messages, report_configuration, basic_configuration):
-    same_name_keywords = _check_name_relevance(keyword.kwname, report_configuration.keywords+basic_configuration.keywords)
+    same_name_keywords = _check_name_relevance(
+        keyword.kwname,
+        report_configuration.keywords + basic_configuration.keywords,
+    )
     if not same_name_keywords:
         return False
 
     same_path_keywords = _check_path_relevance(keyword, same_name_keywords)
     if not same_path_keywords:
         return False
-    
+
     same_index_keywords = _check_index_relevance(call_index, same_path_keywords)
     if not same_index_keywords:
         return False
 
-    if True in [k.set for k in same_index_keywords] and \
-        keyword.messages[0].message in [m.message for m in report_messages]:
-            return False
+    if True in [k.set for k in same_index_keywords] and keyword.messages[0].message in [
+        m.message for m in report_messages
+    ]:
+        return False
 
     return True
 
 
 def _message_shall_be_ignored(message, report_configuration, basic_configuration, last_message):
     if message == last_message:  # same messages next to each other are never needed
         return True
 
-    for ignored_message in report_configuration.ignored_messages+basic_configuration.ignored_messages:
+    for ignored_message in report_configuration.ignored_messages + basic_configuration.ignored_messages:
         if ignored_message.lower() in message.lower():
             return True
 
-    for pattern in report_configuration.ignored_message_pattern+basic_configuration.ignored_message_pattern:
-        if regex.findall(pattern, message, regex.I+regex.DOTALL):
+    for pattern in report_configuration.ignored_message_pattern + basic_configuration.ignored_message_pattern:
+        if regex.findall(pattern, message, regex.I + regex.DOTALL):
             return True
     return False
 
 
 def _message_content_is_relevant(message, report_configuration, basic_configuration, last_message):
     if _message_shall_be_ignored(message, report_configuration, basic_configuration, last_message):
         return False
 
-    for pattern in report_configuration.message_pattern+basic_configuration.message_pattern:
-        if regex.findall(pattern, message, regex.I+regex.DOTALL):
+    for pattern in report_configuration.message_pattern + basic_configuration.message_pattern:
+        if regex.findall(pattern, message, regex.I + regex.DOTALL):
             return True
 
-    for text in report_configuration.message_text+basic_configuration.message_text:
+    for text in report_configuration.message_text + basic_configuration.message_text:
         if text.lower() in message.lower():
             return True
     return False
+
+
+def _message_status_is_relevant(message_level: str, relevant_levels: list):
+    """checks if message is relevant due to his status
+
+    Args:
+        message_level (str): Level of the message to be checked
+        relevant_levels (lsit): List with accepted levels
+    """
+    return message_level.lower() in [r.lower() for r in relevant_levels]
```

### Comparing `robotframework_reportmodifier-0.1.9/PKG-INFO` & `robotframework_reportmodifier-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: robotframework-reportmodifier
-Version: 0.1.9
+Version: 0.2.0
 Summary: Filter report content.
+Home-page: https://github.com/MarketSquare/robotframework-reportmodifier
 Author: Matthias Gunther
 Author-email: matthiasgunther@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pydantic (>=1.10.4,<2.0.0)
-Requires-Dist: robotframework (>=4.1)
-Requires-Dist: rule-engine (>=3.5.0,<4.0.0)
+Requires-Dist: robotframework (>=6.1,<7.0)
+Requires-Dist: rule-engine (>=4,<5)
 Description-Content-Type: text/markdown
 
 ## Introduction 
 The high complexity of tests and the amount of information that can be logged makes the final report very confusing and unreadable for colleagues who aren't testers with Robot Framework knowledge but need to know the rough test flow and result. To provide a better overview of the test content, the library can filter the content by message content, keyword names or even keyword paths.
 
 ## Configuration assignment
 
@@ -62,21 +63,22 @@
  - Second Level Keyword. Third Level Keyword    → All logged contents of the keyword *Second Level Keyword. Third Level Keyword* are included, regardless of how often this call was made in the test case.
 ```
 
 **Option "messages"**
 
 Filtering based on message content.
 
-The message configuration collects logs that contain a specific text or correspond to a specific regular expression. It means, the message is valid as soos as defined text is found in the message or the regular expression has any foundings. For the definition of the RegEx pattern, we recommend an online test, e.g. on regex.com. Characters such as $ must be escaped with a backslash (\).
+The message configuration collects logs that contain a specific text or correspond to a specific regular expression. It means, the message is valid as soon as defined text is found in the message or the regular expression has any foundings. For the definition of the RegEx pattern, we recommend an online test, e.g. on regex.com. Characters such as $ must be escaped with a backslash (\). You can specify text, pattern of status.
 Examples: 
 ```shell
 message = "Starting test case with a custom log."
 messages:
  - text: custom                → Log is relevant because message contains the word "custom" 
  - pattern: Starting .* log    → Log is relevant because regex.findall("Starting .* log", "message", regex.IGNORECASE) returns at least one hit
+ - status: FAIL | PASS | SKIP  → Log is relevant if the message level is equal to predefined status
 ```
 
 **Option "ignored_messages"**
 
 Removal of unwanted content that was taken along by previous configuration, e.g.:
 
 message 1 = "Starting test case with a custom log."
```

