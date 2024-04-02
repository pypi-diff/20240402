# Comparing `tmp/boomgate-0.0.1.dev2.tar.gz` & `tmp/boomgate-0.0.2.tar.gz`

## Comparing `boomgate-0.0.1.dev2.tar` & `boomgate-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,14 @@
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 boomgate-0.0.1.dev2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 boomgate-0.0.1.dev2/.github/workflows/release.yaml
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 boomgate-0.0.1.dev2/src/boomgate/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 boomgate-0.0.1.dev2/src/boomgate/__init__.py
--rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 boomgate-0.0.1.dev2/src/boomgate/cached_http.py
--rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 boomgate-0.0.1.dev2/src/boomgate/cli.py
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 boomgate-0.0.1.dev2/src/boomgate/inspect.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 boomgate-0.0.1.dev2/src/boomgate/logging.py
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 boomgate-0.0.1.dev2/src/boomgate/vulnerabilities.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 boomgate-0.0.1.dev2/src/boomgate/ecosystems/__init__.py
--rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 boomgate-0.0.1.dev2/src/boomgate/ecosystems/pypi.py
--rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 boomgate-0.0.1.dev2/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 boomgate-0.0.1.dev2/LICENSE
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 boomgate-0.0.1.dev2/README.md
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 boomgate-0.0.1.dev2/pyproject.toml
--rw-r--r--   0        0        0    42533 2020-02-02 00:00:00.000000 boomgate-0.0.1.dev2/PKG-INFO
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 boomgate-0.0.2/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 boomgate-0.0.2/src/boomgate/__init__.py
+-rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 boomgate-0.0.2/src/boomgate/cached_http.py
+-rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 boomgate-0.0.2/src/boomgate/cli.py
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 boomgate-0.0.2/src/boomgate/inspect.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 boomgate-0.0.2/src/boomgate/logging.py
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 boomgate-0.0.2/src/boomgate/vulnerabilities.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 boomgate-0.0.2/src/boomgate/ecosystems/__init__.py
+-rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 boomgate-0.0.2/src/boomgate/ecosystems/pypi.py
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 boomgate-0.0.2/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 boomgate-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 boomgate-0.0.2/README.md
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 boomgate-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    43020 2020-02-02 00:00:00.000000 boomgate-0.0.2/PKG-INFO
```

### Comparing `boomgate-0.0.1.dev2/src/boomgate/cached_http.py` & `boomgate-0.0.2/src/boomgate/cached_http.py`

 * *Files identical despite different names*

### Comparing `boomgate-0.0.1.dev2/src/boomgate/cli.py` & `boomgate-0.0.2/src/boomgate/cli.py`

 * *Files identical despite different names*

### Comparing `boomgate-0.0.1.dev2/src/boomgate/inspect.py` & `boomgate-0.0.2/src/boomgate/inspect.py`

 * *Files identical despite different names*

### Comparing `boomgate-0.0.1.dev2/src/boomgate/logging.py` & `boomgate-0.0.2/src/boomgate/logging.py`

 * *Files identical despite different names*

### Comparing `boomgate-0.0.1.dev2/src/boomgate/vulnerabilities.py` & `boomgate-0.0.2/src/boomgate/vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `boomgate-0.0.1.dev2/src/boomgate/ecosystems/__init__.py` & `boomgate-0.0.2/src/boomgate/ecosystems/__init__.py`

 * *Files identical despite different names*

### Comparing `boomgate-0.0.1.dev2/src/boomgate/ecosystems/pypi.py` & `boomgate-0.0.2/src/boomgate/ecosystems/pypi.py`

 * *Files identical despite different names*

### Comparing `boomgate-0.0.1.dev2/.gitignore` & `boomgate-0.0.2/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -154,8 +154,9 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
-.request_cache
+
+/.request_cache
```

### Comparing `boomgate-0.0.1.dev2/LICENSE` & `boomgate-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `boomgate-0.0.1.dev2/README.md` & `boomgate-0.0.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,109 +1,135 @@
-00000000: 2320 626f 6f6d 6761 7465 0a0a 426f 6f6d  # boomgate..Boom
-00000010: 6761 7465 2068 656c 7073 2079 6f75 2069  gate helps you i
-00000020: 6465 6e74 6966 7920 616e 6420 6d69 7469  dentify and miti
-00000030: 6761 7465 2074 6865 2072 6973 6b73 206f  gate the risks o
-00000040: 6620 7573 696e 6720 7468 6972 642d 7061  f using third-pa
-00000050: 7274 7920 6c69 6272 6172 6965 7320 696e  rty libraries in
-00000060: 0a79 6f75 7220 5079 7468 6f6e 2070 726f  .your Python pro
-00000070: 6a65 6374 732e 0a0a 2323 20e2 9aa0 efb8  jects...## .....
-00000080: 8f20 5468 6973 2069 7320 696e 2061 2070  . This is in a p
-00000090: 7265 2d70 7265 2d70 7265 2d72 656c 6561  re-pre-pre-relea
-000000a0: 7365 2073 7461 7465 2120 e29a a0ef b88f  se state! ......
-000000b0: 0a0a 5468 6973 2070 726f 6a65 6374 2069  ..This project i
-000000c0: 7320 6e6f 7420 7265 6d6f 7465 6c79 2072  s not remotely r
-000000d0: 6561 6479 2066 6f72 2061 6e79 6f6e 6520  eady for anyone 
-000000e0: 746f 206c 6f6f 6b20 6174 2c20 6c65 7420  to look at, let 
-000000f0: 616c 6f6e 6520 7573 652e 2049 7420 6973  alone use. It is
-00000100: 2069 6e20 6120 7665 7279 0a65 6172 6c79   in a very.early
-00000110: 2070 726f 6f66 2d6f 662d 636f 6e63 6570   proof-of-concep
-00000120: 7420 7374 6167 652c 2066 6f63 7573 696e  t stage, focusin
-00000130: 6720 6f6e 2069 7465 7261 7469 7665 2072  g on iterative r
-00000140: 6573 6561 7263 6820 616e 6420 6465 7665  esearch and deve
-00000150: 6c6f 706d 656e 742e 2049 2068 6176 6520  lopment. I have 
-00000160: 6e6f 740a 7365 7474 6c65 6420 6f6e 2074  not.settled on t
-00000170: 6865 2070 726f 6a65 6374 2773 2061 7263  he project's arc
-00000180: 6869 7465 6374 7572 652c 2061 6e64 2049  hitecture, and I
-00000190: 2061 6d20 7374 696c 6c20 6578 706c 6f72   am still explor
-000001a0: 696e 6720 7468 6520 7072 6f62 6c65 6d20  ing the problem 
-000001b0: 7370 6163 652e 2041 730a 7375 6368 2c20  space. As.such, 
-000001c0: 7468 6520 7175 616c 6974 7920 6f66 2074  the quality of t
-000001d0: 6865 2063 6f64 6520 6973 2076 6572 7920  he code is very 
-000001e0: 706f 6f72 2c20 616e 6420 7468 696e 6773  poor, and things
-000001f0: 2061 7265 2067 7561 7261 6e74 6565 6420   are guaranteed 
-00000200: 746f 2063 6861 6e67 652e 0a0a 4920 7769  to change...I wi
-00000210: 6c6c 206e 6f74 2070 726f 7669 6465 2073  ll not provide s
-00000220: 7570 706f 7274 2c20 6e6f 7220 7769 6c6c  upport, nor will
-00000230: 2049 2061 6363 6570 7420 5052 7320 6174   I accept PRs at
-00000240: 2074 6869 7320 7469 6d65 2e0a 0a23 2320   this time...## 
-00000250: 5669 7369 6f6e 0a0a 4920 696e 7465 6e64  Vision..I intend
-00000260: 2066 6f72 2042 6f6f 6d67 6174 6520 746f   for Boomgate to
-00000270: 2061 6c6c 6f77 2079 6f75 2074 6f20 6465   allow you to de
-00000280: 6669 6e65 2061 2070 6f6c 6963 7920 666f  fine a policy fo
-00000290: 7220 796f 7572 2070 726f 6a65 6374 2074  r your project t
-000002a0: 6861 7420 6465 7363 7269 6265 730a 7468  hat describes.th
-000002b0: 6520 7269 736b 7320 796f 7520 6172 6520  e risks you are 
-000002c0: 7769 6c6c 696e 6720 746f 2061 6363 6570  willing to accep
-000002d0: 7420 7768 656e 2075 7369 6e67 2074 6869  t when using thi
-000002e0: 7264 2d70 6172 7479 206c 6962 7261 7269  rd-party librari
-000002f0: 6573 2e20 426f 6f6d 6761 7465 2077 696c  es. Boomgate wil
-00000300: 6c0a 6576 616c 7561 7465 2079 6f75 7220  l.evaluate your 
-00000310: 7072 6f6a 6563 7427 7320 6465 7065 6e64  project's depend
-00000320: 656e 6369 6573 2061 6761 696e 7374 2074  encies against t
-00000330: 6869 7320 706f 6c69 6379 2c20 7265 706f  his policy, repo
-00000340: 7274 206f 6e20 616e 7920 7269 736b 7320  rt on any risks 
-00000350: 7468 6174 2079 6f75 0a64 6565 6d20 756e  that you.deem un
-00000360: 6163 6365 7074 6162 6c65 2c20 616e 64e2  acceptable, and.
-00000370: 8094 616c 736f 2070 6572 2079 6f75 7220  ..also per your 
-00000380: 6465 6669 6e65 6420 706f 6c69 6379 e280  defined policy..
-00000390: 9473 7567 6765 7374 206d 6974 6967 6174  .suggest mitigat
-000003a0: 696f 6e20 7374 7261 7465 6769 6573 2e0a  ion strategies..
-000003b0: 0a46 6f72 2065 7861 6d70 6c65 2c20 796f  .For example, yo
-000003c0: 7520 6d61 7920 6465 6369 6465 2074 6861  u may decide tha
-000003d0: 7420 796f 7520 6172 6520 6e6f 7420 7769  t you are not wi
-000003e0: 6c6c 696e 6720 746f 2075 7365 2061 2064  lling to use a d
-000003f0: 6570 656e 6465 6e63 7920 6966 2069 7473  ependency if its
-00000400: 2061 7574 686f 7227 730a 656d 6169 6c20   author's.email 
-00000410: 6164 6472 6573 7327 7320 646f 6d61 696e  address's domain
-00000420: 2069 7320 6e6f 7420 7265 6769 7374 6572   is not register
-00000430: 6564 2028 692e 652e 2044 4e53 2072 6574  ed (i.e. DNS ret
-00000440: 7572 6e73 2060 4e58 444f 4d41 494e 6029  urns `NXDOMAIN`)
-00000450: 2c20 6f72 2079 6f75 206d 6179 0a64 6563  , or you may.dec
-00000460: 6964 6520 7468 6174 2061 6c6c 2064 6570  ide that all dep
-00000470: 656e 6465 6e63 6965 7320 2862 6172 7269  endencies (barri
-00000480: 6e67 2061 206c 6973 7420 6f66 2065 7863  ng a list of exc
-00000490: 6570 7465 6420 2774 7275 7374 6564 2720  epted 'trusted' 
-000004a0: 6465 7065 6e64 656e 6369 6573 2920 7265  dependencies) re
-000004b0: 7175 6972 650a 6120 7365 6375 7269 7479  quire.a security
-000004c0: 2061 7564 6974 2062 6566 6f72 6520 7468   audit before th
-000004d0: 6579 2063 616e 2062 6520 7573 6564 2e0a  ey can be used..
-000004e0: 0a49 6e20 7468 6973 2065 7861 6d70 6c65  .In this example
-000004f0: 2c20 426f 6f6d 6761 7465 2063 616e 2062  , Boomgate can b
-00000500: 6520 636f 6e66 6967 7572 6564 2074 6f20  e configured to 
-00000510: 626c 6f63 6b20 796f 7572 2070 726f 6a65  block your proje
-00000520: 6374 2773 2043 492f 4344 2070 6970 656c  ct's CI/CD pipel
-00000530: 696e 6520 6966 0a6f 6e65 206f 6620 7468  ine if.one of th
-00000540: 6573 6520 636f 6e64 6974 696f 6e73 2069  ese conditions i
-00000550: 7320 6d65 7420 6279 2079 6f75 7220 7072  s met by your pr
-00000560: 6f6a 6563 7427 7320 7265 736f 6c76 6564  oject's resolved
-00000570: 2064 6570 656e 6465 6e63 6965 732e 0a0a   dependencies...
-00000580: 5365 6520 6d79 2072 6f75 6768 206c 6973  See my rough lis
-00000590: 7420 6f66 2069 6465 6120 696e 2074 6865  t of idea in the
-000005a0: 0a5b 4769 7448 7562 2069 7373 7565 7320  .[GitHub issues 
-000005b0: 6c69 7374 5d28 6874 7470 733a 2f2f 6769  list](https://gi
-000005c0: 7468 7562 2e63 6f6d 2f4b 7965 5275 7373  thub.com/KyeRuss
-000005d0: 656c 6c2f 626f 6f6d 6761 7465 2f69 7373  ell/boomgate/iss
-000005e0: 7565 7329 2e0a 0a23 2320 4465 7665 6c6f  ues)...## Develo
-000005f0: 7069 6e67 0a0a 546f 2067 6574 2073 7461  ping..To get sta
-00000600: 7274 6564 2c20 636c 6f6e 6520 7468 6520  rted, clone the 
-00000610: 7265 706f 7369 746f 7279 2061 6e64 2072  repository and r
-00000620: 756e 2074 6865 2066 6f6c 6c6f 7769 6e67  un the following
-00000630: 2063 6f6d 6d61 6e64 3a0a 0a60 6060 6261   command:..```ba
-00000640: 7368 0a75 7620 7069 7020 696e 7374 616c  sh.uv pip instal
-00000650: 6c20 2d65 202e 202d 7220 7079 7072 6f6a  l -e . -r pyproj
-00000660: 6563 742e 746f 6d6c 202d 2d65 7874 7261  ect.toml --extra
-00000670: 3d64 6576 0a60 6060 0a0a 5468 6973 2077  =dev.```..This w
-00000680: 696c 6c20 696e 7374 616c 6c20 7468 6520  ill install the 
-00000690: 7072 6f6a 6563 7420 696e 2065 6469 7461  project in edita
-000006a0: 626c 6520 6d6f 6465 2077 6974 6820 616c  ble mode with al
-000006b0: 6c20 6465 7665 6c6f 706d 656e 7420 6465  l development de
-000006c0: 7065 6e64 656e 6369 6573 2e0a            pendencies..
+00000000: 3c68 3220 616c 6967 6e3d 2263 656e 7465  <h2 align="cente
+00000010: 7222 3e42 6f6f 6d67 6174 653c 2f68 323e  r">Boomgate</h2>
+00000020: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+00000030: 7222 3e3c 656d 3e0a 2020 2020 4964 656e  r"><em>.    Iden
+00000040: 7469 6679 2061 6e64 206d 6974 6967 6174  tify and mitigat
+00000050: 6520 7468 6520 7269 736b 7320 6f66 2075  e the risks of u
+00000060: 7369 6e67 2074 6869 7264 2d70 6172 7479  sing third-party
+00000070: 206c 6962 7261 7269 6573 2e0a 3c2f 656d   libraries..</em
+00000080: 3e3c 2f70 3e0a 0a3c 7020 616c 6967 6e3d  ></p>..<p align=
+00000090: 2263 656e 7465 7222 3e0a 2020 2020 3c61  "center">.    <a
+000000a0: 2068 7265 663d 2268 7474 7073 3a2f 2f70   href="https://p
+000000b0: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
+000000c0: 626f 6f6d 6761 7465 2f22 3e0a 2020 2020  boomgate/">.    
+000000d0: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
+000000e0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+000000f0: 732e 696f 2f70 7970 692f 762f 626f 6f6d  s.io/pypi/v/boom
+00000100: 6761 7465 3f63 6f6c 6f72 3d25 3233 3334  gate?color=%2334
+00000110: 4430 3538 266c 6162 656c 3d50 7950 4925  D058&label=PyPI%
+00000120: 3230 7061 636b 6167 6522 2061 6c74 3d22  20package" alt="
+00000130: 5079 5049 2076 6572 7369 6f6e 223e 0a20  PyPI version">. 
+00000140: 2020 203c 2f61 3e0a 2020 2020 3c61 2068     </a>.    <a h
+00000150: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+00000160: 6875 622e 636f 6d2f 4b79 6552 7573 7365  hub.com/KyeRusse
+00000170: 6c6c 2f62 6f6f 6d67 6174 652f 6163 7469  ll/boomgate/acti
+00000180: 6f6e 732f 776f 726b 666c 6f77 732f 7265  ons/workflows/re
+00000190: 6c65 6173 652e 7961 6d6c 223e 0a20 2020  lease.yaml">.   
+000001a0: 2020 2020 203c 696d 6720 7372 633d 2268       <img src="h
+000001b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000001c0: 6d2f 4b79 6552 7573 7365 6c6c 2f62 6f6f  m/KyeRussell/boo
+000001d0: 6d67 6174 652f 6163 7469 6f6e 732f 776f  mgate/actions/wo
+000001e0: 726b 666c 6f77 732f 7265 6c65 6173 652e  rkflows/release.
+000001f0: 7961 6d6c 2f62 6164 6765 2e73 7667 2220  yaml/badge.svg" 
+00000200: 616c 743d 2252 656c 6561 7365 2077 6f72  alt="Release wor
+00000210: 6b66 6c6f 7720 7374 6174 7573 223e 0a20  kflow status">. 
+00000220: 2020 203c 2f61 3e0a 3c2f 703e 0a0a 2d2d     </a>.</p>..--
+00000230: 2d0a 0a3e 205b 2149 4d50 4f52 5441 4e54  -..> [!IMPORTANT
+00000240: 5d0a 3e20 5468 6973 2070 726f 6a65 6374  ].> This project
+00000250: 2069 7320 6e6f 7420 7265 6d6f 7465 6c79   is not remotely
+00000260: 2072 6561 6479 2066 6f72 2061 6e79 6f6e   ready for anyon
+00000270: 6520 746f 206c 6f6f 6b20 6174 2c20 6c65  e to look at, le
+00000280: 7420 616c 6f6e 6520 7573 652e 2049 7420  t alone use. It 
+00000290: 6973 2069 6e20 610a 3e20 7665 7279 2065  is in a.> very e
+000002a0: 6172 6c79 2070 726f 6f66 2d6f 662d 636f  arly proof-of-co
+000002b0: 6e63 6570 7420 7374 6167 652c 2066 6f63  ncept stage, foc
+000002c0: 7573 696e 6720 6f6e 2069 7465 7261 7469  using on iterati
+000002d0: 7665 2072 6573 6561 7263 6820 616e 6420  ve research and 
+000002e0: 6465 7665 6c6f 706d 656e 742e 2049 0a3e  development. I.>
+000002f0: 2068 6176 6520 6e6f 7420 7365 7474 6c65   have not settle
+00000300: 6420 6f6e 2074 6865 2070 726f 6a65 6374  d on the project
+00000310: 2773 2061 7263 6869 7465 6374 7572 652c  's architecture,
+00000320: 2061 6e64 2049 2061 6d20 7374 696c 6c20   and I am still 
+00000330: 6578 706c 6f72 696e 6720 7468 6520 7072  exploring the pr
+00000340: 6f62 6c65 6d0a 3e20 7370 6163 652e 2041  oblem.> space. A
+00000350: 7320 7375 6368 2c20 7468 6520 7175 616c  s such, the qual
+00000360: 6974 7920 6f66 2074 6865 2063 6f64 6520  ity of the code 
+00000370: 6973 2076 6572 7920 706f 6f72 2c20 616e  is very poor, an
+00000380: 6420 7468 696e 6773 2061 7265 2067 7561  d things are gua
+00000390: 7261 6e74 6565 6420 746f 0a3e 2063 6861  ranteed to.> cha
+000003a0: 6e67 652e 0a3e 0a3e 2049 2077 696c 6c20  nge..>.> I will 
+000003b0: 6e6f 7420 7072 6f76 6964 6520 7375 7070  not provide supp
+000003c0: 6f72 742c 206e 6f72 2077 696c 6c20 4920  ort, nor will I 
+000003d0: 6163 6365 7074 2050 5273 2061 7420 7468  accept PRs at th
+000003e0: 6973 2074 696d 652e 0a0a 2d2d 2d0a 0a23  is time...---..#
+000003f0: 2320 5669 7369 6f6e 0a0a 4920 696e 7465  # Vision..I inte
+00000400: 6e64 2066 6f72 2042 6f6f 6d67 6174 6520  nd for Boomgate 
+00000410: 746f 2061 6c6c 6f77 2079 6f75 2074 6f20  to allow you to 
+00000420: 6465 6669 6e65 2061 2070 6f6c 6963 7920  define a policy 
+00000430: 666f 7220 796f 7572 2070 726f 6a65 6374  for your project
+00000440: 2074 6861 7420 6465 7363 7269 6265 730a   that describes.
+00000450: 7468 6520 7269 736b 7320 796f 7520 6172  the risks you ar
+00000460: 6520 7769 6c6c 696e 6720 746f 2061 6363  e willing to acc
+00000470: 6570 7420 7768 656e 2075 7369 6e67 2074  ept when using t
+00000480: 6869 7264 2d70 6172 7479 206c 6962 7261  hird-party libra
+00000490: 7269 6573 2e20 426f 6f6d 6761 7465 2077  ries. Boomgate w
+000004a0: 696c 6c0a 6576 616c 7561 7465 2079 6f75  ill.evaluate you
+000004b0: 7220 7072 6f6a 6563 7427 7320 6465 7065  r project's depe
+000004c0: 6e64 656e 6369 6573 2061 6761 696e 7374  ndencies against
+000004d0: 2074 6869 7320 706f 6c69 6379 2c20 7265   this policy, re
+000004e0: 706f 7274 206f 6e20 616e 7920 7269 736b  port on any risk
+000004f0: 7320 7468 6174 2079 6f75 0a64 6565 6d20  s that you.deem 
+00000500: 756e 6163 6365 7074 6162 6c65 2c20 616e  unacceptable, an
+00000510: 64e2 8094 616c 736f 2070 6572 2079 6f75  d...also per you
+00000520: 7220 6465 6669 6e65 6420 706f 6c69 6379  r defined policy
+00000530: e280 9473 7567 6765 7374 206d 6974 6967  ...suggest mitig
+00000540: 6174 696f 6e20 7374 7261 7465 6769 6573  ation strategies
+00000550: 2e0a 0a46 6f72 2065 7861 6d70 6c65 2c20  ...For example, 
+00000560: 796f 7520 6d61 7920 6465 6369 6465 2074  you may decide t
+00000570: 6861 7420 796f 7520 6172 6520 6e6f 7420  hat you are not 
+00000580: 7769 6c6c 696e 6720 746f 2075 7365 2061  willing to use a
+00000590: 2064 6570 656e 6465 6e63 7920 6966 2069   dependency if i
+000005a0: 7473 2061 7574 686f 7227 730a 656d 6169  ts author's.emai
+000005b0: 6c20 6164 6472 6573 7327 7320 646f 6d61  l address's doma
+000005c0: 696e 2069 7320 6e6f 7420 7265 6769 7374  in is not regist
+000005d0: 6572 6564 2028 692e 652e 2044 4e53 2072  ered (i.e. DNS r
+000005e0: 6574 7572 6e73 2060 4e58 444f 4d41 494e  eturns `NXDOMAIN
+000005f0: 6029 2c20 6f72 2079 6f75 206d 6179 0a64  `), or you may.d
+00000600: 6563 6964 6520 7468 6174 2061 6c6c 2064  ecide that all d
+00000610: 6570 656e 6465 6e63 6965 7320 2862 6172  ependencies (bar
+00000620: 7269 6e67 2061 206c 6973 7420 6f66 2065  ring a list of e
+00000630: 7863 6570 7465 6420 2774 7275 7374 6564  xcepted 'trusted
+00000640: 2720 6465 7065 6e64 656e 6369 6573 2920  ' dependencies) 
+00000650: 7265 7175 6972 650a 6120 7365 6375 7269  require.a securi
+00000660: 7479 2061 7564 6974 2062 6566 6f72 6520  ty audit before 
+00000670: 7468 6579 2063 616e 2062 6520 7573 6564  they can be used
+00000680: 2e0a 0a49 6e20 7468 6973 2065 7861 6d70  ...In this examp
+00000690: 6c65 2c20 426f 6f6d 6761 7465 2063 616e  le, Boomgate can
+000006a0: 2062 6520 636f 6e66 6967 7572 6564 2074   be configured t
+000006b0: 6f20 626c 6f63 6b20 796f 7572 2070 726f  o block your pro
+000006c0: 6a65 6374 2773 2043 492f 4344 2070 6970  ject's CI/CD pip
+000006d0: 656c 696e 6520 6966 0a6f 6e65 206f 6620  eline if.one of 
+000006e0: 7468 6573 6520 636f 6e64 6974 696f 6e73  these conditions
+000006f0: 2069 7320 6d65 7420 6279 2079 6f75 7220   is met by your 
+00000700: 7072 6f6a 6563 7427 7320 7265 736f 6c76  project's resolv
+00000710: 6564 2064 6570 656e 6465 6e63 6965 732e  ed dependencies.
+00000720: 0a0a 5365 6520 6d79 2072 6f75 6768 206c  ..See my rough l
+00000730: 6973 7420 6f66 2069 6465 6120 696e 2074  ist of idea in t
+00000740: 6865 0a5b 4769 7448 7562 2069 7373 7565  he.[GitHub issue
+00000750: 7320 6c69 7374 5d28 6874 7470 733a 2f2f  s list](https://
+00000760: 6769 7468 7562 2e63 6f6d 2f4b 7965 5275  github.com/KyeRu
+00000770: 7373 656c 6c2f 626f 6f6d 6761 7465 2f69  ssell/boomgate/i
+00000780: 7373 7565 7329 2e0a 0a23 2320 4465 7665  ssues)...## Deve
+00000790: 6c6f 7069 6e67 0a0a 546f 2067 6574 2073  loping..To get s
+000007a0: 7461 7274 6564 2c20 636c 6f6e 6520 7468  tarted, clone th
+000007b0: 6520 7265 706f 7369 746f 7279 2061 6e64  e repository and
+000007c0: 2072 756e 2074 6865 2066 6f6c 6c6f 7769   run the followi
+000007d0: 6e67 2063 6f6d 6d61 6e64 3a0a 0a60 6060  ng command:..```
+000007e0: 6261 7368 0a75 7620 7069 7020 696e 7374  bash.uv pip inst
+000007f0: 616c 6c20 2d65 202e 202d 7220 7079 7072  all -e . -r pypr
+00000800: 6f6a 6563 742e 746f 6d6c 202d 2d65 7874  oject.toml --ext
+00000810: 7261 3d64 6576 0a60 6060 0a0a 5468 6973  ra=dev.```..This
+00000820: 2077 696c 6c20 696e 7374 616c 6c20 7468   will install th
+00000830: 6520 7072 6f6a 6563 7420 696e 2065 6469  e project in edi
+00000840: 7461 626c 6520 6d6f 6465 2077 6974 6820  table mode with 
+00000850: 616c 6c20 6465 7665 6c6f 706d 656e 7420  all development 
+00000860: 6465 7065 6e64 656e 6369 6573 2e0a       dependencies..
```

### Comparing `boomgate-0.0.1.dev2/pyproject.toml` & `boomgate-0.0.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["hatchling"]
+requires = ["hatchling", "hatch-vcs"]
 build-backend = "hatchling.build"
 
 [project]
 name = "boomgate"
 authors = [{ name = "Kye Russell", email = "me@kye.id.au" }]
 description = "A software supply chain risk management tool"
 readme = "README.md"
@@ -20,18 +20,25 @@
     "Topic :: System :: Archiving :: Packaging",
     "Topic :: Utilities",
 ]
 keywords = ["security", "dependency", "supply chain"]
 dynamic = ["version"]
 
 [project.optional-dependencies]
-dev = ["ruff", "pre-commit", "mypy"]
+dev = ["ruff", "pre-commit", "mypy", "build", "hatch"]
 
 [project.scripts]
 boomgate = "boomgate.cli:main"
 
 [project.urls]
 Homepage = "https://github.com/KyeRussell/boomgate"
 Issues = "https://github.com/KyeRussell/boomgate/issues"
 
 [tool.hatch.version]
-path = "src/boomgate/__about__.py"
+source = "vcs"
+
+[tool.hatch.build.hooks.vcs]
+version-file = "_version.py"
+
+[tool.hatch.build.targets.sdist]
+include = ["src/*", "LICENSE"]
+exclude = ["*.json", "pkg/_compat.py"]
```

### Comparing `boomgate-0.0.1.dev2/PKG-INFO` & `boomgate-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: boomgate
-Version: 0.0.1.dev2
+Version: 0.0.2
 Summary: A software supply chain risk management tool
 Project-URL: Homepage, https://github.com/KyeRussell/boomgate
 Project-URL: Issues, https://github.com/KyeRussell/boomgate/issues
 Author-email: Kye Russell <me@kye.id.au>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
@@ -677,32 +677,47 @@
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 Requires-Dist: httpx
 Requires-Dist: rich
 Requires-Dist: typer
 Provides-Extra: dev
+Requires-Dist: build; extra == 'dev'
+Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
 Description-Content-Type: text/markdown
 
-# boomgate
+<h2 align="center">Boomgate</h2>
+<p align="center"><em>
+    Identify and mitigate the risks of using third-party libraries.
+</em></p>
 
-Boomgate helps you identify and mitigate the risks of using third-party libraries in
-your Python projects.
+<p align="center">
+    <a href="https://pypi.org/project/boomgate/">
+        <img src="https://img.shields.io/pypi/v/boomgate?color=%2334D058&label=PyPI%20package" alt="PyPI version">
+    </a>
+    <a href="https://github.com/KyeRussell/boomgate/actions/workflows/release.yaml">
+        <img src="https://github.com/KyeRussell/boomgate/actions/workflows/release.yaml/badge.svg" alt="Release workflow status">
+    </a>
+</p>
 
-## ⚠️ This is in a pre-pre-pre-release state! ⚠️
+---
 
-This project is not remotely ready for anyone to look at, let alone use. It is in a very
-early proof-of-concept stage, focusing on iterative research and development. I have not
-settled on the project's architecture, and I am still exploring the problem space. As
-such, the quality of the code is very poor, and things are guaranteed to change.
+> [!IMPORTANT]
+> This project is not remotely ready for anyone to look at, let alone use. It is in a
+> very early proof-of-concept stage, focusing on iterative research and development. I
+> have not settled on the project's architecture, and I am still exploring the problem
+> space. As such, the quality of the code is very poor, and things are guaranteed to
+> change.
+>
+> I will not provide support, nor will I accept PRs at this time.
 
-I will not provide support, nor will I accept PRs at this time.
+---
 
 ## Vision
 
 I intend for Boomgate to allow you to define a policy for your project that describes
 the risks you are willing to accept when using third-party libraries. Boomgate will
 evaluate your project's dependencies against this policy, report on any risks that you
 deem unacceptable, and—also per your defined policy—suggest mitigation strategies.
```

