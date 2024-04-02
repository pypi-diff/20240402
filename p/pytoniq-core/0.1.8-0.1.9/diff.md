# Comparing `tmp/pytoniq-core-0.1.8.tar.gz` & `tmp/pytoniq-core-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytoniq-core-0.1.8.tar", last modified: Tue Sep 12 14:54:49 2023, max compression
+gzip compressed data, was "pytoniq-core-0.1.9.tar", last modified: Fri Oct 13 15:03:34 2023, max compression
```

## Comparing `pytoniq-core-0.1.8.tar` & `pytoniq-core-0.1.9.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-09-12 14:54:49.405463 pytoniq-core-0.1.8/
--rw-r--r--   0 yungwine   (501) staff       (20)       34 2023-08-03 15:43:19.000000 pytoniq-core-0.1.8/MANIFEST.in
--rw-r--r--   0 yungwine   (501) staff       (20)     1639 2023-09-12 14:54:49.405291 pytoniq-core-0.1.8/PKG-INFO
--rw-r--r--   0 yungwine   (501) staff       (20)     1228 2023-08-27 11:45:59.000000 pytoniq-core-0.1.8/README.md
-drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-09-12 14:54:49.394757 pytoniq-core-0.1.8/pytoniq_core/
--rw-r--r--   0 yungwine   (501) staff       (20)       98 2023-08-03 13:42:45.000000 pytoniq-core-0.1.8/pytoniq_core/__init__.py
-drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-09-12 14:54:49.396956 pytoniq-core-0.1.8/pytoniq_core/boc/
--rw-r--r--   0 yungwine   (501) staff       (20)      222 2023-07-23 15:42:41.000000 pytoniq-core-0.1.8/pytoniq_core/boc/__init__.py
--rw-r--r--   0 yungwine   (501) staff       (20)     3672 2023-08-03 13:37:49.000000 pytoniq-core-0.1.8/pytoniq_core/boc/address.py
--rw-r--r--   0 yungwine   (501) staff       (20)     5340 2023-09-05 07:50:12.000000 pytoniq-core-0.1.8/pytoniq_core/boc/builder.py
--rw-r--r--   0 yungwine   (501) staff       (20)    11009 2023-08-03 12:39:07.000000 pytoniq-core-0.1.8/pytoniq_core/boc/cell.py
--rw-r--r--   0 yungwine   (501) staff       (20)     9079 2023-07-28 16:29:36.000000 pytoniq-core-0.1.8/pytoniq_core/boc/deserialize.py
-drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-09-12 14:54:49.397488 pytoniq-core-0.1.8/pytoniq_core/boc/dict/
--rw-r--r--   0 yungwine   (501) staff       (20)       41 2023-07-23 15:42:41.000000 pytoniq-core-0.1.8/pytoniq_core/boc/dict/__init__.py
--rw-r--r--   0 yungwine   (501) staff       (20)     5307 2023-08-03 14:29:33.000000 pytoniq-core-0.1.8/pytoniq_core/boc/dict/dict.py
--rw-r--r--   0 yungwine   (501) staff       (20)     3919 2023-07-23 17:27:59.000000 pytoniq-core-0.1.8/pytoniq_core/boc/dict/parse.py
--rw-r--r--   0 yungwine   (501) staff       (20)     4989 2023-06-19 11:55:15.000000 pytoniq-core-0.1.8/pytoniq_core/boc/dict/utils.py
--rw-r--r--   0 yungwine   (501) staff       (20)     1026 2023-07-23 13:47:12.000000 pytoniq-core-0.1.8/pytoniq_core/boc/exotic.py
--rw-r--r--   0 yungwine   (501) staff       (20)     8212 2023-08-14 11:42:11.000000 pytoniq-core-0.1.8/pytoniq_core/boc/slice.py
--rw-r--r--   0 yungwine   (501) staff       (20)     1866 2023-07-05 13:08:40.000000 pytoniq-core-0.1.8/pytoniq_core/boc/tvm_bitarray.py
--rw-r--r--   0 yungwine   (501) staff       (20)      298 2023-07-13 12:16:46.000000 pytoniq-core-0.1.8/pytoniq_core/boc/utils.py
-drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-09-12 14:54:49.398292 pytoniq-core-0.1.8/pytoniq_core/crypto/
--rw-r--r--   0 yungwine   (501) staff       (20)        0 2023-06-17 12:05:39.000000 pytoniq-core-0.1.8/pytoniq_core/crypto/__init__.py
--rw-r--r--   0 yungwine   (501) staff       (20)     4177 2023-08-06 10:04:24.000000 pytoniq-core-0.1.8/pytoniq_core/crypto/ciphers.py
--rw-r--r--   0 yungwine   (501) staff       (20)     6558 2023-06-17 13:10:44.000000 pytoniq-core-0.1.8/pytoniq_core/crypto/crc.py
--rw-r--r--   0 yungwine   (501) staff       (20)    22014 2023-07-22 13:35:04.000000 pytoniq-core-0.1.8/pytoniq_core/crypto/keys.py
--rw-r--r--   0 yungwine   (501) staff       (20)      819 2023-08-14 07:09:49.000000 pytoniq-core-0.1.8/pytoniq_core/crypto/signature.py
-drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-09-12 14:54:49.398733 pytoniq-core-0.1.8/pytoniq_core/proof/
--rw-r--r--   0 yungwine   (501) staff       (20)      186 2023-07-23 15:42:41.000000 pytoniq-core-0.1.8/pytoniq_core/proof/__init__.py
--rw-r--r--   0 yungwine   (501) staff       (20)     6193 2023-07-21 11:26:13.000000 pytoniq-core-0.1.8/pytoniq_core/proof/check_proof.py
-drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-09-12 14:54:49.399173 pytoniq-core-0.1.8/pytoniq_core/tl/
--rw-r--r--   0 yungwine   (501) staff       (20)      118 2023-07-23 15:42:41.000000 pytoniq-core-0.1.8/pytoniq_core/tl/__init__.py
--rw-r--r--   0 yungwine   (501) staff       (20)     2990 2023-07-23 08:44:15.000000 pytoniq-core-0.1.8/pytoniq_core/tl/block.py
--rw-r--r--   0 yungwine   (501) staff       (20)    14750 2023-08-14 08:08:40.000000 pytoniq-core-0.1.8/pytoniq_core/tl/generator.py
-drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-09-12 14:54:49.400105 pytoniq-core-0.1.8/pytoniq_core/tl/schemas/
--rw-r--r--   0 yungwine   (501) staff       (20)     7204 2023-07-30 12:46:41.000000 pytoniq-core-0.1.8/pytoniq_core/tl/schemas/lite_api.tl
--rw-r--r--   0 yungwine   (501) staff       (20)    45439 2023-09-12 14:54:14.000000 pytoniq-core-0.1.8/pytoniq_core/tl/schemas/ton_api.tl
--rw-r--r--   0 yungwine   (501) staff       (20)    18697 2023-05-29 07:39:43.000000 pytoniq-core-0.1.8/pytoniq_core/tl/schemas/tonlib_api.tl
-drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-09-12 14:54:49.404677 pytoniq-core-0.1.8/pytoniq_core/tlb/
--rw-r--r--   0 yungwine   (501) staff       (20)      924 2023-07-24 08:29:16.000000 pytoniq-core-0.1.8/pytoniq_core/tlb/__init__.py
--rw-r--r--   0 yungwine   (501) staff       (20)    12202 2023-08-14 13:25:23.000000 pytoniq-core-0.1.8/pytoniq_core/tlb/account.py
--rw-r--r--   0 yungwine   (501) staff       (20)    35555 2023-08-26 12:27:46.000000 pytoniq-core-0.1.8/pytoniq_core/tlb/block.py
--rw-r--r--   0 yungwine   (501) staff       (20)     5137 2023-06-30 16:07:22.000000 pytoniq-core-0.1.8/pytoniq_core/tlb/code_generator.py
--rw-r--r--   0 yungwine   (501) staff       (20)    56951 2023-07-13 14:13:51.000000 pytoniq-core-0.1.8/pytoniq_core/tlb/config.py
-drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-09-12 14:54:49.405054 pytoniq-core-0.1.8/pytoniq_core/tlb/custom/
--rw-r--r--   0 yungwine   (501) staff       (20)       91 2023-07-27 17:13:15.000000 pytoniq-core-0.1.8/pytoniq_core/tlb/custom/__init__.py
--rw-r--r--   0 yungwine   (501) staff       (20)     5309 2023-08-03 12:37:28.000000 pytoniq-core-0.1.8/pytoniq_core/tlb/custom/nft.py
--rw-r--r--   0 yungwine   (501) staff       (20)     4584 2023-07-23 14:27:13.000000 pytoniq-core-0.1.8/pytoniq_core/tlb/custom/wallet.py
--rw-r--r--   0 yungwine   (501) staff       (20)    12530 2023-07-27 17:28:35.000000 pytoniq-core-0.1.8/pytoniq_core/tlb/generator.py
--rw-r--r--   0 yungwine   (501) staff       (20)     1053 2023-08-03 15:23:58.000000 pytoniq-core-0.1.8/pytoniq_core/tlb/tlb.py
--rw-r--r--   0 yungwine   (501) staff       (20)    46194 2023-08-24 06:29:52.000000 pytoniq-core-0.1.8/pytoniq_core/tlb/transaction.py
--rw-r--r--   0 yungwine   (501) staff       (20)     2551 2023-08-23 07:00:37.000000 pytoniq-core-0.1.8/pytoniq_core/tlb/utils.py
--rw-r--r--   0 yungwine   (501) staff       (20)    15591 2023-08-01 07:42:26.000000 pytoniq-core-0.1.8/pytoniq_core/tlb/vm_stack.py
-drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-09-12 14:54:49.395495 pytoniq-core-0.1.8/pytoniq_core.egg-info/
--rw-r--r--   0 yungwine   (501) staff       (20)     1639 2023-09-12 14:54:49.000000 pytoniq-core-0.1.8/pytoniq_core.egg-info/PKG-INFO
--rw-r--r--   0 yungwine   (501) staff       (20)     1408 2023-09-12 14:54:49.000000 pytoniq-core-0.1.8/pytoniq_core.egg-info/SOURCES.txt
--rw-r--r--   0 yungwine   (501) staff       (20)        1 2023-09-12 14:54:49.000000 pytoniq-core-0.1.8/pytoniq_core.egg-info/dependency_links.txt
--rw-r--r--   0 yungwine   (501) staff       (20)      102 2023-09-12 14:54:49.000000 pytoniq-core-0.1.8/pytoniq_core.egg-info/requires.txt
--rw-r--r--   0 yungwine   (501) staff       (20)       13 2023-09-12 14:54:49.000000 pytoniq-core-0.1.8/pytoniq_core.egg-info/top_level.txt
--rw-r--r--   0 yungwine   (501) staff       (20)       38 2023-09-12 14:54:49.405501 pytoniq-core-0.1.8/setup.cfg
--rw-r--r--   0 yungwine   (501) staff       (20)      985 2023-09-12 14:54:25.000000 pytoniq-core-0.1.8/setup.py
+drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-10-13 15:03:34.414704 pytoniq-core-0.1.9/
+-rw-r--r--   0 yungwine   (501) staff       (20)       34 2023-08-03 15:43:19.000000 pytoniq-core-0.1.9/MANIFEST.in
+-rw-r--r--   0 yungwine   (501) staff       (20)     1639 2023-10-13 15:03:34.414590 pytoniq-core-0.1.9/PKG-INFO
+-rw-r--r--   0 yungwine   (501) staff       (20)     1228 2023-08-27 11:45:59.000000 pytoniq-core-0.1.9/README.md
+drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-10-13 15:03:34.406589 pytoniq-core-0.1.9/pytoniq_core/
+-rw-r--r--   0 yungwine   (501) staff       (20)       98 2023-08-03 13:42:45.000000 pytoniq-core-0.1.9/pytoniq_core/__init__.py
+drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-10-13 15:03:34.408900 pytoniq-core-0.1.9/pytoniq_core/boc/
+-rw-r--r--   0 yungwine   (501) staff       (20)      222 2023-07-23 15:42:41.000000 pytoniq-core-0.1.9/pytoniq_core/boc/__init__.py
+-rw-r--r--   0 yungwine   (501) staff       (20)     3672 2023-08-03 13:37:49.000000 pytoniq-core-0.1.9/pytoniq_core/boc/address.py
+-rw-r--r--   0 yungwine   (501) staff       (20)     5340 2023-09-05 07:50:12.000000 pytoniq-core-0.1.9/pytoniq_core/boc/builder.py
+-rw-r--r--   0 yungwine   (501) staff       (20)    11009 2023-08-03 12:39:07.000000 pytoniq-core-0.1.9/pytoniq_core/boc/cell.py
+-rw-r--r--   0 yungwine   (501) staff       (20)     9079 2023-07-28 16:29:36.000000 pytoniq-core-0.1.9/pytoniq_core/boc/deserialize.py
+drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-10-13 15:03:34.409495 pytoniq-core-0.1.9/pytoniq_core/boc/dict/
+-rw-r--r--   0 yungwine   (501) staff       (20)       41 2023-07-23 15:42:41.000000 pytoniq-core-0.1.9/pytoniq_core/boc/dict/__init__.py
+-rw-r--r--   0 yungwine   (501) staff       (20)     5307 2023-08-03 14:29:33.000000 pytoniq-core-0.1.9/pytoniq_core/boc/dict/dict.py
+-rw-r--r--   0 yungwine   (501) staff       (20)     3919 2023-07-23 17:27:59.000000 pytoniq-core-0.1.9/pytoniq_core/boc/dict/parse.py
+-rw-r--r--   0 yungwine   (501) staff       (20)     4989 2023-06-19 11:55:15.000000 pytoniq-core-0.1.9/pytoniq_core/boc/dict/utils.py
+-rw-r--r--   0 yungwine   (501) staff       (20)     1026 2023-07-23 13:47:12.000000 pytoniq-core-0.1.9/pytoniq_core/boc/exotic.py
+-rw-r--r--   0 yungwine   (501) staff       (20)     8212 2023-08-14 11:42:11.000000 pytoniq-core-0.1.9/pytoniq_core/boc/slice.py
+-rw-r--r--   0 yungwine   (501) staff       (20)     1866 2023-07-05 13:08:40.000000 pytoniq-core-0.1.9/pytoniq_core/boc/tvm_bitarray.py
+-rw-r--r--   0 yungwine   (501) staff       (20)      298 2023-07-13 12:16:46.000000 pytoniq-core-0.1.9/pytoniq_core/boc/utils.py
+drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-10-13 15:03:34.410134 pytoniq-core-0.1.9/pytoniq_core/crypto/
+-rw-r--r--   0 yungwine   (501) staff       (20)        0 2023-06-17 12:05:39.000000 pytoniq-core-0.1.9/pytoniq_core/crypto/__init__.py
+-rw-r--r--   0 yungwine   (501) staff       (20)     4177 2023-08-06 10:04:24.000000 pytoniq-core-0.1.9/pytoniq_core/crypto/ciphers.py
+-rw-r--r--   0 yungwine   (501) staff       (20)     6558 2023-06-17 13:10:44.000000 pytoniq-core-0.1.9/pytoniq_core/crypto/crc.py
+-rw-r--r--   0 yungwine   (501) staff       (20)    22014 2023-07-22 13:35:04.000000 pytoniq-core-0.1.9/pytoniq_core/crypto/keys.py
+-rw-r--r--   0 yungwine   (501) staff       (20)      819 2023-08-14 07:09:49.000000 pytoniq-core-0.1.9/pytoniq_core/crypto/signature.py
+drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-10-13 15:03:34.410444 pytoniq-core-0.1.9/pytoniq_core/proof/
+-rw-r--r--   0 yungwine   (501) staff       (20)      186 2023-07-23 15:42:41.000000 pytoniq-core-0.1.9/pytoniq_core/proof/__init__.py
+-rw-r--r--   0 yungwine   (501) staff       (20)     6193 2023-07-21 11:26:13.000000 pytoniq-core-0.1.9/pytoniq_core/proof/check_proof.py
+drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-10-13 15:03:34.410814 pytoniq-core-0.1.9/pytoniq_core/tl/
+-rw-r--r--   0 yungwine   (501) staff       (20)      118 2023-07-23 15:42:41.000000 pytoniq-core-0.1.9/pytoniq_core/tl/__init__.py
+-rw-r--r--   0 yungwine   (501) staff       (20)     2990 2023-07-23 08:44:15.000000 pytoniq-core-0.1.9/pytoniq_core/tl/block.py
+-rw-r--r--   0 yungwine   (501) staff       (20)    14750 2023-08-14 08:08:40.000000 pytoniq-core-0.1.9/pytoniq_core/tl/generator.py
+drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-10-13 15:03:34.411584 pytoniq-core-0.1.9/pytoniq_core/tl/schemas/
+-rw-r--r--   0 yungwine   (501) staff       (20)     7204 2023-07-30 12:46:41.000000 pytoniq-core-0.1.9/pytoniq_core/tl/schemas/lite_api.tl
+-rw-r--r--   0 yungwine   (501) staff       (20)    45439 2023-09-27 14:01:56.000000 pytoniq-core-0.1.9/pytoniq_core/tl/schemas/ton_api.tl
+-rw-r--r--   0 yungwine   (501) staff       (20)    18697 2023-05-29 07:39:43.000000 pytoniq-core-0.1.9/pytoniq_core/tl/schemas/tonlib_api.tl
+drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-10-13 15:03:34.413991 pytoniq-core-0.1.9/pytoniq_core/tlb/
+-rw-r--r--   0 yungwine   (501) staff       (20)      924 2023-07-24 08:29:16.000000 pytoniq-core-0.1.9/pytoniq_core/tlb/__init__.py
+-rw-r--r--   0 yungwine   (501) staff       (20)    12202 2023-08-14 13:25:23.000000 pytoniq-core-0.1.9/pytoniq_core/tlb/account.py
+-rw-r--r--   0 yungwine   (501) staff       (20)    35555 2023-08-26 12:27:46.000000 pytoniq-core-0.1.9/pytoniq_core/tlb/block.py
+-rw-r--r--   0 yungwine   (501) staff       (20)     5137 2023-06-30 16:07:22.000000 pytoniq-core-0.1.9/pytoniq_core/tlb/code_generator.py
+-rw-r--r--   0 yungwine   (501) staff       (20)    56951 2023-07-13 14:13:51.000000 pytoniq-core-0.1.9/pytoniq_core/tlb/config.py
+drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-10-13 15:03:34.414377 pytoniq-core-0.1.9/pytoniq_core/tlb/custom/
+-rw-r--r--   0 yungwine   (501) staff       (20)       91 2023-07-27 17:13:15.000000 pytoniq-core-0.1.9/pytoniq_core/tlb/custom/__init__.py
+-rw-r--r--   0 yungwine   (501) staff       (20)     5309 2023-08-03 12:37:28.000000 pytoniq-core-0.1.9/pytoniq_core/tlb/custom/nft.py
+-rw-r--r--   0 yungwine   (501) staff       (20)     4584 2023-07-23 14:27:13.000000 pytoniq-core-0.1.9/pytoniq_core/tlb/custom/wallet.py
+-rw-r--r--   0 yungwine   (501) staff       (20)    12530 2023-07-27 17:28:35.000000 pytoniq-core-0.1.9/pytoniq_core/tlb/generator.py
+-rw-r--r--   0 yungwine   (501) staff       (20)     1053 2023-08-03 15:23:58.000000 pytoniq-core-0.1.9/pytoniq_core/tlb/tlb.py
+-rw-r--r--   0 yungwine   (501) staff       (20)    46597 2023-10-13 15:02:03.000000 pytoniq-core-0.1.9/pytoniq_core/tlb/transaction.py
+-rw-r--r--   0 yungwine   (501) staff       (20)     2551 2023-08-23 07:00:37.000000 pytoniq-core-0.1.9/pytoniq_core/tlb/utils.py
+-rw-r--r--   0 yungwine   (501) staff       (20)    15591 2023-08-01 07:42:26.000000 pytoniq-core-0.1.9/pytoniq_core/tlb/vm_stack.py
+drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-10-13 15:03:34.407203 pytoniq-core-0.1.9/pytoniq_core.egg-info/
+-rw-r--r--   0 yungwine   (501) staff       (20)     1639 2023-10-13 15:03:34.000000 pytoniq-core-0.1.9/pytoniq_core.egg-info/PKG-INFO
+-rw-r--r--   0 yungwine   (501) staff       (20)     1408 2023-10-13 15:03:34.000000 pytoniq-core-0.1.9/pytoniq_core.egg-info/SOURCES.txt
+-rw-r--r--   0 yungwine   (501) staff       (20)        1 2023-10-13 15:03:34.000000 pytoniq-core-0.1.9/pytoniq_core.egg-info/dependency_links.txt
+-rw-r--r--   0 yungwine   (501) staff       (20)      102 2023-10-13 15:03:34.000000 pytoniq-core-0.1.9/pytoniq_core.egg-info/requires.txt
+-rw-r--r--   0 yungwine   (501) staff       (20)       13 2023-10-13 15:03:34.000000 pytoniq-core-0.1.9/pytoniq_core.egg-info/top_level.txt
+-rw-r--r--   0 yungwine   (501) staff       (20)       38 2023-10-13 15:03:34.414743 pytoniq-core-0.1.9/setup.cfg
+-rw-r--r--   0 yungwine   (501) staff       (20)      985 2023-10-13 15:03:16.000000 pytoniq-core-0.1.9/setup.py
```

### Comparing `pytoniq-core-0.1.8/PKG-INFO` & `pytoniq-core-0.1.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytoniq-core
-Version: 0.1.8
+Version: 0.1.9
 Summary: TON Blockchain SDK
 Home-page: https://github.com/yungwine/pytoniq
 Author: Maksim Kurbatov
 Author-email: cyrbatoff@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `pytoniq-core-0.1.8/README.md` & `pytoniq-core-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pytoniq-core-0.1.8/pytoniq_core/boc/address.py` & `pytoniq-core-0.1.9/pytoniq_core/boc/address.py`

 * *Files identical despite different names*

### Comparing `pytoniq-core-0.1.8/pytoniq_core/boc/builder.py` & `pytoniq-core-0.1.9/pytoniq_core/boc/builder.py`

 * *Files identical despite different names*

### Comparing `pytoniq-core-0.1.8/pytoniq_core/boc/cell.py` & `pytoniq-core-0.1.9/pytoniq_core/boc/cell.py`

 * *Files identical despite different names*

### Comparing `pytoniq-core-0.1.8/pytoniq_core/boc/deserialize.py` & `pytoniq-core-0.1.9/pytoniq_core/boc/deserialize.py`

 * *Files identical despite different names*

### Comparing `pytoniq-core-0.1.8/pytoniq_core/boc/dict/dict.py` & `pytoniq-core-0.1.9/pytoniq_core/boc/dict/dict.py`

 * *Files identical despite different names*

### Comparing `pytoniq-core-0.1.8/pytoniq_core/boc/dict/parse.py` & `pytoniq-core-0.1.9/pytoniq_core/boc/dict/parse.py`

 * *Files identical despite different names*

### Comparing `pytoniq-core-0.1.8/pytoniq_core/boc/dict/utils.py` & `pytoniq-core-0.1.9/pytoniq_core/boc/dict/utils.py`

 * *Files identical despite different names*

### Comparing `pytoniq-core-0.1.8/pytoniq_core/boc/exotic.py` & `pytoniq-core-0.1.9/pytoniq_core/boc/exotic.py`

 * *Files identical despite different names*

### Comparing `pytoniq-core-0.1.8/pytoniq_core/boc/slice.py` & `pytoniq-core-0.1.9/pytoniq_core/boc/slice.py`

 * *Files identical despite different names*

### Comparing `pytoniq-core-0.1.8/pytoniq_core/boc/tvm_bitarray.py` & `pytoniq-core-0.1.9/pytoniq_core/boc/tvm_bitarray.py`

 * *Files identical despite different names*

### Comparing `pytoniq-core-0.1.8/pytoniq_core/crypto/ciphers.py` & `pytoniq-core-0.1.9/pytoniq_core/crypto/ciphers.py`

 * *Files identical despite different names*

### Comparing `pytoniq-core-0.1.8/pytoniq_core/crypto/crc.py` & `pytoniq-core-0.1.9/pytoniq_core/crypto/crc.py`

 * *Files identical despite different names*

### Comparing `pytoniq-core-0.1.8/pytoniq_core/crypto/keys.py` & `pytoniq-core-0.1.9/pytoniq_core/crypto/keys.py`

 * *Files identical despite different names*

### Comparing `pytoniq-core-0.1.8/pytoniq_core/crypto/signature.py` & `pytoniq-core-0.1.9/pytoniq_core/crypto/signature.py`

 * *Files identical despite different names*

### Comparing `pytoniq-core-0.1.8/pytoniq_core/proof/check_proof.py` & `pytoniq-core-0.1.9/pytoniq_core/proof/check_proof.py`

 * *Files identical despite different names*

### Comparing `pytoniq-core-0.1.8/pytoniq_core/tl/block.py` & `pytoniq-core-0.1.9/pytoniq_core/tl/block.py`

 * *Files identical despite different names*

### Comparing `pytoniq-core-0.1.8/pytoniq_core/tl/generator.py` & `pytoniq-core-0.1.9/pytoniq_core/tl/generator.py`

 * *Files identical despite different names*

### Comparing `pytoniq-core-0.1.8/pytoniq_core/tl/schemas/lite_api.tl` & `pytoniq-core-0.1.9/pytoniq_core/tl/schemas/lite_api.tl`

 * *Files identical despite different names*

### Comparing `pytoniq-core-0.1.8/pytoniq_core/tl/schemas/ton_api.tl` & `pytoniq-core-0.1.9/pytoniq_core/tl/schemas/ton_api.tl`

 * *Files identical despite different names*

### Comparing `pytoniq-core-0.1.8/pytoniq_core/tl/schemas/tonlib_api.tl` & `pytoniq-core-0.1.9/pytoniq_core/tl/schemas/tonlib_api.tl`

 * *Files identical despite different names*

### Comparing `pytoniq-core-0.1.8/pytoniq_core/tlb/__init__.py` & `pytoniq-core-0.1.9/pytoniq_core/tlb/__init__.py`

 * *Files identical despite different names*

### Comparing `pytoniq-core-0.1.8/pytoniq_core/tlb/account.py` & `pytoniq-core-0.1.9/pytoniq_core/tlb/account.py`

 * *Files identical despite different names*

### Comparing `pytoniq-core-0.1.8/pytoniq_core/tlb/block.py` & `pytoniq-core-0.1.9/pytoniq_core/tlb/block.py`

 * *Files identical despite different names*

### Comparing `pytoniq-core-0.1.8/pytoniq_core/tlb/code_generator.py` & `pytoniq-core-0.1.9/pytoniq_core/tlb/code_generator.py`

 * *Files identical despite different names*

### Comparing `pytoniq-core-0.1.8/pytoniq_core/tlb/config.py` & `pytoniq-core-0.1.9/pytoniq_core/tlb/config.py`

 * *Files identical despite different names*

### Comparing `pytoniq-core-0.1.8/pytoniq_core/tlb/custom/nft.py` & `pytoniq-core-0.1.9/pytoniq_core/tlb/custom/nft.py`

 * *Files identical despite different names*

### Comparing `pytoniq-core-0.1.8/pytoniq_core/tlb/custom/wallet.py` & `pytoniq-core-0.1.9/pytoniq_core/tlb/custom/wallet.py`

 * *Files identical despite different names*

### Comparing `pytoniq-core-0.1.8/pytoniq_core/tlb/generator.py` & `pytoniq-core-0.1.9/pytoniq_core/tlb/generator.py`

 * *Files identical despite different names*

### Comparing `pytoniq-core-0.1.8/pytoniq_core/tlb/tlb.py` & `pytoniq-core-0.1.9/pytoniq_core/tlb/tlb.py`

 * *Files identical despite different names*

### Comparing `pytoniq-core-0.1.8/pytoniq_core/tlb/transaction.py` & `pytoniq-core-0.1.9/pytoniq_core/tlb/transaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,19 +155,28 @@
     def is_external_out(self):
         return isinstance(self.info, ExternalOutMsgInfo)
 
     def serialize(self) -> Cell:
         builder = Builder().store_cell(self.info.serialize())
         if self.init:
             builder.store_bit(1)  # maybe true
-            builder.store_bit(1)  # Either right
-            builder.store_ref(self.init.serialize())
+            if len(self.init.serialize().bits) <= builder.available_bits:
+                builder.store_bit(0)  # Either left
+                builder.store_cell(self.init.serialize())
+            else:
+                builder.store_bit(1)  # Either right
+                builder.store_ref(self.init.serialize())
         else:
             builder.store_bit(0)  # maybe false
-        builder.store_maybe_ref(self.body)  # Either right
+        if len(self.body.bits) <= builder.available_bits:
+            builder.store_bit(0)  # Either left
+            builder.store_cell(self.body)
+        else:
+            builder.store_bit(1)  # Either right
+            builder.store_ref(self.body)
         return builder.end_cell()
 
     @classmethod
     def deserialize(cls, cell_slice: Slice):
         info = CommonMsgInfo.deserialize(cell_slice)
         init = None
         maybe = cell_slice.load_bit()
```

### Comparing `pytoniq-core-0.1.8/pytoniq_core/tlb/utils.py` & `pytoniq-core-0.1.9/pytoniq_core/tlb/utils.py`

 * *Files identical despite different names*

### Comparing `pytoniq-core-0.1.8/pytoniq_core/tlb/vm_stack.py` & `pytoniq-core-0.1.9/pytoniq_core/tlb/vm_stack.py`

 * *Files identical despite different names*

### Comparing `pytoniq-core-0.1.8/pytoniq_core.egg-info/PKG-INFO` & `pytoniq-core-0.1.9/pytoniq_core.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytoniq-core
-Version: 0.1.8
+Version: 0.1.9
 Summary: TON Blockchain SDK
 Home-page: https://github.com/yungwine/pytoniq
 Author: Maksim Kurbatov
 Author-email: cyrbatoff@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `pytoniq-core-0.1.8/pytoniq_core.egg-info/SOURCES.txt` & `pytoniq-core-0.1.9/pytoniq_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytoniq-core-0.1.8/setup.py` & `pytoniq-core-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pytoniq-core",
-    version="0.1.8",
+    version="0.1.9",
     author="Maksim Kurbatov",
     author_email="cyrbatoff@gmail.com",
     description="TON Blockchain SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages('.', exclude=['.idea', 'tests', 'examples', 'pytoniq_core/tlb/generator.py']),
     include_package_data=True,
```

