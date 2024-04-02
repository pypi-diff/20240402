# Comparing `tmp/robotframework_reportmodifier-0.2.0.tar.gz` & `tmp/robotframework_reportmodifier-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_reportmodifier-0.2.0.tar", max compression
+gzip compressed data, was "robotframework_reportmodifier-0.2.1.tar", max compression
```

## Comparing `robotframework_reportmodifier-0.2.0.tar` & `robotframework_reportmodifier-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35801 2024-02-12 08:28:04.348570 robotframework_reportmodifier-0.2.0/LICENSE
--rw-r--r--   0        0        0     2032 2024-03-28 08:50:33.654585 robotframework_reportmodifier-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4848 2024-03-28 08:21:54.396809 robotframework_reportmodifier-0.2.0/README.md
--rw-r--r--   0        0        0       44 2024-03-28 08:26:32.278869 robotframework_reportmodifier-0.2.0/src/reportmodifier/__init__.py
--rw-r--r--   0        0        0       22 2024-03-18 14:55:57.436001 robotframework_reportmodifier-0.2.0/src/reportmodifier/__version__.py
--rw-r--r--   0        0        0     1664 2024-03-26 08:36:58.839614 robotframework_reportmodifier-0.2.0/src/reportmodifier/_file_tools.py
--rw-r--r--   0        0        0     5981 2024-03-26 12:34:37.585293 robotframework_reportmodifier-0.2.0/src/reportmodifier/_report_configuration.py
--rw-r--r--   0        0        0     6905 2024-03-28 08:46:21.576313 robotframework_reportmodifier-0.2.0/src/reportmodifier/ReportModifier.py
--rw-r--r--   0        0        0    11922 2024-03-28 08:42:48.616199 robotframework_reportmodifier-0.2.0/src/reportmodifier/ReportModifierVisitor.py
--rw-r--r--   0        0        0       79 2024-03-18 15:11:07.246558 robotframework_reportmodifier-0.2.0/src/ReportModifierListener/__init__.py
--rw-r--r--   0        0        0      879 2024-03-27 07:28:27.461714 robotframework_reportmodifier-0.2.0/src/ReportModifierListener/ReportModifierListener.py
--rw-r--r--   0        0        0     5482 1970-01-01 00:00:00.000000 robotframework_reportmodifier-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35801 2024-02-12 08:28:04.348570 robotframework_reportmodifier-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2005 2024-04-02 09:07:29.799020 robotframework_reportmodifier-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4848 2024-03-28 08:21:54.396809 robotframework_reportmodifier-0.2.1/README.md
+-rw-r--r--   0        0        0       44 2024-03-28 08:26:32.278869 robotframework_reportmodifier-0.2.1/src/reportmodifier/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-02 09:04:48.042038 robotframework_reportmodifier-0.2.1/src/reportmodifier/__version__.py
+-rw-r--r--   0        0        0     1664 2024-03-26 08:36:58.839614 robotframework_reportmodifier-0.2.1/src/reportmodifier/_file_tools.py
+-rw-r--r--   0        0        0     5981 2024-03-26 12:34:37.585293 robotframework_reportmodifier-0.2.1/src/reportmodifier/_report_configuration.py
+-rw-r--r--   0        0        0     6905 2024-03-28 08:46:21.576313 robotframework_reportmodifier-0.2.1/src/reportmodifier/ReportModifier.py
+-rw-r--r--   0        0        0    11986 2024-04-02 09:04:07.994579 robotframework_reportmodifier-0.2.1/src/reportmodifier/ReportModifierVisitor.py
+-rw-r--r--   0        0        0       79 2024-03-18 15:11:07.246558 robotframework_reportmodifier-0.2.1/src/ReportModifierListener/__init__.py
+-rw-r--r--   0        0        0      879 2024-03-27 07:28:27.461714 robotframework_reportmodifier-0.2.1/src/ReportModifierListener/ReportModifierListener.py
+-rw-r--r--   0        0        0     5433 1970-01-01 00:00:00.000000 robotframework_reportmodifier-0.2.1/PKG-INFO
```

### Comparing `robotframework_reportmodifier-0.2.0/LICENSE` & `robotframework_reportmodifier-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_reportmodifier-0.2.0/pyproject.toml` & `robotframework_reportmodifier-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 5b74 6f6f 6c2e 706f 6574 7279 5d0d 0a6e  [tool.poetry]..n
 00000010: 616d 6520 3d20 2272 6f62 6f74 6672 616d  ame = "robotfram
 00000020: 6577 6f72 6b2d 7265 706f 7274 6d6f 6469  ework-reportmodi
 00000030: 6669 6572 220d 0a76 6572 7369 6f6e 203d  fier"..version =
-00000040: 2022 302e 322e 3022 0d0a 6465 7363 7269   "0.2.0"..descri
+00000040: 2022 302e 322e 3122 0d0a 6465 7363 7269   "0.2.1"..descri
 00000050: 7074 696f 6e20 3d20 2246 696c 7465 7220  ption = "Filter 
 00000060: 7265 706f 7274 2063 6f6e 7465 6e74 2e22  report content."
 00000070: 0d0a 6175 7468 6f72 7320 3d20 5b22 4d61  ..authors = ["Ma
 00000080: 7474 6869 6173 2047 756e 7468 6572 203c  tthias Gunther <
 00000090: 6d61 7474 6869 6173 6775 6e74 6865 7240  matthiasgunther@
 000000a0: 676d 6169 6c2e 636f 6d3e 225d 0d0a 686f  gmail.com>"]..ho
 000000b0: 6d65 7061 6765 203d 2022 6874 7470 733a  mepage = "https:
@@ -28,100 +28,99 @@
 000001b0: 6f65 7472 792d 636f 7265 225d 0d0a 6275  oetry-core"]..bu
 000001c0: 696c 642d 6261 636b 656e 6420 3d20 2270  ild-backend = "p
 000001d0: 6f65 7472 792e 636f 7265 2e6d 6173 6f6e  oetry.core.mason
 000001e0: 7279 2e61 7069 220d 0a0d 0a5b 746f 6f6c  ry.api"....[tool
 000001f0: 2e70 6f65 7472 792e 6465 7065 6e64 656e  .poetry.dependen
 00000200: 6369 6573 5d0d 0a70 7974 686f 6e20 3d20  cies]..python = 
 00000210: 225e 332e 3822 0d0a 726f 626f 7466 7261  "^3.8"..robotfra
-00000220: 6d65 776f 726b 203d 2022 5e36 2e31 220d  mework = "^6.1".
-00000230: 0a70 7964 616e 7469 6320 3d20 225e 312e  .pydantic = "^1.
-00000240: 3130 2e34 220d 0a72 756c 652d 656e 6769  10.4"..rule-engi
-00000250: 6e65 203d 2022 5e34 220d 0a0d 0a5b 746f  ne = "^4"....[to
-00000260: 6f6c 2e70 6f65 7472 792e 6772 6f75 702e  ol.poetry.group.
-00000270: 636f 6e66 6967 2e64 6570 656e 6465 6e63  config.dependenc
-00000280: 6965 735d 0d0a 5079 5941 4d4c 203d 2022  ies]..PyYAML = "
-00000290: 5e36 2e30 220d 0a70 6174 686c 6962 203d  ^6.0"..pathlib =
-000002a0: 2022 5e31 2e30 2e31 220d 0a72 6567 6578   "^1.0.1"..regex
-000002b0: 203d 2022 5e32 3032 332e 3130 2e33 220d   = "^2023.10.3".
-000002c0: 0a0d 0a5b 746f 6f6c 2e70 6f65 7472 792e  ...[tool.poetry.
-000002d0: 6772 6f75 702e 6465 762e 6465 7065 6e64  group.dev.depend
-000002e0: 656e 6369 6573 5d0d 0a72 6f62 6f74 6672  encies]..robotfr
-000002f0: 616d 6577 6f72 6b20 3d20 225e 362e 3122  amework = "^6.1"
-00000300: 0d0a 7275 6666 203d 2022 2a22 0d0a 6d79  ..ruff = "*"..my
-00000310: 7079 203d 2022 2a22 0d0a 626c 6163 6b20  py = "*"..black 
-00000320: 3d20 222a 220d 0a0d 0a5b 746f 6f6c 2e72  = "*"....[tool.r
-00000330: 7566 665d 0d0a 6c69 6e65 2d6c 656e 6774  uff]..line-lengt
-00000340: 6820 3d20 3132 300d 0a74 6172 6765 742d  h = 120..target-
-00000350: 7665 7273 696f 6e20 3d20 2270 7933 3822  version = "py38"
-00000360: 0d0a 6578 636c 7564 6520 3d20 5b0d 0a20  ..exclude = [.. 
-00000370: 2022 2e76 7363 6f64 6522 2c0d 0a20 2022   ".vscode",..  "
-00000380: 5c5c 2e76 656e 7622 2c0d 0a20 2022 2e67  \\.venv",..  ".g
-00000390: 6974 222c 0d0a 2020 222e 6d79 7079 5f63  it",..  ".mypy_c
-000003a0: 6163 6865 222c 0d0a 2020 222e 7275 6666  ache",..  ".ruff
-000003b0: 5f63 6163 6865 222c 0d0a 2020 225f 6275  _cache",..  "_bu
-000003c0: 696c 6422 2c0d 0a20 2022 6275 636b 2d6f  ild",..  "buck-o
-000003d0: 7574 222c 0d0a 2020 2262 7569 6c64 222c  ut",..  "build",
-000003e0: 0d0a 2020 2264 6973 7422 2c0d 0a20 2022  ..  "dist",..  "
-000003f0: 7461 736b 732e 7079 220d 0a5d 0d0a 0d0a  tasks.py"..]....
-00000400: 5b74 6f6f 6c2e 7275 6666 2e6c 696e 745d  [tool.ruff.lint]
-00000410: 2020 2320 4669 6c65 2072 6566 6572 656e    # File referen
-00000420: 6365 2068 6572 6520 2d20 6874 7470 733a  ce here - https:
-00000430: 2f2f 646f 6373 2e61 7374 7261 6c2e 7368  //docs.astral.sh
-00000440: 2f72 7566 662f 7275 6c65 732f 0d0a 6578  /ruff/rules/..ex
-00000450: 7465 6e64 2d73 656c 6563 7420 3d20 5b22  tend-select = ["
-00000460: 4535 3031 225d 0d0a 6967 6e6f 7265 203d  E501"]..ignore =
-00000470: 205b 2245 3734 3122 2c20 224e 3830 3522   ["E741", "N805"
-00000480: 2c20 2250 5430 3039 222c 2022 5245 5435  , "PT009", "RET5
-00000490: 3033 225d 0d0a 7365 6c65 6374 203d 205b  03"]..select = [
-000004a0: 0d0a 2020 2245 222c 0d0a 2020 2246 222c  ..  "E",..  "F",
-000004b0: 0d0a 2020 2257 222c 0d0a 2020 2249 222c  ..  "W",..  "I",
-000004c0: 0d0a 2020 224e 222c 0d0a 2020 2255 5022  ..  "N",..  "UP"
-000004d0: 2c0d 0a20 2022 5954 5422 2c0d 0a20 2022  ,..  "YTT",..  "
-000004e0: 424c 4522 2c0d 0a20 2022 4222 2c0d 0a20  BLE",..  "B",.. 
-000004f0: 2022 4122 2c0d 0a20 2022 4334 222c 0d0a   "A",..  "C4",..
-00000500: 2020 2244 545a 222c 0d0a 2020 2254 3130    "DTZ",..  "T10
-00000510: 222c 0d0a 2020 2245 4d22 2c0d 0a20 2022  ",..  "EM",..  "
-00000520: 4722 2c0d 0a20 2022 494e 5022 2c0d 0a20  G",..  "INP",.. 
-00000530: 2022 5049 4522 2c0d 0a20 2022 5432 3022   "PIE",..  "T20"
-00000540: 2c0d 0a20 2022 5054 222c 0d0a 2020 2251  ,..  "PT",..  "Q
-00000550: 222c 0d0a 2020 2252 4554 222c 0d0a 2020  ",..  "RET",..  
-00000560: 2254 4944 222c 0d0a 2020 2254 4348 222c  "TID",..  "TCH",
-00000570: 0d0a 2020 2241 5247 222c 0d0a 2020 2250  ..  "ARG",..  "P
-00000580: 5448 220d 0a5d 0d0a 0d0a 5b74 6f6f 6c2e  TH"..]....[tool.
-00000590: 7275 6666 2e6c 696e 742e 7065 722d 6669  ruff.lint.per-fi
-000005a0: 6c65 2d69 676e 6f72 6573 5d0d 0a22 5f5f  le-ignores].."__
-000005b0: 696e 6974 5f5f 2e70 7922 203d 205b 2246  init__.py" = ["F
-000005c0: 3430 3122 5d0d 0a0d 0a0d 0a5b 746f 6f6c  401"]......[tool
-000005d0: 2e6d 7970 795d 0d0a 2320 4d79 5079 2063  .mypy]..# MyPy c
-000005e0: 6f6e 6669 670d 0a23 2046 696c 6520 7265  onfig..# File re
-000005f0: 6665 7265 6e63 6520 6865 7265 202d 2068  ference here - h
-00000600: 7474 703a 2f2f 6d79 7079 2e72 6561 6474  ttp://mypy.readt
-00000610: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
-00000620: 6573 742f 636f 6e66 6967 5f66 696c 652e  est/config_file.
-00000630: 6874 6d6c 2363 6f6e 6669 672d 6669 6c65  html#config-file
-00000640: 0d0a 7079 7468 6f6e 5f76 6572 7369 6f6e  ..python_version
-00000650: 203d 2033 2e38 0d0a 7761 726e 5f72 6564   = 3.8..warn_red
-00000660: 756e 6461 6e74 5f63 6173 7473 203d 2074  undant_casts = t
-00000670: 7275 650d 0a77 6172 6e5f 756e 7573 6564  rue..warn_unused
-00000680: 5f69 676e 6f72 6573 203d 2074 7275 650d  _ignores = true.
-00000690: 0a77 6172 6e5f 7265 7475 726e 5f61 6e79  .warn_return_any
-000006a0: 203d 2074 7275 650d 0a77 6172 6e5f 756e   = true..warn_un
-000006b0: 7573 6564 5f63 6f6e 6669 6773 203d 2074  used_configs = t
-000006c0: 7275 650d 0a73 7472 6963 7420 3d20 7472  rue..strict = tr
-000006d0: 7565 0d0a 6469 7361 6c6c 6f77 5f73 7562  ue..disallow_sub
-000006e0: 636c 6173 7369 6e67 5f61 6e79 203d 2066  classing_any = f
-000006f0: 616c 7365 0d0a 2369 676e 6f72 655f 6d69  alse..#ignore_mi
-00000700: 7373 696e 675f 696d 706f 7274 7320 3d20  ssing_imports = 
-00000710: 7472 7565 0d0a 6578 636c 7564 6520 3d20  true..exclude = 
-00000720: 5b0d 0a20 2022 5c5c 2e6d 7970 795f 6361  [..  "\\.mypy_ca
-00000730: 6368 6522 2c0d 0a20 2022 5c5c 2e76 656e  che",..  "\\.ven
-00000740: 7622 2c0d 0a20 2022 6275 696c 6422 2c0d  v",..  "build",.
-00000750: 0a20 2022 6469 7374 222c 0d0a 2020 226f  .  "dist",..  "o
-00000760: 7574 222c 0d0a 2020 2270 6c61 7967 726f  ut",..  "playgro
-00000770: 756e 6422 2c0d 0a20 2022 7363 7269 7074  und",..  "script
-00000780: 7322 0d0a 5d0d 0a0d 0a5b 5b74 6f6f 6c2e  s"..]....[[tool.
-00000790: 6d79 7079 2e6f 7665 7272 6964 6573 5d5d  mypy.overrides]]
-000007a0: 0d0a 6d6f 6475 6c65 203d 205b 2272 6f62  ..module = ["rob
-000007b0: 6f74 2e2a 222c 2022 726f 626f 7469 6479  ot.*", "robotidy
-000007c0: 2e2a 222c 2022 726f 626f 636f 702e 2a22  .*", "robocop.*"
-000007d0: 5d0d 0a69 676e 6f72 655f 6d69 7373 696e  ]..ignore_missin
-000007e0: 675f 696d 706f 7274 7320 3d20 7472 7565  g_imports = true
+00000220: 6d65 776f 726b 203d 2022 5e36 220d 0a70  mework = "^6"..p
+00000230: 7964 616e 7469 6320 3d20 225e 3122 0d0a  ydantic = "^1"..
+00000240: 0d0a 5b74 6f6f 6c2e 706f 6574 7279 2e67  ..[tool.poetry.g
+00000250: 726f 7570 2e63 6f6e 6669 672e 6465 7065  roup.config.depe
+00000260: 6e64 656e 6369 6573 5d0d 0a50 7959 414d  ndencies]..PyYAM
+00000270: 4c20 3d20 225e 362e 3022 0d0a 7061 7468  L = "^6.0"..path
+00000280: 6c69 6220 3d20 225e 312e 302e 3122 0d0a  lib = "^1.0.1"..
+00000290: 7265 6765 7820 3d20 225e 3230 3233 2e31  regex = "^2023.1
+000002a0: 302e 3322 0d0a 0d0a 5b74 6f6f 6c2e 706f  0.3"....[tool.po
+000002b0: 6574 7279 2e67 726f 7570 2e64 6576 2e64  etry.group.dev.d
+000002c0: 6570 656e 6465 6e63 6965 735d 0d0a 726f  ependencies]..ro
+000002d0: 626f 7466 7261 6d65 776f 726b 203d 2022  botframework = "
+000002e0: 5e36 2e31 220d 0a72 7566 6620 3d20 222a  ^6.1"..ruff = "*
+000002f0: 220d 0a6d 7970 7920 3d20 222a 220d 0a62  "..mypy = "*"..b
+00000300: 6c61 636b 203d 2022 2a22 0d0a 0d0a 5b74  lack = "*"....[t
+00000310: 6f6f 6c2e 7275 6666 5d0d 0a6c 696e 652d  ool.ruff]..line-
+00000320: 6c65 6e67 7468 203d 2031 3230 0d0a 7461  length = 120..ta
+00000330: 7267 6574 2d76 6572 7369 6f6e 203d 2022  rget-version = "
+00000340: 7079 3338 220d 0a65 7863 6c75 6465 203d  py38"..exclude =
+00000350: 205b 0d0a 2020 222e 7673 636f 6465 222c   [..  ".vscode",
+00000360: 0d0a 2020 225c 5c2e 7665 6e76 222c 0d0a  ..  "\\.venv",..
+00000370: 2020 222e 6769 7422 2c0d 0a20 2022 2e6d    ".git",..  ".m
+00000380: 7970 795f 6361 6368 6522 2c0d 0a20 2022  ypy_cache",..  "
+00000390: 2e72 7566 665f 6361 6368 6522 2c0d 0a20  .ruff_cache",.. 
+000003a0: 2022 5f62 7569 6c64 222c 0d0a 2020 2262   "_build",..  "b
+000003b0: 7563 6b2d 6f75 7422 2c0d 0a20 2022 6275  uck-out",..  "bu
+000003c0: 696c 6422 2c0d 0a20 2022 6469 7374 222c  ild",..  "dist",
+000003d0: 0d0a 2020 2274 6173 6b73 2e70 7922 0d0a  ..  "tasks.py"..
+000003e0: 5d0d 0a0d 0a5b 746f 6f6c 2e72 7566 662e  ]....[tool.ruff.
+000003f0: 6c69 6e74 5d20 2023 2046 696c 6520 7265  lint]  # File re
+00000400: 6665 7265 6e63 6520 6865 7265 202d 2068  ference here - h
+00000410: 7474 7073 3a2f 2f64 6f63 732e 6173 7472  ttps://docs.astr
+00000420: 616c 2e73 682f 7275 6666 2f72 756c 6573  al.sh/ruff/rules
+00000430: 2f0d 0a65 7874 656e 642d 7365 6c65 6374  /..extend-select
+00000440: 203d 205b 2245 3530 3122 5d0d 0a69 676e   = ["E501"]..ign
+00000450: 6f72 6520 3d20 5b22 4537 3431 222c 2022  ore = ["E741", "
+00000460: 4e38 3035 222c 2022 5054 3030 3922 2c20  N805", "PT009", 
+00000470: 2252 4554 3530 3322 5d0d 0a73 656c 6563  "RET503"]..selec
+00000480: 7420 3d20 5b0d 0a20 2022 4522 2c0d 0a20  t = [..  "E",.. 
+00000490: 2022 4622 2c0d 0a20 2022 5722 2c0d 0a20   "F",..  "W",.. 
+000004a0: 2022 4922 2c0d 0a20 2022 4e22 2c0d 0a20   "I",..  "N",.. 
+000004b0: 2022 5550 222c 0d0a 2020 2259 5454 222c   "UP",..  "YTT",
+000004c0: 0d0a 2020 2242 4c45 222c 0d0a 2020 2242  ..  "BLE",..  "B
+000004d0: 222c 0d0a 2020 2241 222c 0d0a 2020 2243  ",..  "A",..  "C
+000004e0: 3422 2c0d 0a20 2022 4454 5a22 2c0d 0a20  4",..  "DTZ",.. 
+000004f0: 2022 5431 3022 2c0d 0a20 2022 454d 222c   "T10",..  "EM",
+00000500: 0d0a 2020 2247 222c 0d0a 2020 2249 4e50  ..  "G",..  "INP
+00000510: 222c 0d0a 2020 2250 4945 222c 0d0a 2020  ",..  "PIE",..  
+00000520: 2254 3230 222c 0d0a 2020 2250 5422 2c0d  "T20",..  "PT",.
+00000530: 0a20 2022 5122 2c0d 0a20 2022 5245 5422  .  "Q",..  "RET"
+00000540: 2c0d 0a20 2022 5449 4422 2c0d 0a20 2022  ,..  "TID",..  "
+00000550: 5443 4822 2c0d 0a20 2022 4152 4722 2c0d  TCH",..  "ARG",.
+00000560: 0a20 2022 5054 4822 0d0a 5d0d 0a0d 0a5b  .  "PTH"..]....[
+00000570: 746f 6f6c 2e72 7566 662e 6c69 6e74 2e70  tool.ruff.lint.p
+00000580: 6572 2d66 696c 652d 6967 6e6f 7265 735d  er-file-ignores]
+00000590: 0d0a 225f 5f69 6e69 745f 5f2e 7079 2220  .."__init__.py" 
+000005a0: 3d20 5b22 4634 3031 225d 0d0a 0d0a 0d0a  = ["F401"]......
+000005b0: 5b74 6f6f 6c2e 6d79 7079 5d0d 0a23 204d  [tool.mypy]..# M
+000005c0: 7950 7920 636f 6e66 6967 0d0a 2320 4669  yPy config..# Fi
+000005d0: 6c65 2072 6566 6572 656e 6365 2068 6572  le reference her
+000005e0: 6520 2d20 6874 7470 3a2f 2f6d 7970 792e  e - http://mypy.
+000005f0: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
+00000600: 6e2f 6c61 7465 7374 2f63 6f6e 6669 675f  n/latest/config_
+00000610: 6669 6c65 2e68 746d 6c23 636f 6e66 6967  file.html#config
+00000620: 2d66 696c 650d 0a70 7974 686f 6e5f 7665  -file..python_ve
+00000630: 7273 696f 6e20 3d20 332e 380d 0a77 6172  rsion = 3.8..war
+00000640: 6e5f 7265 6475 6e64 616e 745f 6361 7374  n_redundant_cast
+00000650: 7320 3d20 7472 7565 0d0a 7761 726e 5f75  s = true..warn_u
+00000660: 6e75 7365 645f 6967 6e6f 7265 7320 3d20  nused_ignores = 
+00000670: 7472 7565 0d0a 7761 726e 5f72 6574 7572  true..warn_retur
+00000680: 6e5f 616e 7920 3d20 7472 7565 0d0a 7761  n_any = true..wa
+00000690: 726e 5f75 6e75 7365 645f 636f 6e66 6967  rn_unused_config
+000006a0: 7320 3d20 7472 7565 0d0a 7374 7269 6374  s = true..strict
+000006b0: 203d 2074 7275 650d 0a64 6973 616c 6c6f   = true..disallo
+000006c0: 775f 7375 6263 6c61 7373 696e 675f 616e  w_subclassing_an
+000006d0: 7920 3d20 6661 6c73 650d 0a23 6967 6e6f  y = false..#igno
+000006e0: 7265 5f6d 6973 7369 6e67 5f69 6d70 6f72  re_missing_impor
+000006f0: 7473 203d 2074 7275 650d 0a65 7863 6c75  ts = true..exclu
+00000700: 6465 203d 205b 0d0a 2020 225c 5c2e 6d79  de = [..  "\\.my
+00000710: 7079 5f63 6163 6865 222c 0d0a 2020 225c  py_cache",..  "\
+00000720: 5c2e 7665 6e76 222c 0d0a 2020 2262 7569  \.venv",..  "bui
+00000730: 6c64 222c 0d0a 2020 2264 6973 7422 2c0d  ld",..  "dist",.
+00000740: 0a20 2022 6f75 7422 2c0d 0a20 2022 706c  .  "out",..  "pl
+00000750: 6179 6772 6f75 6e64 222c 0d0a 2020 2273  ayground",..  "s
+00000760: 6372 6970 7473 220d 0a5d 0d0a 0d0a 5b5b  cripts"..]....[[
+00000770: 746f 6f6c 2e6d 7970 792e 6f76 6572 7269  tool.mypy.overri
+00000780: 6465 735d 5d0d 0a6d 6f64 756c 6520 3d20  des]]..module = 
+00000790: 5b22 726f 626f 742e 2a22 2c20 2272 6f62  ["robot.*", "rob
+000007a0: 6f74 6964 792e 2a22 2c20 2272 6f62 6f63  otidy.*", "roboc
+000007b0: 6f70 2e2a 225d 0d0a 6967 6e6f 7265 5f6d  op.*"]..ignore_m
+000007c0: 6973 7369 6e67 5f69 6d70 6f72 7473 203d  issing_imports =
+000007d0: 2074 7275 65                              true
```

### Comparing `robotframework_reportmodifier-0.2.0/README.md` & `robotframework_reportmodifier-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `robotframework_reportmodifier-0.2.0/src/reportmodifier/_file_tools.py` & `robotframework_reportmodifier-0.2.1/src/reportmodifier/_file_tools.py`

 * *Files identical despite different names*

### Comparing `robotframework_reportmodifier-0.2.0/src/reportmodifier/_report_configuration.py` & `robotframework_reportmodifier-0.2.1/src/reportmodifier/_report_configuration.py`

 * *Files identical despite different names*

### Comparing `robotframework_reportmodifier-0.2.0/src/reportmodifier/ReportModifier.py` & `robotframework_reportmodifier-0.2.1/src/reportmodifier/ReportModifier.py`

 * *Files identical despite different names*

### Comparing `robotframework_reportmodifier-0.2.0/src/reportmodifier/ReportModifierVisitor.py` & `robotframework_reportmodifier-0.2.1/src/reportmodifier/ReportModifierVisitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,19 +53,20 @@
     def start_test(self, test: TestCase):
         self._relevant_messages = defaultdict(list)
         self._relevant_keyword_calls = []
         self.report_configuration = ReportConfiguration(None)
         for tag in test.tags:
             if tag.startswith(("fb_report:", "report:")):
                 report_configuration = tag.split("report:")[-1].strip()
+                report_configuration = report_configuration.lower().replace(".yaml", "")
                 test_path = Path(test.source)
                 test_dir = Path(*test_path.parts[0 : test_path.parts.index("tests") + 1])
                 configuration_path = get_files_in_folder(
                     top_level_dir=test_dir,
-                    condition_callback=lambda p: Path(p).stem.lower() == report_configuration.split(".yaml")[0].lower()  # noqa: B023
+                    condition_callback=lambda p: Path(p).stem.lower() == report_configuration  # noqa: B023
                     and Path(p).suffix == ".yaml",
                     recursive=True,
                 )
                 if not configuration_path:
                     logger.error(
                         f'Could not find custon log configuration "{report_configuration}" of test  {test.name}',
                     )
```

### Comparing `robotframework_reportmodifier-0.2.0/src/ReportModifierListener/ReportModifierListener.py` & `robotframework_reportmodifier-0.2.1/src/ReportModifierListener/ReportModifierListener.py`

 * *Files identical despite different names*

### Comparing `robotframework_reportmodifier-0.2.0/PKG-INFO` & `robotframework_reportmodifier-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: robotframework-reportmodifier
-Version: 0.2.0
+Version: 0.2.1
 Summary: Filter report content.
 Home-page: https://github.com/MarketSquare/robotframework-reportmodifier
 Author: Matthias Gunther
 Author-email: matthiasgunther@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: pydantic (>=1.10.4,<2.0.0)
-Requires-Dist: robotframework (>=6.1,<7.0)
-Requires-Dist: rule-engine (>=4,<5)
+Requires-Dist: pydantic (>=1,<2)
+Requires-Dist: robotframework (>=6,<7)
 Description-Content-Type: text/markdown
 
 ## Introduction 
 The high complexity of tests and the amount of information that can be logged makes the final report very confusing and unreadable for colleagues who aren't testers with Robot Framework knowledge but need to know the rough test flow and result. To provide a better overview of the test content, the library can filter the content by message content, keyword names or even keyword paths.
 
 ## Configuration assignment
```

