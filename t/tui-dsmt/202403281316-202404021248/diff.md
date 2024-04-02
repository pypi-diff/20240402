# Comparing `tmp/tui_dsmt-202403281316.tar.gz` & `tmp/tui_dsmt-202404021248.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tui_dsmt-202403281316.tar", last modified: Thu Mar 28 13:16:21 2024, max compression
+gzip compressed data, was "tui_dsmt-202404021248.tar", last modified: Tue Apr  2 12:48:35 2024, max compression
```

## Comparing `tui_dsmt-202403281316.tar` & `tui_dsmt-202404021248.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:16:21.572785 tui_dsmt-202403281316/
--rw-r--r--   0 root         (0) root         (0)      761 2024-03-28 13:16:21.572785 tui_dsmt-202403281316/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-28 13:16:21.572785 tui_dsmt-202403281316/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1101 2024-03-26 13:16:19.000000 tui_dsmt-202403281316/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:16:21.540785 tui_dsmt-202403281316/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:16:21.540785 tui_dsmt-202403281316/src/tui_dsmt/
--rw-rw-rw-   0 root         (0) root         (0)      569 2024-03-26 11:20:40.000000 tui_dsmt-202403281316/src/tui_dsmt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:16:21.544785 tui_dsmt-202403281316/src/tui_dsmt/clustering/
--rw-rw-rw-   0 root         (0) root         (0)      210 2024-03-08 12:22:54.000000 tui_dsmt-202403281316/src/tui_dsmt/clustering/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2691 2024-03-08 12:22:54.000000 tui_dsmt-202403281316/src/tui_dsmt/clustering/animation.py
--rw-rw-rw-   0 root         (0) root         (0)    18964 2024-03-08 12:22:54.000000 tui_dsmt-202403281316/src/tui_dsmt/clustering/datasets.py
--rw-rw-rw-   0 root         (0) root         (0)      260 2024-03-08 12:22:54.000000 tui_dsmt-202403281316/src/tui_dsmt/clustering/draw.py
--rw-rw-rw-   0 root         (0) root         (0)     1749 2024-03-08 12:22:54.000000 tui_dsmt-202403281316/src/tui_dsmt/clustering/evaluation.py
--rw-rw-rw-   0 root         (0) root         (0)      945 2024-03-08 12:22:54.000000 tui_dsmt-202403281316/src/tui_dsmt/clustering/interactive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:16:21.552785 tui_dsmt-202403281316/src/tui_dsmt/fpm/
--rw-rw-rw-   0 root         (0) root         (0)    14098 2024-03-08 12:22:54.000000 tui_dsmt-202403281316/src/tui_dsmt/fpm/BruteForceFI.py
--rw-rw-rw-   0 root         (0) root         (0)     4055 2024-03-08 12:22:54.000000 tui_dsmt-202403281316/src/tui_dsmt/fpm/ConditionalFPTree.py
--rw-rw-rw-   0 root         (0) root         (0)     5522 2024-03-08 12:22:54.000000 tui_dsmt-202403281316/src/tui_dsmt/fpm/ConditionalPatternBase.py
--rw-rw-rw-   0 root         (0) root         (0)    10145 2024-03-08 12:22:54.000000 tui_dsmt-202403281316/src/tui_dsmt/fpm/FPTree.py
--rw-rw-rw-   0 root         (0) root         (0)     1380 2024-03-08 12:22:54.000000 tui_dsmt-202403281316/src/tui_dsmt/fpm/Itemset.py
--rw-rw-rw-   0 root         (0) root         (0)     3036 2024-03-08 12:22:54.000000 tui_dsmt-202403281316/src/tui_dsmt/fpm/ItemsetGrid.py
--rw-rw-rw-   0 root         (0) root         (0)     5942 2024-03-08 12:22:54.000000 tui_dsmt-202403281316/src/tui_dsmt/fpm/ItemsetGridApriori.py
--rw-rw-rw-   0 root         (0) root         (0)     5865 2024-03-26 11:20:40.000000 tui_dsmt-202403281316/src/tui_dsmt/fpm/ItemsetGridECLAT.py
--rw-rw-rw-   0 root         (0) root         (0)     1262 2024-03-08 12:22:54.000000 tui_dsmt-202403281316/src/tui_dsmt/fpm/SequentialDatabase.py
--rw-rw-rw-   0 root         (0) root         (0)     1129 2024-03-08 12:22:54.000000 tui_dsmt-202403281316/src/tui_dsmt/fpm/SequentialItemset.py
--rw-rw-rw-   0 root         (0) root         (0)     1181 2024-03-08 12:22:54.000000 tui_dsmt-202403281316/src/tui_dsmt/fpm/TransactionDatabase.py
--rw-rw-rw-   0 root         (0) root         (0)     2028 2024-03-14 12:42:03.000000 tui_dsmt-202403281316/src/tui_dsmt/fpm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:16:21.568785 tui_dsmt-202403281316/src/tui_dsmt/graph/
--rw-rw-rw-   0 root         (0) root         (0)     3894 2024-03-08 12:22:54.000000 tui_dsmt-202403281316/src/tui_dsmt/graph/BFS.py
--rw-rw-rw-   0 root         (0) root         (0)     1585 2024-03-08 12:22:54.000000 tui_dsmt-202403281316/src/tui_dsmt/graph/BipartiteFlow.py
--rw-rw-rw-   0 root         (0) root         (0)     3478 2024-03-08 12:22:54.000000 tui_dsmt-202403281316/src/tui_dsmt/graph/DFS.py
--rw-rw-rw-   0 root         (0) root         (0)     5843 2024-03-26 11:20:40.000000 tui_dsmt-202403281316/src/tui_dsmt/graph/Dijkstra.py
--rw-rw-rw-   0 root         (0) root         (0)      175 2024-03-08 12:22:54.000000 tui_dsmt-202403281316/src/tui_dsmt/graph/EdmondsKarp.py
--rw-rw-rw-   0 root         (0) root         (0)     4747 2024-03-08 12:22:54.000000 tui_dsmt-202403281316/src/tui_dsmt/graph/FordFulkerson.py
--rw-rw-rw-   0 root         (0) root         (0)     4461 2024-03-08 12:22:54.000000 tui_dsmt-202403281316/src/tui_dsmt/graph/Hall.py
--rw-rw-rw-   0 root         (0) root         (0)     2095 2024-03-08 12:22:54.000000 tui_dsmt-202403281316/src/tui_dsmt/graph/InteractiveGraph.py
--rw-rw-rw-   0 root         (0) root         (0)     3142 2024-03-08 12:22:54.000000 tui_dsmt-202403281316/src/tui_dsmt/graph/Kruskal.py
--rw-rw-rw-   0 root         (0) root         (0)     2234 2024-03-08 12:22:54.000000 tui_dsmt-202403281316/src/tui_dsmt/graph/MaximumFlow.py
--rw-rw-rw-   0 root         (0) root         (0)   419077 2024-03-26 11:20:40.000000 tui_dsmt-202403281316/src/tui_dsmt/graph/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5267 2024-03-08 12:22:54.000000 tui_dsmt-202403281316/src/tui_dsmt/graph/game.py
--rw-rw-rw-   0 root         (0) root         (0)     5403 2024-03-08 12:22:54.000000 tui_dsmt-202403281316/src/tui_dsmt/graph/html.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2024-03-08 12:22:54.000000 tui_dsmt-202403281316/src/tui_dsmt/graph/representation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:16:21.568785 tui_dsmt-202403281316/src/tui_dsmt/jpanim/
--rw-rw-rw-   0 root         (0) root         (0)     2063 2024-03-08 12:22:54.000000 tui_dsmt-202403281316/src/tui_dsmt/jpanim/JupyterAnimation.py
--rw-rw-rw-   0 root         (0) root         (0)       47 2024-03-08 12:22:54.000000 tui_dsmt-202403281316/src/tui_dsmt/jpanim/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:16:21.572785 tui_dsmt-202403281316/src/tui_dsmt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      761 2024-03-28 13:16:21.000000 tui_dsmt-202403281316/src/tui_dsmt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1366 2024-03-28 13:16:21.000000 tui_dsmt-202403281316/src/tui_dsmt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-28 13:16:21.000000 tui_dsmt-202403281316/src/tui_dsmt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      118 2024-03-28 13:16:21.000000 tui_dsmt-202403281316/src/tui_dsmt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-03-28 13:16:21.000000 tui_dsmt-202403281316/src/tui_dsmt.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 12:48:35.815340 tui_dsmt-202404021248/
+-rw-r--r--   0 root         (0) root         (0)      761 2024-04-02 12:48:35.815340 tui_dsmt-202404021248/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 12:48:35.815340 tui_dsmt-202404021248/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1101 2024-04-02 09:59:49.000000 tui_dsmt-202404021248/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 12:48:35.807340 tui_dsmt-202404021248/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 12:48:35.807340 tui_dsmt-202404021248/src/tui_dsmt/
+-rw-rw-rw-   0 root         (0) root         (0)      569 2024-03-26 11:20:40.000000 tui_dsmt-202404021248/src/tui_dsmt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 12:48:35.807340 tui_dsmt-202404021248/src/tui_dsmt/clustering/
+-rw-rw-rw-   0 root         (0) root         (0)      210 2024-04-02 12:48:28.000000 tui_dsmt-202404021248/src/tui_dsmt/clustering/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2691 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/clustering/animation.py
+-rw-rw-rw-   0 root         (0) root         (0)    18964 2024-04-02 12:48:28.000000 tui_dsmt-202404021248/src/tui_dsmt/clustering/datasets.py
+-rw-rw-rw-   0 root         (0) root         (0)      260 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/clustering/draw.py
+-rw-rw-rw-   0 root         (0) root         (0)     1749 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/clustering/evaluation.py
+-rw-rw-rw-   0 root         (0) root         (0)      945 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/clustering/interactive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 12:48:35.811340 tui_dsmt-202404021248/src/tui_dsmt/fpm/
+-rw-rw-rw-   0 root         (0) root         (0)    14098 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/fpm/BruteForceFI.py
+-rw-rw-rw-   0 root         (0) root         (0)     4055 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/fpm/ConditionalFPTree.py
+-rw-rw-rw-   0 root         (0) root         (0)     5522 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/fpm/ConditionalPatternBase.py
+-rw-rw-rw-   0 root         (0) root         (0)    10145 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/fpm/FPTree.py
+-rw-rw-rw-   0 root         (0) root         (0)     1380 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/fpm/Itemset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3036 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/fpm/ItemsetGrid.py
+-rw-rw-rw-   0 root         (0) root         (0)     5942 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/fpm/ItemsetGridApriori.py
+-rw-rw-rw-   0 root         (0) root         (0)     5865 2024-03-26 11:20:40.000000 tui_dsmt-202404021248/src/tui_dsmt/fpm/ItemsetGridECLAT.py
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/fpm/SequentialDatabase.py
+-rw-rw-rw-   0 root         (0) root         (0)     1129 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/fpm/SequentialItemset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/fpm/TransactionDatabase.py
+-rw-rw-rw-   0 root         (0) root         (0)     2028 2024-03-14 12:42:03.000000 tui_dsmt-202404021248/src/tui_dsmt/fpm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 12:48:35.815340 tui_dsmt-202404021248/src/tui_dsmt/graph/
+-rw-rw-rw-   0 root         (0) root         (0)     3894 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/graph/BFS.py
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/graph/BipartiteFlow.py
+-rw-rw-rw-   0 root         (0) root         (0)     3478 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/graph/DFS.py
+-rw-rw-rw-   0 root         (0) root         (0)     5843 2024-03-26 11:20:40.000000 tui_dsmt-202404021248/src/tui_dsmt/graph/Dijkstra.py
+-rw-rw-rw-   0 root         (0) root         (0)      175 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/graph/EdmondsKarp.py
+-rw-rw-rw-   0 root         (0) root         (0)     4747 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/graph/FordFulkerson.py
+-rw-rw-rw-   0 root         (0) root         (0)     4461 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/graph/Hall.py
+-rw-rw-rw-   0 root         (0) root         (0)     2095 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/graph/InteractiveGraph.py
+-rw-rw-rw-   0 root         (0) root         (0)     3142 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/graph/Kruskal.py
+-rw-rw-rw-   0 root         (0) root         (0)     2234 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/graph/MaximumFlow.py
+-rw-rw-rw-   0 root         (0) root         (0)   419077 2024-03-26 11:20:40.000000 tui_dsmt-202404021248/src/tui_dsmt/graph/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5267 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/graph/game.py
+-rw-rw-rw-   0 root         (0) root         (0)     5403 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/graph/html.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/graph/representation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 12:48:35.815340 tui_dsmt-202404021248/src/tui_dsmt/jpanim/
+-rw-rw-rw-   0 root         (0) root         (0)     2063 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/jpanim/JupyterAnimation.py
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-03-08 12:22:54.000000 tui_dsmt-202404021248/src/tui_dsmt/jpanim/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 12:48:35.815340 tui_dsmt-202404021248/src/tui_dsmt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      761 2024-04-02 12:48:35.000000 tui_dsmt-202404021248/src/tui_dsmt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1366 2024-04-02 12:48:35.000000 tui_dsmt-202404021248/src/tui_dsmt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 12:48:35.000000 tui_dsmt-202404021248/src/tui_dsmt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      118 2024-04-02 12:48:35.000000 tui_dsmt-202404021248/src/tui_dsmt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-02 12:48:35.000000 tui_dsmt-202404021248/src/tui_dsmt.egg-info/top_level.txt
```

### Comparing `tui_dsmt-202403281316/PKG-INFO` & `tui_dsmt-202404021248/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: tui_dsmt
-Version: 202403281316
+Version: 202404021248
 Summary: everything you need for our jupyter notebooks
 Home-page: https://dbgit.prakinf.tu-ilmenau.de/lectures/data-science-methoden-und-techniken
 Author: Eric Tröbs
 Author-email: eric.troebs@tu-ilmenau.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: jupyter
 Requires-Dist: ipywidgets
 Requires-Dist: checkmarkandcross
 Requires-Dist: networkx~=3.2.1
-Requires-Dist: plotly~=5.18.0
-Requires-Dist: pandas~=2.2.0
-Requires-Dist: pyarrow~=15.0.0
+Requires-Dist: plotly~=5.20.0
+Requires-Dist: pandas~=2.2.1
+Requires-Dist: pyarrow~=15.0.2
 Requires-Dist: scikit-learn~=1.4.0
 
 everything you need for our jupyter notebooks
```

### Comparing `tui_dsmt-202403281316/setup.py` & `tui_dsmt-202404021248/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     packages=find_packages(where='src'),
     python_requires='>=3.10',
     install_requires=[
         'jupyter',
         'ipywidgets',
         'checkmarkandcross',
         'networkx~=3.2.1',
-        'plotly~=5.18.0',
-        'pandas~=2.2.0',
-        'pyarrow~=15.0.0',
+        'plotly~=5.20.0',
+        'pandas~=2.2.1',
+        'pyarrow~=15.0.2',
         'scikit-learn~=1.4.0'
     ],
     package_data={},
     include_package_data=True
 )
```

### Comparing `tui_dsmt-202403281316/src/tui_dsmt/__init__.py` & `tui_dsmt-202404021248/src/tui_dsmt/__init__.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202403281316/src/tui_dsmt/clustering/animation.py` & `tui_dsmt-202404021248/src/tui_dsmt/clustering/animation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202403281316/src/tui_dsmt/clustering/datasets.py` & `tui_dsmt-202404021248/src/tui_dsmt/clustering/datasets.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202403281316/src/tui_dsmt/clustering/evaluation.py` & `tui_dsmt-202404021248/src/tui_dsmt/clustering/evaluation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202403281316/src/tui_dsmt/clustering/interactive.py` & `tui_dsmt-202404021248/src/tui_dsmt/clustering/interactive.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202403281316/src/tui_dsmt/fpm/BruteForceFI.py` & `tui_dsmt-202404021248/src/tui_dsmt/fpm/BruteForceFI.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202403281316/src/tui_dsmt/fpm/ConditionalFPTree.py` & `tui_dsmt-202404021248/src/tui_dsmt/fpm/ConditionalFPTree.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202403281316/src/tui_dsmt/fpm/ConditionalPatternBase.py` & `tui_dsmt-202404021248/src/tui_dsmt/fpm/ConditionalPatternBase.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202403281316/src/tui_dsmt/fpm/FPTree.py` & `tui_dsmt-202404021248/src/tui_dsmt/fpm/FPTree.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202403281316/src/tui_dsmt/fpm/Itemset.py` & `tui_dsmt-202404021248/src/tui_dsmt/fpm/Itemset.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202403281316/src/tui_dsmt/fpm/ItemsetGrid.py` & `tui_dsmt-202404021248/src/tui_dsmt/fpm/ItemsetGrid.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202403281316/src/tui_dsmt/fpm/ItemsetGridApriori.py` & `tui_dsmt-202404021248/src/tui_dsmt/fpm/ItemsetGridApriori.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202403281316/src/tui_dsmt/fpm/ItemsetGridECLAT.py` & `tui_dsmt-202404021248/src/tui_dsmt/fpm/ItemsetGridECLAT.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202403281316/src/tui_dsmt/fpm/SequentialDatabase.py` & `tui_dsmt-202404021248/src/tui_dsmt/fpm/SequentialDatabase.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202403281316/src/tui_dsmt/fpm/SequentialItemset.py` & `tui_dsmt-202404021248/src/tui_dsmt/fpm/SequentialItemset.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202403281316/src/tui_dsmt/fpm/TransactionDatabase.py` & `tui_dsmt-202404021248/src/tui_dsmt/fpm/TransactionDatabase.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202403281316/src/tui_dsmt/fpm/__init__.py` & `tui_dsmt-202404021248/src/tui_dsmt/fpm/__init__.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202403281316/src/tui_dsmt/graph/BFS.py` & `tui_dsmt-202404021248/src/tui_dsmt/graph/BFS.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202403281316/src/tui_dsmt/graph/BipartiteFlow.py` & `tui_dsmt-202404021248/src/tui_dsmt/graph/BipartiteFlow.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202403281316/src/tui_dsmt/graph/DFS.py` & `tui_dsmt-202404021248/src/tui_dsmt/graph/DFS.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202403281316/src/tui_dsmt/graph/Dijkstra.py` & `tui_dsmt-202404021248/src/tui_dsmt/graph/Dijkstra.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202403281316/src/tui_dsmt/graph/FordFulkerson.py` & `tui_dsmt-202404021248/src/tui_dsmt/graph/FordFulkerson.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202403281316/src/tui_dsmt/graph/Hall.py` & `tui_dsmt-202404021248/src/tui_dsmt/graph/Hall.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202403281316/src/tui_dsmt/graph/InteractiveGraph.py` & `tui_dsmt-202404021248/src/tui_dsmt/graph/InteractiveGraph.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202403281316/src/tui_dsmt/graph/Kruskal.py` & `tui_dsmt-202404021248/src/tui_dsmt/graph/Kruskal.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202403281316/src/tui_dsmt/graph/MaximumFlow.py` & `tui_dsmt-202404021248/src/tui_dsmt/graph/MaximumFlow.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202403281316/src/tui_dsmt/graph/__init__.py` & `tui_dsmt-202404021248/src/tui_dsmt/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202403281316/src/tui_dsmt/graph/game.py` & `tui_dsmt-202404021248/src/tui_dsmt/graph/game.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202403281316/src/tui_dsmt/graph/html.py` & `tui_dsmt-202404021248/src/tui_dsmt/graph/html.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202403281316/src/tui_dsmt/graph/representation.py` & `tui_dsmt-202404021248/src/tui_dsmt/graph/representation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202403281316/src/tui_dsmt/jpanim/JupyterAnimation.py` & `tui_dsmt-202404021248/src/tui_dsmt/jpanim/JupyterAnimation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202403281316/src/tui_dsmt.egg-info/PKG-INFO` & `tui_dsmt-202404021248/src/tui_dsmt.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: tui_dsmt
-Version: 202403281316
+Version: 202404021248
 Summary: everything you need for our jupyter notebooks
 Home-page: https://dbgit.prakinf.tu-ilmenau.de/lectures/data-science-methoden-und-techniken
 Author: Eric Tröbs
 Author-email: eric.troebs@tu-ilmenau.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: jupyter
 Requires-Dist: ipywidgets
 Requires-Dist: checkmarkandcross
 Requires-Dist: networkx~=3.2.1
-Requires-Dist: plotly~=5.18.0
-Requires-Dist: pandas~=2.2.0
-Requires-Dist: pyarrow~=15.0.0
+Requires-Dist: plotly~=5.20.0
+Requires-Dist: pandas~=2.2.1
+Requires-Dist: pyarrow~=15.0.2
 Requires-Dist: scikit-learn~=1.4.0
 
 everything you need for our jupyter notebooks
```

### Comparing `tui_dsmt-202403281316/src/tui_dsmt.egg-info/SOURCES.txt` & `tui_dsmt-202404021248/src/tui_dsmt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

