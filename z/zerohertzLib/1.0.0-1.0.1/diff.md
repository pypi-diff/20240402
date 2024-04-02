# Comparing `tmp/zerohertzLib-1.0.0.tar.gz` & `tmp/zerohertzLib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zerohertzLib-1.0.0.tar", last modified: Mon Apr  1 08:06:06 2024, max compression
+gzip compressed data, was "zerohertzLib-1.0.1.tar", last modified: Tue Apr  2 05:07:21 2024, max compression
```

## Comparing `zerohertzLib-1.0.0.tar` & `zerohertzLib-1.0.1.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:06:06.289720 zerohertzLib-1.0.0/
--rw-r--r--   0 root         (0) root         (0)     1067 2024-04-01 08:06:00.000000 zerohertzLib-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       16 2024-04-01 08:06:00.000000 zerohertzLib-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3338 2024-04-01 08:06:06.289720 zerohertzLib-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2316 2024-04-01 08:06:00.000000 zerohertzLib-1.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-01 08:06:06.289720 zerohertzLib-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2704 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:06:06.277718 zerohertzLib-1.0.0/test/
--rw-r--r--   0 root         (0) root         (0)     4501 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/test/test_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     1820 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/test/test_api.py
--rw-r--r--   0 root         (0) root         (0)     1230 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/test/test_logging.py
--rw-r--r--   0 root         (0) root         (0)      220 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/test/test_monitoring.py
--rw-r--r--   0 root         (0) root         (0)     8641 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/test/test_plot.py
--rw-r--r--   0 root         (0) root         (0)     2150 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/test/test_quant.py
--rw-r--r--   0 root         (0) root         (0)     1961 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/test/test_util.py
--rw-r--r--   0 root         (0) root         (0)    14679 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/test/test_vision.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:06:06.277718 zerohertzLib-1.0.0/zerohertzLib/
--rw-r--r--   0 root         (0) root         (0)     1794 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:06:06.277718 zerohertzLib-1.0.0/zerohertzLib/algorithm/
--rw-r--r--   0 root         (0) root         (0)     1040 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/algorithm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2626 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/algorithm/bisect.py
--rw-r--r--   0 root         (0) root         (0)     6708 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/algorithm/collections.py
--rw-r--r--   0 root         (0) root         (0)     2420 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/algorithm/fft.py
--rw-r--r--   0 root         (0) root         (0)     7065 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/algorithm/graph.py
--rw-r--r--   0 root         (0) root         (0)     1676 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/algorithm/prime.py
--rw-r--r--   0 root         (0) root         (0)     8048 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/algorithm/sort.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:06:06.277718 zerohertzLib-1.0.0/zerohertzLib/api/
--rw-r--r--   0 root         (0) root         (0)      446 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3865 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/api/discord.py
--rw-r--r--   0 root         (0) root         (0)    11096 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/api/github.py
--rw-r--r--   0 root         (0) root         (0)    30846 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/api/koreainvestment.py
--rw-r--r--   0 root         (0) root         (0)     4652 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/api/open_ai.py
--rw-r--r--   0 root         (0) root         (0)     8841 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/api/slack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:06:06.277718 zerohertzLib-1.0.0/zerohertzLib/logging/
--rw-r--r--   0 root         (0) root         (0)      359 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/logging/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4738 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/logging/handler.py
--rw-r--r--   0 root         (0) root         (0)     4794 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/logging/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:06:06.277718 zerohertzLib-1.0.0/zerohertzLib/mlops/
--rw-r--r--   0 root         (0) root         (0)      273 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/mlops/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12372 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/mlops/triton.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:06:06.277718 zerohertzLib-1.0.0/zerohertzLib/monitoring/
--rw-r--r--   0 root         (0) root         (0)      333 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/monitoring/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2829 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/monitoring/cpu.py
--rw-r--r--   0 root         (0) root         (0)     5184 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/monitoring/gpu.py
--rw-r--r--   0 root         (0) root         (0)     2678 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/monitoring/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:06:06.277718 zerohertzLib-1.0.0/zerohertzLib/plot/
--rw-r--r--   0 root         (0) root         (0)     1552 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/plot/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12219 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/plot/bar_chart.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:06:06.285719 zerohertzLib-1.0.0/zerohertzLib/plot/fonts/
--rw-r--r--   0 root         (0) root         (0)  7549348 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/plot/fonts/NotoSerifKR-Medium.otf
--rw-r--r--   0 root         (0) root         (0)   347988 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/plot/fonts/times.ttf
--rw-r--r--   0 root         (0) root         (0)     3435 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/plot/pie.py
--rw-r--r--   0 root         (0) root         (0)    11476 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/plot/plot.py
--rw-r--r--   0 root         (0) root         (0)     4046 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/plot/scatter.py
--rw-r--r--   0 root         (0) root         (0)     3292 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/plot/table.py
--rw-r--r--   0 root         (0) root         (0)     4838 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/plot/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:06:06.289720 zerohertzLib-1.0.0/zerohertzLib/quant/
--rw-r--r--   0 root         (0) root         (0)      885 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/quant/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14935 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/quant/backtest.py
--rw-r--r--   0 root         (0) root         (0)    13182 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/quant/methods.py
--rw-r--r--   0 root         (0) root         (0)    40727 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/quant/quant.py
--rw-r--r--   0 root         (0) root         (0)     3755 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/quant/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:06:06.289720 zerohertzLib-1.0.0/zerohertzLib/util/
--rw-r--r--   0 root         (0) root         (0)      458 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4527 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/util/csv.py
--rw-r--r--   0 root         (0) root         (0)    11173 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/util/data.py
--rw-r--r--   0 root         (0) root         (0)    11650 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/util/json.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:06:06.289720 zerohertzLib-1.0.0/zerohertzLib/vision/
--rw-r--r--   0 root         (0) root         (0)     1623 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/vision/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6964 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/vision/compare.py
--rw-r--r--   0 root         (0) root         (0)    12885 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/vision/convert.py
--rw-r--r--   0 root         (0) root         (0)    20047 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/vision/data.py
--rw-r--r--   0 root         (0) root         (0)    14878 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/vision/eval.py
--rw-r--r--   0 root         (0) root         (0)     4188 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/vision/gif.py
--rw-r--r--   0 root         (0) root         (0)    20881 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/vision/loader.py
--rw-r--r--   0 root         (0) root         (0)     7170 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/vision/transform.py
--rw-r--r--   0 root         (0) root         (0)     4219 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/vision/util.py
--rw-r--r--   0 root         (0) root         (0)    17510 2024-04-01 08:06:01.000000 zerohertzLib-1.0.0/zerohertzLib/vision/visual.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:06:06.277718 zerohertzLib-1.0.0/zerohertzLib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3338 2024-04-01 08:06:06.000000 zerohertzLib-1.0.0/zerohertzLib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1923 2024-04-01 08:06:06.000000 zerohertzLib-1.0.0/zerohertzLib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-01 08:06:06.000000 zerohertzLib-1.0.0/zerohertzLib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      390 2024-04-01 08:06:06.000000 zerohertzLib-1.0.0/zerohertzLib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-01 08:06:06.000000 zerohertzLib-1.0.0/zerohertzLib.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 05:07:21.929219 zerohertzLib-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)     1067 2024-04-02 05:07:16.000000 zerohertzLib-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-02 05:07:16.000000 zerohertzLib-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3338 2024-04-02 05:07:21.929219 zerohertzLib-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2316 2024-04-02 05:07:16.000000 zerohertzLib-1.0.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 05:07:21.929219 zerohertzLib-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2704 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 05:07:21.917219 zerohertzLib-1.0.1/test/
+-rw-r--r--   0 root         (0) root         (0)     4501 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/test/test_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/test/test_api.py
+-rw-r--r--   0 root         (0) root         (0)     1230 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/test/test_logging.py
+-rw-r--r--   0 root         (0) root         (0)      220 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/test/test_monitoring.py
+-rw-r--r--   0 root         (0) root         (0)     8641 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/test/test_plot.py
+-rw-r--r--   0 root         (0) root         (0)     2150 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/test/test_quant.py
+-rw-r--r--   0 root         (0) root         (0)     1961 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/test/test_util.py
+-rw-r--r--   0 root         (0) root         (0)    14679 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/test/test_vision.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 05:07:21.917219 zerohertzLib-1.0.1/zerohertzLib/
+-rw-r--r--   0 root         (0) root         (0)     1794 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 05:07:21.921219 zerohertzLib-1.0.1/zerohertzLib/algorithm/
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/algorithm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2626 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/algorithm/bisect.py
+-rw-r--r--   0 root         (0) root         (0)     6708 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/algorithm/collections.py
+-rw-r--r--   0 root         (0) root         (0)     2420 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/algorithm/fft.py
+-rw-r--r--   0 root         (0) root         (0)     7065 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/algorithm/graph.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/algorithm/prime.py
+-rw-r--r--   0 root         (0) root         (0)     8048 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/algorithm/sort.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 05:07:21.921219 zerohertzLib-1.0.1/zerohertzLib/api/
+-rw-r--r--   0 root         (0) root         (0)      446 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3865 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/api/discord.py
+-rw-r--r--   0 root         (0) root         (0)    11096 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/api/github.py
+-rw-r--r--   0 root         (0) root         (0)    30846 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/api/koreainvestment.py
+-rw-r--r--   0 root         (0) root         (0)     4652 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/api/open_ai.py
+-rw-r--r--   0 root         (0) root         (0)     8841 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/api/slack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 05:07:21.921219 zerohertzLib-1.0.1/zerohertzLib/logging/
+-rw-r--r--   0 root         (0) root         (0)      359 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/logging/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4738 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/logging/handler.py
+-rw-r--r--   0 root         (0) root         (0)     4794 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/logging/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 05:07:21.921219 zerohertzLib-1.0.1/zerohertzLib/mlops/
+-rw-r--r--   0 root         (0) root         (0)      273 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/mlops/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12372 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/mlops/triton.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 05:07:21.921219 zerohertzLib-1.0.1/zerohertzLib/monitoring/
+-rw-r--r--   0 root         (0) root         (0)      333 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/monitoring/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2829 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/monitoring/cpu.py
+-rw-r--r--   0 root         (0) root         (0)     5184 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/monitoring/gpu.py
+-rw-r--r--   0 root         (0) root         (0)     2678 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/monitoring/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 05:07:21.921219 zerohertzLib-1.0.1/zerohertzLib/plot/
+-rw-r--r--   0 root         (0) root         (0)     1552 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/plot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15381 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/plot/bar_chart.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 05:07:21.925219 zerohertzLib-1.0.1/zerohertzLib/plot/fonts/
+-rw-r--r--   0 root         (0) root         (0)  7549348 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/plot/fonts/NotoSerifKR-Medium.otf
+-rw-r--r--   0 root         (0) root         (0)   347988 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/plot/fonts/times.ttf
+-rw-r--r--   0 root         (0) root         (0)     3435 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/plot/pie.py
+-rw-r--r--   0 root         (0) root         (0)    11476 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/plot/plot.py
+-rw-r--r--   0 root         (0) root         (0)     4046 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/plot/scatter.py
+-rw-r--r--   0 root         (0) root         (0)     3292 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/plot/table.py
+-rw-r--r--   0 root         (0) root         (0)     4838 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/plot/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 05:07:21.925219 zerohertzLib-1.0.1/zerohertzLib/quant/
+-rw-r--r--   0 root         (0) root         (0)      885 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/quant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14935 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/quant/backtest.py
+-rw-r--r--   0 root         (0) root         (0)    13182 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/quant/methods.py
+-rw-r--r--   0 root         (0) root         (0)    41316 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/quant/quant.py
+-rw-r--r--   0 root         (0) root         (0)     3755 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/quant/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 05:07:21.925219 zerohertzLib-1.0.1/zerohertzLib/util/
+-rw-r--r--   0 root         (0) root         (0)      458 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4527 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/util/csv.py
+-rw-r--r--   0 root         (0) root         (0)    11173 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/util/data.py
+-rw-r--r--   0 root         (0) root         (0)    11650 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/util/json.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 05:07:21.929219 zerohertzLib-1.0.1/zerohertzLib/vision/
+-rw-r--r--   0 root         (0) root         (0)     1623 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/vision/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6964 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/vision/compare.py
+-rw-r--r--   0 root         (0) root         (0)    12885 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/vision/convert.py
+-rw-r--r--   0 root         (0) root         (0)    20047 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/vision/data.py
+-rw-r--r--   0 root         (0) root         (0)    14878 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/vision/eval.py
+-rw-r--r--   0 root         (0) root         (0)     4188 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/vision/gif.py
+-rw-r--r--   0 root         (0) root         (0)    20881 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/vision/loader.py
+-rw-r--r--   0 root         (0) root         (0)     7170 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/vision/transform.py
+-rw-r--r--   0 root         (0) root         (0)     4219 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/vision/util.py
+-rw-r--r--   0 root         (0) root         (0)    17510 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/vision/visual.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 05:07:21.917219 zerohertzLib-1.0.1/zerohertzLib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3338 2024-04-02 05:07:21.000000 zerohertzLib-1.0.1/zerohertzLib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1923 2024-04-02 05:07:21.000000 zerohertzLib-1.0.1/zerohertzLib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 05:07:21.000000 zerohertzLib-1.0.1/zerohertzLib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      390 2024-04-02 05:07:21.000000 zerohertzLib-1.0.1/zerohertzLib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-02 05:07:21.000000 zerohertzLib-1.0.1/zerohertzLib.egg-info/top_level.txt
```

### Comparing `zerohertzLib-1.0.0/LICENSE` & `zerohertzLib-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/PKG-INFO` & `zerohertzLib-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerohertzLib
-Version: 1.0.0
+Version: 1.0.1
 Summary: Zerohertz's Library
 Home-page: https://github.com/Zerohertz/zerohertzLib
 Author: Zerohertz
 Author-email: ohg3417@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zerohertzLib Version: 1.0.0 Summary: Zerohertz's
+Metadata-Version: 2.1 Name: zerohertzLib Version: 1.0.1 Summary: Zerohertz's
 Library Home-page: https://github.com/Zerohertz/zerohertzLib Author: Zerohertz
 Author-email: ohg3417@gmail.com License: MIT Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
```

### Comparing `zerohertzLib-1.0.0/README.md` & `zerohertzLib-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/setup.py` & `zerohertzLib-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/test/test_algorithm.py` & `zerohertzLib-1.0.1/test/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/test/test_api.py` & `zerohertzLib-1.0.1/test/test_api.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/test/test_logging.py` & `zerohertzLib-1.0.1/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/test/test_plot.py` & `zerohertzLib-1.0.1/test/test_plot.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/test/test_quant.py` & `zerohertzLib-1.0.1/test/test_quant.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/test/test_util.py` & `zerohertzLib-1.0.1/test/test_util.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/test/test_vision.py` & `zerohertzLib-1.0.1/test/test_vision.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/__init__.py` & `zerohertzLib-1.0.1/zerohertzLib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,8 +52,8 @@
     print("=" * 100)
     print(f"[Warning] {error}")
     print("Please Install OpenCV Dependency")
     print("--->\t$ sudo apt install python3-opencv -y\t<---")
     print("(but you can use other submodules except zerohertzLib.vision)")
     print("=" * 100)
 
-__version__ = "v1.0.0"
+__version__ = "v1.0.1"
```

### Comparing `zerohertzLib-1.0.0/zerohertzLib/algorithm/__init__.py` & `zerohertzLib-1.0.1/zerohertzLib/algorithm/__init__.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/algorithm/bisect.py` & `zerohertzLib-1.0.1/zerohertzLib/algorithm/bisect.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/algorithm/collections.py` & `zerohertzLib-1.0.1/zerohertzLib/algorithm/collections.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/algorithm/fft.py` & `zerohertzLib-1.0.1/zerohertzLib/algorithm/fft.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/algorithm/graph.py` & `zerohertzLib-1.0.1/zerohertzLib/algorithm/graph.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/algorithm/prime.py` & `zerohertzLib-1.0.1/zerohertzLib/algorithm/prime.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/algorithm/sort.py` & `zerohertzLib-1.0.1/zerohertzLib/algorithm/sort.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/api/discord.py` & `zerohertzLib-1.0.1/zerohertzLib/api/discord.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/api/github.py` & `zerohertzLib-1.0.1/zerohertzLib/api/github.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/api/koreainvestment.py` & `zerohertzLib-1.0.1/zerohertzLib/api/koreainvestment.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/api/open_ai.py` & `zerohertzLib-1.0.1/zerohertzLib/api/open_ai.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/api/slack.py` & `zerohertzLib-1.0.1/zerohertzLib/api/slack.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/logging/handler.py` & `zerohertzLib-1.0.1/zerohertzLib/logging/handler.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/logging/logger.py` & `zerohertzLib-1.0.1/zerohertzLib/logging/logger.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/mlops/triton.py` & `zerohertzLib-1.0.1/zerohertzLib/mlops/triton.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/monitoring/cpu.py` & `zerohertzLib-1.0.1/zerohertzLib/monitoring/cpu.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/monitoring/gpu.py` & `zerohertzLib-1.0.1/zerohertzLib/monitoring/gpu.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/monitoring/storage.py` & `zerohertzLib-1.0.1/zerohertzLib/monitoring/storage.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/plot/__init__.py` & `zerohertzLib-1.0.1/zerohertzLib/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/plot/bar_chart.py` & `zerohertzLib-1.0.1/zerohertzLib/plot/bar_chart.py`

 * *Files 13% similar despite different names*

```diff
@@ -37,15 +37,17 @@
     ylab: Optional[str] = None,
     xlim: Optional[List[Union[int, float]]] = None,
     ylim: Optional[List[Union[int, float]]] = None,
     title: Optional[str] = "tmp",
     colors: Optional[Union[str, List]] = None,
     figsize: Optional[Tuple[int]] = (15, 10),
     rot: Optional[int] = 0,
-    per: Optional[bool] = True,
+    dim: Optional[str] = None,
+    dimsize: Optional[float] = 10,
+    sign: Optional[int] = 1,
     dpi: Optional[int] = 300,
     save: Optional[bool] = True,
 ) -> str:
     """Dictionary로 입력받은 data를 가로 bar chart로 시각화
 
     Args:
         data (``Dict[str, Any]``): 입력 data
@@ -53,26 +55,28 @@
         ylab (``Optional[str]``): Graph에 출력될 Y축 label
         xlim (``Optional[List[Union[int, float]]]``): Graph에 출력될 X축 limit
         ylim (``Optional[List[Union[int, float]]]``): Graph에 출력될 Y축 limit
         title (``Optional[str]``): Graph에 표시될 제목 및 file 이름
         colors (``Optional[Union[str, List]]``): 각 요소의 색
         figsize (``Optional[Tuple[int]]``): Graph의 가로, 세로 길이
         rot (``Optional[int]``): X축의 눈금 회전 각도
-        per (``Optional[bool]``): 각 bar 상단에 percentage 표시 여부
+        dim (``Optional[str]``): 각 bar 상단에 표시될 값의 단위 (``%``: percentage)
+        dimsize (``Optional[float]``): 각 bar 상단에 표시될 값의 크기
+        sign (``Optional[int]``): 각 bar 상단에 표시될 값의 유효숫자
         dpi (``Optional[int]``): Graph 저장 시 DPI (Dots Per Inch)
         save (``Optional[bool]``): Graph 저장 여부
 
     Returns:
         ``str``: 저장된 graph의 절대 경로
 
     Examples:
-        >>> data = {"Terran": 27, "Zerg": 40, "Protoss": 30}
-        >>> zz.plot.barv(data, xlab="Races", ylab="Population", title="Star Craft")
+        >>> data = {"Terran": 27, "Zerg": 40, "Protoss": -30}
+        >>> zz.plot.barv(data, xlab="Races", ylab="Population", title="Star Craft", dim="")
         >>> data = {"xticks": ["Terran", "Zerg", "Protoss"], "Type A": [4, 5, 6], "Type B": [4, 3, 2], "Type C": [8, 5, 12], "Type D": [6, 3, 2]}
-        >>> zz.plot.barv(data, xlab="Races", ylab="Time [sec]", title="Star Craft")
+        >>> zz.plot.barv(data, xlab="Races", ylab="Time [sec]", title="Star Craft", dim="%", sign=2)
 
         .. image:: _static/examples/dynamic/plot.barv.png
             :align: center
             :width: 600px
     """
     colors = _color(data, colors)
     if save:
@@ -87,47 +91,83 @@
         for i, (key, value) in enumerate(data.items()):
             bars = plt.bar(
                 xticks, value, color=colors[i], zorder=2, label=key, bottom=bottom
             )
             bottom += np.array(value)
         plt.legend()
         plt.ylim([0, 1.1 * bottom.max()])
-        if per:
+        if dim is None:
+            pass
+        elif dim == "%":
             maximum = bottom.max()
             total = bottom.sum()
             for bar_, bot in zip(bars, bottom):
                 percentage = (bot / total) * 100
                 plt.text(
                     bar_.get_x() + bar_.get_width() / 2,
                     bot + maximum * 0.01,
-                    f"{percentage:.1f}%",
+                    f"{percentage:.{sign}f}%",
                     ha="center",
                     va="bottom",
+                    fontsize=dimsize,
+                )
+        else:
+            maximum = bottom.max()
+            for bar_, bot in zip(bars, bottom):
+                plt.text(
+                    bar_.get_x() + bar_.get_width() / 2,
+                    bot + maximum * 0.01,
+                    f"{bot:.{sign}f}{dim}",
+                    ha="center",
+                    va="bottom",
+                    fontsize=dimsize,
                 )
     else:
         bars = plt.bar(
             data.keys(),
             data.values(),
             color=colors,
             zorder=2,
         )
         if min(data.values()) > 0:
             plt.ylim([0, 1.1 * max(list(data.values()))])
-        if per:
+        if dim is None:
+            pass
+        elif dim == "%":
             maximum = max(list(data.values()))
             total = sum(list(data.values()))
             for bar_ in bars:
                 height = bar_.get_height()
                 percentage = (height / total) * 100
                 plt.text(
                     bar_.get_x() + bar_.get_width() / 2,
                     height + maximum * 0.01,
-                    f"{percentage:.1f}%",
+                    f"{percentage:.{sign}f}%",
                     ha="center",
                     va="bottom",
+                    fontsize=dimsize,
+                )
+        else:
+            maximum = max(list(data.values()))
+            minimum = min(list(data.values()))
+            for bar_ in bars:
+                height = position = bar_.get_height()
+                if height < 0:
+                    position -= (maximum - minimum) * 0.01
+                    va = "top"
+                else:
+                    position += (maximum - minimum) * 0.01
+                    va = "bottom"
+                plt.text(
+                    bar_.get_x() + bar_.get_width() / 2,
+                    position,
+                    f"{height:.{sign}f}{dim}",
+                    ha="center",
+                    va=va,
+                    fontsize=dimsize,
                 )
     plt.grid(zorder=0)
     if xlab:
         plt.xlabel(xlab)
     if ylab:
         plt.ylabel(ylab)
     if xlim:
@@ -147,15 +187,17 @@
     ylab: Optional[str] = None,
     xlim: Optional[List[Union[int, float]]] = None,
     ylim: Optional[List[Union[int, float]]] = None,
     title: Optional[str] = "tmp",
     colors: Optional[Union[str, List]] = None,
     figsize: Optional[Tuple[int]] = (10, 15),
     rot: Optional[int] = 0,
-    per: Optional[bool] = True,
+    dim: Optional[str] = None,
+    dimsize: Optional[float] = 10,
+    sign: Optional[int] = 1,
     dpi: Optional[int] = 300,
     save: Optional[bool] = True,
 ) -> str:
     """Dictionary로 입력받은 data를 세로 bar chart로 시각화
 
     Args:
         data (``Dict[str, Any]``): 입력 data
@@ -163,26 +205,28 @@
         ylab (``Optional[str]``): Graph에 출력될 Y축 label
         xlim (``Optional[List[Union[int, float]]]``): Graph에 출력될 X축 limit
         ylim (``Optional[List[Union[int, float]]]``): Graph에 출력될 Y축 limit
         title (``Optional[str]``): Graph에 표시될 제목 및 file 이름
         colors (``Optional[Union[str, List]]``): 각 요소의 색
         figsize (``Optional[Tuple[int]]``): Graph의 가로, 세로 길이
         rot (``Optional[int]``): X축의 눈금 회전 각도
-        per (``Optional[bool]``): 각 bar 상단에 percentage 표시 여부
+        dim (``Optional[str]``): 각 bar 상단에 표시될 값의 단위 (``%``: percentage)
+        dimsize (``Optional[float]``): 각 bar 상단에 표시될 값의 크기
+        sign (``Optional[int]``): 각 bar 상단에 표시될 값의 유효숫자
         dpi (``Optional[int]``): Graph 저장 시 DPI (Dots Per Inch)
         save (``Optional[bool]``): Graph 저장 여부
 
     Returns:
         ``str``: 저장된 graph의 절대 경로
 
     Examples:
-        >>> data = {"Terran": 27, "Zerg": 40, "Protoss": 30}
-        >>> zz.plot.barh(data, xlab="Population", ylab="Races", title="Star Craft")
+        >>> data = {"Terran": 27, "Zerg": 40, "Protoss": -30}
+        >>> zz.plot.barh(data, xlab="Population", ylab="Races", title="Star Craft", dim="")
         >>> data = {"yticks": ["Terran", "Zerg", "Protoss"], "Type A": [4, 5, 6], "Type B": [4, 3, 2], "Type C": [8, 5, 12], "Type D": [6, 3, 2]}
-        >>> zz.plot.barh(data, xlab="Time [Sec]", ylab="Races", title="Star Craft")
+        >>> zz.plot.barh(data, xlab="Time [Sec]", ylab="Races", title="Star Craft", dim="%", sign=2)
 
         .. image:: _static/examples/dynamic/plot.barh.png
             :align: center
             :width: 450px
     """
     colors = _color(data, colors)
     if save:
@@ -197,44 +241,82 @@
         for i, (key, value) in enumerate(data.items()):
             bars = plt.barh(
                 yticks, value, color=colors[i], zorder=2, label=key, left=left
             )
             left += np.array(value)
         plt.legend()
         plt.xlim([0, 1.1 * left.max()])
-        if per:
+        if dim is None:
+            pass
+        elif dim == "%":
             maximum = left.max()
             total = left.sum()
             for bar_, left_ in zip(bars, left):
                 percentage = (left_ / total) * 100
                 plt.text(
                     left_ + maximum * 0.01,
                     bar_.get_y() + bar_.get_height() / 2,
-                    f"{percentage:.1f}%",
+                    f"{percentage:.{sign}f}%",
+                    ha="left",
+                    va="center",
+                    rotation=270,
+                    fontsize=dimsize,
+                )
+        else:
+            maximum = left.max()
+            for bar_, left_ in zip(bars, left):
+                plt.text(
+                    left_ + maximum * 0.01,
+                    bar_.get_y() + bar_.get_height() / 2,
+                    f"{left_:.{sign}f}{dim}",
                     ha="left",
                     va="center",
                     rotation=270,
+                    fontsize=dimsize,
                 )
     else:
         bars = plt.barh(list(data.keys()), list(data.values()), color=colors, zorder=2)
         if min(data.values()) > 0:
             plt.xlim([0, 1.1 * max(list(data.values()))])
-        if per:
+        if dim is None:
+            pass
+        elif dim == "%":
             maximum = max(list(data.values()))
             total = sum(list(data.values()))
             for bar_ in bars:
                 width = bar_.get_width()
                 percentage = (width / total) * 100
                 plt.text(
                     width + maximum * 0.01,
                     bar_.get_y() + bar_.get_height() / 2,
-                    f"{percentage:.1f}%",
+                    f"{percentage:.{sign}f}%",
                     ha="left",
                     va="center",
                     rotation=270,
+                    fontsize=dimsize,
+                )
+        else:
+            maximum = max(list(data.values()))
+            minimum = min(list(data.values()))
+            for bar_ in bars:
+                width = position = bar_.get_width()
+                if width < 0:
+                    position -= (maximum - minimum) * 0.01
+                    ha = "right"
+                else:
+                    position += (maximum - minimum) * 0.01
+                    ha = "left"
+                plt.text(
+                    position,
+                    bar_.get_y() + bar_.get_height() / 2,
+                    f"{width:.{sign}f}{dim}",
+                    ha=ha,
+                    va="center",
+                    rotation=270,
+                    fontsize=dimsize,
                 )
     plt.grid(zorder=0)
     if xlab:
         plt.xlabel(xlab)
     if ylab:
         plt.ylabel(ylab)
     if xlim:
```

### Comparing `zerohertzLib-1.0.0/zerohertzLib/plot/fonts/NotoSerifKR-Medium.otf` & `zerohertzLib-1.0.1/zerohertzLib/plot/fonts/NotoSerifKR-Medium.otf`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/plot/fonts/times.ttf` & `zerohertzLib-1.0.1/zerohertzLib/plot/fonts/times.ttf`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/plot/pie.py` & `zerohertzLib-1.0.1/zerohertzLib/plot/pie.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/plot/plot.py` & `zerohertzLib-1.0.1/zerohertzLib/plot/plot.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/plot/scatter.py` & `zerohertzLib-1.0.1/zerohertzLib/plot/scatter.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/plot/table.py` & `zerohertzLib-1.0.1/zerohertzLib/plot/table.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/plot/util.py` & `zerohertzLib-1.0.1/zerohertzLib/plot/util.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/quant/__init__.py` & `zerohertzLib-1.0.1/zerohertzLib/quant/__init__.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/quant/backtest.py` & `zerohertzLib-1.0.1/zerohertzLib/quant/backtest.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/quant/methods.py` & `zerohertzLib-1.0.1/zerohertzLib/quant/methods.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/quant/quant.py` & `zerohertzLib-1.0.1/zerohertzLib/quant/quant.py`

 * *Files 1% similar despite different names*

```diff
@@ -336,19 +336,28 @@
                         stock["pdno"],  # 종목번호
                         float(stock["avg_unpr3"]),  # 평균단가
                         float(stock["ovrs_now_pric1"]),  # 해외현재가격
                         int(float(stock["ccld_qty_smtl1"])),  # 해외잔고수량
                         float(stock["evlu_pfls_rt1"]),  # 평가손익율
                         float(stock["evlu_pfls_amt2"]),  # 평가손익금액
                     ]
+            # self.balance["cash"] = (
+            #     int(response["output3"]["tot_asst_amt"])  # 총자산금액
+            #     - int(response["output3"]["ustl_sll_amt_smtl"])  # 미결제매도금액합계
+            #     - int(response["output3"]["ustl_buy_amt_smtl"])  # 미결제매수금액합계
+            # ) / self._exchange()
             self.balance["cash"] = (
-                int(response["output3"]["tot_asst_amt"])  # 총자산금액
-                - int(response["output3"]["ustl_sll_amt_smtl"])  # 미결제매도금액합계
-                - int(response["output3"]["ustl_buy_amt_smtl"])  # 미결제매수금액합계
+                float(response["output3"]["evlu_amt_smtl_amt"])  # 평가금액합계금액
+                + float(response["output3"]["frcr_use_psbl_amt"])  # 외화사용가능금액
             ) / self._exchange()
+            # self.balance["cash"] = (
+            #     float(response["output3"]["evlu_amt_smtl"])  # 평가금액합계
+            #     + float(response["output3"]["frcr_use_psbl_amt"])  # 외화사용가능금액
+            #     / self._exchange()
+            # )
         self.balance["stock"] = dict(
             sorted(
                 self.balance["stock"].items(),
                 key=lambda item: item[1][1] * item[1][3],
                 reverse=True,
             )
         )
@@ -769,14 +778,15 @@
         response = self.message("> :memo: Parameter Analysis")
         thread_ts = response.json()["ts"]
         figure((30, 20))
         plt.subplot(2, 2, 1)
         barv(
             dict(sorted(self.miu_cnt.items())),
             title=f"Methods in Use (Avg: {sum(self.miu_cnt.values()) / self.quant_cnt:.2f})",
+            dim="%",
             save=False,
         )
         plt.subplot(2, 2, 2)
         hist(
             {"": self.total_cnt},
             title=f"Distribution of Methods in Use (Avg: {sum(self.total_cnt) / self.quant_cnt:.2f})",
             cnt=max(self.total_cnt) * 2,
@@ -785,14 +795,15 @@
         )
         plt.subplot(2, 2, 3)
         barv(
             dict(
                 ((key, sum(value)) for key, value in sorted(self.methods_cnt.items()))
             ),
             title="Available Methods",
+            dim="%",
             save=False,
         )
         plt.subplot(2, 2, 4)
         hist(
             dict(sorted(self.methods_cnt.items())),
             title="Distribution of Available Methods",
             cnt=self.top * 2,
@@ -803,15 +814,15 @@
         self.file(path, thread_ts)
         for method, cnt in self.exps_cnt.items():
             figure((18, 8))
             stg = True
             for idx, count in enumerate(cnt):
                 try:
                     plt.subplot(1, len(cnt), idx + 1)
-                    barh(count, title="", save=False)
+                    barh(count, title="", dim="%", save=False)
                 except IndexError:
                     stg = False
                     print(f"'{method}' was not available: {count}")
                     break
             if stg:
                 path = savefig(method, dpi=100)
                 self.file(path, thread_ts)
```

### Comparing `zerohertzLib-1.0.0/zerohertzLib/quant/util.py` & `zerohertzLib-1.0.1/zerohertzLib/quant/util.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/util/csv.py` & `zerohertzLib-1.0.1/zerohertzLib/util/csv.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/util/data.py` & `zerohertzLib-1.0.1/zerohertzLib/util/data.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/util/json.py` & `zerohertzLib-1.0.1/zerohertzLib/util/json.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/vision/__init__.py` & `zerohertzLib-1.0.1/zerohertzLib/vision/__init__.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/vision/compare.py` & `zerohertzLib-1.0.1/zerohertzLib/vision/compare.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/vision/convert.py` & `zerohertzLib-1.0.1/zerohertzLib/vision/convert.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/vision/data.py` & `zerohertzLib-1.0.1/zerohertzLib/vision/data.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/vision/eval.py` & `zerohertzLib-1.0.1/zerohertzLib/vision/eval.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/vision/gif.py` & `zerohertzLib-1.0.1/zerohertzLib/vision/gif.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/vision/loader.py` & `zerohertzLib-1.0.1/zerohertzLib/vision/loader.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/vision/transform.py` & `zerohertzLib-1.0.1/zerohertzLib/vision/transform.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/vision/util.py` & `zerohertzLib-1.0.1/zerohertzLib/vision/util.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib/vision/visual.py` & `zerohertzLib-1.0.1/zerohertzLib/vision/visual.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.0/zerohertzLib.egg-info/PKG-INFO` & `zerohertzLib-1.0.1/zerohertzLib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerohertzLib
-Version: 1.0.0
+Version: 1.0.1
 Summary: Zerohertz's Library
 Home-page: https://github.com/Zerohertz/zerohertzLib
 Author: Zerohertz
 Author-email: ohg3417@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zerohertzLib Version: 1.0.0 Summary: Zerohertz's
+Metadata-Version: 2.1 Name: zerohertzLib Version: 1.0.1 Summary: Zerohertz's
 Library Home-page: https://github.com/Zerohertz/zerohertzLib Author: Zerohertz
 Author-email: ohg3417@gmail.com License: MIT Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
```

### Comparing `zerohertzLib-1.0.0/zerohertzLib.egg-info/SOURCES.txt` & `zerohertzLib-1.0.1/zerohertzLib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

