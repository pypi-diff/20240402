# Comparing `tmp/bencheval-1.3.1.tar.gz` & `tmp/bencheval-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bencheval-1.3.1.tar", last modified: Tue Mar 19 15:07:03 2024, max compression
+gzip compressed data, was "bencheval-1.3.2.tar", last modified: Tue Apr  2 13:58:06 2024, max compression
```

## Comparing `bencheval-1.3.1.tar` & `bencheval-1.3.2.tar`

### file list

```diff
@@ -1,95 +1,97 @@
-drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-03-19 15:07:03.709715 bencheval-1.3.1/
--rw-r--r--   0 gzhang    (3204)     1040     1068 2024-03-18 09:00:38.000000 bencheval-1.3.1/LICENSE.txt
--rw-r--r--   0 gzhang    (3204)     1040       52 2024-03-18 09:00:38.000000 bencheval-1.3.1/MANIFEST.in
--rw-r--r--   0 gzhang    (3204)     1040     3315 2024-03-19 15:07:03.709436 bencheval-1.3.1/PKG-INFO
--rw-r--r--   0 gzhang    (3204)     1040     2282 2024-03-18 09:00:38.000000 bencheval-1.3.1/README.md
-drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-03-19 15:07:03.682682 bencheval-1.3.1/bencheval/
--rw-r--r--   0 gzhang    (3204)     1040        0 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/__init__.py
-drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-03-19 15:07:03.683789 bencheval-1.3.1/bencheval/data/
--rw-r--r--   0 gzhang    (3204)     1040     4171 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/__init__.py
-drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-03-19 15:07:03.686543 bencheval-1.3.1/bencheval/data/bbh/
--rw-r--r--   0 gzhang    (3204)     1040      208 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/bbh/__init__.py
--rw-r--r--   0 gzhang    (3204)     1040      636 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/bbh/cols.txt
--rw-r--r--   0 gzhang    (3204)     1040      542 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/bbh/format.py
--rw-r--r--   0 gzhang    (3204)     1040    18964 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/bbh/leaderboard.tsv
--rw-r--r--   0 gzhang    (3204)     1040     1021 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/bbh/statistic.py
--rw-r--r--   0 gzhang    (3204)     1040    18436 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/bbh/vanilla.tsv
-drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-03-19 15:07:03.688102 bencheval-1.3.1/bencheval/data/bigcode/
--rw-r--r--   0 gzhang    (3204)     1040      338 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/bigcode/__init__.py
--rw-r--r--   0 gzhang    (3204)     1040      430 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/bigcode/format.py
--rw-r--r--   0 gzhang    (3204)     1040     2169 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/bigcode/leaderboard.tsv
--rw-r--r--   0 gzhang    (3204)     1040     2226 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/bigcode/vanilla.txt
-drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-03-19 15:07:03.688359 bencheval-1.3.1/bencheval/data/dummy/
--rw-r--r--   0 gzhang    (3204)     1040     1404 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/dummy/__init__.py
-drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-03-19 15:07:03.689000 bencheval-1.3.1/bencheval/data/glue/
--rw-r--r--   0 gzhang    (3204)     1040     1077 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/glue/__init__.py
--rw-r--r--   0 gzhang    (3204)     1040     9876 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/glue/leaderboard.tsv
-drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-03-19 15:07:03.693534 bencheval-1.3.1/bencheval/data/heim/
--rw-r--r--   0 gzhang    (3204)     1040      767 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/heim/__init__.py
--rw-r--r--   0 gzhang    (3204)     1040    13934 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/heim/aesthetics_auto.tsv
--rw-r--r--   0 gzhang    (3204)     1040     5206 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/heim/aesthetics_human.tsv
--rw-r--r--   0 gzhang    (3204)     1040    10394 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/heim/alignment_auto.tsv
--rw-r--r--   0 gzhang    (3204)     1040     5830 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/heim/alignment_human.tsv
--rw-r--r--   0 gzhang    (3204)     1040     3765 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/heim/black_out.tsv
--rw-r--r--   0 gzhang    (3204)     1040     4494 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/heim/nsfw.tsv
--rw-r--r--   0 gzhang    (3204)     1040     4809 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/heim/nudity.tsv
--rw-r--r--   0 gzhang    (3204)     1040     3643 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/heim/originality.tsv
--rw-r--r--   0 gzhang    (3204)     1040     3343 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/heim/quality_auto.tsv
--rw-r--r--   0 gzhang    (3204)     1040     2554 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/heim/quality_human.tsv
-drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-03-19 15:07:03.697371 bencheval-1.3.1/bencheval/data/helm/
--rw-r--r--   0 gzhang    (3204)     1040      890 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/helm/__init__.py
--rw-r--r--   0 gzhang    (3204)     1040     7516 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/helm/accuracy.tsv
--rw-r--r--   0 gzhang    (3204)     1040    14741 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/helm/bias.tsv
--rw-r--r--   0 gzhang    (3204)     1040     5563 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/helm/calibration.tsv
--rw-r--r--   0 gzhang    (3204)     1040     5858 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/helm/efficiency.tsv
--rw-r--r--   0 gzhang    (3204)     1040     6993 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/helm/fairness.tsv
--rw-r--r--   0 gzhang    (3204)     1040     7035 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/helm/robustness.tsv
--rw-r--r--   0 gzhang    (3204)     1040     6495 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/helm/summarization.tsv
--rw-r--r--   0 gzhang    (3204)     1040     4663 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/helm/toxicity.tsv
-drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-03-19 15:07:03.700837 bencheval-1.3.1/bencheval/data/imagenet/
--rw-r--r--   0 gzhang    (3204)     1040     1435 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/imagenet/__init__.py
--rw-r--r--   0 gzhang    (3204)     1040     1058 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/imagenet/format.py
--rw-r--r--   0 gzhang    (3204)     1040   554910 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/imagenet/leaderboard.tsv
--rw-r--r--   0 gzhang    (3204)     1040     7562 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/imagenet/leaderboard_raw.tsv
--rw-r--r--   0 gzhang    (3204)     1040    11304 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/imagenet/run.sh
--rw-r--r--   0 gzhang    (3204)     1040     2587 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/imagenet/run_imagenet.py
--rw-r--r--   0 gzhang    (3204)     1040     8324 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/imagenet/vanilla.txt
-drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-03-19 15:07:03.702682 bencheval-1.3.1/bencheval/data/mmlu/
--rw-r--r--   0 gzhang    (3204)     1040      367 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/mmlu/__init__.py
--rw-r--r--   0 gzhang    (3204)     1040     2113 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/mmlu/format.py
--rw-r--r--   0 gzhang    (3204)     1040   101533 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/mmlu/leaderboard.tsv
--rw-r--r--   0 gzhang    (3204)     1040     5831 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/mmlu/leaderboard_raw.csv
-drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-03-19 15:07:03.704009 bencheval-1.3.1/bencheval/data/mteb/
--rw-r--r--   0 gzhang    (3204)     1040      810 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/mteb/__init__.py
--rw-r--r--   0 gzhang    (3204)     1040      430 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/mteb/format.py
--rw-r--r--   0 gzhang    (3204)     1040     7313 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/mteb/leaderboard.tsv
--rw-r--r--   0 gzhang    (3204)     1040     7199 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/mteb/vanilla.txt
-drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-03-19 15:07:03.705527 bencheval-1.3.1/bencheval/data/openllm/
--rw-r--r--   0 gzhang    (3204)     1040      456 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/openllm/__init__.py
--rw-r--r--   0 gzhang    (3204)     1040      431 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/openllm/format.py
--rw-r--r--   0 gzhang    (3204)     1040     7511 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/openllm/leaderboard.tsv
--rw-r--r--   0 gzhang    (3204)     1040      196 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/openllm/statistic.py
--rw-r--r--   0 gzhang    (3204)     1040     8119 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/openllm/vanilla.txt
-drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-03-19 15:07:03.706280 bencheval-1.3.1/bencheval/data/superglue/
--rw-r--r--   0 gzhang    (3204)     1040      958 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/superglue/__init__.py
--rw-r--r--   0 gzhang    (3204)     1040     3297 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/superglue/leaderboard.tsv
-drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-03-19 15:07:03.706822 bencheval-1.3.1/bencheval/data/vtab/
--rw-r--r--   0 gzhang    (3204)     1040      331 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/vtab/__init__.py
--rw-r--r--   0 gzhang    (3204)     1040     1970 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/data/vtab/leaderboard.tsv
-drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-03-19 15:07:03.707586 bencheval-1.3.1/bencheval/measures/
--rw-r--r--   0 gzhang    (3204)     1040     4569 2024-03-19 12:55:27.000000 bencheval-1.3.1/bencheval/measures/cardinal.py
--rw-r--r--   0 gzhang    (3204)     1040     5321 2024-03-18 09:00:38.000000 bencheval-1.3.1/bencheval/measures/ordinal.py
-drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-03-19 15:07:03.708850 bencheval-1.3.1/bencheval/utils/
--rw-r--r--   0 gzhang    (3204)     1040        0 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/utils/__init__.py
--rw-r--r--   0 gzhang    (3204)     1040     1458 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/utils/base.py
--rw-r--r--   0 gzhang    (3204)     1040     4158 2024-03-19 15:00:57.000000 bencheval-1.3.1/bencheval/utils/metric.py
--rw-r--r--   0 gzhang    (3204)     1040     1358 2024-03-16 13:21:55.000000 bencheval-1.3.1/bencheval/utils/win_rate.py
-drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-03-19 15:07:03.709149 bencheval-1.3.1/bencheval.egg-info/
--rw-r--r--   0 gzhang    (3204)     1040     3315 2024-03-19 15:07:03.000000 bencheval-1.3.1/bencheval.egg-info/PKG-INFO
--rw-r--r--   0 gzhang    (3204)     1040     2428 2024-03-19 15:07:03.000000 bencheval-1.3.1/bencheval.egg-info/SOURCES.txt
--rw-r--r--   0 gzhang    (3204)     1040        1 2024-03-19 15:07:03.000000 bencheval-1.3.1/bencheval.egg-info/dependency_links.txt
--rw-r--r--   0 gzhang    (3204)     1040       62 2024-03-19 15:07:03.000000 bencheval-1.3.1/bencheval.egg-info/requires.txt
--rw-r--r--   0 gzhang    (3204)     1040       10 2024-03-19 15:07:03.000000 bencheval-1.3.1/bencheval.egg-info/top_level.txt
--rw-r--r--   0 gzhang    (3204)     1040     1176 2024-03-19 14:03:56.000000 bencheval-1.3.1/pyproject.toml
--rw-r--r--   0 gzhang    (3204)     1040      129 2024-03-16 13:21:55.000000 bencheval-1.3.1/requirements.txt
--rw-r--r--   0 gzhang    (3204)     1040       38 2024-03-19 15:07:03.709774 bencheval-1.3.1/setup.cfg
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.409004 bencheval-1.3.2/
+-rw-r--r--   0 gzhang    (3204)     1040     1068 2024-03-18 09:00:38.000000 bencheval-1.3.2/LICENSE.txt
+-rw-r--r--   0 gzhang    (3204)     1040       52 2024-03-18 09:00:38.000000 bencheval-1.3.2/MANIFEST.in
+-rw-r--r--   0 gzhang    (3204)     1040     3315 2024-04-02 13:58:06.408818 bencheval-1.3.2/PKG-INFO
+-rw-r--r--   0 gzhang    (3204)     1040     2282 2024-03-18 09:00:38.000000 bencheval-1.3.2/README.md
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.396232 bencheval-1.3.2/bencheval/
+-rw-r--r--   0 gzhang    (3204)     1040        0 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/__init__.py
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.396932 bencheval-1.3.2/bencheval/data/
+-rw-r--r--   0 gzhang    (3204)     1040     4171 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/__init__.py
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.397188 bencheval-1.3.2/bencheval/data/__pycache__/
+-rw-r--r--   0 gzhang    (3204)     1040     5711 2024-03-27 13:57:41.000000 bencheval-1.3.2/bencheval/data/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.398193 bencheval-1.3.2/bencheval/data/bbh/
+-rw-r--r--   0 gzhang    (3204)     1040      208 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/bbh/__init__.py
+-rw-r--r--   0 gzhang    (3204)     1040      636 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/bbh/cols.txt
+-rw-r--r--   0 gzhang    (3204)     1040      542 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/bbh/format.py
+-rw-r--r--   0 gzhang    (3204)     1040    18964 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/bbh/leaderboard.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     1021 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/bbh/statistic.py
+-rw-r--r--   0 gzhang    (3204)     1040    18436 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/bbh/vanilla.tsv
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.398764 bencheval-1.3.2/bencheval/data/bigcode/
+-rw-r--r--   0 gzhang    (3204)     1040      338 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/bigcode/__init__.py
+-rw-r--r--   0 gzhang    (3204)     1040      430 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/bigcode/format.py
+-rw-r--r--   0 gzhang    (3204)     1040     2169 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/bigcode/leaderboard.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     2226 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/bigcode/vanilla.txt
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.398895 bencheval-1.3.2/bencheval/data/dummy/
+-rw-r--r--   0 gzhang    (3204)     1040     1404 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/dummy/__init__.py
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.399303 bencheval-1.3.2/bencheval/data/glue/
+-rw-r--r--   0 gzhang    (3204)     1040     1077 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/glue/__init__.py
+-rw-r--r--   0 gzhang    (3204)     1040     9876 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/glue/leaderboard.tsv
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.401373 bencheval-1.3.2/bencheval/data/heim/
+-rw-r--r--   0 gzhang    (3204)     1040      767 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/heim/__init__.py
+-rw-r--r--   0 gzhang    (3204)     1040    13934 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/heim/aesthetics_auto.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     5206 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/heim/aesthetics_human.tsv
+-rw-r--r--   0 gzhang    (3204)     1040    10394 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/heim/alignment_auto.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     5830 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/heim/alignment_human.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     3765 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/heim/black_out.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     4494 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/heim/nsfw.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     4809 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/heim/nudity.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     3643 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/heim/originality.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     3343 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/heim/quality_auto.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     2554 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/heim/quality_human.tsv
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.403214 bencheval-1.3.2/bencheval/data/helm/
+-rw-r--r--   0 gzhang    (3204)     1040      890 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/helm/__init__.py
+-rw-r--r--   0 gzhang    (3204)     1040     7516 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/helm/accuracy.tsv
+-rw-r--r--   0 gzhang    (3204)     1040    14741 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/helm/bias.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     5563 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/helm/calibration.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     5858 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/helm/efficiency.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     6993 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/helm/fairness.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     7035 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/helm/robustness.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     6495 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/helm/summarization.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     4663 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/helm/toxicity.tsv
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.404636 bencheval-1.3.2/bencheval/data/imagenet/
+-rw-r--r--   0 gzhang    (3204)     1040     1435 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/imagenet/__init__.py
+-rw-r--r--   0 gzhang    (3204)     1040     1058 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/imagenet/format.py
+-rw-r--r--   0 gzhang    (3204)     1040   554910 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/imagenet/leaderboard.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     7562 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/imagenet/leaderboard_raw.tsv
+-rw-r--r--   0 gzhang    (3204)     1040    11304 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/imagenet/run.sh
+-rw-r--r--   0 gzhang    (3204)     1040     2587 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/imagenet/run_imagenet.py
+-rw-r--r--   0 gzhang    (3204)     1040     8324 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/imagenet/vanilla.txt
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.405220 bencheval-1.3.2/bencheval/data/mmlu/
+-rw-r--r--   0 gzhang    (3204)     1040      367 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/mmlu/__init__.py
+-rw-r--r--   0 gzhang    (3204)     1040     2113 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/mmlu/format.py
+-rw-r--r--   0 gzhang    (3204)     1040   101533 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/mmlu/leaderboard.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     5831 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/mmlu/leaderboard_raw.csv
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.405966 bencheval-1.3.2/bencheval/data/mteb/
+-rw-r--r--   0 gzhang    (3204)     1040      810 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/mteb/__init__.py
+-rw-r--r--   0 gzhang    (3204)     1040      430 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/mteb/format.py
+-rw-r--r--   0 gzhang    (3204)     1040     7313 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/mteb/leaderboard.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     7199 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/mteb/vanilla.txt
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.406839 bencheval-1.3.2/bencheval/data/openllm/
+-rw-r--r--   0 gzhang    (3204)     1040      456 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/openllm/__init__.py
+-rw-r--r--   0 gzhang    (3204)     1040      431 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/openllm/format.py
+-rw-r--r--   0 gzhang    (3204)     1040     7511 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/openllm/leaderboard.tsv
+-rw-r--r--   0 gzhang    (3204)     1040      196 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/openllm/statistic.py
+-rw-r--r--   0 gzhang    (3204)     1040     8119 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/openllm/vanilla.txt
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.407196 bencheval-1.3.2/bencheval/data/superglue/
+-rw-r--r--   0 gzhang    (3204)     1040      958 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/superglue/__init__.py
+-rw-r--r--   0 gzhang    (3204)     1040     3297 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/superglue/leaderboard.tsv
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.407429 bencheval-1.3.2/bencheval/data/vtab/
+-rw-r--r--   0 gzhang    (3204)     1040      331 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/vtab/__init__.py
+-rw-r--r--   0 gzhang    (3204)     1040     1970 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/vtab/leaderboard.tsv
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.407779 bencheval-1.3.2/bencheval/measures/
+-rw-r--r--   0 gzhang    (3204)     1040     4697 2024-04-02 13:14:28.000000 bencheval-1.3.2/bencheval/measures/cardinal.py
+-rw-r--r--   0 gzhang    (3204)     1040     5334 2024-04-02 11:52:38.000000 bencheval-1.3.2/bencheval/measures/ordinal.py
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.408467 bencheval-1.3.2/bencheval/utils/
+-rw-r--r--   0 gzhang    (3204)     1040        0 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/utils/__init__.py
+-rw-r--r--   0 gzhang    (3204)     1040     2077 2024-04-02 11:55:56.000000 bencheval-1.3.2/bencheval/utils/base.py
+-rw-r--r--   0 gzhang    (3204)     1040     4158 2024-03-19 15:00:57.000000 bencheval-1.3.2/bencheval/utils/metric.py
+-rw-r--r--   0 gzhang    (3204)     1040     1358 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/utils/win_rate.py
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.408619 bencheval-1.3.2/bencheval.egg-info/
+-rw-r--r--   0 gzhang    (3204)     1040     3315 2024-04-02 13:58:06.000000 bencheval-1.3.2/bencheval.egg-info/PKG-INFO
+-rw-r--r--   0 gzhang    (3204)     1040     2480 2024-04-02 13:58:06.000000 bencheval-1.3.2/bencheval.egg-info/SOURCES.txt
+-rw-r--r--   0 gzhang    (3204)     1040        1 2024-04-02 13:58:06.000000 bencheval-1.3.2/bencheval.egg-info/dependency_links.txt
+-rw-r--r--   0 gzhang    (3204)     1040       62 2024-04-02 13:58:06.000000 bencheval-1.3.2/bencheval.egg-info/requires.txt
+-rw-r--r--   0 gzhang    (3204)     1040       10 2024-04-02 13:58:06.000000 bencheval-1.3.2/bencheval.egg-info/top_level.txt
+-rw-r--r--   0 gzhang    (3204)     1040     1176 2024-04-02 08:41:37.000000 bencheval-1.3.2/pyproject.toml
+-rw-r--r--   0 gzhang    (3204)     1040      129 2024-03-16 13:21:55.000000 bencheval-1.3.2/requirements.txt
+-rw-r--r--   0 gzhang    (3204)     1040       38 2024-04-02 13:58:06.409040 bencheval-1.3.2/setup.cfg
```

### Comparing `bencheval-1.3.1/LICENSE.txt` & `bencheval-1.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/PKG-INFO` & `bencheval-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bencheval
-Version: 1.3.1
+Version: 1.3.2
 Summary: Tools for measuring sensitivity and diversity of multi-task benchmarks.
 Author: Guanhua Zhang
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `bencheval-1.3.1/README.md` & `bencheval-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/__init__.py` & `bencheval-1.3.2/bencheval/data/__init__.py`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/bbh/cols.txt` & `bencheval-1.3.2/bencheval/data/bbh/cols.txt`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/bbh/format.py` & `bencheval-1.3.2/bencheval/data/bbh/format.py`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/bbh/leaderboard.tsv` & `bencheval-1.3.2/bencheval/data/bbh/leaderboard.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/bbh/statistic.py` & `bencheval-1.3.2/bencheval/data/bbh/statistic.py`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/bbh/vanilla.tsv` & `bencheval-1.3.2/bencheval/data/bbh/vanilla.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/bigcode/leaderboard.tsv` & `bencheval-1.3.2/bencheval/data/bigcode/leaderboard.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/bigcode/vanilla.txt` & `bencheval-1.3.2/bencheval/data/bigcode/vanilla.txt`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/dummy/__init__.py` & `bencheval-1.3.2/bencheval/data/dummy/__init__.py`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/glue/__init__.py` & `bencheval-1.3.2/bencheval/data/glue/__init__.py`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/glue/leaderboard.tsv` & `bencheval-1.3.2/bencheval/data/glue/leaderboard.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/heim/__init__.py` & `bencheval-1.3.2/bencheval/data/heim/__init__.py`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/heim/aesthetics_auto.tsv` & `bencheval-1.3.2/bencheval/data/heim/aesthetics_auto.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/heim/aesthetics_human.tsv` & `bencheval-1.3.2/bencheval/data/heim/aesthetics_human.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/heim/alignment_auto.tsv` & `bencheval-1.3.2/bencheval/data/heim/alignment_auto.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/heim/alignment_human.tsv` & `bencheval-1.3.2/bencheval/data/heim/alignment_human.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/heim/black_out.tsv` & `bencheval-1.3.2/bencheval/data/heim/black_out.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/heim/nsfw.tsv` & `bencheval-1.3.2/bencheval/data/heim/nsfw.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/heim/nudity.tsv` & `bencheval-1.3.2/bencheval/data/heim/nudity.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/heim/originality.tsv` & `bencheval-1.3.2/bencheval/data/heim/originality.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/heim/quality_auto.tsv` & `bencheval-1.3.2/bencheval/data/heim/quality_auto.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/heim/quality_human.tsv` & `bencheval-1.3.2/bencheval/data/heim/quality_human.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/helm/__init__.py` & `bencheval-1.3.2/bencheval/data/helm/__init__.py`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/helm/accuracy.tsv` & `bencheval-1.3.2/bencheval/data/helm/accuracy.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/helm/bias.tsv` & `bencheval-1.3.2/bencheval/data/helm/bias.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/helm/calibration.tsv` & `bencheval-1.3.2/bencheval/data/helm/calibration.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/helm/efficiency.tsv` & `bencheval-1.3.2/bencheval/data/helm/efficiency.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/helm/fairness.tsv` & `bencheval-1.3.2/bencheval/data/helm/fairness.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/helm/robustness.tsv` & `bencheval-1.3.2/bencheval/data/helm/robustness.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/helm/summarization.tsv` & `bencheval-1.3.2/bencheval/data/helm/summarization.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/helm/toxicity.tsv` & `bencheval-1.3.2/bencheval/data/helm/toxicity.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/imagenet/__init__.py` & `bencheval-1.3.2/bencheval/data/imagenet/__init__.py`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/imagenet/format.py` & `bencheval-1.3.2/bencheval/data/imagenet/format.py`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/imagenet/leaderboard.tsv` & `bencheval-1.3.2/bencheval/data/imagenet/leaderboard.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/imagenet/leaderboard_raw.tsv` & `bencheval-1.3.2/bencheval/data/imagenet/leaderboard_raw.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/imagenet/run.sh` & `bencheval-1.3.2/bencheval/data/imagenet/run.sh`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/imagenet/run_imagenet.py` & `bencheval-1.3.2/bencheval/data/imagenet/run_imagenet.py`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/imagenet/vanilla.txt` & `bencheval-1.3.2/bencheval/data/imagenet/vanilla.txt`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/mmlu/format.py` & `bencheval-1.3.2/bencheval/data/mmlu/format.py`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/mmlu/leaderboard.tsv` & `bencheval-1.3.2/bencheval/data/mmlu/leaderboard.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/mmlu/leaderboard_raw.csv` & `bencheval-1.3.2/bencheval/data/mmlu/leaderboard_raw.csv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/mteb/__init__.py` & `bencheval-1.3.2/bencheval/data/mteb/__init__.py`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/mteb/leaderboard.tsv` & `bencheval-1.3.2/bencheval/data/mteb/leaderboard.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/mteb/vanilla.txt` & `bencheval-1.3.2/bencheval/data/mteb/vanilla.txt`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/openllm/leaderboard.tsv` & `bencheval-1.3.2/bencheval/data/openllm/leaderboard.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/openllm/vanilla.txt` & `bencheval-1.3.2/bencheval/data/openllm/vanilla.txt`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/superglue/__init__.py` & `bencheval-1.3.2/bencheval/data/superglue/__init__.py`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/superglue/leaderboard.tsv` & `bencheval-1.3.2/bencheval/data/superglue/leaderboard.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/data/vtab/leaderboard.tsv` & `bencheval-1.3.2/bencheval/data/vtab/leaderboard.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/measures/cardinal.py` & `bencheval-1.3.2/bencheval/measures/cardinal.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch
 import numpy as np
-from scipy.stats import rankdata
 from torch.optim import SGD
 
+from ..utils.base import rankdata
 from ..utils.metric import get_rank_diff, get_rank_variance
 
 
 def appr_rank_diff(score, old_rank, use_weighted_loss=False):
     """
     Approximate the rank difference between the old rank and the new rank.
 
@@ -60,19 +60,20 @@
         else:
             return max(a[0], b[0])
 
     data = data[cols].values
     data = torch.tensor(data)
     data_std = data.std(0)
     data = data[:, [i for i, _std in enumerate(data_std) if _std > 1e-8]]
+    orig_data = data.clone()
     if normalize_data:
         data = data - data.mean(0)
         data = data / data.std(0)
 
-    old_score = data.mean(1).detach().numpy()
+    old_score = orig_data.mean(1).detach().numpy()
     old_rank = rankdata(-old_score, method="average")
 
     weight = torch.ones(data.shape[1], requires_grad=True)
 
     def normalize_func(w):
         w1 = torch.softmax(w, dim=0)
         w2 = (w1 + min_value / (1 - min_value))
@@ -95,16 +96,18 @@
         if np.fabs(loss.item() - last_loss) < stop_threshold:
             break
         last_loss = loss.item()
         if verbose:
             print("Step %d, Loss = %.2lf" % (step, loss.item()))
 
     norm_weight = normalize_func(weight).detach().numpy()
+    # if normalize_data:
+    #     norm_weight = norm_weight / orig_data.std(0).numpy()
     norm_weight = norm_weight / norm_weight.max()
-    new_score = (data * norm_weight).mean(1).detach().numpy()
+    new_score = (orig_data * norm_weight).mean(1).detach().numpy()
     new_rank = rankdata(-new_score, method="average")
     rank_diff = get_rank_diff(new_rank, old_rank)
     if return_weight:
         return rank_diff, norm_weight
     else:
         return rank_diff
```

### Comparing `bencheval-1.3.1/bencheval/measures/ordinal.py` & `bencheval-1.3.2/bencheval/measures/ordinal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import torch
 import numpy as np
 import pandas as pd
 from torch.optim import Adam
-from scipy.stats import rankdata
 from sklearn.impute import KNNImputer
 
+from ..utils.base import rankdata
 from ..utils.metric import get_rank_diff, get_rank_variance
 from ..utils.win_rate import WinningRate
 
 
 def appr_rank_diff(new_win_rate, inv_indices, orig_rank):
     """
     Approximate the rank difference between the original win rate and the new win rate.
@@ -76,20 +76,20 @@
     Returns:
         tuple: ((tau, MRC), indices) if return_indices is True, else (tau, MRC)
     """
     if inv_indices is None:
         inv_indices = np.arange(len(data) // 5)
 
     torch.manual_seed(0)
-    win_rate_matrix = torch.tensor(WinningRate(data, cols).win_rate).float()
+    win_rate_matrix = torch.tensor(WinningRate(data, cols).win_rate)
 
     orig_win_rate = win_rate_matrix[inv_indices][:, inv_indices].mean(axis=1).numpy()
     orig_rank = rankdata(-orig_win_rate, method="average")
 
-    w = torch.zeros(len(data), requires_grad=True)
+    w = torch.zeros(len(data), requires_grad=True, dtype=torch.double)
     optimizer = Adam([w], lr=lr)
     history = []
     for episode in range(num_step):
         new_win_rate, new_indices = get_selected_win_rate(win_rate_matrix, w, inv_indices)
         loss = appr_rank_diff(new_win_rate, inv_indices, orig_rank)
         if type(loss) is float:
             break
```

### Comparing `bencheval-1.3.1/bencheval/utils/metric.py` & `bencheval-1.3.2/bencheval/utils/metric.py`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval/utils/win_rate.py` & `bencheval-1.3.2/bencheval/utils/win_rate.py`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.1/bencheval.egg-info/PKG-INFO` & `bencheval-1.3.2/bencheval.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bencheval
-Version: 1.3.1
+Version: 1.3.2
 Summary: Tools for measuring sensitivity and diversity of multi-task benchmarks.
 Author: Guanhua Zhang
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `bencheval-1.3.1/bencheval.egg-info/SOURCES.txt` & `bencheval-1.3.2/bencheval.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 bencheval/__init__.py
 bencheval.egg-info/PKG-INFO
 bencheval.egg-info/SOURCES.txt
 bencheval.egg-info/dependency_links.txt
 bencheval.egg-info/requires.txt
 bencheval.egg-info/top_level.txt
 bencheval/data/__init__.py
+bencheval/data/__pycache__/__init__.cpython-311.pyc
 bencheval/data/bbh/__init__.py
 bencheval/data/bbh/cols.txt
 bencheval/data/bbh/format.py
 bencheval/data/bbh/leaderboard.tsv
 bencheval/data/bbh/statistic.py
 bencheval/data/bbh/vanilla.tsv
 bencheval/data/bigcode/__init__.py
```

### Comparing `bencheval-1.3.1/pyproject.toml` & `bencheval-1.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "bencheval"
 authors = [
     {name = "Guanhua Zhang"},
 ]
 description = "Tools for measuring sensitivity and diversity of multi-task benchmarks."
-version = "1.3.1"
+version = "1.3.2"
 requires-python = ">=3.7"
 readme = "README.md"
 license = {text = "MIT"}
 classifiers=[
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: MIT License",
     "Intended Audience :: Science/Research",
```

