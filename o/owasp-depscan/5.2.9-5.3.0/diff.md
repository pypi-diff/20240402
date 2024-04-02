# Comparing `tmp/owasp-depscan-5.2.9.tar.gz` & `tmp/owasp-depscan-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owasp-depscan-5.2.9.tar", last modified: Wed Feb 14 19:00:26 2024, max compression
+gzip compressed data, was "owasp-depscan-5.3.0.tar", last modified: Tue Apr  2 10:34:25 2024, max compression
```

## Comparing `owasp-depscan-5.2.9.tar` & `owasp-depscan-5.3.0.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:00:26.186227 owasp-depscan-5.2.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    28084 2024-02-14 19:00:26.186227 owasp-depscan-5.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    26607 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:00:26.170227 owasp-depscan-5.2.9/depscan/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/depscan/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    38835 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/depscan/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:00:26.174227 owasp-depscan-5.2.9/depscan/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/depscan/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    58149 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/depscan/lib/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/depscan/lib/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)    16718 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/depscan/lib/bom.py
--rw-r--r--   0 runner    (1001) docker     (127)    14515 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/depscan/lib/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    81781 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/depscan/lib/csaf.py
--rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/depscan/lib/explainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/depscan/lib/github.py
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/depscan/lib/license.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/depscan/lib/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    11872 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/depscan/lib/normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/depscan/lib/orasclient.py
--rw-r--r--   0 runner    (1001) docker     (127)    20082 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/depscan/lib/pkg_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    14763 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/depscan/lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:00:26.186227 owasp-depscan-5.2.9/owasp_depscan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    28084 2024-02-14 19:00:26.000000 owasp-depscan-5.2.9/owasp_depscan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-02-14 19:00:26.000000 owasp-depscan-5.2.9/owasp_depscan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 19:00:26.000000 owasp-depscan-5.2.9/owasp_depscan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-14 19:00:26.000000 owasp-depscan-5.2.9/owasp_depscan.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-14 19:00:26.000000 owasp-depscan-5.2.9/owasp_depscan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-14 19:00:26.000000 owasp-depscan-5.2.9/owasp_depscan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 19:00:26.186227 owasp-depscan-5.2.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:00:26.174227 owasp-depscan-5.2.9/test/
--rw-r--r--   0 runner    (1001) docker     (127)    32402 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/test/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/test/test_bom.py
--rw-r--r--   0 runner    (1001) docker     (127)    37991 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/test/test_csaf.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/test/test_explainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/test/test_github.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/test/test_license.py
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/test/test_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8072 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/test/test_pkg_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/test/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:00:26.178227 owasp-depscan-5.2.9/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:00:26.170227 owasp-depscan-5.2.9/vendor/choosealicense.com/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:00:26.178227 owasp-depscan-5.2.9/vendor/choosealicense.com/_data/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_data/fields.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_data/meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_data/rules.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:00:26.186227 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/0bsd.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11142 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/afl-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35944 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/agpl-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12624 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9649 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/artistic-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/bsd-2-clause.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/bsd-3-clause-clear.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/bsd-3-clause.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/bsd-4-clause.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/bsl-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    19759 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/cc-by-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    21473 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/cc-by-sa-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8437 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/cc0-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    23872 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/cecill-2.1.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10202 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/cern-ohl-p-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14802 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/cern-ohl-s-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15986 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/cern-ohl-w-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12156 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/ecl-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12461 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/epl-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15112 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/epl-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14163 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/eupl-1.1.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14871 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/eupl-1.2.txt
--rw-r--r--   0 runner    (1001) docker     (127)    23969 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/gfdl-1.3.txt
--rw-r--r--   0 runner    (1001) docker     (127)    19293 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/gpl-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    36394 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/gpl-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/isc.txt
--rw-r--r--   0 runner    (1001) docker     (127)    27491 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/lgpl-2.1.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/lgpl-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    19902 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/lppl-1.3c.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/mit-0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/mit.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18103 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/mpl-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/ms-pl.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/ms-rl.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/mulanpsl-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/ncsa.txt
--rw-r--r--   0 runner    (1001) docker     (127)    26179 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/odbl-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/ofl-1.1.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11580 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/osl-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/postgresql.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/upl-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/vim.txt
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/wtfpl.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/zlib.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:00:26.170227 owasp-depscan-5.2.9/vendor/spdx/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:00:26.186227 owasp-depscan-5.2.9/vendor/spdx/json/
--rw-r--r--   0 runner    (1001) docker     (127)   275192 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/spdx/json/licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:34:25.803510 owasp-depscan-5.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    28084 2024-04-02 10:34:25.803510 owasp-depscan-5.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    26607 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:34:25.787510 owasp-depscan-5.3.0/depscan/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/depscan/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    38835 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/depscan/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:34:25.787510 owasp-depscan-5.3.0/depscan/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/depscan/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58212 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/depscan/lib/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/depscan/lib/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16718 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/depscan/lib/bom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14540 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/depscan/lib/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81781 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/depscan/lib/csaf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/depscan/lib/explainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/depscan/lib/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/depscan/lib/license.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/depscan/lib/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12443 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/depscan/lib/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/depscan/lib/orasclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20394 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/depscan/lib/pkg_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14763 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/depscan/lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:34:25.803510 owasp-depscan-5.3.0/owasp_depscan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28084 2024-04-02 10:34:25.000000 owasp-depscan-5.3.0/owasp_depscan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-02 10:34:25.000000 owasp-depscan-5.3.0/owasp_depscan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 10:34:25.000000 owasp-depscan-5.3.0/owasp_depscan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-02 10:34:25.000000 owasp-depscan-5.3.0/owasp_depscan.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-02 10:34:25.000000 owasp-depscan-5.3.0/owasp_depscan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-02 10:34:25.000000 owasp-depscan-5.3.0/owasp_depscan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 10:34:25.803510 owasp-depscan-5.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:34:25.791510 owasp-depscan-5.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    32402 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/test/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/test/test_bom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37991 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/test/test_csaf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/test/test_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/test/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/test/test_license.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/test/test_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8072 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/test/test_pkg_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:34:25.791510 owasp-depscan-5.3.0/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:34:25.783510 owasp-depscan-5.3.0/vendor/choosealicense.com/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:34:25.791510 owasp-depscan-5.3.0/vendor/choosealicense.com/_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_data/fields.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_data/meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_data/rules.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:34:25.799510 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/0bsd.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11142 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/afl-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35944 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/agpl-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12624 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9649 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/artistic-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/bsd-2-clause.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/bsd-3-clause-clear.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/bsd-3-clause.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/bsd-4-clause.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/bsl-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19759 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/cc-by-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21473 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/cc-by-sa-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8437 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/cc0-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    23872 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/cecill-2.1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10202 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/cern-ohl-p-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14802 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/cern-ohl-s-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15986 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/cern-ohl-w-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12156 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/ecl-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12461 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/epl-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15112 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/epl-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14163 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/eupl-1.1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14871 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/eupl-1.2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    23969 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/gfdl-1.3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19293 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/gpl-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    36394 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/gpl-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/isc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    27491 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/lgpl-2.1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/lgpl-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19902 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/lppl-1.3c.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/mit-0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/mit.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18103 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/mpl-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/ms-pl.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/ms-rl.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/mulanpsl-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/ncsa.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    26179 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/odbl-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/ofl-1.1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11580 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/osl-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/postgresql.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/upl-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/vim.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/wtfpl.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/zlib.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:34:25.787510 owasp-depscan-5.3.0/vendor/spdx/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:34:25.799510 owasp-depscan-5.3.0/vendor/spdx/json/
+-rw-r--r--   0 runner    (1001) docker     (127)   275192 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/spdx/json/licenses.json
```

### Comparing `owasp-depscan-5.2.9/LICENSE` & `owasp-depscan-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/PKG-INFO` & `owasp-depscan-5.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owasp-depscan
-Version: 5.2.9
+Version: 5.3.0
 Summary: Fully open-source security audit for project dependencies based on known vulnerabilities and advisories.
 Author-email: Team AppThreat <cloud@appthreat.com>
 License: MIT
 Project-URL: Homepage, https://github.com/owasp-dep-scan/dep-scan
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -16,17 +16,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: appthreat-vulnerability-db==5.6.2
+Requires-Dist: appthreat-vulnerability-db==5.6.6
 Requires-Dist: defusedxml
-Requires-Dist: oras==0.1.26
+Requires-Dist: oras~=0.1.26
 Requires-Dist: PyYAML
 Requires-Dist: rich
 Requires-Dist: quart
 Requires-Dist: PyGithub
 Requires-Dist: toml
 Requires-Dist: pdfkit
 Requires-Dist: Jinja2
```

### Comparing `owasp-depscan-5.2.9/README.md` & `owasp-depscan-5.3.0/README.md`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/depscan/cli.py` & `owasp-depscan-5.3.0/depscan/cli.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/depscan/lib/analysis.py` & `owasp-depscan-5.3.0/depscan/lib/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1220,14 +1220,15 @@
             package_usage = "[magenta]No"
             package_usage_simple = "No"
         if not risk_metrics:
             continue
         if risk_metrics.get("risk_score") and (
             risk_metrics.get("risk_score") > config.pkg_max_risk_score
             or risk_metrics.get("pkg_private_on_public_registry_risk")
+            or risk_metrics.get("pkg_deprecated_risk")
         ):
             risk_score = f"""{round(risk_metrics.get("risk_score"), 2)}"""
             data = [
                 pkg,
                 package_usage,
                 risk_score,
             ]
@@ -1491,11 +1492,11 @@
                     reached_purls[apurl] += 1
     if bom_file and os.path.exists(bom_file):
         # For now we will also include usability slice as well
         with open(bom_file, "r", encoding="utf-8") as f:
             data = json.load(f)
 
         for c in data["components"]:
-            purl = c["purl"]
+            purl = c.get("purl", "")
             if c.get("evidence") and c["evidence"].get("occurrences"):
                 direct_purls[purl] += len(c["evidence"].get("occurrences"))
     return dict(direct_purls), dict(reached_purls)
```

### Comparing `owasp-depscan-5.2.9/depscan/lib/audit.py` & `owasp-depscan-5.3.0/depscan/lib/audit.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from vdb.lib.npm import NpmSource
 
 from depscan.lib import config
 from depscan.lib.pkg_query import npm_metadata, pypi_metadata
 
 # Dict mapping project type to the audit source
-type_audit_map = {"nodejs": NpmSource(), "js": NpmSource(), "npm": NpmSource()}
+type_audit_map = {"nodejs": NpmSource(), "js": NpmSource(), "javascript": NpmSource(), "ts": NpmSource(),
+                  "typescript": NpmSource(), "npm": NpmSource()}
 
 # Dict mapping project type to risk audit
 risk_audit_map = {
     "npm": npm_metadata,
     "nodejs": npm_metadata,
     "js": npm_metadata,
+    "javascript": npm_metadata,
+    "ts": npm_metadata,
+    "typescript": npm_metadata,
     "python": pypi_metadata,
     "py": pypi_metadata,
     "pypi": pypi_metadata,
 }
 
 
 def audit(project_type, pkg_list):
```

### Comparing `owasp-depscan-5.2.9/depscan/lib/bom.py` & `owasp-depscan-5.3.0/depscan/lib/bom.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/depscan/lib/config.py` & `owasp-depscan-5.3.0/depscan/lib/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,15 @@
     "ro.pippo": "pippo",
     "ca.uhn.hapi.fhir": "fhir",
     "tensorflow": "google",
     "ansible": "redhat",
     "io.springfox": "smartbear",
     "log4net": "apache",
     "github": "github actions",
+    "microsoft": "azure"
 }
 
 # Package aliases
 package_alias = {
     "struts2-core": "struts",
     "struts2-rest-plugin": "struts",
     "struts2-showcase": "struts",
```

### Comparing `owasp-depscan-5.2.9/depscan/lib/csaf.py` & `owasp-depscan-5.3.0/depscan/lib/csaf.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/depscan/lib/explainer.py` & `owasp-depscan-5.3.0/depscan/lib/explainer.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/depscan/lib/github.py` & `owasp-depscan-5.3.0/depscan/lib/github.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/depscan/lib/license.py` & `owasp-depscan-5.3.0/depscan/lib/license.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/depscan/lib/logger.py` & `owasp-depscan-5.3.0/depscan/lib/logger.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/depscan/lib/normalize.py` & `owasp-depscan-5.3.0/depscan/lib/normalize.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,22 +126,31 @@
             vendor_aliases.add(name + "_project")
         for k, v in config.vendor_alias.items():
             if vendor and (vendor.startswith(k) or k.startswith(vendor)):
                 vendor_aliases.add(k)
                 vendor_aliases.add(v)
             elif name == k:
                 vendor_aliases.add(v)
+            elif name.startswith(v):
+                vendor_aliases.add(k)
     # This will add false positives to ubuntu
     if "/" in name and os_distro and "ubuntu" not in os_distro:
         name_aliases.add(name.split("/")[-1])
     # Pypi specific vendor aliases
     if purl.startswith("pkg:pypi"):
         if not name.startswith("python-"):
             name_aliases.add("python-" + name)
             name_aliases.add("python-" + name + "_project")
+            # Eg: numpy:numpy
+            vendor_aliases.add(name)
+            # Issue #262
+            # Eg: cpe:2.3:a:microsoft:azure_storage_blobs:*:*:*:*:*:python:*:*
+            # pypi name is pkg:pypi/azure-storage-blob@12.8.0
+            if not name.endswith("s"):
+                name_aliases.add(name.replace("-", "_") + "s")
         vendor_aliases.add("pip")
         vendor_aliases.add("pypi")
         vendor_aliases.add("python")
         vendor_aliases.add("python-" + name)
         vendor_aliases.add(name + "project")
     elif purl.startswith("pkg:npm"):
         # pg-promise CVE is filed as pg
@@ -193,36 +202,38 @@
         if "lib" in name:
             name_aliases.add(name.replace("lib", ""))
         elif "lib" not in name:
             name_aliases.add("lib" + name)
         if "-bin" not in name:
             name_aliases.add(name + "-bin")
     else:
-        # Filter vendor aliases that are also name aliases
-        vendor_aliases = [
-            x for x in vendor_aliases if x not in name_aliases or x == vendor
-        ]
+        # Filter vendor aliases that are also name aliases for non pypi packages
+        # This is needed for numpy which has the vendor name numpy
+        if not purl.startswith("pkg:pypi"):
+            vendor_aliases = [
+                x for x in vendor_aliases if x not in name_aliases or x == vendor
+            ]
     if len(vendor_aliases) > 1:
         for vvar in list(vendor_aliases):
             for nvar in list(name_aliases):
                 pkg_list.append(
                     {
                         "vendor": vvar,
                         "name": nvar,
-                        "version": pkg_dict["version"],
+                        "version": pkg_dict.get("version", ""),
                     }
                 )
     elif len(name_aliases) > 1:
         for nvar in list(name_aliases):
             # vendor could be none which is fine
             pkg_list.append(
                 {
                     "vendor": pkg_dict.get("vendor"),
                     "name": nvar,
-                    "version": pkg_dict["version"],
+                    "version": pkg_dict.get("version", ""),
                 }
             )
     return pkg_list
 
 
 def dealias_packages(pkg_list, pkg_aliases, purl_aliases):
     """
```

### Comparing `owasp-depscan-5.2.9/depscan/lib/orasclient.py` & `owasp-depscan-5.3.0/depscan/lib/orasclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 class VdbDistributionRegistry(oras.provider.Registry):
     """
     We override the default registry to make things compatible with ghcr. Without this, the below error is thrown.
 
     jsonschema.exceptions.ValidationError: Additional properties are not allowed ('artifactType' was unexpected)
     """
 
-    def get_manifest(self, container, allowed_media_type=None):
+    def get_manifest(self, container, allowed_media_type=None, refresh_headers=True):
         """
         Retrieve a manifest for a package.
 
         :param container:  parsed container URI
         :type container: oras.container.Container or str
         :param allowed_media_type: one or more allowed media types
         :type allowed_media_type: str
```

### Comparing `owasp-depscan-5.2.9/depscan/lib/pkg_query.py` & `owasp-depscan-5.3.0/depscan/lib/pkg_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -315,14 +315,19 @@
         "pkg_min_maintainers_risk": False,
         "pkg_private_on_public_registry_risk": False,
     }
     info = pkg_metadata.get("info", {})
     versions_dict = pkg_metadata.get("releases", {})
     versions = [ver[0] for k, ver in versions_dict.items() if ver]
     is_deprecated = info.get("yanked") and info.get("yanked_reason")
+    # Some packages like pypi:azure only mention deprecated in the description
+    # without yanking the package
+    pkg_description = info.get("description", "").lower()
+    if not is_deprecated and ("is deprecated" in pkg_description or "no longer maintained" in pkg_description):
+        is_deprecated = True
     latest_deprecated = False
     first_version = None
     latest_version = None
 
     # Is the private package available publicly? Dependency confusion.
     if is_private_pkg and pkg_metadata:
         risk_metrics["pkg_private_on_public_registry_risk"] = True
```

### Comparing `owasp-depscan-5.2.9/depscan/lib/utils.py` & `owasp-depscan-5.3.0/depscan/lib/utils.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/owasp_depscan.egg-info/PKG-INFO` & `owasp-depscan-5.3.0/owasp_depscan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owasp-depscan
-Version: 5.2.9
+Version: 5.3.0
 Summary: Fully open-source security audit for project dependencies based on known vulnerabilities and advisories.
 Author-email: Team AppThreat <cloud@appthreat.com>
 License: MIT
 Project-URL: Homepage, https://github.com/owasp-dep-scan/dep-scan
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -16,17 +16,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: appthreat-vulnerability-db==5.6.2
+Requires-Dist: appthreat-vulnerability-db==5.6.6
 Requires-Dist: defusedxml
-Requires-Dist: oras==0.1.26
+Requires-Dist: oras~=0.1.26
 Requires-Dist: PyYAML
 Requires-Dist: rich
 Requires-Dist: quart
 Requires-Dist: PyGithub
 Requires-Dist: toml
 Requires-Dist: pdfkit
 Requires-Dist: Jinja2
```

### Comparing `owasp-depscan-5.2.9/owasp_depscan.egg-info/SOURCES.txt` & `owasp-depscan-5.3.0/owasp_depscan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/pyproject.toml` & `owasp-depscan-5.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name = "owasp-depscan"
-version = "5.2.9"
+version = "5.3.0"
 description = "Fully open-source security audit for project dependencies based on known vulnerabilities and advisories."
 authors = [
     {name = "Team AppThreat", email = "cloud@appthreat.com"},
 ]
 dependencies = [
-    "appthreat-vulnerability-db==5.6.2",
+    "appthreat-vulnerability-db==5.6.6",
     "defusedxml",
-    "oras==0.1.26",
+    "oras~=0.1.26",
     "PyYAML",
     "rich",
     "quart",
     "PyGithub",
     "toml",
     "pdfkit",
     "Jinja2",
```

### Comparing `owasp-depscan-5.2.9/test/test_analysis.py` & `owasp-depscan-5.3.0/test/test_analysis.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/test/test_bom.py` & `owasp-depscan-5.3.0/test/test_bom.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/test/test_csaf.py` & `owasp-depscan-5.3.0/test/test_csaf.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/test/test_github.py` & `owasp-depscan-5.3.0/test/test_github.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/test/test_license.py` & `owasp-depscan-5.3.0/test/test_license.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/test/test_norm.py` & `owasp-depscan-5.3.0/test/test_norm.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/test/test_pkg_query.py` & `owasp-depscan-5.3.0/test/test_pkg_query.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/test/test_utils.py` & `owasp-depscan-5.3.0/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_data/fields.yml` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_data/fields.yml`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_data/meta.yml` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_data/meta.yml`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_data/rules.yml` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_data/rules.yml`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/0bsd.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/0bsd.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/afl-3.0.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/afl-3.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/agpl-3.0.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/agpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/apache-2.0.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/artistic-2.0.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/artistic-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/bsd-2-clause.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/bsd-2-clause.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/bsd-3-clause-clear.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/bsd-3-clause-clear.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/bsd-3-clause.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/bsd-3-clause.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/bsd-4-clause.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/bsd-4-clause.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/bsl-1.0.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/bsl-1.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/cc-by-4.0.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/cc-by-4.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/cc-by-sa-4.0.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/cc-by-sa-4.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/cc0-1.0.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/cc0-1.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/cecill-2.1.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/cecill-2.1.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/cern-ohl-p-2.0.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/cern-ohl-p-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/cern-ohl-s-2.0.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/cern-ohl-s-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/cern-ohl-w-2.0.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/cern-ohl-w-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/ecl-2.0.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/ecl-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/epl-1.0.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/epl-1.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/epl-2.0.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/epl-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/eupl-1.1.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/eupl-1.1.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/eupl-1.2.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/eupl-1.2.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/gfdl-1.3.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/gfdl-1.3.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/gpl-2.0.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/gpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/gpl-3.0.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/gpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/isc.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/isc.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/lgpl-2.1.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/lgpl-2.1.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/lgpl-3.0.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/lgpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/lppl-1.3c.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/lppl-1.3c.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/mit-0.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/mit-0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/mit.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/mit.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/mpl-2.0.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/mpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/ms-pl.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/ms-pl.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/ms-rl.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/ms-rl.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/mulanpsl-2.0.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/mulanpsl-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/ncsa.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/ncsa.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/odbl-1.0.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/odbl-1.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/ofl-1.1.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/ofl-1.1.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/osl-3.0.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/osl-3.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/postgresql.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/postgresql.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/unlicense.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/unlicense.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/upl-1.0.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/upl-1.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/vim.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/vim.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/wtfpl.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/wtfpl.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/zlib.txt` & `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/zlib.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.9/vendor/spdx/json/licenses.json` & `owasp-depscan-5.3.0/vendor/spdx/json/licenses.json`

 * *Files identical despite different names*

