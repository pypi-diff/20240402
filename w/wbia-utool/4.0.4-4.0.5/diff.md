# Comparing `tmp/wbia-utool-4.0.4.tar.gz` & `tmp/wbia-utool-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbia-utool-4.0.4.tar", last modified: Tue Dec 14 06:36:44 2021, max compression
+gzip compressed data, was "wbia-utool-4.0.5.tar", last modified: Tue Apr  2 01:41:20 2024, max compression
```

## Comparing `wbia-utool-4.0.4.tar` & `wbia-utool-4.0.5.tar`

### file list

```diff
@@ -1,291 +1,296 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 06:36:44.541099 wbia-utool-4.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 06:36:44.469099 wbia-utool-4.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 06:36:44.473099 wbia-utool-4.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1891 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1664 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/.github/workflows/testing.yml
--rw-r--r--   0 runner    (1001) docker     (121)      669 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1326 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      698 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/.pypirc
--rw-r--r--   0 runner    (1001) docker     (121)    10616 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/.travis.yml
--rwxr-xr-x   0 runner    (1001) docker     (121)    11324 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3023 2021-12-14 06:36:44.541099 wbia-utool-4.0.4/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (121)     1972 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      619 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 06:36:44.473099 wbia-utool-4.0.4/_docs/
--rw-r--r--   0 runner    (1001) docker     (121)      581 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/_docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     2007 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/_docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      440 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/_docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      787 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/_docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)     2638 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/_docs/utool._internal.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1043 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/_docs/utool.experimental.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8922 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/_docs/utool.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1051 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/_docs/utool.tests.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)      238 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/build_documentation.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      276 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/clean.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 06:36:44.481099 wbia-utool-4.0.4/docs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/.nojekyll
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 06:36:44.481099 wbia-utool-4.0.4/docs/_modules/
--rw-r--r--   0 runner    (1001) docker     (121)     8657 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/index.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 06:36:44.497099 wbia-utool-4.0.4/docs/_modules/utool/
--rw-r--r--   0 runner    (1001) docker     (121)    19158 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/DynamicStruct.html
--rw-r--r--   0 runner    (1001) docker     (121)   105537 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/Preferences.html
--rw-r--r--   0 runner    (1001) docker     (121)    37431 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/Printable.html
--rw-r--r--   0 runner    (1001) docker     (121)     5718 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/__main__.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 06:36:44.501099 wbia-utool-4.0.4/docs/_modules/utool/_internal/
--rw-r--r--   0 runner    (1001) docker     (121)    19753 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/_internal/meta_util_arg.html
--rw-r--r--   0 runner    (1001) docker     (121)     8026 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/_internal/meta_util_cache.html
--rw-r--r--   0 runner    (1001) docker     (121)     8082 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/_internal/meta_util_cplat.html
--rw-r--r--   0 runner    (1001) docker     (121)    10789 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/_internal/meta_util_dbg.html
--rw-r--r--   0 runner    (1001) docker     (121)     9336 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/_internal/meta_util_iter.html
--rw-r--r--   0 runner    (1001) docker     (121)     8024 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/_internal/meta_util_path.html
--rw-r--r--   0 runner    (1001) docker     (121)    20553 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/_internal/meta_util_six.html
--rw-r--r--   0 runner    (1001) docker     (121)     9905 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/_internal/py2_syntax_funcs.html
--rw-r--r--   0 runner    (1001) docker     (121)    20279 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/_internal/randomwrap.html
--rw-r--r--   0 runner    (1001) docker     (121)    64995 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/_internal/util_importer.html
--rw-r--r--   0 runner    (1001) docker     (121)    81827 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/_internal/win32_send_keys.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 06:36:44.501099 wbia-utool-4.0.4/docs/_modules/utool/experimental/
--rw-r--r--   0 runner    (1001) docker     (121)   135119 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/experimental/dynamic_connectivity.html
--rw-r--r--   0 runner    (1001) docker     (121)   159219 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/experimental/euler_tour_tree_avl.html
--rw-r--r--   0 runner    (1001) docker     (121)    44205 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/experimental/pandas_highlight.html
--rw-r--r--   0 runner    (1001) docker     (121)    70251 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/oldalg.html
--rw-r--r--   0 runner    (1001) docker     (121)     8699 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/sandbox.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 06:36:44.501099 wbia-utool-4.0.4/docs/_modules/utool/tests/
--rw-r--r--   0 runner    (1001) docker     (121)    32661 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/tests/_oldtest_decor.html
--rw-r--r--   0 runner    (1001) docker     (121)    22738 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/tests/_oldtest_hash.html
--rw-r--r--   0 runner    (1001) docker     (121)    13945 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/tests/_oldtest_logging.html
--rw-r--r--   0 runner    (1001) docker     (121)    11699 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/tests/_oldtest_reloading.html
--rw-r--r--   0 runner    (1001) docker     (121)    23792 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/tests/run_tests.html
--rw-r--r--   0 runner    (1001) docker     (121)   352426 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_alg.html
--rw-r--r--   0 runner    (1001) docker     (121)   166412 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_arg.html
--rw-r--r--   0 runner    (1001) docker     (121)    59493 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_assert.html
--rw-r--r--   0 runner    (1001) docker     (121)   136173 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_autogen.html
--rw-r--r--   0 runner    (1001) docker     (121)   237764 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_cache.html
--rw-r--r--   0 runner    (1001) docker     (121)   134920 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_class.html
--rw-r--r--   0 runner    (1001) docker     (121)    11236 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_config.html
--rw-r--r--   0 runner    (1001) docker     (121)   185917 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_cplat.html
--rw-r--r--   0 runner    (1001) docker     (121)    72608 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_csv.html
--rw-r--r--   0 runner    (1001) docker     (121)   196784 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_dbg.html
--rw-r--r--   0 runner    (1001) docker     (121)   116604 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_decor.html
--rw-r--r--   0 runner    (1001) docker     (121)    13449 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_depricated.html
--rw-r--r--   0 runner    (1001) docker     (121)   477572 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_dev.html
--rw-r--r--   0 runner    (1001) docker     (121)   237254 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_dict.html
--rw-r--r--   0 runner    (1001) docker     (121)     7046 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_func.html
--rw-r--r--   0 runner    (1001) docker     (121)   170577 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_git.html
--rw-r--r--   0 runner    (1001) docker     (121)   166931 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_grabdata.html
--rw-r--r--   0 runner    (1001) docker     (121)   324520 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_graph.html
--rw-r--r--   0 runner    (1001) docker     (121)   312161 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_gridsearch.html
--rw-r--r--   0 runner    (1001) docker     (121)   139077 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_hash.html
--rw-r--r--   0 runner    (1001) docker     (121)    67983 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_import.html
--rw-r--r--   0 runner    (1001) docker     (121)    92304 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_inject.html
--rw-r--r--   0 runner    (1001) docker     (121)   439580 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_inspect.html
--rw-r--r--   0 runner    (1001) docker     (121)   104618 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_io.html
--rw-r--r--   0 runner    (1001) docker     (121)    50057 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_ipynb.html
--rw-r--r--   0 runner    (1001) docker     (121)    66256 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_iter.html
--rw-r--r--   0 runner    (1001) docker     (121)   150716 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_latex.html
--rw-r--r--   0 runner    (1001) docker     (121)   359802 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_list.html
--rw-r--r--   0 runner    (1001) docker     (121)    75688 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_logging.html
--rw-r--r--   0 runner    (1001) docker     (121)    24138 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_num.html
--rw-r--r--   0 runner    (1001) docker     (121)    51857 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_numpy.html
--rw-r--r--   0 runner    (1001) docker     (121)   124344 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_parallel.html
--rw-r--r--   0 runner    (1001) docker     (121)   352194 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_path.html
--rw-r--r--   0 runner    (1001) docker     (121)    46622 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_print.html
--rw-r--r--   0 runner    (1001) docker     (121)    36271 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_profile.html
--rw-r--r--   0 runner    (1001) docker     (121)   128224 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_progress.html
--rw-r--r--   0 runner    (1001) docker     (121)   114713 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_project.html
--rw-r--r--   0 runner    (1001) docker     (121)    62997 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_regex.html
--rw-r--r--   0 runner    (1001) docker     (121)    40201 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_resources.html
--rw-r--r--   0 runner    (1001) docker     (121)    24973 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_set.html
--rw-r--r--   0 runner    (1001) docker     (121)    86103 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_setup.html
--rw-r--r--   0 runner    (1001) docker     (121)    32862 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_sqlite.html
--rw-r--r--   0 runner    (1001) docker     (121)   435678 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_str.html
--rw-r--r--   0 runner    (1001) docker     (121)    35175 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_sysreq.html
--rw-r--r--   0 runner    (1001) docker     (121)    45414 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_tags.html
--rw-r--r--   0 runner    (1001) docker     (121)   294334 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_tests.html
--rw-r--r--   0 runner    (1001) docker     (121)   142619 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_time.html
--rw-r--r--   0 runner    (1001) docker     (121)    63603 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_type.html
--rw-r--r--   0 runner    (1001) docker     (121)   100574 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_ubuntu.html
--rw-r--r--   0 runner    (1001) docker     (121)    18905 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_web.html
--rw-r--r--   0 runner    (1001) docker     (121)    19568 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool/util_win32.html
--rw-r--r--   0 runner    (1001) docker     (121)   172719 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_modules/utool.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 06:36:44.501099 wbia-utool-4.0.4/docs/_sources/
--rw-r--r--   0 runner    (1001) docker     (121)      440 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_sources/index.rst.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2638 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_sources/utool._internal.rst.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1043 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_sources/utool.experimental.rst.txt
--rw-r--r--   0 runner    (1001) docker     (121)     8922 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_sources/utool.rst.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1051 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_sources/utool.tests.rst.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 06:36:44.505099 wbia-utool-4.0.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)    11185 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/alabaster.css
--rw-r--r--   0 runner    (1001) docker     (121)    14667 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/basic.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 06:36:44.505099 wbia-utool-4.0.4/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (121)     3275 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/css/badge_only.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 06:36:44.513099 wbia-utool-4.0.4/docs/_static/css/fonts/
--rw-r--r--   0 runner    (1001) docker     (121)    87624 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (121)    67312 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    86288 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (121)    66444 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (121)   165742 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (121)   444379 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (121)   165548 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    98024 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (121)    77160 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 runner    (1001) docker     (121)   323344 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0 runner    (1001) docker     (121)   193308 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (121)   309728 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/css/fonts/lato-bold.woff
--rw-r--r--   0 runner    (1001) docker     (121)   184912 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0 runner    (1001) docker     (121)   328412 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0 runner    (1001) docker     (121)   195704 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (121)   309192 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/css/fonts/lato-normal.woff
--rw-r--r--   0 runner    (1001) docker     (121)   182708 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0 runner    (1001) docker     (121)   129674 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/css/theme.css
--rw-r--r--   0 runner    (1001) docker     (121)       42 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (121)     9630 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (121)      355 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/documentation_options.js
--rw-r--r--   0 runner    (1001) docker     (121)      286 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (121)   287630 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/jquery-3.5.1.js
--rw-r--r--   0 runner    (1001) docker     (121)    89476 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/jquery.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 06:36:44.513099 wbia-utool-4.0.4/docs/_static/js/
--rw-r--r--   0 runner    (1001) docker     (121)      934 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/js/badge_only.js
--rw-r--r--   0 runner    (1001) docker     (121)     4370 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0 runner    (1001) docker     (121)     2734 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/js/html5shiv.min.js
--rw-r--r--   0 runner    (1001) docker     (121)     5023 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/js/theme.js
--rw-r--r--   0 runner    (1001) docker     (121)    10854 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/language_data.js
--rw-r--r--   0 runner    (1001) docker     (121)       90 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (121)       90 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (121)     4819 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (121)    16793 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (121)    68420 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/underscore-1.13.1.js
--rw-r--r--   0 runner    (1001) docker     (121)    19530 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/_static/underscore.js
--rw-r--r--   0 runner    (1001) docker     (121)   285224 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/genindex.html
--rw-r--r--   0 runner    (1001) docker     (121)    17645 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (121)    16779 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/objects.inv
--rw-r--r--   0 runner    (1001) docker     (121)    22349 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/py-modindex.html
--rw-r--r--   0 runner    (1001) docker     (121)     3679 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/search.html
--rw-r--r--   0 runner    (1001) docker     (121)   153481 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/searchindex.js
--rw-r--r--   0 runner    (1001) docker     (121)    64718 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/utool._internal.html
--rw-r--r--   0 runner    (1001) docker     (121)   154499 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/utool.experimental.html
--rw-r--r--   0 runner    (1001) docker     (121)  4066098 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/utool.html
--rw-r--r--   0 runner    (1001) docker     (121)    42157 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/docs/utool.tests.html
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 06:36:44.517099 wbia-utool-4.0.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)       63 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/requirements/build.txt
--rw-r--r--   0 runner    (1001) docker     (121)      141 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/requirements/optional.txt
--rw-r--r--   0 runner    (1001) docker     (121)      140 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/requirements/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (121)       80 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)      122 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/run_developer_setup.sh
--rw-r--r--   0 runner    (1001) docker     (121)     2429 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     7715 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 06:36:44.529099 wbia-utool-4.0.4/utool/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3428 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/DynamicStruct.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    25499 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/Preferences.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6623 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/Printable.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6926 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/__depricated_utils
--rwxr-xr-x   0 runner    (1001) docker     (121)    52920 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      568 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 06:36:44.529099 wbia-utool-4.0.4/utool/_graveyard/
--rwxr-xr-x   0 runner    (1001) docker     (121)     9193 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/_graveyard/__prefwidg_dep.py
--rw-r--r--   0 runner    (1001) docker     (121)     4165 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/_graveyard/broken.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5119 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/_graveyard/util_distances.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 06:36:44.533099 wbia-utool-4.0.4/utool/_internal/
--rwxr-xr-x   0 runner    (1001) docker     (121)      316 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/_internal/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3961 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/_internal/meta_util_arg.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1204 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/_internal/meta_util_cache.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      253 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/_internal/meta_util_constants.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1216 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/_internal/meta_util_cplat.py
--rw-r--r--   0 runner    (1001) docker     (121)     1573 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/_internal/meta_util_dbg.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1418 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/_internal/meta_util_git.py
--rw-r--r--   0 runner    (1001) docker     (121)     2386 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/_internal/meta_util_iter.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      916 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/_internal/meta_util_path.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4377 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/_internal/meta_util_six.py
--rw-r--r--   0 runner    (1001) docker     (121)     2478 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/_internal/py2_syntax_funcs.py
--rw-r--r--   0 runner    (1001) docker     (121)     5533 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/_internal/randomwrap.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    17734 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/_internal/util_importer.py
--rw-r--r--   0 runner    (1001) docker     (121)    18318 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/_internal/win32_send_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 06:36:44.533099 wbia-utool-4.0.4/utool/experimental/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12986 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/experimental/bytecode_optimizations.py
--rw-r--r--   0 runner    (1001) docker     (121)    32017 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/experimental/dynamic_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (121)    37431 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/experimental/euler_tour_tree_avl.py
--rw-r--r--   0 runner    (1001) docker     (121)     8897 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/experimental/pandas_highlight.py
--rw-r--r--   0 runner    (1001) docker     (121)     1538 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/experimental/tmp.py.bak
--rw-r--r--   0 runner    (1001) docker     (121)    16673 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/oldalg.py
--rw-r--r--   0 runner    (1001) docker     (121)     1289 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/sandbox.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 06:36:44.537099 wbia-utool-4.0.4/utool/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       89 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4991 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/tests/_oldtest_decor.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4552 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/tests/_oldtest_hash.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2279 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/tests/_oldtest_logging.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1654 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/tests/_oldtest_reloading.py
--rw-r--r--   0 runner    (1001) docker     (121)     5616 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/tests/run_tests.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    98002 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_alg.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      421 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_aliases.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    45912 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_arg.py
--rw-r--r--   0 runner    (1001) docker     (121)    11386 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_assert.py
--rw-r--r--   0 runner    (1001) docker     (121)    38066 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_autogen.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    55959 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_cache.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    36265 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_class.py
--rw-r--r--   0 runner    (1001) docker     (121)     2169 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     4494 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_const.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    49128 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_cplat.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    13888 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_csv.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    49518 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_dbg.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    35005 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_decor.py
--rw-r--r--   0 runner    (1001) docker     (121)     3372 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_depricated.py
--rwxr-xr-x   0 runner    (1001) docker     (121)   117101 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_dev.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    69217 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_dict.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1430 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_func.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    38400 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_git.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    47333 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_grabdata.py
--rw-r--r--   0 runner    (1001) docker     (121)    85854 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_graph.py
--rw-r--r--   0 runner    (1001) docker     (121)    86907 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_gridsearch.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    40756 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_hash.py
--rw-r--r--   0 runner    (1001) docker     (121)    21490 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_import.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    22153 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_inject.py
--rwxr-xr-x   0 runner    (1001) docker     (121)   121614 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_inspect.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    29907 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_io.py
--rw-r--r--   0 runner    (1001) docker     (121)    11856 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_ipynb.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    19841 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_iter.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    34814 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_latex.py
--rwxr-xr-x   0 runner    (1001) docker     (121)   105602 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_list.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    21349 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_logging.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4256 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_num.py
--rw-r--r--   0 runner    (1001) docker     (121)    12790 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_numpy.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    38011 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_parallel.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    93724 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_path.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11590 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_print.py
--rw-r--r--   0 runner    (1001) docker     (121)     7742 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_profile.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    37570 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_progress.py
--rw-r--r--   0 runner    (1001) docker     (121)    35144 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_project.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    14805 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_regex.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9872 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 06:36:44.541099 wbia-utool-4.0.4/utool/util_scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)      360 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_scripts/autogen_sphinx_docs.py
--rw-r--r--   0 runner    (1001) docker     (121)     4894 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_scripts/check_jedi.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3500 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_scripts/classfuncs.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      202 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_scripts/dump_utool_init.py
--rw-r--r--   0 runner    (1001) docker     (121)     7950 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_scripts/ensure_python3_compatible.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      530 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_scripts/grabzippedurl.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2571 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_scripts/local_info.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      271 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_scripts/makeinit.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2081 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_scripts/makesetup.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1080 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_scripts/permit_gitrepo.py
--rw-r--r--   0 runner    (1001) docker     (121)     3151 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_scripts/pipinfo.py
--rw-r--r--   0 runner    (1001) docker     (121)     2686 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_scripts/pyproj_checker.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      308 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_scripts/remove_injects.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      324 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_scripts/util_lite_resource.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      641 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_scripts/utoolwc.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4189 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_scripts/utprof.sh
--rw-r--r--   0 runner    (1001) docker     (121)      391 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_scripts/viewdir.py
--rw-r--r--   0 runner    (1001) docker     (121)     5265 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_set.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    22623 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_setup.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      105 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_six.py
--rw-r--r--   0 runner    (1001) docker     (121)     7308 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_sqlite.py
--rwxr-xr-x   0 runner    (1001) docker     (121)   119678 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_str.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8321 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_sysreq.py
--rw-r--r--   0 runner    (1001) docker     (121)    10793 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_tags.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    79118 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_tests.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    37689 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_time.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    15670 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    25982 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_ubuntu.py
--rw-r--r--   0 runner    (1001) docker     (121)     3855 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_web.py
--rw-r--r--   0 runner    (1001) docker     (121)     3850 2021-12-14 06:36:31.000000 wbia-utool-4.0.4/utool/util_win32.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:41:20.868203 wbia-utool-4.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:41:20.788203 wbia-utool-4.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:41:20.792203 wbia-utool-4.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/.github/workflows/testing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/.pre-commit-config.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11324 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-04-02 01:41:20.868203 wbia-utool-4.0.5/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1972 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:41:20.796203 wbia-utool-4.0.5/_docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/_docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/_docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/_docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/_docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/_docs/utool._internal.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/_docs/utool.experimental.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/_docs/utool.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/_docs/utool.tests.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)      181 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/build_documentation.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      276 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/clean.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:41:20.804203 wbia-utool-4.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/.nojekyll
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:41:20.804203 wbia-utool-4.0.5/docs/_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     8657 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:41:20.820203 wbia-utool-4.0.5/docs/_modules/utool/
+-rw-r--r--   0 runner    (1001) docker     (127)    19158 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/DynamicStruct.html
+-rw-r--r--   0 runner    (1001) docker     (127)   105537 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/Preferences.html
+-rw-r--r--   0 runner    (1001) docker     (127)    37431 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/Printable.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/__main__.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:41:20.824203 wbia-utool-4.0.5/docs/_modules/utool/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)    19753 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/_internal/meta_util_arg.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/_internal/meta_util_cache.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8082 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/_internal/meta_util_cplat.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/_internal/meta_util_dbg.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9336 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/_internal/meta_util_iter.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8024 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/_internal/meta_util_path.html
+-rw-r--r--   0 runner    (1001) docker     (127)    20553 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/_internal/meta_util_six.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9905 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/_internal/py2_syntax_funcs.html
+-rw-r--r--   0 runner    (1001) docker     (127)    20279 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/_internal/randomwrap.html
+-rw-r--r--   0 runner    (1001) docker     (127)    64995 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/_internal/util_importer.html
+-rw-r--r--   0 runner    (1001) docker     (127)    81827 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/_internal/win32_send_keys.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:41:20.824203 wbia-utool-4.0.5/docs/_modules/utool/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)   135119 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/experimental/dynamic_connectivity.html
+-rw-r--r--   0 runner    (1001) docker     (127)   159219 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/experimental/euler_tour_tree_avl.html
+-rw-r--r--   0 runner    (1001) docker     (127)    44205 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/experimental/pandas_highlight.html
+-rw-r--r--   0 runner    (1001) docker     (127)    70251 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/oldalg.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8699 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/sandbox.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:41:20.824203 wbia-utool-4.0.5/docs/_modules/utool/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    32661 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/tests/_oldtest_decor.html
+-rw-r--r--   0 runner    (1001) docker     (127)    22738 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/tests/_oldtest_hash.html
+-rw-r--r--   0 runner    (1001) docker     (127)    13945 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/tests/_oldtest_logging.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11699 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/tests/_oldtest_reloading.html
+-rw-r--r--   0 runner    (1001) docker     (127)    23792 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/tests/run_tests.html
+-rw-r--r--   0 runner    (1001) docker     (127)   352426 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_alg.html
+-rw-r--r--   0 runner    (1001) docker     (127)   166412 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_arg.html
+-rw-r--r--   0 runner    (1001) docker     (127)    59493 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_assert.html
+-rw-r--r--   0 runner    (1001) docker     (127)   136173 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_autogen.html
+-rw-r--r--   0 runner    (1001) docker     (127)   237764 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_cache.html
+-rw-r--r--   0 runner    (1001) docker     (127)   134920 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_class.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11236 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_config.html
+-rw-r--r--   0 runner    (1001) docker     (127)   185917 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_cplat.html
+-rw-r--r--   0 runner    (1001) docker     (127)    72608 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_csv.html
+-rw-r--r--   0 runner    (1001) docker     (127)   196784 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_dbg.html
+-rw-r--r--   0 runner    (1001) docker     (127)   116604 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_decor.html
+-rw-r--r--   0 runner    (1001) docker     (127)    13449 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_depricated.html
+-rw-r--r--   0 runner    (1001) docker     (127)   477572 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_dev.html
+-rw-r--r--   0 runner    (1001) docker     (127)   237254 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_dict.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7046 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_func.html
+-rw-r--r--   0 runner    (1001) docker     (127)   170577 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_git.html
+-rw-r--r--   0 runner    (1001) docker     (127)   166931 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_grabdata.html
+-rw-r--r--   0 runner    (1001) docker     (127)   324520 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_graph.html
+-rw-r--r--   0 runner    (1001) docker     (127)   312161 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_gridsearch.html
+-rw-r--r--   0 runner    (1001) docker     (127)   139077 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_hash.html
+-rw-r--r--   0 runner    (1001) docker     (127)    67983 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_import.html
+-rw-r--r--   0 runner    (1001) docker     (127)    92304 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_inject.html
+-rw-r--r--   0 runner    (1001) docker     (127)   439580 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_inspect.html
+-rw-r--r--   0 runner    (1001) docker     (127)   104618 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_io.html
+-rw-r--r--   0 runner    (1001) docker     (127)    50057 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_ipynb.html
+-rw-r--r--   0 runner    (1001) docker     (127)    66256 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_iter.html
+-rw-r--r--   0 runner    (1001) docker     (127)   150716 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_latex.html
+-rw-r--r--   0 runner    (1001) docker     (127)   359802 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)    75688 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_logging.html
+-rw-r--r--   0 runner    (1001) docker     (127)    24138 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_num.html
+-rw-r--r--   0 runner    (1001) docker     (127)    51857 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_numpy.html
+-rw-r--r--   0 runner    (1001) docker     (127)   124344 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_parallel.html
+-rw-r--r--   0 runner    (1001) docker     (127)   352194 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_path.html
+-rw-r--r--   0 runner    (1001) docker     (127)    46622 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_print.html
+-rw-r--r--   0 runner    (1001) docker     (127)    36271 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_profile.html
+-rw-r--r--   0 runner    (1001) docker     (127)   128224 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_progress.html
+-rw-r--r--   0 runner    (1001) docker     (127)   114713 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_project.html
+-rw-r--r--   0 runner    (1001) docker     (127)    62997 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_regex.html
+-rw-r--r--   0 runner    (1001) docker     (127)    40201 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_resources.html
+-rw-r--r--   0 runner    (1001) docker     (127)    24973 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_set.html
+-rw-r--r--   0 runner    (1001) docker     (127)    86103 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_setup.html
+-rw-r--r--   0 runner    (1001) docker     (127)    32862 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_sqlite.html
+-rw-r--r--   0 runner    (1001) docker     (127)   435678 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_str.html
+-rw-r--r--   0 runner    (1001) docker     (127)    35175 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_sysreq.html
+-rw-r--r--   0 runner    (1001) docker     (127)    45414 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_tags.html
+-rw-r--r--   0 runner    (1001) docker     (127)   294334 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_tests.html
+-rw-r--r--   0 runner    (1001) docker     (127)   142619 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_time.html
+-rw-r--r--   0 runner    (1001) docker     (127)    63603 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_type.html
+-rw-r--r--   0 runner    (1001) docker     (127)   100574 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_ubuntu.html
+-rw-r--r--   0 runner    (1001) docker     (127)    18905 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_web.html
+-rw-r--r--   0 runner    (1001) docker     (127)    19568 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool/util_win32.html
+-rw-r--r--   0 runner    (1001) docker     (127)   172719 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_modules/utool.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:41:20.828203 wbia-utool-4.0.5/docs/_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_sources/index.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_sources/utool._internal.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_sources/utool.experimental.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_sources/utool.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_sources/utool.tests.rst.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:41:20.828203 wbia-utool-4.0.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    11185 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/alabaster.css
+-rw-r--r--   0 runner    (1001) docker     (127)    14667 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/basic.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:41:20.832203 wbia-utool-4.0.5/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/css/badge_only.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:41:20.836203 wbia-utool-4.0.5/docs/_static/css/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    87624 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    67312 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    86288 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    66444 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   165742 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   444379 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   165548 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    98024 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    77160 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   323344 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   193308 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   309728 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   184912 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   328412 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   195704 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   309192 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   182708 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   129674 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/css/theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     9630 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/doctools.js
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/documentation_options.js
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/file.png
+-rw-r--r--   0 runner    (1001) docker     (127)   287630 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/jquery-3.5.1.js
+-rw-r--r--   0 runner    (1001) docker     (127)    89476 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/jquery.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:41:20.836203 wbia-utool-4.0.5/docs/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/js/badge_only.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/js/html5shiv.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/js/theme.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10854 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/language_data.js
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (127)    16793 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/searchtools.js
+-rw-r--r--   0 runner    (1001) docker     (127)    68420 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/underscore-1.13.1.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19530 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/_static/underscore.js
+-rw-r--r--   0 runner    (1001) docker     (127)   285013 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (127)    17521 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    16766 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/objects.inv
+-rw-r--r--   0 runner    (1001) docker     (127)    22148 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/py-modindex.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/search.html
+-rw-r--r--   0 runner    (1001) docker     (127)   153460 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/searchindex.js
+-rw-r--r--   0 runner    (1001) docker     (127)    64718 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/utool._internal.html
+-rw-r--r--   0 runner    (1001) docker     (127)   154499 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/utool.experimental.html
+-rw-r--r--   0 runner    (1001) docker     (127)  4065772 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/utool.html
+-rw-r--r--   0 runner    (1001) docker     (127)    42157 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/docs/utool.tests.html
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:41:20.840203 wbia-utool-4.0.5/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/requirements/build.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/requirements/optional.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/requirements/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      122 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/run_developer_setup.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-02 01:41:20.868203 wbia-utool-4.0.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7715 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:41:20.852203 wbia-utool-4.0.5/utool/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3428 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/DynamicStruct.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25499 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/Preferences.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6623 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/Printable.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6926 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/__depricated_utils
+-rwxr-xr-x   0 runner    (1001) docker     (127)    52920 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:41:20.852203 wbia-utool-4.0.5/utool/_graveyard/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9193 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/_graveyard/__prefwidg_dep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/_graveyard/broken.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5119 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/_graveyard/util_distances.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:41:20.856203 wbia-utool-4.0.5/utool/_internal/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      316 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/_internal/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3961 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/_internal/meta_util_arg.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1204 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/_internal/meta_util_cache.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      253 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/_internal/meta_util_constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1216 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/_internal/meta_util_cplat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/_internal/meta_util_dbg.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1418 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/_internal/meta_util_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/_internal/meta_util_iter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      916 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/_internal/meta_util_path.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4377 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/_internal/meta_util_six.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/_internal/py2_syntax_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/_internal/randomwrap.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17734 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/_internal/util_importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18318 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/_internal/win32_send_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-02 01:41:20.000000 wbia-utool-4.0.5/utool/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:41:20.856203 wbia-utool-4.0.5/utool/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12986 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/experimental/bytecode_optimizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32017 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/experimental/dynamic_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37431 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/experimental/euler_tour_tree_avl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8897 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/experimental/pandas_highlight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/experimental/tmp.py.bak
+-rw-r--r--   0 runner    (1001) docker     (127)    16673 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/oldalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/sandbox.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:41:20.856203 wbia-utool-4.0.5/utool/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/tests/_oldtest_decor.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4552 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/tests/_oldtest_hash.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2279 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/tests/_oldtest_logging.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1654 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/tests/_oldtest_reloading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/tests/run_tests.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    98002 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_alg.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      421 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_aliases.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    45912 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_arg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11386 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_assert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38066 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_autogen.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    55959 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_cache.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    36265 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_const.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    49128 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_cplat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13888 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_csv.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    49518 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_dbg.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35005 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_decor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_depricated.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   117101 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_dev.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    69217 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_dict.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1430 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_func.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    38400 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_git.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    47710 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_grabdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86330 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86907 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_gridsearch.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    40756 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21490 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_import.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22153 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_inject.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   121614 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_inspect.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29907 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11856 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_ipynb.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19841 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_iter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    34814 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_latex.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   105602 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_list.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21349 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_logging.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4256 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_num.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12790 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_numpy.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    38011 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_parallel.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    93724 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_path.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11590 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_print.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7742 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_profile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    37570 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35144 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_project.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14805 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_regex.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9872 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:41:20.860203 wbia-utool-4.0.5/utool/util_scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      360 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_scripts/autogen_sphinx_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_scripts/check_jedi.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3500 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_scripts/classfuncs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      202 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_scripts/dump_utool_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7950 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_scripts/ensure_python3_compatible.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      530 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_scripts/grabzippedurl.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2571 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_scripts/local_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      271 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_scripts/makeinit.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2081 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_scripts/makesetup.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1080 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_scripts/permit_gitrepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_scripts/pipinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_scripts/pyproj_checker.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      308 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_scripts/remove_injects.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      324 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_scripts/util_lite_resource.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      641 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_scripts/utoolwc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4189 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_scripts/utprof.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_scripts/viewdir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_set.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22623 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      105 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_six.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_sqlite.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   119678 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_str.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8321 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_sysreq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10793 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_tags.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    79118 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_tests.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    37689 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_time.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15670 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25982 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_ubuntu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_web.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-04-02 01:41:10.000000 wbia-utool-4.0.5/utool/util_win32.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:41:20.860203 wbia-utool-4.0.5/wbia_utool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-04-02 01:41:20.000000 wbia-utool-4.0.5/wbia_utool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8291 2024-04-02 01:41:20.000000 wbia-utool-4.0.5/wbia_utool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 01:41:20.000000 wbia-utool-4.0.5/wbia_utool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-02 01:41:20.000000 wbia-utool-4.0.5/wbia_utool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-02 01:41:20.000000 wbia-utool-4.0.5/wbia_utool.egg-info/top_level.txt
```

### Comparing `wbia-utool-4.0.4/.github/workflows/python-publish.yml` & `wbia-utool-4.0.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/.github/workflows/testing.yml` & `wbia-utool-4.0.5/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/.gitignore` & `wbia-utool-4.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/.pre-commit-config.yaml` & `wbia-utool-4.0.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/LICENSE` & `wbia-utool-4.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/README.rst` & `wbia-utool-4.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/SECURITY.md` & `wbia-utool-4.0.5/SECURITY.md`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/_docs/Makefile` & `wbia-utool-4.0.5/_docs/Makefile`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/_docs/conf.py` & `wbia-utool-4.0.5/_docs/conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 # -*- coding: utf-8 -*-
 from sphinx.ext.autodoc import between
 from datetime import date
 import sys
 import os
 
-try:
-    from _version import __version__
-except Exception:
-    __version__ = 'latest'
-
 sys.path.append(sys.path.insert(0, os.path.abspath('../')))
 
 autosummary_generate = True
 
 modindex_common_prefix = ['_']
 
 master_doc = 'index'
@@ -31,16 +26,24 @@
         'donate.html',
     ]
 }
 
 # -- Project information -----------------------------------------------------
 
 project = 'wbia-utool'
+
 copyright = f'{date.today().year}, Wild Me'
 author = 'Wild Me (wildme.org)'
+
+try:
+    from importlib.metadata import version
+
+    __version__ = version(project)
+except Exception:
+    __version__ = 'latest'
 version = __version__
 release = version
 
 # -- General configuration ---------------------------------------------------
 
 MOCK_MODULES = []
 if len(MOCK_MODULES) > 0:
```

### Comparing `wbia-utool-4.0.4/_docs/make.bat` & `wbia-utool-4.0.5/_docs/make.bat`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/_docs/utool._internal.rst` & `wbia-utool-4.0.5/_docs/utool._internal.rst`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/_docs/utool.experimental.rst` & `wbia-utool-4.0.5/_docs/utool.experimental.rst`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/_docs/utool.rst` & `wbia-utool-4.0.5/_docs/utool.rst`

 * *Files 0% similar despite different names*

```diff
@@ -41,22 +41,14 @@
 -------------------------
 
 .. automodule:: utool.__main__
     :members:
     :undoc-members:
     :show-inheritance:
 
-utool.\_version module
-----------------------
-
-.. automodule:: utool._version
-    :members:
-    :undoc-members:
-    :show-inheritance:
-
 utool.oldalg module
 -------------------
 
 .. automodule:: utool.oldalg
     :members:
     :undoc-members:
     :show-inheritance:
```

### Comparing `wbia-utool-4.0.4/_docs/utool.tests.rst` & `wbia-utool-4.0.5/_docs/utool.tests.rst`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/index.html` & `wbia-utool-4.0.5/docs/_modules/index.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/DynamicStruct.html` & `wbia-utool-4.0.5/docs/_modules/utool/DynamicStruct.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/Preferences.html` & `wbia-utool-4.0.5/docs/_modules/utool/Preferences.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/Printable.html` & `wbia-utool-4.0.5/docs/_modules/utool/Printable.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/__main__.html` & `wbia-utool-4.0.5/docs/_modules/utool/__main__.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/_internal/meta_util_arg.html` & `wbia-utool-4.0.5/docs/_modules/utool/_internal/meta_util_arg.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/_internal/meta_util_cache.html` & `wbia-utool-4.0.5/docs/_modules/utool/_internal/meta_util_cache.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/_internal/meta_util_cplat.html` & `wbia-utool-4.0.5/docs/_modules/utool/_internal/meta_util_cplat.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/_internal/meta_util_dbg.html` & `wbia-utool-4.0.5/docs/_modules/utool/_internal/meta_util_dbg.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/_internal/meta_util_iter.html` & `wbia-utool-4.0.5/docs/_modules/utool/_internal/meta_util_iter.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/_internal/meta_util_path.html` & `wbia-utool-4.0.5/docs/_modules/utool/_internal/meta_util_path.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/_internal/meta_util_six.html` & `wbia-utool-4.0.5/docs/_modules/utool/_internal/meta_util_six.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/_internal/py2_syntax_funcs.html` & `wbia-utool-4.0.5/docs/_modules/utool/_internal/py2_syntax_funcs.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/_internal/randomwrap.html` & `wbia-utool-4.0.5/docs/_modules/utool/_internal/randomwrap.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/_internal/util_importer.html` & `wbia-utool-4.0.5/docs/_modules/utool/_internal/util_importer.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/_internal/win32_send_keys.html` & `wbia-utool-4.0.5/docs/_modules/utool/_internal/win32_send_keys.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/experimental/dynamic_connectivity.html` & `wbia-utool-4.0.5/docs/_modules/utool/experimental/dynamic_connectivity.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/experimental/euler_tour_tree_avl.html` & `wbia-utool-4.0.5/docs/_modules/utool/experimental/euler_tour_tree_avl.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/experimental/pandas_highlight.html` & `wbia-utool-4.0.5/docs/_modules/utool/experimental/pandas_highlight.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/oldalg.html` & `wbia-utool-4.0.5/docs/_modules/utool/oldalg.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/sandbox.html` & `wbia-utool-4.0.5/docs/_modules/utool/sandbox.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/tests/_oldtest_decor.html` & `wbia-utool-4.0.5/docs/_modules/utool/tests/_oldtest_decor.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/tests/_oldtest_hash.html` & `wbia-utool-4.0.5/docs/_modules/utool/tests/_oldtest_hash.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/tests/_oldtest_logging.html` & `wbia-utool-4.0.5/docs/_modules/utool/tests/_oldtest_logging.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/tests/_oldtest_reloading.html` & `wbia-utool-4.0.5/docs/_modules/utool/tests/_oldtest_reloading.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/tests/run_tests.html` & `wbia-utool-4.0.5/docs/_modules/utool/tests/run_tests.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_alg.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_alg.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_arg.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_arg.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_assert.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_assert.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_autogen.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_autogen.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_cache.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_cache.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_class.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_class.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_config.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_config.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_cplat.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_cplat.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_csv.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_csv.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_dbg.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_dbg.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_decor.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_decor.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_depricated.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_depricated.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_dev.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_dev.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_dict.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_dict.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_func.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_func.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_git.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_git.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_grabdata.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_grabdata.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_graph.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_graph.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_gridsearch.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_gridsearch.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_hash.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_hash.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_import.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_import.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_inject.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_inject.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_inspect.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_inspect.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_io.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_io.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_ipynb.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_ipynb.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_iter.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_iter.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_latex.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_latex.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_list.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_list.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_logging.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_logging.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_num.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_num.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_numpy.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_numpy.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_parallel.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_parallel.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_path.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_path.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_print.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_print.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_profile.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_profile.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_progress.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_progress.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_project.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_project.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_regex.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_regex.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_resources.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_resources.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_set.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_set.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_setup.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_setup.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_sqlite.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_sqlite.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_str.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_str.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_sysreq.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_sysreq.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_tags.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_tags.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_tests.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_tests.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_time.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_time.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_type.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_type.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_ubuntu.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_ubuntu.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_web.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_web.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool/util_win32.html` & `wbia-utool-4.0.5/docs/_modules/utool/util_win32.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_modules/utool.html` & `wbia-utool-4.0.5/docs/_modules/utool.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_sources/utool._internal.rst.txt` & `wbia-utool-4.0.5/docs/_sources/utool._internal.rst.txt`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_sources/utool.experimental.rst.txt` & `wbia-utool-4.0.5/docs/_sources/utool.experimental.rst.txt`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_sources/utool.rst.txt` & `wbia-utool-4.0.5/docs/_sources/utool.rst.txt`

 * *Files 0% similar despite different names*

```diff
@@ -41,22 +41,14 @@
 -------------------------
 
 .. automodule:: utool.__main__
     :members:
     :undoc-members:
     :show-inheritance:
 
-utool.\_version module
-----------------------
-
-.. automodule:: utool._version
-    :members:
-    :undoc-members:
-    :show-inheritance:
-
 utool.oldalg module
 -------------------
 
 .. automodule:: utool.oldalg
     :members:
     :undoc-members:
     :show-inheritance:
```

### Comparing `wbia-utool-4.0.4/docs/_sources/utool.tests.rst.txt` & `wbia-utool-4.0.5/docs/_sources/utool.tests.rst.txt`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_static/alabaster.css` & `wbia-utool-4.0.5/docs/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_static/basic.css` & `wbia-utool-4.0.5/docs/_static/basic.css`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_static/css/badge_only.css` & `wbia-utool-4.0.5/docs/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_static/css/fonts/Roboto-Slab-Bold.woff` & `wbia-utool-4.0.5/docs/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_static/css/fonts/Roboto-Slab-Bold.woff2` & `wbia-utool-4.0.5/docs/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_static/css/fonts/Roboto-Slab-Regular.woff` & `wbia-utool-4.0.5/docs/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_static/css/fonts/Roboto-Slab-Regular.woff2` & `wbia-utool-4.0.5/docs/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_static/css/fonts/fontawesome-webfont.eot` & `wbia-utool-4.0.5/docs/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_static/css/fonts/fontawesome-webfont.svg` & `wbia-utool-4.0.5/docs/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_static/css/fonts/fontawesome-webfont.ttf` & `wbia-utool-4.0.5/docs/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_static/css/fonts/fontawesome-webfont.woff` & `wbia-utool-4.0.5/docs/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_static/css/fonts/fontawesome-webfont.woff2` & `wbia-utool-4.0.5/docs/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_static/css/fonts/lato-bold-italic.woff` & `wbia-utool-4.0.5/docs/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_static/css/fonts/lato-bold-italic.woff2` & `wbia-utool-4.0.5/docs/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_static/css/fonts/lato-bold.woff` & `wbia-utool-4.0.5/docs/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_static/css/fonts/lato-bold.woff2` & `wbia-utool-4.0.5/docs/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_static/css/fonts/lato-normal-italic.woff` & `wbia-utool-4.0.5/docs/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_static/css/fonts/lato-normal-italic.woff2` & `wbia-utool-4.0.5/docs/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_static/css/fonts/lato-normal.woff` & `wbia-utool-4.0.5/docs/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_static/css/fonts/lato-normal.woff2` & `wbia-utool-4.0.5/docs/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_static/css/theme.css` & `wbia-utool-4.0.5/docs/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_static/doctools.js` & `wbia-utool-4.0.5/docs/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_static/jquery-3.5.1.js` & `wbia-utool-4.0.5/docs/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_static/jquery.js` & `wbia-utool-4.0.5/docs/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_static/js/badge_only.js` & `wbia-utool-4.0.5/docs/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_static/js/html5shiv-printshiv.min.js` & `wbia-utool-4.0.5/docs/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_static/js/html5shiv.min.js` & `wbia-utool-4.0.5/docs/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_static/js/theme.js` & `wbia-utool-4.0.5/docs/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_static/language_data.js` & `wbia-utool-4.0.5/docs/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_static/pygments.css` & `wbia-utool-4.0.5/docs/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_static/searchtools.js` & `wbia-utool-4.0.5/docs/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_static/underscore-1.13.1.js` & `wbia-utool-4.0.5/docs/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/_static/underscore.js` & `wbia-utool-4.0.5/docs/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/genindex.html` & `wbia-utool-4.0.5/docs/genindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -2955,16 +2955,14 @@
 </li>
         <li><a href="utool._internal.html#module-utool._internal.randomwrap">utool._internal.randomwrap</a>
 </li>
         <li><a href="utool._internal.html#module-utool._internal.util_importer">utool._internal.util_importer</a>
 </li>
         <li><a href="utool._internal.html#module-utool._internal.win32_send_keys">utool._internal.win32_send_keys</a>
 </li>
-        <li><a href="utool.html#module-utool._version">utool._version</a>
-</li>
         <li><a href="utool.html#module-utool.DynamicStruct">utool.DynamicStruct</a>
 </li>
         <li><a href="utool.experimental.html#module-utool.experimental">utool.experimental</a>
 </li>
         <li><a href="utool.experimental.html#module-utool.experimental.bytecode_optimizations">utool.experimental.bytecode_optimizations</a>
 </li>
         <li><a href="utool.experimental.html#module-utool.experimental.dynamic_connectivity">utool.experimental.dynamic_connectivity</a>
@@ -4691,21 +4689,14 @@
     utool._internal.win32_send_keys
 
       <ul>
         <li><a href="utool._internal.html#module-utool._internal.win32_send_keys">module</a>
 </li>
       </ul></li>
       <li>
-    utool._version
-
-      <ul>
-        <li><a href="utool.html#module-utool._version">module</a>
-</li>
-      </ul></li>
-      <li>
     utool.DynamicStruct
 
       <ul>
         <li><a href="utool.html#module-utool.DynamicStruct">module</a>
 </li>
       </ul></li>
       <li>
@@ -4788,23 +4779,23 @@
       <li>
     utool.tests._oldtest_hash
 
       <ul>
         <li><a href="utool.tests.html#module-utool.tests._oldtest_hash">module</a>
 </li>
       </ul></li>
-  </ul></td>
-  <td style="width: 33%; vertical-align: top;"><ul>
       <li>
     utool.tests._oldtest_logging
 
       <ul>
         <li><a href="utool.tests.html#module-utool.tests._oldtest_logging">module</a>
 </li>
       </ul></li>
+  </ul></td>
+  <td style="width: 33%; vertical-align: top;"><ul>
       <li>
     utool.tests._oldtest_reloading
 
       <ul>
         <li><a href="utool.tests.html#module-utool.tests._oldtest_reloading">module</a>
 </li>
       </ul></li>
```

#### html2text {}

```diff
@@ -1262,15 +1262,14 @@
           o _u_t_o_o_l_.___i_n_t_e_r_n_a_l_._m_e_t_a___u_t_i_l___i_t_e_r
           o _u_t_o_o_l_.___i_n_t_e_r_n_a_l_._m_e_t_a___u_t_i_l___p_a_t_h
           o _u_t_o_o_l_.___i_n_t_e_r_n_a_l_._m_e_t_a___u_t_i_l___s_i_x
           o _u_t_o_o_l_.___i_n_t_e_r_n_a_l_._p_y_2___s_y_n_t_a_x___f_u_n_c_s
           o _u_t_o_o_l_.___i_n_t_e_r_n_a_l_._r_a_n_d_o_m_w_r_a_p
           o _u_t_o_o_l_.___i_n_t_e_r_n_a_l_._u_t_i_l___i_m_p_o_r_t_e_r
           o _u_t_o_o_l_.___i_n_t_e_r_n_a_l_._w_i_n_3_2___s_e_n_d___k_e_y_s
-          o _u_t_o_o_l_.___v_e_r_s_i_o_n
           o _u_t_o_o_l_._D_y_n_a_m_i_c_S_t_r_u_c_t
           o _u_t_o_o_l_._e_x_p_e_r_i_m_e_n_t_a_l
           o _u_t_o_o_l_._e_x_p_e_r_i_m_e_n_t_a_l_._b_y_t_e_c_o_d_e___o_p_t_i_m_i_z_a_t_i_o_n_s
           o _u_t_o_o_l_._e_x_p_e_r_i_m_e_n_t_a_l_._d_y_n_a_m_i_c___c_o_n_n_e_c_t_i_v_i_t_y
           o _u_t_o_o_l_._e_x_p_e_r_i_m_e_n_t_a_l_._e_u_l_e_r___t_o_u_r___t_r_e_e___a_v_l
           o _u_t_o_o_l_._e_x_p_e_r_i_m_e_n_t_a_l_._p_a_n_d_a_s___h_i_g_h_l_i_g_h_t
           o _u_t_o_o_l_._o_l_d_a_l_g
@@ -1841,102 +1840,100 @@
     * _t_i_m_e___s_t_r_2_(_)_ _(_i_n_ _m_o_d_u_l_e
       _u_t_o_o_l_._u_t_i_l___r_e_s_o_u_r_c_e_s_)
     * _t_i_m_e_i_t___c_o_m_p_a_r_e_(_)_ _(_i_n_ _m_o_d_u_l_e
       _u_t_o_o_l_._u_t_i_l___d_e_v_)
     * _t_i_m_e_i_t___g_r_i_d_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___d_e_v_)
     * _T_i_m_e_r_ _(_c_l_a_s_s_ _i_n_ _u_t_o_o_l_._u_t_i_l___t_i_m_e_)
 ********** UU **********
-    * _u_n_a_r_c_h_i_v_e___f_i_l_e_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___g_r_a_b_d_a_t_a_)                 * utool.tests._oldtest_logging
+    * _u_n_a_r_c_h_i_v_e___f_i_l_e_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___g_r_a_b_d_a_t_a_)                 * utool.tests._oldtest_reloading
     * _u_n_e_v_a_l_u_a_t_e_d___k_e_y_s_(_)_ _(_u_t_o_o_l_._u_t_i_l___c_a_c_h_e_._L_a_z_y_D_i_c_t_ _m_e_t_h_o_d_)                  o _m_o_d_u_l_e
-    * _u_n_e_x_p_a_n_d_u_s_e_r_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___p_a_t_h_)                       * utool.tests._oldtest_reloading
+    * _u_n_e_x_p_a_n_d_u_s_e_r_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___p_a_t_h_)                       * utool.tests.run_tests
     * _u_n_f_l_a_t___m_a_p_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___l_i_s_t_)                               o _m_o_d_u_l_e
-    * _u_n_f_l_a_t___t_a_k_e_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___l_i_s_t_)                        * utool.tests.run_tests
+    * _u_n_f_l_a_t___t_a_k_e_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___l_i_s_t_)                        * utool.util_alg
     * _u_n_f_l_a_t___u_n_i_q_u_e___r_o_w_i_d___m_a_p_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___l_i_s_t_)                  o _m_o_d_u_l_e
-    * _u_n_f_l_a_t___v_e_c_m_a_p_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___l_i_s_t_)                      * utool.util_alg
+    * _u_n_f_l_a_t___v_e_c_m_a_p_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___l_i_s_t_)                      * utool.util_aliases
     * _u_n_f_l_a_t_t_e_n_1_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___l_i_s_t_)                               o _m_o_d_u_l_e
-    * _u_n_f_l_a_t_t_e_n_2_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___l_i_s_t_)                         * utool.util_aliases
+    * _u_n_f_l_a_t_t_e_n_2_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___l_i_s_t_)                         * utool.util_arg
     * _u_n_f_o_r_m_a_t___t_e_x_t___a_s___d_o_c_s_t_r_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___s_t_r_)                   o _m_o_d_u_l_e
-    * _u_n_g_r_o_u_p_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___a_l_g_)                             * utool.util_arg
+    * _u_n_g_r_o_u_p_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___a_l_g_)                             * utool.util_assert
     * _u_n_g_r_o_u_p___g_e_n_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___a_l_g_)                               o _m_o_d_u_l_e
-    * _u_n_g_r_o_u_p___u_n_i_q_u_e_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___a_l_g_)                      * utool.util_assert
+    * _u_n_g_r_o_u_p___u_n_i_q_u_e_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___a_l_g_)                      * utool.util_autogen
     * _u_n_i_n_d_e_n_t_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___s_t_r_)                                  o _m_o_d_u_l_e
-    * _u_n_i_n_v_e_r_t___u_n_i_q_u_e___t_w_o___l_i_s_t_s_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___d_e_v_)           * utool.util_autogen
+    * _u_n_i_n_v_e_r_t___u_n_i_q_u_e___t_w_o___l_i_s_t_s_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___d_e_v_)           * utool.util_cache
     * _u_n_i_o_n_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___l_i_s_t_)                                    o _m_o_d_u_l_e
-          o _(_u_t_o_o_l_._u_t_i_l___g_i_t_._R_e_p_o_M_a_n_a_g_e_r_ _m_e_t_h_o_d_)                        * utool.util_cache
+          o _(_u_t_o_o_l_._u_t_i_l___g_i_t_._R_e_p_o_M_a_n_a_g_e_r_ _m_e_t_h_o_d_)                        * utool.util_class
           o _(_u_t_o_o_l_._u_t_i_l___s_e_t_._O_r_d_e_r_e_d_S_e_t_ _c_l_a_s_s_ _m_e_t_h_o_d_)                         o _m_o_d_u_l_e
-    * _u_n_i_o_n___o_r_d_e_r_e_d_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___l_i_s_t_)                      * utool.util_class
+    * _u_n_i_o_n___o_r_d_e_r_e_d_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___l_i_s_t_)                      * utool.util_config
     * _u_n_i_q_u_e_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___l_i_s_t_)                                   o _m_o_d_u_l_e
-    * _u_n_i_q_u_e___f_l_a_g_s_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___l_i_s_t_)                       * utool.util_config
+    * _u_n_i_q_u_e___f_l_a_g_s_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___l_i_s_t_)                       * utool.util_const
     * _u_n_i_q_u_e___i_n_d_i_c_e_s_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___l_i_s_t_)                           o _m_o_d_u_l_e
-    * _u_n_i_q_u_e___i_n_v_e_r_s_e_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___l_i_s_t_)                     * utool.util_const
+    * _u_n_i_q_u_e___i_n_v_e_r_s_e_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___l_i_s_t_)                     * utool.util_cplat
     * _u_n_i_q_u_e___o_r_d_e_r_e_d_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___l_i_s_t_)                           o _m_o_d_u_l_e
-    * _u_n_i_q_u_e___u_n_o_r_d_e_r_e_d_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___l_i_s_t_)                   * utool.util_cplat
+    * _u_n_i_q_u_e___u_n_o_r_d_e_r_e_d_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___l_i_s_t_)                   * utool.util_csv
     * _u_n_i_x_j_o_i_n_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_.___i_n_t_e_r_n_a_l_._m_e_t_a___u_t_i_l___p_a_t_h_)                  o _m_o_d_u_l_e
-    * _u_n_i_x_p_a_t_h_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_.___i_n_t_e_r_n_a_l_._m_e_t_a___u_t_i_l___p_a_t_h_)            * utool.util_csv
+    * _u_n_i_x_p_a_t_h_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_.___i_n_t_e_r_n_a_l_._m_e_t_a___u_t_i_l___p_a_t_h_)            * utool.util_dbg
     * _u_n_i_x_t_i_m_e___h_o_u_r_d_i_f_f_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___a_l_g_)                         o _m_o_d_u_l_e
-    * _u_n_i_x_t_i_m_e___t_o___d_a_t_e_t_i_m_e_o_b_j_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___t_i_m_e_)            * utool.util_dbg
+    * _u_n_i_x_t_i_m_e___t_o___d_a_t_e_t_i_m_e_o_b_j_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___t_i_m_e_)            * utool.util_decor
     * _u_n_i_x_t_i_m_e___t_o___d_a_t_e_t_i_m_e_s_t_r_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___t_i_m_e_)                  o _m_o_d_u_l_e
-    * _u_n_i_x_t_i_m_e___t_o___t_i_m_e_d_e_l_t_a_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___t_i_m_e_)              * utool.util_decor
+    * _u_n_i_x_t_i_m_e___t_o___t_i_m_e_d_e_l_t_a_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___t_i_m_e_)              * utool.util_depricated
     * _u_n_l_o_a_d___m_o_d_u_l_e_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___c_p_l_a_t_)                           o _m_o_d_u_l_e
-    * _u_n_p_a_c_k___i_t_e_r_a_b_l_e_s_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___l_i_s_t_)                   * utool.util_depricated
+    * _u_n_p_a_c_k___i_t_e_r_a_b_l_e_s_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___l_i_s_t_)                   * utool.util_dev
     * _u_n_t_a_r___f_i_l_e_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___g_r_a_b_d_a_t_a_)                           o _m_o_d_u_l_e
-    * _u_n_z_i_p___f_i_l_e_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___g_r_a_b_d_a_t_a_)                     * utool.util_dev
+    * _u_n_z_i_p___f_i_l_e_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___g_r_a_b_d_a_t_a_)                     * utool.util_dict
     * _u_p_d_a_t_e_(_)_ _(_u_t_o_o_l_._D_y_n_a_m_i_c_S_t_r_u_c_t_._D_y_n_S_t_r_u_c_t_ _m_e_t_h_o_d_)                        o _m_o_d_u_l_e
-          o _(_u_t_o_o_l_._e_x_p_e_r_i_m_e_n_t_a_l_._d_y_n_a_m_i_c___c_o_n_n_e_c_t_i_v_i_t_y_._E_u_l_e_r_T_o_u_r_L_i_s_t     * utool.util_dict
+          o _(_u_t_o_o_l_._e_x_p_e_r_i_m_e_n_t_a_l_._d_y_n_a_m_i_c___c_o_n_n_e_c_t_i_v_i_t_y_._E_u_l_e_r_T_o_u_r_L_i_s_t     * utool.util_func
             _m_e_t_h_o_d_)                                                          o _m_o_d_u_l_e
-          o _(_u_t_o_o_l_._P_r_e_f_e_r_e_n_c_e_s_._P_r_e_f_ _m_e_t_h_o_d_)                            * utool.util_func
+          o _(_u_t_o_o_l_._P_r_e_f_e_r_e_n_c_e_s_._P_r_e_f_ _m_e_t_h_o_d_)                            * utool.util_git
           o _(_u_t_o_o_l_._u_t_i_l___c_a_c_h_e_._L_a_z_y_D_i_c_t_ _m_e_t_h_o_d_)                               o _m_o_d_u_l_e
-          o _(_u_t_o_o_l_._u_t_i_l___d_e_v_._P_r_i_o_r_i_t_y_Q_u_e_u_e_ _m_e_t_h_o_d_)                      * utool.util_git
+          o _(_u_t_o_o_l_._u_t_i_l___d_e_v_._P_r_i_o_r_i_t_y_Q_u_e_u_e_ _m_e_t_h_o_d_)                      * utool.util_grabdata
           o _(_u_t_o_o_l_._u_t_i_l___d_i_c_t_._h_a_s_h_d_i_c_t_ _m_e_t_h_o_d_)                                o _m_o_d_u_l_e
-          o _(_u_t_o_o_l_._u_t_i_l___s_e_t_._O_r_d_e_r_e_d_S_e_t_ _m_e_t_h_o_d_)                         * utool.util_grabdata
+          o _(_u_t_o_o_l_._u_t_i_l___s_e_t_._O_r_d_e_r_e_d_S_e_t_ _m_e_t_h_o_d_)                         * utool.util_graph
     * _u_p_d_a_t_e___d_i_c_t_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___d_i_c_t_)                              o _m_o_d_u_l_e
-    * _u_p_d_a_t_e___e_x_i_s_t_i_n_g_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___d_i_c_t_)                    * utool.util_graph
+    * _u_p_d_a_t_e___e_x_i_s_t_i_n_g_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___d_i_c_t_)                    * utool.util_gridsearch
     * _u_p_d_a_t_e_d___c_f_g_d_i_c_t_(_)_ _(_u_t_o_o_l_._u_t_i_l___g_r_i_d_s_e_a_r_c_h_._P_a_r_a_m_I_n_f_o_L_i_s_t                 o _m_o_d_u_l_e
-      _m_e_t_h_o_d_)                                                          * utool.util_gridsearch
+      _m_e_t_h_o_d_)                                                          * utool.util_hash
     * _u_p_p_e_r___d_i_a_g___s_e_l_f___p_r_o_d_x_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___a_l_g_)                     o _m_o_d_u_l_e
-    * _u_r_l___r_e_a_d_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___g_r_a_b_d_a_t_a_)                       * utool.util_hash
+    * _u_r_l___r_e_a_d_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___g_r_a_b_d_a_t_a_)                       * utool.util_import
     * _u_r_l___r_e_a_d___t_e_x_t_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___g_r_a_b_d_a_t_a_)                        o _m_o_d_u_l_e
-    * _u_s_e_d___m_e_m_o_r_y_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___r_e_s_o_u_r_c_e_s_)                   * utool.util_import
+    * _u_s_e_d___m_e_m_o_r_y_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___r_e_s_o_u_r_c_e_s_)                   * utool.util_inject
     * _u_s_e_r___c_m_d_l_i_n_e___p_r_o_m_p_t_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___d_e_v_)                       o _m_o_d_u_l_e
-    * _U_s_e_r_P_r_o_f_i_l_e_ _(_c_l_a_s_s_ _i_n_ _u_t_o_o_l_._u_t_i_l___p_r_o_j_e_c_t_)                        * utool.util_inject
+    * _U_s_e_r_P_r_o_f_i_l_e_ _(_c_l_a_s_s_ _i_n_ _u_t_o_o_l_._u_t_i_l___p_r_o_j_e_c_t_)                        * utool.util_inspect
     * _u_t_c_n_o_w___t_z_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___t_i_m_e_)                                o _m_o_d_u_l_e
-    * _u_t_f_8___l_e_n_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___s_t_r_)                            * utool.util_inspect
+    * _u_t_f_8___l_e_n_(_)_ _(_i_n_ _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___s_t_r_)                            * utool.util_io
     * utool                                                                  o _m_o_d_u_l_e
-          o _m_o_d_u_l_e                                                     * utool.util_io
-    * utool.__main__                                                         o _m_o_d_u_l_e
           o _m_o_d_u_l_e                                                     * utool.util_ipynb
-    * utool._internal                                                        o _m_o_d_u_l_e
+    * utool.__main__                                                         o _m_o_d_u_l_e
           o _m_o_d_u_l_e                                                     * utool.util_iter
-    * utool._internal.meta_util_arg                                          o _m_o_d_u_l_e
+    * utool._internal                                                        o _m_o_d_u_l_e
           o _m_o_d_u_l_e                                                     * utool.util_latex
-    * utool._internal.meta_util_cache                                        o _m_o_d_u_l_e
+    * utool._internal.meta_util_arg                                          o _m_o_d_u_l_e
           o _m_o_d_u_l_e                                                     * utool.util_list
-    * utool._internal.meta_util_constants                                    o _m_o_d_u_l_e
+    * utool._internal.meta_util_cache                                        o _m_o_d_u_l_e
           o _m_o_d_u_l_e                                                     * utool.util_logging
-    * utool._internal.meta_util_cplat                                        o _m_o_d_u_l_e
+    * utool._internal.meta_util_constants                                    o _m_o_d_u_l_e
           o _m_o_d_u_l_e                                                     * utool.util_num
-    * utool._internal.meta_util_dbg                                          o _m_o_d_u_l_e
+    * utool._internal.meta_util_cplat                                        o _m_o_d_u_l_e
           o _m_o_d_u_l_e                                                     * utool.util_numpy
-    * utool._internal.meta_util_git                                          o _m_o_d_u_l_e
+    * utool._internal.meta_util_dbg                                          o _m_o_d_u_l_e
           o _m_o_d_u_l_e                                                     * utool.util_parallel
-    * utool._internal.meta_util_iter                                         o _m_o_d_u_l_e
+    * utool._internal.meta_util_git                                          o _m_o_d_u_l_e
           o _m_o_d_u_l_e                                                     * utool.util_path
-    * utool._internal.meta_util_path                                         o _m_o_d_u_l_e
+    * utool._internal.meta_util_iter                                         o _m_o_d_u_l_e
           o _m_o_d_u_l_e                                                     * utool.util_print
-    * utool._internal.meta_util_six                                          o _m_o_d_u_l_e
+    * utool._internal.meta_util_path                                         o _m_o_d_u_l_e
           o _m_o_d_u_l_e                                                     * utool.util_profile
-    * utool._internal.py2_syntax_funcs                                       o _m_o_d_u_l_e
+    * utool._internal.meta_util_six                                          o _m_o_d_u_l_e
           o _m_o_d_u_l_e                                                     * utool.util_progress
-    * utool._internal.randomwrap                                             o _m_o_d_u_l_e
+    * utool._internal.py2_syntax_funcs                                       o _m_o_d_u_l_e
           o _m_o_d_u_l_e                                                     * utool.util_project
-    * utool._internal.util_importer                                          o _m_o_d_u_l_e
+    * utool._internal.randomwrap                                             o _m_o_d_u_l_e
           o _m_o_d_u_l_e                                                     * utool.util_regex
-    * utool._internal.win32_send_keys                                        o _m_o_d_u_l_e
+    * utool._internal.util_importer                                          o _m_o_d_u_l_e
           o _m_o_d_u_l_e                                                     * utool.util_resources
-    * utool._version                                                         o _m_o_d_u_l_e
+    * utool._internal.win32_send_keys                                        o _m_o_d_u_l_e
           o _m_o_d_u_l_e                                                     * utool.util_set
     * utool.DynamicStruct                                                    o _m_o_d_u_l_e
           o _m_o_d_u_l_e                                                     * utool.util_setup
     * utool.experimental                                                     o _m_o_d_u_l_e
           o _m_o_d_u_l_e                                                     * utool.util_six
     * utool.experimental.bytecode_optimizations                              o _m_o_d_u_l_e
           o _m_o_d_u_l_e                                                     * utool.util_sqlite
@@ -1956,14 +1953,16 @@
           o _m_o_d_u_l_e                                                     * utool.util_ubuntu
     * utool.tests                                                            o _m_o_d_u_l_e
           o _m_o_d_u_l_e                                                     * utool.util_web
     * utool.tests._oldtest_decor                                             o _m_o_d_u_l_e
           o _m_o_d_u_l_e                                                     * utool.util_win32
     * utool.tests._oldtest_hash                                              o _m_o_d_u_l_e
           o _m_o_d_u_l_e
+    * utool.tests._oldtest_logging
+          o _m_o_d_u_l_e
 ********** VV **********
     * _v_a_l_ _(_u_t_o_o_l_._e_x_p_e_r_i_m_e_n_t_a_l_._e_u_l_e_r___t_o_u_r___t_r_e_e___a_v_l_._N_o_d_e          * _v_a_r_i_n_f_o___s_t_r_(_)_ _(_i_n
       _p_r_o_p_e_r_t_y_)                                                   _m_o_d_u_l_e_ _u_t_o_o_l_._u_t_i_l___s_t_r_)
     * _v_a_l_u_e_(_)_ _(_u_t_o_o_l_._P_r_e_f_e_r_e_n_c_e_s_._P_r_e_f_ _m_e_t_h_o_d_)                   * _v_d_(_)_ _(_i_n_ _m_o_d_u_l_e
     * _v_a_l_u_e_s_(_)_                                                    _u_t_o_o_l_._u_t_i_l___c_p_l_a_t_)
       _(_u_t_o_o_l_._e_x_p_e_r_i_m_e_n_t_a_l_._e_u_l_e_r___t_o_u_r___t_r_e_e___a_v_l_._E_u_l_e_r_T_o_u_r_T_r_e_e     * _v_e_r_t_s___s_t_r_(_)_ _(_i_n_ _m_o_d_u_l_e
       _m_e_t_h_o_d_)                                                     _u_t_o_o_l_._u_t_i_l___s_t_r_)
```

### Comparing `wbia-utool-4.0.4/docs/index.html` & `wbia-utool-4.0.5/docs/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,14 @@
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="utool.html#submodules">Submodules</a></li>
 <li class="toctree-l2"><a class="reference internal" href="utool.html#module-utool.DynamicStruct">utool.DynamicStruct module</a></li>
 <li class="toctree-l2"><a class="reference internal" href="utool.html#module-utool.Preferences">utool.Preferences module</a></li>
 <li class="toctree-l2"><a class="reference internal" href="utool.html#module-utool.Printable">utool.Printable module</a></li>
 <li class="toctree-l2"><a class="reference internal" href="utool.html#module-utool.__main__">utool.__main__ module</a></li>
-<li class="toctree-l2"><a class="reference internal" href="utool.html#module-utool._version">utool._version module</a></li>
 <li class="toctree-l2"><a class="reference internal" href="utool.html#module-utool.oldalg">utool.oldalg module</a></li>
 <li class="toctree-l2"><a class="reference internal" href="utool.html#module-utool.sandbox">utool.sandbox module</a></li>
 <li class="toctree-l2"><a class="reference internal" href="utool.html#module-utool.util_alg">utool.util_alg module</a></li>
 <li class="toctree-l2"><a class="reference internal" href="utool.html#module-utool.util_aliases">utool.util_aliases module</a></li>
 <li class="toctree-l2"><a class="reference internal" href="utool.html#module-utool.util_arg">utool.util_arg module</a></li>
 <li class="toctree-l2"><a class="reference internal" href="utool.html#module-utool.util_assert">utool.util_assert module</a></li>
 <li class="toctree-l2"><a class="reference internal" href="utool.html#module-utool.util_autogen">utool.util_autogen module</a></li>
```

#### html2text {}

```diff
@@ -44,15 +44,14 @@
                       # _u_t_o_o_l_._t_e_s_t_s_._r_u_n___t_e_s_t_s_ _m_o_d_u_l_e
                       # _M_o_d_u_l_e_ _c_o_n_t_e_n_t_s
           o _S_u_b_m_o_d_u_l_e_s
           o _u_t_o_o_l_._D_y_n_a_m_i_c_S_t_r_u_c_t_ _m_o_d_u_l_e
           o _u_t_o_o_l_._P_r_e_f_e_r_e_n_c_e_s_ _m_o_d_u_l_e
           o _u_t_o_o_l_._P_r_i_n_t_a_b_l_e_ _m_o_d_u_l_e
           o _u_t_o_o_l_._____m_a_i_n_____ _m_o_d_u_l_e
-          o _u_t_o_o_l_.___v_e_r_s_i_o_n_ _m_o_d_u_l_e
           o _u_t_o_o_l_._o_l_d_a_l_g_ _m_o_d_u_l_e
           o _u_t_o_o_l_._s_a_n_d_b_o_x_ _m_o_d_u_l_e
           o _u_t_o_o_l_._u_t_i_l___a_l_g_ _m_o_d_u_l_e
           o _u_t_o_o_l_._u_t_i_l___a_l_i_a_s_e_s_ _m_o_d_u_l_e
           o _u_t_o_o_l_._u_t_i_l___a_r_g_ _m_o_d_u_l_e
           o _u_t_o_o_l_._u_t_i_l___a_s_s_e_r_t_ _m_o_d_u_l_e
           o _u_t_o_o_l_._u_t_i_l___a_u_t_o_g_e_n_ _m_o_d_u_l_e
```

### Comparing `wbia-utool-4.0.4/docs/py-modindex.html` & `wbia-utool-4.0.5/docs/py-modindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -159,19 +159,14 @@
        <td></td>
        <td>&#160;&#160;&#160;
        <a href="utool._internal.html#module-utool._internal.win32_send_keys"><code class="xref">utool._internal.win32_send_keys</code></a></td><td>
        <em></em></td></tr>
      <tr class="cg-1">
        <td></td>
        <td>&#160;&#160;&#160;
-       <a href="utool.html#module-utool._version"><code class="xref">utool._version</code></a></td><td>
-       <em></em></td></tr>
-     <tr class="cg-1">
-       <td></td>
-       <td>&#160;&#160;&#160;
        <a href="utool.html#module-utool.DynamicStruct"><code class="xref">utool.DynamicStruct</code></a></td><td>
        <em></em></td></tr>
      <tr class="cg-1">
        <td></td>
        <td>&#160;&#160;&#160;
        <a href="utool.experimental.html#module-utool.experimental"><code class="xref">utool.experimental</code></a></td><td>
        <em></em></td></tr>
```

#### html2text {}

```diff
@@ -23,15 +23,14 @@
         _u_t_o_o_l_.___i_n_t_e_r_n_a_l_._m_e_t_a___u_t_i_l___i_t_e_r
         _u_t_o_o_l_.___i_n_t_e_r_n_a_l_._m_e_t_a___u_t_i_l___p_a_t_h
         _u_t_o_o_l_.___i_n_t_e_r_n_a_l_._m_e_t_a___u_t_i_l___s_i_x
         _u_t_o_o_l_.___i_n_t_e_r_n_a_l_._p_y_2___s_y_n_t_a_x___f_u_n_c_s
         _u_t_o_o_l_.___i_n_t_e_r_n_a_l_._r_a_n_d_o_m_w_r_a_p
         _u_t_o_o_l_.___i_n_t_e_r_n_a_l_._u_t_i_l___i_m_p_o_r_t_e_r
         _u_t_o_o_l_.___i_n_t_e_r_n_a_l_._w_i_n_3_2___s_e_n_d___k_e_y_s
-        _u_t_o_o_l_.___v_e_r_s_i_o_n
         _u_t_o_o_l_._D_y_n_a_m_i_c_S_t_r_u_c_t
         _u_t_o_o_l_._e_x_p_e_r_i_m_e_n_t_a_l
         _u_t_o_o_l_._e_x_p_e_r_i_m_e_n_t_a_l_._b_y_t_e_c_o_d_e___o_p_t_i_m_i_z_a_t_i_o_n_s
         _u_t_o_o_l_._e_x_p_e_r_i_m_e_n_t_a_l_._d_y_n_a_m_i_c___c_o_n_n_e_c_t_i_v_i_t_y
         _u_t_o_o_l_._e_x_p_e_r_i_m_e_n_t_a_l_._e_u_l_e_r___t_o_u_r___t_r_e_e___a_v_l
         _u_t_o_o_l_._e_x_p_e_r_i_m_e_n_t_a_l_._p_a_n_d_a_s___h_i_g_h_l_i_g_h_t
         _u_t_o_o_l_._o_l_d_a_l_g
```

### Comparing `wbia-utool-4.0.4/docs/search.html` & `wbia-utool-4.0.5/docs/search.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/searchindex.js` & `wbia-utool-4.0.5/docs/searchindex.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -2358,15 +2358,14 @@
         ],
         utool: [
             [1, 0, 0, "-", "DynamicStruct"],
             [1, 0, 0, "-", "Preferences"],
             [1, 0, 0, "-", "Printable"],
             [1, 0, 0, "-", "__main__"],
             [2, 0, 0, "-", "_internal"],
-            [1, 0, 0, "-", "_version"],
             [3, 0, 0, "-", "experimental"],
             [1, 0, 0, "-", "oldalg"],
             [1, 3, 1, "", "reassign_submodule_attributes"],
             [1, 3, 1, "", "reload_subs"],
             [1, 3, 1, "", "rrrr"],
             [1, 0, 0, "-", "sandbox"],
             [4, 0, 0, "-", "tests"],
@@ -3108,15 +3107,15 @@
         _testgen: 1,
         _traverse_nod: 3,
         _tryorder: 1,
         _union: 1,
         _utool_flush: 1,
         _utool_print: 1,
         _utool_writ: 1,
-        _version: 0,
+        _version: [],
         _vpgwpcafbjkkpjdf: 1,
         _wrp_preserve1: 1,
         _wrp_preserve2: 1,
         a01eda32: 1,
         a0: 1,
         a1: 1,
         a2: 1,
@@ -9616,15 +9615,15 @@
     titleterms: {
         __main__: 1,
         _intern: 2,
         _oldtest_decor: 4,
         _oldtest_hash: 4,
         _oldtest_log: 4,
         _oldtest_reload: 4,
-        _version: 1,
+        _version: [],
         bytecode_optim: 3,
         content: [0, 1, 2, 3, 4],
         document: 0,
         dynamic_connect: 3,
         dynamicstruct: 1,
         euler_tour_tree_avl: 3,
         experiment: 3,
```

### Comparing `wbia-utool-4.0.4/docs/utool._internal.html` & `wbia-utool-4.0.5/docs/utool._internal.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/utool.experimental.html` & `wbia-utool-4.0.5/docs/utool.experimental.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/docs/utool.html` & `wbia-utool-4.0.5/docs/utool.html`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,14 @@
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="#submodules">Submodules</a></li>
 <li class="toctree-l2"><a class="reference internal" href="#module-utool.DynamicStruct">utool.DynamicStruct module</a></li>
 <li class="toctree-l2"><a class="reference internal" href="#module-utool.Preferences">utool.Preferences module</a></li>
 <li class="toctree-l2"><a class="reference internal" href="#module-utool.Printable">utool.Printable module</a></li>
 <li class="toctree-l2"><a class="reference internal" href="#module-utool.__main__">utool.__main__ module</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#module-utool._version">utool._version module</a></li>
 <li class="toctree-l2"><a class="reference internal" href="#module-utool.oldalg">utool.oldalg module</a></li>
 <li class="toctree-l2"><a class="reference internal" href="#module-utool.sandbox">utool.sandbox module</a></li>
 <li class="toctree-l2"><a class="reference internal" href="#module-utool.util_alg">utool.util_alg module</a></li>
 <li class="toctree-l2"><a class="reference internal" href="#module-utool.util_aliases">utool.util_aliases module</a></li>
 <li class="toctree-l2"><a class="reference internal" href="#module-utool.util_arg">utool.util_arg module</a></li>
 <li class="toctree-l2"><a class="reference internal" href="#module-utool.util_assert">utool.util_assert module</a></li>
 <li class="toctree-l2"><a class="reference internal" href="#module-utool.util_autogen">utool.util_autogen module</a></li>
@@ -534,17 +533,14 @@
 <span id="utool-main-module"></span><h2>utool.__main__ module<a class="headerlink" href="#module-utool.__main__" title="Permalink to this headline"></a></h2>
 <dl class="py function">
 <dt class="sig sig-object py" id="utool.__main__.main">
 <span class="sig-prename descclassname"><span class="pre">utool.__main__.</span></span><span class="sig-name descname"><span class="pre">main</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/utool/__main__.html#main"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#utool.__main__.main" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 </section>
-<section id="module-utool._version">
-<span id="utool-version-module"></span><h2>utool._version module<a class="headerlink" href="#module-utool._version" title="Permalink to this headline"></a></h2>
-</section>
 <section id="module-utool.oldalg">
 <span id="utool-oldalg-module"></span><h2>utool.oldalg module<a class="headerlink" href="#module-utool.oldalg" title="Permalink to this headline"></a></h2>
 <dl class="py function">
 <dt class="sig sig-object py" id="utool.oldalg.bayesnet">
 <span class="sig-prename descclassname"><span class="pre">utool.oldalg.</span></span><span class="sig-name descname"><span class="pre">bayesnet</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/utool/oldalg.html#bayesnet"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#utool.oldalg.bayesnet" title="Permalink to this definition"></a></dt>
 <dd><p class="rubric">References</p>
 <p><a class="reference external" href="https://class.coursera.org/pgm-003/lecture/17">https://class.coursera.org/pgm-003/lecture/17</a>
```

#### html2text {}

```diff
@@ -8,15 +8,14 @@
                 # _u_t_o_o_l_._e_x_p_e_r_i_m_e_n_t_a_l_ _p_a_c_k_a_g_e
                 # _u_t_o_o_l_._t_e_s_t_s_ _p_a_c_k_a_g_e
           o _S_u_b_m_o_d_u_l_e_s
           o _u_t_o_o_l_._D_y_n_a_m_i_c_S_t_r_u_c_t_ _m_o_d_u_l_e
           o _u_t_o_o_l_._P_r_e_f_e_r_e_n_c_e_s_ _m_o_d_u_l_e
           o _u_t_o_o_l_._P_r_i_n_t_a_b_l_e_ _m_o_d_u_l_e
           o _u_t_o_o_l_._____m_a_i_n_____ _m_o_d_u_l_e
-          o _u_t_o_o_l_.___v_e_r_s_i_o_n_ _m_o_d_u_l_e
           o _u_t_o_o_l_._o_l_d_a_l_g_ _m_o_d_u_l_e
           o _u_t_o_o_l_._s_a_n_d_b_o_x_ _m_o_d_u_l_e
           o _u_t_o_o_l_._u_t_i_l___a_l_g_ _m_o_d_u_l_e
           o _u_t_o_o_l_._u_t_i_l___a_l_i_a_s_e_s_ _m_o_d_u_l_e
           o _u_t_o_o_l_._u_t_i_l___a_r_g_ _m_o_d_u_l_e
           o _u_t_o_o_l_._u_t_i_l___a_s_s_e_r_t_ _m_o_d_u_l_e
           o _u_t_o_o_l_._u_t_i_l___a_u_t_o_g_e_n_ _m_o_d_u_l_e
@@ -226,15 +225,14 @@
       Tries to make a nice type string for a value. Can also pass in a
       Printable parent object
   utool.Printable.printableVal(vvaall, ttyyppee__bbiitt==TTrruuee, jjuussttlleennggtthh==FFaallssee)_[_s_o_u_r_c_e_]_
       Very old way of doing pretty printing. Need to update and refactor.
       DEPRICATE
 ********** uuttooooll..____mmaaiinn____ mmoodduullee_? **********
   utool.__main__.main()_[_s_o_u_r_c_e_]_
-********** uuttooooll..__vveerrssiioonn mmoodduullee_? **********
 ********** uuttooooll..oollddaallgg mmoodduullee_? **********
   utool.oldalg.bayesnet()_[_s_o_u_r_c_e_]_
       References
       _h_t_t_p_s_:_/_/_c_l_a_s_s_._c_o_u_r_s_e_r_a_._o_r_g_/_p_g_m_-_0_0_3_/_l_e_c_t_u_r_e_/_1_7 _h_t_t_p_:_/_/_w_w_w_._c_s_._u_b_c_._c_a_/
       _~_m_u_r_p_h_y_k_/_B_a_y_e_s_/_b_n_i_n_t_r_o_._h_t_m_l _h_t_t_p_:_/_/_w_w_w_3_._c_s_._s_t_o_n_y_b_r_o_o_k_._e_d_u_/_~_s_a_e_l_/_t_e_a_c_h_i_n_g_/
       _c_s_e_5_3_7_/_S_l_i_d_e_s_/_c_h_a_p_t_e_r_1_4_d___B_P_._p_d_f _h_t_t_p_:_/_/_w_w_w_._c_s_e_._u_n_s_w_._e_d_u_._a_u_/_~_c_s_9_4_1_7_m_l_/
       _B_a_y_e_s_/_P_a_g_e_s_/_P_e_a_r_l_P_r_o_p_a_g_a_t_i_o_n_._h_t_m_l _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_p_g_m_p_y_/_p_g_m_p_y_._g_i_t
```

### Comparing `wbia-utool-4.0.4/docs/utool.tests.html` & `wbia-utool-4.0.5/docs/utool.tests.html`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/setup.py` & `wbia-utool-4.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/DynamicStruct.py` & `wbia-utool-4.0.5/utool/DynamicStruct.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/Preferences.py` & `wbia-utool-4.0.5/utool/Preferences.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/Printable.py` & `wbia-utool-4.0.5/utool/Printable.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/__depricated_utils` & `wbia-utool-4.0.5/utool/__depricated_utils`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/__init__.py` & `wbia-utool-4.0.5/utool/__init__.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/__main__.py` & `wbia-utool-4.0.5/utool/__main__.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/_graveyard/__prefwidg_dep.py` & `wbia-utool-4.0.5/utool/_graveyard/__prefwidg_dep.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/_graveyard/broken.py` & `wbia-utool-4.0.5/utool/_graveyard/broken.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/_graveyard/util_distances.py` & `wbia-utool-4.0.5/utool/_graveyard/util_distances.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/_internal/meta_util_arg.py` & `wbia-utool-4.0.5/utool/_internal/meta_util_arg.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/_internal/meta_util_cache.py` & `wbia-utool-4.0.5/utool/_internal/meta_util_cache.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/_internal/meta_util_cplat.py` & `wbia-utool-4.0.5/utool/_internal/meta_util_cplat.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/_internal/meta_util_dbg.py` & `wbia-utool-4.0.5/utool/_internal/meta_util_dbg.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/_internal/meta_util_git.py` & `wbia-utool-4.0.5/utool/_internal/meta_util_git.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/_internal/meta_util_iter.py` & `wbia-utool-4.0.5/utool/_internal/meta_util_iter.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/_internal/meta_util_path.py` & `wbia-utool-4.0.5/utool/_internal/meta_util_path.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/_internal/meta_util_six.py` & `wbia-utool-4.0.5/utool/_internal/meta_util_six.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/_internal/py2_syntax_funcs.py` & `wbia-utool-4.0.5/utool/_internal/py2_syntax_funcs.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/_internal/randomwrap.py` & `wbia-utool-4.0.5/utool/_internal/randomwrap.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/_internal/util_importer.py` & `wbia-utool-4.0.5/utool/_internal/util_importer.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/_internal/win32_send_keys.py` & `wbia-utool-4.0.5/utool/_internal/win32_send_keys.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/experimental/bytecode_optimizations.py` & `wbia-utool-4.0.5/utool/experimental/bytecode_optimizations.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/experimental/dynamic_connectivity.py` & `wbia-utool-4.0.5/utool/experimental/dynamic_connectivity.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/experimental/euler_tour_tree_avl.py` & `wbia-utool-4.0.5/utool/experimental/euler_tour_tree_avl.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/experimental/pandas_highlight.py` & `wbia-utool-4.0.5/utool/experimental/pandas_highlight.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/experimental/tmp.py.bak` & `wbia-utool-4.0.5/utool/experimental/tmp.py.bak`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/oldalg.py` & `wbia-utool-4.0.5/utool/oldalg.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/sandbox.py` & `wbia-utool-4.0.5/utool/sandbox.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/tests/_oldtest_decor.py` & `wbia-utool-4.0.5/utool/tests/_oldtest_decor.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/tests/_oldtest_hash.py` & `wbia-utool-4.0.5/utool/tests/_oldtest_hash.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/tests/_oldtest_logging.py` & `wbia-utool-4.0.5/utool/tests/_oldtest_logging.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/tests/_oldtest_reloading.py` & `wbia-utool-4.0.5/utool/tests/_oldtest_reloading.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/tests/run_tests.py` & `wbia-utool-4.0.5/utool/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_alg.py` & `wbia-utool-4.0.5/utool/util_alg.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_arg.py` & `wbia-utool-4.0.5/utool/util_arg.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_assert.py` & `wbia-utool-4.0.5/utool/util_assert.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_autogen.py` & `wbia-utool-4.0.5/utool/util_autogen.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_cache.py` & `wbia-utool-4.0.5/utool/util_cache.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_class.py` & `wbia-utool-4.0.5/utool/util_class.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_config.py` & `wbia-utool-4.0.5/utool/util_config.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_const.py` & `wbia-utool-4.0.5/utool/util_const.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_cplat.py` & `wbia-utool-4.0.5/utool/util_cplat.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_csv.py` & `wbia-utool-4.0.5/utool/util_csv.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_dbg.py` & `wbia-utool-4.0.5/utool/util_dbg.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_decor.py` & `wbia-utool-4.0.5/utool/util_decor.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_depricated.py` & `wbia-utool-4.0.5/utool/util_depricated.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_dev.py` & `wbia-utool-4.0.5/utool/util_dev.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_dict.py` & `wbia-utool-4.0.5/utool/util_dict.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_func.py` & `wbia-utool-4.0.5/utool/util_func.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_git.py` & `wbia-utool-4.0.5/utool/util_git.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_grabdata.py` & `wbia-utool-4.0.5/utool/util_grabdata.py`

 * *Files 3% similar despite different names*

```diff
@@ -609,28 +609,28 @@
             break
     else:
         name, ext = splitext(path)
     return name, ext
 
 
 TESTIMG_URL_DICT = {
-    'grace.jpg': 'http://i.imgur.com/rgQyu7r.jpg',
-    'jeff.png': 'http://i.imgur.com/l00rECD.png',
-    'ada2.jpg': 'http://i.imgur.com/zHOpTCb.jpg',
-    'ada.jpg': 'http://i.imgur.com/iXNf4Me.jpg',
-    'lena.png': 'http://i.imgur.com/JGrqMnV.png',  # depricate lena
-    'astro.png': 'https://i.imgur.com/KXhKM72.png',  # Use instead of lena
-    'carl.jpg': 'http://i.imgur.com/flTHWFD.jpg',
-    'easy1.png': 'http://i.imgur.com/Qqd0VNq.png',
-    'easy2.png': 'http://i.imgur.com/BDP8MIu.png',
-    'easy3.png': 'http://i.imgur.com/zBcm5mS.png',
-    'hard3.png': 'http://i.imgur.com/ST91yBf.png',
-    'zebra.png': 'http://i.imgur.com/58hbGcd.png',
-    'star.png': 'http://i.imgur.com/d2FHuIU.png',
-    'patsy.jpg': 'http://i.imgur.com/C1lNRfT.jpg',
+    'grace.jpg': 'https://cthulhu.dyn.wildme.io/public/testimgs/rgQyu7r.jpg',
+    'jeff.png': 'https://cthulhu.dyn.wildme.io/public/testimgs/l00rECD.png',
+    'ada2.jpg': 'https://cthulhu.dyn.wildme.io/public/testimgs/zHOpTCb.jpg',
+    'ada.jpg': 'https://cthulhu.dyn.wildme.io/public/testimgs/iXNf4Me.jpg',
+    'lena.png': 'https://cthulhu.dyn.wildme.io/public/testimgs/JGrqMnV.png',  # depricate lena
+    'astro.png': 'https://cthulhu.dyn.wildme.io/public/testimgs/KXhKM72.png',  # Use instead of lena
+    'carl.jpg': 'https://cthulhu.dyn.wildme.io/public/testimgs/flTHWFD.jpg',
+    'easy1.png': 'https://cthulhu.dyn.wildme.io/public/testimgs/Qqd0VNq.png',
+    'easy2.png': 'https://cthulhu.dyn.wildme.io/public/testimgs/BDP8MIu.png',
+    'easy3.png': 'https://cthulhu.dyn.wildme.io/public/testimgs/zBcm5mS.png',
+    'hard3.png': 'https://cthulhu.dyn.wildme.io/public/testimgs/ST91yBf.png',
+    'zebra.png': 'https://cthulhu.dyn.wildme.io/public/testimgs/58hbGcd.png',
+    'star.png': 'https://cthulhu.dyn.wildme.io/public/testimgs/d2FHuIU.png',
+    'patsy.jpg': 'https://cthulhu.dyn.wildme.io/public/testimgs/C1lNRfT.jpg',
 }
 
 
 def get_valid_test_imgkeys():
     r"""returns valid keys for grab_test_imgpath"""
     return sorted(TESTIMG_URL_DICT.keys())
```

### Comparing `wbia-utool-4.0.4/utool/util_graph.py` & `wbia-utool-4.0.5/utool/util_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,15 @@
     CommandLine:
         python -m utool.util_graph nx_transitive_reduction --show
 
     Example:
         >>> # DISABLE_DOCTEST
         >>> from utool.util_graph import *  # NOQA
         >>> import utool as ut
+        >>> import networkx as nx
         >>> G = nx.DiGraph([('a', 'b'), ('a', 'c'), ('a', 'e'),
         >>>                 ('a', 'd'), ('b', 'd'), ('c', 'e'),
         >>>                 ('d', 'e'), ('c', 'e'), ('c', 'd')])
         >>> G = testdata_graph()[1]
         >>> G_tr = nx_transitive_reduction(G, mode=1)
         >>> G_tr2 = nx_transitive_reduction(G, mode=1)
         >>> ut.quit_if_noshow()
@@ -261,14 +262,15 @@
         pt.qt4ensure()
         pt.show_nx(graph)
 
     Example:
         >>> # ENABLE_DOCTEST
         >>> from utool.util_graph import *  # NOQA
         >>> import utool as ut
+        >>> import networkx as nx
         >>> adj_dict = {0: [5], 1: [5], 2: [1], 3: [4], 4: [0], 5: [], 6: [4], 7: [9], 8: [6], 9: [1]}
         >>> nodes = [2, 1, 5]
         >>> f_graph = ut.nx_from_adj_dict(adj_dict, nx.DiGraph)
         >>> graph = f_graph.reverse()
         >>> #ranks = ut.nx_dag_node_rank(graph, nodes)
         >>> ranks = ut.nx_dag_node_rank(graph, nodes)
         >>> result = ('ranks = %r' % (ranks,))
@@ -377,14 +379,15 @@
     CommandLine:
         python -m utool.util_graph --test-nx_edges_between
 
     Example:
         >>> # ENABLE_DOCTEST
         >>> from utool.util_graph import *  # NOQA
         >>> import utool as ut
+        >>> import networkx as nx
         >>> edges = [
         >>>     (1, 2), (2, 3), (3, 4), (4, 1), (4, 3),  # cc 1234
         >>>     (1, 5), (7, 2), (5, 1),  # cc 567 / 5678
         >>>     (7, 5), (5, 6), (8, 7),
         >>> ]
         >>> digraph = nx.DiGraph(edges)
         >>> graph = nx.Graph(edges)
@@ -570,14 +573,15 @@
 def nx_delete_node_attr(graph, name, nodes=None):
     """
     Removes node attributes
 
     Example:
         >>> from utool.util_graph import *  # NOQA
         >>> import utool as ut
+        >>> import networkx as nx
         >>> G = nx.karate_club_graph()
         >>> nx.set_node_attributes(G, name='foo', values='bar')
         >>> datas = nx.get_node_attributes(G, 'club')
         >>> assert len(nx.get_node_attributes(G, 'club')) == 34
         >>> assert len(nx.get_node_attributes(G, 'foo')) == 34
         >>> ut.nx_delete_node_attr(G, ['club', 'foo'], nodes=[1, 2])
         >>> assert len(nx.get_node_attributes(G, 'club')) == 32
@@ -614,14 +618,15 @@
 def nx_delete_edge_attr(graph, name, edges=None):
     """
     Removes an attributes from specific edges in the graph
 
     Example:
         >>> from utool.util_graph import *  # NOQA
         >>> import utool as ut
+        >>> import networkx as nx
         >>> G = nx.karate_club_graph()
         >>> nx.set_edge_attributes(G, name='spam', values='eggs')
         >>> nx.set_edge_attributes(G, name='foo', values='bar')
         >>> assert len(nx.get_edge_attributes(G, 'spam')) == 78
         >>> assert len(nx.get_edge_attributes(G, 'foo')) == 78
         >>> ut.nx_delete_edge_attr(G, ['spam', 'foo'], edges=[(1, 2)])
         >>> assert len(nx.get_edge_attributes(G, 'spam')) == 77
@@ -629,14 +634,15 @@
         >>> ut.nx_delete_edge_attr(G, ['spam'])
         >>> assert len(nx.get_edge_attributes(G, 'spam')) == 0
         >>> assert len(nx.get_edge_attributes(G, 'foo')) == 77
 
     Example:
         >>> from utool.util_graph import *  # NOQA
         >>> import utool as ut
+        >>> import networkx as nx
         >>> G = nx.MultiGraph()
         >>> G.add_edges_from([(1, 2), (2, 3), (3, 4), (4, 5), (4, 5), (1, 2)])
         >>> nx.set_edge_attributes(G, name='spam', values='eggs')
         >>> nx.set_edge_attributes(G, name='foo', values='bar')
         >>> assert len(nx.get_edge_attributes(G, 'spam')) == 6
         >>> assert len(nx.get_edge_attributes(G, 'foo')) == 6
         >>> ut.nx_delete_edge_attr(G, ['spam', 'foo'], edges=[(1, 2, 0)])
@@ -791,14 +797,15 @@
             default - returns node, but uses value specified by default
             filter - skips the node
 
     Example:
         >>> # ENABLE_DOCTEST
         >>> from utool.util_graph import *  # NOQA
         >>> import utool as ut
+        >>> import networkx as nx
         >>> G = nx.Graph([(1, 2), (2, 3)])
         >>> nx.set_node_attributes(G, name='part', values={1: 'bar', 3: 'baz'})
         >>> nodes = [1, 2, 3, 4]
         >>> #
         >>> assert len(list(ut.nx_gen_node_attrs(G, 'part', default=None, on_missing='error', on_keyerr='default'))) == 3
         >>> assert len(list(ut.nx_gen_node_attrs(G, 'part', default=None, on_missing='error', on_keyerr='filter'))) == 2
         >>> ut.assert_raises(KeyError, list, ut.nx_gen_node_attrs(G, 'part', on_missing='error', on_keyerr='error'))
@@ -812,14 +819,15 @@
         >>> ut.assert_raises(KeyError, list, ut.nx_gen_node_attrs(G, 'part', nodes, on_missing='default', on_keyerr='error'))
 
     Example:
         >>> # DISABLE_DOCTEST
         >>> # ALL CASES
         >>> from utool.util_graph import *  # NOQA
         >>> import utool as ut
+        >>> import networkx as nx
         >>> G = nx.Graph([(1, 2), (2, 3)])
         >>> nx.set_node_attributes(G, name='full', values={1: 'A', 2: 'B', 3: 'C'})
         >>> nx.set_node_attributes(G, name='part', values={1: 'bar', 3: 'baz'})
         >>> nodes = [1, 2, 3, 4]
         >>> attrs = dict(ut.nx_gen_node_attrs(G, 'full'))
         >>> input_grid = {
         >>>     'nodes': [None, (1, 2, 3, 4)],
@@ -964,14 +972,15 @@
             Can be {'error', 'default', 'filter'}.  defaults to 'default'
             if default is specified, otherwise defaults to 'error'.
 
     Example:
         >>> # ENABLE_DOCTEST
         >>> from utool.util_graph import *  # NOQA
         >>> import utool as ut
+        >>> import networkx as nx
         >>> G = nx.Graph([(1, 2), (2, 3), (3, 4)])
         >>> nx.set_edge_attributes(G, name='part', values={(1, 2): 'bar', (2, 3): 'baz'})
         >>> edges = [(1, 2), (2, 3), (3, 4), (4, 5)]
         >>> func = ut.partial(ut.nx_gen_edge_attrs, G, 'part', default=None)
         >>> #
         >>> assert len(list(func(on_missing='error', on_keyerr='default'))) == 3
         >>> assert len(list(func(on_missing='error', on_keyerr='filter'))) == 2
@@ -1182,14 +1191,15 @@
     CommandLine:
         python -m utool.util_graph --exec-testdata_graph --show
 
     Example:
         >>> # DISABLE_DOCTEST
         >>> from utool.util_graph import *  # NOQA
         >>> import utool as ut
+        >>> import networkx as nx
         >>> (graph, G) = testdata_graph()
         >>> import wbia.plottool as pt
         >>> ut.ensureqt()
         >>> pt.show_nx(G, layout='agraph')
         >>> ut.show_if_requested()
     """
     import utool as ut
@@ -1286,14 +1296,15 @@
         python -m utool.util_graph --exec-paths_to_root:0
         python -m utool.util_graph --exec-paths_to_root:1
 
     Example:
         >>> # ENABLE_DOCTEST
         >>> from utool.util_graph import *  # NOQA
         >>> import utool as ut
+        >>> import networkx as nx
         >>> child_to_parents = {
         >>>     'chip': ['dummy_annot'],
         >>>     'chipmask': ['dummy_annot'],
         >>>     'descriptor': ['keypoint'],
         >>>     'fgweight': ['keypoint', 'probchip'],
         >>>     'keypoint': ['chip'],
         >>>     'notch': ['dummy_annot'],
@@ -1590,14 +1601,15 @@
         python2 -c "import networkx as nx; print(nx.__version__)"
         python3 -c "import networkx as nx; print(nx.__version__)"
 
     Ignore:
         >>> # ENABLE_DOCTEST
         >>> from utool.util_graph import *  # NOQA
         >>> import utool as ut
+        >>> import networkx as nx
         >>> graph = nx.DiGraph([('a', 'b'), ('a', 'c'), ('a', 'e'),
         >>>                     ('a', 'd'), ('b', 'd'), ('c', 'e'),
         >>>                     ('d', 'e'), ('c', 'e'), ('c', 'd')])
         >>> new_graph = simplify_graph(graph)
         >>> result = ut.repr2(list(new_graph.edges()))
         >>> #adj_list = sorted(list(nx.generate_adjlist(new_graph)))
         >>> #result = ut.repr2(adj_list)
@@ -2131,14 +2143,15 @@
     CommandLine:
         python -m utool.util_graph approx_min_num_components
 
     Example:
         >>> # ENABLE_DOCTEST
         >>> from utool.util_graph import *  # NOQA
         >>> import utool as ut
+        >>> import networkx as nx
         >>> nodes = [1, 2, 3, 4, 5, 6, 7, 8, 9]
         >>> edges = [(1, 2), (2, 3), (3, 1),
         >>>          (4, 5), (5, 6), (6, 4),
         >>>          (7, 8), (8, 9), (9, 7),
         >>>          (1, 4), (4, 7), (7, 1),
         >>>         ]
         >>> g_pos = nx.Graph()
@@ -2279,14 +2292,15 @@
         \subseteq V, D) so that C \subseteq U.  This tree T approximates an
         optimal B-augmentation.
 
     Example:
         >>> # ENABLE_DOCTEST
         >>> from utool.util_graph import *  # NOQA
         >>> import utool as ut
+        >>> import networkx as nx
         >>> graph = nx.Graph()
         >>> if nx.__version__.startswith('1'):
         >>>     nx.add_path = nx.Graph.add_path
         >>> nx.add_path(graph, range(6))
         >>> #cost_func   = lambda e: e[0] + e[1]
         >>> cost_func   = lambda e: 1
         >>> weight_func = lambda e: (e[0]) / e[1]
```

### Comparing `wbia-utool-4.0.4/utool/util_gridsearch.py` & `wbia-utool-4.0.5/utool/util_gridsearch.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_hash.py` & `wbia-utool-4.0.5/utool/util_hash.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_import.py` & `wbia-utool-4.0.5/utool/util_import.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_inject.py` & `wbia-utool-4.0.5/utool/util_inject.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_inspect.py` & `wbia-utool-4.0.5/utool/util_inspect.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_io.py` & `wbia-utool-4.0.5/utool/util_io.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_ipynb.py` & `wbia-utool-4.0.5/utool/util_ipynb.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_iter.py` & `wbia-utool-4.0.5/utool/util_iter.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_latex.py` & `wbia-utool-4.0.5/utool/util_latex.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_list.py` & `wbia-utool-4.0.5/utool/util_list.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_logging.py` & `wbia-utool-4.0.5/utool/util_logging.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_num.py` & `wbia-utool-4.0.5/utool/util_num.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_numpy.py` & `wbia-utool-4.0.5/utool/util_numpy.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_parallel.py` & `wbia-utool-4.0.5/utool/util_parallel.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_path.py` & `wbia-utool-4.0.5/utool/util_path.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_print.py` & `wbia-utool-4.0.5/utool/util_print.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_profile.py` & `wbia-utool-4.0.5/utool/util_profile.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_progress.py` & `wbia-utool-4.0.5/utool/util_progress.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_project.py` & `wbia-utool-4.0.5/utool/util_project.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_regex.py` & `wbia-utool-4.0.5/utool/util_regex.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_resources.py` & `wbia-utool-4.0.5/utool/util_resources.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_scripts/check_jedi.py` & `wbia-utool-4.0.5/utool/util_scripts/check_jedi.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_scripts/classfuncs.py` & `wbia-utool-4.0.5/utool/util_scripts/classfuncs.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_scripts/ensure_python3_compatible.py` & `wbia-utool-4.0.5/utool/util_scripts/ensure_python3_compatible.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_scripts/grabzippedurl.py` & `wbia-utool-4.0.5/utool/util_scripts/grabzippedurl.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_scripts/local_info.py` & `wbia-utool-4.0.5/utool/util_scripts/local_info.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_scripts/makesetup.py` & `wbia-utool-4.0.5/utool/util_scripts/makesetup.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_scripts/permit_gitrepo.py` & `wbia-utool-4.0.5/utool/util_scripts/permit_gitrepo.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_scripts/pipinfo.py` & `wbia-utool-4.0.5/utool/util_scripts/pipinfo.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_scripts/pyproj_checker.py` & `wbia-utool-4.0.5/utool/util_scripts/pyproj_checker.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_scripts/utoolwc.py` & `wbia-utool-4.0.5/utool/util_scripts/utoolwc.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_scripts/utprof.sh` & `wbia-utool-4.0.5/utool/util_scripts/utprof.sh`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_set.py` & `wbia-utool-4.0.5/utool/util_set.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_setup.py` & `wbia-utool-4.0.5/utool/util_setup.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_sqlite.py` & `wbia-utool-4.0.5/utool/util_sqlite.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_str.py` & `wbia-utool-4.0.5/utool/util_str.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_sysreq.py` & `wbia-utool-4.0.5/utool/util_sysreq.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_tags.py` & `wbia-utool-4.0.5/utool/util_tags.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_tests.py` & `wbia-utool-4.0.5/utool/util_tests.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_time.py` & `wbia-utool-4.0.5/utool/util_time.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_type.py` & `wbia-utool-4.0.5/utool/util_type.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_ubuntu.py` & `wbia-utool-4.0.5/utool/util_ubuntu.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_web.py` & `wbia-utool-4.0.5/utool/util_web.py`

 * *Files identical despite different names*

### Comparing `wbia-utool-4.0.4/utool/util_win32.py` & `wbia-utool-4.0.5/utool/util_win32.py`

 * *Files identical despite different names*

