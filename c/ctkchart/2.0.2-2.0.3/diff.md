# Comparing `tmp/ctkchart-2.0.2.tar.gz` & `tmp/ctkchart-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctkchart-2.0.2.tar", last modified: Fri Mar 22 05:48:33 2024, max compression
+gzip compressed data, was "ctkchart-2.0.3.tar", last modified: Mon Apr  1 23:36:59 2024, max compression
```

## Comparing `ctkchart-2.0.2.tar` & `ctkchart-2.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-03-22 05:48:33.730351 ctkchart-2.0.2/
--rw-rw-rw-   0        0        0     1091 2024-02-14 05:02:34.000000 ctkchart-2.0.2/LICENSE
--rw-rw-rw-   0        0        0     3674 2024-03-22 05:48:33.730351 ctkchart-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1530 2024-03-22 05:46:46.000000 ctkchart-2.0.2/README.md
--rw-rw-rw-   0        0        0     1011 2024-03-22 05:42:00.000000 ctkchart-2.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-22 05:48:33.730351 ctkchart-2.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-22 05:48:33.714726 ctkchart-2.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-03-22 05:48:33.714726 ctkchart-2.0.2/src/ctkchart/
--rw-rw-rw-   0        0        0     8045 2024-03-22 03:51:41.000000 ctkchart-2.0.2/src/ctkchart/CTkLine.py
--rw-rw-rw-   0        0        0    91594 2024-03-22 05:15:07.000000 ctkchart-2.0.2/src/ctkchart/CTkLineChart.py
--rw-rw-rw-   0        0        0     1804 2024-03-11 17:43:59.000000 ctkchart-2.0.2/src/ctkchart/FontStyle.py
--rw-rw-rw-   0        0        0     1916 2024-03-22 05:40:12.000000 ctkchart-2.0.2/src/ctkchart/Utils.py
--rw-rw-rw-   0        0        0    10459 2024-03-22 05:41:02.000000 ctkchart-2.0.2/src/ctkchart/Validate.py
--rw-rw-rw-   0        0        0      267 2024-03-22 05:41:54.000000 ctkchart-2.0.2/src/ctkchart/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-22 05:48:33.730351 ctkchart-2.0.2/src/ctkchart.egg-info/
--rw-rw-rw-   0        0        0     3674 2024-03-22 05:48:33.000000 ctkchart-2.0.2/src/ctkchart.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2024-03-22 05:48:33.000000 ctkchart-2.0.2/src/ctkchart.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-22 05:48:33.000000 ctkchart-2.0.2/src/ctkchart.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-03-22 05:48:33.000000 ctkchart-2.0.2/src/ctkchart.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 23:36:59.516157 ctkchart-2.0.3/
+-rw-rw-rw-   0        0        0     1091 2024-02-14 05:02:34.000000 ctkchart-2.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3638 2024-04-01 23:36:59.500905 ctkchart-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1491 2024-04-01 23:35:38.000000 ctkchart-2.0.3/README.md
+-rw-rw-rw-   0        0        0     1011 2024-04-01 11:03:36.000000 ctkchart-2.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-01 23:36:59.517134 ctkchart-2.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-01 23:36:59.127618 ctkchart-2.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-01 23:36:59.488140 ctkchart-2.0.3/src/ctkchart/
+-rw-rw-rw-   0        0        0     9191 2024-04-01 05:35:12.000000 ctkchart-2.0.3/src/ctkchart/CTkLine.py
+-rw-rw-rw-   0        0        0    98481 2024-04-01 23:20:48.000000 ctkchart-2.0.3/src/ctkchart/CTkLineChart.py
+-rw-rw-rw-   0        0        0     1804 2024-03-31 14:08:39.000000 ctkchart-2.0.3/src/ctkchart/FontStyle.py
+-rw-rw-rw-   0        0        0     1916 2024-03-22 05:40:12.000000 ctkchart-2.0.3/src/ctkchart/Utils.py
+-rw-rw-rw-   0        0        0    10886 2024-04-01 18:33:10.000000 ctkchart-2.0.3/src/ctkchart/Validate.py
+-rw-rw-rw-   0        0        0      289 2024-04-01 23:24:49.000000 ctkchart-2.0.3/src/ctkchart/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 23:36:59.499930 ctkchart-2.0.3/src/ctkchart.egg-info/
+-rw-rw-rw-   0        0        0     3638 2024-04-01 23:36:59.000000 ctkchart-2.0.3/src/ctkchart.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2024-04-01 23:36:59.000000 ctkchart-2.0.3/src/ctkchart.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 23:36:59.000000 ctkchart-2.0.3/src/ctkchart.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-01 23:36:59.000000 ctkchart-2.0.3/src/ctkchart.egg-info/top_level.txt
```

### Comparing `ctkchart-2.0.2/LICENSE` & `ctkchart-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ctkchart-2.0.2/PKG-INFO` & `ctkchart-2.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2063 746b  : 2.1..Name: ctk
 00000020: 6368 6172 740d 0a56 6572 7369 6f6e 3a20  chart..Version: 
-00000030: 322e 302e 320d 0a53 756d 6d61 7279 3a20  2.0.2..Summary: 
+00000030: 322e 302e 330d 0a53 756d 6d61 7279 3a20  2.0.3..Summary: 
 00000040: 6374 6b63 6861 7274 2069 7320 6120 5079  ctkchart is a Py
 00000050: 7468 6f6e 206c 6962 7261 7279 2066 6f72  thon library for
 00000060: 2063 7265 6174 696e 6720 6c69 7665 2075   creating live u
 00000070: 7064 6174 696e 6720 6c69 6e65 2063 6861  pdating line cha
 00000080: 7274 7320 696e 2063 7573 746f 6d74 6b69  rts in customtki
 00000090: 6e74 6572 2e0d 0a41 7574 686f 723a 2054  nter...Author: T
 000000a0: 6869 7361 6c2d 440d 0a4c 6963 656e 7365  hisal-D..License
@@ -160,71 +160,69 @@
 000009f0: 7374 6174 6963 2e70 6570 792e 7465 6368  static.pepy.tech
 00000a00: 2f62 6164 6765 2f63 746b 6368 6172 742f  /badge/ctkchart/
 00000a10: 7765 656b 295d 2868 7474 7073 3a2f 2f70  week)](https://p
 00000a20: 6570 792e 7465 6368 2f70 726f 6a65 6374  epy.tech/project
 00000a30: 2f63 746b 6368 6172 7429 0d0a 0d0a 3c69  /ctkchart)....<i
 00000a40: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
 00000a50: 6472 6976 652e 676f 6f67 6c65 2e63 6f6d  drive.google.com
-00000a60: 2f74 6875 6d62 6e61 696c 3f69 643d 316a  /thumbnail?id=1j
-00000a70: 4f6c 7454 3571 4276 4c6d 4b41 6453 5536  OltT5qBvLmKAdSU6
-00000a80: 7a62 3977 6a68 3347 5961 366a 5276 4426  zb9wjh3GYa6jRvD&
-00000a90: 737a 3d77 3138 3022 3e0d 0a0d 0a3c 2f64  sz=w180">....</d
-00000aa0: 6976 3e0d 0a0d 0a23 2323 203c 6c69 3e63  iv>....### <li>c
-00000ab0: 746b 6368 6172 7420 6973 2061 2050 7974  tkchart is a Pyt
-00000ac0: 686f 6e20 6c69 6272 6172 7920 666f 7220  hon library for 
-00000ad0: 6372 6561 7469 6e67 206c 6976 6520 7570  creating live up
-00000ae0: 6461 7469 6e67 206c 696e 6520 6368 6172  dating line char
-00000af0: 7473 2069 6e20 6375 7374 6f6d 746b 696e  ts in customtkin
-00000b00: 7465 722e 3c2f 6c69 3e0d 0a0d 0a3c 2f64  ter.</li>....</d
-00000b10: 6976 3e0d 0a0d 0a23 2320 4665 6174 7572  iv>....## Featur
-00000b20: 6573 0d0a 0d0a 2d20 2a2a 4c69 7665 2055  es....- **Live U
-00000b30: 7064 6174 652a 2a3a 2044 6973 706c 6179  pdate**: Display
-00000b40: 206c 6976 6520 6461 7461 2077 6974 6820   live data with 
-00000b50: 6c69 6e65 2063 6861 7274 732e 0d0a 2d20  line charts...- 
-00000b60: 2a2a 4d75 6c74 6970 6c65 204c 696e 6573  **Multiple Lines
-00000b70: 2a2a 3a20 5375 7070 6f72 7420 666f 7220  **: Support for 
-00000b80: 706c 6f74 7469 6e67 206d 756c 7469 706c  plotting multipl
-00000b90: 6520 6c69 6e65 7320 6f6e 2074 6865 2073  e lines on the s
-00000ba0: 616d 6520 6368 6172 7420 666f 7220 6561  ame chart for ea
-00000bb0: 7379 2063 6f6d 7061 7269 736f 6e2e 0d0a  sy comparison...
-00000bc0: 2d20 2a2a 436f 6c6f 7220 4375 7374 6f6d  - **Color Custom
-00000bd0: 697a 6174 696f 6e2a 2a3a 2043 7573 746f  ization**: Custo
-00000be0: 6d69 7a65 2063 6f6c 6f72 7320 746f 206d  mize colors to m
-00000bf0: 6174 6368 2079 6f75 7220 6170 706c 6963  atch your applic
-00000c00: 6174 696f 6e27 7320 6465 7369 676e 206f  ation's design o
-00000c10: 7220 6461 7461 2072 6570 7265 7365 6e74  r data represent
-00000c20: 6174 696f 6e2e 0d0a 2d20 2a2a 4479 6e61  ation...- **Dyna
-00000c30: 6d69 6320 436f 6c6f 7220 4368 616e 6765  mic Color Change
-00000c40: 2a2a 3a20 4479 6e61 6d69 6320 436f 6c6f  **: Dynamic Colo
-00000c50: 7220 4368 616e 6765 2066 6f72 2044 6172  r Change for Dar
-00000c60: 6b20 2620 4c69 6768 742e 0d0a 2d20 2a2a  k & Light...- **
-00000c70: 466f 6e74 2043 7573 746f 6d69 7a61 7469  Font Customizati
-00000c80: 6f6e 2a2a 3a20 4164 6a75 7374 2066 6f6e  on**: Adjust fon
-00000c90: 7473 2066 6f72 2074 6578 7420 656c 656d  ts for text elem
-00000ca0: 656e 7473 2074 6f20 656e 6861 6e63 6520  ents to enhance 
-00000cb0: 7265 6164 6162 696c 6974 792e 0d0a 2d20  readability...- 
-00000cc0: 2a2a 4469 6d65 6e73 696f 6e20 4375 7374  **Dimension Cust
-00000cd0: 6f6d 697a 6174 696f 6e2a 2a3a 2043 7573  omization**: Cus
-00000ce0: 746f 6d69 7a65 2063 6861 7274 2064 696d  tomize chart dim
-00000cf0: 656e 7369 6f6e 7320 746f 2066 6974 2076  ensions to fit v
-00000d00: 6172 696f 7573 2064 6973 706c 6179 2073  arious display s
-00000d10: 697a 6573 2061 6e64 206c 6179 6f75 7473  izes and layouts
-00000d20: 2e0d 0a0d 0a23 2320 496d 706f 7274 696e  .....## Importin
-00000d30: 6720 2620 496e 7374 616c 6c61 7469 6f6e  g & Installation
-00000d40: 0d0a 2a20 496e 7374 616c 6c61 7469 6f6e  ..* Installation
-00000d50: 0d0a 2020 2020 6060 600d 0a20 2020 2070  ..    ```..    p
-00000d60: 6970 2069 6e73 7461 6c6c 2063 746b 6368  ip install ctkch
-00000d70: 6172 740d 0a20 2020 2060 6060 0d0a 0d0a  art..    ```....
-00000d80: 2a20 496d 706f 7274 696e 670d 0a20 2020  * Importing..   
-00000d90: 2020 6060 600d 0a20 2020 2069 6d70 6f72    ```..    impor
-00000da0: 7420 6374 6b63 6861 7274 0d0a 2020 2020  t ctkchart..    
-00000db0: 6060 600d 0a0d 0a23 204c 696e 6b73 0d0a  ```....# Links..
-00000dc0: 0d0a 2d20 2a2a 5669 7369 7420 4769 7448  ..- **Visit GitH
-00000dd0: 7562 2066 6f72 204d 6f72 6520 4465 7461  ub for More Deta
-00000de0: 696c 732e 2e2e 2e2e 2a2a 0d0a 2d20 2323  ils.....**..- ##
-00000df0: 202a 2a47 6974 4875 622e 636f 6d2a 2a20   **GitHub.com** 
-00000e00: 2020 3a20 203c 6120 6872 6566 3d22 6874    :  <a href="ht
-00000e10: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000e20: 2f54 6869 7361 6c2d 442f 6374 6b63 6861  /Thisal-D/ctkcha
-00000e30: 7274 2220 7461 7267 6574 3d22 5f62 6c61  rt" target="_bla
-00000e40: 6e6b 2220 3e3c 693e 6374 6b63 6861 7274  nk" ><i>ctkchart
-00000e50: 3c2f 693e 3c2f 613e 0d0a                 </i></a>..
+00000a60: 2f74 6875 6d62 6e61 696c 3f69 643d 3163  /thumbnail?id=1c
+00000a70: 4872 7346 494c 484a 3761 3262 674d 5876  HrsFILHJ7a2bgMXv
+00000a80: 6b2d 5057 6c6e 4c5a 7831 7643 6e56 5226  k-PWlnLZx1vCnVR&
+00000a90: 737a 3d77 3138 3022 3e0d 0a0d 0a0d 0a3c  sz=w180">......<
+00000aa0: 2f64 6976 3e0d 0a0d 0a23 2323 203c 6c69  /div>....### <li
+00000ab0: 3e63 746b 6368 6172 7420 6973 2061 2050  >ctkchart is a P
+00000ac0: 7974 686f 6e20 6c69 6272 6172 7920 666f  ython library fo
+00000ad0: 7220 6372 6561 7469 6e67 206c 6976 6520  r creating live 
+00000ae0: 7570 6461 7469 6e67 206c 696e 6520 6368  updating line ch
+00000af0: 6172 7473 2069 6e20 6375 7374 6f6d 746b  arts in customtk
+00000b00: 696e 7465 722e 3c2f 6c69 3e0d 0a0d 0a3c  inter.</li>....<
+00000b10: 2f64 6976 3e0d 0a0d 0a23 2320 4665 6174  /div>....## Feat
+00000b20: 7572 6573 0d0a 0d0a 2d20 2a2a 4c69 7665  ures....- **Live
+00000b30: 2055 7064 6174 652a 2a3a 2044 6973 706c   Update**: Displ
+00000b40: 6179 206c 6976 6520 6461 7461 2077 6974  ay live data wit
+00000b50: 6820 6c69 6e65 2063 6861 7274 732e 0d0a  h line charts...
+00000b60: 2d20 2a2a 4d75 6c74 6970 6c65 204c 696e  - **Multiple Lin
+00000b70: 6573 2a2a 3a20 5375 7070 6f72 7420 666f  es**: Support fo
+00000b80: 7220 706c 6f74 7469 6e67 206d 756c 7469  r plotting multi
+00000b90: 706c 6520 6c69 6e65 7320 6f6e 2074 6865  ple lines on the
+00000ba0: 2073 616d 6520 6368 6172 7420 666f 7220   same chart for 
+00000bb0: 6561 7379 2063 6f6d 7061 7269 736f 6e2e  easy comparison.
+00000bc0: 0d0a 2d20 2a2a 436f 6c6f 7220 4375 7374  ..- **Color Cust
+00000bd0: 6f6d 697a 6174 696f 6e2a 2a3a 2043 7573  omization**: Cus
+00000be0: 746f 6d69 7a65 2063 6f6c 6f72 7320 746f  tomize colors to
+00000bf0: 206d 6174 6368 2079 6f75 7220 6170 706c   match your appl
+00000c00: 6963 6174 696f 6e27 7320 6465 7369 676e  ication's design
+00000c10: 206f 7220 6461 7461 2072 6570 7265 7365   or data represe
+00000c20: 6e74 6174 696f 6e2e 0d0a 2d20 2a2a 4479  ntation...- **Dy
+00000c30: 6e61 6d69 6320 436f 6c6f 7220 4368 616e  namic Color Chan
+00000c40: 6765 2a2a 3a20 4479 6e61 6d69 6320 436f  ge**: Dynamic Co
+00000c50: 6c6f 7220 4368 616e 6765 2066 6f72 2044  lor Change for D
+00000c60: 6172 6b20 2620 4c69 6768 742e 0d0a 2d20  ark & Light...- 
+00000c70: 2a2a 466f 6e74 2043 7573 746f 6d69 7a61  **Font Customiza
+00000c80: 7469 6f6e 2a2a 3a20 4164 6a75 7374 2066  tion**: Adjust f
+00000c90: 6f6e 7473 2066 6f72 2074 6578 7420 656c  onts for text el
+00000ca0: 656d 656e 7473 2074 6f20 656e 6861 6e63  ements to enhanc
+00000cb0: 6520 7265 6164 6162 696c 6974 792e 0d0a  e readability...
+00000cc0: 2d20 2a2a 4469 6d65 6e73 696f 6e20 4375  - **Dimension Cu
+00000cd0: 7374 6f6d 697a 6174 696f 6e2a 2a3a 2043  stomization**: C
+00000ce0: 7573 746f 6d69 7a65 2063 6861 7274 2064  ustomize chart d
+00000cf0: 696d 656e 7369 6f6e 7320 746f 2066 6974  imensions to fit
+00000d00: 2076 6172 696f 7573 2064 6973 706c 6179   various display
+00000d10: 2073 697a 6573 2061 6e64 206c 6179 6f75   sizes and layou
+00000d20: 7473 2e0d 0a0d 0a23 2320 496d 706f 7274  ts.....## Import
+00000d30: 696e 6720 2620 496e 7374 616c 6c61 7469  ing & Installati
+00000d40: 6f6e 0d0a 2a20 496e 7374 616c 6c61 7469  on..* Installati
+00000d50: 6f6e 0d0a 2020 2020 6060 600d 0a20 2020  on..    ```..   
+00000d60: 2070 6970 2069 6e73 7461 6c6c 2063 746b   pip install ctk
+00000d70: 6368 6172 740d 0a20 2020 2060 6060 0d0a  chart..    ```..
+00000d80: 0d0a 2a20 496d 706f 7274 696e 670d 0a20  ..* Importing.. 
+00000d90: 2020 2020 6060 600d 0a20 2020 2069 6d70      ```..    imp
+00000da0: 6f72 7420 6374 6b63 6861 7274 0d0a 2020  ort ctkchart..  
+00000db0: 2020 6060 600d 0a0d 0a23 204c 696e 6b73    ```....# Links
+00000dc0: 0d0a 0d0a 2a2a 5669 7369 7420 4769 7448  ....**Visit GitH
+00000dd0: 7562 2066 6f72 2044 6f63 756d 656e 7461  ub for Documenta
+00000de0: 7469 6f6e 3a2a 2a0d 0a0d 0a2d 202a 2a47  tion:**....- **G
+00000df0: 6974 4875 6220 5265 706f 7369 746f 7279  itHub Repository
+00000e00: 3a2a 2a20 5b63 746b 6368 6172 745d 2868  :** [ctkchart](h
+00000e10: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000e20: 6d2f 5468 6973 616c 2d44 2f63 746b 6368  m/Thisal-D/ctkch
+00000e30: 6172 7429 0d0a                           art)..
```

### Comparing `ctkchart-2.0.2/README.md` & `ctkchart-2.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -28,69 +28,67 @@
 000001b0: 2f2f 7374 6174 6963 2e70 6570 792e 7465  //static.pepy.te
 000001c0: 6368 2f62 6164 6765 2f63 746b 6368 6172  ch/badge/ctkchar
 000001d0: 742f 7765 656b 295d 2868 7474 7073 3a2f  t/week)](https:/
 000001e0: 2f70 6570 792e 7465 6368 2f70 726f 6a65  /pepy.tech/proje
 000001f0: 6374 2f63 746b 6368 6172 7429 0a0a 3c69  ct/ctkchart)..<i
 00000200: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
 00000210: 6472 6976 652e 676f 6f67 6c65 2e63 6f6d  drive.google.com
-00000220: 2f74 6875 6d62 6e61 696c 3f69 643d 316a  /thumbnail?id=1j
-00000230: 4f6c 7454 3571 4276 4c6d 4b41 6453 5536  OltT5qBvLmKAdSU6
-00000240: 7a62 3977 6a68 3347 5961 366a 5276 4426  zb9wjh3GYa6jRvD&
-00000250: 737a 3d77 3138 3022 3e0a 0a3c 2f64 6976  sz=w180">..</div
-00000260: 3e0a 0a23 2323 203c 6c69 3e63 746b 6368  >..### <li>ctkch
-00000270: 6172 7420 6973 2061 2050 7974 686f 6e20  art is a Python 
-00000280: 6c69 6272 6172 7920 666f 7220 6372 6561  library for crea
-00000290: 7469 6e67 206c 6976 6520 7570 6461 7469  ting live updati
-000002a0: 6e67 206c 696e 6520 6368 6172 7473 2069  ng line charts i
-000002b0: 6e20 6375 7374 6f6d 746b 696e 7465 722e  n customtkinter.
-000002c0: 3c2f 6c69 3e0a 0a3c 2f64 6976 3e0a 0a23  </li>..</div>..#
-000002d0: 2320 4665 6174 7572 6573 0a0a 2d20 2a2a  # Features..- **
-000002e0: 4c69 7665 2055 7064 6174 652a 2a3a 2044  Live Update**: D
-000002f0: 6973 706c 6179 206c 6976 6520 6461 7461  isplay live data
-00000300: 2077 6974 6820 6c69 6e65 2063 6861 7274   with line chart
-00000310: 732e 0a2d 202a 2a4d 756c 7469 706c 6520  s..- **Multiple 
-00000320: 4c69 6e65 732a 2a3a 2053 7570 706f 7274  Lines**: Support
-00000330: 2066 6f72 2070 6c6f 7474 696e 6720 6d75   for plotting mu
-00000340: 6c74 6970 6c65 206c 696e 6573 206f 6e20  ltiple lines on 
-00000350: 7468 6520 7361 6d65 2063 6861 7274 2066  the same chart f
-00000360: 6f72 2065 6173 7920 636f 6d70 6172 6973  or easy comparis
-00000370: 6f6e 2e0a 2d20 2a2a 436f 6c6f 7220 4375  on..- **Color Cu
-00000380: 7374 6f6d 697a 6174 696f 6e2a 2a3a 2043  stomization**: C
-00000390: 7573 746f 6d69 7a65 2063 6f6c 6f72 7320  ustomize colors 
-000003a0: 746f 206d 6174 6368 2079 6f75 7220 6170  to match your ap
-000003b0: 706c 6963 6174 696f 6e27 7320 6465 7369  plication's desi
-000003c0: 676e 206f 7220 6461 7461 2072 6570 7265  gn or data repre
-000003d0: 7365 6e74 6174 696f 6e2e 0a2d 202a 2a44  sentation..- **D
-000003e0: 796e 616d 6963 2043 6f6c 6f72 2043 6861  ynamic Color Cha
-000003f0: 6e67 652a 2a3a 2044 796e 616d 6963 2043  nge**: Dynamic C
-00000400: 6f6c 6f72 2043 6861 6e67 6520 666f 7220  olor Change for 
-00000410: 4461 726b 2026 204c 6967 6874 2e0a 2d20  Dark & Light..- 
-00000420: 2a2a 466f 6e74 2043 7573 746f 6d69 7a61  **Font Customiza
-00000430: 7469 6f6e 2a2a 3a20 4164 6a75 7374 2066  tion**: Adjust f
-00000440: 6f6e 7473 2066 6f72 2074 6578 7420 656c  onts for text el
-00000450: 656d 656e 7473 2074 6f20 656e 6861 6e63  ements to enhanc
-00000460: 6520 7265 6164 6162 696c 6974 792e 0a2d  e readability..-
-00000470: 202a 2a44 696d 656e 7369 6f6e 2043 7573   **Dimension Cus
-00000480: 746f 6d69 7a61 7469 6f6e 2a2a 3a20 4375  tomization**: Cu
-00000490: 7374 6f6d 697a 6520 6368 6172 7420 6469  stomize chart di
-000004a0: 6d65 6e73 696f 6e73 2074 6f20 6669 7420  mensions to fit 
-000004b0: 7661 7269 6f75 7320 6469 7370 6c61 7920  various display 
-000004c0: 7369 7a65 7320 616e 6420 6c61 796f 7574  sizes and layout
-000004d0: 732e 0a0a 2323 2049 6d70 6f72 7469 6e67  s...## Importing
-000004e0: 2026 2049 6e73 7461 6c6c 6174 696f 6e0a   & Installation.
-000004f0: 2a20 496e 7374 616c 6c61 7469 6f6e 0a20  * Installation. 
-00000500: 2020 2060 6060 0a20 2020 2070 6970 2069     ```.    pip i
-00000510: 6e73 7461 6c6c 2063 746b 6368 6172 740a  nstall ctkchart.
-00000520: 2020 2020 6060 600a 0a2a 2049 6d70 6f72      ```..* Impor
-00000530: 7469 6e67 0a20 2020 2020 6060 600a 2020  ting.     ```.  
-00000540: 2020 696d 706f 7274 2063 746b 6368 6172    import ctkchar
-00000550: 740a 2020 2020 6060 600a 0a23 204c 696e  t.    ```..# Lin
-00000560: 6b73 0a0a 2d20 2a2a 5669 7369 7420 4769  ks..- **Visit Gi
-00000570: 7448 7562 2066 6f72 204d 6f72 6520 4465  tHub for More De
-00000580: 7461 696c 732e 2e2e 2e2e 2a2a 0a2d 2023  tails.....**.- #
-00000590: 2320 2a2a 4769 7448 7562 2e63 6f6d 2a2a  # **GitHub.com**
-000005a0: 2020 203a 2020 3c61 2068 7265 663d 2268     :  <a href="h
-000005b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000005c0: 6d2f 5468 6973 616c 2d44 2f63 746b 6368  m/Thisal-D/ctkch
-000005d0: 6172 7422 2074 6172 6765 743d 225f 626c  art" target="_bl
-000005e0: 616e 6b22 203e 3c69 3e63 746b 6368 6172  ank" ><i>ctkchar
-000005f0: 743c 2f69 3e3c 2f61 3e0a                 t</i></a>.
+00000220: 2f74 6875 6d62 6e61 696c 3f69 643d 3163  /thumbnail?id=1c
+00000230: 4872 7346 494c 484a 3761 3262 674d 5876  HrsFILHJ7a2bgMXv
+00000240: 6b2d 5057 6c6e 4c5a 7831 7643 6e56 5226  k-PWlnLZx1vCnVR&
+00000250: 737a 3d77 3138 3022 3e0a 0a0a 3c2f 6469  sz=w180">...</di
+00000260: 763e 0a0a 2323 2320 3c6c 693e 6374 6b63  v>..### <li>ctkc
+00000270: 6861 7274 2069 7320 6120 5079 7468 6f6e  hart is a Python
+00000280: 206c 6962 7261 7279 2066 6f72 2063 7265   library for cre
+00000290: 6174 696e 6720 6c69 7665 2075 7064 6174  ating live updat
+000002a0: 696e 6720 6c69 6e65 2063 6861 7274 7320  ing line charts 
+000002b0: 696e 2063 7573 746f 6d74 6b69 6e74 6572  in customtkinter
+000002c0: 2e3c 2f6c 693e 0a0a 3c2f 6469 763e 0a0a  .</li>..</div>..
+000002d0: 2323 2046 6561 7475 7265 730a 0a2d 202a  ## Features..- *
+000002e0: 2a4c 6976 6520 5570 6461 7465 2a2a 3a20  *Live Update**: 
+000002f0: 4469 7370 6c61 7920 6c69 7665 2064 6174  Display live dat
+00000300: 6120 7769 7468 206c 696e 6520 6368 6172  a with line char
+00000310: 7473 2e0a 2d20 2a2a 4d75 6c74 6970 6c65  ts..- **Multiple
+00000320: 204c 696e 6573 2a2a 3a20 5375 7070 6f72   Lines**: Suppor
+00000330: 7420 666f 7220 706c 6f74 7469 6e67 206d  t for plotting m
+00000340: 756c 7469 706c 6520 6c69 6e65 7320 6f6e  ultiple lines on
+00000350: 2074 6865 2073 616d 6520 6368 6172 7420   the same chart 
+00000360: 666f 7220 6561 7379 2063 6f6d 7061 7269  for easy compari
+00000370: 736f 6e2e 0a2d 202a 2a43 6f6c 6f72 2043  son..- **Color C
+00000380: 7573 746f 6d69 7a61 7469 6f6e 2a2a 3a20  ustomization**: 
+00000390: 4375 7374 6f6d 697a 6520 636f 6c6f 7273  Customize colors
+000003a0: 2074 6f20 6d61 7463 6820 796f 7572 2061   to match your a
+000003b0: 7070 6c69 6361 7469 6f6e 2773 2064 6573  pplication's des
+000003c0: 6967 6e20 6f72 2064 6174 6120 7265 7072  ign or data repr
+000003d0: 6573 656e 7461 7469 6f6e 2e0a 2d20 2a2a  esentation..- **
+000003e0: 4479 6e61 6d69 6320 436f 6c6f 7220 4368  Dynamic Color Ch
+000003f0: 616e 6765 2a2a 3a20 4479 6e61 6d69 6320  ange**: Dynamic 
+00000400: 436f 6c6f 7220 4368 616e 6765 2066 6f72  Color Change for
+00000410: 2044 6172 6b20 2620 4c69 6768 742e 0a2d   Dark & Light..-
+00000420: 202a 2a46 6f6e 7420 4375 7374 6f6d 697a   **Font Customiz
+00000430: 6174 696f 6e2a 2a3a 2041 646a 7573 7420  ation**: Adjust 
+00000440: 666f 6e74 7320 666f 7220 7465 7874 2065  fonts for text e
+00000450: 6c65 6d65 6e74 7320 746f 2065 6e68 616e  lements to enhan
+00000460: 6365 2072 6561 6461 6269 6c69 7479 2e0a  ce readability..
+00000470: 2d20 2a2a 4469 6d65 6e73 696f 6e20 4375  - **Dimension Cu
+00000480: 7374 6f6d 697a 6174 696f 6e2a 2a3a 2043  stomization**: C
+00000490: 7573 746f 6d69 7a65 2063 6861 7274 2064  ustomize chart d
+000004a0: 696d 656e 7369 6f6e 7320 746f 2066 6974  imensions to fit
+000004b0: 2076 6172 696f 7573 2064 6973 706c 6179   various display
+000004c0: 2073 697a 6573 2061 6e64 206c 6179 6f75   sizes and layou
+000004d0: 7473 2e0a 0a23 2320 496d 706f 7274 696e  ts...## Importin
+000004e0: 6720 2620 496e 7374 616c 6c61 7469 6f6e  g & Installation
+000004f0: 0a2a 2049 6e73 7461 6c6c 6174 696f 6e0a  .* Installation.
+00000500: 2020 2020 6060 600a 2020 2020 7069 7020      ```.    pip 
+00000510: 696e 7374 616c 6c20 6374 6b63 6861 7274  install ctkchart
+00000520: 0a20 2020 2060 6060 0a0a 2a20 496d 706f  .    ```..* Impo
+00000530: 7274 696e 670a 2020 2020 2060 6060 0a20  rting.     ```. 
+00000540: 2020 2069 6d70 6f72 7420 6374 6b63 6861     import ctkcha
+00000550: 7274 0a20 2020 2060 6060 0a0a 2320 4c69  rt.    ```..# Li
+00000560: 6e6b 730a 0a2a 2a56 6973 6974 2047 6974  nks..**Visit Git
+00000570: 4875 6220 666f 7220 446f 6375 6d65 6e74  Hub for Document
+00000580: 6174 696f 6e3a 2a2a 0a0a 2d20 2a2a 4769  ation:**..- **Gi
+00000590: 7448 7562 2052 6570 6f73 6974 6f72 793a  tHub Repository:
+000005a0: 2a2a 205b 6374 6b63 6861 7274 5d28 6874  ** [ctkchart](ht
+000005b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000005c0: 2f54 6869 7361 6c2d 442f 6374 6b63 6861  /Thisal-D/ctkcha
+000005d0: 7274 29                                  rt)
```

### Comparing `ctkchart-2.0.2/pyproject.toml` & `ctkchart-2.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 00000010: 7265 7175 6972 6573 203d 205b 2273 6574  requires = ["set
 00000020: 7570 746f 6f6c 7322 2c20 2277 6865 656c  uptools", "wheel
 00000030: 225d 0d0a 6275 696c 642d 6261 636b 656e  "]..build-backen
 00000040: 6420 3d20 2273 6574 7570 746f 6f6c 732e  d = "setuptools.
 00000050: 6275 696c 645f 6d65 7461 220d 0a0d 0a5b  build_meta"....[
 00000060: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000070: 2022 6374 6b63 6861 7274 220d 0a76 6572   "ctkchart"..ver
-00000080: 7369 6f6e 203d 2022 322e 302e 3222 0d0a  sion = "2.0.2"..
+00000080: 7369 6f6e 203d 2022 322e 302e 3322 0d0a  sion = "2.0.3"..
 00000090: 6175 7468 6f72 7320 3d20 5b0d 0a20 207b  authors = [..  {
 000000a0: 206e 616d 6520 3d20 2254 6869 7361 6c2d   name = "Thisal-
 000000b0: 4422 207d 0d0a 5d0d 0a0d 0a6c 6963 656e  D" }..]....licen
 000000c0: 7365 203d 207b 2066 696c 6520 3d20 224c  se = { file = "L
 000000d0: 4943 454e 5345 2220 7d0d 0a0d 0a64 6573  ICENSE" }....des
 000000e0: 6372 6970 7469 6f6e 203d 2022 6374 6b63  cription = "ctkc
 000000f0: 6861 7274 2069 7320 6120 5079 7468 6f6e  hart is a Python
```

### Comparing `ctkchart-2.0.2/src/ctkchart/CTkLine.py` & `ctkchart-2.0.3/src/ctkchart/CTkLine.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import Union, Tuple
+from typing import Union, Tuple, Literal
 from .Validate import Validate
 from .FontStyle import FontStyle
 
 
 class CTkLine():
    def __init__(self,
                master: any = None,
                color: Union[Tuple[str, str], str] = ("#768df1", "#768df1"),
                size: int = 1,
-               style: str = "normal", 
+               style: Literal["normal", "dashed", "dotted"] = "normal", 
                style_type: Tuple[int, int] = (4,4),
-               point_highlight: str = "disabled",
+               point_highlight: Literal["enabled", "disabled"] = "disabled",
                point_highlight_size: int = 8,
                point_highlight_color: Union[Tuple[str, str], str] = ("#768df1", "#768df1"),
-               fill: str = "disabled",
+               fill: Literal["enabled", "disabled"] = "disabled",
                fill_color: Union[Tuple[str, str], str] = ("#bdc6ed", "#5d6db6"),
                *args: any
                ) -> None:
       """
       Initialize a CTkLine object.
 
          Args:
@@ -54,33 +54,34 @@
       self.__color = color
       self.__size = size
       self.__y_end = 0
       self.__x_end  = self.__master._CTkLineChart__x_axis_point_spacing* -1
       self.__data = []
       self.__temp_data = []
       self.__ret_data = []
-      self.__hide_state = False
+      self.__visibility = self.__master._CTkLineChart__visibility
       self.__style = style
       self.__style_type = style_type
       self.__point_highlight = point_highlight
       self.__point_highlight_size = point_highlight_size
       self.__point_highlight_color = point_highlight_color
       self.__fill = fill
       self.__fill_color = fill_color
 
+      self.__master._CTkLineChart__lines.append(self)
 
    def configure(self, 
                   color: Union[Tuple[str, str], str] = None, 
                   size: int = None,
-                  style: str = None,
+                  style: Literal["normal", "dashed", "dotted"] = None,
                   style_type: Tuple[int, int] = None,
-                  point_highlight: str = None,
+                  point_highlight: Literal["enabled", "disabled"] = None,
                   point_highlight_size: int = None,
                   point_highlight_color: Union[Tuple[str, str], str] = None,
-                  fill: str = None,
+                  fill: Literal["enabled", "disabled"] = None,
                   fill_color: Union[Tuple[str, str], str] = None,
                  ) -> None:
       """
       Configure attributes of the CTkLine object.
 
          Args:
             color (Union[Tuple[str, str], str]): The color of the line.
@@ -150,24 +151,39 @@
       Reset the CTkLine object.
       """
       
       self.__y_end = 0
       self.__x_end  = self.__master._CTkLineChart__x_axis_point_spacing* -1
       self.__data = []
       
-   
+      
    def reset(self) -> None:
       """
       Reset the line.
       """
       self.__reset()
       self.__master._CTkLineChart__call_reshow_data()
       
       
-   def cget(self, attribute_name: str) -> any:
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
+         self.__master._CTkLineChart__call_reshow_data()
+         
+   
+   def cget(self, attribute_name: Literal["master", "color", "size", "style", "style_type",
+                                          "point_highlight", "point_highlight_size", "point_highlight_color",
+                                          "fill", "fill_color", "__all__"]) -> any:
       """
       Get the value of a CTkLine attribute.
 
          Args:
                attribute_name (str): Name of the attribute.
 
          Returns:
@@ -195,8 +211,18 @@
          "point_highlight" : self.__point_highlight,
          "point_highlight_size" : self.__point_highlight_size,
          "point_highlight_color" : self.__point_highlight_color,
          "fill" : self.__fill,
          "fill_color" : self.__fill_color
          }
          
-      Validate._invalidCget(attribute_name)
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

### Comparing `ctkchart-2.0.2/src/ctkchart/CTkLineChart.py` & `ctkchart-2.0.3/src/ctkchart/CTkLineChart.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import customtkinter
 import tkinter
-from typing import Union, List, Tuple
+from typing import Union, List, Tuple, Literal
 from .Utils import Utils
 from .CTkLine import CTkLine
 from .Validate import Validate
 
 
 class CTkLineChart():
    def __init__(self, master: any = None,
@@ -20,41 +20,41 @@
 
                   y_axis_precision: int = 0,
                   y_axis_data: any = "Y",
                   y_axis_label_count: int = 1,
                   y_axis_values: Tuple[Union[int, float], Union[int, float]] = (None, None),
                   y_axis_font_color: Union[Tuple[str, str], str] = ("#AAAAAA", "#606060"),
                   y_axis_data_font_color: Union[Tuple[str, str], str] = ("#999999", "#707070"),
-                  y_axis_data_position: str = "top",
+                  y_axis_data_position: Literal["top", "side"] = "top",
                   y_axis_section_count: int = 0,
-                  y_axis_section_style: str = "normal",
+                  y_axis_section_style: Literal["normal", "dashed"] = "normal",
                   y_axis_section_style_type: Tuple[int, int] = (100, 50),
                   y_axis_section_color: Union[Tuple[str, str], str] = ("#EBEBEB", "#2C2C2C"),
 
                   x_axis_data: str = "X",
                   x_axis_label_count: int = None,
                   x_axis_values: Tuple[any, ...] = (None, "None", None, "None"),
                   x_axis_display_values_indices: Tuple[int, ...] = None,
                   x_axis_font_color: Union[Tuple[str, str], str] = ("#AAAAAA", "#606060"),
                   x_axis_data_font_color: Union[Tuple[str, str], str] = ("#999999", "#707070"),
-                  x_axis_data_position: str = "top",
+                  x_axis_data_position: Literal["top", "side"] = "top",
                   x_axis_section_count: int = 0,
-                  x_axis_section_style: str = "normal",
+                  x_axis_section_style: Literal["normal", "dashed"] = "normal",
                   x_axis_section_style_type: Tuple[int, int] = (100, 50),
                   x_axis_section_color: Union[Tuple[str, str], str] = ("#ebebeb", "#2c2c2c"),
 
-                  x_axis_point_spacing: Union[int, str] = "auto",
+                  x_axis_point_spacing: Union[int, Literal["auto"]] = "auto",
                   y_space: int = 0,
                   x_space: int = 0,
 
-                  pointer_state: str = "disabled",
+                  pointer_state: Literal["enabled", "disabled"] = "disabled",
                   pointing_callback_function: callable = None,
                   pointer_color: Union[Tuple[str, str], str] = ("#CCCCCC", "#606060"),
                   pointing_values_precision: int = 1,
-                  pointer_lock: str = "disabled",
+                  pointer_lock: Literal["enabled", "disabled"] = "disabled",
                   pointer_size: int = 1,
                   
                   *args: any,
                   ) -> None:
       """
       Initialize the CTkLineChart.
 
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
       
       self.__theme = "unknown"
       self.__margin = 10
 
       self.__create_widgets()
       self.__configure_required_widget_size()
       self.__configure_x_axis_labels_info()
@@ -276,15 +278,18 @@
          Internal loop to track theme changes and update the widget appearance.
          """
          
          if self.__theme !=  customtkinter.get_appearance_mode():
             self.__theme = customtkinter.get_appearance_mode()
             self.__configure_widget_for_theme_changes()
             self.__call_reshow_data()
-         self.master.after(1000,__track_theme_changes_loop)
+         try:
+            self.master.after(1000,__track_theme_changes_loop)
+         except AttributeError:
+            Validate._invalidMaster(self.master)
       __track_theme_changes_loop()
       
       
    def __configure_widget_for_theme_changes(self) -> None:
       """
       Configure the widget appearance to match changes in the theme.
 
@@ -303,22 +308,22 @@
 
          This method initializes the main frame along with frames for the y-axis, x-axis, 
          y-axis values, x-axis values, y-axis data label, x-axis data label, output frame,
          output canvas, and pointer.
       """
       
       self.__main_frame = customtkinter.CTkFrame(master=self.master)
-      self.__y_axis_frame = tkinter.Frame(master=self.__main_frame)
-      self.__x_axis_frame = tkinter.Frame(master=self.__main_frame)
       self.__x_axis_values_frame = customtkinter.CTkFrame(master=self.__main_frame)
       self.__y_axis_values_frame = customtkinter.CTkFrame(master=self.__main_frame)
       self.__y_axis_data_label = customtkinter.CTkLabel(master=self.__main_frame)
       self.__x_axis_data_label = customtkinter.CTkLabel(master=self.__main_frame)
       self.__output_frame = customtkinter.CTkFrame(master=self.__main_frame)
       self.__output_canvas = tkinter.Canvas(master=self.__output_frame, highlightthickness=0)
+      self.__y_axis_frame = tkinter.Frame(master=self.__main_frame)
+      self.__x_axis_frame = tkinter.Frame(master=self.__main_frame)
       self.__pointer = tkinter.Frame(master=self.__output_canvas)
       
    
    def __set_pointer_state(self) -> None:
       """
       Set the state of the pointer.
 
@@ -414,49 +419,60 @@
          based on the specified dimensions and positions.
       """
       
       self.__main_frame.configure(width=self.__width, height=self.__height)
       
       self.__y_axis_data_label.place_forget()
       self.__x_axis_data_label.place_forget()
-      if self.__y_axis_data_position=="top":
-         self.__y_axis_data_label.place(x=self.__margin, y=0)
-      else:
-         self.__y_axis_data_label.place(x=self.__margin, y=self.__y_space+self.__y_special_height_space+self.__real_height/2,anchor="w")
-      if self.__x_axis_data_position=="top":
-         self.__x_axis_data_label.place(rely=1, relx=1, x=-self.__x_axis_data_req_width+-self.__margin, y=-self.__x_axis_data_req_height)
-      else:
-         self.__x_axis_data_label.place(rely=1, y=-self.__x_axis_data_req_height, relx=0, anchor="n",
-                                  x=(self.__real_width/2)+self.__y_axis_data_req_width_space_side+self.__y_value_req_width_space+self.__axis_size+self.__x_axis_data_req_width_space_top+self.__x_special_width_space+self.__margin)
+      if self.__y_axis_data != "":
+         if self.__y_axis_data_position=="top":
+            self.__y_axis_data_label.place(x=self.__margin, y=0)
+         else:
+            self.__y_axis_data_label.place(x=self.__margin, y=self.__y_space+self.__y_special_height_space+self.__real_height/2,anchor="w")
+      
+      if self.__x_axis_data != "":
+         if self.__x_axis_data_position=="top":
+            self.__x_axis_data_label.place(rely=1, relx=1, x=-self.__x_axis_data_req_width+-self.__margin, y=-self.__x_axis_data_req_height)
+         else:
+            self.__x_axis_data_label.place(rely=1, y=-self.__x_axis_data_req_height, relx=0, anchor="n",
+                                    x=(self.__real_width/2)+self.__y_axis_data_req_width_space_side+self.__y_value_req_width_space+self.__axis_size+self.__x_axis_data_req_width_space_top+self.__x_special_width_space+self.__margin)
       
       self.__y_axis_frame.configure(width=self.__axis_size)
       self.__x_axis_frame.configure(height=self.__axis_size)
 
       self.__y_axis_frame.place(x=self.__y_value_req_width_space+self.__y_axis_data_req_width_space_side+self.__margin,
                          y=float(self.__y_axis_data_req_height_space_top+(self.__y_value_req_height_space/2)+self.__y_special_height_space),
                          )
       self.__y_axis_frame.configure(height=self.__const_real_height+self.__y_space+self.__axis_size)
       self.__x_axis_frame.place(x=self.__y_value_req_width_space+self.__y_axis_data_req_width_space_side+self.__margin,
                               rely=1,
                               y=-self.__axis_size+-self.__x_value_req_height_space+-self.__x_axis_data_req_height_space_side,
                               )
+      
       self.__x_axis_frame.configure(width=self.__const_real_width+self.__axis_size+self.__x_space)
       
       self.__output_frame.place(x=self.__y_value_req_width_space+self.__axis_size+self.__y_axis_data_req_width_space_side+self.__margin,
                                 y=float(self.__y_axis_data_req_height_space_top+(self.__y_value_req_height_space/2)+self.__y_special_height_space+self.__y_space))
       self.__output_frame.configure( width=self.__const_real_width,
                                 height=self.__const_real_height,)
       
       self.__output_canvas.place(y=0, x=0)
       self.__output_canvas.configure(height=self.__const_real_height, width=self.__const_real_width)
       
-      self.__y_axis_values_frame.place(x=self.__y_axis_data_req_width_space_side+self.__margin)
-      self.__y_axis_values_frame.configure(width=self.__y_value_req_width_space, height=self.__height)
-      self.__x_axis_values_frame.place(x=self.__margin, rely=1, y=-self.__x_value_req_height_space+-self.__x_axis_data_req_height_space_side)
-      self.__x_axis_values_frame.configure(height=self.__x_value_req_height_space, width=self.__width-(self.__margin*2))
+      if self.__y_values_frame_place_req:
+         self.__y_axis_values_frame.place(x=self.__y_axis_data_req_width_space_side+self.__margin)
+         self.__y_axis_values_frame.configure(width=self.__y_value_req_width_space, height=self.__height)
+      else:
+         self.__y_axis_values_frame.place_forget()
+         
+      if self.__x_values_frame_place_req:
+         self.__x_axis_values_frame.place(x=self.__margin, rely=1, y=-self.__x_value_req_height_space+-self.__x_axis_data_req_height_space_side)
+         self.__x_axis_values_frame.configure(height=self.__x_value_req_height_space, width=self.__width-(self.__margin*2))
+      else:
+         self.__x_axis_values_frame.place_forget()
 
 
    def __configure_x_axis_point_spacing(self) -> None:
       """
       Configure the spacing between points on the x-axis.
 
          This method calculates and sets the spacing between points on the x-axis based on the 
@@ -476,56 +492,72 @@
       Configure the required sizes of the LineChart's widgets.
 
          This method calculates and sets the required sizes for various widgets in the LineChart,
          such as axis labels, based on the provided data and styling options. It determines the
          necessary space for displaying the data labels, axis values, and adjusts the real width
          and height of the LineChart accordingly.
       """
-    
+      
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
+      
+      if self.__y_value_req_height_space/2 > self.__x_value_req_height_space:
+         self.__x_value_req_height_space = self.__y_value_req_height_space/2
       
       self.__real_width = self.__width - (self.__y_value_req_width_space+self.__axis_size+self.__x_axis_data_req_width_space_top+self.__y_axis_data_req_width_space_side+\
-                                          (self.__x_value_req_width_space/2)+self.__x_special_width_space+self.__x_space) - (self.__margin*2)
+                                          (self.__x_value_req_width_space/2)+self.__x_special_width_space+self.__x_space+self.__margin*2)
       
       self.__const_real_width = self.__real_width 
       self.__real_height = self.__height - (self.__y_axis_data_req_height_space_top+self.__axis_size+self.__x_value_req_height_space+self.__x_axis_data_req_height_space_side+\
                                           (self.__y_value_req_height_space/2)+self.__y_special_height_space+self.__y_space)
       self.__real_height = self.__real_height  
       
       self.__const_real_height = int(self.__real_height)
@@ -719,27 +751,26 @@
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
          
       elif self.__x_axis_values_handle_by=="label_count":
          if self.__x_axis_label_count == 0:
             return
+         if self.__x_axis_label_count == None:
+            self.__x_axis_label_count = len(self.__x_axis_values)
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
 
@@ -818,52 +849,52 @@
             widget.destroy()
                
          
    def configure(self,
                   width: int = None,
                   height: int = None,
                   axis_size: int = None,
-                  x_axis_point_spacing: Union[int, str] = None, 
+                  x_axis_point_spacing: Union[int, Literal["auto"]] = None, 
                   
                   fg_color: Union[Tuple[str, str], str] = None,
                   axis_color: Union[Tuple[str, str], str] = None,
                   bg_color: Union[Tuple[str, str], str] = None,
                   data_font_style: Tuple[str, int, str] = None,
                   axis_font_style: Tuple[str, int, str] = None,
             
                   y_axis_values: Union[int, float]=None,
                   y_axis_precision: int = None,
                   y_axis_font_color: Union[Tuple[str, str], str] = None,
                   y_axis_data_font_color: Union[Tuple[str, str], str] = None,
                   y_axis_section_count: int = None,
                   y_axis_section_color: Union[Tuple[str, str], str] = None,
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
                   x_axis_font_color: Union[Tuple[str, str], str] = None,
                   x_axis_data_font_color: Union[Tuple[str, str], str] = None,
                   x_axis_label_count: int = None,
                   x_axis_section_count: int = None,
-                  x_axis_section_style: str = None,
+                  x_axis_section_style: Literal["normal", "dashed"] = None,
                   x_axis_section_style_type: Tuple[int, int] = None,
                   x_axis_section_color: Union[Tuple[str, str], str] = None,
                   x_axis_display_values_indices: Tuple[int, ...] = None,
-                  x_axis_data_position: str = None,
+                  x_axis_data_position: Literal["top", "side"] = None,
                   x_space: int = None ,
                   
-                  pointer_state: str = None,
+                  pointer_state: Literal["enabled", "disabled"] = None,
                   pointing_values_precision: int = None,
                   pointer_color: Union[Tuple[str, str], str] = None, 
-                  pointer_lock: str = None,
+                  pointer_lock: Literal["enabled", "disabled"] = None,
                   pointing_callback_function: callable = None, 
                   pointer_size: int = None
                   ) -> None:
       
       """
       Configures the properties of the chart widget based on the provided arguments.
       
@@ -914,15 +945,14 @@
             pointer_size: The size of the pointer.
       """
          
       chart_reset_req = False
       widget_color_change_req = False
       widget_size_change_req = False
       widget_font_change_req = False
-      chart_y_values_change_req = False
       chart_x_values_change_req = False
       chart_sections_change_req = False
       chart_sections_color_change_req = False
       chart_x_labels_change_req = False
       chart_y_labels_change_req = False
       pointer_state_change_req = False
       pointer_size_change_req = False
@@ -1132,14 +1162,16 @@
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
@@ -1216,15 +1248,15 @@
          self.__set_x_axis_values()
          
       if chart_sections_change_req or chart_sections_color_change_req:
          self.__destroy_x_y_sections()
          self.__create_y_axis_sections()
          self.__create_x_axis_sections()
             
-      if widget_color_change_req :
+      if widget_color_change_req : 
          self.__set_customtkinter_widgets_colors()
          self.__set_tkinter_widgets_colors()
       
       if widget_size_change_req == True:
          self.__set_pointer_size()
          
       if reshow_data_req:
@@ -1340,28 +1372,32 @@
       """
       Show data on the chart for the given line.
 
          Args:
             line (Line): The line object to which the data belongs.
             data (List[Union[int, float]]): The list of data points to be displayed.
 
+         Raises:
+            ValueError: If the provided line object is not valid or not found in the chart.
+         
          This method adds the provided data to the line's existing data, adjusts the display of the chart accordingly,
          and shows the data points on the chart. It also handles various styles for displaying the data points,
          such as dashed or dotted lines, and highlights for individual data points.
       """
       
       Validate._isValidCTkLine(line, "line")
       Validate._isValidData(data, "data")
       
       re_show_data = False
       if line not in self.__lines:
-         self.__lines.append(line)
+         Validate._invalidLine(line)
+      
       line._CTkLine__data += data
       
-      if line._CTkLine__hide_state != True :
+      if line._CTkLine__visibility:
          
          line_color = self.__get_color_by_theme(line._CTkLine__color)
          highlight_color = self.__get_color_by_theme(line._CTkLine__point_highlight_color)
          fill_color = self.__get_color_by_theme(line._CTkLine__fill_color)
          
          for d in data:
             self.__is_data_showing_working = True
@@ -1580,15 +1616,15 @@
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
@@ -1606,16 +1642,16 @@
       
       
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
@@ -1638,15 +1674,15 @@
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
@@ -1671,122 +1707,129 @@
       
    def place_forget(self) -> None:
       """
       Remove the widget from the grid.
       """
       
       self.__main_frame.place_forget()
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
-      
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
+      self.__grid_info_column = None
+      self.__grid_info_columnspan = None
+      self.__grid_info_padx = None
+      self.__grid_info_pady = None
+      self.__grid_info_row = None
+      self.__grid_info_rowspan = None
+      self.__grid_info_sticky = None
       
       
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
-                             padx=self.__grid_info_padx,  pady=self.__grid_info_pady,
-                             row=self.__grid_info_row, rowspan=self.__grid_info_rowspan, sticky=self.__grid_info_sticky)
-      
-      
-   def hide(self, line: CTkLine, state: bool) -> None:
+   def set_line_visibility(self, line: CTkLine, state: bool) -> None:
       """
       Hide or show a specific line.
 
          Args:
             line (Line): The line object to hide or show.
             state (bool): The hide/show state of the line.
       """
       
       Validate._isValidCTkLine(line, "line")
       Validate._isBool(state, "state")
-      if line._CTkLine__hide_state != state:
-         line._CTkLine__hide_state = state
+      if line._CTkLine__visibility != state or self.__visibility != state:
+         line._CTkLine__visibility = state
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
-         line._CTkLine__hide_state = state
+         line._CTkLine__visibility = state
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
@@ -1818,46 +1861,163 @@
       if attribute_name == "pointer_color": return self.__pointer_color
       if attribute_name == "pointing_values_precision": return self.__pointing_values_precision
       if attribute_name == "pointer_lock": return self.__pointer_lock
       if attribute_name == "pointer_size": return self.__pointer_size
       
       if attribute_name == "__all__":
          return {
-            "axis_color" : self.__axis_color,
-            "bg_color" : self.__bg_color,
-            "fg_color" : self.__fg_color,
-            "data_font_style" : self.__data_font_style,
-            "axis_font_style" : self.__axis_font_style,
-            "y_axis_precision" : self.__y_axis_precision,
-            "y_axis_data" : self.__y_axis_data,
-            "y_axis_label_count" : self.__y_axis_label_count,
-            "y_axis_values" : self.__y_axis_values,
-            "y_axis_font_color" : self.__y_axis_font_color,
-            "y_axis_data_font_color" : self.__y_axis_data_font_color,
-            "y_axis_data_position" : self.__y_axis_data_position,
-            "y_axis_section_count" : self.__y_axis_section_count,
-            "y_axis_section_style" : self.__y_axis_section_style,
+            "width": self.__width,
+            "height": self.__height,
+            "axis_color": self.__axis_color,
+            "bg_color": self.__bg_color,
+            "fg_color": self.__fg_color,
+            "data_font_style": self.__data_font_style,
+            "axis_font_style": self.__axis_font_style,
+            "y_axis_precision": self.__y_axis_precision,
+            "y_axis_data": self.__y_axis_data,
+            "y_axis_label_count": self.__y_axis_label_count,
+            "y_axis_values": self.__y_axis_values,
+            "y_axis_font_color": self.__y_axis_font_color,
+            "y_axis_data_font_color": self.__y_axis_data_font_color,
+            "y_axis_data_position": self.__y_axis_data_position,
+            "y_axis_section_count": self.__y_axis_section_count,
+            "y_axis_section_style": self.__y_axis_section_style,
             "y_axis_section_style_type" : self.__y_axis_section_style_type,
-            "y_axis_section_color" : self.__y_axis_section_color,
-            "x_axis_data" : self.__x_axis_data,
-            "x_axis_label_count" : self.__x_axis_label_count,
-            "x_axis_values" : self.__x_axis_values,
-            "x_axis_display_values_indices" : self.__x_axis_display_values_indices,
-            "x_axis_font_color" : self.__x_axis_font_color,
-            "x_axis_data_font_color" : self.__x_axis_data_font_color,
-            "x_axis_data_position" : self.__x_axis_data_position,
-            "x_axis_section_count" : self.__x_axis_section_count,
-            "x_axis_section_style" : self.__x_axis_section_style,
-            "x_axis_section_style_type" : self.__x_axis_section_style_type,
-            "x_axis_section_color" : self.__x_axis_section_color,
-            "x_axis_point_spacing" : self.__x_axis_point_spacing,
-            "y_space" : self.__y_space,
-            "x_space" : self.__x_space,
-            "pointer_state" : self.__pointer_state,
-            "pointing_callback_function" : self.__pointing_callback_function,
-            "pointer_color" : self.__pointer_color,
-            "pointing_values_precision" : self.__pointing_values_precision,
-            "pointer_lock" : self.__pointer_lock,
-            "pointer_size" : self.__pointer_size
+            "y_axis_section_color": self.__y_axis_section_color,
+            "x_axis_data": self.__x_axis_data,
+            "x_axis_label_count": self.__x_axis_label_count,
+            "x_axis_values": self.__x_axis_values,
+            "x_axis_display_values_indices": self.__x_axis_display_values_indices,
+            "x_axis_font_color": self.__x_axis_font_color,
+            "x_axis_data_font_color": self.__x_axis_data_font_color,
+            "x_axis_data_position": self.__x_axis_data_position,
+            "x_axis_section_count": self.__x_axis_section_count,
+            "x_axis_section_style": self.__x_axis_section_style,
+            "x_axis_section_style_type": self.__x_axis_section_style_type,
+            "x_axis_section_color": self.__x_axis_section_color,
+            "x_axis_point_spacing": self.__x_axis_point_spacing,
+            "y_space": self.__y_space,
+            "x_space": self.__x_space,
+            "pointer_state": self.__pointer_state,
+            "pointing_callback_function": self.__pointing_callback_function,
+            "pointer_color": self.__pointer_color,
+            "pointing_values_precision": self.__pointing_values_precision,
+            "pointer_lock": self.__pointer_lock,
+            "pointer_size": self.__pointer_size
             }
          
-      Validate._invalidCget(attribute_name)
+      Validate._invalidCget(attribute_name)
+
+   
+   def get_line_visibility(self, line: CTkLine):
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
+         return line._CTkLine__visibility;
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
+      Validate._invalidCget(attribute_name)
+
```

### Comparing `ctkchart-2.0.2/src/ctkchart/FontStyle.py` & `ctkchart-2.0.3/src/ctkchart/FontStyle.py`

 * *Files identical despite different names*

### Comparing `ctkchart-2.0.2/src/ctkchart/Utils.py` & `ctkchart-2.0.3/src/ctkchart/Utils.py`

 * *Files identical despite different names*

### Comparing `ctkchart-2.0.2/src/ctkchart/Validate.py` & `ctkchart-2.0.3/src/ctkchart/Validate.py`

 * *Files 2% similar despite different names*

```diff
@@ -284,9 +284,21 @@
             raise TypeError(
                 f'''{Validate._var_font(var)} {Validate._error_font("all values should be int.")}'''
             )
             
     
     def _invalidCget(var: str) -> None:
         raise TypeError(
-                f'''{Validate._var_font(var)} {Validate._error_font("Invalid attribute.")}'''
+                f'''{Validate._var_font(str(var))} {Validate._error_font("Invalid attribute.")}'''
+            )
+        
+    
+    def _invalidLine(line) -> None:
+        raise ValueError(
+                f'''{Validate._var_font(str(line))} {Validate._error_font("The line is not part of this line chart.")}'''
+            )
+        
+        
+    def  _invalidMaster(value):
+        raise ValueError(
+                f'''{Validate._var_font(str(value))} {Validate._error_font("Invalid Master for chart.")}'''
             )
```

### Comparing `ctkchart-2.0.2/src/ctkchart.egg-info/PKG-INFO` & `ctkchart-2.0.3/src/ctkchart.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2063 746b  : 2.1..Name: ctk
 00000020: 6368 6172 740d 0a56 6572 7369 6f6e 3a20  chart..Version: 
-00000030: 322e 302e 320d 0a53 756d 6d61 7279 3a20  2.0.2..Summary: 
+00000030: 322e 302e 330d 0a53 756d 6d61 7279 3a20  2.0.3..Summary: 
 00000040: 6374 6b63 6861 7274 2069 7320 6120 5079  ctkchart is a Py
 00000050: 7468 6f6e 206c 6962 7261 7279 2066 6f72  thon library for
 00000060: 2063 7265 6174 696e 6720 6c69 7665 2075   creating live u
 00000070: 7064 6174 696e 6720 6c69 6e65 2063 6861  pdating line cha
 00000080: 7274 7320 696e 2063 7573 746f 6d74 6b69  rts in customtki
 00000090: 6e74 6572 2e0d 0a41 7574 686f 723a 2054  nter...Author: T
 000000a0: 6869 7361 6c2d 440d 0a4c 6963 656e 7365  hisal-D..License
@@ -160,71 +160,69 @@
 000009f0: 7374 6174 6963 2e70 6570 792e 7465 6368  static.pepy.tech
 00000a00: 2f62 6164 6765 2f63 746b 6368 6172 742f  /badge/ctkchart/
 00000a10: 7765 656b 295d 2868 7474 7073 3a2f 2f70  week)](https://p
 00000a20: 6570 792e 7465 6368 2f70 726f 6a65 6374  epy.tech/project
 00000a30: 2f63 746b 6368 6172 7429 0d0a 0d0a 3c69  /ctkchart)....<i
 00000a40: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
 00000a50: 6472 6976 652e 676f 6f67 6c65 2e63 6f6d  drive.google.com
-00000a60: 2f74 6875 6d62 6e61 696c 3f69 643d 316a  /thumbnail?id=1j
-00000a70: 4f6c 7454 3571 4276 4c6d 4b41 6453 5536  OltT5qBvLmKAdSU6
-00000a80: 7a62 3977 6a68 3347 5961 366a 5276 4426  zb9wjh3GYa6jRvD&
-00000a90: 737a 3d77 3138 3022 3e0d 0a0d 0a3c 2f64  sz=w180">....</d
-00000aa0: 6976 3e0d 0a0d 0a23 2323 203c 6c69 3e63  iv>....### <li>c
-00000ab0: 746b 6368 6172 7420 6973 2061 2050 7974  tkchart is a Pyt
-00000ac0: 686f 6e20 6c69 6272 6172 7920 666f 7220  hon library for 
-00000ad0: 6372 6561 7469 6e67 206c 6976 6520 7570  creating live up
-00000ae0: 6461 7469 6e67 206c 696e 6520 6368 6172  dating line char
-00000af0: 7473 2069 6e20 6375 7374 6f6d 746b 696e  ts in customtkin
-00000b00: 7465 722e 3c2f 6c69 3e0d 0a0d 0a3c 2f64  ter.</li>....</d
-00000b10: 6976 3e0d 0a0d 0a23 2320 4665 6174 7572  iv>....## Featur
-00000b20: 6573 0d0a 0d0a 2d20 2a2a 4c69 7665 2055  es....- **Live U
-00000b30: 7064 6174 652a 2a3a 2044 6973 706c 6179  pdate**: Display
-00000b40: 206c 6976 6520 6461 7461 2077 6974 6820   live data with 
-00000b50: 6c69 6e65 2063 6861 7274 732e 0d0a 2d20  line charts...- 
-00000b60: 2a2a 4d75 6c74 6970 6c65 204c 696e 6573  **Multiple Lines
-00000b70: 2a2a 3a20 5375 7070 6f72 7420 666f 7220  **: Support for 
-00000b80: 706c 6f74 7469 6e67 206d 756c 7469 706c  plotting multipl
-00000b90: 6520 6c69 6e65 7320 6f6e 2074 6865 2073  e lines on the s
-00000ba0: 616d 6520 6368 6172 7420 666f 7220 6561  ame chart for ea
-00000bb0: 7379 2063 6f6d 7061 7269 736f 6e2e 0d0a  sy comparison...
-00000bc0: 2d20 2a2a 436f 6c6f 7220 4375 7374 6f6d  - **Color Custom
-00000bd0: 697a 6174 696f 6e2a 2a3a 2043 7573 746f  ization**: Custo
-00000be0: 6d69 7a65 2063 6f6c 6f72 7320 746f 206d  mize colors to m
-00000bf0: 6174 6368 2079 6f75 7220 6170 706c 6963  atch your applic
-00000c00: 6174 696f 6e27 7320 6465 7369 676e 206f  ation's design o
-00000c10: 7220 6461 7461 2072 6570 7265 7365 6e74  r data represent
-00000c20: 6174 696f 6e2e 0d0a 2d20 2a2a 4479 6e61  ation...- **Dyna
-00000c30: 6d69 6320 436f 6c6f 7220 4368 616e 6765  mic Color Change
-00000c40: 2a2a 3a20 4479 6e61 6d69 6320 436f 6c6f  **: Dynamic Colo
-00000c50: 7220 4368 616e 6765 2066 6f72 2044 6172  r Change for Dar
-00000c60: 6b20 2620 4c69 6768 742e 0d0a 2d20 2a2a  k & Light...- **
-00000c70: 466f 6e74 2043 7573 746f 6d69 7a61 7469  Font Customizati
-00000c80: 6f6e 2a2a 3a20 4164 6a75 7374 2066 6f6e  on**: Adjust fon
-00000c90: 7473 2066 6f72 2074 6578 7420 656c 656d  ts for text elem
-00000ca0: 656e 7473 2074 6f20 656e 6861 6e63 6520  ents to enhance 
-00000cb0: 7265 6164 6162 696c 6974 792e 0d0a 2d20  readability...- 
-00000cc0: 2a2a 4469 6d65 6e73 696f 6e20 4375 7374  **Dimension Cust
-00000cd0: 6f6d 697a 6174 696f 6e2a 2a3a 2043 7573  omization**: Cus
-00000ce0: 746f 6d69 7a65 2063 6861 7274 2064 696d  tomize chart dim
-00000cf0: 656e 7369 6f6e 7320 746f 2066 6974 2076  ensions to fit v
-00000d00: 6172 696f 7573 2064 6973 706c 6179 2073  arious display s
-00000d10: 697a 6573 2061 6e64 206c 6179 6f75 7473  izes and layouts
-00000d20: 2e0d 0a0d 0a23 2320 496d 706f 7274 696e  .....## Importin
-00000d30: 6720 2620 496e 7374 616c 6c61 7469 6f6e  g & Installation
-00000d40: 0d0a 2a20 496e 7374 616c 6c61 7469 6f6e  ..* Installation
-00000d50: 0d0a 2020 2020 6060 600d 0a20 2020 2070  ..    ```..    p
-00000d60: 6970 2069 6e73 7461 6c6c 2063 746b 6368  ip install ctkch
-00000d70: 6172 740d 0a20 2020 2060 6060 0d0a 0d0a  art..    ```....
-00000d80: 2a20 496d 706f 7274 696e 670d 0a20 2020  * Importing..   
-00000d90: 2020 6060 600d 0a20 2020 2069 6d70 6f72    ```..    impor
-00000da0: 7420 6374 6b63 6861 7274 0d0a 2020 2020  t ctkchart..    
-00000db0: 6060 600d 0a0d 0a23 204c 696e 6b73 0d0a  ```....# Links..
-00000dc0: 0d0a 2d20 2a2a 5669 7369 7420 4769 7448  ..- **Visit GitH
-00000dd0: 7562 2066 6f72 204d 6f72 6520 4465 7461  ub for More Deta
-00000de0: 696c 732e 2e2e 2e2e 2a2a 0d0a 2d20 2323  ils.....**..- ##
-00000df0: 202a 2a47 6974 4875 622e 636f 6d2a 2a20   **GitHub.com** 
-00000e00: 2020 3a20 203c 6120 6872 6566 3d22 6874    :  <a href="ht
-00000e10: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000e20: 2f54 6869 7361 6c2d 442f 6374 6b63 6861  /Thisal-D/ctkcha
-00000e30: 7274 2220 7461 7267 6574 3d22 5f62 6c61  rt" target="_bla
-00000e40: 6e6b 2220 3e3c 693e 6374 6b63 6861 7274  nk" ><i>ctkchart
-00000e50: 3c2f 693e 3c2f 613e 0d0a                 </i></a>..
+00000a60: 2f74 6875 6d62 6e61 696c 3f69 643d 3163  /thumbnail?id=1c
+00000a70: 4872 7346 494c 484a 3761 3262 674d 5876  HrsFILHJ7a2bgMXv
+00000a80: 6b2d 5057 6c6e 4c5a 7831 7643 6e56 5226  k-PWlnLZx1vCnVR&
+00000a90: 737a 3d77 3138 3022 3e0d 0a0d 0a0d 0a3c  sz=w180">......<
+00000aa0: 2f64 6976 3e0d 0a0d 0a23 2323 203c 6c69  /div>....### <li
+00000ab0: 3e63 746b 6368 6172 7420 6973 2061 2050  >ctkchart is a P
+00000ac0: 7974 686f 6e20 6c69 6272 6172 7920 666f  ython library fo
+00000ad0: 7220 6372 6561 7469 6e67 206c 6976 6520  r creating live 
+00000ae0: 7570 6461 7469 6e67 206c 696e 6520 6368  updating line ch
+00000af0: 6172 7473 2069 6e20 6375 7374 6f6d 746b  arts in customtk
+00000b00: 696e 7465 722e 3c2f 6c69 3e0d 0a0d 0a3c  inter.</li>....<
+00000b10: 2f64 6976 3e0d 0a0d 0a23 2320 4665 6174  /div>....## Feat
+00000b20: 7572 6573 0d0a 0d0a 2d20 2a2a 4c69 7665  ures....- **Live
+00000b30: 2055 7064 6174 652a 2a3a 2044 6973 706c   Update**: Displ
+00000b40: 6179 206c 6976 6520 6461 7461 2077 6974  ay live data wit
+00000b50: 6820 6c69 6e65 2063 6861 7274 732e 0d0a  h line charts...
+00000b60: 2d20 2a2a 4d75 6c74 6970 6c65 204c 696e  - **Multiple Lin
+00000b70: 6573 2a2a 3a20 5375 7070 6f72 7420 666f  es**: Support fo
+00000b80: 7220 706c 6f74 7469 6e67 206d 756c 7469  r plotting multi
+00000b90: 706c 6520 6c69 6e65 7320 6f6e 2074 6865  ple lines on the
+00000ba0: 2073 616d 6520 6368 6172 7420 666f 7220   same chart for 
+00000bb0: 6561 7379 2063 6f6d 7061 7269 736f 6e2e  easy comparison.
+00000bc0: 0d0a 2d20 2a2a 436f 6c6f 7220 4375 7374  ..- **Color Cust
+00000bd0: 6f6d 697a 6174 696f 6e2a 2a3a 2043 7573  omization**: Cus
+00000be0: 746f 6d69 7a65 2063 6f6c 6f72 7320 746f  tomize colors to
+00000bf0: 206d 6174 6368 2079 6f75 7220 6170 706c   match your appl
+00000c00: 6963 6174 696f 6e27 7320 6465 7369 676e  ication's design
+00000c10: 206f 7220 6461 7461 2072 6570 7265 7365   or data represe
+00000c20: 6e74 6174 696f 6e2e 0d0a 2d20 2a2a 4479  ntation...- **Dy
+00000c30: 6e61 6d69 6320 436f 6c6f 7220 4368 616e  namic Color Chan
+00000c40: 6765 2a2a 3a20 4479 6e61 6d69 6320 436f  ge**: Dynamic Co
+00000c50: 6c6f 7220 4368 616e 6765 2066 6f72 2044  lor Change for D
+00000c60: 6172 6b20 2620 4c69 6768 742e 0d0a 2d20  ark & Light...- 
+00000c70: 2a2a 466f 6e74 2043 7573 746f 6d69 7a61  **Font Customiza
+00000c80: 7469 6f6e 2a2a 3a20 4164 6a75 7374 2066  tion**: Adjust f
+00000c90: 6f6e 7473 2066 6f72 2074 6578 7420 656c  onts for text el
+00000ca0: 656d 656e 7473 2074 6f20 656e 6861 6e63  ements to enhanc
+00000cb0: 6520 7265 6164 6162 696c 6974 792e 0d0a  e readability...
+00000cc0: 2d20 2a2a 4469 6d65 6e73 696f 6e20 4375  - **Dimension Cu
+00000cd0: 7374 6f6d 697a 6174 696f 6e2a 2a3a 2043  stomization**: C
+00000ce0: 7573 746f 6d69 7a65 2063 6861 7274 2064  ustomize chart d
+00000cf0: 696d 656e 7369 6f6e 7320 746f 2066 6974  imensions to fit
+00000d00: 2076 6172 696f 7573 2064 6973 706c 6179   various display
+00000d10: 2073 697a 6573 2061 6e64 206c 6179 6f75   sizes and layou
+00000d20: 7473 2e0d 0a0d 0a23 2320 496d 706f 7274  ts.....## Import
+00000d30: 696e 6720 2620 496e 7374 616c 6c61 7469  ing & Installati
+00000d40: 6f6e 0d0a 2a20 496e 7374 616c 6c61 7469  on..* Installati
+00000d50: 6f6e 0d0a 2020 2020 6060 600d 0a20 2020  on..    ```..   
+00000d60: 2070 6970 2069 6e73 7461 6c6c 2063 746b   pip install ctk
+00000d70: 6368 6172 740d 0a20 2020 2060 6060 0d0a  chart..    ```..
+00000d80: 0d0a 2a20 496d 706f 7274 696e 670d 0a20  ..* Importing.. 
+00000d90: 2020 2020 6060 600d 0a20 2020 2069 6d70      ```..    imp
+00000da0: 6f72 7420 6374 6b63 6861 7274 0d0a 2020  ort ctkchart..  
+00000db0: 2020 6060 600d 0a0d 0a23 204c 696e 6b73    ```....# Links
+00000dc0: 0d0a 0d0a 2a2a 5669 7369 7420 4769 7448  ....**Visit GitH
+00000dd0: 7562 2066 6f72 2044 6f63 756d 656e 7461  ub for Documenta
+00000de0: 7469 6f6e 3a2a 2a0d 0a0d 0a2d 202a 2a47  tion:**....- **G
+00000df0: 6974 4875 6220 5265 706f 7369 746f 7279  itHub Repository
+00000e00: 3a2a 2a20 5b63 746b 6368 6172 745d 2868  :** [ctkchart](h
+00000e10: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000e20: 6d2f 5468 6973 616c 2d44 2f63 746b 6368  m/Thisal-D/ctkch
+00000e30: 6172 7429 0d0a                           art)..
```

