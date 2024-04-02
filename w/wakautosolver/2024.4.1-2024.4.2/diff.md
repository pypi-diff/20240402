# Comparing `tmp/wakautosolver-2024.4.1-py3-none-any.whl.zip` & `tmp/wakautosolver-2024.4.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2004865 bytes, number of entries: 31
+Zip file size: 2005125 bytes, number of entries: 31
 -rw-r--r--  2.0 fat    16725 b- defN 20-Feb-02 00:00 LICENSE
 -rw-r--r--  2.0 fat   453356 b- defN 20-Feb-02 00:00 .venv/Lib/site-packages/scripts/item_data.bz2
 -rw-r--r--  2.0 fat   137411 b- defN 20-Feb-02 00:00 .venv/Lib/site-packages/scripts/locale_bundle.bz2
 -rw-r--r--  2.0 fat   453356 b- defN 20-Feb-02 00:00 scripts/item_data.bz2
 -rw-r--r--  2.0 fat      510 b- defN 20-Feb-02 00:00 wakautosolver/__init__.py
 -rw-r--r--  2.0 fat      764 b- defN 20-Feb-02 00:00 wakautosolver/__main__.py
 -rw-r--r--  2.0 fat     3851 b- defN 20-Feb-02 00:00 wakautosolver/_build_codes.py
@@ -17,17 +17,17 @@
 -rw-r--r--  2.0 fat    12530 b- defN 20-Feb-02 00:00 wakautosolver/versioned_entrypoints.py
 -rw-r--r--  2.0 fat     7126 b- defN 20-Feb-02 00:00 wakautosolver/wakforge_buildcodes.py
 -rw-r--r--  2.0 fat      366 b- defN 20-Feb-02 00:00 wakautosolver/b2048/__init__.py
 -rw-r--r--  2.0 fat    49861 b- defN 20-Feb-02 00:00 wakautosolver/b2048/dec_table.py
 -rw-r--r--  2.0 fat    21610 b- defN 20-Feb-02 00:00 wakautosolver/b2048/enc_table.py
 -rw-r--r--  2.0 fat     3634 b- defN 20-Feb-02 00:00 wakautosolver/b2048/encoder.py
 -rw-r--r--  2.0 fat  1212416 b- defN 20-Feb-02 00:00 wakautosolver/data/items.db
--rw-r--r--  2.0 fat  1991094 b- defN 20-Feb-02 00:00 wakautosolver/data/items.sql
+-rw-r--r--  2.0 fat  1992029 b- defN 20-Feb-02 00:00 wakautosolver/data/items.sql
 -rw-r--r--  2.0 fat   137716 b- defN 20-Feb-02 00:00 wakautosolver/data/locale_bundle.bz2
 -rw-r--r--  2.0 fat       75 b- defN 20-Feb-02 00:00 wakautosolver/data/readme.md
--rw-r--r--  2.0 fat     2779 b- defN 20-Feb-02 00:00 wakautosolver/data/source_info.bz2
+-rw-r--r--  2.0 fat     2816 b- defN 20-Feb-02 00:00 wakautosolver/data/source_info.bz2
 -rw-r--r--  2.0 fat    85259 b- defN 20-Feb-02 00:00 wakautosolver/data/stat_only_bundle.bz2
-?rw-r--r--  2.0 fat     6104 b- defN 20-Feb-02 00:00 wakautosolver-2024.4.1.dist-info/METADATA
-?rw-r--r--  2.0 fat       87 b- defN 20-Feb-02 00:00 wakautosolver-2024.4.1.dist-info/WHEEL
-?rw-r--r--  2.0 fat    16725 b- defN 20-Feb-02 00:00 wakautosolver-2024.4.1.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 fat     2713 b- defN 20-Feb-02 00:00 wakautosolver-2024.4.1.dist-info/RECORD
-31 files, 4704170 bytes uncompressed, 2000511 bytes compressed:  57.5%
+?rw-r--r--  2.0 fat     6104 b- defN 20-Feb-02 00:00 wakautosolver-2024.4.2.dist-info/METADATA
+?rw-r--r--  2.0 fat       87 b- defN 20-Feb-02 00:00 wakautosolver-2024.4.2.dist-info/WHEEL
+?rw-r--r--  2.0 fat    16725 b- defN 20-Feb-02 00:00 wakautosolver-2024.4.2.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 fat     2713 b- defN 20-Feb-02 00:00 wakautosolver-2024.4.2.dist-info/RECORD
+31 files, 4705142 bytes uncompressed, 2000771 bytes compressed:  57.5%
```

## zipnote {}

```diff
@@ -75,20 +75,20 @@
 
 Filename: wakautosolver/data/source_info.bz2
 Comment: 
 
 Filename: wakautosolver/data/stat_only_bundle.bz2
 Comment: 
 
-Filename: wakautosolver-2024.4.1.dist-info/METADATA
+Filename: wakautosolver-2024.4.2.dist-info/METADATA
 Comment: 
 
-Filename: wakautosolver-2024.4.1.dist-info/WHEEL
+Filename: wakautosolver-2024.4.2.dist-info/WHEEL
 Comment: 
 
-Filename: wakautosolver-2024.4.1.dist-info/licenses/LICENSE
+Filename: wakautosolver-2024.4.2.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: wakautosolver-2024.4.1.dist-info/RECORD
+Filename: wakautosolver-2024.4.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wakautosolver/__init__.py

```diff
@@ -2,15 +2,15 @@
 This Source Code Form is subject to the terms of the Mozilla Public
 License, v. 2.0. If a copy of the MPL was not distributed with this
 file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 Copyright (C) 2023 Michael Hall <https://github.com/mikeshardmind>
 """
 
-__version__ = "2024.04.01"
+__version__ = "2024.04.02"
 
 from . import object_parsing, solver
 from .b2048 import decode as b2048_decode
 from .b2048 import encode as b2048_encode
 
 __all__ = [
     "b2048_decode",
```

## wakautosolver/data/items.db

### sqlite3 {} .dump

```diff
@@ -271,14 +271,15 @@
 INSERT INTO legacy_items VALUES(18679);
 INSERT INTO legacy_items VALUES(18680);
 INSERT INTO legacy_items VALUES(18681);
 CREATE TABLE ub_items (
     item_id INTEGER NOT NULL REFERENCES items(item_id),
     PRIMARY KEY (item_id)
 ) STRICT, WITHOUT ROWID ;
+INSERT INTO ub_items VALUES(3195);
 INSERT INTO ub_items VALUES(8247);
 INSERT INTO ub_items VALUES(8248);
 INSERT INTO ub_items VALUES(8249);
 INSERT INTO ub_items VALUES(12381);
 INSERT INTO ub_items VALUES(12382);
 INSERT INTO ub_items VALUES(12383);
 INSERT INTO ub_items VALUES(12384);
@@ -700,14 +701,39 @@
 INSERT INTO ub_items VALUES(29806);
 INSERT INTO ub_items VALUES(29808);
 INSERT INTO ub_items VALUES(29810);
 INSERT INTO ub_items VALUES(29812);
 INSERT INTO ub_items VALUES(29816);
 INSERT INTO ub_items VALUES(29818);
 INSERT INTO ub_items VALUES(29820);
+INSERT INTO ub_items VALUES(31337);
+INSERT INTO ub_items VALUES(31338);
+INSERT INTO ub_items VALUES(31339);
+INSERT INTO ub_items VALUES(31340);
+INSERT INTO ub_items VALUES(31341);
+INSERT INTO ub_items VALUES(31343);
+INSERT INTO ub_items VALUES(31344);
+INSERT INTO ub_items VALUES(31345);
+INSERT INTO ub_items VALUES(31346);
+INSERT INTO ub_items VALUES(31347);
+INSERT INTO ub_items VALUES(31348);
+INSERT INTO ub_items VALUES(31349);
+INSERT INTO ub_items VALUES(31350);
+INSERT INTO ub_items VALUES(31351);
+INSERT INTO ub_items VALUES(31352);
+INSERT INTO ub_items VALUES(31353);
+INSERT INTO ub_items VALUES(31354);
+INSERT INTO ub_items VALUES(31355);
+INSERT INTO ub_items VALUES(31356);
+INSERT INTO ub_items VALUES(31357);
+INSERT INTO ub_items VALUES(31358);
+INSERT INTO ub_items VALUES(31359);
+INSERT INTO ub_items VALUES(31360);
+INSERT INTO ub_items VALUES(31380);
+INSERT INTO ub_items VALUES(31381);
 CREATE TABLE pvp_items (
     item_id INTEGER NOT NULL REFERENCES items(item_id),
     PRIMARY KEY (item_id)
 ) STRICT, WITHOUT ROWID ;
 INSERT INTO pvp_items VALUES(19242);
 INSERT INTO pvp_items VALUES(19243);
 INSERT INTO pvp_items VALUES(19244);
```

## wakautosolver/data/items.sql

```diff
@@ -20443,14 +20443,15 @@
 INSERT INTO recipes VALUES(31466,0,0);
 
 DROP TABLE IF EXISTS ub_items;
 CREATE TABLE ub_items (
     item_id INTEGER NOT NULL REFERENCES items(item_id),
     PRIMARY KEY (item_id)
 ) STRICT, WITHOUT ROWID ;
+INSERT INTO ub_items VALUES(3195);
 INSERT INTO ub_items VALUES(8247);
 INSERT INTO ub_items VALUES(8248);
 INSERT INTO ub_items VALUES(8249);
 INSERT INTO ub_items VALUES(12381);
 INSERT INTO ub_items VALUES(12382);
 INSERT INTO ub_items VALUES(12383);
 INSERT INTO ub_items VALUES(12384);
@@ -20872,14 +20873,39 @@
 INSERT INTO ub_items VALUES(29806);
 INSERT INTO ub_items VALUES(29808);
 INSERT INTO ub_items VALUES(29810);
 INSERT INTO ub_items VALUES(29812);
 INSERT INTO ub_items VALUES(29816);
 INSERT INTO ub_items VALUES(29818);
 INSERT INTO ub_items VALUES(29820);
+INSERT INTO ub_items VALUES(31337);
+INSERT INTO ub_items VALUES(31338);
+INSERT INTO ub_items VALUES(31339);
+INSERT INTO ub_items VALUES(31340);
+INSERT INTO ub_items VALUES(31341);
+INSERT INTO ub_items VALUES(31343);
+INSERT INTO ub_items VALUES(31344);
+INSERT INTO ub_items VALUES(31345);
+INSERT INTO ub_items VALUES(31346);
+INSERT INTO ub_items VALUES(31347);
+INSERT INTO ub_items VALUES(31348);
+INSERT INTO ub_items VALUES(31349);
+INSERT INTO ub_items VALUES(31350);
+INSERT INTO ub_items VALUES(31351);
+INSERT INTO ub_items VALUES(31352);
+INSERT INTO ub_items VALUES(31353);
+INSERT INTO ub_items VALUES(31354);
+INSERT INTO ub_items VALUES(31355);
+INSERT INTO ub_items VALUES(31356);
+INSERT INTO ub_items VALUES(31357);
+INSERT INTO ub_items VALUES(31358);
+INSERT INTO ub_items VALUES(31359);
+INSERT INTO ub_items VALUES(31360);
+INSERT INTO ub_items VALUES(31380);
+INSERT INTO ub_items VALUES(31381);
 
 DROP TABLE IF EXISTS unobtainable_items;
 CREATE TABLE unobtainable_items (
     item_id INTEGER NOT NULL REFERENCES items(item_id),
     PRIMARY KEY (item_id)
 ) STRICT, WITHOUT ROWID ;
 INSERT INTO unobtainable_items VALUES(20790);
```

## wakautosolver/data/source_info.bz2

### source_info

```diff
@@ -180,94 +180,99 @@
 00000b30: 5fd7 cd5f d8cd 5fd9 cd5f dacd 5fdb cd5f  _.._.._.._.._.._
 00000b40: dccd 5fdd cd5f decd 5fdf cd5f e0cd 5fe1  .._.._.._.._.._.
 00000b50: cd5f e2cd 5fe3 cd5f e4cd 5fe5 cd5f e6cd  ._.._.._.._.._..
 00000b60: 5fe7 cd5f e8cd 5fe9 cd5f eacd 5feb cd5f  _.._.._.._.._.._
 00000b70: eccd 5fed cd5f eecd 5fef cd5f f0cd 5ff1  .._.._.._.._.._.
 00000b80: cd5f f2cd 5ff3 cd5f f4cd 5ff5 cd5f f6cd  ._.._.._.._.._..
 00000b90: 5ff7 cd5f f8cd 5ff9 cd5f facd 5ffb cd5f  _.._.._.._.._.._
-00000ba0: fccd 5ffd cd5f fecd 5fff dc01 adcd 5800  .._.._.._.....X.
+00000ba0: fccd 5ffd cd5f fecd 5fff dc01 c7cd 5800  .._.._.._.....X.
 00000bb0: cd58 01cd 5802 cd58 03cd 5804 cd58 05cd  .X..X..X..X..X..
 00000bc0: 5806 cd58 07cd 5808 cd20 37cd 2038 cd20  X..X..X.. 7. 8. 
 00000bd0: 39cd 305d cd30 5ecd 305f cd30 60cd 3061  9.0].0^.0_.0`.0a
-00000be0: cd30 62cd 30c4 cd30 c8cd 60da cd60 dbcd  .0b.0..0..`..`..
-00000bf0: 50ef cd50 f0cd 50f2 cd50 f3cd 50f4 cd50  P..P..P..P..P..P
-00000c00: f5cd 50f6 cd50 f7cd 50f8 cd50 f9cd 50fa  ..P..P..P..P..P.
-00000c10: cd50 fbcd 50fc cd50 fdcd 50fe cd50 ffcd  .P..P..P..P..P..
-00000c20: 312c cd31 2dcd 69b8 cd69 b9cd 69ba cd31  1,.1-.i..i..i..1
-00000c30: dfcd 31e0 cd31 e1cd 31e2 cd42 45cd 4246  ..1..1..1..BE.BF
-00000c40: cd42 47cd 6a47 cd42 49cd 424a cd42 4bcd  .BG.jG.BI.BJ.BK.
-00000c50: 424c cd42 4ecd 424f cd42 50cd 4251 cd42  BL.BN.BO.BP.BQ.B
-00000c60: 6fcd 5a86 cd5a 87cd 5a88 cd5a 89cd 5a8b  o.Z..Z..Z..Z..Z.
-00000c70: cd5a 8dcd 5a8e cd5a 8fcd 5a90 cd5a 91cd  .Z..Z..Z..Z..Z..
-00000c80: 5a92 cd5a 93cd 5a94 cd5a 95cd 5a97 cd5a  Z..Z..Z..Z..Z..Z
-00000c90: 98cd 5a99 cd5a 9acd 5a9b cd5a 9ccd 5a9d  ..Z..Z..Z..Z..Z.
-00000ca0: cd5a 9ecd 5a9f cd5a a0cd 5aa1 cd5a a2cd  .Z..Z..Z..Z..Z..
-00000cb0: 5aa5 cd5a a6cd 5aa7 cd5a a8cd 730e cd73  Z..Z..Z..Z..s..s
-00000cc0: 0fcd 7310 cd73 11cd 7312 cd73 13cd 7314  ..s..s..s..s..s.
-00000cd0: cd73 15cd 7316 cd73 17cd 7318 cd73 19cd  .s..s..s..s..s..
-00000ce0: 731a cd73 1bcd 731c cd73 1dcd 731e cd73  s..s..s..s..s..s
-00000cf0: 1fcd 7320 cd73 21cd 7322 cd73 23cd 7324  ..s .s!.s".s#.s$
-00000d00: cd73 25cd 7326 cd73 27cd 7328 cd73 29cd  .s%.s&.s'.s(.s).
-00000d10: 732a cd73 2bcd 732c cd73 2dcd 732e cd73  s*.s+.s,.s-.s..s
-00000d20: 2fcd 7330 cd73 31cd 7332 cd73 33cd 7334  /.s0.s1.s2.s3.s4
-00000d30: cd73 4ccd 734d cd73 4ecd 734f cd73 50cd  .sL.sM.sN.sO.sP.
-00000d40: 7351 cd73 52cd 7353 cd73 54cd 7355 cd73  sQ.sR.sS.sT.sU.s
-00000d50: 56cd 7357 cd73 58cd 7359 cd73 5acd 735b  V.sW.sX.sY.sZ.s[
-00000d60: cd73 5ccd 735d cd73 5ecd 735f cd73 60cd  .s\.s].s^.s_.s`.
-00000d70: 7361 cd73 62cd 7363 cd73 64cd 7365 cd73  sa.sb.sc.sd.se.s
-00000d80: 66cd 7367 cd73 68cd 7369 cd73 6acd 736b  f.sg.sh.si.sj.sk
-00000d90: cd73 b6cd 73b7 cd73 b8cd 73b9 cd73 bacd  .s..s..s..s..s..
-00000da0: 73bb cd73 bccd 73bd cd73 becd 73bf cd73  s..s..s..s..s..s
-00000db0: c0cd 73c1 cd73 c2cd 73c3 cd73 c4cd 73c5  ..s..s..s..s..s.
-00000dc0: cd73 c6cd 73c7 cd73 c8cd 73c9 cd73 cacd  .s..s..s..s..s..
-00000dd0: 73cb cd73 cccd 73cd cd73 cecd 4bd2 cd4b  s..s..s..s..K..K
-00000de0: d3cd 4bd4 cd4b d5cd 4bd6 cd4b d7cd 4bd8  ..K..K..K..K..K.
-00000df0: cd4b d9cd 4bdc cd4b ddcd 4bde cd4b dfcd  .K..K..K..K..K..
-00000e00: 4be0 cd4b e1cd 4be2 cd4b e3cd 4be5 cd4b  K..K..K..K..K..K
-00000e10: e6cd 4be7 cd4b e8cd 6c28 cd6c 29cd 6c2a  ..K..K..l(.l).l*
-00000e20: cd6c 2bcd 6c2c cd6c 2dcd 6c2e cd6c 2fcd  .l+.l,.l-.l..l/.
-00000e30: 746c cd74 6ecd 7470 cd74 72cd 7474 cd74  tl.tn.tp.tr.tt.t
-00000e40: 78cd 747a cd74 7ccd 6c9e cd6c a0cd 5d23  x.tz.t|.l..l..]#
-00000e50: cd5d 24cd 5d25 cd5d 26cd 5d27 cd5d 28cd  .]$.]%.]&.]'.](.
-00000e60: 5d2a cd5d 2bcd 5d2c cd5d 2dcd 5d2f cd5d  ]*.]+.],.]-.]/.]
-00000e70: 30cd 5d31 cd5d 34cd 5d37 cd5d 9dcd 5d9f  0.]1.]4.]7.]..].
-00000e80: cd5d a0cd 5da1 cd5d a2cd 5da3 cd5d a4cd  .]..]..]..]..]..
-00000e90: 5da5 cd5d a6cd 5da7 cd5d a8cd 5da9 cd5d  ]..]..]..]..]..]
-00000ea0: aacd 5dab cd5d accd 5dad cd5d aecd 5daf  ..]..]..]..]..].
-00000eb0: cd5d b0cd 5db1 cd5d b2cd 5db3 cd5d b4cd  .]..]..]..]..]..
-00000ec0: 5db5 cd5d b6cd 5db7 cd5d b8cd 5dba cd5d  ]..]..]..]..]..]
-00000ed0: bbcd 5dbc cd5d bdcd 5dbe cd5d bfcd 5dc0  ..]..]..]..]..].
-00000ee0: cd5d c1cd 5dc2 cd5d c3cd 5dc4 cd5d c5cd  .]..]..]..]..]..
-00000ef0: 5dc6 cd5d c7cd 5dc8 cd5d c9cd 5dca cd5d  ]..]..]..]..]..]
-00000f00: cbcd 5dcc cd5d cecd 5dcf cd5d d0cd 5dd1  ..]..]..]..]..].
-00000f10: cd5d d2cd 5dd3 cd5d d4cd 5dd5 cd5d d6cd  .]..]..]..]..]..
-00000f20: 5dd7 cd5d d8cd 5dd9 cd5d dacd 5ddb cd5d  ]..]..]..]..]..]
-00000f30: dccd 3deb cd5e 39cd 6696 cd66 97cd 6698  ..=..^9.f..f..f.
-00000f40: cd66 99cd 669a cd66 9bcd 669c cd66 9dcd  .f..f..f..f..f..
-00000f50: 66af cd66 b0cd 66b1 cd66 b2cd 66b3 cd66  f..f..f..f..f..f
-00000f60: b4cd 66b5 cd66 b6cd 66b7 cd66 b8cd 66b9  ..f..f..f..f..f.
-00000f70: cd66 bacd 66bb cd66 bccd 66bd cd66 becd  .f..f..f..f..f..
-00000f80: 66bf cd66 c0cd 66c6 cd66 c7cd 66c8 cd66  f..f..f..f..f..f
-00000f90: c9cd 66ca cd66 cbcd 66cc cd66 cdcd 66ce  ..f..f..f..f..f.
-00000fa0: cd66 cfcd 66d1 cd66 d2cd 66d3 cd66 d4cd  .f..f..f..f..f..
-00000fb0: 6ef9 cd6e facd 4f16 cd4f 17cd 4f18 cd4f  n..n..O..O..O..O
-00000fc0: 19cd 4f1a cd4f 1bcd 4f1c cd4f 1dcd 3723  ..O..O..O..O..7#
-00000fd0: cd37 24cd 3725 cd37 26cd 3727 cd37 28cd  .7$.7%.7&.7'.7(.
-00000fe0: 3729 cd37 2acd 372b cd37 2ccd 372d cd37  7).7*.7+.7,.7-.7
-00000ff0: 30cd 3731 cd37 33cd 3734 cd4f 35cd 3736  0.71.73.74.O5.76
-00001000: cd4f 37cd 3737 cd37 38cd 3739 cd37 3acd  .O7.77.78.79.7:.
-00001010: 4f36 cd37 3ccd 373d cd37 3ecd 373f cd37  O6.7<.7=.7>.7?.7
-00001020: 40cd 4f39 cd37 43cd 4f45 cd4f 46cd 4f47  @.O9.7C.OE.OF.OG
-00001030: cd4f 8acd 4f8b cd4f 8ccd 4f8d cd4f 8fcd  .O..O..O..O..O..
-00001040: 4f90 cd4f 91cd 57aa cd57 abcd 57ac cd57  O..O..W..W..W..W
-00001050: adcd 57ae cd57 afcd 57b0 cd57 b1cd 57b2  ..W..W..W..W..W.
-00001060: cd57 b3cd 57b4 cd57 b5cd 57b6 cd57 bfcd  .W..W..W..W..W..
-00001070: 57c0 cd57 c1cd 57c2 cd57 c3cd 57c4 cd57  W..W..W..W..W..W
-00001080: c5cd 67c6 cd67 c7cd 67c8 cd57 c6cd 57c7  ..g..g..g..W..W.
-00001090: cd57 c8cd 57c9 cd57 cacd 57cb cd67 c9cd  .W..W..W..W..g..
-000010a0: 67cc cd57 d9cd 57fb cd57 fccd 57fd cd57  g..W..W..W..W..W
-000010b0: fecd 57ff dc00 1ccd 3bb4 cd3b b5cd 3bb6  ..W.....;..;..;.
-000010c0: cd3b b7cd 3bb8 cd3b b9cd 3bba cd3b bbcd  .;..;..;..;..;..
-000010d0: 3bbc cd3b bdcd 3bbe cd3b bfcd 3bc0 cd3b  ;..;..;..;..;..;
-000010e0: c1cd 3bc2 cd3b c3cd 48ee cd48 efcd 48f0  ..;..;..H..H..H.
-000010f0: cd48 f1cd 48f2 cd48 f3cd 48f4 cd48 f5cd  .H..H..H..H..H..
-00001100: 48f6 cd48 f7cd 48f8 cd48 f9              H..H..H..H.
+00000be0: cd30 62cd 7a95 cd30 c4cd 30c8 cd60 dacd  .0b.z..0..0..`..
+00000bf0: 60db cd50 efcd 50f0 cd50 f2cd 50f3 cd50  `..P..P..P..P..P
+00000c00: f4cd 50f5 cd50 f6cd 50f7 cd50 f8cd 50f9  ..P..P..P..P..P.
+00000c10: cd50 facd 50fb cd50 fccd 50fd cd50 fecd  .P..P..P..P..P..
+00000c20: 50ff cd31 2ccd 312d cd69 b8cd 69b9 cd69  P..1,.1-.i..i..i
+00000c30: bacd 31df cd31 e0cd 31e1 cd31 e2cd 4245  ..1..1..1..1..BE
+00000c40: cd42 46cd 4247 cd6a 47cd 4249 cd42 4acd  .BF.BG.jG.BI.BJ.
+00000c50: 424b cd42 4ccd 424e cd42 4fcd 4250 cd42  BK.BL.BN.BO.BP.B
+00000c60: 51cd 7a69 cd7a 6acd 7a6b cd7a 6ccd 7a6d  Q.zi.zj.zk.zl.zm
+00000c70: cd42 6fcd 7a6f cd7a 70cd 7a71 cd7a 72cd  .Bo.zo.zp.zq.zr.
+00000c80: 7a73 cd7a 74cd 7a75 cd7a 76cd 7a77 cd7a  zs.zt.zu.zv.zw.z
+00000c90: 78cd 7a79 cd7a 7acd 7a7b cd7a 7ccd 7a7d  x.zy.zz.z{.z|.z}
+00000ca0: cd7a 7ecd 7a7f cd7a 80cd 5a86 cd5a 87cd  .z~.z..z..Z..Z..
+00000cb0: 5a88 cd5a 89cd 5a8b cd5a 8dcd 5a8e cd5a  Z..Z..Z..Z..Z..Z
+00000cc0: 8fcd 5a90 cd5a 91cd 5a92 cd5a 93cd 5a94  ..Z..Z..Z..Z..Z.
+00000cd0: cd5a 95cd 7a94 cd5a 97cd 5a98 cd5a 99cd  .Z..z..Z..Z..Z..
+00000ce0: 5a9a cd5a 9bcd 5a9c cd5a 9dcd 5a9e cd5a  Z..Z..Z..Z..Z..Z
+00000cf0: 9fcd 5aa0 cd5a a1cd 5aa2 cd5a a5cd 5aa6  ..Z..Z..Z..Z..Z.
+00000d00: cd5a a7cd 5aa8 cd73 0ecd 730f cd73 10cd  .Z..Z..s..s..s..
+00000d10: 7311 cd73 12cd 7313 cd73 14cd 7315 cd73  s..s..s..s..s..s
+00000d20: 16cd 7317 cd73 18cd 7319 cd73 1acd 731b  ..s..s..s..s..s.
+00000d30: cd73 1ccd 731d cd73 1ecd 731f cd73 20cd  .s..s..s..s..s .
+00000d40: 7321 cd73 22cd 7323 cd73 24cd 7325 cd73  s!.s".s#.s$.s%.s
+00000d50: 26cd 7327 cd73 28cd 7329 cd73 2acd 732b  &.s'.s(.s).s*.s+
+00000d60: cd73 2ccd 732d cd73 2ecd 732f cd73 30cd  .s,.s-.s..s/.s0.
+00000d70: 7331 cd73 32cd 7333 cd73 34cd 734c cd73  s1.s2.s3.s4.sL.s
+00000d80: 4dcd 734e cd73 4fcd 7350 cd73 51cd 7352  M.sN.sO.sP.sQ.sR
+00000d90: cd73 53cd 7354 cd73 55cd 7356 cd73 57cd  .sS.sT.sU.sV.sW.
+00000da0: 7358 cd73 59cd 735a cd73 5bcd 735c cd73  sX.sY.sZ.s[.s\.s
+00000db0: 5dcd 735e cd73 5fcd 7360 cd73 61cd 7362  ].s^.s_.s`.sa.sb
+00000dc0: cd73 63cd 7364 cd73 65cd 7366 cd73 67cd  .sc.sd.se.sf.sg.
+00000dd0: 7368 cd73 69cd 736a cd73 6bcd 73b6 cd73  sh.si.sj.sk.s..s
+00000de0: b7cd 73b8 cd73 b9cd 73ba cd73 bbcd 73bc  ..s..s..s..s..s.
+00000df0: cd73 bdcd 73be cd73 bfcd 73c0 cd73 c1cd  .s..s..s..s..s..
+00000e00: 73c2 cd73 c3cd 73c4 cd73 c5cd 73c6 cd73  s..s..s..s..s..s
+00000e10: c7cd 73c8 cd73 c9cd 73ca cd73 cbcd 73cc  ..s..s..s..s..s.
+00000e20: cd73 cdcd 73ce cd4b d2cd 4bd3 cd4b d4cd  .s..s..K..K..K..
+00000e30: 4bd5 cd4b d6cd 4bd7 cd4b d8cd 4bd9 cd4b  K..K..K..K..K..K
+00000e40: dccd 4bdd cd4b decd 4bdf cd4b e0cd 4be1  ..K..K..K..K..K.
+00000e50: cd4b e2cd 4be3 cd4b e5cd 4be6 cd4b e7cd  .K..K..K..K..K..
+00000e60: 4be8 cd6c 28cd 6c29 cd6c 2acd 6c2b cd6c  K..l(.l).l*.l+.l
+00000e70: 2ccd 6c2d cd6c 2ecd 6c2f cd74 6ccd 746e  ,.l-.l..l/.tl.tn
+00000e80: cd74 70cd 7472 cd74 74cd 7478 cd74 7acd  .tp.tr.tt.tx.tz.
+00000e90: 0c7b cd74 7ccd 6c9e cd6c a0cd 5d23 cd5d  .{.t|.l..l..]#.]
+00000ea0: 24cd 5d25 cd5d 26cd 5d27 cd5d 28cd 5d2a  $.]%.]&.]'.](.]*
+00000eb0: cd5d 2bcd 5d2c cd5d 2dcd 5d2f cd5d 30cd  .]+.],.]-.]/.]0.
+00000ec0: 5d31 cd5d 34cd 5d37 cd5d 9dcd 5d9f cd5d  ]1.]4.]7.]..]..]
+00000ed0: a0cd 5da1 cd5d a2cd 5da3 cd5d a4cd 5da5  ..]..]..]..]..].
+00000ee0: cd5d a6cd 5da7 cd5d a8cd 5da9 cd5d aacd  .]..]..]..]..]..
+00000ef0: 5dab cd5d accd 5dad cd5d aecd 5daf cd5d  ]..]..]..]..]..]
+00000f00: b0cd 5db1 cd5d b2cd 5db3 cd5d b4cd 5db5  ..]..]..]..]..].
+00000f10: cd5d b6cd 5db7 cd5d b8cd 5dba cd5d bbcd  .]..]..]..]..]..
+00000f20: 5dbc cd5d bdcd 5dbe cd5d bfcd 5dc0 cd5d  ]..]..]..]..]..]
+00000f30: c1cd 5dc2 cd5d c3cd 5dc4 cd5d c5cd 5dc6  ..]..]..]..]..].
+00000f40: cd5d c7cd 5dc8 cd5d c9cd 5dca cd5d cbcd  .]..]..]..]..]..
+00000f50: 5dcc cd5d cecd 5dcf cd5d d0cd 5dd1 cd5d  ]..]..]..]..]..]
+00000f60: d2cd 5dd3 cd5d d4cd 5dd5 cd5d d6cd 5dd7  ..]..]..]..]..].
+00000f70: cd5d d8cd 5dd9 cd5d dacd 5ddb cd5d dccd  .]..]..]..]..]..
+00000f80: 3deb cd5e 39cd 6696 cd66 97cd 6698 cd66  =..^9.f..f..f..f
+00000f90: 99cd 669a cd66 9bcd 669c cd66 9dcd 66af  ..f..f..f..f..f.
+00000fa0: cd66 b0cd 66b1 cd66 b2cd 66b3 cd66 b4cd  .f..f..f..f..f..
+00000fb0: 66b5 cd66 b6cd 66b7 cd66 b8cd 66b9 cd66  f..f..f..f..f..f
+00000fc0: bacd 66bb cd66 bccd 66bd cd66 becd 66bf  ..f..f..f..f..f.
+00000fd0: cd66 c0cd 66c6 cd66 c7cd 66c8 cd66 c9cd  .f..f..f..f..f..
+00000fe0: 66ca cd66 cbcd 66cc cd66 cdcd 66ce cd66  f..f..f..f..f..f
+00000ff0: cfcd 66d1 cd66 d2cd 66d3 cd66 d4cd 6ef9  ..f..f..f..f..n.
+00001000: cd6e facd 4f16 cd4f 17cd 4f18 cd4f 19cd  .n..O..O..O..O..
+00001010: 4f1a cd4f 1bcd 4f1c cd4f 1dcd 3723 cd37  O..O..O..O..7#.7
+00001020: 24cd 3725 cd37 26cd 3727 cd37 28cd 3729  $.7%.7&.7'.7(.7)
+00001030: cd37 2acd 372b cd37 2ccd 372d cd37 30cd  .7*.7+.7,.7-.70.
+00001040: 3731 cd37 33cd 3734 cd4f 35cd 3736 cd4f  71.73.74.O5.76.O
+00001050: 37cd 3737 cd37 38cd 3739 cd37 3acd 4f36  7.77.78.79.7:.O6
+00001060: cd37 3ccd 373d cd37 3ecd 373f cd37 40cd  .7<.7=.7>.7?.7@.
+00001070: 4f39 cd37 43cd 4f45 cd4f 46cd 4f47 cd4f  O9.7C.OE.OF.OG.O
+00001080: 8acd 4f8b cd4f 8ccd 4f8d cd4f 8fcd 4f90  ..O..O..O..O..O.
+00001090: cd4f 91cd 57aa cd57 abcd 57ac cd57 adcd  .O..W..W..W..W..
+000010a0: 57ae cd57 afcd 57b0 cd57 b1cd 57b2 cd57  W..W..W..W..W..W
+000010b0: b3cd 57b4 cd57 b5cd 57b6 cd57 bfcd 57c0  ..W..W..W..W..W.
+000010c0: cd57 c1cd 57c2 cd57 c3cd 57c4 cd57 c5cd  .W..W..W..W..W..
+000010d0: 67c6 cd67 c7cd 57c6 cd57 c7cd 57c8 cd57  g..g..W..W..W..W
+000010e0: c9cd 57ca cd57 cbcd 67c8 cd67 c9cd 67cc  ..W..W..g..g..g.
+000010f0: cd57 d9cd 57fb cd57 fccd 57fd cd57 fecd  .W..W..W..W..W..
+00001100: 57ff dc00 1ccd 3bb4 cd3b b5cd 3bb6 cd3b  W.....;..;..;..;
+00001110: b7cd 3bb8 cd3b b9cd 3bba cd3b bbcd 3bbc  ..;..;..;..;..;.
+00001120: cd3b bdcd 3bbe cd3b bfcd 3bc0 cd3b c1cd  .;..;..;..;..;..
+00001130: 3bc2 cd3b c3cd 48ee cd48 efcd 48f0 cd48  ;..;..H..H..H..H
+00001140: f1cd 48f2 cd48 f3cd 48f4 cd48 f5cd 48f6  ..H..H..H..H..H.
+00001150: cd48 f7cd 48f8 cd48 f9                   .H..H..H.
```

## Comparing `wakautosolver-2024.4.1.dist-info/METADATA` & `wakautosolver-2024.4.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wakautosolver
-Version: 2024.4.1
+Version: 2024.4.2
 Project-URL: Homepage, https://github.com/mikeshardmind/wakfu-utils
 Author-email: Michael Hall <michael@michaelhall.tech>
 License-Expression: MPL-2.0
 License-File: LICENSE
 Requires-Python: >=3.11
 Requires-Dist: msgspec>=0.18.4
 Requires-Dist: tqdm>=4.66.1
```

## Comparing `wakautosolver-2024.4.1.dist-info/licenses/LICENSE` & `wakautosolver-2024.4.2.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `wakautosolver-2024.4.1.dist-info/RECORD` & `wakautosolver-2024.4.2.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 LICENSE,sha256=HyVuytGSiAUQ6ErWBHTqt1iSGHhLmlC8fO7jTCuR8dU,16725
 .venv/Lib/site-packages/scripts/item_data.bz2,sha256=f_QL9zVv3F1o1zt0tCyqb5-UOQ1hTxsvTtD-p-ZYFAU,453356
 .venv/Lib/site-packages/scripts/locale_bundle.bz2,sha256=vZRfALj01hgsmGrlDPpYgGaK9oEXnhrfJusqHTXCKHY,137411
 scripts/item_data.bz2,sha256=f_QL9zVv3F1o1zt0tCyqb5-UOQ1hTxsvTtD-p-ZYFAU,453356
-wakautosolver/__init__.py,sha256=UZjKXBsIAZuzC80tpcRktEb2Rd_ORn-MfQsmioylwmM,510
+wakautosolver/__init__.py,sha256=8m6xaTfGCJuL5scSueFzA_dukcq-SkZ2vouffrniW2o,510
 wakautosolver/__main__.py,sha256=UtGrY1NrAkSGgj2e5SBkbmgRFMuojHZZr0ZE25x-UVY,764
 wakautosolver/_build_codes.py,sha256=oTgmSQqZJYa-SVv4dL1ctVxGtz9gkvGR0mi0vkPPK1E,3851
 wakautosolver/_short_debug_info.py,sha256=8Dq1NJugZJBGWxlcjj5M5gAmXCWpaiqA0Bq2UOB-S7w,1274
 wakautosolver/_typing_memes.py,sha256=ygR25rAn58tPoflK4iZzU45B8e94cii1cqcAkQ6biVQ,1713
 wakautosolver/item_conditions.py,sha256=KnlUyLunO4dY_oO9rtX8cYhYv08kBMgCz0V2ghK-IDk,4466
 wakautosolver/object_parsing.py,sha256=Sb-YhvizUmiwNpkrxroMvjv1E48Oco-xIt5a0G4SgE4,11384
 wakautosolver/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -15,17 +15,17 @@
 wakautosolver/utils.py,sha256=KtuyMFKwOj4J1FMKyVTTuSVbQl3Eqw9GLSZLtaDAiRM,674
 wakautosolver/versioned_entrypoints.py,sha256=YceV9aIlzAn6L0LjGdqr3fainkANGeG3_oDyl5hIRnE,12530
 wakautosolver/wakforge_buildcodes.py,sha256=-xlIEkp4yV_lbkAH7eSNvlyMFHc6pnzeKO_1GmPlopQ,7126
 wakautosolver/b2048/__init__.py,sha256=AbMdWj28dc94x-b-_NuF6uXrZ4eeUU2ZG9nDj8hq_jM,366
 wakautosolver/b2048/dec_table.py,sha256=1LZWoaSeQWs7OeSzkmrYA4FkoSSnDJK_y83gkqRZqQM,49861
 wakautosolver/b2048/enc_table.py,sha256=RE5kddBNQarcYjLbDxK-edOpP4iO5TgqyRoHQdpvHHk,21610
 wakautosolver/b2048/encoder.py,sha256=q8U17Vb-3pVNPxoAnKXEzhzzZDgZPxRNjk7UBnliV0s,3634
-wakautosolver/data/items.db,sha256=05r44aWzqq6UOOOE7s0mNlqG-cF7TOavO712rHI2lJI,1212416
-wakautosolver/data/items.sql,sha256=mLibF8OyWGkU5k_BxWi8jPh1Ca_K3Ad0wWqG9a4JcHE,1991094
+wakautosolver/data/items.db,sha256=1YD6rj7orqZLYpzFvp7rtWxP40EB4ORsYtABY6AMmzE,1212416
+wakautosolver/data/items.sql,sha256=JVdEiOL0orOhBCnMzSwUgxFVjn8SH-Ru9UZvgUkromk,1992029
 wakautosolver/data/locale_bundle.bz2,sha256=qPnB2vjm0f6lx4L0Q3sG4ERn1a3wnWyyhj7OP67Fn_g,137716
 wakautosolver/data/readme.md,sha256=GQ8oPIi_oTVznNypRYsq6v-ptAKPTILRFI3OIJzsYko,75
-wakautosolver/data/source_info.bz2,sha256=bvcp26CdQXyDfP1YtrLMjeKrPEEhLU7g1mCTMeWIQUc,2779
+wakautosolver/data/source_info.bz2,sha256=GFoA1pup08aQLCFcwMSbqkEC_5kX9lQoTKdr3KsdRJ0,2816
 wakautosolver/data/stat_only_bundle.bz2,sha256=Yo2hDD3m96Ow10hxHXdoVqspJahe19yW3QFV71CY-cM,85259
-wakautosolver-2024.4.1.dist-info/METADATA,sha256=MFDL3D7butUJI7R7ywATu0ZvsTpDiJBjWZfwZdci4gM,6104
-wakautosolver-2024.4.1.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
-wakautosolver-2024.4.1.dist-info/licenses/LICENSE,sha256=HyVuytGSiAUQ6ErWBHTqt1iSGHhLmlC8fO7jTCuR8dU,16725
-wakautosolver-2024.4.1.dist-info/RECORD,,
+wakautosolver-2024.4.2.dist-info/METADATA,sha256=1ftNH0xnpcDhStqp8G3meKYXlAQRgfcE6bt0vpPK1xc,6104
+wakautosolver-2024.4.2.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
+wakautosolver-2024.4.2.dist-info/licenses/LICENSE,sha256=HyVuytGSiAUQ6ErWBHTqt1iSGHhLmlC8fO7jTCuR8dU,16725
+wakautosolver-2024.4.2.dist-info/RECORD,,
```

