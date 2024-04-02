# Comparing `tmp/enhanced-cnab-0.0.8.tar.gz` & `tmp/enhanced-cnab-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enhanced-cnab-0.0.8.tar", last modified: Sun Mar 17 19:53:47 2024, max compression
+gzip compressed data, was "enhanced-cnab-0.0.9.tar", last modified: Sun Mar 17 20:28:08 2024, max compression
```

## Comparing `enhanced-cnab-0.0.8.tar` & `enhanced-cnab-0.0.9.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 19:53:47.280873 enhanced-cnab-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-17 19:53:47.280873 enhanced-cnab-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 19:53:47.268873 enhanced-cnab-0.0.8/cnab/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 19:53:47.268873 enhanced-cnab-0.0.8/cnab/banks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/banks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 19:53:47.268873 enhanced-cnab-0.0.8/cnab/banks/banco_brasil/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/banks/banco_brasil/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 19:53:47.268873 enhanced-cnab-0.0.8/cnab/banks/banco_brasil/cnab_240/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/banks/banco_brasil/cnab_240/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7310 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/banks/banco_brasil/cnab_240/registro0.py
--rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/banks/banco_brasil/cnab_240/registro1.py
--rw-r--r--   0 runner    (1001) docker     (127)     8699 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/banks/banco_brasil/cnab_240/registro3P.py
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/banks/banco_brasil/cnab_240/registro3Q.py
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/banks/banco_brasil/cnab_240/registro3R.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/banks/banco_brasil/cnab_240/registro3S1e2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/banks/banco_brasil/cnab_240/registro3S3.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/banks/banco_brasil/cnab_240/registro5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/banks/banco_brasil/cnab_240/registro9.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/banks/banco_brasil/cnab_240/remessa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 19:53:47.268873 enhanced-cnab-0.0.8/cnab/banks/bradesco/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/banks/bradesco/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 19:53:47.272873 enhanced-cnab-0.0.8/cnab/banks/bradesco/cnab_400/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/banks/bradesco/cnab_400/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/banks/bradesco/cnab_400/registro0.py
--rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/banks/bradesco/cnab_400/registro1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/banks/bradesco/cnab_400/registro2.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/banks/bradesco/cnab_400/registro9.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/banks/bradesco/cnab_400/remessa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 19:53:47.272873 enhanced-cnab-0.0.8/cnab/banks/itau/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/banks/itau/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 19:53:47.272873 enhanced-cnab-0.0.8/cnab/banks/itau/cnab_400/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/banks/itau/cnab_400/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/banks/itau/cnab_400/registro0.py
--rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/banks/itau/cnab_400/registro1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/banks/itau/cnab_400/registro2.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/banks/itau/cnab_400/registro9.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/banks/itau/cnab_400/remessa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 19:53:47.272873 enhanced-cnab-0.0.8/cnab/banks/santander/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/banks/santander/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 19:53:47.272873 enhanced-cnab-0.0.8/cnab/banks/santander/cnab_240/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/banks/santander/cnab_240/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/banks/santander/cnab_240/registro0.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/banks/santander/cnab_240/registro1.py
--rw-r--r--   0 runner    (1001) docker     (127)     9770 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/banks/santander/cnab_240/registro3P.py
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/banks/santander/cnab_240/registro3Q.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/banks/santander/cnab_240/registro3R.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/banks/santander/cnab_240/registro5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/banks/santander/cnab_240/registro9.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/banks/santander/cnab_240/remessa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 19:53:47.276873 enhanced-cnab-0.0.8/cnab/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 19:53:47.276873 enhanced-cnab-0.0.8/cnab/base/cnab_240/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/base/cnab_240/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/base/cnab_240/registro0.py
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/base/cnab_240/registro1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/base/cnab_240/registro3.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/base/cnab_240/registro5.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/base/cnab_240/registro9.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 19:53:47.276873 enhanced-cnab-0.0.8/cnab/base/cnab_400/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/base/cnab_400/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/base/cnab_400/registro0.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/base/cnab_400/registro1.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/base/cnab_400/registro2.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/base/cnab_400/registro9.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/base/registro.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/base/registro_remessa.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/base/remessa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 19:53:47.276873 enhanced-cnab-0.0.8/cnab/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/core/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 19:53:47.276873 enhanced-cnab-0.0.8/cnab/core/especie/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/core/especie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/core/especie/banks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/core/especie/enum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 19:53:47.276873 enhanced-cnab-0.0.8/cnab/core/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/core/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/core/exceptions/especie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/core/exceptions/field.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/core/exceptions/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/core/field.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 19:53:47.280873 enhanced-cnab-0.0.8/cnab/core/formatter/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/core/formatter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/core/formatter/alfa.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/core/formatter/alfa2.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/core/formatter/date.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/core/formatter/decimal.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/core/formatter/integer.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/core/formatter/time.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 19:53:47.280873 enhanced-cnab-0.0.8/cnab/core/validators/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/core/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/core/validators/date.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/core/validators/decimal.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/core/validators/integer.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/core/validators/required.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/remessa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 19:53:47.280873 enhanced-cnab-0.0.8/cnab/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/utils/check_digit.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/cnab/utils/dict_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 19:53:47.280873 enhanced-cnab-0.0.8/enhanced_cnab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-17 19:53:47.000000 enhanced-cnab-0.0.8/enhanced_cnab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-03-17 19:53:47.000000 enhanced-cnab-0.0.8/enhanced_cnab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-17 19:53:47.000000 enhanced-cnab-0.0.8/enhanced_cnab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-17 19:53:47.000000 enhanced-cnab-0.0.8/enhanced_cnab.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-17 19:53:47.000000 enhanced-cnab-0.0.8/enhanced_cnab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-17 19:53:47.280873 enhanced-cnab-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-03-17 19:53:43.000000 enhanced-cnab-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 20:28:08.090863 enhanced-cnab-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-17 20:28:08.090863 enhanced-cnab-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 20:28:08.074863 enhanced-cnab-0.0.9/cnab/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 20:28:08.074863 enhanced-cnab-0.0.9/cnab/banks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/banks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 20:28:08.074863 enhanced-cnab-0.0.9/cnab/banks/banco_brasil/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/banks/banco_brasil/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 20:28:08.078863 enhanced-cnab-0.0.9/cnab/banks/banco_brasil/cnab_240/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/banks/banco_brasil/cnab_240/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7310 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/banks/banco_brasil/cnab_240/registro0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/banks/banco_brasil/cnab_240/registro1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8699 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/banks/banco_brasil/cnab_240/registro3P.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/banks/banco_brasil/cnab_240/registro3Q.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/banks/banco_brasil/cnab_240/registro3R.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/banks/banco_brasil/cnab_240/registro3S1e2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/banks/banco_brasil/cnab_240/registro3S3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/banks/banco_brasil/cnab_240/registro5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/banks/banco_brasil/cnab_240/registro9.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/banks/banco_brasil/cnab_240/remessa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 20:28:08.078863 enhanced-cnab-0.0.9/cnab/banks/bradesco/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/banks/bradesco/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 20:28:08.078863 enhanced-cnab-0.0.9/cnab/banks/bradesco/cnab_400/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/banks/bradesco/cnab_400/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/banks/bradesco/cnab_400/registro0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/banks/bradesco/cnab_400/registro1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/banks/bradesco/cnab_400/registro2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/banks/bradesco/cnab_400/registro9.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/banks/bradesco/cnab_400/remessa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 20:28:08.078863 enhanced-cnab-0.0.9/cnab/banks/itau/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/banks/itau/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 20:28:08.078863 enhanced-cnab-0.0.9/cnab/banks/itau/cnab_400/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/banks/itau/cnab_400/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/banks/itau/cnab_400/registro0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7364 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/banks/itau/cnab_400/registro1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/banks/itau/cnab_400/registro2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/banks/itau/cnab_400/registro9.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/banks/itau/cnab_400/remessa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 20:28:08.078863 enhanced-cnab-0.0.9/cnab/banks/santander/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/banks/santander/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 20:28:08.082863 enhanced-cnab-0.0.9/cnab/banks/santander/cnab_240/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/banks/santander/cnab_240/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/banks/santander/cnab_240/registro0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/banks/santander/cnab_240/registro1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9770 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/banks/santander/cnab_240/registro3P.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/banks/santander/cnab_240/registro3Q.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/banks/santander/cnab_240/registro3R.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/banks/santander/cnab_240/registro5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/banks/santander/cnab_240/registro9.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/banks/santander/cnab_240/remessa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 20:28:08.082863 enhanced-cnab-0.0.9/cnab/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 20:28:08.082863 enhanced-cnab-0.0.9/cnab/base/cnab_240/
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/base/cnab_240/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/base/cnab_240/registro0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/base/cnab_240/registro1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/base/cnab_240/registro3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/base/cnab_240/registro5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/base/cnab_240/registro9.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 20:28:08.082863 enhanced-cnab-0.0.9/cnab/base/cnab_400/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/base/cnab_400/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/base/cnab_400/registro0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/base/cnab_400/registro1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/base/cnab_400/registro2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/base/cnab_400/registro9.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/base/registro.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/base/registro_remessa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/base/remessa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 20:28:08.086863 enhanced-cnab-0.0.9/cnab/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/core/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 20:28:08.086863 enhanced-cnab-0.0.9/cnab/core/especie/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/core/especie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/core/especie/banks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/core/especie/enum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 20:28:08.086863 enhanced-cnab-0.0.9/cnab/core/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/core/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/core/exceptions/especie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/core/exceptions/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/core/exceptions/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/core/field.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 20:28:08.086863 enhanced-cnab-0.0.9/cnab/core/formatter/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/core/formatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/core/formatter/alfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/core/formatter/alfa2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/core/formatter/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/core/formatter/decimal.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/core/formatter/integer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/core/formatter/time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 20:28:08.086863 enhanced-cnab-0.0.9/cnab/core/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/core/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/core/validators/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/core/validators/decimal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/core/validators/integer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/core/validators/required.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/remessa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 20:28:08.086863 enhanced-cnab-0.0.9/cnab/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/utils/check_digit.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/cnab/utils/dict_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 20:28:08.090863 enhanced-cnab-0.0.9/enhanced_cnab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-17 20:28:08.000000 enhanced-cnab-0.0.9/enhanced_cnab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-03-17 20:28:08.000000 enhanced-cnab-0.0.9/enhanced_cnab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-17 20:28:08.000000 enhanced-cnab-0.0.9/enhanced_cnab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-17 20:28:07.000000 enhanced-cnab-0.0.9/enhanced_cnab.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-17 20:28:08.000000 enhanced-cnab-0.0.9/enhanced_cnab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-17 20:28:08.090863 enhanced-cnab-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-03-17 20:28:02.000000 enhanced-cnab-0.0.9/setup.py
```

### Comparing `enhanced-cnab-0.0.8/PKG-INFO` & `enhanced-cnab-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enhanced-cnab
-Version: 0.0.8
+Version: 0.0.9
 Summary: Enhanced way to generate brazil banks CNAB files in python.
 Home-page: https://github.com/EduardoJM/enhanced-cnab
 Author: Eduardo Oliveira
 Author-email: eduardo_y05@outlook.com
 License: MIT
 Keywords: cnab,banks,boletos,remessa,lote,cnab240,cnab400
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `enhanced-cnab-0.0.8/cnab/banks/banco_brasil/cnab_240/registro0.py` & `enhanced-cnab-0.0.9/cnab/banks/banco_brasil/cnab_240/registro0.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/banks/banco_brasil/cnab_240/registro1.py` & `enhanced-cnab-0.0.9/cnab/banks/banco_brasil/cnab_240/registro1.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/banks/banco_brasil/cnab_240/registro3P.py` & `enhanced-cnab-0.0.9/cnab/banks/banco_brasil/cnab_240/registro3P.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/banks/banco_brasil/cnab_240/registro3Q.py` & `enhanced-cnab-0.0.9/cnab/banks/banco_brasil/cnab_240/registro3Q.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/banks/banco_brasil/cnab_240/registro3R.py` & `enhanced-cnab-0.0.9/cnab/banks/banco_brasil/cnab_240/registro3R.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/banks/banco_brasil/cnab_240/registro3S1e2.py` & `enhanced-cnab-0.0.9/cnab/banks/banco_brasil/cnab_240/registro3S1e2.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/banks/banco_brasil/cnab_240/registro3S3.py` & `enhanced-cnab-0.0.9/cnab/banks/banco_brasil/cnab_240/registro3S3.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/banks/banco_brasil/cnab_240/registro5.py` & `enhanced-cnab-0.0.9/cnab/banks/banco_brasil/cnab_240/registro5.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/banks/banco_brasil/cnab_240/registro9.py` & `enhanced-cnab-0.0.9/cnab/banks/banco_brasil/cnab_240/registro9.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/banks/banco_brasil/cnab_240/remessa.py` & `enhanced-cnab-0.0.9/cnab/banks/banco_brasil/cnab_240/remessa.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/banks/bradesco/cnab_400/registro0.py` & `enhanced-cnab-0.0.9/cnab/banks/bradesco/cnab_400/registro0.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/banks/bradesco/cnab_400/registro1.py` & `enhanced-cnab-0.0.9/cnab/banks/bradesco/cnab_400/registro1.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/banks/bradesco/cnab_400/registro2.py` & `enhanced-cnab-0.0.9/cnab/banks/bradesco/cnab_400/registro2.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/banks/bradesco/cnab_400/registro9.py` & `enhanced-cnab-0.0.9/cnab/banks/bradesco/cnab_400/registro9.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/banks/bradesco/cnab_400/remessa.py` & `enhanced-cnab-0.0.9/cnab/banks/bradesco/cnab_400/remessa.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/banks/itau/cnab_400/registro0.py` & `enhanced-cnab-0.0.9/cnab/banks/itau/cnab_400/registro0.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/banks/itau/cnab_400/registro1.py` & `enhanced-cnab-0.0.9/cnab/banks/itau/cnab_400/registro1.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,7 +185,10 @@
         super().__init__(header, parent, **kwargs)
         self.inserir_multa(**kwargs)
 
     def inserir_multa(self, **kwargs: dict):
         if not kwargs.get('data_multa'):
             return
         ItauCnab400Registro2(self.header, self, **kwargs)
+
+    def get_agencia_cobradora(self):
+        return self.get_data_or_parent('agencia')
```

### Comparing `enhanced-cnab-0.0.8/cnab/banks/itau/cnab_400/registro2.py` & `enhanced-cnab-0.0.9/cnab/banks/itau/cnab_400/registro2.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/banks/itau/cnab_400/registro9.py` & `enhanced-cnab-0.0.9/cnab/banks/itau/cnab_400/registro9.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/banks/itau/cnab_400/remessa.py` & `enhanced-cnab-0.0.9/cnab/banks/itau/cnab_400/remessa.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/banks/santander/cnab_240/registro0.py` & `enhanced-cnab-0.0.9/cnab/banks/santander/cnab_240/registro0.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/banks/santander/cnab_240/registro1.py` & `enhanced-cnab-0.0.9/cnab/banks/santander/cnab_240/registro1.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/banks/santander/cnab_240/registro3P.py` & `enhanced-cnab-0.0.9/cnab/banks/santander/cnab_240/registro3P.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/banks/santander/cnab_240/registro3Q.py` & `enhanced-cnab-0.0.9/cnab/banks/santander/cnab_240/registro3Q.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/banks/santander/cnab_240/registro3R.py` & `enhanced-cnab-0.0.9/cnab/banks/santander/cnab_240/registro3R.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/banks/santander/cnab_240/registro5.py` & `enhanced-cnab-0.0.9/cnab/banks/santander/cnab_240/registro5.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/banks/santander/cnab_240/registro9.py` & `enhanced-cnab-0.0.9/cnab/banks/santander/cnab_240/registro9.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/base/cnab_240/registro0.py` & `enhanced-cnab-0.0.9/cnab/base/cnab_240/registro0.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/base/cnab_240/registro1.py` & `enhanced-cnab-0.0.9/cnab/base/cnab_240/registro1.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/base/cnab_240/registro3.py` & `enhanced-cnab-0.0.9/cnab/base/cnab_240/registro3.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/base/cnab_240/registro5.py` & `enhanced-cnab-0.0.9/cnab/base/cnab_240/registro5.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/base/cnab_400/registro0.py` & `enhanced-cnab-0.0.9/cnab/base/cnab_400/registro0.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/base/cnab_400/registro1.py` & `enhanced-cnab-0.0.9/cnab/base/cnab_400/registro1.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Optional
 from datetime import datetime
 from cnab.base.registro_remessa import RegistroRemessa
 from cnab.base.registro import Registro
 from cnab.core.enums import TipoServico, TipoInscricao
 from cnab.core.exceptions import CNABInvalidTypeError
+from cnab.core.especie import EspecieTitulo
 
 class CNAB400Registro1(RegistroRemessa):
     def __init__(self, header: Optional["Registro"], parent: Optional["Registro"], **kwargs: dict):
         self.counter = 0
         super().__init__(header, parent, **kwargs)
         self.init_numero_registro()
 
@@ -36,7 +37,15 @@
         return self.get_data_or_parent('conta_dv')
     
     def get_data_emissao(self):
         return datetime.now()
     
     def get_numero_registro(self):
         return self.get_data_or_parent('numero_sequencial')
+
+    def get_especie_titulo(self):
+        field = self.get_field('codigo_banco')
+        return EspecieTitulo.get_real_value(
+            field.default,
+            self._data.get('especie_titulo')
+        )
+
```

### Comparing `enhanced-cnab-0.0.8/cnab/base/registro.py` & `enhanced-cnab-0.0.9/cnab/base/registro.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/base/remessa.py` & `enhanced-cnab-0.0.9/cnab/base/remessa.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/core/especie/banks.py` & `enhanced-cnab-0.0.9/cnab/core/especie/banks.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/core/especie/enum.py` & `enhanced-cnab-0.0.9/cnab/core/especie/enum.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/core/exceptions/__init__.py` & `enhanced-cnab-0.0.9/cnab/core/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/core/exceptions/field.py` & `enhanced-cnab-0.0.9/cnab/core/exceptions/field.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/core/field.py` & `enhanced-cnab-0.0.9/cnab/core/field.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/core/formatter/alfa.py` & `enhanced-cnab-0.0.9/cnab/core/formatter/alfa.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/cnab/utils/check_digit.py` & `enhanced-cnab-0.0.9/cnab/utils/check_digit.py`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/enhanced_cnab.egg-info/PKG-INFO` & `enhanced-cnab-0.0.9/enhanced_cnab.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enhanced-cnab
-Version: 0.0.8
+Version: 0.0.9
 Summary: Enhanced way to generate brazil banks CNAB files in python.
 Home-page: https://github.com/EduardoJM/enhanced-cnab
 Author: Eduardo Oliveira
 Author-email: eduardo_y05@outlook.com
 License: MIT
 Keywords: cnab,banks,boletos,remessa,lote,cnab240,cnab400
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `enhanced-cnab-0.0.8/enhanced_cnab.egg-info/SOURCES.txt` & `enhanced-cnab-0.0.9/enhanced_cnab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enhanced-cnab-0.0.8/setup.py` & `enhanced-cnab-0.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 f = open(os.path.join(os.path.dirname(__file__), 'README.md'))
 readme = f.read()
 f.close()
 
 setup(
     name='enhanced-cnab',
-    version='0.0.8',
+    version='0.0.9',
     description='Enhanced way to generate brazil banks CNAB files in python.',
     long_description=readme,
     long_description_content_type='text/markdown',
     author='Eduardo Oliveira',
     author_email='eduardo_y05@outlook.com',
     url='https://github.com/EduardoJM/enhanced-cnab',
     license='MIT',
```

