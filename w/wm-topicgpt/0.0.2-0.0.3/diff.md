# Comparing `tmp/wm_topicgpt-0.0.2.tar.gz` & `tmp/wm_topicgpt-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wm_topicgpt-0.0.2.tar", last modified: Tue Apr  2 18:07:55 2024, max compression
+gzip compressed data, was "wm_topicgpt-0.0.3.tar", last modified: Tue Apr  2 18:48:56 2024, max compression
```

## Comparing `wm_topicgpt-0.0.2.tar` & `wm_topicgpt-0.0.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-02 18:07:55.520911 wm_topicgpt-0.0.2/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      619 2024-04-02 18:07:55.520484 wm_topicgpt-0.0.2/PKG-INFO
--rw-r--r--   0 y0h07pr    (503) staff       (20)       18 2024-04-02 16:50:46.000000 wm_topicgpt-0.0.2/README.md
--rw-r--r--   0 y0h07pr    (503) staff       (20)       38 2024-04-02 18:07:55.520970 wm_topicgpt-0.0.2/setup.cfg
--rw-r--r--   0 y0h07pr    (503) staff       (20)      360 2024-04-02 18:07:18.000000 wm_topicgpt-0.0.2/setup.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-02 18:07:55.503771 wm_topicgpt-0.0.2/topicgpt/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      196 2024-03-29 15:49:47.000000 wm_topicgpt-0.0.2/topicgpt/__init__.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-02 18:07:55.505015 wm_topicgpt-0.0.2/topicgpt/approach/
--rw-r--r--   0 y0h07pr    (503) staff       (20)       49 2024-04-02 14:08:15.000000 wm_topicgpt-0.0.2/topicgpt/approach/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     1450 2024-04-02 14:11:28.000000 wm_topicgpt-0.0.2/topicgpt/approach/approaches.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-02 18:07:55.508664 wm_topicgpt-0.0.2/topicgpt/cluster/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      483 2024-04-02 14:07:52.000000 wm_topicgpt-0.0.2/topicgpt/cluster/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     4207 2024-04-01 18:42:23.000000 wm_topicgpt-0.0.2/topicgpt/cluster/cluster_base.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     3450 2024-04-01 20:18:33.000000 wm_topicgpt-0.0.2/topicgpt/cluster/hdbscan_cluster.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     1012 2024-04-01 16:07:58.000000 wm_topicgpt-0.0.2/topicgpt/cluster/kmeans_cluster.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)      260 2024-04-02 16:48:50.000000 wm_topicgpt-0.0.2/topicgpt/config.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-02 18:07:55.509976 wm_topicgpt-0.0.2/topicgpt/embedding/
--rw-r--r--   0 y0h07pr    (503) staff       (20)       84 2024-03-29 15:20:23.000000 wm_topicgpt-0.0.2/topicgpt/embedding/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     1416 2024-03-28 20:53:59.000000 wm_topicgpt-0.0.2/topicgpt/embedding/create_embeddings.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-02 18:07:55.510917 wm_topicgpt-0.0.2/topicgpt/feature_extraction/
--rw-r--r--   0 y0h07pr    (503) staff       (20)       85 2024-04-02 16:33:26.000000 wm_topicgpt-0.0.2/topicgpt/feature_extraction/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     2694 2024-04-02 16:39:59.000000 wm_topicgpt-0.0.2/topicgpt/feature_extraction/extract_keywords.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-02 18:07:55.512956 wm_topicgpt-0.0.2/topicgpt/preprocessing/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      206 2024-03-29 15:19:50.000000 wm_topicgpt-0.0.2/topicgpt/preprocessing/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)      847 2024-03-28 20:24:54.000000 wm_topicgpt-0.0.2/topicgpt/preprocessing/drop_data.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     1528 2024-03-28 20:24:28.000000 wm_topicgpt-0.0.2/topicgpt/preprocessing/pii_filters.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)      412 2024-03-28 20:09:22.000000 wm_topicgpt-0.0.2/topicgpt/utils.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-02 18:07:55.513849 wm_topicgpt-0.0.2/topicgpt/visualization/
--rw-r--r--   0 y0h07pr    (503) staff       (20)       44 2024-04-01 20:48:12.000000 wm_topicgpt-0.0.2/topicgpt/visualization/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)      480 2024-04-01 20:43:50.000000 wm_topicgpt-0.0.2/topicgpt/visualization/plot_taxonomy.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-02 18:07:55.515446 wm_topicgpt-0.0.2/topicgpt/walmart_llm/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      230 2024-03-28 16:31:49.000000 wm_topicgpt-0.0.2/topicgpt/walmart_llm/__init__.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     9121 2024-03-28 16:25:13.000000 wm_topicgpt-0.0.2/topicgpt/walmart_llm/chat_model.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     8079 2024-03-28 16:26:16.000000 wm_topicgpt-0.0.2/topicgpt/walmart_llm/embed_model.py
--rw-r--r--   0 y0h07pr    (503) staff       (20)     6144 2024-04-01 16:33:53.000000 wm_topicgpt-0.0.2/topicgpt/walmart_llm/llm_client.py
-drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-02 18:07:55.519864 wm_topicgpt-0.0.2/wm_topicgpt.egg-info/
--rw-r--r--   0 y0h07pr    (503) staff       (20)      619 2024-04-02 18:07:55.000000 wm_topicgpt-0.0.2/wm_topicgpt.egg-info/PKG-INFO
--rw-r--r--   0 y0h07pr    (503) staff       (20)      927 2024-04-02 18:07:55.000000 wm_topicgpt-0.0.2/wm_topicgpt.egg-info/SOURCES.txt
--rw-r--r--   0 y0h07pr    (503) staff       (20)        1 2024-04-02 18:07:55.000000 wm_topicgpt-0.0.2/wm_topicgpt.egg-info/dependency_links.txt
--rw-r--r--   0 y0h07pr    (503) staff       (20)      264 2024-04-02 18:07:55.000000 wm_topicgpt-0.0.2/wm_topicgpt.egg-info/requires.txt
--rw-r--r--   0 y0h07pr    (503) staff       (20)        9 2024-04-02 18:07:55.000000 wm_topicgpt-0.0.2/wm_topicgpt.egg-info/top_level.txt
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-02 18:48:56.399508 wm_topicgpt-0.0.3/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      662 2024-04-02 18:48:56.398890 wm_topicgpt-0.0.3/PKG-INFO
+-rw-r--r--   0 y0h07pr    (503) staff       (20)       18 2024-04-02 16:50:46.000000 wm_topicgpt-0.0.3/README.md
+-rw-r--r--   0 y0h07pr    (503) staff       (20)       38 2024-04-02 18:48:56.399569 wm_topicgpt-0.0.3/setup.cfg
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      360 2024-04-02 18:48:53.000000 wm_topicgpt-0.0.3/setup.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-02 18:48:56.372153 wm_topicgpt-0.0.3/topicgpt/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      196 2024-03-29 15:49:47.000000 wm_topicgpt-0.0.3/topicgpt/__init__.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-02 18:48:56.373929 wm_topicgpt-0.0.3/topicgpt/approach/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)       49 2024-04-02 14:08:15.000000 wm_topicgpt-0.0.3/topicgpt/approach/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     1471 2024-04-02 18:34:37.000000 wm_topicgpt-0.0.3/topicgpt/approach/approaches.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-02 18:48:56.377045 wm_topicgpt-0.0.3/topicgpt/cluster/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      483 2024-04-02 14:07:52.000000 wm_topicgpt-0.0.3/topicgpt/cluster/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     4207 2024-04-01 18:42:23.000000 wm_topicgpt-0.0.3/topicgpt/cluster/cluster_base.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     3450 2024-04-01 20:18:33.000000 wm_topicgpt-0.0.3/topicgpt/cluster/hdbscan_cluster.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     1012 2024-04-01 16:07:58.000000 wm_topicgpt-0.0.3/topicgpt/cluster/kmeans_cluster.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      260 2024-04-02 16:48:50.000000 wm_topicgpt-0.0.3/topicgpt/config.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-02 18:48:56.378748 wm_topicgpt-0.0.3/topicgpt/embedding/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)       84 2024-03-29 15:20:23.000000 wm_topicgpt-0.0.3/topicgpt/embedding/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     1416 2024-03-28 20:53:59.000000 wm_topicgpt-0.0.3/topicgpt/embedding/create_embeddings.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-02 18:48:56.380471 wm_topicgpt-0.0.3/topicgpt/feature_extraction/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)       85 2024-04-02 16:33:26.000000 wm_topicgpt-0.0.3/topicgpt/feature_extraction/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     2694 2024-04-02 16:39:59.000000 wm_topicgpt-0.0.3/topicgpt/feature_extraction/extract_keywords.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-02 18:48:56.383551 wm_topicgpt-0.0.3/topicgpt/preprocessing/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      206 2024-03-29 15:19:50.000000 wm_topicgpt-0.0.3/topicgpt/preprocessing/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      847 2024-03-28 20:24:54.000000 wm_topicgpt-0.0.3/topicgpt/preprocessing/drop_data.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     1528 2024-03-28 20:24:28.000000 wm_topicgpt-0.0.3/topicgpt/preprocessing/pii_filters.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      412 2024-03-28 20:09:22.000000 wm_topicgpt-0.0.3/topicgpt/utils.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-02 18:48:56.385722 wm_topicgpt-0.0.3/topicgpt/visualization/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)       44 2024-04-01 20:48:12.000000 wm_topicgpt-0.0.3/topicgpt/visualization/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      480 2024-04-01 20:43:50.000000 wm_topicgpt-0.0.3/topicgpt/visualization/plot_taxonomy.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-02 18:48:56.390426 wm_topicgpt-0.0.3/topicgpt/walmart_llm/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      230 2024-03-28 16:31:49.000000 wm_topicgpt-0.0.3/topicgpt/walmart_llm/__init__.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     9121 2024-03-28 16:25:13.000000 wm_topicgpt-0.0.3/topicgpt/walmart_llm/chat_model.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     8079 2024-03-28 16:26:16.000000 wm_topicgpt-0.0.3/topicgpt/walmart_llm/embed_model.py
+-rw-r--r--   0 y0h07pr    (503) staff       (20)     6144 2024-04-01 16:33:53.000000 wm_topicgpt-0.0.3/topicgpt/walmart_llm/llm_client.py
+drwxr-xr-x   0 y0h07pr    (503) staff       (20)        0 2024-04-02 18:48:56.397987 wm_topicgpt-0.0.3/wm_topicgpt.egg-info/
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      662 2024-04-02 18:48:56.000000 wm_topicgpt-0.0.3/wm_topicgpt.egg-info/PKG-INFO
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      927 2024-04-02 18:48:56.000000 wm_topicgpt-0.0.3/wm_topicgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 y0h07pr    (503) staff       (20)        1 2024-04-02 18:48:56.000000 wm_topicgpt-0.0.3/wm_topicgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 y0h07pr    (503) staff       (20)      292 2024-04-02 18:48:56.000000 wm_topicgpt-0.0.3/wm_topicgpt.egg-info/requires.txt
+-rw-r--r--   0 y0h07pr    (503) staff       (20)        9 2024-04-02 18:48:56.000000 wm_topicgpt-0.0.3/wm_topicgpt.egg-info/top_level.txt
```

### Comparing `wm_topicgpt-0.0.2/PKG-INFO` & `wm_topicgpt-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: wm_topicgpt
-Version: 0.0.2
+Version: 0.0.3
 Summary: This is a package to generate topics for the text corpus.
 Requires-Python: >=3.9
 Requires-Dist: numpy==1.26.4
 Requires-Dist: pandas==2.2.1
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: azure-ai-textanalytics==5.3.0
 Requires-Dist: aiohttp==3.9.3
 Requires-Dist: langchain==0.1.14
 Requires-Dist: langchain_community==0.0.31
 Requires-Dist: pycryptodome==3.10.1
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: openai==1.16.0
 Requires-Dist: scikit_learn==1.4.0
-Requires-Dist: spacy==3.7.2
 Requires-Dist: umap_learn==0.5.5
 Requires-Dist: sentence_transformers==2.6.1
+Requires-Dist: spacy==3.7.2
+Requires-Dist: en_core_web_sm-3.7.2.tar.gz
```

### Comparing `wm_topicgpt-0.0.2/topicgpt/approach/approaches.py` & `wm_topicgpt-0.0.3/topicgpt/approach/approaches.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,7 +32,9 @@
     
     # clustering
     root = generate_cluster_tree(dataframe, embed_col_name, dim=reduced_dim, n_neighbors=n_neighbors, min_cluster_size=min_cluster_size)
     generate_topic_for_cluster_tree(root, text_col_name, embed_col_name, topk=topk)
 
     # plot
     plot_cluster_tree(root)
+    
+    return root
```

### Comparing `wm_topicgpt-0.0.2/topicgpt/cluster/cluster_base.py` & `wm_topicgpt-0.0.3/topicgpt/cluster/cluster_base.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.2/topicgpt/cluster/hdbscan_cluster.py` & `wm_topicgpt-0.0.3/topicgpt/cluster/hdbscan_cluster.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.2/topicgpt/cluster/kmeans_cluster.py` & `wm_topicgpt-0.0.3/topicgpt/cluster/kmeans_cluster.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.2/topicgpt/embedding/create_embeddings.py` & `wm_topicgpt-0.0.3/topicgpt/embedding/create_embeddings.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.2/topicgpt/feature_extraction/extract_keywords.py` & `wm_topicgpt-0.0.3/topicgpt/feature_extraction/extract_keywords.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.2/topicgpt/preprocessing/drop_data.py` & `wm_topicgpt-0.0.3/topicgpt/preprocessing/drop_data.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.2/topicgpt/preprocessing/pii_filters.py` & `wm_topicgpt-0.0.3/topicgpt/preprocessing/pii_filters.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.2/topicgpt/walmart_llm/chat_model.py` & `wm_topicgpt-0.0.3/topicgpt/walmart_llm/chat_model.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.2/topicgpt/walmart_llm/embed_model.py` & `wm_topicgpt-0.0.3/topicgpt/walmart_llm/embed_model.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.2/topicgpt/walmart_llm/llm_client.py` & `wm_topicgpt-0.0.3/topicgpt/walmart_llm/llm_client.py`

 * *Files identical despite different names*

### Comparing `wm_topicgpt-0.0.2/wm_topicgpt.egg-info/PKG-INFO` & `wm_topicgpt-0.0.3/wm_topicgpt.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: wm-topicgpt
-Version: 0.0.2
+Version: 0.0.3
 Summary: This is a package to generate topics for the text corpus.
 Requires-Python: >=3.9
 Requires-Dist: numpy==1.26.4
 Requires-Dist: pandas==2.2.1
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: azure-ai-textanalytics==5.3.0
 Requires-Dist: aiohttp==3.9.3
 Requires-Dist: langchain==0.1.14
 Requires-Dist: langchain_community==0.0.31
 Requires-Dist: pycryptodome==3.10.1
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: openai==1.16.0
 Requires-Dist: scikit_learn==1.4.0
-Requires-Dist: spacy==3.7.2
 Requires-Dist: umap_learn==0.5.5
 Requires-Dist: sentence_transformers==2.6.1
+Requires-Dist: spacy==3.7.2
+Requires-Dist: en_core_web_sm-3.7.2.tar.gz
```

### Comparing `wm_topicgpt-0.0.2/wm_topicgpt.egg-info/SOURCES.txt` & `wm_topicgpt-0.0.3/wm_topicgpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

