# Comparing `tmp/tkchart-2.0.2.tar.gz` & `tmp/tkchart-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkchart-2.0.2.tar", last modified: Fri Mar 22 05:52:05 2024, max compression
+gzip compressed data, was "tkchart-2.0.3.tar", last modified: Mon Apr  1 23:47:05 2024, max compression
```

## Comparing `tkchart-2.0.2.tar` & `tkchart-2.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-03-22 05:52:05.626560 tkchart-2.0.2/
--rw-rw-rw-   0        0        0     1091 2024-02-14 05:02:34.000000 tkchart-2.0.2/LICENSE
--rw-rw-rw-   0        0        0     3486 2024-03-22 05:52:05.626560 tkchart-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1458 2024-03-22 05:46:07.000000 tkchart-2.0.2/README.md
--rw-rw-rw-   0        0        0      857 2024-03-22 05:42:05.000000 tkchart-2.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-22 05:52:05.626560 tkchart-2.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-22 05:52:05.563613 tkchart-2.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-03-22 05:52:05.610946 tkchart-2.0.2/src/tkchart/
--rw-rw-rw-   0        0        0     1804 2024-03-11 17:44:06.000000 tkchart-2.0.2/src/tkchart/FontStyle.py
--rw-rw-rw-   0        0        0     7654 2024-03-22 03:49:52.000000 tkchart-2.0.2/src/tkchart/Line.py
--rw-rw-rw-   0        0        0    86200 2024-03-22 05:26:13.000000 tkchart-2.0.2/src/tkchart/LineChart.py
--rw-rw-rw-   0        0        0     1816 2024-03-22 05:38:59.000000 tkchart-2.0.2/src/tkchart/Utils.py
--rw-rw-rw-   0        0        0     9827 2024-03-22 05:39:49.000000 tkchart-2.0.2/src/tkchart/Validate.py
--rw-rw-rw-   0        0        0      255 2024-03-22 05:41:48.000000 tkchart-2.0.2/src/tkchart/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-22 05:52:05.626560 tkchart-2.0.2/src/tkchart.egg-info/
--rw-rw-rw-   0        0        0     3486 2024-03-22 05:52:05.000000 tkchart-2.0.2/src/tkchart.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2024-03-22 05:52:05.000000 tkchart-2.0.2/src/tkchart.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-22 05:52:05.000000 tkchart-2.0.2/src/tkchart.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-03-22 05:52:05.000000 tkchart-2.0.2/src/tkchart.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 23:47:05.793302 tkchart-2.0.3/
+-rw-rw-rw-   0        0        0     1091 2024-02-14 05:02:34.000000 tkchart-2.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3450 2024-04-01 23:47:05.792318 tkchart-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1420 2024-04-01 23:40:03.000000 tkchart-2.0.3/README.md
+-rw-rw-rw-   0        0        0      857 2024-04-01 23:45:12.000000 tkchart-2.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-01 23:47:05.793302 tkchart-2.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-01 23:47:05.753206 tkchart-2.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-01 23:47:05.779063 tkchart-2.0.3/src/tkchart/
+-rw-rw-rw-   0        0        0     1804 2024-03-11 17:44:06.000000 tkchart-2.0.3/src/tkchart/FontStyle.py
+-rw-rw-rw-   0        0        0     8808 2024-04-01 05:24:54.000000 tkchart-2.0.3/src/tkchart/Line.py
+-rw-rw-rw-   0        0        0    92978 2024-04-01 23:43:10.000000 tkchart-2.0.3/src/tkchart/LineChart.py
+-rw-rw-rw-   0        0        0     1816 2024-03-22 05:38:59.000000 tkchart-2.0.3/src/tkchart/Utils.py
+-rw-rw-rw-   0        0        0    10049 2024-04-01 01:19:52.000000 tkchart-2.0.3/src/tkchart/Validate.py
+-rw-rw-rw-   0        0        0      277 2024-04-01 23:24:43.000000 tkchart-2.0.3/src/tkchart/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 23:47:05.792318 tkchart-2.0.3/src/tkchart.egg-info/
+-rw-rw-rw-   0        0        0     3450 2024-04-01 23:47:05.000000 tkchart-2.0.3/src/tkchart.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2024-04-01 23:47:05.000000 tkchart-2.0.3/src/tkchart.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 23:47:05.000000 tkchart-2.0.3/src/tkchart.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-01 23:47:05.000000 tkchart-2.0.3/src/tkchart.egg-info/top_level.txt
```

### Comparing `tkchart-2.0.2/LICENSE` & `tkchart-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tkchart-2.0.2/PKG-INFO` & `tkchart-2.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2074 6b63  : 2.1..Name: tkc
 00000020: 6861 7274 0d0a 5665 7273 696f 6e3a 2032  hart..Version: 2
-00000030: 2e30 2e32 0d0a 5375 6d6d 6172 793a 2074  .0.2..Summary: t
+00000030: 2e30 2e33 0d0a 5375 6d6d 6172 793a 2074  .0.3..Summary: t
 00000040: 6b63 6861 7274 2069 7320 6120 5079 7468  kchart is a Pyth
 00000050: 6f6e 206c 6962 7261 7279 2066 6f72 2063  on library for c
 00000060: 7265 6174 696e 6720 6c69 7665 2075 7064  reating live upd
 00000070: 6174 696e 6720 6c69 6e65 2063 6861 7274  ating line chart
 00000080: 7320 696e 2054 6b69 6e74 6572 2e0d 0a41  s in Tkinter...A
 00000090: 7574 686f 723a 2054 6869 7361 6c2d 440d  uthor: Thisal-D.
 000000a0: 0a4c 6963 656e 7365 3a20 436f 7079 7269  .License: Copyri
@@ -151,68 +151,66 @@
 00000960: 7079 2e74 6563 682f 7072 6f6a 6563 742f  py.tech/project/
 00000970: 746b 6368 6172 7429 205b 215b 446f 776e  tkchart) [![Down
 00000980: 6c6f 6164 735d 2868 7474 7073 3a2f 2f73  loads](https://s
 00000990: 7461 7469 632e 7065 7079 2e74 6563 682f  tatic.pepy.tech/
 000009a0: 6261 6467 652f 746b 6368 6172 742f 7765  badge/tkchart/we
 000009b0: 656b 295d 2868 7474 7073 3a2f 2f70 6570  ek)](https://pep
 000009c0: 792e 7465 6368 2f70 726f 6a65 6374 2f74  y.tech/project/t
-000009d0: 6b63 6861 7274 290d 0a0d 0a3c 696d 6720  kchart)....<img 
-000009e0: 7372 633d 2268 7474 7073 3a2f 2f64 7269  src="https://dri
-000009f0: 7665 2e67 6f6f 676c 652e 636f 6d2f 7468  ve.google.com/th
-00000a00: 756d 626e 6169 6c3f 6964 3d31 6a4f 6c74  umbnail?id=1jOlt
-00000a10: 5435 7142 764c 6d4b 4164 5355 367a 6239  T5qBvLmKAdSU6zb9
-00000a20: 776a 6833 4759 6136 6a52 7644 2673 7a3d  wjh3GYa6jRvD&sz=
-00000a30: 7731 3830 223e 0d0a 0d0a 3c2f 6469 763e  w180">....</div>
-00000a40: 0d0a 0d0a 2323 2320 3c6c 693e 746b 6368  ....### <li>tkch
-00000a50: 6172 7420 6973 2061 2050 7974 686f 6e20  art is a Python 
-00000a60: 6c69 6272 6172 7920 666f 7220 6372 6561  library for crea
-00000a70: 7469 6e67 206c 6976 6520 7570 6461 7469  ting live updati
-00000a80: 6e67 206c 696e 6520 6368 6172 7473 2069  ng line charts i
-00000a90: 6e20 546b 696e 7465 722e 3c2f 6c69 3e0d  n Tkinter.</li>.
-00000aa0: 0a0d 0a23 2320 4665 6174 7572 6573 0d0a  ...## Features..
-00000ab0: 0d0a 2d20 2a2a 4c69 7665 2055 7064 6174  ..- **Live Updat
-00000ac0: 652a 2a3a 2044 6973 706c 6179 206c 6976  e**: Display liv
-00000ad0: 6520 6461 7461 2077 6974 6820 6c69 6e65  e data with line
-00000ae0: 2063 6861 7274 732e 0d0a 2d20 2a2a 4d75   charts...- **Mu
-00000af0: 6c74 6970 6c65 204c 696e 6573 2a2a 3a20  ltiple Lines**: 
-00000b00: 5375 7070 6f72 7420 666f 7220 706c 6f74  Support for plot
-00000b10: 7469 6e67 206d 756c 7469 706c 6520 6c69  ting multiple li
-00000b20: 6e65 7320 6f6e 2074 6865 2073 616d 6520  nes on the same 
-00000b30: 6368 6172 7420 666f 7220 6561 7379 2063  chart for easy c
-00000b40: 6f6d 7061 7269 736f 6e2e 0d0a 2d20 2a2a  omparison...- **
-00000b50: 436f 6c6f 7220 4375 7374 6f6d 697a 6174  Color Customizat
-00000b60: 696f 6e2a 2a3a 2043 7573 746f 6d69 7a65  ion**: Customize
-00000b70: 2063 6f6c 6f72 7320 746f 206d 6174 6368   colors to match
-00000b80: 2079 6f75 7220 6170 706c 6963 6174 696f   your applicatio
-00000b90: 6e27 7320 6465 7369 676e 206f 7220 6461  n's design or da
-00000ba0: 7461 2072 6570 7265 7365 6e74 6174 696f  ta representatio
-00000bb0: 6e2e 0d0a 2d20 2a2a 466f 6e74 2043 7573  n...- **Font Cus
-00000bc0: 746f 6d69 7a61 7469 6f6e 2a2a 3a20 4164  tomization**: Ad
-00000bd0: 6a75 7374 2066 6f6e 7473 2066 6f72 2074  just fonts for t
-00000be0: 6578 7420 656c 656d 656e 7473 2074 6f20  ext elements to 
-00000bf0: 656e 6861 6e63 6520 7265 6164 6162 696c  enhance readabil
-00000c00: 6974 792e 0d0a 2d20 2a2a 4469 6d65 6e73  ity...- **Dimens
-00000c10: 696f 6e20 4375 7374 6f6d 697a 6174 696f  ion Customizatio
-00000c20: 6e2a 2a3a 2043 7573 746f 6d69 7a65 2063  n**: Customize c
-00000c30: 6861 7274 2064 696d 656e 7369 6f6e 7320  hart dimensions 
-00000c40: 746f 2066 6974 2076 6172 696f 7573 2064  to fit various d
-00000c50: 6973 706c 6179 2073 697a 6573 2061 6e64  isplay sizes and
-00000c60: 206c 6179 6f75 7473 2e0d 0a0d 0a23 2320   layouts.....## 
-00000c70: 496d 706f 7274 696e 6720 2620 496e 7374  Importing & Inst
-00000c80: 616c 6c61 7469 6f6e 0d0a 2a20 496e 7374  allation..* Inst
-00000c90: 616c 6c61 7469 6f6e 0d0a 2020 2020 6060  allation..    ``
-00000ca0: 600d 0a20 2020 2070 6970 2069 6e73 7461  `..    pip insta
-00000cb0: 6c6c 2074 6b63 6861 7274 0d0a 2020 2020  ll tkchart..    
-00000cc0: 6060 600d 0a0d 0a2a 2049 6d70 6f72 7469  ```....* Importi
-00000cd0: 6e67 0d0a 2020 2020 2060 6060 0d0a 2020  ng..     ```..  
-00000ce0: 2020 696d 706f 7274 2074 6b63 6861 7274    import tkchart
-00000cf0: 0d0a 2020 2020 6060 600d 0a0d 0a23 204c  ..    ```....# L
-00000d00: 696e 6b73 0d0a 0d0a 2d20 2a2a 5669 7369  inks....- **Visi
-00000d10: 7420 4769 7448 7562 2066 6f72 204d 6f72  t GitHub for Mor
-00000d20: 6520 4465 7461 696c 732e 2e2e 2e2e 2a2a  e Details.....**
-00000d30: 0d0a 2d20 2323 202a 2a47 6974 4875 622e  ..- ## **GitHub.
-00000d40: 636f 6d2a 2a20 2020 3a20 203c 6120 6872  com**   :  <a hr
-00000d50: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+000009d0: 6b63 6861 7274 290d 0a0d 0a0d 0a3c 696d  kchart)......<im
+000009e0: 6720 7372 633d 2268 7474 7073 3a2f 2f64  g src="https://d
+000009f0: 7269 7665 2e67 6f6f 676c 652e 636f 6d2f  rive.google.com/
+00000a00: 7468 756d 626e 6169 6c3f 6964 3d31 6348  thumbnail?id=1cH
+00000a10: 7273 4649 4c48 4a37 6132 6267 4d58 766b  rsFILHJ7a2bgMXvk
+00000a20: 2d50 576c 6e4c 5a78 3176 436e 5652 2673  -PWlnLZx1vCnVR&s
+00000a30: 7a3d 7731 3830 223e 0d0a 0d0a 3c2f 6469  z=w180">....</di
+00000a40: 763e 0d0a 0d0a 2323 2320 3c6c 693e 746b  v>....### <li>tk
+00000a50: 6368 6172 7420 6973 2061 2050 7974 686f  chart is a Pytho
+00000a60: 6e20 6c69 6272 6172 7920 666f 7220 6372  n library for cr
+00000a70: 6561 7469 6e67 206c 6976 6520 7570 6461  eating live upda
+00000a80: 7469 6e67 206c 696e 6520 6368 6172 7473  ting line charts
+00000a90: 2069 6e20 546b 696e 7465 722e 3c2f 6c69   in Tkinter.</li
+00000aa0: 3e0d 0a0d 0a23 2320 4665 6174 7572 6573  >....## Features
+00000ab0: 0d0a 0d0a 2d20 2a2a 4c69 7665 2055 7064  ....- **Live Upd
+00000ac0: 6174 652a 2a3a 2044 6973 706c 6179 206c  ate**: Display l
+00000ad0: 6976 6520 6461 7461 2077 6974 6820 6c69  ive data with li
+00000ae0: 6e65 2063 6861 7274 732e 0d0a 2d20 2a2a  ne charts...- **
+00000af0: 4d75 6c74 6970 6c65 204c 696e 6573 2a2a  Multiple Lines**
+00000b00: 3a20 5375 7070 6f72 7420 666f 7220 706c  : Support for pl
+00000b10: 6f74 7469 6e67 206d 756c 7469 706c 6520  otting multiple 
+00000b20: 6c69 6e65 7320 6f6e 2074 6865 2073 616d  lines on the sam
+00000b30: 6520 6368 6172 7420 666f 7220 6561 7379  e chart for easy
+00000b40: 2063 6f6d 7061 7269 736f 6e2e 0d0a 2d20   comparison...- 
+00000b50: 2a2a 436f 6c6f 7220 4375 7374 6f6d 697a  **Color Customiz
+00000b60: 6174 696f 6e2a 2a3a 2043 7573 746f 6d69  ation**: Customi
+00000b70: 7a65 2063 6f6c 6f72 7320 746f 206d 6174  ze colors to mat
+00000b80: 6368 2079 6f75 7220 6170 706c 6963 6174  ch your applicat
+00000b90: 696f 6e27 7320 6465 7369 676e 206f 7220  ion's design or 
+00000ba0: 6461 7461 2072 6570 7265 7365 6e74 6174  data representat
+00000bb0: 696f 6e2e 0d0a 2d20 2a2a 466f 6e74 2043  ion...- **Font C
+00000bc0: 7573 746f 6d69 7a61 7469 6f6e 2a2a 3a20  ustomization**: 
+00000bd0: 4164 6a75 7374 2066 6f6e 7473 2066 6f72  Adjust fonts for
+00000be0: 2074 6578 7420 656c 656d 656e 7473 2074   text elements t
+00000bf0: 6f20 656e 6861 6e63 6520 7265 6164 6162  o enhance readab
+00000c00: 696c 6974 792e 0d0a 2d20 2a2a 4469 6d65  ility...- **Dime
+00000c10: 6e73 696f 6e20 4375 7374 6f6d 697a 6174  nsion Customizat
+00000c20: 696f 6e2a 2a3a 2043 7573 746f 6d69 7a65  ion**: Customize
+00000c30: 2063 6861 7274 2064 696d 656e 7369 6f6e   chart dimension
+00000c40: 7320 746f 2066 6974 2076 6172 696f 7573  s to fit various
+00000c50: 2064 6973 706c 6179 2073 697a 6573 2061   display sizes a
+00000c60: 6e64 206c 6179 6f75 7473 2e0d 0a0d 0a23  nd layouts.....#
+00000c70: 2320 496d 706f 7274 696e 6720 2620 496e  # Importing & In
+00000c80: 7374 616c 6c61 7469 6f6e 0d0a 2a20 496e  stallation..* In
+00000c90: 7374 616c 6c61 7469 6f6e 0d0a 2020 2020  stallation..    
+00000ca0: 6060 600d 0a20 2020 2070 6970 2069 6e73  ```..    pip ins
+00000cb0: 7461 6c6c 2074 6b63 6861 7274 0d0a 2020  tall tkchart..  
+00000cc0: 2020 6060 600d 0a0d 0a2a 2049 6d70 6f72    ```....* Impor
+00000cd0: 7469 6e67 0d0a 2020 2020 2060 6060 0d0a  ting..     ```..
+00000ce0: 2020 2020 696d 706f 7274 2074 6b63 6861      import tkcha
+00000cf0: 7274 0d0a 2020 2020 6060 600d 0a0d 0a23  rt..    ```....#
+00000d00: 204c 696e 6b73 0d0a 0d0a 2a2a 5669 7369   Links....**Visi
+00000d10: 7420 4769 7448 7562 2066 6f72 2044 6f63  t GitHub for Doc
+00000d20: 756d 656e 7461 7469 6f6e 3a2a 2a0d 0a0d  umentation:**...
+00000d30: 0a2d 202a 2a47 6974 4875 6220 5265 706f  .- **GitHub Repo
+00000d40: 7369 746f 7279 3a2a 2a20 5b74 6b63 6861  sitory:** [tkcha
+00000d50: 7274 5d28 6874 7470 733a 2f2f 6769 7468  rt](https://gith
 00000d60: 7562 2e63 6f6d 2f54 6869 7361 6c2d 442f  ub.com/Thisal-D/
-00000d70: 746b 6368 6172 7422 2074 6172 6765 743d  tkchart" target=
-00000d80: 225f 626c 616e 6b22 203e 3c69 3e74 6b63  "_blank" ><i>tkc
-00000d90: 6861 7274 3c2f 693e 3c2f 613e 0d0a       hart</i></a>..
+00000d70: 746b 6368 6172 7429 0d0a                 tkchart)..
```

### Comparing `tkchart-2.0.2/README.md` & `tkchart-2.0.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -26,67 +26,64 @@
 00000190: 2f70 6570 792e 7465 6368 2f70 726f 6a65  /pepy.tech/proje
 000001a0: 6374 2f74 6b63 6861 7274 2920 5b21 5b44  ct/tkchart) [![D
 000001b0: 6f77 6e6c 6f61 6473 5d28 6874 7470 733a  ownloads](https:
 000001c0: 2f2f 7374 6174 6963 2e70 6570 792e 7465  //static.pepy.te
 000001d0: 6368 2f62 6164 6765 2f74 6b63 6861 7274  ch/badge/tkchart
 000001e0: 2f77 6565 6b29 5d28 6874 7470 733a 2f2f  /week)](https://
 000001f0: 7065 7079 2e74 6563 682f 7072 6f6a 6563  pepy.tech/projec
-00000200: 742f 746b 6368 6172 7429 0a0a 3c69 6d67  t/tkchart)..<img
-00000210: 2073 7263 3d22 6874 7470 733a 2f2f 6472   src="https://dr
-00000220: 6976 652e 676f 6f67 6c65 2e63 6f6d 2f74  ive.google.com/t
-00000230: 6875 6d62 6e61 696c 3f69 643d 316a 4f6c  humbnail?id=1jOl
-00000240: 7454 3571 4276 4c6d 4b41 6453 5536 7a62  tT5qBvLmKAdSU6zb
-00000250: 3977 6a68 3347 5961 366a 5276 4426 737a  9wjh3GYa6jRvD&sz
-00000260: 3d77 3138 3022 3e0a 0a3c 2f64 6976 3e0a  =w180">..</div>.
-00000270: 0a23 2323 203c 6c69 3e74 6b63 6861 7274  .### <li>tkchart
-00000280: 2069 7320 6120 5079 7468 6f6e 206c 6962   is a Python lib
-00000290: 7261 7279 2066 6f72 2063 7265 6174 696e  rary for creatin
-000002a0: 6720 6c69 7665 2075 7064 6174 696e 6720  g live updating 
-000002b0: 6c69 6e65 2063 6861 7274 7320 696e 2054  line charts in T
-000002c0: 6b69 6e74 6572 2e3c 2f6c 693e 0a0a 2323  kinter.</li>..##
-000002d0: 2046 6561 7475 7265 730a 0a2d 202a 2a4c   Features..- **L
-000002e0: 6976 6520 5570 6461 7465 2a2a 3a20 4469  ive Update**: Di
-000002f0: 7370 6c61 7920 6c69 7665 2064 6174 6120  splay live data 
-00000300: 7769 7468 206c 696e 6520 6368 6172 7473  with line charts
-00000310: 2e0a 2d20 2a2a 4d75 6c74 6970 6c65 204c  ..- **Multiple L
-00000320: 696e 6573 2a2a 3a20 5375 7070 6f72 7420  ines**: Support 
-00000330: 666f 7220 706c 6f74 7469 6e67 206d 756c  for plotting mul
-00000340: 7469 706c 6520 6c69 6e65 7320 6f6e 2074  tiple lines on t
-00000350: 6865 2073 616d 6520 6368 6172 7420 666f  he same chart fo
-00000360: 7220 6561 7379 2063 6f6d 7061 7269 736f  r easy compariso
-00000370: 6e2e 0a2d 202a 2a43 6f6c 6f72 2043 7573  n..- **Color Cus
-00000380: 746f 6d69 7a61 7469 6f6e 2a2a 3a20 4375  tomization**: Cu
-00000390: 7374 6f6d 697a 6520 636f 6c6f 7273 2074  stomize colors t
-000003a0: 6f20 6d61 7463 6820 796f 7572 2061 7070  o match your app
-000003b0: 6c69 6361 7469 6f6e 2773 2064 6573 6967  lication's desig
-000003c0: 6e20 6f72 2064 6174 6120 7265 7072 6573  n or data repres
-000003d0: 656e 7461 7469 6f6e 2e0a 2d20 2a2a 466f  entation..- **Fo
-000003e0: 6e74 2043 7573 746f 6d69 7a61 7469 6f6e  nt Customization
-000003f0: 2a2a 3a20 4164 6a75 7374 2066 6f6e 7473  **: Adjust fonts
-00000400: 2066 6f72 2074 6578 7420 656c 656d 656e   for text elemen
-00000410: 7473 2074 6f20 656e 6861 6e63 6520 7265  ts to enhance re
-00000420: 6164 6162 696c 6974 792e 0a2d 202a 2a44  adability..- **D
-00000430: 696d 656e 7369 6f6e 2043 7573 746f 6d69  imension Customi
-00000440: 7a61 7469 6f6e 2a2a 3a20 4375 7374 6f6d  zation**: Custom
-00000450: 697a 6520 6368 6172 7420 6469 6d65 6e73  ize chart dimens
-00000460: 696f 6e73 2074 6f20 6669 7420 7661 7269  ions to fit vari
-00000470: 6f75 7320 6469 7370 6c61 7920 7369 7a65  ous display size
-00000480: 7320 616e 6420 6c61 796f 7574 732e 0a0a  s and layouts...
-00000490: 2323 2049 6d70 6f72 7469 6e67 2026 2049  ## Importing & I
-000004a0: 6e73 7461 6c6c 6174 696f 6e0a 2a20 496e  nstallation.* In
-000004b0: 7374 616c 6c61 7469 6f6e 0a20 2020 2060  stallation.    `
-000004c0: 6060 0a20 2020 2070 6970 2069 6e73 7461  ``.    pip insta
-000004d0: 6c6c 2074 6b63 6861 7274 0a20 2020 2060  ll tkchart.    `
-000004e0: 6060 0a0a 2a20 496d 706f 7274 696e 670a  ``..* Importing.
-000004f0: 2020 2020 2060 6060 0a20 2020 2069 6d70       ```.    imp
-00000500: 6f72 7420 746b 6368 6172 740a 2020 2020  ort tkchart.    
-00000510: 6060 600a 0a23 204c 696e 6b73 0a0a 2d20  ```..# Links..- 
-00000520: 2a2a 5669 7369 7420 4769 7448 7562 2066  **Visit GitHub f
-00000530: 6f72 204d 6f72 6520 4465 7461 696c 732e  or More Details.
-00000540: 2e2e 2e2e 2a2a 0a2d 2023 2320 2a2a 4769  ....**.- ## **Gi
-00000550: 7448 7562 2e63 6f6d 2a2a 2020 203a 2020  tHub.com**   :  
-00000560: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00000570: 2f67 6974 6875 622e 636f 6d2f 5468 6973  /github.com/This
-00000580: 616c 2d44 2f74 6b63 6861 7274 2220 7461  al-D/tkchart" ta
-00000590: 7267 6574 3d22 5f62 6c61 6e6b 2220 3e3c  rget="_blank" ><
-000005a0: 693e 746b 6368 6172 743c 2f69 3e3c 2f61  i>tkchart</i></a
-000005b0: 3e0a                                     >.
+00000200: 742f 746b 6368 6172 7429 0a0a 0a3c 696d  t/tkchart)...<im
+00000210: 6720 7372 633d 2268 7474 7073 3a2f 2f64  g src="https://d
+00000220: 7269 7665 2e67 6f6f 676c 652e 636f 6d2f  rive.google.com/
+00000230: 7468 756d 626e 6169 6c3f 6964 3d31 6348  thumbnail?id=1cH
+00000240: 7273 4649 4c48 4a37 6132 6267 4d58 766b  rsFILHJ7a2bgMXvk
+00000250: 2d50 576c 6e4c 5a78 3176 436e 5652 2673  -PWlnLZx1vCnVR&s
+00000260: 7a3d 7731 3830 223e 0a0a 3c2f 6469 763e  z=w180">..</div>
+00000270: 0a0a 2323 2320 3c6c 693e 746b 6368 6172  ..### <li>tkchar
+00000280: 7420 6973 2061 2050 7974 686f 6e20 6c69  t is a Python li
+00000290: 6272 6172 7920 666f 7220 6372 6561 7469  brary for creati
+000002a0: 6e67 206c 6976 6520 7570 6461 7469 6e67  ng live updating
+000002b0: 206c 696e 6520 6368 6172 7473 2069 6e20   line charts in 
+000002c0: 546b 696e 7465 722e 3c2f 6c69 3e0a 0a23  Tkinter.</li>..#
+000002d0: 2320 4665 6174 7572 6573 0a0a 2d20 2a2a  # Features..- **
+000002e0: 4c69 7665 2055 7064 6174 652a 2a3a 2044  Live Update**: D
+000002f0: 6973 706c 6179 206c 6976 6520 6461 7461  isplay live data
+00000300: 2077 6974 6820 6c69 6e65 2063 6861 7274   with line chart
+00000310: 732e 0a2d 202a 2a4d 756c 7469 706c 6520  s..- **Multiple 
+00000320: 4c69 6e65 732a 2a3a 2053 7570 706f 7274  Lines**: Support
+00000330: 2066 6f72 2070 6c6f 7474 696e 6720 6d75   for plotting mu
+00000340: 6c74 6970 6c65 206c 696e 6573 206f 6e20  ltiple lines on 
+00000350: 7468 6520 7361 6d65 2063 6861 7274 2066  the same chart f
+00000360: 6f72 2065 6173 7920 636f 6d70 6172 6973  or easy comparis
+00000370: 6f6e 2e0a 2d20 2a2a 436f 6c6f 7220 4375  on..- **Color Cu
+00000380: 7374 6f6d 697a 6174 696f 6e2a 2a3a 2043  stomization**: C
+00000390: 7573 746f 6d69 7a65 2063 6f6c 6f72 7320  ustomize colors 
+000003a0: 746f 206d 6174 6368 2079 6f75 7220 6170  to match your ap
+000003b0: 706c 6963 6174 696f 6e27 7320 6465 7369  plication's desi
+000003c0: 676e 206f 7220 6461 7461 2072 6570 7265  gn or data repre
+000003d0: 7365 6e74 6174 696f 6e2e 0a2d 202a 2a46  sentation..- **F
+000003e0: 6f6e 7420 4375 7374 6f6d 697a 6174 696f  ont Customizatio
+000003f0: 6e2a 2a3a 2041 646a 7573 7420 666f 6e74  n**: Adjust font
+00000400: 7320 666f 7220 7465 7874 2065 6c65 6d65  s for text eleme
+00000410: 6e74 7320 746f 2065 6e68 616e 6365 2072  nts to enhance r
+00000420: 6561 6461 6269 6c69 7479 2e0a 2d20 2a2a  eadability..- **
+00000430: 4469 6d65 6e73 696f 6e20 4375 7374 6f6d  Dimension Custom
+00000440: 697a 6174 696f 6e2a 2a3a 2043 7573 746f  ization**: Custo
+00000450: 6d69 7a65 2063 6861 7274 2064 696d 656e  mize chart dimen
+00000460: 7369 6f6e 7320 746f 2066 6974 2076 6172  sions to fit var
+00000470: 696f 7573 2064 6973 706c 6179 2073 697a  ious display siz
+00000480: 6573 2061 6e64 206c 6179 6f75 7473 2e0a  es and layouts..
+00000490: 0a23 2320 496d 706f 7274 696e 6720 2620  .## Importing & 
+000004a0: 496e 7374 616c 6c61 7469 6f6e 0a2a 2049  Installation.* I
+000004b0: 6e73 7461 6c6c 6174 696f 6e0a 2020 2020  nstallation.    
+000004c0: 6060 600a 2020 2020 7069 7020 696e 7374  ```.    pip inst
+000004d0: 616c 6c20 746b 6368 6172 740a 2020 2020  all tkchart.    
+000004e0: 6060 600a 0a2a 2049 6d70 6f72 7469 6e67  ```..* Importing
+000004f0: 0a20 2020 2020 6060 600a 2020 2020 696d  .     ```.    im
+00000500: 706f 7274 2074 6b63 6861 7274 0a20 2020  port tkchart.   
+00000510: 2060 6060 0a0a 2320 4c69 6e6b 730a 0a2a   ```..# Links..*
+00000520: 2a56 6973 6974 2047 6974 4875 6220 666f  *Visit GitHub fo
+00000530: 7220 446f 6375 6d65 6e74 6174 696f 6e3a  r Documentation:
+00000540: 2a2a 0a0a 2d20 2a2a 4769 7448 7562 2052  **..- **GitHub R
+00000550: 6570 6f73 6974 6f72 793a 2a2a 205b 746b  epository:** [tk
+00000560: 6368 6172 745d 2868 7474 7073 3a2f 2f67  chart](https://g
+00000570: 6974 6875 622e 636f 6d2f 5468 6973 616c  ithub.com/Thisal
+00000580: 2d44 2f74 6b63 6861 7274 290a            -D/tkchart).
```

### Comparing `tkchart-2.0.2/pyproject.toml` & `tkchart-2.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tkchart"
-version = "2.0.2"
+version = "2.0.3"
 authors = [
   { name = "Thisal-D" }
 ]
 
 license = { file = "LICENSE" }
 
 description = "tkchart is a Python library for creating live updating line charts in Tkinter."
```

### Comparing `tkchart-2.0.2/src/tkchart/FontStyle.py` & `tkchart-2.0.3/src/tkchart/FontStyle.py`

 * *Files identical despite different names*

### Comparing `tkchart-2.0.2/src/tkchart/Line.py` & `tkchart-2.0.3/src/tkchart/Line.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import Union, Tuple
+from typing import Union, Tuple, Literal
 from .Validate import Validate
 from .FontStyle import FontStyle
 
 
 class Line():
    def __init__(self,
                master: any = None,
                color: str = "#768df1",
                size: int = 1,
-               style: str = "normal", 
+               style: Literal["normal", "dashed", "dotted"] = "normal", 
                style_type: Tuple[int, int] = (4,4),
-               point_highlight: str = "disabled",
+               point_highlight: Literal["enabled", "disabled"] = "disabled",
                point_highlight_size: int = 4,
                point_highlight_color: str = "#768df1",
-               fill: str = "disabled",
+               fill: Literal["enabled", "disabled"] = "disabled",
                fill_color: str = "#5d6db6",
                *args: any
                ) -> None:
       """
       Initialize a Line object.
 
          Args:
@@ -54,33 +54,35 @@
       self.__color = color
       self.__size = size
       self.__y_end = 0
       self.__x_end  = self.__master._LineChart__x_axis_point_spacing* -1
       self.__data = []
       self.__temp_data = []
       self.__ret_data = []
-      self.__hide_state = False
+      self.__visibility = self.__master._LineChart__visibility
       self.__style = style
       self.__style_type = style_type
       self.__point_highlight = point_highlight
       self.__point_highlight_size = point_highlight_size
       self.__point_highlight_color = point_highlight_color
       self.__fill = fill
       self.__fill_color = fill_color
+      
+      self.__master._LineChart__lines.append(self)
 
 
    def configure(self, 
                   color: str = None, 
                   size: int = None,
-                  style: str = None,
+                  style: Literal["normal", "dashed", "dotted"] = None,
                   style_type: Tuple[int, int] = None,
-                  point_highlight: str = None,
+                  point_highlight: Literal["enabled", "disabled"] = None,
                   point_highlight_size: int = None,
                   point_highlight_color: str = None,
-                  fill: str = None,
+                  fill: Literal["enabled", "disabled"] = None,
                   fill_color:str = None,
                  ) -> None:
       """
       Configure attributes of the Line object.
 
          Args:
             color (str): The color of the line.
@@ -156,16 +158,31 @@
    def reset(self) -> None:
       """
       Reset the line.
       """
       self.__reset()
       self.__master._LineChart__call_reshow_data()
 
-      
-   def cget(self, attribute_name: str) -> any:
+   
+   def set_visible(self, state: bool) -> None:
+      """
+      Set the visibility of the line.
+
+         Args:
+               state (bool): True if the line should be visible, False otherwise.
+      """
+      Validate._isBool(state, "state")
+      if self.__visibility != state:
+         self.__visibility = state
+         self.__master._LineChart__call_reshow_data()
+         
+         
+   def cget(self, attribute_name:  Literal["master", "color", "size", "style", "style_type",
+                                          "point_highlight", "point_highlight_size", "point_highlight_color",
+                                          "fill", "fill_color", "__all__"]) -> any:
       """
       Get the value of a Line attribute.
 
          Args:
             attribute_name (str): Name of the attribute.
 
          Returns:
@@ -192,8 +209,19 @@
          "style_type" : self.__style_type,
          "point_highlight" : self.__point_highlight,
          "point_highlight_size" : self.__point_highlight_size,
          "point_highlight_color" : self.__point_highlight_color,
          "fill" : self.__fill,
          "fill_color" : self.__fill_color
          }
-      Validate._invalidCget(attribute_name)
+         
+      Validate._invalidCget(attribute_name)
+      
+      
+   def get_visibility(self) -> bool:
+      """
+      Get the visibility of the line.
+
+      Returns:
+         bool: True if the line is visible, False otherwise.
+      """
+      return self.__visibility
```

### Comparing `tkchart-2.0.2/src/tkchart/LineChart.py` & `tkchart-2.0.3/src/tkchart/LineChart.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import tkinter
-from typing import Union, Tuple, List
+from typing import Union, Tuple, List, Literal
 from .Utils import Utils
 from .Line import Line
 from .Validate import Validate
 
 
 class LineChart():
    def __init__(self,
@@ -20,41 +20,41 @@
                   
                   y_axis_precision: int = 0,
                   y_axis_data: any = "Y",
                   y_axis_label_count: int = 1,
                   y_axis_values: Tuple[Union[int, float], Union[int, float]] =  (None, None),
                   y_axis_font_color: str = "#606060",
                   y_axis_data_font_color: str = "#707070",
-                  y_axis_data_position: str = "top",
+                  y_axis_data_position: Literal["top", "side"] = "top",
                   y_axis_section_count: int = 0,
-                  y_axis_section_style: str = "normal",
+                  y_axis_section_style: Literal["normal", "dashed"] = "normal",
                   y_axis_section_style_type: Tuple[int, int] = (100, 50),
                   y_axis_section_color: str = "#2C2C2C",
                   
                   x_axis_data: str = "X",
                   x_axis_label_count: int = None,
                   x_axis_values: Tuple[any, ...] = (None, "None", None, "None"),
                   x_axis_display_values_indices: Tuple[int, ...] = None,
                   x_axis_font_color: str = "#606060",
                   x_axis_data_font_color: str = "#707070",
-                  x_axis_data_position: str = "top",
+                  x_axis_data_position: Literal["top", "side"] = "top",
                   x_axis_section_count: int = 0,
-                  x_axis_section_style: str = "normal",
+                  x_axis_section_style: Literal["normal", "dashed"] = "normal",
                   x_axis_section_style_type: Tuple[int, int] = (100, 50),
                   x_axis_section_color: str = "#2C2C2C",
                   
-                  x_axis_point_spacing: Union[int, str] = "auto",
+                  x_axis_point_spacing: Union[int, Literal["auto"]] = "auto",
                   y_space: int = 0, 
                   x_space: int = 0,
                   
-                  pointer_state: str = "disabled",
+                  pointer_state: Literal["enabled", "disabled"] = "disabled",
                   pointing_callback_function: callable = None,
                   pointer_color: str = "#606060",
                   pointing_values_precision: int = 1,
-                  pointer_lock: str = "disabled",
+                  pointer_lock: Literal["enabled", "disabled"] = "disabled",
                   pointer_size: int = 1,
                   
                   *args: any,
                   ) -> None:
       """
       Initialize a LineChart object.
 
@@ -184,64 +184,66 @@
       self.__x_axis_section_count = x_axis_section_count
       self.__x_axis_label_count = x_axis_label_count
       self.__x_axis_display_values_indices = x_axis_display_values_indices
       self.__x_labels_values_index_change = 1
       self.__x_axis_data = str(x_axis_data)
       self.__x_axis_data_position = x_axis_data_position
       self.__x_axis_values = x_axis_values
-      self.__x_axis_values_handle_by = "auto"
+      self.__x_axis_values_handle_by = "label_count"
       self.__x_space = x_space
       self.__force_to_stop_data_showing = False
       self.__is_data_showing_working = False
       self.__pointer_state = pointer_state
       self.__pointing_callback_function = pointing_callback_function
       self.__pointing_values_precision = pointing_values_precision
       self.__pointer_lock = pointer_lock
       self.__pointer_size = pointer_size
       self.__pointer_color = pointer_color
+      self.__x_values_frame_place_req = True
+      self.__y_values_frame_place_req = True
       
       self.__place_x = 0
       self.__real_height = 0
       self.__real_width = 0
       self.__const_real_height = 0
       self.__const_real_width = 0
+      self.__visibility = True
       
-      self.__place_info_x = 0
-      self.__place_info_y = 0
-      self.__place_info_rely = 0
-      self.__place_info_relx = 0
-      self.__place_info_anchor = 0
-      
-      self.__pack_info_pady = 0
-      self.__pack_info_padx = 0
-      self.__pack_info_before = 0
-      self.__pack_info_after = 0
-      self.__pack_info_side = 0
-      self.__pack_info_anchor = 0
-      
-      self.__grid_info_column = 0
-      self.__grid_info_columnspan = 0
-      self.__grid_info_padx = 0
-      self.__grid_info_pady = 0
-      self.__grid_info_row = 0
-      self.__grid_info_rowspan = 0
-      self.__grid_info_sticky = 0
+      self.__place_info_x = None
+      self.__place_info_y = None
+      self.__place_info_rely = None
+      self.__place_info_relx = None
+      self.__place_info_anchor = None
+      
+      self.__pack_info_pady = None
+      self.__pack_info_padx = None
+      self.__pack_info_before = None
+      self.__pack_info_after = None
+      self.__pack_info_side = None
+      self.__pack_info_anchor = None
+      
+      self.__grid_info_column = None
+      self.__grid_info_columnspan = None
+      self.__grid_info_padx = None
+      self.__grid_info_pady = None
+      self.__grid_info_row = None
+      self.__grid_info_rowspan = None
+      self.__grid_info_sticky = None
       
       if self.__x_axis_point_spacing == "auto":
          self.__x_axis_point_spacing_handle_by = "auto"
       else:
          self.__x_axis_point_spacing_handle_by = "manual"
       
       if  self.__x_axis_display_values_indices != None :
          self.__x_axis_display_values_indices = Utils._sort_tuple(self.__x_axis_display_values_indices)
          self.__x_axis_values_handle_by = "label_indices"
-      elif self.__x_axis_label_count != None:
-         self.__x_axis_values_handle_by = "label_count"
       else:
-         self.__x_axis_values_handle_by = "auto"
+         self.__x_axis_values_handle_by = "label_count"
+    
       
       self.__create_widgets()
       self.__configure_required_widget_size()
       self.__configure_x_axis_labels_info()
       self.__configure_x_axis_point_spacing()
       self.__create_x_axis_labels()
       self.__set_x_axis_values()
@@ -262,24 +264,24 @@
       """
       Create widgets for the LineChart.
 
          This method initializes the main frame along with frames for the y-axis, x-axis, 
          y-axis values, x-axis values, y-axis data label, x-axis data label, output frame,
          output canvas, and pointer.
       """
-      
+   
       self.__main_frame = tkinter.Frame(master=self.__master)
-      self.__y_axis_frame = tkinter.Frame(master=self.__main_frame)
-      self.__x_axis_frame = tkinter.Frame(master=self.__main_frame)
       self.__x_axis_values_frame = tkinter.Frame(master=self.__main_frame)
       self.__y_axis_values_frame = tkinter.Frame(master=self.__main_frame)
       self.__y_axis_data_label = tkinter.Label(master=self.__main_frame)
       self.__x_axis_data_label = tkinter.Label(master=self.__main_frame)
       self.__output_frame = tkinter.Frame(master=self.__main_frame)
       self.__output_canvas = tkinter.Canvas(master=self.__output_frame, highlightthickness=0)
+      self.__y_axis_frame = tkinter.Frame(master=self.__main_frame)
+      self.__x_axis_frame = tkinter.Frame(master=self.__main_frame)
       self.__pointer = tkinter.Frame(master=self.__output_canvas)
    
    
    def __set_pointer_state(self) -> None:
       """
       Set the state of the pointer.
 
@@ -363,29 +365,33 @@
       """
       Place widgets within the LineChart.
 
          This method handles the placement of various widgets within the LineChart, including the main frame,
          y-axis frame, x-axis frame, output frame, output canvas, y-axis values frame, and x-axis values frame,
          based on the specified dimensions and positions.
       """
-   
+      
       self.__main_frame.configure(width=self.__width, height=self.__height)
       
       self.__y_axis_data_label.place_forget()
       self.__x_axis_data_label.place_forget()
-      if self.__y_axis_data_position=="top":
-         self.__y_axis_data_label.place(x=0, y=0)
-      else:
-         self.__y_axis_data_label.place(x=0, y=self.__y_space+self.__y_special_height_space+self.__real_height/2,anchor="w")
-      if self.__x_axis_data_position=="top":
-         self.__x_axis_data_label.place(rely=1, relx=1, x=-self.__x_axis_data_req_width, y=-self.__x_axis_data_req_height)
-      else:
-         self.__x_axis_data_label.place(rely=1, y=-self.__x_axis_data_req_height,relx=0, anchor="n",
-                                  x=(self.__real_width/2)+self.__y_axis_data_req_width_space_side+self.__y_value_req_width_space+self.__axis_size+self.__x_axis_data_req_width_space_top+self.__x_special_width_space)
       
+      if self.__y_axis_data != "":
+         if self.__y_axis_data_position=="top":
+            self.__y_axis_data_label.place(x=0, y=0)
+         else:
+            self.__y_axis_data_label.place(x=0, y=self.__y_space+self.__y_special_height_space+self.__real_height/2,anchor="w")
+            
+      if self.__x_axis_data != "":
+         if self.__x_axis_data_position=="top":
+            self.__x_axis_data_label.place(rely=1, relx=1, x=-self.__x_axis_data_req_width, y=-self.__x_axis_data_req_height)
+         else:
+            self.__x_axis_data_label.place(rely=1, y=-self.__x_axis_data_req_height,relx=0, anchor="n",
+                                    x=(self.__real_width/2)+self.__y_axis_data_req_width_space_side+self.__y_value_req_width_space+self.__axis_size+self.__x_axis_data_req_width_space_top+self.__x_special_width_space)
+         
       self.__y_axis_frame.configure(width=self.__axis_size)
       self.__x_axis_frame.configure(height=self.__axis_size)
       
       self.__y_axis_frame.place(x=self.__y_value_req_width_space+self.__y_axis_data_req_width_space_side,
                          y=float(self.__y_axis_data_req_height_space_top+(self.__y_value_req_height_space/2)+self.__y_special_height_space),
                          height=self.__const_real_height+self.__y_space+self.__axis_size)
       self.__x_axis_frame.place(x=self.__y_value_req_width_space+self.__y_axis_data_req_width_space_side,
@@ -396,17 +402,24 @@
       self.__output_frame.place(x=self.__y_value_req_width_space+self.__axis_size+self.__y_axis_data_req_width_space_side,
                                 width=self.__const_real_width,
                                 height=self.__const_real_height,
                                 y=float(self.__y_axis_data_req_height_space_top+(self.__y_value_req_height_space/2)+self.__y_special_height_space+self.__y_space))
       
       self.__output_canvas.place(y=0, x=0, height=self.__const_real_height, width=self.__const_real_width)
       
-      self.__y_axis_values_frame.place(x=self.__y_axis_data_req_width_space_side, width=self.__y_value_req_width_space, height=self.__height)
-      self.__x_axis_values_frame.place(x=0, rely=1, y=-self.__x_value_req_height_space+-self.__x_axis_data_req_height_space_side, height=self.__x_value_req_height_space, width=self.__width)
-
+      if self.__y_values_frame_place_req:
+         self.__y_axis_values_frame.place(x=self.__y_axis_data_req_width_space_side, width=self.__y_value_req_width_space, height=self.__height)
+      else:
+         self.__y_axis_values_frame.place_forget()
+         
+      if self.__x_values_frame_place_req:   
+         self.__x_axis_values_frame.place(x=0, rely=1, y=-self.__x_value_req_height_space+-self.__x_axis_data_req_height_space_side, height=self.__x_value_req_height_space, width=self.__width)
+      else:
+         self.__x_axis_values_frame.place_forget()
+         
 
    def __configure_x_axis_point_spacing(self) -> None:
       """
       Configure the spacing between points on the x-axis.
 
          This method calculates and sets the spacing between points on the x-axis based on the 
          specified handle method. If the spacing is handled automatically, it calculates the spacing 
@@ -429,50 +442,67 @@
          necessary space for displaying the data labels, axis values, and adjusts the real width
          and height of the LineChart accordingly.
       """
     
       self.__x_axis_data_req_width_space_top = 0
       self.__x_axis_data_req_height_space_side = 0
       self.__x_special_width_space = 0
-      
-      self.__x_axis_data_req_height = Utils._RequiredHeight(text=self.__x_axis_data, font=self.__data_font_style)
-      self.__x_axis_data_req_width = Utils._RequiredWidth(text=self.__x_axis_data, font=self.__data_font_style)
-      if self.__x_axis_data_position == "top":
-         self.__x_special_width_space = 15
-         self.__x_axis_data_req_width_space_top = Utils._RequiredWidth(text=self.__x_axis_data, font=self.__data_font_style)
-      else:
-         self.__x_axis_data_req_height_space_side = Utils._RequiredHeight(text=self.__x_axis_data, font=self.__data_font_style)
+      self.__x_axis_data_req_height = 0
+      self.__x_axis_data_req_width = 0
+      if self.__x_axis_data != "":
+         self.__x_axis_data_req_height = Utils._RequiredHeight(text=self.__x_axis_data, font=self.__data_font_style)
+         self.__x_axis_data_req_width = Utils._RequiredWidth(text=self.__x_axis_data, font=self.__data_font_style)
+         if self.__x_axis_data_position == "top":
+            self.__x_special_width_space = 15
+            self.__x_axis_data_req_width_space_top = Utils._RequiredWidth(text=self.__x_axis_data, font=self.__data_font_style)
+         else:
+            self.__x_axis_data_req_height_space_side = Utils._RequiredHeight(text=self.__x_axis_data, font=self.__data_font_style)
       
       self.__y_axis_data_req_height_space_top = 0
       self.__y_axis_data_req_width_space_side = 0
       self.__y_special_height_space = 0
       
+      self.__y_values_frame_place_req = True
+      self.__x_values_frame_place_req = True
       #self.__y_axis_data_req_height = Utils._RequiredHeight(text=self.__y_axis_data, font=self.__data_font_style)
       #self.__y_axis_data_req_width = Utils._RequiredWidth(text=self.__y_axis_data, font=self.__data_font_style)
-      if self.__y_axis_data_position == "top":
-         self.__y_special_height_space = 15
-         self.__y_axis_data_req_height_space_top = Utils._RequiredHeight(text=self.__y_axis_data, font=self.__data_font_style)
-      else:
-         self.__y_axis_data_req_width_space_side = Utils._RequiredWidth(text=self.__y_axis_data[0], font=self.__data_font_style)
-      
+      if self.__y_axis_data != "":
+         if self.__y_axis_data_position == "top":
+            self.__y_special_height_space = 15
+            self.__y_axis_data_req_height_space_top = Utils._RequiredHeight(text=self.__y_axis_data, font=self.__data_font_style)
+         else:
+            self.__y_axis_data_req_width_space_side = Utils._RequiredWidth(text=self.__y_axis_data[0], font=self.__data_font_style)
+         
       if self.__y_axis_label_count == 0:
-         self.__y_value_req_height_space = 1
-         self.__y_value_req_width_space = 1
+         self.__y_value_req_height_space = 0
+         self.__y_value_req_width_space = 0
+         self.__y_values_frame_place_req = False
       else:
          if len(Utils._format_float_with_precision(self.__y_axis_max_value, self.__y_axis_precision)) > len(Utils._format_float_with_precision(self.__y_axis_min_value, self.__y_axis_precision)) :
             y_value_temp = self.__y_axis_max_value
          else:
             y_value_temp = self.__y_axis_min_value
          self.__y_value_req_height_space = Utils._RequiredHeight(text=Utils._format_float_with_precision(y_value_temp, self.__y_axis_precision), font=self.__axis_font_style)
          self.__y_value_req_width_space = Utils._RequiredWidth(text=Utils._format_float_with_precision(y_value_temp, self.__y_axis_precision), font=self.__axis_font_style)
-         
-      self.__x_value_req_height_space = Utils._RequiredHeight(text=self.__x_axis_values[0], font=self.__axis_font_style)
+      
+      
+      self.__x_value_req_width_space = 0
+      self.__x_value_req_height_space = 0
+      if self.__x_axis_label_count == 0 and self.__x_axis_values_handle_by == "label_count" :
+         self.__x_values_frame_place_req = False
+      elif self.__x_axis_values_handle_by == "label_indices" and  (len(self.__x_axis_display_values_indices) == 0):
+         self.__x_values_frame_place_req = False
+      else:
+         self.__x_value_req_height_space = Utils._RequiredHeight(text=self.__x_axis_values[0], font=self.__axis_font_style)
       #self.__x_value_req_width_space = RequiredWidth(text=format_float_with_precision(self.__x_axis_data_max, self.__x_values_decimals), font=self.__axis_font_style) 
-      self.__x_value_req_width_space = Utils._get_max_required_label_width(data=self.__x_axis_values, font=self.__axis_font_style)
+         self.__x_value_req_width_space = Utils._get_max_required_label_width(data=self.__x_axis_values, font=self.__axis_font_style)
       
+      if self.__y_value_req_height_space/2 > self.__x_value_req_height_space:
+         self.__x_value_req_height_space = self.__y_value_req_height_space/2
+         
       self.__real_width = self.__width - (self.__y_value_req_width_space+self.__axis_size+self.__x_axis_data_req_width_space_top+self.__y_axis_data_req_width_space_side+\
                                           (self.__x_value_req_width_space/2)+self.__x_special_width_space+self.__x_space)
       
       self.__const_real_width = self.__real_width 
       self.__real_height = self.__height - (self.__y_axis_data_req_height_space_top+self.__axis_size+self.__x_value_req_height_space+self.__x_axis_data_req_height_space_side+\
                                           (self.__y_value_req_height_space/2)+self.__y_special_height_space+self.__y_space)
       self.__real_height = self.__real_height  
@@ -669,27 +699,25 @@
          x-axis values. If x-axis values are provided using label indices, it sets the label count to the length
          of the x-axis values. If x-axis values are handled automatically or by label count, it adjusts the label
          count and index change accordingly to ensure proper spacing and distribution of labels.
       """
       
       if self.__x_axis_values_handle_by == "label_indices" : 
          self.__x_axis_label_count = len(self.__x_axis_values)
-        
-      elif self.__x_axis_values_handle_by=="auto":
-         self.__x_axis_label_count=len(self.__x_axis_values)
-         self.__x_labels_values_index_change = 1
+      
          
       elif self.__x_axis_values_handle_by=="label_count":
          if self.__x_axis_label_count == 0:
             return
          x_axis_real_label_count = len(self.__x_axis_values)
          if self.__x_axis_label_count > x_axis_real_label_count:
             self.__x_axis_label_count = x_axis_real_label_count
-         while x_axis_real_label_count%self.__x_axis_label_count != 0:
-            self.__x_axis_label_count+=1
+         else:
+            while x_axis_real_label_count%self.__x_axis_label_count != 0:
+               self.__x_axis_label_count+=1
          self.__x_labels_values_index_change = int(x_axis_real_label_count/self.__x_axis_label_count)
             
             
    def __create_y_axis_sections(self) -> None:
       """
       Create sections on the y-axis.
 
@@ -752,52 +780,52 @@
             widget.destroy()
                
          
    def configure(self,
                   width: int = None,
                   height: int = None,
                   axis_size: int = None,
-                  x_axis_point_spacing: Union[int, str] = None, 
+                  x_axis_point_spacing: Union[int, Literal["auto"]] = None, 
                   
                   bg_color: str = None,
                   axis_color: str = None,
                   fg_color: str = None,
                   data_font_style: Tuple[str, int, str] = None,
                   axis_font_style: Tuple[str, int, str] = None,
             
                   y_axis_values: Union[int, float]=None,
                   y_axis_precision: int = None,
                   y_axis_font_color: str = None,
                   y_axis_data_font_color: str = None,
                   y_axis_section_count: int = None,
                   y_axis_section_color: str = None,
-                  y_axis_section_style: str = None,
+                  y_axis_section_style: Literal["normal", "dashed"] = None,
                   y_axis_section_style_type: Tuple[int, int] = None,
                   y_axis_label_count: int=None,
                   y_axis_data: any = None,
-                  y_axis_data_position: str = None,
+                  y_axis_data_position: Literal["top", "side"] = None,
                   y_space: int = None,
                   
                   x_axis_values: Tuple[any, ...] = None,
                   x_axis_data: any = None,
                   x_axis_font_color: str = None,
                   x_axis_data_font_color: str = None,
                   x_axis_label_count: int = None,
                   x_axis_section_count: int = None,
-                  x_axis_section_style: str = None,
+                  x_axis_section_style: Literal["normal", "dashed"] = None,
                   x_axis_section_style_type: Tuple[int, int] = None,
                   x_axis_section_color: str = None,
                   x_axis_display_values_indices: Tuple[int, ...] = None,
-                  x_axis_data_position: str = None,
+                  x_axis_data_position: Literal["top", "side"] = None,
                   x_space: int = None ,
                   
-                  pointer_state: str = None,
+                  pointer_state: Literal["enabled", "disabled"] = None,
                   pointing_values_precision: int = None,
                   pointer_color: str = None, 
-                  pointer_lock: str = None,
+                  pointer_lock: Literal["enabled", "disabled"] = None,
                   pointing_callback_function: callable = None, 
                   pointer_size: int = None
                   ) -> None:  
       
       """
       Configures the properties of the chart widget based on the provided arguments.
       
@@ -1065,14 +1093,16 @@
             widget_color_change_req = True
             widget_font_change_req = True
       
       elif x_axis_label_count!=None:
          Validate._isValidXAxisLabelCount(x_axis_label_count, "x_axis_label_count")
          self.__x_axis_values_handle_by = "label_count"
          if x_axis_label_count != self.__x_axis_label_count:
+            if x_axis_label_count == 0 or self.__x_axis_label_count == 0:
+               chart_reset_req = True
             self.__x_axis_label_count = x_axis_label_count
             chart_x_labels_change_req = True
             widget_color_change_req = True
             widget_font_change_req = True
          
       if pointer_color!=None:
          Validate._isValidColor(pointer_color, "pointer_color")
@@ -1252,29 +1282,33 @@
    def show_data(self, line: Line, data: List[Union[int, float]]) -> None:
       """
       Show data on the chart for the given line.
 
          Args:
             line (Line): The line object to which the data belongs.
             data (List[Union[int, float]]): The list of data points to be displayed.
-
+            
+         Raises:
+            ValueError: If the provided line object is not valid or not found in the chart.
+         
          This method adds the provided data to the line's existing data, adjusts the display of the chart accordingly,
          and shows the data points on the chart. It also handles various styles for displaying the data points,
          such as dashed or dotted lines, and highlights for individual data points.
       """
       
       Validate._isValidLine(line, "line")
       Validate._isValidData(data, "data")
       
       re_show_data = False
       if line not in self.__lines:
-         self.__lines.append(line)
+         Validate._invalidLine(line)
+         
       line._Line__data += data
       
-      if line._Line__hide_state != True :
+      if  line._Line__visibility:
          for d in data:
             self.__is_data_showing_working = True
             
             if not self.__force_to_stop_data_showing:
                x_start = line._Line__x_end
                y_start = line._Line__y_end
                
@@ -1488,15 +1522,15 @@
          pass
 
    def place(self,
              x: int = None,
              y: int = None,
              rely: Union[int, float] = None,
              relx: Union[int, float] = None,
-             anchor: str = None
+             anchor: Literal["n", "e", "s", "w", "ne", "nw", "se", "sw", "center"] = None
              ) -> None: 
       """
       Place the widget at a specific position within its parent widget.
 
          Args:
             x (int): The x-coordinate of the upper-left corner of the widget.
             y (int): The y-coordinate of the upper-left corner of the widget.
@@ -1514,16 +1548,16 @@
       
       
    def pack(self,
             pady: int = None,
             padx: int = None,
             before: any = None,
             after: any = None,
-            side: str = None,
-            anchor: str = None
+            side: Literal["top", "bottom", "left", "right"] = None,
+            anchor: Literal["n", "e", "s", "w", "ne", "nw", "se", "sw", "center"] = None
             ) -> None:
       """
       Pack the widget into its parent widget.
 
          Args:
             pady (int): Vertical padding.
             padx (int): Horizontal padding.
@@ -1546,15 +1580,15 @@
    def grid(self,
             column: int = None, 
             columnspan: int = None, 
             padx: int = None,  
             pady: int = None, 
             row: int = None, 
             rowspan: int = None, 
-            sticky: str = None
+            sticky: Literal["n", "e", "s", "w", "ne", "nw", "se", "sw"] = None
             ) -> None:
       """
       Grid the widget into its parent widget.
 
          Args:
             column (int): The column in which to place the widget.
             columnspan (int): The number of columns the widget occupies.
@@ -1579,123 +1613,130 @@
       
    def place_forget(self) -> None:
       """
       Remove the widget from the grid.
       """
       
       self.__main_frame.place_forget()
-      
+      self.__place_info_x = None
+      self.__place_info_y = None
+      self.__place_info_rely = None
+      self.__place_info_relx = None
+      self.__place_info_anchor = None
       
    def pack_forget(self) -> None:
       """
       Remove the widget from the pack.
       """
       
       self.__main_frame.pack_forget()
+      self.__pack_info_pady = None
+      self.__pack_info_padx = None
+      self.__pack_info_before = None
+      self.__pack_info_after = None
+      self.__pack_info_side = None
+      self.__pack_info_anchor = None
       
       
    def grid_forget(self) -> None:
       """
       Remove the widget from the grid.
       """
     
       self.__main_frame.grid_forget()
-      
-      
-   def place_back(self) -> None:
-      """
-      Display the widget in its original place using place geometry manager.
-      """
-      
-      self.__main_frame.place(x=self.__place_info_x, y=self.__place_info_y,
-                              rely=self.__place_info_rely, relx=self.__place_info_relx,
-                              anchor=self.__place_info_anchor)
-      
-      
-   def pack_back(self) -> None:
-      """
-      Display the widget in its original place using pack geometry manager.
-      """
-      
-      self.__main_frame.pack(pady=self.__pack_info_pady, padx=self.__pack_info_padx,
-                             before=self.__pack_info_before, after=self.__pack_info_after,
-                             side=self.__pack_info_side, 
-                             anchor=self.__pack_info_anchor)
-      
-      
-   def grid_back(self) -> None:
-      """
-      Display the widget in its original place using grid geometry manager.
-      """
-      
-      self.__main_frame.grid(column=self.__grid_info_column, columnspan=self.__grid_info_columnspan, 
-                           padx=self.__grid_info_padx,  pady=self.__grid_info_pady,
-                           row=self.__grid_info_row, rowspan=self.__grid_info_rowspan, sticky=self.__grid_info_sticky)
+      self.__grid_info_column = None
+      self.__grid_info_columnspan = None
+      self.__grid_info_padx = None
+      self.__grid_info_pady = None
+      self.__grid_info_row = None
+      self.__grid_info_rowspan = None
+      self.__grid_info_sticky = None
       
    
-   def hide(self, line: Line, state: bool) -> None:
+   def set_line_visibility(self, line: Line, state: bool) -> None:
       """
       Hide or show a specific line.
 
          Args:
             line (Line): The line object to hide or show.
             state (bool): The hide/show state of the line.
       """
       
       Validate._isValidLine(line, "line")
       Validate._isBool(state, "state")
-      if line._Line__hide_state != state:
-         line._Line__hide_state = state
+      if line._Line__visibility != state or self.__visibility != state:
+         line._Line__visibility = state
          self.__call_reshow_data()
       
       
-   def hide_all(self, state: bool) -> None:
+   def set_lines_visibility(self, state: bool) -> None:
       """
       Hide or show all lines.
 
          Args:
             state (bool): The hide/show state of all lines.
       """
       
       Validate._isBool(state, "state")
-      if state == True:
+      self.__visibility = state
+      if state == False:
          self.__output_canvas.place_forget()
       for line in self.__lines:
-         line._Line__hide_state = state
+         line._Line__visibility = state
       self.__call_reshow_data()
    
    
    def reset(self) -> None:
       """
       Reset the chart and lines to their initial state.
       """
+      
       self.__reset_chart_info()
       self.__reset_lines_info()
       
       
    def __apply_line_configuration(self) -> None :
       """
       Apply changes to the lines and redraw the chart.
       """
       
       self.__call_reshow_data()
       
    
-   def cget(self, attribute_name: str) -> any :
+   def cget(self, attribute_name: Literal[
+         "width", "height", "axis_color", "bg_color", "fg_color",
+         "data_font_style", "axis_font_style", "y_axis_precision", 
+         "y_axis_data", "y_axis_label_count", "y_axis_values", 
+         "y_axis_font_color", "y_axis_data_font_color", 
+         "y_axis_data_position", "y_axis_section_count", 
+         "y_axis_section_style", "y_axis_section_style_type", 
+         "y_axis_section_color", "x_axis_data", "x_axis_label_count", 
+         "x_axis_values", "x_axis_display_values_indices", 
+         "x_axis_font_color", "x_axis_data_font_color", 
+         "x_axis_data_position", "x_axis_section_count", 
+         "x_axis_section_style", "x_axis_section_style_type", 
+         "x_axis_section_color", "x_axis_point_spacing", 
+         "y_space", "x_space", "pointer_state", 
+         "pointing_callback_function", "pointer_color", 
+         "pointing_values_precision", "pointer_lock", 
+         "pointer_size", "__all__"
+      ] = "__all__") -> any :
       """
       Get the value of the specified attribute.
 
          Args:
             attribute_name (str): The name of the attribute to get.
             __all__ (str): all the attributes as a dict
 
          Returns:
             any: The value of the specified attribute.
       """
       
+      if attribute_name == "width": return self.__width
+      if attribute_name == "height": return self.__height
       if attribute_name == "axis_color": return self.__axis_color
       if attribute_name == "bg_color": return self.__bg_color
       if attribute_name == "fg_color": return self.__fg_color
       if attribute_name == "data_font_style": return self.__data_font_style
       if attribute_name == "axis_font_style": return self.__axis_font_style
       if attribute_name == "y_axis_precision": return self.__y_axis_precision
       if attribute_name == "y_axis_data": return self.__y_axis_data
@@ -1727,14 +1768,16 @@
       if attribute_name == "pointer_color": return self.__pointer_color
       if attribute_name == "pointing_values_precision": return self.__pointing_values_precision
       if attribute_name == "pointer_lock": return self.__pointer_lock
       if attribute_name == "pointer_size": return self.__pointer_size
       
       if attribute_name == "__all__":
          return {
+            "width" : self.__width,
+            "height" : self.__height,
             "axis_color" : self.__axis_color,
             "bg_color" : self.__bg_color,
             "fg_color" : self.__fg_color,
             "data_font_style" : self.__data_font_style,
             "axis_font_style" : self.__axis_font_style,
             "y_axis_precision" : self.__y_axis_precision,
             "y_axis_data" : self.__y_axis_data,
@@ -1765,8 +1808,122 @@
             "pointing_callback_function" : self.__pointing_callback_function,
             "pointer_color" : self.__pointer_color,
             "pointing_values_precision" : self.__pointing_values_precision,
             "pointer_lock" : self.__pointer_lock,
             "pointer_size" : self.__pointer_size
             }
          
+      Validate._invalidCget(attribute_name)
+   
+   
+   def get_line_visibility(self, line: Line):
+      """
+      Get the visibility state of a specific line.
+
+         Args:
+            line (Line): The Line object for which visibility is queried.
+
+         Returns:
+            bool: True if the line is visible, False otherwise.
+
+         Raises:
+            ValueError: If the provided line object is not valid or not found in the chart.
+      """
+    
+      Validate._isValidLine(line, "line")
+      if line in self.__lines:
+         return line._Line__visibility;
+      else:
+         Validate._invalidLine(line)
+
+      
+   def place_info(self, attribute_name: Literal["x", "y", "relx", "rely", "anchor", "__all__"] = "__all__"):
+      """
+      Get the value of the specified place info.
+
+         Args:
+            attribute_name (str): The name of the attribute to get.
+
+         Returns:
+            any: The value of the specified attribute.
+      """
+      
+      if attribute_name == "x": return self.__place_info_x
+      if attribute_name == "y": return self.__place_info_y
+      if attribute_name == "relx": return self.__place_info_relx
+      if attribute_name == "rely": return self.__place_info_rely
+      if attribute_name == "anchor": return self.__place_info_anchor
+      
+      if attribute_name == "__all__":
+         return {
+            "x": self.__place_info_x,
+            "y": self.__place_info_y,
+            "relx": self.__place_info_relx,
+            "rely": self.__place_info_rely,
+            "anchor": self.__place_info_anchor
+         }
+      
+      Validate._invalidCget(attribute_name)
+      
+
+   def pack_info(self, attribute_name: Literal["padx", "pady", "before", "after", "side", "anchor", "__all__"] = "__all__"):
+      """
+      Get the value of the specified pack info.
+
+         Args:
+            attribute_name (str): The name of the attribute to get.
+
+         Returns:
+            any: The value of the specified attribute.
+      """
+      
+      if attribute_name == "padx": return self.__pack_info_padx
+      if attribute_name == "pady": return self.__pack_info_pady
+      if attribute_name == "before": return self.__pack_info_before
+      if attribute_name == "after": return self.__pack_info_after
+      if attribute_name == "side": return self.__pack_info_side 
+      if attribute_name == "anchor": return self.__pack_info_anchor
+      
+      if attribute_name == "__all__":
+         return {
+            "padx": self.__pack_info_padx,
+            "pady": self.__pack_info_pady,
+            "before": self.__pack_info_before,
+            "after": self.__pack_info_after,
+            "side": self.__pack_info_side,
+            "anchor": self.__pack_info_anchor
+         }
+      
+      Validate._invalidCget(attribute_name)
+      
+      
+   def grid_info(self, attribute_name: Literal["row", "column", "rowspan", "columnspan", "padx", "pady", "sticky", "__all__"] = "__all__"):
+      """
+      Get the value of the specified grid info.
+
+         Args:
+            attribute_name (str): The name of the attribute to get.
+
+         Returns:
+            any: The value of the specified attribute.
+      """
+      
+      if attribute_name == "row": return self.__grid_info_row
+      if attribute_name == "column": return self.__grid_info_column
+      if attribute_name == "rowspan": return self.__grid_info_rowspan
+      if attribute_name == "columnspan": return self.__grid_info_columnspan
+      if attribute_name == "padx": return self.__grid_info_padx
+      if attribute_name == "pady": return self.__grid_info_pady
+      if attribute_name == "sticky": return self.__grid_info_sticky
+      
+      if attribute_name == "__all__":
+         return {
+            "row": self.__grid_info_row,
+            "column": self.__grid_info_column,
+            "rowspan": self.__grid_info_rowspan,
+            "columnspan": self.__grid_info_columnspan,
+            "padx": self.__grid_info_padx,
+            "pady": self.__grid_info_pady,
+            "sticky": self.__grid_info_sticky
+         }
+      
       Validate._invalidCget(attribute_name)
```

### Comparing `tkchart-2.0.2/src/tkchart/Utils.py` & `tkchart-2.0.3/src/tkchart/Utils.py`

 * *Files identical despite different names*

### Comparing `tkchart-2.0.2/src/tkchart/Validate.py` & `tkchart-2.0.3/src/tkchart/Validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,8 +267,14 @@
                 f'''{Validate._var_font(var)} {Validate._error_font("all values should be int.")}'''
             )
             
             
     def _invalidCget(var: str) -> None:
         raise ValueError(
                 f'''{Validate._var_font(var)} {Validate._error_font("Invalid attribute.")}'''
+            )
+        
+        
+    def _invalidLine(line) -> None:
+        raise ValueError(
+                f'''{Validate._var_font(str(line))} {Validate._error_font("The line is not part of this line chart.")}'''
             )
```

### Comparing `tkchart-2.0.2/src/tkchart.egg-info/PKG-INFO` & `tkchart-2.0.3/src/tkchart.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2074 6b63  : 2.1..Name: tkc
 00000020: 6861 7274 0d0a 5665 7273 696f 6e3a 2032  hart..Version: 2
-00000030: 2e30 2e32 0d0a 5375 6d6d 6172 793a 2074  .0.2..Summary: t
+00000030: 2e30 2e33 0d0a 5375 6d6d 6172 793a 2074  .0.3..Summary: t
 00000040: 6b63 6861 7274 2069 7320 6120 5079 7468  kchart is a Pyth
 00000050: 6f6e 206c 6962 7261 7279 2066 6f72 2063  on library for c
 00000060: 7265 6174 696e 6720 6c69 7665 2075 7064  reating live upd
 00000070: 6174 696e 6720 6c69 6e65 2063 6861 7274  ating line chart
 00000080: 7320 696e 2054 6b69 6e74 6572 2e0d 0a41  s in Tkinter...A
 00000090: 7574 686f 723a 2054 6869 7361 6c2d 440d  uthor: Thisal-D.
 000000a0: 0a4c 6963 656e 7365 3a20 436f 7079 7269  .License: Copyri
@@ -151,68 +151,66 @@
 00000960: 7079 2e74 6563 682f 7072 6f6a 6563 742f  py.tech/project/
 00000970: 746b 6368 6172 7429 205b 215b 446f 776e  tkchart) [![Down
 00000980: 6c6f 6164 735d 2868 7474 7073 3a2f 2f73  loads](https://s
 00000990: 7461 7469 632e 7065 7079 2e74 6563 682f  tatic.pepy.tech/
 000009a0: 6261 6467 652f 746b 6368 6172 742f 7765  badge/tkchart/we
 000009b0: 656b 295d 2868 7474 7073 3a2f 2f70 6570  ek)](https://pep
 000009c0: 792e 7465 6368 2f70 726f 6a65 6374 2f74  y.tech/project/t
-000009d0: 6b63 6861 7274 290d 0a0d 0a3c 696d 6720  kchart)....<img 
-000009e0: 7372 633d 2268 7474 7073 3a2f 2f64 7269  src="https://dri
-000009f0: 7665 2e67 6f6f 676c 652e 636f 6d2f 7468  ve.google.com/th
-00000a00: 756d 626e 6169 6c3f 6964 3d31 6a4f 6c74  umbnail?id=1jOlt
-00000a10: 5435 7142 764c 6d4b 4164 5355 367a 6239  T5qBvLmKAdSU6zb9
-00000a20: 776a 6833 4759 6136 6a52 7644 2673 7a3d  wjh3GYa6jRvD&sz=
-00000a30: 7731 3830 223e 0d0a 0d0a 3c2f 6469 763e  w180">....</div>
-00000a40: 0d0a 0d0a 2323 2320 3c6c 693e 746b 6368  ....### <li>tkch
-00000a50: 6172 7420 6973 2061 2050 7974 686f 6e20  art is a Python 
-00000a60: 6c69 6272 6172 7920 666f 7220 6372 6561  library for crea
-00000a70: 7469 6e67 206c 6976 6520 7570 6461 7469  ting live updati
-00000a80: 6e67 206c 696e 6520 6368 6172 7473 2069  ng line charts i
-00000a90: 6e20 546b 696e 7465 722e 3c2f 6c69 3e0d  n Tkinter.</li>.
-00000aa0: 0a0d 0a23 2320 4665 6174 7572 6573 0d0a  ...## Features..
-00000ab0: 0d0a 2d20 2a2a 4c69 7665 2055 7064 6174  ..- **Live Updat
-00000ac0: 652a 2a3a 2044 6973 706c 6179 206c 6976  e**: Display liv
-00000ad0: 6520 6461 7461 2077 6974 6820 6c69 6e65  e data with line
-00000ae0: 2063 6861 7274 732e 0d0a 2d20 2a2a 4d75   charts...- **Mu
-00000af0: 6c74 6970 6c65 204c 696e 6573 2a2a 3a20  ltiple Lines**: 
-00000b00: 5375 7070 6f72 7420 666f 7220 706c 6f74  Support for plot
-00000b10: 7469 6e67 206d 756c 7469 706c 6520 6c69  ting multiple li
-00000b20: 6e65 7320 6f6e 2074 6865 2073 616d 6520  nes on the same 
-00000b30: 6368 6172 7420 666f 7220 6561 7379 2063  chart for easy c
-00000b40: 6f6d 7061 7269 736f 6e2e 0d0a 2d20 2a2a  omparison...- **
-00000b50: 436f 6c6f 7220 4375 7374 6f6d 697a 6174  Color Customizat
-00000b60: 696f 6e2a 2a3a 2043 7573 746f 6d69 7a65  ion**: Customize
-00000b70: 2063 6f6c 6f72 7320 746f 206d 6174 6368   colors to match
-00000b80: 2079 6f75 7220 6170 706c 6963 6174 696f   your applicatio
-00000b90: 6e27 7320 6465 7369 676e 206f 7220 6461  n's design or da
-00000ba0: 7461 2072 6570 7265 7365 6e74 6174 696f  ta representatio
-00000bb0: 6e2e 0d0a 2d20 2a2a 466f 6e74 2043 7573  n...- **Font Cus
-00000bc0: 746f 6d69 7a61 7469 6f6e 2a2a 3a20 4164  tomization**: Ad
-00000bd0: 6a75 7374 2066 6f6e 7473 2066 6f72 2074  just fonts for t
-00000be0: 6578 7420 656c 656d 656e 7473 2074 6f20  ext elements to 
-00000bf0: 656e 6861 6e63 6520 7265 6164 6162 696c  enhance readabil
-00000c00: 6974 792e 0d0a 2d20 2a2a 4469 6d65 6e73  ity...- **Dimens
-00000c10: 696f 6e20 4375 7374 6f6d 697a 6174 696f  ion Customizatio
-00000c20: 6e2a 2a3a 2043 7573 746f 6d69 7a65 2063  n**: Customize c
-00000c30: 6861 7274 2064 696d 656e 7369 6f6e 7320  hart dimensions 
-00000c40: 746f 2066 6974 2076 6172 696f 7573 2064  to fit various d
-00000c50: 6973 706c 6179 2073 697a 6573 2061 6e64  isplay sizes and
-00000c60: 206c 6179 6f75 7473 2e0d 0a0d 0a23 2320   layouts.....## 
-00000c70: 496d 706f 7274 696e 6720 2620 496e 7374  Importing & Inst
-00000c80: 616c 6c61 7469 6f6e 0d0a 2a20 496e 7374  allation..* Inst
-00000c90: 616c 6c61 7469 6f6e 0d0a 2020 2020 6060  allation..    ``
-00000ca0: 600d 0a20 2020 2070 6970 2069 6e73 7461  `..    pip insta
-00000cb0: 6c6c 2074 6b63 6861 7274 0d0a 2020 2020  ll tkchart..    
-00000cc0: 6060 600d 0a0d 0a2a 2049 6d70 6f72 7469  ```....* Importi
-00000cd0: 6e67 0d0a 2020 2020 2060 6060 0d0a 2020  ng..     ```..  
-00000ce0: 2020 696d 706f 7274 2074 6b63 6861 7274    import tkchart
-00000cf0: 0d0a 2020 2020 6060 600d 0a0d 0a23 204c  ..    ```....# L
-00000d00: 696e 6b73 0d0a 0d0a 2d20 2a2a 5669 7369  inks....- **Visi
-00000d10: 7420 4769 7448 7562 2066 6f72 204d 6f72  t GitHub for Mor
-00000d20: 6520 4465 7461 696c 732e 2e2e 2e2e 2a2a  e Details.....**
-00000d30: 0d0a 2d20 2323 202a 2a47 6974 4875 622e  ..- ## **GitHub.
-00000d40: 636f 6d2a 2a20 2020 3a20 203c 6120 6872  com**   :  <a hr
-00000d50: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+000009d0: 6b63 6861 7274 290d 0a0d 0a0d 0a3c 696d  kchart)......<im
+000009e0: 6720 7372 633d 2268 7474 7073 3a2f 2f64  g src="https://d
+000009f0: 7269 7665 2e67 6f6f 676c 652e 636f 6d2f  rive.google.com/
+00000a00: 7468 756d 626e 6169 6c3f 6964 3d31 6348  thumbnail?id=1cH
+00000a10: 7273 4649 4c48 4a37 6132 6267 4d58 766b  rsFILHJ7a2bgMXvk
+00000a20: 2d50 576c 6e4c 5a78 3176 436e 5652 2673  -PWlnLZx1vCnVR&s
+00000a30: 7a3d 7731 3830 223e 0d0a 0d0a 3c2f 6469  z=w180">....</di
+00000a40: 763e 0d0a 0d0a 2323 2320 3c6c 693e 746b  v>....### <li>tk
+00000a50: 6368 6172 7420 6973 2061 2050 7974 686f  chart is a Pytho
+00000a60: 6e20 6c69 6272 6172 7920 666f 7220 6372  n library for cr
+00000a70: 6561 7469 6e67 206c 6976 6520 7570 6461  eating live upda
+00000a80: 7469 6e67 206c 696e 6520 6368 6172 7473  ting line charts
+00000a90: 2069 6e20 546b 696e 7465 722e 3c2f 6c69   in Tkinter.</li
+00000aa0: 3e0d 0a0d 0a23 2320 4665 6174 7572 6573  >....## Features
+00000ab0: 0d0a 0d0a 2d20 2a2a 4c69 7665 2055 7064  ....- **Live Upd
+00000ac0: 6174 652a 2a3a 2044 6973 706c 6179 206c  ate**: Display l
+00000ad0: 6976 6520 6461 7461 2077 6974 6820 6c69  ive data with li
+00000ae0: 6e65 2063 6861 7274 732e 0d0a 2d20 2a2a  ne charts...- **
+00000af0: 4d75 6c74 6970 6c65 204c 696e 6573 2a2a  Multiple Lines**
+00000b00: 3a20 5375 7070 6f72 7420 666f 7220 706c  : Support for pl
+00000b10: 6f74 7469 6e67 206d 756c 7469 706c 6520  otting multiple 
+00000b20: 6c69 6e65 7320 6f6e 2074 6865 2073 616d  lines on the sam
+00000b30: 6520 6368 6172 7420 666f 7220 6561 7379  e chart for easy
+00000b40: 2063 6f6d 7061 7269 736f 6e2e 0d0a 2d20   comparison...- 
+00000b50: 2a2a 436f 6c6f 7220 4375 7374 6f6d 697a  **Color Customiz
+00000b60: 6174 696f 6e2a 2a3a 2043 7573 746f 6d69  ation**: Customi
+00000b70: 7a65 2063 6f6c 6f72 7320 746f 206d 6174  ze colors to mat
+00000b80: 6368 2079 6f75 7220 6170 706c 6963 6174  ch your applicat
+00000b90: 696f 6e27 7320 6465 7369 676e 206f 7220  ion's design or 
+00000ba0: 6461 7461 2072 6570 7265 7365 6e74 6174  data representat
+00000bb0: 696f 6e2e 0d0a 2d20 2a2a 466f 6e74 2043  ion...- **Font C
+00000bc0: 7573 746f 6d69 7a61 7469 6f6e 2a2a 3a20  ustomization**: 
+00000bd0: 4164 6a75 7374 2066 6f6e 7473 2066 6f72  Adjust fonts for
+00000be0: 2074 6578 7420 656c 656d 656e 7473 2074   text elements t
+00000bf0: 6f20 656e 6861 6e63 6520 7265 6164 6162  o enhance readab
+00000c00: 696c 6974 792e 0d0a 2d20 2a2a 4469 6d65  ility...- **Dime
+00000c10: 6e73 696f 6e20 4375 7374 6f6d 697a 6174  nsion Customizat
+00000c20: 696f 6e2a 2a3a 2043 7573 746f 6d69 7a65  ion**: Customize
+00000c30: 2063 6861 7274 2064 696d 656e 7369 6f6e   chart dimension
+00000c40: 7320 746f 2066 6974 2076 6172 696f 7573  s to fit various
+00000c50: 2064 6973 706c 6179 2073 697a 6573 2061   display sizes a
+00000c60: 6e64 206c 6179 6f75 7473 2e0d 0a0d 0a23  nd layouts.....#
+00000c70: 2320 496d 706f 7274 696e 6720 2620 496e  # Importing & In
+00000c80: 7374 616c 6c61 7469 6f6e 0d0a 2a20 496e  stallation..* In
+00000c90: 7374 616c 6c61 7469 6f6e 0d0a 2020 2020  stallation..    
+00000ca0: 6060 600d 0a20 2020 2070 6970 2069 6e73  ```..    pip ins
+00000cb0: 7461 6c6c 2074 6b63 6861 7274 0d0a 2020  tall tkchart..  
+00000cc0: 2020 6060 600d 0a0d 0a2a 2049 6d70 6f72    ```....* Impor
+00000cd0: 7469 6e67 0d0a 2020 2020 2060 6060 0d0a  ting..     ```..
+00000ce0: 2020 2020 696d 706f 7274 2074 6b63 6861      import tkcha
+00000cf0: 7274 0d0a 2020 2020 6060 600d 0a0d 0a23  rt..    ```....#
+00000d00: 204c 696e 6b73 0d0a 0d0a 2a2a 5669 7369   Links....**Visi
+00000d10: 7420 4769 7448 7562 2066 6f72 2044 6f63  t GitHub for Doc
+00000d20: 756d 656e 7461 7469 6f6e 3a2a 2a0d 0a0d  umentation:**...
+00000d30: 0a2d 202a 2a47 6974 4875 6220 5265 706f  .- **GitHub Repo
+00000d40: 7369 746f 7279 3a2a 2a20 5b74 6b63 6861  sitory:** [tkcha
+00000d50: 7274 5d28 6874 7470 733a 2f2f 6769 7468  rt](https://gith
 00000d60: 7562 2e63 6f6d 2f54 6869 7361 6c2d 442f  ub.com/Thisal-D/
-00000d70: 746b 6368 6172 7422 2074 6172 6765 743d  tkchart" target=
-00000d80: 225f 626c 616e 6b22 203e 3c69 3e74 6b63  "_blank" ><i>tkc
-00000d90: 6861 7274 3c2f 693e 3c2f 613e 0d0a       hart</i></a>..
+00000d70: 746b 6368 6172 7429 0d0a                 tkchart)..
```

