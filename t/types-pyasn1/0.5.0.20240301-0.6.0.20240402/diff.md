# Comparing `tmp/types-pyasn1-0.5.0.20240301.tar.gz` & `tmp/types-pyasn1-0.6.0.20240402.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-pyasn1-0.5.0.20240301.tar", last modified: Fri Mar  1 02:18:04 2024, max compression
+gzip compressed data, was "types-pyasn1-0.6.0.20240402.tar", last modified: Tue Apr  2 02:17:18 2024, max compression
```

## Comparing `types-pyasn1-0.5.0.20240301.tar` & `types-pyasn1-0.6.0.20240402.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 02:18:04.212147 types-pyasn1-0.5.0.20240301/
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-03-01 02:18:03.000000 types-pyasn1-0.5.0.20240301/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-01 02:18:03.000000 types-pyasn1-0.5.0.20240301/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-03-01 02:18:04.212147 types-pyasn1-0.5.0.20240301/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 02:18:04.204147 types-pyasn1-0.5.0.20240301/pyasn1-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-01 02:18:03.000000 types-pyasn1-0.5.0.20240301/pyasn1-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-01 02:17:43.000000 types-pyasn1-0.5.0.20240301/pyasn1-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 02:18:04.208147 types-pyasn1-0.5.0.20240301/pyasn1-stubs/codec/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 02:17:43.000000 types-pyasn1-0.5.0.20240301/pyasn1-stubs/codec/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 02:18:04.208147 types-pyasn1-0.5.0.20240301/pyasn1-stubs/codec/ber/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 02:17:43.000000 types-pyasn1-0.5.0.20240301/pyasn1-stubs/codec/ber/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10976 2024-03-01 02:17:43.000000 types-pyasn1-0.5.0.20240301/pyasn1-stubs/codec/ber/decoder.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-03-01 02:17:43.000000 types-pyasn1-0.5.0.20240301/pyasn1-stubs/codec/ber/encoder.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-01 02:17:43.000000 types-pyasn1-0.5.0.20240301/pyasn1-stubs/codec/ber/eoo.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 02:18:04.208147 types-pyasn1-0.5.0.20240301/pyasn1-stubs/codec/cer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 02:17:43.000000 types-pyasn1-0.5.0.20240301/pyasn1-stubs/codec/cer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-03-01 02:17:43.000000 types-pyasn1-0.5.0.20240301/pyasn1-stubs/codec/cer/decoder.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-03-01 02:17:43.000000 types-pyasn1-0.5.0.20240301/pyasn1-stubs/codec/cer/encoder.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 02:18:04.208147 types-pyasn1-0.5.0.20240301/pyasn1-stubs/codec/der/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 02:17:43.000000 types-pyasn1-0.5.0.20240301/pyasn1-stubs/codec/der/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-03-01 02:17:43.000000 types-pyasn1-0.5.0.20240301/pyasn1-stubs/codec/der/decoder.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-03-01 02:17:43.000000 types-pyasn1-0.5.0.20240301/pyasn1-stubs/codec/der/encoder.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 02:18:04.208147 types-pyasn1-0.5.0.20240301/pyasn1-stubs/codec/native/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 02:17:43.000000 types-pyasn1-0.5.0.20240301/pyasn1-stubs/codec/native/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-03-01 02:17:43.000000 types-pyasn1-0.5.0.20240301/pyasn1-stubs/codec/native/decoder.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-03-01 02:17:43.000000 types-pyasn1-0.5.0.20240301/pyasn1-stubs/codec/native/encoder.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-03-01 02:17:43.000000 types-pyasn1-0.5.0.20240301/pyasn1-stubs/codec/streaming.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 02:18:04.208147 types-pyasn1-0.5.0.20240301/pyasn1-stubs/compat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 02:17:43.000000 types-pyasn1-0.5.0.20240301/pyasn1-stubs/compat/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-01 02:17:43.000000 types-pyasn1-0.5.0.20240301/pyasn1-stubs/compat/integer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-01 02:17:43.000000 types-pyasn1-0.5.0.20240301/pyasn1-stubs/compat/octets.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-01 02:17:43.000000 types-pyasn1-0.5.0.20240301/pyasn1-stubs/debug.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-01 02:17:43.000000 types-pyasn1-0.5.0.20240301/pyasn1-stubs/error.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 02:18:04.208147 types-pyasn1-0.5.0.20240301/pyasn1-stubs/type/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 02:17:43.000000 types-pyasn1-0.5.0.20240301/pyasn1-stubs/type/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-03-01 02:17:43.000000 types-pyasn1-0.5.0.20240301/pyasn1-stubs/type/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-03-01 02:17:43.000000 types-pyasn1-0.5.0.20240301/pyasn1-stubs/type/char.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-03-01 02:17:43.000000 types-pyasn1-0.5.0.20240301/pyasn1-stubs/type/constraint.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-01 02:17:43.000000 types-pyasn1-0.5.0.20240301/pyasn1-stubs/type/error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-03-01 02:17:43.000000 types-pyasn1-0.5.0.20240301/pyasn1-stubs/type/namedtype.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-01 02:17:43.000000 types-pyasn1-0.5.0.20240301/pyasn1-stubs/type/namedval.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-01 02:17:43.000000 types-pyasn1-0.5.0.20240301/pyasn1-stubs/type/opentype.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-03-01 02:17:43.000000 types-pyasn1-0.5.0.20240301/pyasn1-stubs/type/tag.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-03-01 02:17:43.000000 types-pyasn1-0.5.0.20240301/pyasn1-stubs/type/tagmap.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13396 2024-03-01 02:17:43.000000 types-pyasn1-0.5.0.20240301/pyasn1-stubs/type/univ.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-01 02:17:43.000000 types-pyasn1-0.5.0.20240301/pyasn1-stubs/type/useful.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 02:18:04.212147 types-pyasn1-0.5.0.20240301/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-03-01 02:18:03.000000 types-pyasn1-0.5.0.20240301/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 02:18:04.212147 types-pyasn1-0.5.0.20240301/types_pyasn1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-03-01 02:18:04.000000 types-pyasn1-0.5.0.20240301/types_pyasn1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-03-01 02:18:04.000000 types-pyasn1-0.5.0.20240301/types_pyasn1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 02:18:04.000000 types-pyasn1-0.5.0.20240301/types_pyasn1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-01 02:18:04.000000 types-pyasn1-0.5.0.20240301/types_pyasn1.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:18.068228 types-pyasn1-0.6.0.20240402/
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-02 02:17:16.000000 types-pyasn1-0.6.0.20240402/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-02 02:17:16.000000 types-pyasn1-0.6.0.20240402/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-02 02:17:18.068228 types-pyasn1-0.6.0.20240402/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:18.064228 types-pyasn1-0.6.0.20240402/pyasn1-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-02 02:17:16.000000 types-pyasn1-0.6.0.20240402/pyasn1-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-02 02:17:07.000000 types-pyasn1-0.6.0.20240402/pyasn1-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:18.064228 types-pyasn1-0.6.0.20240402/pyasn1-stubs/codec/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:07.000000 types-pyasn1-0.6.0.20240402/pyasn1-stubs/codec/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:18.064228 types-pyasn1-0.6.0.20240402/pyasn1-stubs/codec/ber/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:07.000000 types-pyasn1-0.6.0.20240402/pyasn1-stubs/codec/ber/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10976 2024-04-02 02:17:07.000000 types-pyasn1-0.6.0.20240402/pyasn1-stubs/codec/ber/decoder.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-02 02:17:07.000000 types-pyasn1-0.6.0.20240402/pyasn1-stubs/codec/ber/encoder.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-02 02:17:07.000000 types-pyasn1-0.6.0.20240402/pyasn1-stubs/codec/ber/eoo.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:18.064228 types-pyasn1-0.6.0.20240402/pyasn1-stubs/codec/cer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:07.000000 types-pyasn1-0.6.0.20240402/pyasn1-stubs/codec/cer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-02 02:17:07.000000 types-pyasn1-0.6.0.20240402/pyasn1-stubs/codec/cer/decoder.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-02 02:17:07.000000 types-pyasn1-0.6.0.20240402/pyasn1-stubs/codec/cer/encoder.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:18.064228 types-pyasn1-0.6.0.20240402/pyasn1-stubs/codec/der/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:07.000000 types-pyasn1-0.6.0.20240402/pyasn1-stubs/codec/der/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-02 02:17:07.000000 types-pyasn1-0.6.0.20240402/pyasn1-stubs/codec/der/decoder.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-02 02:17:07.000000 types-pyasn1-0.6.0.20240402/pyasn1-stubs/codec/der/encoder.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:18.064228 types-pyasn1-0.6.0.20240402/pyasn1-stubs/codec/native/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:07.000000 types-pyasn1-0.6.0.20240402/pyasn1-stubs/codec/native/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-02 02:17:07.000000 types-pyasn1-0.6.0.20240402/pyasn1-stubs/codec/native/decoder.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-02 02:17:07.000000 types-pyasn1-0.6.0.20240402/pyasn1-stubs/codec/native/encoder.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-02 02:17:07.000000 types-pyasn1-0.6.0.20240402/pyasn1-stubs/codec/streaming.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:18.064228 types-pyasn1-0.6.0.20240402/pyasn1-stubs/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:07.000000 types-pyasn1-0.6.0.20240402/pyasn1-stubs/compat/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-02 02:17:07.000000 types-pyasn1-0.6.0.20240402/pyasn1-stubs/compat/integer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-02 02:17:07.000000 types-pyasn1-0.6.0.20240402/pyasn1-stubs/compat/octets.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-02 02:17:07.000000 types-pyasn1-0.6.0.20240402/pyasn1-stubs/debug.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-02 02:17:07.000000 types-pyasn1-0.6.0.20240402/pyasn1-stubs/error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:16.000000 types-pyasn1-0.6.0.20240402/pyasn1-stubs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:18.064228 types-pyasn1-0.6.0.20240402/pyasn1-stubs/type/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:07.000000 types-pyasn1-0.6.0.20240402/pyasn1-stubs/type/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-04-02 02:17:07.000000 types-pyasn1-0.6.0.20240402/pyasn1-stubs/type/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-02 02:17:07.000000 types-pyasn1-0.6.0.20240402/pyasn1-stubs/type/char.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-02 02:17:07.000000 types-pyasn1-0.6.0.20240402/pyasn1-stubs/type/constraint.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-02 02:17:07.000000 types-pyasn1-0.6.0.20240402/pyasn1-stubs/type/error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-02 02:17:07.000000 types-pyasn1-0.6.0.20240402/pyasn1-stubs/type/namedtype.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-02 02:17:07.000000 types-pyasn1-0.6.0.20240402/pyasn1-stubs/type/namedval.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-02 02:17:07.000000 types-pyasn1-0.6.0.20240402/pyasn1-stubs/type/opentype.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-02 02:17:07.000000 types-pyasn1-0.6.0.20240402/pyasn1-stubs/type/tag.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-02 02:17:07.000000 types-pyasn1-0.6.0.20240402/pyasn1-stubs/type/tagmap.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13396 2024-04-02 02:17:07.000000 types-pyasn1-0.6.0.20240402/pyasn1-stubs/type/univ.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-02 02:17:07.000000 types-pyasn1-0.6.0.20240402/pyasn1-stubs/type/useful.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 02:17:18.068228 types-pyasn1-0.6.0.20240402/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-02 02:17:16.000000 types-pyasn1-0.6.0.20240402/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:18.068228 types-pyasn1-0.6.0.20240402/types_pyasn1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-02 02:17:18.000000 types-pyasn1-0.6.0.20240402/types_pyasn1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-02 02:17:18.000000 types-pyasn1-0.6.0.20240402/types_pyasn1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 02:17:18.000000 types-pyasn1-0.6.0.20240402/types_pyasn1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-02 02:17:18.000000 types-pyasn1-0.6.0.20240402/types_pyasn1.egg-info/top_level.txt
```

### Comparing `types-pyasn1-0.5.0.20240301/CHANGELOG.md` & `types-pyasn1-0.6.0.20240402/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 0.6.0.20240402 (2024-04-02)
+
+Bump pyasn1 to 0.6.* (#11681)
+
 ## 0.5.0.20240301 (2024-03-01)
 
 Update `pyright` version to 1.1.350 (#11501)
 
 If you're reading about this commit in an auto-generated changelog: this is an internal change that should have no impact on how these stubs are understood by static-analysis tools such as type checkers or IDEs
 
 ## 0.5.0.20240205 (2024-02-05)
```

### Comparing `types-pyasn1-0.5.0.20240301/PKG-INFO` & `types-pyasn1-0.6.0.20240402/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyasn1
-Version: 0.5.0.20240301
+Version: 0.6.0.20240402
 Summary: Typing stubs for pyasn1
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyasn1.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,16 +22,16 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pyasn1`.
 
 This version of `types-pyasn1` aims to provide accurate annotations
-for `pyasn1==0.5.*`.
+for `pyasn1==0.6.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyasn1. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `e05098681f326b98c635853a40287ac21f771fa2` and was tested
-with mypy 1.8.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `325577cb760c8539435ea6c78c87dc8cd218991c` and was tested
+with mypy 1.9.0, pyright 1.1.356, and
+pytype 2024.3.19.
```

### Comparing `types-pyasn1-0.5.0.20240301/pyasn1-stubs/codec/ber/decoder.pyi` & `types-pyasn1-0.6.0.20240402/pyasn1-stubs/codec/ber/decoder.pyi`

 * *Files identical despite different names*

### Comparing `types-pyasn1-0.5.0.20240301/pyasn1-stubs/codec/ber/encoder.pyi` & `types-pyasn1-0.6.0.20240402/pyasn1-stubs/codec/ber/encoder.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,15 @@
     def encodeValue(self, value, asn1Spec, encodeFun, **options): ...
 
 class ObjectIdentifierEncoder(AbstractItemEncoder):
     supportIndefLenMode: bool
     def encodeValue(self, value, asn1Spec, encodeFun, **options): ...
 
 class RealEncoder(AbstractItemEncoder):
-    # Mistake in the module, should be False, but is 0 at runtime
-    supportIndefLenMode: int  # type: ignore[assignment]
+    supportIndefLenMode: bool
     binEncBase: int
     def encodeValue(self, value, asn1Spec, encodeFun, **options): ...
 
 class SequenceEncoder(AbstractItemEncoder):
     omitEmptyOptionals: bool
     def encodeValue(self, value, asn1Spec, encodeFun, **options): ...
```

### Comparing `types-pyasn1-0.5.0.20240301/pyasn1-stubs/codec/cer/decoder.pyi` & `types-pyasn1-0.6.0.20240402/pyasn1-stubs/codec/cer/decoder.pyi`

 * *Files identical despite different names*

### Comparing `types-pyasn1-0.5.0.20240301/pyasn1-stubs/codec/cer/encoder.pyi` & `types-pyasn1-0.6.0.20240402/pyasn1-stubs/codec/cer/encoder.pyi`

 * *Files identical despite different names*

### Comparing `types-pyasn1-0.5.0.20240301/pyasn1-stubs/codec/der/decoder.pyi` & `types-pyasn1-0.6.0.20240402/pyasn1-stubs/codec/der/decoder.pyi`

 * *Files identical despite different names*

### Comparing `types-pyasn1-0.5.0.20240301/pyasn1-stubs/codec/der/encoder.pyi` & `types-pyasn1-0.6.0.20240402/pyasn1-stubs/codec/der/encoder.pyi`

 * *Files identical despite different names*

### Comparing `types-pyasn1-0.5.0.20240301/pyasn1-stubs/codec/native/decoder.pyi` & `types-pyasn1-0.6.0.20240402/pyasn1-stubs/codec/native/decoder.pyi`

 * *Files identical despite different names*

### Comparing `types-pyasn1-0.5.0.20240301/pyasn1-stubs/codec/native/encoder.pyi` & `types-pyasn1-0.6.0.20240402/pyasn1-stubs/codec/native/encoder.pyi`

 * *Files identical despite different names*

### Comparing `types-pyasn1-0.5.0.20240301/pyasn1-stubs/codec/streaming.pyi` & `types-pyasn1-0.6.0.20240402/pyasn1-stubs/codec/streaming.pyi`

 * *Files identical despite different names*

### Comparing `types-pyasn1-0.5.0.20240301/pyasn1-stubs/debug.pyi` & `types-pyasn1-0.6.0.20240402/pyasn1-stubs/debug.pyi`

 * *Files identical despite different names*

### Comparing `types-pyasn1-0.5.0.20240301/pyasn1-stubs/error.pyi` & `types-pyasn1-0.6.0.20240402/pyasn1-stubs/error.pyi`

 * *Files identical despite different names*

### Comparing `types-pyasn1-0.5.0.20240301/pyasn1-stubs/type/base.pyi` & `types-pyasn1-0.6.0.20240402/pyasn1-stubs/type/base.pyi`

 * *Files identical despite different names*

### Comparing `types-pyasn1-0.5.0.20240301/pyasn1-stubs/type/char.pyi` & `types-pyasn1-0.6.0.20240402/pyasn1-stubs/type/char.pyi`

 * *Files identical despite different names*

### Comparing `types-pyasn1-0.5.0.20240301/pyasn1-stubs/type/constraint.pyi` & `types-pyasn1-0.6.0.20240402/pyasn1-stubs/type/constraint.pyi`

 * *Files identical despite different names*

### Comparing `types-pyasn1-0.5.0.20240301/pyasn1-stubs/type/namedtype.pyi` & `types-pyasn1-0.6.0.20240402/pyasn1-stubs/type/namedtype.pyi`

 * *Files identical despite different names*

### Comparing `types-pyasn1-0.5.0.20240301/pyasn1-stubs/type/namedval.pyi` & `types-pyasn1-0.6.0.20240402/pyasn1-stubs/type/namedval.pyi`

 * *Files identical despite different names*

### Comparing `types-pyasn1-0.5.0.20240301/pyasn1-stubs/type/tag.pyi` & `types-pyasn1-0.6.0.20240402/pyasn1-stubs/type/tag.pyi`

 * *Files identical despite different names*

### Comparing `types-pyasn1-0.5.0.20240301/pyasn1-stubs/type/tagmap.pyi` & `types-pyasn1-0.6.0.20240402/pyasn1-stubs/type/tagmap.pyi`

 * *Files identical despite different names*

### Comparing `types-pyasn1-0.5.0.20240301/pyasn1-stubs/type/univ.pyi` & `types-pyasn1-0.6.0.20240402/pyasn1-stubs/type/univ.pyi`

 * *Files identical despite different names*

### Comparing `types-pyasn1-0.5.0.20240301/pyasn1-stubs/type/useful.pyi` & `types-pyasn1-0.6.0.20240402/pyasn1-stubs/type/useful.pyi`

 * *Files identical despite different names*

### Comparing `types-pyasn1-0.5.0.20240301/setup.py` & `types-pyasn1-0.6.0.20240402/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,40 +11,40 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pyasn1`.
 
 This version of `types-pyasn1` aims to provide accurate annotations
-for `pyasn1==0.5.*`.
+for `pyasn1==0.6.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyasn1. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `e05098681f326b98c635853a40287ac21f771fa2` and was tested
-with mypy 1.8.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `325577cb760c8539435ea6c78c87dc8cd218991c` and was tested
+with mypy 1.9.0, pyright 1.1.356, and
+pytype 2024.3.19.
 '''.lstrip()
 
 setup(name=name,
-      version="0.5.0.20240301",
+      version="0.6.0.20240402",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyasn1.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['pyasn1-stubs'],
-      package_data={'pyasn1-stubs': ['__init__.pyi', 'codec/__init__.pyi', 'codec/ber/__init__.pyi', 'codec/ber/decoder.pyi', 'codec/ber/encoder.pyi', 'codec/ber/eoo.pyi', 'codec/cer/__init__.pyi', 'codec/cer/decoder.pyi', 'codec/cer/encoder.pyi', 'codec/der/__init__.pyi', 'codec/der/decoder.pyi', 'codec/der/encoder.pyi', 'codec/native/__init__.pyi', 'codec/native/decoder.pyi', 'codec/native/encoder.pyi', 'codec/streaming.pyi', 'compat/__init__.pyi', 'compat/integer.pyi', 'compat/octets.pyi', 'debug.pyi', 'error.pyi', 'type/__init__.pyi', 'type/base.pyi', 'type/char.pyi', 'type/constraint.pyi', 'type/error.pyi', 'type/namedtype.pyi', 'type/namedval.pyi', 'type/opentype.pyi', 'type/tag.pyi', 'type/tagmap.pyi', 'type/univ.pyi', 'type/useful.pyi', 'METADATA.toml']},
+      package_data={'pyasn1-stubs': ['__init__.pyi', 'codec/__init__.pyi', 'codec/ber/__init__.pyi', 'codec/ber/decoder.pyi', 'codec/ber/encoder.pyi', 'codec/ber/eoo.pyi', 'codec/cer/__init__.pyi', 'codec/cer/decoder.pyi', 'codec/cer/encoder.pyi', 'codec/der/__init__.pyi', 'codec/der/decoder.pyi', 'codec/der/encoder.pyi', 'codec/native/__init__.pyi', 'codec/native/decoder.pyi', 'codec/native/encoder.pyi', 'codec/streaming.pyi', 'compat/__init__.pyi', 'compat/integer.pyi', 'compat/octets.pyi', 'debug.pyi', 'error.pyi', 'type/__init__.pyi', 'type/base.pyi', 'type/char.pyi', 'type/constraint.pyi', 'type/error.pyi', 'type/namedtype.pyi', 'type/namedval.pyi', 'type/opentype.pyi', 'type/tag.pyi', 'type/tagmap.pyi', 'type/univ.pyi', 'type/useful.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
```

### Comparing `types-pyasn1-0.5.0.20240301/types_pyasn1.egg-info/PKG-INFO` & `types-pyasn1-0.6.0.20240402/types_pyasn1.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyasn1
-Version: 0.5.0.20240301
+Version: 0.6.0.20240402
 Summary: Typing stubs for pyasn1
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyasn1.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,16 +22,16 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pyasn1`.
 
 This version of `types-pyasn1` aims to provide accurate annotations
-for `pyasn1==0.5.*`.
+for `pyasn1==0.6.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyasn1. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `e05098681f326b98c635853a40287ac21f771fa2` and was tested
-with mypy 1.8.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `325577cb760c8539435ea6c78c87dc8cd218991c` and was tested
+with mypy 1.9.0, pyright 1.1.356, and
+pytype 2024.3.19.
```

### Comparing `types-pyasn1-0.5.0.20240301/types_pyasn1.egg-info/SOURCES.txt` & `types-pyasn1-0.6.0.20240402/types_pyasn1.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 CHANGELOG.md
 MANIFEST.in
 setup.py
 pyasn1-stubs/METADATA.toml
 pyasn1-stubs/__init__.pyi
 pyasn1-stubs/debug.pyi
 pyasn1-stubs/error.pyi
+pyasn1-stubs/py.typed
 pyasn1-stubs/codec/__init__.pyi
 pyasn1-stubs/codec/streaming.pyi
 pyasn1-stubs/codec/ber/__init__.pyi
 pyasn1-stubs/codec/ber/decoder.pyi
 pyasn1-stubs/codec/ber/encoder.pyi
 pyasn1-stubs/codec/ber/eoo.pyi
 pyasn1-stubs/codec/cer/__init__.pyi
```

