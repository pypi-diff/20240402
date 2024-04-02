# Comparing `tmp/obsarray-0.2.6.tar.gz` & `tmp/obsarray-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obsarray-0.2.6.tar", last modified: Wed Mar 27 16:18:51 2024, max compression
+gzip compressed data, was "obsarray-0.2.7.tar", last modified: Tue Apr  2 11:02:18 2024, max compression
```

## Comparing `obsarray-0.2.6.tar` & `obsarray-0.2.7.tar`

### file list

```diff
@@ -1,82 +1,80 @@
-drwxr-xr-x   0 seh2     (2077935315) 226434968        0 2024-03-27 16:18:51.764476 obsarray-0.2.6/
--rw-r--r--   0 seh2     (2077935315) 226434968     1385 2024-02-26 10:03:37.000000 obsarray-0.2.6/.gitignore
--rw-r--r--   0 seh2     (2077935315) 226434968       91 2021-10-13 10:25:22.000000 obsarray-0.2.6/.pre-commit-config.yaml
--rw-r--r--   0 seh2     (2077935315) 226434968     7631 2022-05-21 12:09:05.000000 obsarray-0.2.6/LICENSE
--rw-r--r--   0 seh2     (2077935315) 226434968       51 2021-10-13 10:25:22.000000 obsarray-0.2.6/MANIFEST.in
--rw-r--r--   0 seh2     (2077935315) 226434968     2362 2024-03-27 16:18:51.764801 obsarray-0.2.6/PKG-INFO
--rw-r--r--   0 seh2     (2077935315) 226434968     1777 2022-11-30 16:57:18.000000 obsarray-0.2.6/README.md
-drwxr-xr-x   0 seh2     (2077935315) 226434968        0 2024-03-27 16:18:51.691400 obsarray-0.2.6/docs/
--rw-r--r--   0 seh2     (2077935315) 226434968      609 2021-10-13 10:25:22.000000 obsarray-0.2.6/docs/Makefile
--rw-r--r--   0 seh2     (2077935315) 226434968     5456 2024-02-26 10:03:37.000000 obsarray-0.2.6/docs/conf.py
--rw-r--r--   0 seh2     (2077935315) 226434968     2309 2024-02-26 10:03:37.000000 obsarray-0.2.6/docs/index.rst
--rw-r--r--   0 seh2     (2077935315) 226434968      770 2021-10-13 10:25:22.000000 obsarray-0.2.6/docs/make.bat
-drwxr-xr-x   0 seh2     (2077935315) 226434968        0 2024-03-27 16:18:51.767762 obsarray-0.2.6/obsarray/
--rw-r--r--   0 seh2     (2077935315) 226434968      496 2024-03-27 16:17:00.000000 obsarray-0.2.6/obsarray/__init__.py
--rw-r--r--   0 seh2     (2077935315) 226434968      498 2024-03-27 16:18:51.767922 obsarray-0.2.6/obsarray/_version.py
--rw-r--r--   0 seh2     (2077935315) 226434968     9224 2024-03-27 16:17:00.000000 obsarray-0.2.6/obsarray/err_corr.py
--rw-r--r--   0 seh2     (2077935315) 226434968    12922 2024-03-27 16:17:00.000000 obsarray-0.2.6/obsarray/flag_accessor.py
-drwxr-xr-x   0 seh2     (2077935315) 226434968        0 2024-03-27 16:18:51.709036 obsarray-0.2.6/obsarray/templater/
--rw-r--r--   0 seh2     (2077935315) 226434968        0 2021-11-09 11:12:45.000000 obsarray-0.2.6/obsarray/templater/__init__.py
--rw-r--r--   0 seh2     (2077935315) 226434968    21214 2024-03-27 16:17:00.000000 obsarray-0.2.6/obsarray/templater/dataset_util.py
--rw-r--r--   0 seh2     (2077935315) 226434968     9440 2021-11-09 14:43:12.000000 obsarray-0.2.6/obsarray/templater/dsdoc.py
--rw-r--r--   0 seh2     (2077935315) 226434968     4081 2021-11-09 14:43:12.000000 obsarray-0.2.6/obsarray/templater/dstemplater.py
--rw-r--r--   0 seh2     (2077935315) 226434968     3154 2024-03-27 16:17:00.000000 obsarray-0.2.6/obsarray/templater/dswriter.py
--rw-r--r--   0 seh2     (2077935315) 226434968     8717 2024-03-27 16:17:00.000000 obsarray-0.2.6/obsarray/templater/template_util.py
--rw-------   0 seh2     (2077935315) 226434968     6331 2022-12-09 13:27:58.000000 obsarray-0.2.6/obsarray/templater/template_util_jon.py
-drwxr-xr-x   0 seh2     (2077935315) 226434968        0 2024-03-27 16:18:51.713744 obsarray-0.2.6/obsarray/templater/tests/
--rw-r--r--   0 seh2     (2077935315) 226434968        0 2020-05-18 15:26:13.000000 obsarray-0.2.6/obsarray/templater/tests/__init__.py
--rw-r--r--   0 seh2     (2077935315) 226434968    17484 2023-03-20 16:34:30.000000 obsarray-0.2.6/obsarray/templater/tests/test_dataset_util.py
--rw-r--r--   0 seh2     (2077935315) 226434968    10209 2021-11-09 14:38:28.000000 obsarray-0.2.6/obsarray/templater/tests/test_dsdoc.py
--rw-r--r--   0 seh2     (2077935315) 226434968      605 2021-11-09 11:36:20.000000 obsarray-0.2.6/obsarray/templater/tests/test_dswriter.py
--rw-r--r--   0 seh2     (2077935315) 226434968    11415 2022-08-24 14:44:08.000000 obsarray-0.2.6/obsarray/templater/tests/test_template_util.py
-drwxr-xr-x   0 seh2     (2077935315) 226434968        0 2024-03-27 16:18:51.718209 obsarray-0.2.6/obsarray/test/
--rw-r--r--   0 seh2     (2077935315) 226434968        0 2021-10-20 08:21:46.000000 obsarray-0.2.6/obsarray/test/__init__.py
--rw-r--r--   0 seh2     (2077935315) 226434968     6606 2024-03-27 16:17:00.000000 obsarray-0.2.6/obsarray/test/test_err_corr_forms.py
--rw-r--r--   0 seh2     (2077935315) 226434968    12217 2024-03-27 16:17:00.000000 obsarray-0.2.6/obsarray/test/test_flag_accessor.py
--rw-r--r--   0 seh2     (2077935315) 226434968    25003 2024-03-27 16:17:00.000000 obsarray-0.2.6/obsarray/test/test_unc_accessor.py
--rw-r--r--   0 seh2     (2077935315) 226434968    28755 2024-03-27 16:17:00.000000 obsarray-0.2.6/obsarray/unc_accessor.py
--rw-r--r--   0 seh2     (2077935315) 226434968      722 2022-08-05 16:19:54.000000 obsarray-0.2.6/obsarray/utils.py
-drwxr-xr-x   0 seh2     (2077935315) 226434968        0 2024-03-27 16:18:51.703023 obsarray-0.2.6/obsarray.egg-info/
--rw-r--r--   0 seh2     (2077935315) 226434968     2362 2024-03-27 16:18:51.000000 obsarray-0.2.6/obsarray.egg-info/PKG-INFO
--rw-r--r--   0 seh2     (2077935315) 226434968     2364 2024-03-27 16:18:51.000000 obsarray-0.2.6/obsarray.egg-info/SOURCES.txt
--rw-r--r--   0 seh2     (2077935315) 226434968        1 2024-03-27 16:18:51.000000 obsarray-0.2.6/obsarray.egg-info/dependency_links.txt
--rw-r--r--   0 seh2     (2077935315) 226434968      123 2024-03-27 16:18:51.000000 obsarray-0.2.6/obsarray.egg-info/requires.txt
--rw-r--r--   0 seh2     (2077935315) 226434968        9 2024-03-27 16:18:51.000000 obsarray-0.2.6/obsarray.egg-info/top_level.txt
-drwxr-xr-x   0 seh2     (2077935315) 226434968        0 2024-03-27 16:18:51.741106 obsarray-0.2.6/quality_documentation/
--rw-r--r--   0 seh2     (2077935315) 226434968     3205 2021-10-13 10:25:22.000000 obsarray-0.2.6/quality_documentation/.gitignore
--rw-r--r--   0 seh2     (2077935315) 226434968     3869 2021-10-13 10:25:22.000000 obsarray-0.2.6/quality_documentation/QualityDocumentation.tex
-drwxr-xr-x   0 seh2     (2077935315) 226434968        0 2024-03-27 16:18:51.750576 obsarray-0.2.6/quality_documentation/base/
--rw-r--r--   0 seh2     (2077935315) 226434968      294 2021-10-13 10:25:23.000000 obsarray-0.2.6/quality_documentation/base/CookiecutterMacros.tex
--rw-r--r--   0 seh2     (2077935315) 226434968      164 2021-10-13 10:25:23.000000 obsarray-0.2.6/quality_documentation/base/acronyms.tex
--rw-r--r--   0 seh2     (2077935315) 226434968      366 2021-10-13 10:25:23.000000 obsarray-0.2.6/quality_documentation/base/history.tex
--rw-r--r--   0 seh2     (2077935315) 226434968      584 2021-10-13 10:25:23.000000 obsarray-0.2.6/quality_documentation/base/metadata.tex
--rw-r--r--   0 seh2     (2077935315) 226434968      470 2021-10-13 10:25:23.000000 obsarray-0.2.6/quality_documentation/base/pythoninputstyle.tex
--rw-r--r--   0 seh2     (2077935315) 226434968      920 2021-10-13 10:25:23.000000 obsarray-0.2.6/quality_documentation/base/sil2.tex
--rw-r--r--   0 seh2     (2077935315) 226434968      909 2021-10-13 10:25:23.000000 obsarray-0.2.6/quality_documentation/base/sil3.tex
--rw-r--r--   0 seh2     (2077935315) 226434968      481 2021-10-13 10:25:23.000000 obsarray-0.2.6/quality_documentation/base/sources.bib
--rw-r--r--   0 seh2     (2077935315) 226434968       90 2021-10-13 10:25:23.000000 obsarray-0.2.6/quality_documentation/base/sources.tex
--rw-r--r--   0 seh2     (2077935315) 226434968      307 2021-10-13 10:25:22.000000 obsarray-0.2.6/quality_documentation/countpdfpages.sh
--rw-r--r--   0 seh2     (2077935315) 226434968     8888 2021-10-13 10:25:22.000000 obsarray-0.2.6/quality_documentation/footnotehyper-sphinx.sty
--rw-r--r--   0 seh2     (2077935315) 226434968    98870 2021-10-13 10:25:22.000000 obsarray-0.2.6/quality_documentation/obsarray_QF-59.docm
--rw-r--r--   0 seh2     (2077935315) 226434968   123009 2021-10-13 10:25:22.000000 obsarray-0.2.6/quality_documentation/obsarray_requirements.docx
-drwxr-xr-x   0 seh2     (2077935315) 226434968        0 2024-03-27 16:18:51.762023 obsarray-0.2.6/quality_documentation/review_checklists/
--rw-r--r--   0 seh2     (2077935315) 226434968    20652 2021-10-13 10:25:23.000000 obsarray-0.2.6/quality_documentation/review_checklists/qf-16a.docx
--rw-r--r--   0 seh2     (2077935315) 226434968    38673 2021-10-13 10:25:22.000000 obsarray-0.2.6/quality_documentation/review_checklists/qf-16b.docx
--rw-r--r--   0 seh2     (2077935315) 226434968    22441 2021-10-13 10:25:22.000000 obsarray-0.2.6/quality_documentation/review_checklists/qf-16c.docx
--rw-r--r--   0 seh2     (2077935315) 226434968    44592 2021-10-13 10:25:22.000000 obsarray-0.2.6/quality_documentation/review_checklists/qf-16d.docx
--rw-r--r--   0 seh2     (2077935315) 226434968    21030 2021-10-13 10:25:23.000000 obsarray-0.2.6/quality_documentation/review_checklists/qf-16e.docx
--rw-r--r--   0 seh2     (2077935315) 226434968    21190 2021-10-13 10:25:23.000000 obsarray-0.2.6/quality_documentation/review_checklists/qf-16f.docx
--rw-r--r--   0 seh2     (2077935315) 226434968     6760 2021-10-13 10:25:22.000000 obsarray-0.2.6/quality_documentation/softwareRequirements.sty
--rw-r--r--   0 seh2     (2077935315) 226434968    82250 2021-10-13 10:25:22.000000 obsarray-0.2.6/quality_documentation/sphinx.sty
--rw-r--r--   0 seh2     (2077935315) 226434968     2583 2021-10-13 10:25:22.000000 obsarray-0.2.6/quality_documentation/sphinxcyrillic.sty
--rw-r--r--   0 seh2     (2077935315) 226434968     8137 2021-10-13 10:25:22.000000 obsarray-0.2.6/quality_documentation/sphinxhighlight.sty
--rw-r--r--   0 seh2     (2077935315) 226434968     3251 2021-10-13 10:25:22.000000 obsarray-0.2.6/quality_documentation/sphinxhowto.cls
--rw-r--r--   0 seh2     (2077935315) 226434968     4236 2021-10-13 10:25:22.000000 obsarray-0.2.6/quality_documentation/sphinxmanual.cls
--rw-r--r--   0 seh2     (2077935315) 226434968      745 2021-10-13 10:25:22.000000 obsarray-0.2.6/quality_documentation/sphinxmessages.sty
--rw-r--r--   0 seh2     (2077935315) 226434968    14606 2021-10-13 10:25:22.000000 obsarray-0.2.6/quality_documentation/sphinxmulticell.sty
-drwxr-xr-x   0 seh2     (2077935315) 226434968        0 2024-03-27 16:18:51.763738 obsarray-0.2.6/quality_documentation/uml/
--rw-r--r--   0 seh2     (2077935315) 226434968      102 2021-10-13 10:25:22.000000 obsarray-0.2.6/quality_documentation/uml/copy your design png file into this folder.txt
--rw-r--r--   0 seh2     (2077935315) 226434968      439 2024-03-27 16:18:51.766402 obsarray-0.2.6/setup.cfg
--rw-r--r--   0 seh2     (2077935315) 226434968     1400 2024-03-27 16:17:00.000000 obsarray-0.2.6/setup.py
--rw-r--r--   0 seh2     (2077935315) 226434968      245 2021-10-13 10:25:22.000000 obsarray-0.2.6/tox.ini
--rw-r--r--   0 seh2     (2077935315) 226434968    68750 2024-02-26 10:03:37.000000 obsarray-0.2.6/versioneer.py
+drwxr-xr-x   0 seh2     (2077935315) 226434968        0 2024-04-02 11:02:18.560184 obsarray-0.2.7/
+-rw-r--r--   0 seh2     (2077935315) 226434968     1385 2024-02-26 10:03:37.000000 obsarray-0.2.7/.gitignore
+-rw-r--r--   0 seh2     (2077935315) 226434968       91 2021-10-13 10:25:22.000000 obsarray-0.2.7/.pre-commit-config.yaml
+-rw-r--r--   0 seh2     (2077935315) 226434968     7631 2022-05-21 12:09:05.000000 obsarray-0.2.7/LICENSE
+-rw-r--r--   0 seh2     (2077935315) 226434968       51 2021-10-13 10:25:22.000000 obsarray-0.2.7/MANIFEST.in
+-rw-r--r--   0 seh2     (2077935315) 226434968     2362 2024-04-02 11:02:18.560333 obsarray-0.2.7/PKG-INFO
+-rw-r--r--   0 seh2     (2077935315) 226434968     1777 2022-11-30 16:57:18.000000 obsarray-0.2.7/README.md
+drwxr-xr-x   0 seh2     (2077935315) 226434968        0 2024-04-02 11:02:18.522480 obsarray-0.2.7/docs/
+-rw-r--r--   0 seh2     (2077935315) 226434968      609 2021-10-13 10:25:22.000000 obsarray-0.2.7/docs/Makefile
+-rw-r--r--   0 seh2     (2077935315) 226434968     5456 2024-02-26 10:03:37.000000 obsarray-0.2.7/docs/conf.py
+-rw-r--r--   0 seh2     (2077935315) 226434968     2309 2024-02-26 10:03:37.000000 obsarray-0.2.7/docs/index.rst
+-rw-r--r--   0 seh2     (2077935315) 226434968      770 2021-10-13 10:25:22.000000 obsarray-0.2.7/docs/make.bat
+drwxr-xr-x   0 seh2     (2077935315) 226434968        0 2024-04-02 11:02:18.561704 obsarray-0.2.7/obsarray/
+-rw-r--r--   0 seh2     (2077935315) 226434968      496 2024-03-27 16:17:00.000000 obsarray-0.2.7/obsarray/__init__.py
+-rw-r--r--   0 seh2     (2077935315) 226434968      498 2024-04-02 11:02:18.561812 obsarray-0.2.7/obsarray/_version.py
+-rw-r--r--   0 seh2     (2077935315) 226434968    10096 2024-04-02 11:01:59.000000 obsarray-0.2.7/obsarray/err_corr.py
+-rw-r--r--   0 seh2     (2077935315) 226434968    12922 2024-03-27 16:17:00.000000 obsarray-0.2.7/obsarray/flag_accessor.py
+drwxr-xr-x   0 seh2     (2077935315) 226434968        0 2024-04-02 11:02:18.530196 obsarray-0.2.7/obsarray/templater/
+-rw-r--r--   0 seh2     (2077935315) 226434968        0 2021-11-09 11:12:45.000000 obsarray-0.2.7/obsarray/templater/__init__.py
+-rw-r--r--   0 seh2     (2077935315) 226434968    21214 2024-03-27 16:17:00.000000 obsarray-0.2.7/obsarray/templater/dataset_util.py
+-rw-r--r--   0 seh2     (2077935315) 226434968     4081 2021-11-09 14:43:12.000000 obsarray-0.2.7/obsarray/templater/dstemplater.py
+-rw-r--r--   0 seh2     (2077935315) 226434968     3154 2024-03-27 16:17:00.000000 obsarray-0.2.7/obsarray/templater/dswriter.py
+-rw-r--r--   0 seh2     (2077935315) 226434968     8717 2024-03-27 16:17:00.000000 obsarray-0.2.7/obsarray/templater/template_util.py
+-rw-------   0 seh2     (2077935315) 226434968     6331 2022-12-09 13:27:58.000000 obsarray-0.2.7/obsarray/templater/template_util_jon.py
+drwxr-xr-x   0 seh2     (2077935315) 226434968        0 2024-04-02 11:02:18.532304 obsarray-0.2.7/obsarray/templater/tests/
+-rw-r--r--   0 seh2     (2077935315) 226434968        0 2020-05-18 15:26:13.000000 obsarray-0.2.7/obsarray/templater/tests/__init__.py
+-rw-r--r--   0 seh2     (2077935315) 226434968    17484 2023-03-20 16:34:30.000000 obsarray-0.2.7/obsarray/templater/tests/test_dataset_util.py
+-rw-r--r--   0 seh2     (2077935315) 226434968      605 2021-11-09 11:36:20.000000 obsarray-0.2.7/obsarray/templater/tests/test_dswriter.py
+-rw-r--r--   0 seh2     (2077935315) 226434968    11415 2022-08-24 14:44:08.000000 obsarray-0.2.7/obsarray/templater/tests/test_template_util.py
+drwxr-xr-x   0 seh2     (2077935315) 226434968        0 2024-04-02 11:02:18.534397 obsarray-0.2.7/obsarray/test/
+-rw-r--r--   0 seh2     (2077935315) 226434968        0 2021-10-20 08:21:46.000000 obsarray-0.2.7/obsarray/test/__init__.py
+-rw-r--r--   0 seh2     (2077935315) 226434968     7985 2024-04-02 11:01:59.000000 obsarray-0.2.7/obsarray/test/test_err_corr_forms.py
+-rw-r--r--   0 seh2     (2077935315) 226434968    12217 2024-03-27 16:17:00.000000 obsarray-0.2.7/obsarray/test/test_flag_accessor.py
+-rw-r--r--   0 seh2     (2077935315) 226434968    25015 2024-04-02 11:01:59.000000 obsarray-0.2.7/obsarray/test/test_unc_accessor.py
+-rw-r--r--   0 seh2     (2077935315) 226434968    28759 2024-04-02 11:01:59.000000 obsarray-0.2.7/obsarray/unc_accessor.py
+-rw-r--r--   0 seh2     (2077935315) 226434968      722 2022-08-05 16:19:54.000000 obsarray-0.2.7/obsarray/utils.py
+drwxr-xr-x   0 seh2     (2077935315) 226434968        0 2024-04-02 11:02:18.527028 obsarray-0.2.7/obsarray.egg-info/
+-rw-r--r--   0 seh2     (2077935315) 226434968     2362 2024-04-02 11:02:18.000000 obsarray-0.2.7/obsarray.egg-info/PKG-INFO
+-rw-r--r--   0 seh2     (2077935315) 226434968     2297 2024-04-02 11:02:18.000000 obsarray-0.2.7/obsarray.egg-info/SOURCES.txt
+-rw-r--r--   0 seh2     (2077935315) 226434968        1 2024-04-02 11:02:18.000000 obsarray-0.2.7/obsarray.egg-info/dependency_links.txt
+-rw-r--r--   0 seh2     (2077935315) 226434968      123 2024-04-02 11:02:18.000000 obsarray-0.2.7/obsarray.egg-info/requires.txt
+-rw-r--r--   0 seh2     (2077935315) 226434968        9 2024-04-02 11:02:18.000000 obsarray-0.2.7/obsarray.egg-info/top_level.txt
+drwxr-xr-x   0 seh2     (2077935315) 226434968        0 2024-04-02 11:02:18.545771 obsarray-0.2.7/quality_documentation/
+-rw-r--r--   0 seh2     (2077935315) 226434968     3205 2021-10-13 10:25:22.000000 obsarray-0.2.7/quality_documentation/.gitignore
+-rw-r--r--   0 seh2     (2077935315) 226434968     3869 2021-10-13 10:25:22.000000 obsarray-0.2.7/quality_documentation/QualityDocumentation.tex
+drwxr-xr-x   0 seh2     (2077935315) 226434968        0 2024-04-02 11:02:18.552768 obsarray-0.2.7/quality_documentation/base/
+-rw-r--r--   0 seh2     (2077935315) 226434968      294 2021-10-13 10:25:23.000000 obsarray-0.2.7/quality_documentation/base/CookiecutterMacros.tex
+-rw-r--r--   0 seh2     (2077935315) 226434968      164 2021-10-13 10:25:23.000000 obsarray-0.2.7/quality_documentation/base/acronyms.tex
+-rw-r--r--   0 seh2     (2077935315) 226434968      366 2021-10-13 10:25:23.000000 obsarray-0.2.7/quality_documentation/base/history.tex
+-rw-r--r--   0 seh2     (2077935315) 226434968      584 2021-10-13 10:25:23.000000 obsarray-0.2.7/quality_documentation/base/metadata.tex
+-rw-r--r--   0 seh2     (2077935315) 226434968      470 2021-10-13 10:25:23.000000 obsarray-0.2.7/quality_documentation/base/pythoninputstyle.tex
+-rw-r--r--   0 seh2     (2077935315) 226434968      920 2021-10-13 10:25:23.000000 obsarray-0.2.7/quality_documentation/base/sil2.tex
+-rw-r--r--   0 seh2     (2077935315) 226434968      909 2021-10-13 10:25:23.000000 obsarray-0.2.7/quality_documentation/base/sil3.tex
+-rw-r--r--   0 seh2     (2077935315) 226434968      481 2021-10-13 10:25:23.000000 obsarray-0.2.7/quality_documentation/base/sources.bib
+-rw-r--r--   0 seh2     (2077935315) 226434968       90 2021-10-13 10:25:23.000000 obsarray-0.2.7/quality_documentation/base/sources.tex
+-rw-r--r--   0 seh2     (2077935315) 226434968      307 2021-10-13 10:25:22.000000 obsarray-0.2.7/quality_documentation/countpdfpages.sh
+-rw-r--r--   0 seh2     (2077935315) 226434968     8888 2021-10-13 10:25:22.000000 obsarray-0.2.7/quality_documentation/footnotehyper-sphinx.sty
+-rw-r--r--   0 seh2     (2077935315) 226434968    98870 2021-10-13 10:25:22.000000 obsarray-0.2.7/quality_documentation/obsarray_QF-59.docm
+-rw-r--r--   0 seh2     (2077935315) 226434968   123009 2021-10-13 10:25:22.000000 obsarray-0.2.7/quality_documentation/obsarray_requirements.docx
+drwxr-xr-x   0 seh2     (2077935315) 226434968        0 2024-04-02 11:02:18.558576 obsarray-0.2.7/quality_documentation/review_checklists/
+-rw-r--r--   0 seh2     (2077935315) 226434968    20652 2021-10-13 10:25:23.000000 obsarray-0.2.7/quality_documentation/review_checklists/qf-16a.docx
+-rw-r--r--   0 seh2     (2077935315) 226434968    38673 2021-10-13 10:25:22.000000 obsarray-0.2.7/quality_documentation/review_checklists/qf-16b.docx
+-rw-r--r--   0 seh2     (2077935315) 226434968    22441 2021-10-13 10:25:22.000000 obsarray-0.2.7/quality_documentation/review_checklists/qf-16c.docx
+-rw-r--r--   0 seh2     (2077935315) 226434968    44592 2021-10-13 10:25:22.000000 obsarray-0.2.7/quality_documentation/review_checklists/qf-16d.docx
+-rw-r--r--   0 seh2     (2077935315) 226434968    21030 2021-10-13 10:25:23.000000 obsarray-0.2.7/quality_documentation/review_checklists/qf-16e.docx
+-rw-r--r--   0 seh2     (2077935315) 226434968    21190 2021-10-13 10:25:23.000000 obsarray-0.2.7/quality_documentation/review_checklists/qf-16f.docx
+-rw-r--r--   0 seh2     (2077935315) 226434968     6760 2021-10-13 10:25:22.000000 obsarray-0.2.7/quality_documentation/softwareRequirements.sty
+-rw-r--r--   0 seh2     (2077935315) 226434968    82250 2021-10-13 10:25:22.000000 obsarray-0.2.7/quality_documentation/sphinx.sty
+-rw-r--r--   0 seh2     (2077935315) 226434968     2583 2021-10-13 10:25:22.000000 obsarray-0.2.7/quality_documentation/sphinxcyrillic.sty
+-rw-r--r--   0 seh2     (2077935315) 226434968     8137 2021-10-13 10:25:22.000000 obsarray-0.2.7/quality_documentation/sphinxhighlight.sty
+-rw-r--r--   0 seh2     (2077935315) 226434968     3251 2021-10-13 10:25:22.000000 obsarray-0.2.7/quality_documentation/sphinxhowto.cls
+-rw-r--r--   0 seh2     (2077935315) 226434968     4236 2021-10-13 10:25:22.000000 obsarray-0.2.7/quality_documentation/sphinxmanual.cls
+-rw-r--r--   0 seh2     (2077935315) 226434968      745 2021-10-13 10:25:22.000000 obsarray-0.2.7/quality_documentation/sphinxmessages.sty
+-rw-r--r--   0 seh2     (2077935315) 226434968    14606 2021-10-13 10:25:22.000000 obsarray-0.2.7/quality_documentation/sphinxmulticell.sty
+drwxr-xr-x   0 seh2     (2077935315) 226434968        0 2024-04-02 11:02:18.559531 obsarray-0.2.7/quality_documentation/uml/
+-rw-r--r--   0 seh2     (2077935315) 226434968      102 2021-10-13 10:25:22.000000 obsarray-0.2.7/quality_documentation/uml/copy your design png file into this folder.txt
+-rw-r--r--   0 seh2     (2077935315) 226434968      439 2024-04-02 11:02:18.561126 obsarray-0.2.7/setup.cfg
+-rw-r--r--   0 seh2     (2077935315) 226434968     1400 2024-03-27 16:17:00.000000 obsarray-0.2.7/setup.py
+-rw-r--r--   0 seh2     (2077935315) 226434968      245 2021-10-13 10:25:22.000000 obsarray-0.2.7/tox.ini
+-rw-r--r--   0 seh2     (2077935315) 226434968    68750 2024-02-26 10:03:37.000000 obsarray-0.2.7/versioneer.py
```

### Comparing `obsarray-0.2.6/.gitignore` & `obsarray-0.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/LICENSE` & `obsarray-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/PKG-INFO` & `obsarray-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obsarray
-Version: 0.2.6
+Version: 0.2.7
 Summary: Measurement data handling in Python
 Home-page: https://github.com/comet-toolkit/obsarray
 Author: CoMet Toolkit Team
 Author-email: team@comet-toolkit.org
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `obsarray-0.2.6/README.md` & `obsarray-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/docs/Makefile` & `obsarray-0.2.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/docs/conf.py` & `obsarray-0.2.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/docs/index.rst` & `obsarray-0.2.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/docs/make.bat` & `obsarray-0.2.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/obsarray/err_corr.py` & `obsarray-0.2.7/obsarray/err_corr.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,44 +65,45 @@
 
     @property
     @abc.abstractmethod
     def form(self) -> str:
         """Form name"""
         pass
 
-    def expand_dim_matrix(
-        self, submatrix: np.ndarray, submatrix_dim: Union[str, List[str]], sli: tuple
-    ):
-        return expand_errcorr_dims(
-            in_corr=submatrix,
-            in_dim=submatrix_dim,
-            out_dim=list(self._obj[self._unc_var_name][sli].dims),
-            dim_sizes=self.get_sliced_dim_sizes_uncvar(sli),
-        )
+    def get_varshape_errcorr(self):
+        """
+        return shape of uncertainty variable, including only dimensions which are included in the current error correlation form.
+
+        :return: shape of included dimensions
+        """
+        all_dims = self._obj[self._unc_var_name].dims
+        all_dims_sizes = self._obj.sizes
+
+        return tuple([all_dims_sizes[dim] for dim in all_dims if dim in self.dims])
 
     def get_sliced_dim_sizes_uncvar(self, sli: tuple) -> dict:
         """
         Return dictionary with sizes of sliced dimensions of unc variable, including all dimensions.
 
         :param sli: slice (tuple with slice for each dimension)
-        :return: shape of included sliced dimensions
+        :return: dictionary with shape of included sliced dimensions
         """
         uncvar_dims = self._obj[self._unc_var_name][sli].dims
         uncvar_shape = self._obj[self._unc_var_name][sli].shape
         return {
             uncvar_dims[idim]: uncvar_shape[idim] for idim in range(len(uncvar_dims))
         }
 
     def get_sliced_dim_sizes_errcorr(self, sli: tuple) -> dict:
         """
         Return dictionary with sizes of sliced dimensions of unc variable, including only dimensions which are
         included in the current error correlation form.
 
         :param sli: slice (tuple with slice for each dimension)
-        :return: shape of included sliced dimensions
+        :return: dictionary with shape of included sliced dimensions
         """
         uncvar_sizes = self.get_sliced_dim_sizes_uncvar(sli)
         sliced_dims = self.get_sliced_dims_errcorr(sli)
 
         return {dim: uncvar_sizes[dim] for dim in sliced_dims}
 
     def get_sliced_dims_errcorr(self, sli: tuple) -> list:
@@ -127,25 +128,29 @@
         :return: shape of included sliced dimensions
         """
         uncvar_sizes = self.get_sliced_dim_sizes_uncvar(sli)
         sliced_dims = self.get_sliced_dims_errcorr(sli)
 
         return tuple([uncvar_sizes[dim] for dim in sliced_dims])
 
-    def slice_full_cov(self, full_matrix: np.ndarray, sli: tuple) -> np.ndarray:
-        return self.slice_flattened_matrix(
-            full_matrix, self._obj[self._unc_var_name].shape, sli
-        )
+    def slice_errcorr_matrix(self, err_corr_matrix, variable_shape, sli) -> np.ndarray:
+        """
+        Slice the provided error correlation matrix (typically the error correlation matrix of the
+        BaseErrCorrForm) using the
 
-    def slice_flattened_matrix(self, flattened_matrix, variable_shape, sli):
+        :param err_corr_matrix: error correlation matrix to be sliced
+        :param variable_shape: tuple with the length of the dimensions in the error correlation matrix (in correct order for flattening)
+        :param sli: slice of observation variable to return error-correlation matrix for
+        :return: sliced error correlation matrix
+        """
         mask_array = np.ones(variable_shape, dtype=bool)
         mask_array[sli] = False
 
         return np.delete(
-            np.delete(flattened_matrix, mask_array.ravel(), 0), mask_array.ravel(), 1
+            np.delete(err_corr_matrix, mask_array.ravel(), 0), mask_array.ravel(), 1
         )
 
     @abc.abstractmethod
     def build_matrix(self, sli: Union[np.ndarray, tuple]) -> np.ndarray:
         """
         Returns uncertainty effect error-correlation matrix, populated with error-correlation values defined
         in this parameterisation
@@ -154,24 +159,32 @@
 
         :return: populated error-correlation matrix
         """
         pass
 
     def build_dot_matrix(self, sli: Union[np.ndarray, tuple]) -> np.ndarray:
         """
-        Returns uncertainty effect error-correlation matrix, populated with error-correlation values defined
-        in this parameterisation
+        Returns expanded error correlation matrix for use in dot product with error correlation
+        in other dimensions.
 
-        :param sli: slice of observation variable to return error-correlation matrix for
+        The (sliced) error correlation matrix for this BaseErrCorrForm is expanded from its current
+        (sliced) dimensions (which often don't include all dimensions of the associated uncertainty
+        variable) to the dimensions of the full (sliced) error correlation (i.e. all dimensions of
+        the uncertainty).
+        The returned matrix is not meaningfull unless combined in a dot product with the expanded
+        matrices of other error correlation matrices (together spanning all uncertainty dimensions).
 
-        :return: populated error-correlation matrix
+        :param sli: slice of observation variable to return error-correlation matrix for
+        :return: expanded matrix for use in dot product with error correlation in other dimensions.
         """
-
-        return self.expand_dim_matrix(
-            self.build_matrix(sli), self.get_sliced_dims_errcorr(sli), sli
+        return expand_errcorr_dims(
+            in_corr=self.build_matrix(sli),
+            in_dim=self.get_sliced_dims_errcorr(sli),
+            out_dim=list(self._obj[self._unc_var_name][sli].dims),
+            dim_sizes=self.get_sliced_dim_sizes_uncvar(sli),
         )
 
 
 def register_err_corr_form(form_name: str) -> Callable:
     """
     Decorator for registering error-correlation parmaterisation form definition to package definition container
 
@@ -246,32 +259,22 @@
         Returns uncertainty effect error-correlation matrix, populated with error-correlation values defined
         in this parameterisation
 
         :param sli: slice of observation variable to return error-correlation matrix for
 
         :return: populated error-correlation matrix
         """
-
         all_dims = self._obj[self._unc_var_name].dims
-        all_dims_sizes = self._obj.sizes
 
         sli_submatrix = tuple(
             [sli[i] for i in range(len(all_dims)) if all_dims[i] in self.dims]
         )
 
-        sliced_shape = tuple(
-            [
-                all_dims_sizes[all_dims[i]]
-                for i in range(len(all_dims))
-                if all_dims[i] in self.dims
-            ]
-        )
-
-        submatrix = self.slice_flattened_matrix(
-            self._obj[self.params[0]], sliced_shape, sli_submatrix
+        submatrix = self.slice_errcorr_matrix(
+            self._obj[self.params[0]], self.get_varshape_errcorr(), sli_submatrix
         )
 
         return submatrix
 
 
 @register_err_corr_form("ensemble")
 class EnsembleCorrelation(BaseErrCorrForm):
```

### Comparing `obsarray-0.2.6/obsarray/flag_accessor.py` & `obsarray-0.2.7/obsarray/flag_accessor.py`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/obsarray/templater/dataset_util.py` & `obsarray-0.2.7/obsarray/templater/dataset_util.py`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/obsarray/templater/dstemplater.py` & `obsarray-0.2.7/obsarray/templater/dstemplater.py`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/obsarray/templater/dswriter.py` & `obsarray-0.2.7/obsarray/templater/dswriter.py`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/obsarray/templater/template_util.py` & `obsarray-0.2.7/obsarray/templater/template_util.py`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/obsarray/templater/template_util_jon.py` & `obsarray-0.2.7/obsarray/templater/template_util_jon.py`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/obsarray/templater/tests/test_dataset_util.py` & `obsarray-0.2.7/obsarray/templater/tests/test_dataset_util.py`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/obsarray/templater/tests/test_dswriter.py` & `obsarray-0.2.7/obsarray/templater/tests/test_dswriter.py`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/obsarray/templater/tests/test_template_util.py` & `obsarray-0.2.7/obsarray/templater/tests/test_template_util.py`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/obsarray/test/test_err_corr_forms.py` & `obsarray-0.2.7/obsarray/test/test_err_corr_forms.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import unittest
 import numpy as np
 from obsarray.err_corr import (
     BaseErrCorrForm,
     ErrCorrForms,
     RandomCorrelation,
     SystematicCorrelation,
+    ErrCorrMatrixCorrelation,
 )
 from obsarray.test.test_unc_accessor import create_ds
 
 __author__ = "Sam Hunt <sam.hunt@npl.co.uk>"
 __all__ = []
 
 
@@ -61,26 +62,34 @@
     def setUp(self) -> None:
         self.ds = create_ds()
 
         class BasicErrCorrForm(BaseErrCorrForm):
             form = "basic"
 
             def build_matrix(self, sli):
-                return None
+                full_matrix = np.arange(144).reshape((12, 12))
+                return self.slice_errcorr_matrix(full_matrix, (2, 2, 3), sli)
 
         self.BasicErrCorrForm = BasicErrCorrForm
 
+    def test_get_varshape_errcorr(self):
+        basicerrcorr = self.BasicErrCorrForm(
+            self.ds, "u_ran_temperature", ["x", "y", "time"], [], []
+        )
+        shape = basicerrcorr.get_varshape_errcorr()
+        np.testing.assert_equal(shape, (2, 2, 3))
+
     def test_slice_full_cov_full(self):
         basicerrcorr = self.BasicErrCorrForm(
             self.ds, "u_ran_temperature", ["x"], [], []
         )
 
         full_matrix = np.arange(144).reshape((12, 12))
-        slice_matrix = basicerrcorr.slice_full_cov(
-            full_matrix, (slice(None), slice(None), slice(None))
+        slice_matrix = basicerrcorr.build_matrix(
+            (slice(None), slice(None), slice(None))
         )
 
         np.testing.assert_equal(full_matrix, slice_matrix)
 
     def test_get_sliced_dim_sizes_uncvar(self):
         basicerrcorr = self.BasicErrCorrForm(
             self.ds, "u_ran_temperature", ["x"], [], []
@@ -114,39 +123,36 @@
         assert shape == (2,)
         basicerrcorr = self.BasicErrCorrForm(
             self.ds, "u_ran_temperature", ["x", "time"], [], []
         )
         shape = basicerrcorr.get_sliced_shape_errcorr((slice(None), 0, slice(0, 2, 1)))
         assert shape == (2, 2)
 
-    def test_slice_flattened_matrix(self):
+    def test_slice_errcorr_matrix(self):
         basicerrcorr = self.BasicErrCorrForm(
-            self.ds, "u_ran_temperature", ["x"], [], []
+            self.ds, "u_ran_temperature", ["x", "y", "z"], [], []
         )
 
         full_matrix = np.arange(144).reshape((12, 12))
-        slice_matrix = basicerrcorr.slice_flattened_matrix(
+        slice_matrix = basicerrcorr.slice_errcorr_matrix(
             full_matrix, (2, 2, 3), (slice(None), slice(None), 0)
         )
 
         exp_slice_matrix = np.array(
             [[0, 3, 6, 9], [36, 39, 42, 45], [72, 75, 78, 81], [108, 111, 114, 117]]
         )
 
         np.testing.assert_equal(slice_matrix, exp_slice_matrix)
 
     def test_slice_full_cov_slice(self):
         basicerrcorr = self.BasicErrCorrForm(
-            self.ds, "u_ran_temperature", ["x"], [], []
+            self.ds, "u_ran_temperature", ["x", "y", "z"], [], []
         )
 
-        full_matrix = np.arange(144).reshape((12, 12))
-        slice_matrix = basicerrcorr.slice_full_cov(
-            full_matrix, (slice(None), slice(None), 0)
-        )
+        slice_matrix = basicerrcorr.build_dot_matrix((slice(None), slice(None), 0))
 
         exp_slice_matrix = np.array(
             [[0, 3, 6, 9], [36, 39, 42, 45], [72, 75, 78, 81], [108, 111, 114, 117]]
         )
 
         np.testing.assert_equal(slice_matrix, exp_slice_matrix)
 
@@ -202,9 +208,44 @@
         x = self.build_matrix_1stdim()
         y = self.build_matrix_2nddim()
         time = self.build_matrix_3ddim()
         print(x.dot(y), x, y)
         np.testing.assert_equal((x.dot(y)).dot(time), np.ones((12, 12)))
 
 
+class TestErrCorrMatrixCorrelation(unittest.TestCase):
+    def setUp(self) -> None:
+        self.ds = create_ds()
+
+    def test_build_matrix_full(self):
+        ec = ErrCorrMatrixCorrelation(
+            self.ds,
+            "u_str_temperature",
+            ["x", "time"],
+            ["err_corr_str_temperature"],
+            [],
+        )
+
+        ecrm = ec.build_matrix((slice(None), slice(None), slice(None)))
+        np.testing.assert_equal(ecrm, np.ones((6, 6)))
+
+    def test_build_matrix_sliced(self):
+        ec = ErrCorrMatrixCorrelation(
+            self.ds,
+            "u_str_temperature",
+            ["x", "time"],
+            ["err_corr_str_temperature"],
+            [],
+        )
+
+        ecrm = ec.build_matrix((0, slice(None), slice(None)))
+        np.testing.assert_equal(ecrm, np.ones((3, 3)))
+
+        ecrm = ec.build_matrix((slice(None), 0, slice(None)))
+        np.testing.assert_equal(ecrm, np.ones((6, 6)))
+
+        ecrm = ec.build_matrix((slice(None), slice(None), 0))
+        np.testing.assert_equal(ecrm, np.ones((2, 2)))
+
+
 if __name__ == "main":
     unittest.main()
```

### Comparing `obsarray-0.2.6/obsarray/test/test_flag_accessor.py` & `obsarray-0.2.7/obsarray/test/test_flag_accessor.py`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/obsarray/test/test_unc_accessor.py` & `obsarray-0.2.7/obsarray/test/test_unc_accessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,36 +94,36 @@
     ds.unc["temperature"]["u_str_temperature"] = (
         ["x", "y", "time"],
         temperature * 0.1,
         {
             "units": "K",
             "err_corr": [
                 {
-                    "dim": "x",
+                    "dim": ["x", "time"],
                     "form": "err_corr_matrix",
                     "params": ["err_corr_str_temperature"],
                 },
                 {
                     "dim": "y",
                     "form": "systematic",
                     "params": [],
                 },
-                {
-                    "dim": "time",
-                    "form": "systematic",
-                    "params": [],
-                },
             ],
             "pdf_shape": "gaussian",
         },
     )
 
     ds["err_corr_str_temperature"] = (
-        ["x", "x"],
-        np.eye(temperature.shape[0]),
+        ["x.time", "x.time"],
+        np.ones(
+            (
+                temperature.shape[0] * temperature.shape[2],
+                temperature.shape[0] * temperature.shape[2],
+            )
+        ),
     )
 
     return ds
 
 
 class TestUncAccessor(unittest.TestCase):
     def setUp(self):
```

### Comparing `obsarray-0.2.6/obsarray/unc_accessor.py` & `obsarray-0.2.7/obsarray/unc_accessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -350,15 +350,15 @@
 
         :return: Error-covariance matrix
         """
 
         err_cov_matrix = empty_err_corr_matrix(self._obj[self._unc_var_name][self._sli])
 
         err_cov_matrix.values = convert_corr_to_cov(
-            self.err_corr_matrix().values, self.value.values
+            self.err_corr_matrix().values, self.abs_value.values
         )
 
         return err_cov_matrix
 
 
 class VariableUncertainty:
     """
```

### Comparing `obsarray-0.2.6/obsarray/utils.py` & `obsarray-0.2.7/obsarray/utils.py`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/obsarray.egg-info/PKG-INFO` & `obsarray-0.2.7/obsarray.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obsarray
-Version: 0.2.6
+Version: 0.2.7
 Summary: Measurement data handling in Python
 Home-page: https://github.com/comet-toolkit/obsarray
 Author: CoMet Toolkit Team
 Author-email: team@comet-toolkit.org
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `obsarray-0.2.6/obsarray.egg-info/SOURCES.txt` & `obsarray-0.2.7/obsarray.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -20,22 +20,20 @@
 obsarray.egg-info/PKG-INFO
 obsarray.egg-info/SOURCES.txt
 obsarray.egg-info/dependency_links.txt
 obsarray.egg-info/requires.txt
 obsarray.egg-info/top_level.txt
 obsarray/templater/__init__.py
 obsarray/templater/dataset_util.py
-obsarray/templater/dsdoc.py
 obsarray/templater/dstemplater.py
 obsarray/templater/dswriter.py
 obsarray/templater/template_util.py
 obsarray/templater/template_util_jon.py
 obsarray/templater/tests/__init__.py
 obsarray/templater/tests/test_dataset_util.py
-obsarray/templater/tests/test_dsdoc.py
 obsarray/templater/tests/test_dswriter.py
 obsarray/templater/tests/test_template_util.py
 obsarray/test/__init__.py
 obsarray/test/test_err_corr_forms.py
 obsarray/test/test_flag_accessor.py
 obsarray/test/test_unc_accessor.py
 quality_documentation/.gitignore
```

### Comparing `obsarray-0.2.6/quality_documentation/.gitignore` & `obsarray-0.2.7/quality_documentation/.gitignore`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/quality_documentation/QualityDocumentation.tex` & `obsarray-0.2.7/quality_documentation/QualityDocumentation.tex`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/quality_documentation/base/metadata.tex` & `obsarray-0.2.7/quality_documentation/base/metadata.tex`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/quality_documentation/base/sil2.tex` & `obsarray-0.2.7/quality_documentation/base/sil2.tex`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/quality_documentation/base/sil3.tex` & `obsarray-0.2.7/quality_documentation/base/sil3.tex`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/quality_documentation/footnotehyper-sphinx.sty` & `obsarray-0.2.7/quality_documentation/footnotehyper-sphinx.sty`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/quality_documentation/obsarray_QF-59.docm` & `obsarray-0.2.7/quality_documentation/obsarray_QF-59.docm`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/quality_documentation/obsarray_requirements.docx` & `obsarray-0.2.7/quality_documentation/obsarray_requirements.docx`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/quality_documentation/review_checklists/qf-16a.docx` & `obsarray-0.2.7/quality_documentation/review_checklists/qf-16a.docx`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/quality_documentation/review_checklists/qf-16b.docx` & `obsarray-0.2.7/quality_documentation/review_checklists/qf-16b.docx`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/quality_documentation/review_checklists/qf-16c.docx` & `obsarray-0.2.7/quality_documentation/review_checklists/qf-16c.docx`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/quality_documentation/review_checklists/qf-16d.docx` & `obsarray-0.2.7/quality_documentation/review_checklists/qf-16d.docx`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/quality_documentation/review_checklists/qf-16e.docx` & `obsarray-0.2.7/quality_documentation/review_checklists/qf-16e.docx`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/quality_documentation/review_checklists/qf-16f.docx` & `obsarray-0.2.7/quality_documentation/review_checklists/qf-16f.docx`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/quality_documentation/softwareRequirements.sty` & `obsarray-0.2.7/quality_documentation/softwareRequirements.sty`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/quality_documentation/sphinx.sty` & `obsarray-0.2.7/quality_documentation/sphinx.sty`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/quality_documentation/sphinxcyrillic.sty` & `obsarray-0.2.7/quality_documentation/sphinxcyrillic.sty`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/quality_documentation/sphinxhighlight.sty` & `obsarray-0.2.7/quality_documentation/sphinxhighlight.sty`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/quality_documentation/sphinxhowto.cls` & `obsarray-0.2.7/quality_documentation/sphinxhowto.cls`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/quality_documentation/sphinxmanual.cls` & `obsarray-0.2.7/quality_documentation/sphinxmanual.cls`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/quality_documentation/sphinxmessages.sty` & `obsarray-0.2.7/quality_documentation/sphinxmessages.sty`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/quality_documentation/sphinxmulticell.sty` & `obsarray-0.2.7/quality_documentation/sphinxmulticell.sty`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/setup.py` & `obsarray-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `obsarray-0.2.6/versioneer.py` & `obsarray-0.2.7/versioneer.py`

 * *Files identical despite different names*

