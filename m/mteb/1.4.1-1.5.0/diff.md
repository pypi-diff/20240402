# Comparing `tmp/mteb-1.4.1.tar.gz` & `tmp/mteb-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mteb-1.4.1.tar", last modified: Mon Apr  1 14:19:08 2024, max compression
+gzip compressed data, was "mteb-1.5.0.tar", last modified: Tue Apr  2 17:03:38 2024, max compression
```

## Comparing `mteb-1.4.1.tar` & `mteb-1.5.0.tar`

### file list

```diff
@@ -1,370 +1,371 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.945355 mteb-1.4.1/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-04-01 14:19:04.000000 mteb-1.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    23581 2024-04-01 14:19:08.945355 mteb-1.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9190 2024-04-01 14:19:04.000000 mteb-1.4.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.885354 mteb-1.4.1/mteb/
--rw-r--r--   0 root         (0) root         (0)     1917 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.893354 mteb-1.4.1/mteb/abstasks/
--rw-r--r--   0 root         (0) root         (0)     1592 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/abstasks/AbsTask.py
--rw-r--r--   0 root         (0) root         (0)     3063 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/abstasks/AbsTaskBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     5881 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/abstasks/AbsTaskClassification.py
--rw-r--r--   0 root         (0) root         (0)     2389 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/abstasks/AbsTaskClustering.py
--rw-r--r--   0 root         (0) root         (0)     2542 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/abstasks/AbsTaskPairClassification.py
--rw-r--r--   0 root         (0) root         (0)     1120 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/abstasks/AbsTaskReranking.py
--rw-r--r--   0 root         (0) root         (0)    11832 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/abstasks/AbsTaskRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2007 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/abstasks/AbsTaskSTS.py
--rw-r--r--   0 root         (0) root         (0)     2296 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/abstasks/AbsTaskSummarization.py
--rw-r--r--   0 root         (0) root         (0)      961 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/abstasks/CrosslingualTask.py
--rw-r--r--   0 root         (0) root         (0)     2831 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/abstasks/LangMapping.py
--rw-r--r--   0 root         (0) root         (0)     1052 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/abstasks/MultilingualTask.py
--rw-r--r--   0 root         (0) root         (0)     5356 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/abstasks/TaskMetadata.py
--rw-r--r--   0 root         (0) root         (0)      422 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/abstasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5296 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.893354 mteb-1.4.1/mteb/evaluation/
--rw-r--r--   0 root         (0) root         (0)    13067 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/evaluation/MTEB.py
--rw-r--r--   0 root         (0) root         (0)       56 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/evaluation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.893354 mteb-1.4.1/mteb/evaluation/evaluators/
--rw-r--r--   0 root         (0) root         (0)     5849 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/evaluation/evaluators/BitextMiningEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     8942 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/evaluation/evaluators/ClassificationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1463 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/evaluation/evaluators/ClusteringEvaluator.py
--rw-r--r--   0 root         (0) root         (0)      744 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/evaluation/evaluators/Evaluator.py
--rw-r--r--   0 root         (0) root         (0)     7140 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/evaluation/evaluators/PairClassificationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     9613 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/evaluation/evaluators/RerankingEvaluator.py
--rw-r--r--   0 root         (0) root         (0)    12487 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/evaluation/evaluators/RetrievalEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     2394 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/evaluation/evaluators/STSEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     4841 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/evaluation/evaluators/SummarizationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)      324 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/evaluation/evaluators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5482 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/evaluation/evaluators/utils.py
--rw-r--r--   0 root         (0) root         (0)      835 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.893354 mteb-1.4.1/mteb/tasks/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.893354 mteb-1.4.1/mteb/tasks/BitextMining/
--rw-r--r--   0 root         (0) root         (0)      369 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/BitextMining/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.893354 mteb-1.4.1/mteb/tasks/BitextMining/da/
--rw-r--r--   0 root         (0) root         (0)     1800 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/BitextMining/da/BornholmskBitextMining.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/BitextMining/da/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.897354 mteb-1.4.1/mteb/tasks/BitextMining/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1040 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     2257 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     5808 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     1813 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     2761 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/BitextMining/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.897354 mteb-1.4.1/mteb/tasks/BitextMining/nb/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/BitextMining/nb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1806 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/BitextMining/nb/norwegian_courts_bitext_mining.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.897354 mteb-1.4.1/mteb/tasks/Classification/
--rw-r--r--   0 root         (0) root         (0)     1232 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Classification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.897354 mteb-1.4.1/mteb/tasks/Classification/da/
--rw-r--r--   0 root         (0) root         (0)     1278 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Classification/da/AngryTweetsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1978 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Classification/da/DKHateClassification.py
--rw-r--r--   0 root         (0) root         (0)     2881 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Classification/da/DalajClassification.py
--rw-r--r--   0 root         (0) root         (0)     1967 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Classification/da/DanishPoliticalCommentsClassification.py
--rw-r--r--   0 root         (0) root         (0)     3303 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Classification/da/DdiscoCohesionClassification.py
--rw-r--r--   0 root         (0) root         (0)     1217 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Classification/da/LccSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Classification/da/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.897354 mteb-1.4.1/mteb/tasks/Classification/en/
--rw-r--r--   0 root         (0) root         (0)      999 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Classification/en/AmazonPolarityClassification.py
--rw-r--r--   0 root         (0) root         (0)     1012 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Classification/en/Banking77Classification.py
--rw-r--r--   0 root         (0) root         (0)     1330 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Classification/en/EmotionClassification.py
--rw-r--r--   0 root         (0) root         (0)      948 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Classification/en/ImdbClassification.py
--rw-r--r--   0 root         (0) root         (0)     1368 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Classification/en/ToxicConversationsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1239 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Classification/en/TweetSentimentExtractionClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Classification/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.901354 mteb-1.4.1/mteb/tasks/Classification/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1447 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py
--rw-r--r--   0 root         (0) root         (0)     1199 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1128 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py
--rw-r--r--   0 root         (0) root         (0)     1128 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1367 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py
--rw-r--r--   0 root         (0) root         (0)     1787 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1793 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py
--rw-r--r--   0 root         (0) root         (0)     1841 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Classification/multilingual/NordicLangClassification.py
--rw-r--r--   0 root         (0) root         (0)     7434 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Classification/multilingual/ScalaClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Classification/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.901354 mteb-1.4.1/mteb/tasks/Classification/nb/
--rw-r--r--   0 root         (0) root         (0)     1063 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Classification/nb/NoRecClassification.py
--rw-r--r--   0 root         (0) root         (0)     1124 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Classification/nb/NorwegianParliamentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Classification/nb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.901354 mteb-1.4.1/mteb/tasks/Classification/pl/
--rw-r--r--   0 root         (0) root         (0)     4712 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Classification/pl/PolishClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Classification/pl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.901354 mteb-1.4.1/mteb/tasks/Classification/sv/
--rw-r--r--   0 root         (0) root         (0)      995 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Classification/sv/SweRecClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Classification/sv/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.901354 mteb-1.4.1/mteb/tasks/Classification/zh/
--rw-r--r--   0 root         (0) root         (0)     6307 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Classification/zh/CMTEBClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Classification/zh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.901354 mteb-1.4.1/mteb/tasks/Clustering/
--rw-r--r--   0 root         (0) root         (0)     1249 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.905354 mteb-1.4.1/mteb/tasks/Clustering/de/
--rw-r--r--   0 root         (0) root         (0)     1090 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/de/BlurbsClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1073 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/de/BlurbsClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1058 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/de/TenKGnadClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1038 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/de/TenKGnadClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/de/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.905354 mteb-1.4.1/mteb/tasks/Clustering/en/
--rw-r--r--   0 root         (0) root         (0)     1059 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/en/ArxivClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1045 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/en/ArxivClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1086 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/en/BigPatentClustering.py
--rw-r--r--   0 root         (0) root         (0)     1029 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/en/BiorxivClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1019 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/en/BiorxivClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1030 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/en/MedrxivClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1020 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/en/MedrxivClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1060 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/en/RedditClustering.py
--rw-r--r--   0 root         (0) root         (0)     1049 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/en/RedditClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1085 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/en/StackExchangeClustering.py
--rw-r--r--   0 root         (0) root         (0)     1073 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/en/StackExchangeClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1042 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/en/TwentyNewsgroupsClustering.py
--rw-r--r--   0 root         (0) root         (0)     1093 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/en/WikiCitiesClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.905354 mteb-1.4.1/mteb/tasks/Clustering/es/
--rw-r--r--   0 root         (0) root         (0)      987 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/es/FloresClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1016 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/es/SpanishNewsClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/es/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.909355 mteb-1.4.1/mteb/tasks/Clustering/fr/
--rw-r--r--   0 root         (0) root         (0)     2278 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/fr/AlloProfClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     2123 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/fr/AlloProfClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1985 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/fr/HALClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     2334 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/fr/MLSUMClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     2149 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/fr/MLSUMClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/fr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.909355 mteb-1.4.1/mteb/tasks/Clustering/multilingual/
--rw-r--r--   0 root         (0) root         (0)     2522 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     2541 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.909355 mteb-1.4.1/mteb/tasks/Clustering/nb/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/nb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3837 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/nb/snl_clustering.py
--rw-r--r--   0 root         (0) root         (0)     3991 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/nb/vg_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.909355 mteb-1.4.1/mteb/tasks/Clustering/pl/
--rw-r--r--   0 root         (0) root         (0)     1093 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/pl/PolishClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/pl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.909355 mteb-1.4.1/mteb/tasks/Clustering/sv/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/sv/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4342 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/sv/swedn_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.909355 mteb-1.4.1/mteb/tasks/Clustering/zh/
--rw-r--r--   0 root         (0) root         (0)     3441 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/zh/CMTEBClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Clustering/zh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.909355 mteb-1.4.1/mteb/tasks/PairClassification/
--rw-r--r--   0 root         (0) root         (0)      301 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/PairClassification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.913354 mteb-1.4.1/mteb/tasks/PairClassification/en/
--rw-r--r--   0 root         (0) root         (0)     1110 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/PairClassification/en/SprintDuplicateQuestionsPC.py
--rw-r--r--   0 root         (0) root         (0)     1044 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/PairClassification/en/TwitterSemEval2015PC.py
--rw-r--r--   0 root         (0) root         (0)      998 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/PairClassification/en/TwitterURLCorpusPC.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/PairClassification/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.913354 mteb-1.4.1/mteb/tasks/PairClassification/multilingual/
--rw-r--r--   0 root         (0) root         (0)     2720 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py
--rw-r--r--   0 root         (0) root         (0)     1930 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/PairClassification/multilingual/PawsX.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/PairClassification/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.913354 mteb-1.4.1/mteb/tasks/PairClassification/pl/
--rw-r--r--   0 root         (0) root         (0)     3298 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/PairClassification/pl/PolishPC.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/PairClassification/pl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.913354 mteb-1.4.1/mteb/tasks/PairClassification/zh/
--rw-r--r--   0 root         (0) root         (0)     1765 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/PairClassification/zh/CMTEBPairClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/PairClassification/zh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.913354 mteb-1.4.1/mteb/tasks/Reranking/
--rw-r--r--   0 root         (0) root         (0)      339 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Reranking/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.913354 mteb-1.4.1/mteb/tasks/Reranking/en/
--rw-r--r--   0 root         (0) root         (0)     1076 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Reranking/en/AskUbuntuDupQuestions.py
--rw-r--r--   0 root         (0) root         (0)     1022 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Reranking/en/MindSmallReranking.py
--rw-r--r--   0 root         (0) root         (0)     2974 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Reranking/en/SciDocsReranking.py
--rw-r--r--   0 root         (0) root         (0)     1095 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Reranking/en/StackOverflowDupQuestions.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Reranking/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.913354 mteb-1.4.1/mteb/tasks/Reranking/fr/
--rw-r--r--   0 root         (0) root         (0)     1137 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Reranking/fr/AlloprofReranking.py
--rw-r--r--   0 root         (0) root         (0)     1023 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Reranking/fr/SyntecReranking.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Reranking/fr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.913354 mteb-1.4.1/mteb/tasks/Reranking/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1170 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Reranking/multilingual/MIRACLReranking.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Reranking/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.913354 mteb-1.4.1/mteb/tasks/Reranking/zh/
--rw-r--r--   0 root         (0) root         (0)     3360 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Reranking/zh/CMTEBReranking.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Reranking/zh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.913354 mteb-1.4.1/mteb/tasks/Retrieval/
--rw-r--r--   0 root         (0) root         (0)     2462 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.917355 mteb-1.4.1/mteb/tasks/Retrieval/da/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/da/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4206 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/da/dan_fever.py
--rw-r--r--   0 root         (0) root         (0)     2978 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/da/t2nord_retrieval.py
--rw-r--r--   0 root         (0) root         (0)     3543 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/da/twitterhjerne.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.917355 mteb-1.4.1/mteb/tasks/Retrieval/de/
--rw-r--r--   0 root         (0) root         (0)     2186 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/de/GerDaLIRRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2925 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/de/GermanDPRRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2067 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/de/GermanQuADRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/de/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.921355 mteb-1.4.1/mteb/tasks/Retrieval/en/
--rw-r--r--   0 root         (0) root         (0)      969 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/en/ArguAnaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1023 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/en/CQADupstackAndroidRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1023 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/en/CQADupstackEnglishRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1020 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/en/CQADupstackGamingRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1011 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/en/CQADupstackGisRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1035 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/en/CQADupstackMathematicaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1023 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/en/CQADupstackPhysicsRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1035 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/en/CQADupstackProgrammersRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1017 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/en/CQADupstackStatsRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1011 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/en/CQADupstackTexRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1014 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/en/CQADupstackUnixRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1032 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/en/CQADupstackWebmastersRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1029 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/en/CQADupstackWordpressRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1053 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/en/ClimateFEVERRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      989 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/en/DBPediaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1133 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/en/FEVERRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      941 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/en/FiQA2018Retrieval.py
--rw-r--r--   0 root         (0) root         (0)     3652 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/en/HagridRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1109 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/en/HotpotQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)      967 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/en/MSMARCORetrieval.py
--rw-r--r--   0 root         (0) root         (0)      997 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/en/MSMARCOv2Retrieval.py
--rw-r--r--   0 root         (0) root         (0)      982 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/en/NFCorpusRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      957 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/en/NQRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1938 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/en/NarrativeQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1113 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/en/QuoraRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1072 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/en/SCIDOCSRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1004 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/en/SciFactRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1027 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/en/TRECCOVIDRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      967 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/en/Touche2020Retrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.921355 mteb-1.4.1/mteb/tasks/Retrieval/es/
--rw-r--r--   0 root         (0) root         (0)     2074 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2P.py
--rw-r--r--   0 root         (0) root         (0)     2074 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/es/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.925355 mteb-1.4.1/mteb/tasks/Retrieval/fr/
--rw-r--r--   0 root         (0) root         (0)     2067 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/fr/AlloprofRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2540 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/fr/BSARDRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2053 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/fr/SyntecRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/fr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.925355 mteb-1.4.1/mteb/tasks/Retrieval/ko/
--rw-r--r--   0 root         (0) root         (0)      864 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/ko/KoMiracl.py
--rw-r--r--   0 root         (0) root         (0)      864 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/ko/KoMrtydi.py
--rw-r--r--   0 root         (0) root         (0)      880 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/ko/KoStrategyQA.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/ko/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.925355 mteb-1.4.1/mteb/tasks/Retrieval/multilingual/
--rw-r--r--   0 root         (0) root         (0)     3197 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2854 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3083 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2870 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2874 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.925355 mteb-1.4.1/mteb/tasks/Retrieval/nb/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/nb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4347 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/nb/norquad.py
--rw-r--r--   0 root         (0) root         (0)     3103 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/nb/snl_retrieval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.929355 mteb-1.4.1/mteb/tasks/Retrieval/pl/
--rw-r--r--   0 root         (0) root         (0)      925 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/pl/ArguAnaPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      998 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/pl/DBPediaPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      942 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/pl/FiQAPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1070 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/pl/HotpotQAPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      967 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/pl/MSMARCOPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      998 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/pl/NFCorpusPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      955 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/pl/NQPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1121 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/pl/QuoraPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1049 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/pl/SCIDOCSPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1011 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/pl/SciFactPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1043 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/pl/TRECCOVIDPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/pl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.929355 mteb-1.4.1/mteb/tasks/Retrieval/sv/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/sv/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3635 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/sv/swedn_retrieval.py
--rw-r--r--   0 root         (0) root         (0)     3035 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/sv/swefaq_retrieval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.929355 mteb-1.4.1/mteb/tasks/Retrieval/zh/
--rw-r--r--   0 root         (0) root         (0)     9421 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/zh/CMTEBRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Retrieval/zh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.929355 mteb-1.4.1/mteb/tasks/STS/
--rw-r--r--   0 root         (0) root         (0)      562 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/STS/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.929355 mteb-1.4.1/mteb/tasks/STS/de/
--rw-r--r--   0 root         (0) root         (0)     1326 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/STS/de/GermanSTSBenchmarkSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/STS/de/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.933355 mteb-1.4.1/mteb/tasks/STS/en/
--rw-r--r--   0 root         (0) root         (0)     1140 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/STS/en/BiossesSTS.py
--rw-r--r--   0 root         (0) root         (0)     1109 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/STS/en/STS12STS.py
--rw-r--r--   0 root         (0) root         (0)     1106 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/STS/en/STS13STS.py
--rw-r--r--   0 root         (0) root         (0)     1140 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/STS/en/STS14STS.py
--rw-r--r--   0 root         (0) root         (0)     1104 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/STS/en/STS15STS.py
--rw-r--r--   0 root         (0) root         (0)     1104 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/STS/en/STS16STS.py
--rw-r--r--   0 root         (0) root         (0)     1164 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/STS/en/STSBenchmarkSTS.py
--rw-r--r--   0 root         (0) root         (0)     1149 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/STS/en/SickrSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/STS/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.933355 mteb-1.4.1/mteb/tasks/STS/es/
--rw-r--r--   0 root         (0) root         (0)     1686 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/STS/es/STSES.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/STS/es/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.933355 mteb-1.4.1/mteb/tasks/STS/fr/
--rw-r--r--   0 root         (0) root         (0)     1804 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/STS/fr/SickFrSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/STS/fr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.933355 mteb-1.4.1/mteb/tasks/STS/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1324 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py
--rw-r--r--   0 root         (0) root         (0)     1446 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py
--rw-r--r--   0 root         (0) root         (0)     2556 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/STS/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.933355 mteb-1.4.1/mteb/tasks/STS/pl/
--rw-r--r--   0 root         (0) root         (0)     2180 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/STS/pl/PolishSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/STS/pl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.933355 mteb-1.4.1/mteb/tasks/STS/zh/
--rw-r--r--   0 root         (0) root         (0)     6816 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/STS/zh/CMTEBSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/STS/zh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.933355 mteb-1.4.1/mteb/tasks/Summarization/
--rw-r--r--   0 root         (0) root         (0)      122 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Summarization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.933355 mteb-1.4.1/mteb/tasks/Summarization/en/
--rw-r--r--   0 root         (0) root         (0)     1199 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Summarization/en/SummEvalSummarization.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Summarization/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.937355 mteb-1.4.1/mteb/tasks/Summarization/fr/
--rw-r--r--   0 root         (0) root         (0)     1239 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Summarization/fr/SummEvalFrSummarization.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/Summarization/fr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      252 2024-04-01 14:19:04.000000 mteb-1.4.1/mteb/tasks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.941355 mteb-1.4.1/mteb.egg-info/
--rw-r--r--   0 root         (0) root         (0)    23581 2024-04-01 14:19:08.000000 mteb-1.4.1/mteb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12552 2024-04-01 14:19:08.000000 mteb-1.4.1/mteb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-01 14:19:08.000000 mteb-1.4.1/mteb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-04-01 14:19:08.000000 mteb-1.4.1/mteb.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      234 2024-04-01 14:19:08.000000 mteb-1.4.1/mteb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-04-01 14:19:08.000000 mteb-1.4.1/mteb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2120 2024-04-01 14:19:05.000000 mteb-1.4.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.937355 mteb-1.4.1/scripts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.937355 mteb-1.4.1/scripts/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.937355 mteb-1.4.1/scripts/data/amazon_polarity/
--rw-r--r--   0 root         (0) root         (0)      842 2024-04-01 14:19:04.000000 mteb-1.4.1/scripts/data/amazon_polarity/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.937355 mteb-1.4.1/scripts/data/amazon_reviews_multi/
--rw-r--r--   0 root         (0) root         (0)     1379 2024-04-01 14:19:04.000000 mteb-1.4.1/scripts/data/amazon_reviews_multi/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.937355 mteb-1.4.1/scripts/data/arxiv/
--rw-r--r--   0 root         (0) root         (0)     3146 2024-04-01 14:19:04.000000 mteb-1.4.1/scripts/data/arxiv/script_clustering.py
--rw-r--r--   0 root         (0) root         (0)     1451 2024-04-01 14:19:04.000000 mteb-1.4.1/scripts/data/arxiv/script_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.937355 mteb-1.4.1/scripts/data/biorxiv/
--rw-r--r--   0 root         (0) root         (0)     1781 2024-04-01 14:19:04.000000 mteb-1.4.1/scripts/data/biorxiv/script_clustering.py
--rw-r--r--   0 root         (0) root         (0)     1674 2024-04-01 14:19:04.000000 mteb-1.4.1/scripts/data/biorxiv/script_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.937355 mteb-1.4.1/scripts/data/bucc/
--rw-r--r--   0 root         (0) root         (0)     1171 2024-04-01 14:19:04.000000 mteb-1.4.1/scripts/data/bucc/create_data.py
--rw-r--r--   0 root         (0) root         (0)     5933 2024-04-01 14:19:04.000000 mteb-1.4.1/scripts/data/create_task_table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.937355 mteb-1.4.1/scripts/data/germanquad/
--rw-r--r--   0 root         (0) root         (0)     2132 2024-04-01 14:19:04.000000 mteb-1.4.1/scripts/data/germanquad/process_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.937355 mteb-1.4.1/scripts/data/hal/
--rw-r--r--   0 root         (0) root         (0)     1512 2024-04-01 14:19:04.000000 mteb-1.4.1/scripts/data/hal/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.941355 mteb-1.4.1/scripts/data/imdb/
--rw-r--r--   0 root         (0) root         (0)      682 2024-04-01 14:19:04.000000 mteb-1.4.1/scripts/data/imdb/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.941355 mteb-1.4.1/scripts/data/medrxiv/
--rw-r--r--   0 root         (0) root         (0)     1780 2024-04-01 14:19:04.000000 mteb-1.4.1/scripts/data/medrxiv/script_clustering.py
--rw-r--r--   0 root         (0) root         (0)     1617 2024-04-01 14:19:04.000000 mteb-1.4.1/scripts/data/medrxiv/script_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.941355 mteb-1.4.1/scripts/data/mind/
--rw-r--r--   0 root         (0) root         (0)     1377 2024-04-01 14:19:04.000000 mteb-1.4.1/scripts/data/mind/prepare_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.941355 mteb-1.4.1/scripts/data/redditp2p/
--rw-r--r--   0 root         (0) root         (0)     1880 2024-04-01 14:19:04.000000 mteb-1.4.1/scripts/data/redditp2p/script_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.941355 mteb-1.4.1/scripts/data/stackexchangep2p/
--rw-r--r--   0 root         (0) root         (0)     1627 2024-04-01 14:19:04.000000 mteb-1.4.1/scripts/data/stackexchangep2p/script_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.941355 mteb-1.4.1/scripts/data/sts22-crosslingual-sts/
--rw-r--r--   0 root         (0) root         (0)     2436 2024-04-01 14:19:04.000000 mteb-1.4.1/scripts/data/sts22-crosslingual-sts/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.941355 mteb-1.4.1/scripts/data/summeval_fr/
--rw-r--r--   0 root         (0) root         (0)     1692 2024-04-01 14:19:04.000000 mteb-1.4.1/scripts/data/summeval_fr/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.941355 mteb-1.4.1/scripts/data/toxic_conversations_50k/
--rw-r--r--   0 root         (0) root         (0)     1151 2024-04-01 14:19:04.000000 mteb-1.4.1/scripts/data/toxic_conversations_50k/create_data.py
--rw-r--r--   0 root         (0) root         (0)     2516 2024-04-01 14:19:04.000000 mteb-1.4.1/scripts/merge_cqadupstack.py
--rw-r--r--   0 root         (0) root         (0)     5155 2024-04-01 14:19:04.000000 mteb-1.4.1/scripts/mteb_meta.py
--rw-r--r--   0 root         (0) root         (0)      673 2024-04-01 14:19:04.000000 mteb-1.4.1/scripts/run_mteb_chinese.py
--rw-r--r--   0 root         (0) root         (0)     2819 2024-04-01 14:19:04.000000 mteb-1.4.1/scripts/run_mteb_english.py
--rw-r--r--   0 root         (0) root         (0)     1852 2024-04-01 14:19:04.000000 mteb-1.4.1/scripts/run_mteb_french.py
--rw-r--r--   0 root         (0) root         (0)     1305 2024-04-01 14:19:04.000000 mteb-1.4.1/scripts/run_mteb_german.py
--rw-r--r--   0 root         (0) root         (0)     1033 2024-04-01 14:19:04.000000 mteb-1.4.1/scripts/run_mteb_korean.py
--rw-r--r--   0 root         (0) root         (0)      975 2024-04-01 14:19:04.000000 mteb-1.4.1/scripts/run_mteb_polish.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-01 14:19:08.945355 mteb-1.4.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 14:19:08.941355 mteb-1.4.1/tests/
--rw-r--r--   0 root         (0) root         (0)      632 2024-04-01 14:19:04.000000 mteb-1.4.1/tests/test_ClusteringEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1560 2024-04-01 14:19:04.000000 mteb-1.4.1/tests/test_PairClassificationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1130 2024-04-01 14:19:04.000000 mteb-1.4.1/tests/test_RerankingEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1113 2024-04-01 14:19:04.000000 mteb-1.4.1/tests/test_RetrievalEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1419 2024-04-01 14:19:04.000000 mteb-1.4.1/tests/test_all_abstasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.082607 mteb-1.5.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-04-02 17:03:33.000000 mteb-1.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    23581 2024-04-02 17:03:38.082607 mteb-1.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9190 2024-04-02 17:03:33.000000 mteb-1.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.026606 mteb-1.5.0/mteb/
+-rw-r--r--   0 root         (0) root         (0)     1917 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.030607 mteb-1.5.0/mteb/abstasks/
+-rw-r--r--   0 root         (0) root         (0)     1751 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/abstasks/AbsTask.py
+-rw-r--r--   0 root         (0) root         (0)     3063 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/abstasks/AbsTaskBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     5881 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/abstasks/AbsTaskClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2389 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/abstasks/AbsTaskClustering.py
+-rw-r--r--   0 root         (0) root         (0)     2542 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/abstasks/AbsTaskPairClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1120 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/abstasks/AbsTaskReranking.py
+-rw-r--r--   0 root         (0) root         (0)    11806 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/abstasks/AbsTaskRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2007 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/abstasks/AbsTaskSTS.py
+-rw-r--r--   0 root         (0) root         (0)     2296 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/abstasks/AbsTaskSummarization.py
+-rw-r--r--   0 root         (0) root         (0)      880 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/abstasks/CrosslingualTask.py
+-rw-r--r--   0 root         (0) root         (0)     2831 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/abstasks/LangMapping.py
+-rw-r--r--   0 root         (0) root         (0)      998 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/abstasks/MultilingualTask.py
+-rw-r--r--   0 root         (0) root         (0)     6391 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/abstasks/TaskMetadata.py
+-rw-r--r--   0 root         (0) root         (0)      422 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/abstasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5296 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/cmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.030607 mteb-1.5.0/mteb/evaluation/
+-rw-r--r--   0 root         (0) root         (0)    13078 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/evaluation/MTEB.py
+-rw-r--r--   0 root         (0) root         (0)       56 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/evaluation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.030607 mteb-1.5.0/mteb/evaluation/evaluators/
+-rw-r--r--   0 root         (0) root         (0)     5849 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/evaluation/evaluators/BitextMiningEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     8942 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/evaluation/evaluators/ClassificationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1463 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/evaluation/evaluators/ClusteringEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)      744 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/evaluation/evaluators/Evaluator.py
+-rw-r--r--   0 root         (0) root         (0)     7140 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/evaluation/evaluators/PairClassificationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     9613 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/evaluation/evaluators/RerankingEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)    12487 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/evaluation/evaluators/RetrievalEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     2394 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/evaluation/evaluators/STSEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     4841 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/evaluation/evaluators/SummarizationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)      324 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/evaluation/evaluators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5482 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/evaluation/evaluators/utils.py
+-rw-r--r--   0 root         (0) root         (0)      835 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.034607 mteb-1.5.0/mteb/tasks/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.034607 mteb-1.5.0/mteb/tasks/BitextMining/
+-rw-r--r--   0 root         (0) root         (0)      369 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/BitextMining/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.034607 mteb-1.5.0/mteb/tasks/BitextMining/da/
+-rw-r--r--   0 root         (0) root         (0)     1398 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/BitextMining/da/BornholmskBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/BitextMining/da/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.034607 mteb-1.5.0/mteb/tasks/BitextMining/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1076 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     2194 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     5780 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     1411 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     2797 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/BitextMining/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.034607 mteb-1.5.0/mteb/tasks/BitextMining/nb/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/BitextMining/nb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1351 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/BitextMining/nb/norwegian_courts_bitext_mining.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.034607 mteb-1.5.0/mteb/tasks/Classification/
+-rw-r--r--   0 root         (0) root         (0)     1232 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.034607 mteb-1.5.0/mteb/tasks/Classification/da/
+-rw-r--r--   0 root         (0) root         (0)     1316 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/da/AngryTweetsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1615 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/da/DKHateClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2505 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/da/DalajClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1610 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/da/DanishPoliticalCommentsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2937 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/da/DdiscoCohesionClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1255 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/da/LccSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/da/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.038607 mteb-1.5.0/mteb/tasks/Classification/en/
+-rw-r--r--   0 root         (0) root         (0)     1035 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/en/AmazonPolarityClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1048 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/en/Banking77Classification.py
+-rw-r--r--   0 root         (0) root         (0)     1368 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/en/EmotionClassification.py
+-rw-r--r--   0 root         (0) root         (0)      984 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/en/ImdbClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1400 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/en/ToxicConversationsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/en/TweetSentimentExtractionClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.038607 mteb-1.5.0/mteb/tasks/Classification/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1485 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1235 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1164 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1164 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1403 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1823 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1468 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/multilingual/NordicLangClassification.py
+-rw-r--r--   0 root         (0) root         (0)     6035 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/multilingual/ScalaClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.038607 mteb-1.5.0/mteb/tasks/Classification/nb/
+-rw-r--r--   0 root         (0) root         (0)     1110 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/nb/NoRecClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/nb/NorwegianParliamentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/nb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.042607 mteb-1.5.0/mteb/tasks/Classification/pl/
+-rw-r--r--   0 root         (0) root         (0)     4892 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/pl/PolishClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/pl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.042607 mteb-1.5.0/mteb/tasks/Classification/sv/
+-rw-r--r--   0 root         (0) root         (0)     1031 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/sv/SweRecClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/sv/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.042607 mteb-1.5.0/mteb/tasks/Classification/zh/
+-rw-r--r--   0 root         (0) root         (0)     6535 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/zh/CMTEBClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Classification/zh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.042607 mteb-1.5.0/mteb/tasks/Clustering/
+-rw-r--r--   0 root         (0) root         (0)     1249 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.042607 mteb-1.5.0/mteb/tasks/Clustering/de/
+-rw-r--r--   0 root         (0) root         (0)     1126 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/de/BlurbsClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1109 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/de/BlurbsClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1094 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/de/TenKGnadClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1074 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/de/TenKGnadClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/de/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.046607 mteb-1.5.0/mteb/tasks/Clustering/en/
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/en/ArxivClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1081 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/en/ArxivClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1122 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/en/BigPatentClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/en/BiorxivClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1055 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/en/BiorxivClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1066 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/en/MedrxivClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/en/MedrxivClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1096 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/en/RedditClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1085 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/en/RedditClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1121 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/en/StackExchangeClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1109 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/en/StackExchangeClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1078 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/en/TwentyNewsgroupsClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1129 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/en/WikiCitiesClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.046607 mteb-1.5.0/mteb/tasks/Clustering/es/
+-rw-r--r--   0 root         (0) root         (0)     1023 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/es/FloresClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1052 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/es/SpanishNewsClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/es/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.046607 mteb-1.5.0/mteb/tasks/Clustering/fr/
+-rw-r--r--   0 root         (0) root         (0)     1901 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/fr/AlloProfClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1747 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/fr/AlloProfClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1600 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/fr/HALClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1931 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/fr/MLSUMClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1746 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/fr/MLSUMClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/fr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.046607 mteb-1.5.0/mteb/tasks/Clustering/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     2494 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.046607 mteb-1.5.0/mteb/tasks/Clustering/nb/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/nb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3436 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/nb/snl_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     3590 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/nb/vg_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.046607 mteb-1.5.0/mteb/tasks/Clustering/pl/
+-rw-r--r--   0 root         (0) root         (0)     1129 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/pl/PolishClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/pl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.050607 mteb-1.5.0/mteb/tasks/Clustering/sv/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/sv/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3920 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/sv/swedn_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.050607 mteb-1.5.0/mteb/tasks/Clustering/zh/
+-rw-r--r--   0 root         (0) root         (0)     3585 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/zh/CMTEBClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Clustering/zh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.050607 mteb-1.5.0/mteb/tasks/PairClassification/
+-rw-r--r--   0 root         (0) root         (0)      301 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/PairClassification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.050607 mteb-1.5.0/mteb/tasks/PairClassification/en/
+-rw-r--r--   0 root         (0) root         (0)     1146 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/PairClassification/en/SprintDuplicateQuestionsPC.py
+-rw-r--r--   0 root         (0) root         (0)     1080 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/PairClassification/en/TwitterSemEval2015PC.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/PairClassification/en/TwitterURLCorpusPC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/PairClassification/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.050607 mteb-1.5.0/mteb/tasks/PairClassification/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     2687 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py
+-rw-r--r--   0 root         (0) root         (0)     1902 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/PairClassification/multilingual/PawsX.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/PairClassification/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.050607 mteb-1.5.0/mteb/tasks/PairClassification/pl/
+-rw-r--r--   0 root         (0) root         (0)     3442 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/PairClassification/pl/PolishPC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/PairClassification/pl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.050607 mteb-1.5.0/mteb/tasks/PairClassification/zh/
+-rw-r--r--   0 root         (0) root         (0)     1837 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/PairClassification/zh/CMTEBPairClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/PairClassification/zh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.050607 mteb-1.5.0/mteb/tasks/Reranking/
+-rw-r--r--   0 root         (0) root         (0)      339 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Reranking/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.054607 mteb-1.5.0/mteb/tasks/Reranking/en/
+-rw-r--r--   0 root         (0) root         (0)     1112 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Reranking/en/AskUbuntuDupQuestions.py
+-rw-r--r--   0 root         (0) root         (0)     1058 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Reranking/en/MindSmallReranking.py
+-rw-r--r--   0 root         (0) root         (0)     3010 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Reranking/en/SciDocsReranking.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Reranking/en/StackOverflowDupQuestions.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Reranking/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.054607 mteb-1.5.0/mteb/tasks/Reranking/fr/
+-rw-r--r--   0 root         (0) root         (0)     1173 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Reranking/fr/AlloprofReranking.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Reranking/fr/SyntecReranking.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Reranking/fr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.054607 mteb-1.5.0/mteb/tasks/Reranking/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1206 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Reranking/multilingual/MIRACLReranking.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Reranking/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.054607 mteb-1.5.0/mteb/tasks/Reranking/zh/
+-rw-r--r--   0 root         (0) root         (0)     3504 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Reranking/zh/CMTEBReranking.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Reranking/zh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.054607 mteb-1.5.0/mteb/tasks/Retrieval/
+-rw-r--r--   0 root         (0) root         (0)     2462 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.054607 mteb-1.5.0/mteb/tasks/Retrieval/da/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/da/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3788 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/da/dan_fever.py
+-rw-r--r--   0 root         (0) root         (0)     2577 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/da/t2nord_retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3142 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/da/twitterhjerne.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.054607 mteb-1.5.0/mteb/tasks/Retrieval/de/
+-rw-r--r--   0 root         (0) root         (0)     1997 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/de/GerDaLIRRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2896 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/de/GermanDPRRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2111 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/de/GermanQuADRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/de/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.062607 mteb-1.5.0/mteb/tasks/Retrieval/en/
+-rw-r--r--   0 root         (0) root         (0)     1005 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/ArguAnaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackAndroidRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackEnglishRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackGamingRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackGisRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackMathematicaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackPhysicsRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackProgrammersRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackStatsRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackTexRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1050 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackUnixRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1068 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackWebmastersRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackWordpressRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1089 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/ClimateFEVERRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/DBPediaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1169 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/FEVERRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      977 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/FiQA2018Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3699 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/HagridRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1145 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/HotpotQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1003 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/MSMARCORetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/MSMARCOv2Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1018 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/NFCorpusRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      993 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/NQRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2032 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/NarrativeQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1149 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/QuoraRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1108 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/SCIDOCSRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/SciFactRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/TRECCOVIDRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1003 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/Touche2020Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.062607 mteb-1.5.0/mteb/tasks/Retrieval/es/
+-rw-r--r--   0 root         (0) root         (0)     2117 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2P.py
+-rw-r--r--   0 root         (0) root         (0)     2119 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/es/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.062607 mteb-1.5.0/mteb/tasks/Retrieval/fr/
+-rw-r--r--   0 root         (0) root         (0)     2178 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/fr/AlloprofRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2456 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/fr/BSARDRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2164 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/fr/SyntecRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/fr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.062607 mteb-1.5.0/mteb/tasks/Retrieval/ko/
+-rw-r--r--   0 root         (0) root         (0)      900 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/ko/KoMiracl.py
+-rw-r--r--   0 root         (0) root         (0)      900 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/ko/KoMrtydi.py
+-rw-r--r--   0 root         (0) root         (0)      916 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/ko/KoStrategyQA.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/ko/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.066607 mteb-1.5.0/mteb/tasks/Retrieval/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     3248 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2905 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3250 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2921 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2925 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.066607 mteb-1.5.0/mteb/tasks/Retrieval/nb/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/nb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3946 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/nb/norquad.py
+-rw-r--r--   0 root         (0) root         (0)     2702 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/nb/snl_retrieval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.066607 mteb-1.5.0/mteb/tasks/Retrieval/pl/
+-rw-r--r--   0 root         (0) root         (0)      961 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/pl/ArguAnaPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/pl/DBPediaPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      978 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/pl/FiQAPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1106 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/pl/HotpotQAPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1003 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/pl/MSMARCOPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/pl/NFCorpusPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      991 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/pl/NQPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1157 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/pl/QuoraPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1085 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/pl/SCIDOCSPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/pl/SciFactPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1079 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/pl/TRECCOVIDPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/pl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.066607 mteb-1.5.0/mteb/tasks/Retrieval/sv/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/sv/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3213 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/sv/swedn_retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2613 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/sv/swefaq_retrieval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.070607 mteb-1.5.0/mteb/tasks/Retrieval/zh/
+-rw-r--r--   0 root         (0) root         (0)    10336 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/zh/CMTEBRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Retrieval/zh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.070607 mteb-1.5.0/mteb/tasks/STS/
+-rw-r--r--   0 root         (0) root         (0)      562 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.070607 mteb-1.5.0/mteb/tasks/STS/de/
+-rw-r--r--   0 root         (0) root         (0)     1364 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/de/GermanSTSBenchmarkSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/de/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.070607 mteb-1.5.0/mteb/tasks/STS/en/
+-rw-r--r--   0 root         (0) root         (0)     1178 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/en/BiossesSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/en/STS12STS.py
+-rw-r--r--   0 root         (0) root         (0)     1144 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/en/STS13STS.py
+-rw-r--r--   0 root         (0) root         (0)     1178 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/en/STS14STS.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/en/STS15STS.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/en/STS16STS.py
+-rw-r--r--   0 root         (0) root         (0)     1202 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/en/STSBenchmarkSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1187 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/en/SickrSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.070607 mteb-1.5.0/mteb/tasks/STS/es/
+-rw-r--r--   0 root         (0) root         (0)     1515 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/es/STSES.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/es/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.070607 mteb-1.5.0/mteb/tasks/STS/fr/
+-rw-r--r--   0 root         (0) root         (0)     1483 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/fr/SickFrSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/fr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.070607 mteb-1.5.0/mteb/tasks/STS/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1362 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1484 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)     2518 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.074607 mteb-1.5.0/mteb/tasks/STS/pl/
+-rw-r--r--   0 root         (0) root         (0)     2256 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/pl/PolishSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/pl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.074607 mteb-1.5.0/mteb/tasks/STS/zh/
+-rw-r--r--   0 root         (0) root         (0)     7080 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/zh/CMTEBSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/STS/zh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.074607 mteb-1.5.0/mteb/tasks/Summarization/
+-rw-r--r--   0 root         (0) root         (0)      122 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Summarization/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.074607 mteb-1.5.0/mteb/tasks/Summarization/en/
+-rw-r--r--   0 root         (0) root         (0)     1237 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Summarization/en/SummEvalSummarization.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Summarization/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.074607 mteb-1.5.0/mteb/tasks/Summarization/fr/
+-rw-r--r--   0 root         (0) root         (0)     1277 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Summarization/fr/SummEvalFrSummarization.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/Summarization/fr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      252 2024-04-02 17:03:33.000000 mteb-1.5.0/mteb/tasks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.082607 mteb-1.5.0/mteb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    23581 2024-04-02 17:03:37.000000 mteb-1.5.0/mteb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12579 2024-04-02 17:03:38.000000 mteb-1.5.0/mteb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 17:03:37.000000 mteb-1.5.0/mteb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-04-02 17:03:37.000000 mteb-1.5.0/mteb.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      234 2024-04-02 17:03:37.000000 mteb-1.5.0/mteb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-02 17:03:37.000000 mteb-1.5.0/mteb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2120 2024-04-02 17:03:34.000000 mteb-1.5.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.074607 mteb-1.5.0/scripts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.074607 mteb-1.5.0/scripts/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.074607 mteb-1.5.0/scripts/data/amazon_polarity/
+-rw-r--r--   0 root         (0) root         (0)      842 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/amazon_polarity/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.074607 mteb-1.5.0/scripts/data/amazon_reviews_multi/
+-rw-r--r--   0 root         (0) root         (0)     1379 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/amazon_reviews_multi/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.078607 mteb-1.5.0/scripts/data/arxiv/
+-rw-r--r--   0 root         (0) root         (0)     3146 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/arxiv/script_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/arxiv/script_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.078607 mteb-1.5.0/scripts/data/biorxiv/
+-rw-r--r--   0 root         (0) root         (0)     1781 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/biorxiv/script_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/biorxiv/script_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.078607 mteb-1.5.0/scripts/data/bucc/
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/bucc/create_data.py
+-rw-r--r--   0 root         (0) root         (0)     5929 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/create_task_table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.078607 mteb-1.5.0/scripts/data/germanquad/
+-rw-r--r--   0 root         (0) root         (0)     2132 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/germanquad/process_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.078607 mteb-1.5.0/scripts/data/hal/
+-rw-r--r--   0 root         (0) root         (0)     1512 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/hal/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.078607 mteb-1.5.0/scripts/data/imdb/
+-rw-r--r--   0 root         (0) root         (0)      682 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/imdb/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.078607 mteb-1.5.0/scripts/data/medrxiv/
+-rw-r--r--   0 root         (0) root         (0)     1780 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/medrxiv/script_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/medrxiv/script_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.078607 mteb-1.5.0/scripts/data/mind/
+-rw-r--r--   0 root         (0) root         (0)     1377 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/mind/prepare_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.078607 mteb-1.5.0/scripts/data/redditp2p/
+-rw-r--r--   0 root         (0) root         (0)     1880 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/redditp2p/script_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.078607 mteb-1.5.0/scripts/data/stackexchangep2p/
+-rw-r--r--   0 root         (0) root         (0)     1627 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/stackexchangep2p/script_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.078607 mteb-1.5.0/scripts/data/sts22-crosslingual-sts/
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/sts22-crosslingual-sts/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.078607 mteb-1.5.0/scripts/data/summeval_fr/
+-rw-r--r--   0 root         (0) root         (0)     1692 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/summeval_fr/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.078607 mteb-1.5.0/scripts/data/toxic_conversations_50k/
+-rw-r--r--   0 root         (0) root         (0)     1151 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/data/toxic_conversations_50k/create_data.py
+-rw-r--r--   0 root         (0) root         (0)     2516 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/merge_cqadupstack.py
+-rw-r--r--   0 root         (0) root         (0)     5217 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/mteb_meta.py
+-rw-r--r--   0 root         (0) root         (0)      673 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/run_mteb_chinese.py
+-rw-r--r--   0 root         (0) root         (0)     2819 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/run_mteb_english.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/run_mteb_french.py
+-rw-r--r--   0 root         (0) root         (0)     1305 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/run_mteb_german.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/run_mteb_korean.py
+-rw-r--r--   0 root         (0) root         (0)      975 2024-04-02 17:03:33.000000 mteb-1.5.0/scripts/run_mteb_polish.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 17:03:38.082607 mteb-1.5.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:03:38.082607 mteb-1.5.0/tests/
+-rw-r--r--   0 root         (0) root         (0)      632 2024-04-02 17:03:33.000000 mteb-1.5.0/tests/test_ClusteringEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1560 2024-04-02 17:03:33.000000 mteb-1.5.0/tests/test_PairClassificationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2024-04-02 17:03:33.000000 mteb-1.5.0/tests/test_RerankingEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1113 2024-04-02 17:03:33.000000 mteb-1.5.0/tests/test_RetrievalEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     3501 2024-04-02 17:03:33.000000 mteb-1.5.0/tests/test_TaskMetadata.py
+-rw-r--r--   0 root         (0) root         (0)     2137 2024-04-02 17:03:33.000000 mteb-1.5.0/tests/test_all_abstasks.py
```

### Comparing `mteb-1.4.1/LICENSE` & `mteb-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/PKG-INFO` & `mteb-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mteb
-Version: 1.4.1
+Version: 1.5.0
 Summary: Massive Text Embedding Benchmark
 Author-email: MTEB Contributors <niklas@huggingface.co>, nouamane@huggingface.co, info@nils-reimers.de
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `mteb-1.4.1/README.md` & `mteb-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/mteb/__init__.py` & `mteb-1.5.0/mteb/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/mteb/abstasks/AbsTask.py` & `mteb-1.5.0/mteb/abstasks/AbsTask.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,31 +22,35 @@
 
         self.seed = seed
         random.seed(self.seed)
         np.random.seed(self.seed)
         torch.manual_seed(self.seed)
         torch.cuda.manual_seed_all(self.seed)
 
+    def dataset_transform(self):
+        """
+        Transform operations applied to the dataset after loading.
+        Override this method if your dataset requires any transformation.
+        """
+        pass
+
     def load_data(self, **kwargs):
         """
         Load dataset from HuggingFace hub
         """
         if self.data_loaded:
             return
-
-        # TODO: add split argument
-        self.dataset = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            revision=self.metadata_dict.get("revision", None),
-        )
+        self.dataset = datasets.load_dataset(**self.metadata_dict["dataset"])
+        self.dataset_transform()
         self.data_loaded = True
 
     @property
     def metadata_dict(self) -> dict[str, str]:
-        return dict(self.metadata)
+        metadata_dict = dict(self.metadata)
+        return metadata_dict
 
     @abstractmethod
     def evaluate(self, model, split="test"):
         """
         Evaluates a Sentence Embedding Model on the task.
         Returns a dict (that can be serialized to json).
         :param model: Sentence embedding method. Implements a encode(sentences) method, that encodes sentences
```

### Comparing `mteb-1.4.1/mteb/abstasks/AbsTaskBitextMining.py` & `mteb-1.5.0/mteb/abstasks/AbsTaskBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/mteb/abstasks/AbsTaskClassification.py` & `mteb-1.5.0/mteb/abstasks/AbsTaskClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/mteb/abstasks/AbsTaskClustering.py` & `mteb-1.5.0/mteb/abstasks/AbsTaskClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/mteb/abstasks/AbsTaskPairClassification.py` & `mteb-1.5.0/mteb/abstasks/AbsTaskPairClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/mteb/abstasks/AbsTaskReranking.py` & `mteb-1.5.0/mteb/abstasks/AbsTaskReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/mteb/abstasks/AbsTaskRetrieval.py` & `mteb-1.5.0/mteb/abstasks/AbsTaskRetrieval.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,22 +214,21 @@
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
     def load_data(self, **kwargs):
         if self.data_loaded:
             return
         self.corpus, self.queries, self.relevant_docs = {}, {}, {}
+        dataset_path = self.metadata_dict["dataset"]["path"]
         hf_repo_qrels = (
-            self.metadata_dict["hf_hub_name"] + "-qrels"
-            if "clarin-knext" in self.metadata_dict["hf_hub_name"]
-            else None
+            dataset_path + "-qrels" if "clarin-knext" in dataset_path else None
         )
         for split in kwargs.get("eval_splits", self.metadata_dict["eval_splits"]):
             corpus, queries, qrels = HFDataLoader(
-                hf_repo=self.metadata_dict["hf_hub_name"],
+                hf_repo=dataset_path,
                 hf_repo_qrels=hf_repo_qrels,
                 streaming=False,
                 keep_in_memory=False,
             ).load(split=split)
             # Conversion from DataSet
             queries = {query["id"]: query["text"] for query in queries}
             corpus = {
```

### Comparing `mteb-1.4.1/mteb/abstasks/AbsTaskSTS.py` & `mteb-1.5.0/mteb/abstasks/AbsTaskSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/mteb/abstasks/AbsTaskSummarization.py` & `mteb-1.5.0/mteb/abstasks/AbsTaskSummarization.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/mteb/abstasks/CrosslingualTask.py` & `mteb-1.5.0/mteb/abstasks/CrosslingualTask.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,12 +21,10 @@
         Load dataset from HuggingFace hub
         """
         if self.data_loaded:
             return
         self.dataset = {}
         for lang in self.langs:
             self.dataset[lang] = datasets.load_dataset(
-                self.metadata_dict["hf_hub_name"],
-                lang,
-                revision=self.metadata_dict.get("revision", None),
+                name=lang, **self.metadata_dict["dataset"]
             )
         self.data_loaded = True
```

### Comparing `mteb-1.4.1/mteb/abstasks/LangMapping.py` & `mteb-1.5.0/mteb/abstasks/LangMapping.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/mteb/abstasks/MultilingualTask.py` & `mteb-1.5.0/mteb/abstasks/MultilingualTask.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,12 +23,11 @@
         Load dataset from HuggingFace hub
         """
         if self.data_loaded:
             return
         self.dataset = {}
         for lang in self.langs:
             self.dataset[lang] = datasets.load_dataset(
-                self.metadata_dict["hf_hub_name"],
-                lang,
-                revision=self.metadata_dict.get("revision", None),
+                name=lang,
+                **self.metadata_dict.get("dataset", None),
             )
         self.data_loaded = True
```

### Comparing `mteb-1.4.1/mteb/abstasks/TaskMetadata.py` & `mteb-1.5.0/mteb/abstasks/TaskMetadata.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from __future__ import annotations
 
+import logging
 from datetime import date
 
 from pydantic import (
     AnyUrl,
     BaseModel,
     BeforeValidator,
     TypeAdapter,
+    field_validator,
+    model_validator,
 )
 from typing_extensions import Annotated, Literal
 
 TASK_SUBTYPE = Literal[
     "Article retrieval",
     "Dialect pairing",
     "Dialog Systems",
@@ -87,21 +90,23 @@
 STR_DATE = Annotated[
     str, BeforeValidator(lambda value: str(pastdate_adapter.validate_python(value)))
 ]  # Allows the type to be a string, but ensures that the string is a valid date
 
 SPLIT_NAME = str
 
 
+logger = logging.getLogger(__name__)
+
+
 class TaskMetadata(BaseModel):
     """
     Metadata for a task.
 
     Args:
-        hf_hub_name: The name of the dataset for the task on the Hugging Face Hub.
-        revision: The revision of the dataset for the task on the Hugging Face Hub.
+        dataset: All arguments to pass to datasets.load_dataset to load the dataset for the task. Refer to https://huggingface.co/docs/datasets/v2.18.0/en/package_reference/loading_methods#datasets.load_dataset
         name: The name of the task.
         description: A description of the task.
         type: The type of the task. These includes "Classification", "Summarization", "STS", "Retrieval", "Reranking", "Clustering",
             "PairClassification", "BitextMining". The type should match the abstask type.
         category: The category of the task. E.g. includes "s2s", "s2p", "p2p" (s=sentence, p=paragraph).
         reference: A URL to the documentation of the task. E.g. a published paper.
         eval_splits: The splits of the dataset used for evaluation.
@@ -120,16 +125,15 @@
         text_creation: The method of text creation. Includes "found", "created", "machine-translated", "machine-translated and verified", and
             "machine-translated and localized".
         bibtex_citation: The BibTeX citation for the dataset.
         n_samples: The number of samples in the dataset. This should only be for the splits evaluated on.
         avg_character_length: The average character length of the samples in the dataset. This should only be for the splits evaluated on.
     """
 
-    hf_hub_name: str
-    revision: str
+    dataset: dict
 
     name: str
     description: str
     type: TASK_TYPE
     category: TASK_CATEGORY
     reference: STR_URL | None  # URL to documentation, e.g. published paper
 
@@ -148,7 +152,27 @@
     dialect: list[str] | None
 
     text_creation: TEXT_CREATION_METHOD | None
     bibtex_citation: str | None
 
     n_samples: dict[SPLIT_NAME, int] | None
     avg_character_length: dict[SPLIT_NAME, float] | None
+
+    @field_validator("dataset")
+    def _check_dataset_path_is_specified(cls, dataset):
+        """
+        This method checks that the dataset path is specified.
+        """
+        if "path" not in dataset or dataset["path"] is None:
+            raise ValueError(
+                "You must specify the path to the dataset in the dataset dictionary. "
+                "See https://huggingface.co/docs/datasets/main/en/package_reference/loading_methods#datasets.load_dataset"
+            )
+        return dataset
+
+    @field_validator("dataset")
+    def _check_dataset_revision_is_specified(cls, dataset):
+        if "revision" not in dataset:
+            raise ValueError("You must explicitly specify a revision for the dataset (either a SHA or None).")
+        if dataset["revision"] is None:
+            logging.warning("It is encourage to specify a dataset revision for reproducability")
+        return dataset
```

### Comparing `mteb-1.4.1/mteb/cmd.py` & `mteb-1.5.0/mteb/cmd.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/mteb/evaluation/MTEB.py` & `mteb-1.5.0/mteb/evaluation/MTEB.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,15 +300,15 @@
                 # load data
                 logger.info(f"Loading dataset for {task.metadata_dict['name']}")
                 task.load_data(eval_splits=task_eval_splits, **kwargs)
 
                 # run evaluation
                 task_results = {
                     "mteb_version": version("mteb"),  # noqa: F405
-                    "dataset_revision": task.metadata_dict.get("revision", None),
+                    "dataset_revision": task.metadata_dict["dataset"].get("revision", None),
                     "mteb_dataset_name": task.metadata_dict["name"],
                 }
                 for split in task_eval_splits:
                     tick = time()
                     results = task.evaluate(
                         model, split, output_folder=output_folder, **kwargs
                     )
```

### Comparing `mteb-1.4.1/mteb/evaluation/evaluators/BitextMiningEvaluator.py` & `mteb-1.5.0/mteb/evaluation/evaluators/BitextMiningEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/mteb/evaluation/evaluators/ClassificationEvaluator.py` & `mteb-1.5.0/mteb/evaluation/evaluators/ClassificationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/mteb/evaluation/evaluators/ClusteringEvaluator.py` & `mteb-1.5.0/mteb/evaluation/evaluators/ClusteringEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/mteb/evaluation/evaluators/Evaluator.py` & `mteb-1.5.0/mteb/evaluation/evaluators/Evaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/mteb/evaluation/evaluators/PairClassificationEvaluator.py` & `mteb-1.5.0/mteb/evaluation/evaluators/PairClassificationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/mteb/evaluation/evaluators/RerankingEvaluator.py` & `mteb-1.5.0/mteb/evaluation/evaluators/RerankingEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/mteb/evaluation/evaluators/RetrievalEvaluator.py` & `mteb-1.5.0/mteb/evaluation/evaluators/RetrievalEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/mteb/evaluation/evaluators/STSEvaluator.py` & `mteb-1.5.0/mteb/evaluation/evaluators/STSEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/mteb/evaluation/evaluators/SummarizationEvaluator.py` & `mteb-1.5.0/mteb/evaluation/evaluators/SummarizationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/mteb/evaluation/evaluators/utils.py` & `mteb-1.5.0/mteb/evaluation/evaluators/utils.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/mteb/logging.py` & `mteb-1.5.0/mteb/logging.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/mteb/tasks/BitextMining/da/BornholmskBitextMining.py` & `mteb-1.5.0/mteb/tasks/BitextMining/da/BornholmskBitextMining.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,38 @@
 from __future__ import annotations
 
-import datasets
-
 from mteb.abstasks import AbsTaskBitextMining
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 
 class BornholmBitextMining(AbsTaskBitextMining):
     metadata = TaskMetadata(
         name="BornholmBitextMining",
-        hf_hub_name="strombergnlp/bornholmsk_parallel",
+        dataset={
+            "path": "strombergnlp/bornholmsk_parallel",
+            "revision": "3bc5cfb4ec514264fe2db5615fac9016f7251552",
+        },
         description="Danish Bornholmsk Parallel Corpus. Bornholmsk is a Danish dialect spoken on the island of Bornholm, Denmark. Historically it is a part of east Danish which was also spoken in Scania and Halland, Sweden.",
         reference="https://aclanthology.org/W19-6138/",
         type="BitextMining",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["da", "da-bornholm"],
         main_score="f1",
-        revision="3bc5cfb4ec514264fe2db5615fac9016f7251552",
         date=None,
         form=None,
         domains=None,
         license=None,
         task_subtypes=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
         avg_character_length={"test": 89.7},
         n_samples={"test": 500},
     )
 
-    def load_data(self, **kwargs):
-        """
-        Load dataset from HuggingFace hub and convert it to the standard format.
-        """
-        if self.data_loaded:
-            return
-
-        self.dataset = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            revision=self.metadata_dict.get("revision", None),
-        )
-        self.dataset_transform()
-        self.data_loaded = True
-
     def dataset_transform(self):
         # Convert to standard format
         self.dataset = self.dataset.rename_column("da", "sentence1")
         self.dataset = self.dataset.rename_column("da_bornholm", "sentence2")
```

### Comparing `mteb-1.4.1/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py` & `mteb-1.5.0/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,23 +6,25 @@
 
 _LANGUAGES = ["de-en", "fr-en", "ru-en", "zh-en"]
 
 
 class BUCCBitextMining(AbsTaskBitextMining, CrosslingualTask):
     metadata = TaskMetadata(
         name="BUCC",
-        hf_hub_name="mteb/bucc-bitext-mining",
+        dataset={
+            "path": "mteb/bucc-bitext-mining",
+            "revision": "d51519689f32196a32af33b075a01d0e7c51e252",
+        },
         description="BUCC bitext mining dataset",
         reference="https://comparable.limsi.fr/bucc2018/bucc2018-task.html",
         type="BitextMining",
         category="s2s",
         eval_splits=["test"],
         eval_langs=_LANGUAGES,
         main_score="f1",
-        revision="d51519689f32196a32af33b075a01d0e7c51e252",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py` & `mteb-1.5.0/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2P.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from __future__ import annotations
 
 import datasets
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks import AbsTaskBitextMining, CrosslingualTask
+from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class DiaBLaBitextMining(AbsTaskBitextMining, CrosslingualTask):
+class SpanishPassageRetrievalS2P(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="DiaBlaBitextMining",
-        hf_hub_name="rbawden/DiaBLa",
-        description="English-French Parallel Corpus. DiaBLa is an English-French dataset for the evaluation of Machine Translation (MT) for informal, written bilingual dialogue.",
-        reference="https://inria.hal.science/hal-03021633",
-        type="BitextMining",
-        category="s2s",
+        name="SpanishPassageRetrievalS2P",
+        description="Test collection for passage retrieval from health-related Web resources in Spanish.",
+        reference="https://mklab.iti.gr/results/spanish-passage-retrieval-dataset/",
+        dataset={
+            "path": "jinaai/spanish_passage_retrieval",
+            "revision": "9cddf2ce5209ade52c2115ccfa00eb22c6d3a837",
+        },
+        type="Retrieval",
+        category="s2p",
         eval_splits=["test"],
-        eval_langs=["fr-en", "en-fr"],
-        main_score="f1",
-        revision="5345895c56a601afe1a98519ce3199be60a27dba",
+        eval_langs=["es"],
+        main_score="ndcg_at_10",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -30,38 +32,38 @@
         text_creation=None,
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
     def load_data(self, **kwargs):
-        """
-        Load dataset from HuggingFace hub and convert it to the standard format.
-        """
         if self.data_loaded:
             return
 
-        self.dataset = {}
-        for lang in self.langs:
-            self.dataset[lang] = datasets.load_dataset(
-                self.metadata_dict["hf_hub_name"],
-                revision=self.metadata_dict.get("revision", None),
-            )
+        # BUGFIX: the revision is now used
+        query_rows = datasets.load_dataset(
+            name="queries",
+            split="test",
+            trust_remote_code=True,
+        )
+        corpus_rows = datasets.load_dataset(
+            name="corpus.documents",
+            split="test",
+            trust_remote_code=True,
+            **self.metadata_dict["dataset"],
+        )
+        qrels_rows = datasets.load_dataset(
+            name="qrels.s2p",
+            split="test",
+            trust_remote_code=True,
+            **self.metadata_dict["dataset"],
+        )
+
+        self.queries = {"test": {row["_id"]: row["text"] for row in query_rows}}
+        self.corpus = {"test": {row["_id"]: row for row in corpus_rows}}
+        self.relevant_docs = {
+            "test": {
+                row["_id"]: {v: 1 for v in row["text"].split(" ")} for row in qrels_rows
+            }
+        }
 
-        self.dataset_transform()
         self.data_loaded = True
-
-    def dataset_transform(self):
-        def create_columns(row):
-            """Put all French texts in column 'sentence1' and English texts in 'sentence2' column"""
-            row["orig_lang"] = row["utterance_meta"]["lang"]
-            row["sentence1"] = (
-                row["orig"] if row["orig_lang"] == "french" else row["ref"]
-            )
-            row["sentence2"] = (
-                row["orig"] if not row["orig_lang"] == "french" else row["ref"]
-            )
-            return row
-
-        # Convert to standard format
-        for lang in self.langs:
-            self.dataset[lang] = self.dataset[lang].map(create_columns)
```

### Comparing `mteb-1.4.1/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py` & `mteb-1.5.0/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py`

 * *Files 5% similar despite different names*

```diff
@@ -231,23 +231,25 @@
 
 extend_lang_pairs()
 
 
 class FloresBitextMining(AbsTaskBitextMining, CrosslingualTask):
     metadata = TaskMetadata(
         name="FloresBitextMining",
-        hf_hub_name="facebook/flores",
+        dataset={
+            "path": "facebook/flores",
+            "revision": "80dc3040d19756742c9a18267ab30f54fb8e226b",
+        },
         description="FLORES is a benchmark dataset for machine translation between English and low-resource languages.",
         reference="https://huggingface.co/datasets/facebook/flores",
         type="BitextMining",
         category="s2s",
         eval_splits=_SPLIT,
         eval_langs=_LANGUAGES_PAIRS,
         main_score="f1",
-        revision="80dc3040d19756742c9a18267ab30f54fb8e226b",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -263,17 +265,16 @@
         Load dataset from HuggingFace hub
         """
         if self.data_loaded:
             return
         self.dataset = {}
         for lang in self.langs:
             self.dataset[lang] = datasets.load_dataset(
-                self.metadata_dict["hf_hub_name"],
-                lang,
-                revision=self.metadata_dict.get("revision", None),
+                name=lang,
+                **self.metadata_dict["dataset"],
             )
         self.dataset_transform()
         self.data_loaded = True
 
     def dataset_transform(self):
         # Convert to standard format
         for lang in self.langs:
```

### Comparing `mteb-1.4.1/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py` & `mteb-1.5.0/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,67 @@
 from __future__ import annotations
 
 import datasets
 
-from mteb.abstasks import AbsTaskBitextMining
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
+from ....abstasks import AbsTaskBitextMining, CrosslingualTask
 
-class NorwegianCourtsBitextMining(AbsTaskBitextMining):
+
+class DiaBLaBitextMining(AbsTaskBitextMining, CrosslingualTask):
     metadata = TaskMetadata(
-        name="NorwegianCourtsBitextMining",
-        hf_hub_name="kardosdrur/norwegian-courts",
-        description="Nynorsk and Bokmål parallel corpus from Norwegian courts. Norwegian courts have two standardised written languages. Bokmål is a variant closer to Danish, while Nynorsk was created to resemble regional dialects of Norwegian.",
-        reference="https://opus.nlpl.eu/index.php",
+        name="DiaBlaBitextMining",
+        dataset={
+            "path": "rbawden/DiaBLa",
+            "revision": "5345895c56a601afe1a98519ce3199be60a27dba",
+        },
+        description="English-French Parallel Corpus. DiaBLa is an English-French dataset for the evaluation of Machine Translation (MT) for informal, written bilingual dialogue.",
+        reference="https://inria.hal.science/hal-03021633",
         type="BitextMining",
         category="s2s",
         eval_splits=["test"],
-        eval_langs=["nb", "nn"],
+        eval_langs=["fr-en", "en-fr"],
         main_score="f1",
-        revision="d79af07e969a6678fcbbe819956840425816468f",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples={"test": 2050},
-        avg_character_length={"test": 1884.0},
+        n_samples=None,
+        avg_character_length=None,
     )
 
     def load_data(self, **kwargs):
         """
         Load dataset from HuggingFace hub and convert it to the standard format.
         """
         if self.data_loaded:
             return
 
-        self.dataset = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            revision=self.metadata_dict.get("revision", None),
-        )
+        self.dataset = {}
+
+        for lang in self.langs:
+            self.dataset[lang] = datasets.load_dataset(**self.metadata_dict["dataset"])
+
         self.dataset_transform()
         self.data_loaded = True
 
     def dataset_transform(self):
+        def create_columns(row):
+            """Put all French texts in column 'sentence1' and English texts in 'sentence2' column"""
+            row["orig_lang"] = row["utterance_meta"]["lang"]
+            row["sentence1"] = (
+                row["orig"] if row["orig_lang"] == "french" else row["ref"]
+            )
+            row["sentence2"] = (
+                row["orig"] if not row["orig_lang"] == "french" else row["ref"]
+            )
+            return row
+
         # Convert to standard format
-        self.dataset = self.dataset.rename_column("nb", "sentence1")
-        self.dataset = self.dataset.rename_column("nn", "sentence2")
+        for lang in self.langs:
+            self.dataset[lang] = self.dataset[lang].map(create_columns)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mteb-1.4.1/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py` & `mteb-1.5.0/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,23 +119,25 @@
     "wuu-eng",
 ]
 
 
 class TatoebaBitextMining(AbsTaskBitextMining, CrosslingualTask):
     metadata = TaskMetadata(
         name="Tatoeba",
-        hf_hub_name="mteb/tatoeba-bitext-mining",
+        dataset={
+            "path": "mteb/tatoeba-bitext-mining",
+            "revision": "9080400076fbadbb4c4dcb136ff4eddc40b42553",
+        },
         description="1,000 English-aligned sentence pairs for each language based on the Tatoeba corpus",
         reference="https://github.com/facebookresearch/LASER/tree/main/data/tatoeba/v1",
         type="BitextMining",
         category="s2s",
         eval_splits=["test"],
         eval_langs=_LANGUAGES,
         main_score="f1",
-        revision="9080400076fbadbb4c4dcb136ff4eddc40b42553",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/BitextMining/nb/norwegian_courts_bitext_mining.py` & `mteb-1.5.0/mteb/tasks/BitextMining/nb/norwegian_courts_bitext_mining.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,52 +1,36 @@
-from typing import Any
-
-import datasets
-
 from mteb.abstasks import AbsTaskBitextMining
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 
 class NorwegianCourtsBitextMining(AbsTaskBitextMining):
     metadata = TaskMetadata(
         name="NorwegianCourtsBitextMining",
-        hf_hub_name="kaedrodrur/norwegian-courts",
+        dataset={
+            "path": "kaedrodrur/norwegian-courts",
+            "revision": "d79af07e969a6678fcbbe819956840425816468f",
+        },
         description="Nynorsk and Bokmål parallel corpus from Norwegian courts. ",
         reference="https://opus.nlpl.eu/ELRC-Courts_Norway-v1.php",
         type="BitextMining",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["nb", "nn"],
         main_score="accuracy",
-        revision="d79af07e969a6678fcbbe819956840425816468f",
         date=("2000-01-01", "2020-12-31"),  # approximate guess
         form=["spoken"],
         domains=["Spoken"],
         task_subtypes=["Political classification"],
         license="openUnder-PSI",
         socioeconomic_status="high",
         annotations_creators="derived",  # best guess
         dialect=[],
         text_creation="found",
         bibtex_citation=None,
         n_samples={"test": 456},
         avg_character_length={"test": 82.11},
     )
 
-    def load_data(self, **kwargs: Any) -> None:  # noqa: ARG002
-        """
-        Load dataset from HuggingFace hub and convert it to the standard format.
-        """
-        if self.data_loaded:
-            return
-
-        self.dataset = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            revision=self.metadata_dict.get("revision", None),
-        )
-        self.dataset_transform()
-        self.data_loaded = True
-
     def dataset_transform(self) -> None:
         # Convert to standard format
         self.dataset = self.dataset.rename_column("nb", "sentence1")
         self.dataset = self.dataset.rename_column("nn", "sentence2")
```

### Comparing `mteb-1.4.1/mteb/tasks/Classification/__init__.py` & `mteb-1.5.0/mteb/tasks/Classification/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/mteb/tasks/Classification/da/AngryTweetsClassification.py` & `mteb-1.5.0/mteb/tasks/Classification/da/AngryTweetsClassification.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,23 +3,25 @@
 from mteb.abstasks.AbsTaskClassification import AbsTaskClassification
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 
 class AngryTweetsClassification(AbsTaskClassification):
     metadata = TaskMetadata(
         name="AngryTweetsClassification",
-        hf_hub_name="DDSC/angry-tweets",
+        dataset={
+            "path": "DDSC/angry-tweets",
+            "revision": "20b0e6081892e78179356fada741b7afa381443d",
+        },
         description="A sentiment dataset with 3 classes (positiv, negativ, neutral) for Danish tweets",
         reference="https://aclanthology.org/2021.nodalida-main.53/",
         type="Classification",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["da"],
         main_score="accuracy",
-        revision="20b0e6081892e78179356fada741b7afa381443d",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -28,11 +30,11 @@
         bibtex_citation=None,
         n_samples={"test": 1050},
         avg_character_length={"test": 156.1},
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
+        metadata_dict = super().metadata_dict
         metadata_dict["n_experiments"] = 10
         metadata_dict["samples_per_label"] = 16
         return metadata_dict
```

### Comparing `mteb-1.4.1/mteb/tasks/Classification/da/DKHateClassification.py` & `mteb-1.5.0/mteb/tasks/Classification/da/DKHateClassification.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from __future__ import annotations
 
-import datasets
-
 from mteb.abstasks.AbsTaskClassification import AbsTaskClassification
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 
 class DKHateClassification(AbsTaskClassification):
     metadata = TaskMetadata(
         name="DKHateClassification",
-        hf_hub_name="DDSC/dkhate",
+        dataset={
+            "path": "DDSC/dkhate",
+            "revision": "59d12749a3c91a186063c7d729ec392fda94681c",
+        },
         description="Danish Tweets annotated for Hate Speech either being Offensive or not",
         reference="https://aclanthology.org/2020.lrec-1.430/",
         type="Classification",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["da"],
         main_score="accuracy",
-        revision="59d12749a3c91a186063c7d729ec392fda94681c",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -35,28 +35,14 @@
     @property
     def metadata_dict(self) -> dict[str, str]:
         metadata_dict = dict(self.metadata)
         metadata_dict["n_experiments"] = 10
         metadata_dict["samples_per_label"] = 16
         return metadata_dict
 
-    def load_data(self, **kwargs):
-        """
-        Load dataset from HuggingFace hub
-        """
-        if self.data_loaded:
-            return
-
-        self.dataset = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            revision=self.metadata_dict.get("revision", None),
-        )
-        self.dataset_transform()
-        self.data_loaded = True
-
     def dataset_transform(self):
         # convert label to a 0/1 label
         labels = self.dataset["train"]["label"]  # type: ignore
         lab2idx = {lab: idx for idx, lab in enumerate(set(labels))}
         self.dataset = self.dataset.map(
             lambda x: {"label": lab2idx[x["label"]]}, remove_columns=["label"]
         )
```

### Comparing `mteb-1.4.1/mteb/tasks/Classification/da/DalajClassification.py` & `mteb-1.5.0/mteb/tasks/Classification/da/DalajClassification.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # SuperLIM tasks
 from __future__ import annotations
 
-import datasets
-
 from mteb.abstasks import AbsTaskClassification
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 
 class DalajClassification(AbsTaskClassification):
     metadata = TaskMetadata(
         name="DalajClassification",
-        hf_hub_name="AI-Sweden/SuperLim",
+        dataset={
+            "path": "AI-Sweden/SuperLim",
+            "revision": "7ebf0b4caa7b2ae39698a889de782c09e6f5ee56",
+            "name": "dalaj",
+        },
         description="A Swedish dataset for linguistic acceptability. Available as a part of Superlim.",
         reference="https://spraakbanken.gu.se/en/resources/superlim",
         type="Classification",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["da"],
         main_score="accuracy",
-        revision="7ebf0b4caa7b2ae39698a889de782c09e6f5ee56",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -31,34 +32,19 @@
         bibtex_citation=None,
         n_samples={"test": 444},
         avg_character_length={"test": 243.8},
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
+        metadata_dict = super().metadata_dict
         metadata_dict["n_experiments"] = 10
         metadata_dict["samples_per_label"] = 16
         return metadata_dict
 
-    def load_data(self, **kwargs):
-        """
-        Load dataset from HuggingFace hub
-        """
-        if self.data_loaded:
-            return
-
-        self.dataset = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            "dalaj",  # chose the relevant subset
-            revision=self.metadata_dict.get("revision"),
-        )
-        self.dataset_transform()
-        self.data_loaded = True
-
     def dataset_transform(self):
         """
         This dataset consist of two columns of relevance, "original_sentence" and "corrected_sentence".
         We will use the original sentence as we "wrong" sentence and the corrected sentence as the "correct" sentence
         """
 
         def __convert_sample_to_classification(sample):
```

### Comparing `mteb-1.4.1/mteb/tasks/Classification/da/DanishPoliticalCommentsClassification.py` & `mteb-1.5.0/mteb/tasks/Classification/da/DanishPoliticalCommentsClassification.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from __future__ import annotations
 
-import datasets
-
 from mteb.abstasks import AbsTaskClassification
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 
 class DanishPoliticalCommentsClassification(AbsTaskClassification):
     metadata = TaskMetadata(
         name="DanishPoliticalCommentsClassification",
-        hf_hub_name="danish_political_comments",
+        dataset={
+            "path": "danish_political_comments",
+            "revision": "edbb03726c04a0efab14fc8c3b8b79e4d420e5a1",
+        },
         description="A dataset of Danish political comments rated for sentiment",
         reference="https://huggingface.co/datasets/danish_political_comments",
         type="Classification",
         category="s2s",
         eval_splits=["train"],
         eval_langs=["da"],
         main_score="accuracy",
-        revision="edbb03726c04a0efab14fc8c3b8b79e4d420e5a1",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -35,27 +35,13 @@
     @property
     def metadata_dict(self) -> dict[str, str]:
         metadata_dict = dict(self.metadata)
         metadata_dict["n_experiments"] = 10
         metadata_dict["samples_per_label"] = 16
         return metadata_dict
 
-    def load_data(self, **kwargs):
-        """
-        Load dataset from HuggingFace hub
-        """
-        if self.data_loaded:
-            return
-
-        self.dataset = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            revision=self.metadata_dict.get("revision"),
-        )
-        self.dataset_transform()
-        self.data_loaded = True
-
     def dataset_transform(self):
         self.dataset = self.dataset.rename_column("sentence", "text")
         self.dataset = self.dataset.rename_column("target", "label")
 
         # create train and test splits
         self.dataset = self.dataset["train"].train_test_split(0.2, seed=self.seed)
```

### Comparing `mteb-1.4.1/mteb/tasks/Classification/da/DdiscoCohesionClassification.py` & `mteb-1.5.0/mteb/tasks/Classification/da/DdiscoCohesionClassification.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from __future__ import annotations
 
-from datasets import load_dataset
-
 from mteb.abstasks.AbsTaskClassification import AbsTaskClassification
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 
 class DdiscoCohesionClassification(AbsTaskClassification):
     metadata = TaskMetadata(
         name="Ddisco",
-        hf_hub_name="DDSC/ddisco",
+        dataset={
+            "path": "DDSC/ddisco",
+            "revision": "514ab557579fcfba538a4078d6d647248a0e6eb7",
+        },
         description="A Danish Discourse dataset with values for coherence and source (Wikipedia or Reddit)",
         reference="https://aclanthology.org/2022.lrec-1.260/",
         type="Classification",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["da"],
         main_score="accuracy",
-        revision="514ab557579fcfba538a4078d6d647248a0e6eb7",
         date=("2021-01-01", "2022-06-25"),
         form=["written"],
         domains=["Non-fiction", "Social"],
         dialect=[],
         task_subtypes=["Discourse coherence"],
         license="cc-by-sa-3.0",
         socioeconomic_status="high",
@@ -57,25 +57,11 @@
     abstract = "To date, there has been no resource for studying discourse coherence on real-world Danish texts. Discourse coherence has mostly been approached with the assumption that incoherent texts can be represented by coherent texts in which sentences have been shuffled. However, incoherent real-world texts rarely resemble that. We thus present DDisCo, a dataset including text from the Danish Wikipedia and Reddit annotated for discourse coherence. We choose to annotate real-world texts instead of relying on artificially incoherent text for training and testing models. Then, we evaluate the performance of several methods, including neural networks, on the dataset.",
 }
         """,
         n_samples=None,
         avg_character_length=None,
     )
 
-    def load_data(self, **kwargs):
-        """
-        Load dataset from HuggingFace hub
-        """
-        if self.data_loaded:
-            return
-
-        self.dataset = load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            revision=self.metadata_dict.get("revision"),
-        )
-        self.dataset_transform()
-        self.data_loaded = True
-
     def dataset_transform(self):
         self.dataset = self.dataset.rename_columns({"rating": "label"}).remove_columns(
             ["domain"]
         )
```

### Comparing `mteb-1.4.1/mteb/tasks/Classification/da/LccSentimentClassification.py` & `mteb-1.5.0/mteb/tasks/Classification/da/LccSentimentClassification.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,23 +3,25 @@
 from mteb.abstasks import AbsTaskClassification
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 
 class LccSentimentClassification(AbsTaskClassification):
     metadata = TaskMetadata(
         name="LccSentimentClassification",
-        hf_hub_name="DDSC/lcc",
+        dataset={
+            "path": "DDSC/lcc",
+            "revision": "de7ba3406ee55ea2cc52a0a41408fa6aede6d3c6",
+        },
         description="The leipzig corpora collection, annotated for sentiment",
         reference="https://github.com/fnielsen/lcc-sentiment",
         type="Classification",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["da"],
         main_score="accuracy",
-        revision="de7ba3406ee55ea2cc52a0a41408fa6aede6d3c6",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -28,11 +30,11 @@
         bibtex_citation=None,
         n_samples={"test": 150},
         avg_character_length={"test": 118.7},
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
+        metadata_dict = super().metadata_dict
         metadata_dict["n_experiments"] = 10
         metadata_dict["samples_per_label"] = 16
         return metadata_dict
```

### Comparing `mteb-1.4.1/mteb/tasks/Classification/en/AmazonPolarityClassification.py` & `mteb-1.5.0/mteb/tasks/Classification/en/AmazonPolarityClassification.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 
 
 class AmazonPolarityClassification(AbsTaskClassification):
     metadata = TaskMetadata(
         name="AmazonPolarityClassification",
         description="Amazon Polarity Classification Dataset.",
         reference="https://huggingface.co/datasets/amazon_polarity",
-        hf_hub_name="mteb/amazon_polarity",
+        dataset={
+            "path": "mteb/amazon_polarity",
+            "revision": "e2d317d38cd51312af73b3d32a06d1a08b442046",
+        },
         type="Classification",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="accuracy",
-        revision="e2d317d38cd51312af73b3d32a06d1a08b442046",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Classification/en/Banking77Classification.py` & `mteb-1.5.0/mteb/tasks/Classification/en/Banking77Classification.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 
 
 class Banking77Classification(AbsTaskClassification):
     metadata = TaskMetadata(
         name="Banking77Classification",
         description="Dataset composed of online banking queries annotated with their corresponding intents.",
         reference="https://arxiv.org/abs/2003.04807",
-        hf_hub_name="mteb/banking77",
+        dataset={
+            "path": "mteb/banking77",
+            "revision": "0fd18e25b25c072e09e0d92ab615fda904d66300",
+        },
         type="Classification",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="accuracy",
-        revision="0fd18e25b25c072e09e0d92ab615fda904d66300",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Classification/en/EmotionClassification.py` & `mteb-1.5.0/mteb/tasks/Classification/en/EmotionClassification.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 
 
 class EmotionClassification(AbsTaskClassification):
     metadata = TaskMetadata(
         name="EmotionClassification",
         description="Emotion is a dataset of English Twitter messages with six basic emotions: anger, fear, joy, love, sadness, and surprise.",
         reference="https://www.aclweb.org/anthology/D18-1404",
-        hf_hub_name="mteb/emotion",
+        dataset={
+            "path": "mteb/emotion",
+            "revision": "4f58c6b202a23cf9a4da393831edf4f9183cad37",
+        },
         type="Classification",
         category="s2s",
         eval_splits=["validation", "test"],
         eval_langs=["en"],
         main_score="accuracy",
-        revision="4f58c6b202a23cf9a4da393831edf4f9183cad37",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -29,11 +31,11 @@
         bibtex_citation=None,
         n_samples={"validation": 2000, "test": 2000},
         avg_character_length={"validation": 95.3, "test": 95.6},
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
+        metadata_dict = super().metadata_dict
         metadata_dict["n_experiments"] = 10
         metadata_dict["samples_per_label"] = 16
         return metadata_dict
```

### Comparing `mteb-1.4.1/mteb/tasks/Classification/en/ImdbClassification.py` & `mteb-1.5.0/mteb/tasks/Classification/nb/NoRecClassification.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from __future__ import annotations
 
+from mteb.abstasks import AbsTaskClassification
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks import AbsTaskClassification
 
-
-class ImdbClassification(AbsTaskClassification):
+class NoRecClassification(AbsTaskClassification):
     metadata = TaskMetadata(
-        name="ImdbClassification",
-        description="Large Movie Review Dataset",
-        hf_hub_name="mteb/imdb",
-        reference="http://www.aclweb.org/anthology/P11-1015",
+        name="NoRecClassification",
+        description="A Norwegian dataset for sentiment classification on review",
+        reference="https://aclanthology.org/L18-1661/",
+        dataset={
+            # using the mini version to keep results ~comparable to the ScandEval benchmark
+            "path": "ScandEval/norec-mini",
+            "revision": "07b99ab3363c2e7f8f87015b01c21f4d9b917ce3",
+        },
         type="Classification",
-        category="p2p",
+        category="s2s",
         eval_splits=["test"],
-        eval_langs=["en"],
+        eval_langs=["nb"],
         main_score="accuracy",
-        revision="3d86128a09e091d6018b6d26cad27f2739fc2db7",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples={"test": 25000},
-        avg_character_length={"test": 1293.8},
+        n_samples={"test": 2050},
+        avg_character_length={"test": 82},
     )
```

### Comparing `mteb-1.4.1/mteb/tasks/Classification/en/ToxicConversationsClassification.py` & `mteb-1.5.0/mteb/tasks/Classification/en/ToxicConversationsClassification.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 
 
 class ToxicConversationsClassification(AbsTaskClassification):
     metadata = TaskMetadata(
         name="ToxicConversationsClassification",
         description="Collection of comments from the Civil Comments platform together with annotations if the comment is toxic or not.",
         reference="https://www.kaggle.com/competitions/jigsaw-unintended-bias-in-toxicity-classification/overview",
-        hf_hub_name="mteb/toxic_conversations_50k",
+        dataset={
+            "path": "mteb/toxic_conversations_50k",
+            "revision": "edfaf9da55d3dd50d43143d90c1ac476895ae6de",
+        },
         type="Classification",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="accuracy",
-        revision="edfaf9da55d3dd50d43143d90c1ac476895ae6de",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -29,11 +31,11 @@
         bibtex_citation=None,
         n_samples={"test": 50000},
         avg_character_length={"test": 296.6},
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
+        metadata_dict = super().metadata_dict
         metadata_dict["n_experiments"] = 10
         metadata_dict["samples_per_label"] = 16
-        return dict(self.metadata)
+        return metadata_dict
```

### Comparing `mteb-1.4.1/mteb/tasks/Classification/en/TweetSentimentExtractionClassification.py` & `mteb-1.5.0/mteb/tasks/Classification/en/TweetSentimentExtractionClassification.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 
 
 class TweetSentimentExtractionClassification(AbsTaskClassification):
     metadata = TaskMetadata(
         name="TweetSentimentExtractionClassification",
         description="",
         reference="https://www.kaggle.com/competitions/tweet-sentiment-extraction/overview",
-        hf_hub_name="mteb/tweet_sentiment_extraction",
+        dataset={
+            "path": "mteb/tweet_sentiment_extraction",
+            "revision": "d604517c81ca91fe16a244d1248fc021f9ecee7a",
+        },
         type="Classification",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="accuracy",
-        revision="d604517c81ca91fe16a244d1248fc021f9ecee7a",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py` & `mteb-1.5.0/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,36 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks import AbsTaskClassification, MultilingualTask
 
-_LANGUAGES = ["en", "de", "en-ext", "ja"]
+_LANGUAGES = ["en", "de", "es", "fr", "ja", "zh"]
 
 
-class AmazonCounterfactualClassification(MultilingualTask, AbsTaskClassification):
+class AmazonReviewsClassification(MultilingualTask, AbsTaskClassification):
     metadata = TaskMetadata(
-        name="AmazonCounterfactualClassification",
-        hf_hub_name="mteb/amazon_counterfactual",
-        description=(
-            "A collection of Amazon customer reviews annotated for counterfactual detection pair classification."
-        ),
-        reference="https://arxiv.org/abs/2104.06893",
+        name="AmazonReviewsClassification",
+        dataset={
+            "path": "mteb/amazon_reviews_multi",
+            "revision": "1399c76144fd37290681b995c656ef9b2e06e26d",
+        },
+        description="A collection of Amazon reviews specifically designed to aid research in multilingual text classification.",
+        reference="https://arxiv.org/abs/2010.02573",
         category="s2s",
         type="Classification",
         eval_splits=["validation", "test"],
         eval_langs=_LANGUAGES,
         main_score="accuracy",
-        revision="e8379541af4e31359cca9fbcf4b00f2671dba205",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples={"validation": 335, "test": 670},
-        avg_character_length={"validation": 109.2, "test": 106.1},
+        n_samples={"validation": 30000, "test": 30000},
+        avg_character_length={"validation": 159.2, "test": 160.4},
     )
-
-    @property
-    def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
-        metadata_dict["n_experiments"] = 10
-        metadata_dict["samples_per_label"] = 32
-        return metadata_dict
```

### Comparing `mteb-1.4.1/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py` & `mteb-1.5.0/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks import AbsTaskClassification, MultilingualTask
 
-_LANGUAGES = ["en", "de", "es", "fr", "ja", "zh"]
+_LANGUAGES = ["en", "de", "es", "fr", "hi", "th"]
 
 
-class AmazonReviewsClassification(MultilingualTask, AbsTaskClassification):
+class MTOPIntentClassification(MultilingualTask, AbsTaskClassification):
     metadata = TaskMetadata(
-        name="AmazonReviewsClassification",
-        hf_hub_name="mteb/amazon_reviews_multi",
-        description="A collection of Amazon reviews specifically designed to aid research in multilingual text classification.",
-        reference="https://arxiv.org/abs/2010.02573",
+        name="MTOPIntentClassification",
+        dataset={
+            "path": "mteb/mtop_intent",
+            "revision": "ae001d0e6b1228650b7bd1c2c65fb50ad11a8aba",
+        },
+        description="MTOP: Multilingual Task-Oriented Semantic Parsing",
+        reference="https://arxiv.org/pdf/2008.09335.pdf",
         category="s2s",
         type="Classification",
         eval_splits=["validation", "test"],
         eval_langs=_LANGUAGES,
         main_score="accuracy",
-        revision="1399c76144fd37290681b995c656ef9b2e06e26d",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples={"validation": 30000, "test": 30000},
-        avg_character_length={"validation": 159.2, "test": 160.4},
+        n_samples={"validation": 2235, "test": 4386},
+        avg_character_length={"validation": 36.5, "test": 36.8},
     )
```

### Comparing `mteb-1.4.1/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py` & `mteb-1.5.0/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,23 +6,25 @@
 
 _LANGUAGES = ["en", "de", "es", "fr", "hi", "th"]
 
 
 class MTOPDomainClassification(MultilingualTask, AbsTaskClassification):
     metadata = TaskMetadata(
         name="MTOPDomainClassification",
-        hf_hub_name="mteb/mtop_domain",
+        dataset={
+            "path": "mteb/mtop_domain",
+            "revision": "d80d48c1eb48d3562165c59d59d0034df9fff0bf",
+        },
         description="MTOP: Multilingual Task-Oriented Semantic Parsing",
         reference="https://arxiv.org/pdf/2008.09335.pdf",
         category="s2s",
         type="Classification",
         eval_splits=["validation", "test"],
         eval_langs=_LANGUAGES,
         main_score="accuracy",
-        revision="d80d48c1eb48d3562165c59d59d0034df9fff0bf",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py` & `mteb-1.5.0/mteb/tasks/PairClassification/en/TwitterURLCorpusPC.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks import AbsTaskClassification, MultilingualTask
+from ....abstasks.AbsTaskPairClassification import AbsTaskPairClassification
 
-_LANGUAGES = ["en", "de", "es", "fr", "hi", "th"]
 
-
-class MTOPIntentClassification(MultilingualTask, AbsTaskClassification):
+class TwitterURLCorpusPC(AbsTaskPairClassification):
     metadata = TaskMetadata(
-        name="MTOPIntentClassification",
-        hf_hub_name="mteb/mtop_intent",
-        description="MTOP: Multilingual Task-Oriented Semantic Parsing",
-        reference="https://arxiv.org/pdf/2008.09335.pdf",
+        name="TwitterURLCorpus",
+        dataset={
+            "path": "mteb/twitterurlcorpus-pairclassification",
+            "revision": "8b6510b0b1fa4e4c4f879467980e9be563ec1cdf",
+        },
+        description="Paraphrase-Pairs of Tweets.",
+        reference="https://languagenet.github.io/",
         category="s2s",
-        type="Classification",
-        eval_splits=["validation", "test"],
-        eval_langs=_LANGUAGES,
-        main_score="accuracy",
-        revision="ae001d0e6b1228650b7bd1c2c65fb50ad11a8aba",
+        type="PairClassification",
+        eval_splits=["test"],
+        eval_langs=["en"],
+        main_score="ap",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples={"validation": 2235, "test": 4386},
-        avg_character_length={"validation": 36.5, "test": 36.8},
+        n_samples={"test": 51534},
+        avg_character_length={"test": 79.5},
     )
```

### Comparing `mteb-1.4.1/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py` & `mteb-1.5.0/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,23 +23,25 @@
     "yor",
 ]
 
 
 class MasakhaNEWSClassification(AbsTaskClassification, MultilingualTask):
     metadata = TaskMetadata(
         name="MasakhaNEWSClassification",
-        hf_hub_name="masakhane/masakhanews",
+        dataset={
+            "path": "masakhane/masakhanews",
+            "revision": "8ccc72e69e65f40c70e117d8b3c08306bb788b60",
+        },
         description="MasakhaNEWS is the largest publicly available dataset for news topic classification in 16 languages widely spoken in Africa. The train/validation/test sets are available for all the 16 languages.",
         reference="https://arxiv.org/abs/2304.09972",
         category="s2s",
         type="Classification",
         eval_splits=["test"],
         eval_langs=_LANGUAGES,
         main_score="accuracy",
-        revision="8ccc72e69e65f40c70e117d8b3c08306bb788b60",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py` & `mteb-1.5.0/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,23 +58,25 @@
     "zh-TW",
 ]
 
 
 class MassiveIntentClassification(MultilingualTask, AbsTaskClassification):
     metadata = TaskMetadata(
         name="MassiveIntentClassification",
-        hf_hub_name="mteb/amazon_massive_intent",
+        dataset={
+            "path": "mteb/amazon_massive_intent",
+            "revision": "31efe3c427b0bae9c22cbb560b8f15491cc6bed7",
+        },
         description="MASSIVE: A 1M-Example Multilingual Natural Language Understanding Dataset with 51 Typologically-Diverse Languages",
         reference="https://arxiv.org/abs/2204.08582#:~:text=MASSIVE%20contains%201M%20realistic%2C%20parallel,diverse%20languages%20from%2029%20genera.",
         category="s2s",
         type="Classification",
         eval_splits=["validation", "test"],
         eval_langs=_LANGUAGES,
         main_score="accuracy",
-        revision="31efe3c427b0bae9c22cbb560b8f15491cc6bed7",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py` & `mteb-1.5.0/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py`

 * *Files 11% similar despite different names*

```diff
@@ -58,23 +58,25 @@
     "zh-TW",
 ]
 
 
 class MassiveScenarioClassification(MultilingualTask, AbsTaskClassification):
     metadata = TaskMetadata(
         name="MassiveScenarioClassification",
-        hf_hub_name="mteb/amazon_massive_scenario",
+        dataset={
+            "path": "mteb/amazon_massive_scenario",
+            "revision": "7d571f92784cd94a019292a1f45445077d0ef634",
+        },
         description="MASSIVE: A 1M-Example Multilingual Natural Language Understanding Dataset with 51 Typologically-Diverse Languages",
         reference="https://arxiv.org/abs/2204.08582#:~:text=MASSIVE%20contains%201M%20realistic%2C%20parallel,diverse%20languages%20from%2029%20genera.",
         category="s2s",
         type="Classification",
         eval_splits=["validation", "test"],
         eval_langs=_LANGUAGES,
         main_score="accuracy",
-        revision="7d571f92784cd94a019292a1f45445077d0ef634",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Classification/multilingual/NordicLangClassification.py` & `mteb-1.5.0/mteb/tasks/Classification/multilingual/NordicLangClassification.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from __future__ import annotations
 
-import datasets
-
 from mteb.abstasks import AbsTaskClassification
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 
 class NordicLangClassification(AbsTaskClassification):
     metadata = TaskMetadata(
         name="NordicLangClassification",
         description="A dataset for Nordic language identification.",
         reference="https://aclanthology.org/2021.vardial-1.8/",
-        hf_hub_name="strombergnlp/nordic_langid",
+        dataset={
+            "path": "strombergnlp/nordic_langid",
+            "revision": "e254179d18ab0165fdb6dbef91178266222bee2a",
+            "name": "10k",
+        },
         type="Classification",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["no", "nn"],
         main_score="accuracy",
-        revision="e254179d18ab0165fdb6dbef91178266222bee2a",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -30,30 +31,15 @@
         bibtex_citation=None,
         n_samples={"test": 3000},
         avg_character_length={"test": 78.2},
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
+        metadata_dict = super().metadata_dict
         metadata_dict["n_experiments"] = 10
         metadata_dict["samples_per_label"] = 32
         return metadata_dict
 
-    def load_data(self, **kwargs):
-        """
-        Load dataset from HuggingFace hub
-        """
-        if self.data_loaded:
-            return
-
-        self.dataset = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            "10k",
-            revision=self.metadata_dict.get("revision"),  # select relevant subset
-        )
-        self.dataset_transform()
-        self.data_loaded = True
-
     def dataset_transform(self):
         self.dataset = self.dataset.rename_column("sentence", "text")
         self.dataset = self.dataset.rename_column("language", "label")
```

### Comparing `mteb-1.4.1/mteb/tasks/Classification/multilingual/ScalaClassification.py` & `mteb-1.5.0/mteb/tasks/Classification/multilingual/ScalaClassification.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from __future__ import annotations
 
-import datasets
-
 from mteb.abstasks import AbsTaskClassification
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 
 class ScalaDaClassification(AbsTaskClassification):
     metadata = TaskMetadata(
         name="ScalaDaClassification",
         description="A modified version of DDT modified for linguistic acceptability classification",
         reference="https://aclanthology.org/2023.nodalida-1.20/",
-        hf_hub_name="ScandEval/scala-da",
+        dataset={
+            "path": "ScandEval/scala-da",
+            "revision": "1de08520a7b361e92ffa2a2201ebd41942c54675",
+        },
         type="Classification",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["da"],
         main_score="accuracy",
-        revision="1de08520a7b361e92ffa2a2201ebd41942c54675",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -30,54 +30,42 @@
         bibtex_citation=None,
         n_samples={"test": 1024},
         avg_character_length={"test": 109.4},
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
+        metadata_dict = super().metadata_dict
         metadata_dict["n_experiments"] = 10
         metadata_dict["samples_per_label"] = 32
         return metadata_dict
 
-    def load_data(self, **kwargs):
-        """
-        Load dataset from HuggingFace hub
-        """
-        if self.data_loaded:
-            return
-
-        self.dataset = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            revision=self.metadata_dict.get("revision", None),
-        )
-        self.dataset_transform()
-        self.data_loaded = True
-
     def dataset_transform(self):
         # convert label to a 0/1 label
         labels = self.dataset["train"]["label"]  # type: ignore
         lab2idx = {lab: idx for idx, lab in enumerate(set(labels))}
         self.dataset = self.dataset.map(
             lambda x: {"label": lab2idx[x["label"]]}, remove_columns=["label"]
         )
 
 
 class ScalaNbClassification(AbsTaskClassification):
     metadata = TaskMetadata(
         name="ScalaNbClassification",
         description="A Norwegian dataset for linguistic acceptability classification for Bokmål",
         reference="https://aclanthology.org/2023.nodalida-1.20/",
-        hf_hub_name="ScandEval/scala-nb",
+        dataset={
+            "path": "ScandEval/scala-nb",
+            "revision": "237111a078ad5a834a55c57803d40bbe410ed03b",
+        },
         type="Classification",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["nb"],
         main_score="accuracy",
-        revision="237111a078ad5a834a55c57803d40bbe410ed03b",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -86,32 +74,18 @@
         bibtex_citation=None,
         n_samples={"test": 1024},
         avg_character_length={"test": 98.4},
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
+        metadata_dict = super().metadata_dict
         metadata_dict["n_experiments"] = 10
         metadata_dict["samples_per_label"] = 32
-        return dict(self.metadata)
-
-    def load_data(self, **kwargs):
-        """
-        Load dataset from HuggingFace hub
-        """
-        if self.data_loaded:
-            return
-
-        self.dataset = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            revision=self.metadata_dict.get("revision", None),
-        )
-        self.dataset_transform()
-        self.data_loaded = True
+        return metadata_dict
 
     def dataset_transform(self):
         # convert label to a 0/1 label
         labels = self.dataset["train"]["label"]  # type: ignore
         lab2idx = {lab: idx for idx, lab in enumerate(set(labels))}
         self.dataset = self.dataset.map(
             lambda x: {"label": lab2idx[x["label"]]}, remove_columns=["label"]
@@ -119,21 +93,23 @@
 
 
 class ScalaNnClassification(AbsTaskClassification):
     metadata = TaskMetadata(
         name="ScalaNnClassification",
         description="A Norwegian dataset for linguistic acceptability classification for Nynorsk",
         reference="https://aclanthology.org/2023.nodalida-1.20/",
-        hf_hub_name="ScandEval/scala-nn",
+        dataset={
+            "path": "ScandEval/scala-nn",
+            "revision": "9d9a2a4092ed3cacf0744592f6d2f32ab8ef4c0b",
+        },
         type="Classification",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["nn"],
         main_score="accuracy",
-        revision="9d9a2a4092ed3cacf0744592f6d2f32ab8ef4c0b",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -142,54 +118,42 @@
         bibtex_citation=None,
         n_samples={"test": 1024},
         avg_character_length={"test": 104.8},
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
+        metadata_dict = super().metadata_dict
         metadata_dict["n_experiments"] = 10
         metadata_dict["samples_per_label"] = 32
         return metadata_dict
 
-    def load_data(self, **kwargs):
-        """
-        Load dataset from HuggingFace hub
-        """
-        if self.data_loaded:
-            return
-
-        self.dataset = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            revision=self.metadata_dict.get("revision", None),
-        )
-        self.dataset_transform()
-        self.data_loaded = True
-
     def dataset_transform(self):
         # convert label to a 0/1 label
         labels = self.dataset["train"]["label"]  # type: ignore
         lab2idx = {lab: idx for idx, lab in enumerate(set(labels))}
         self.dataset = self.dataset.map(
             lambda x: {"label": lab2idx[x["label"]]}, remove_columns=["label"]
         )
 
 
 class ScalaSvClassification(AbsTaskClassification):
     metadata = TaskMetadata(
         name="ScalaSvClassification",
         description="A Swedish dataset for linguistic acceptability classification",
         reference="https://aclanthology.org/2023.nodalida-1.20/",
-        hf_hub_name="ScandEval/scala-sv",
+        dataset={
+            "path": "ScandEval/scala-sv",
+            "revision": "1b48e3dcb02872335ff985ff938a054a4ed99008",
+        },
         type="Classification",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["sv"],
         main_score="accuracy",
-        revision="1b48e3dcb02872335ff985ff938a054a4ed99008",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -198,33 +162,19 @@
         bibtex_citation=None,
         n_samples={"test": 1024},
         avg_character_length={"test": 98.3},
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
+        metadata_dict = super().metadata_dict
         metadata_dict["n_experiments"] = 10
         metadata_dict["samples_per_label"] = 32
         return metadata_dict
 
-    def load_data(self, **kwargs):
-        """
-        Load dataset from HuggingFace hub
-        """
-        if self.data_loaded:
-            return
-
-        self.dataset = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            revision=self.metadata_dict.get("revision", None),
-        )
-        self.dataset_transform()
-        self.data_loaded = True
-
     def dataset_transform(self):
         # convert label to a 0/1 label
         labels = self.dataset["train"]["label"]  # type: ignore
         lab2idx = {lab: idx for idx, lab in enumerate(set(labels))}
         self.dataset = self.dataset.map(
             lambda x: {"label": lab2idx[x["label"]]}, remove_columns=["label"]
         )
```

### Comparing `mteb-1.4.1/mteb/tasks/Classification/nb/NoRecClassification.py` & `mteb-1.5.0/mteb/tasks/Retrieval/pl/NQPLRetrieval.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 from __future__ import annotations
 
-from mteb.abstasks import AbsTaskClassification
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
+from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
-class NoRecClassification(AbsTaskClassification):
+
+class NQPL(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="NoRecClassification",
-        description="A Norwegian dataset for sentiment classification on review",
-        reference="https://aclanthology.org/L18-1661/",
-        hf_hub_name="ScandEval/norec-mini",  # using the mini version to keep results ~comparable to the ScandEval benchmark
-        type="Classification",
-        category="s2s",
+        name="NQ-PL",
+        description="Natural Questions: A Benchmark for Question Answering Research",
+        reference="https://ai.google.com/research/NaturalQuestions/",
+        dataset={
+            "path": "clarin-knext/nq-pl",
+            "revision": "f171245712cf85dd4700b06bef18001578d0ca8d",
+        },
+        type="Retrieval",
+        category="s2p",
         eval_splits=["test"],
-        eval_langs=["nb"],
-        main_score="accuracy",
-        revision="07b99ab3363c2e7f8f87015b01c21f4d9b917ce3",
+        eval_langs=["pl"],
+        main_score="ndcg_at_10",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples={"test": 2050},
-        avg_character_length={"test": 82},
+        n_samples=None,
+        avg_character_length=None,
     )
```

### Comparing `mteb-1.4.1/mteb/tasks/Classification/nb/NorwegianParliamentClassification.py` & `mteb-1.5.0/mteb/tasks/Classification/nb/NorwegianParliamentClassification.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 
 
 class NorwegianParliamentClassification(AbsTaskClassification):
     metadata = TaskMetadata(
         name="NorwegianParliamentClassification",
         description="Norwegian parliament speeches annotated for sentiment",
         reference="https://huggingface.co/datasets/NbAiLab/norwegian_parliament",
-        hf_hub_name="NbAiLab/norwegian_parliament",
+        dataset={
+            "path": "NbAiLab/norwegian_parliament",
+            "revision": "f7393532774c66312378d30b197610b43d751972",
+        },
         type="Classification",
         category="s2s",
         eval_splits=["test", "validation"],
         eval_langs=["nb"],  # assumed to be bokmål
         main_score="accuracy",
-        revision="f7393532774c66312378d30b197610b43d751972",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Classification/pl/PolishClassification.py` & `mteb-1.5.0/mteb/tasks/Classification/pl/PolishClassification.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 
 
 class CbdClassification(AbsTaskClassification):
     metadata = TaskMetadata(
         name="CBD",
         description="Polish Tweets annotated for cyberbullying detection.",
         reference="http://2019.poleval.pl/files/poleval2019.pdf",
-        hf_hub_name="PL-MTEB/cbd",
+        dataset={
+            "path": "PL-MTEB/cbd",
+            "revision": "59d12749a3c91a186063c7d729ec392fda94681c",
+        },
         type="Classification",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["pl"],
         main_score="accuracy",
-        revision="59d12749a3c91a186063c7d729ec392fda94681c",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -34,21 +36,23 @@
 
 class PolEmo2InClassification(AbsTaskClassification):
     metadata = TaskMetadata(
         name="PolEmo2.0-IN",
         description="A collection of Polish online reviews from four domains: medicine, hotels, products and "
         "school. The PolEmo2.0-IN task is to predict the sentiment of in-domain (medicine and hotels) reviews.",
         reference="https://aclanthology.org/K19-1092.pdf",
-        hf_hub_name="PL-MTEB/polemo2_in",
+        dataset={
+            "path": "PL-MTEB/polemo2_in",
+            "revision": "9e9b1f8ef51616073f47f306f7f47dd91663f86a",
+        },
         type="Classification",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["pl"],
         main_score="accuracy",
-        revision="9e9b1f8ef51616073f47f306f7f47dd91663f86a",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -63,21 +67,23 @@
 class PolEmo2OutClassification(AbsTaskClassification):
     metadata = TaskMetadata(
         name="PolEmo2.0-OUT",
         description="A collection of Polish online reviews from four domains: medicine, hotels, products and "
         "school. The PolEmo2.0-OUT task is to predict the sentiment of out-of-domain (products and "
         "school) reviews using models train on reviews from medicine and hotels domains.",
         reference="https://aclanthology.org/K19-1092.pdf",
-        hf_hub_name="PL-MTEB/polemo2_out",
+        dataset={
+            "path": "PL-MTEB/polemo2_out",
+            "revision": "c99d599f0a6ab9b85b065da6f9d94f9cf731679f",
+        },
         type="Classification",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["pl"],
         main_score="accuracy",
-        revision="c99d599f0a6ab9b85b065da6f9d94f9cf731679f",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -90,21 +96,23 @@
 
 
 class AllegroReviewsClassification(AbsTaskClassification):
     metadata = TaskMetadata(
         name="AllegroReviews",
         description="A Polish dataset for sentiment classification on reviews from e-commerce marketplace Allegro.",
         reference="https://aclanthology.org/2020.acl-main.111.pdf",
-        hf_hub_name="PL-MTEB/allegro-reviews",
+        dataset={
+            "path": "PL-MTEB/allegro-reviews",
+            "revision": "477b8bd4448b5ef8ed01ba82bf9ff67f6e109207",
+        },
         type="Classification",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["pl"],
         main_score="accuracy",
-        revision="477b8bd4448b5ef8ed01ba82bf9ff67f6e109207",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -117,21 +125,23 @@
 
 
 class PacClassification(AbsTaskClassification):
     metadata = TaskMetadata(
         name="PAC",
         description="Polish Paraphrase Corpus",
         reference="https://arxiv.org/pdf/2211.13112.pdf",
-        hf_hub_name="laugustyniak/abusive-clauses-pl",
+        dataset={
+            "path": "laugustyniak/abusive-clauses-pl",
+            "revision": "8a04d940a42cd40658986fdd8e3da561533a3646",
+        },
         type="Classification",
         category="p2p",
         eval_splits=["test"],
         eval_langs=["pl"],
         main_score="accuracy",
-        revision="8a04d940a42cd40658986fdd8e3da561533a3646",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Classification/sv/SweRecClassification.py` & `mteb-1.5.0/mteb/tasks/Classification/sv/SweRecClassification.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 
 
 class SweRecClassification(AbsTaskClassification):
     metadata = TaskMetadata(
         name="SweRecClassification",
         description="A Swedish dataset for sentiment classification on review",
         reference="https://aclanthology.org/2023.nodalida-1.20/",
-        hf_hub_name="SweRecClassification",
+        dataset={
+            "path": "SweRecClassification",
+            "revision": "3c62f26bafdc4c4e1c16401ad4b32f0a94b46612",
+        },
         type="Classification",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["sv"],
         main_score="accuracy",
-        revision="3c62f26bafdc4c4e1c16401ad4b32f0a94b46612",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Classification/zh/CMTEBClassification.py` & `mteb-1.5.0/mteb/tasks/Classification/zh/CMTEBClassification.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 
 
 class TNews(AbsTaskClassification):
     metadata = TaskMetadata(
         name="TNews",
         description="Short Text Classification for News",
         reference="https://www.cluebenchmarks.com/introduce.html",
-        hf_hub_name="C-MTEB/TNews-classification",
+        dataset={
+            "path": "C-MTEB/TNews-classification",
+            "revision": "317f262bf1e6126357bbe89e875451e4b0938fe4",
+        },
         type="Classification",
         category="s2s",
         eval_splits=["validation", "test"],
         eval_langs=["zh"],
         main_score="accuracy",
-        revision="317f262bf1e6126357bbe89e875451e4b0938fe4",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -29,31 +31,33 @@
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
+        metadata_dict = super().metadata_dict
         metadata_dict["samples_per_label"] = 32
         return metadata_dict
 
 
 class IFlyTek(AbsTaskClassification):
     metadata = TaskMetadata(
         name="IFlyTek",
         description="Long Text classification for the description of Apps",
         reference="https://www.cluebenchmarks.com/introduce.html",
-        hf_hub_name="C-MTEB/IFlyTek-classification",
+        dataset={
+            "path": "C-MTEB/IFlyTek-classification",
+            "revision": "421605374b29664c5fc098418fe20ada9bd55f8a",
+        },
         type="Classification",
         category="s2s",
         eval_splits=["validation", "test"],
         eval_langs=["zh"],
         main_score="accuracy",
-        revision="421605374b29664c5fc098418fe20ada9bd55f8a",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -62,32 +66,34 @@
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
+        metadata_dict = super().metadata_dict
         metadata_dict["samples_per_label"] = 32
         metadata_dict["n_experiments"] = 5
         return metadata_dict
 
 
 class MultilingualSentiment(AbsTaskClassification):
     metadata = TaskMetadata(
         name="MultilingualSentiment",
         description="A collection of multilingual sentiments datasets grouped into 3 classes -- positive, neutral, negative",
         reference="https://github.com/tyqiangz/multilingual-sentiment-datasets",
-        hf_hub_name="C-MTEB/MultilingualSentiment-classification",
+        dataset={
+            "path": "C-MTEB/MultilingualSentiment-classification",
+            "revision": "46958b007a63fdbf239b7672c25d0bea67b5ea1a",
+        },
         type="Classification",
         category="s2s",
         eval_splits=["validation", "test"],
         eval_langs=["zh"],
         main_score="accuracy",
-        revision="46958b007a63fdbf239b7672c25d0bea67b5ea1a",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -96,31 +102,33 @@
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
+        metadata_dict = super().metadata_dict
         metadata_dict["samples_per_label"] = 32
         return metadata_dict
 
 
 class JDReview(AbsTaskClassification):
     metadata = TaskMetadata(
         name="JDReview",
         description="review for iphone",
         reference="https://aclanthology.org/2023.nodalida-1.20/",
-        hf_hub_name="C-MTEB/JDReview-classification",
+        dataset={
+            "path": "C-MTEB/JDReview-classification",
+            "revision": "b7c64bd89eb87f8ded463478346f76731f07bf8b",
+        },
         type="Classification",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["zh"],
         main_score="accuracy",
-        revision="b7c64bd89eb87f8ded463478346f76731f07bf8b",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -129,31 +137,33 @@
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
+        metadata_dict = super().metadata_dict
         metadata_dict["samples_per_label"] = 32
         return metadata_dict
 
 
 class OnlineShopping(AbsTaskClassification):
     metadata = TaskMetadata(
         name="OnlineShopping",
         description="Sentiment Analysis of User Reviews on Online Shopping Websites",
         reference="https://aclanthology.org/2023.nodalida-1.20/",
-        hf_hub_name="C-MTEB/OnlineShopping-classification",
+        dataset={
+            "path": "C-MTEB/OnlineShopping-classification",
+            "revision": "e610f2ebd179a8fda30ae534c3878750a96db120",
+        },
         type="Classification",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["zh"],
         main_score="accuracy",
-        revision="e610f2ebd179a8fda30ae534c3878750a96db120",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -162,31 +172,33 @@
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
+        metadata_dict = super().metadata_dict
         metadata_dict["samples_per_label"] = 32
         return metadata_dict
 
 
 class Waimai(AbsTaskClassification):
     metadata = TaskMetadata(
         name="Waimai",
         description="Sentiment Analysis of user reviews on takeaway platforms",
         reference="https://aclanthology.org/2023.nodalida-1.20/",
-        hf_hub_name="C-MTEB/waimai-classification",
+        dataset={
+            "path": "C-MTEB/waimai-classification",
+            "revision": "339287def212450dcaa9df8c22bf93e9980c7023",
+        },
         type="Classification",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["zh"],
         main_score="accuracy",
-        revision="339287def212450dcaa9df8c22bf93e9980c7023",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -195,11 +207,11 @@
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
+        metadata_dict = super().metadata_dict
         metadata_dict["samples_per_label"] = 32
 
         return metadata_dict
```

### Comparing `mteb-1.4.1/mteb/tasks/Clustering/__init__.py` & `mteb-1.5.0/mteb/tasks/Clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/mteb/tasks/Clustering/de/BlurbsClusteringP2P.py` & `mteb-1.5.0/mteb/tasks/Clustering/en/MedrxivClusteringP2P.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 from __future__ import annotations
 
-from mteb.abstasks.AbsTaskClustering import AbsTaskClustering
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
+from ....abstasks.AbsTaskClustering import AbsTaskClustering
 
-class BlurbsClusteringP2P(AbsTaskClustering):
+
+class MedrxivClusteringP2P(AbsTaskClustering):
     metadata = TaskMetadata(
-        name="BlurbsClusteringP2P",
-        description="Clustering of book titles+blurbs. Clustering of 28 sets, either on the main or secondary genre.",
-        reference="https://www.inf.uni-hamburg.de/en/inst/ab/lt/resources/data/germeval-2019-hmc.html",
-        hf_hub_name="slvnwhrl/blurbs-clustering-p2p",
+        name="MedrxivClusteringP2P",
+        description="Clustering of titles+abstract from medrxiv. Clustering of 10 sets, based on the main category.",
+        reference="https://api.medrxiv.org/",
+        dataset={
+            "path": "mteb/medrxiv-clustering-p2p",
+            "revision": "e7a26af6f3ae46b30dde8737f02c07b1505bcc73",
+        },
         type="Clustering",
         category="p2p",
         eval_splits=["test"],
-        eval_langs=["de"],
+        eval_langs=["en"],
         main_score="v_measure",
-        revision="a2dd5b02a77de3466a3eaa98ae586b5610314496",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples={"test": 174637},
-        avg_character_length={"test": 664.09},
+        n_samples={"test": 375000},
+        avg_character_length={"test": 1981.2},
     )
```

### Comparing `mteb-1.4.1/mteb/tasks/Clustering/de/BlurbsClusteringS2S.py` & `mteb-1.5.0/mteb/tasks/Clustering/de/TenKGnadClusteringP2P.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskClustering import AbsTaskClustering
 
 
-class BlurbsClusteringS2S(AbsTaskClustering):
+class TenKGnadClusteringP2P(AbsTaskClustering):
     metadata = TaskMetadata(
-        name="BlurbsClusteringS2S",
-        description="Clustering of book titles. Clustering of 28 sets, either on the main or secondary genre.",
-        reference="https://www.inf.uni-hamburg.de/en/inst/ab/lt/resources/data/germeval-2019-hmc.html",
-        hf_hub_name="slvnwhrl/blurbs-clustering-s2s",
+        name="TenKGnadClusteringP2P",
+        description="Clustering of news article titles+subheadings+texts. Clustering of 10 splits on the news article category.",
+        reference="https://tblock.github.io/10kGNAD/",
+        dataset={
+            "path": "slvnwhrl/tenkgnad-clustering-p2p",
+            "revision": "5c59e41555244b7e45c9a6be2d720ab4bafae558",
+        },
         type="Clustering",
-        category="s2s",
+        category="p2p",
         eval_splits=["test"],
         eval_langs=["de"],
         main_score="v_measure",
-        revision="5bfd9ee0ae3d2ef0d9a0e0bd0c3b2d0",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples={"test": 174637},
-        avg_character_length={"test": 23.02},
+        n_samples={"test": 45914},
+        avg_character_length={"test": 2641.03},
     )
```

### Comparing `mteb-1.4.1/mteb/tasks/Clustering/de/TenKGnadClusteringP2P.py` & `mteb-1.5.0/mteb/tasks/Clustering/de/TenKGnadClusteringS2S.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskClustering import AbsTaskClustering
 
 
-class TenKGnadClusteringP2P(AbsTaskClustering):
+class TenKGnadClusteringS2S(AbsTaskClustering):
     metadata = TaskMetadata(
-        name="TenKGnadClusteringP2P",
-        description="Clustering of news article titles+subheadings+texts. Clustering of 10 splits on the news article category.",
+        name="TenKGnadClusteringS2S",
+        description="Clustering of news article titles. Clustering of 10 splits on the news article category.",
         reference="https://tblock.github.io/10kGNAD/",
-        hf_hub_name="slvnwhrl/tenkgnad-clustering-p2p",
+        dataset={
+            "path": "slvnwhrl/tenkgnad-clustering-s2s",
+            "revision": "6cddbe003f12b9b140aec477b583ac4191f01786",
+        },
         type="Clustering",
-        category="p2p",
+        category="s2s",
         eval_splits=["test"],
         eval_langs=["de"],
         main_score="v_measure",
-        revision="5c59e41555244b7e45c9a6be2d720ab4bafae558",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
         n_samples={"test": 45914},
-        avg_character_length={"test": 2641.03},
+        avg_character_length={"test": 50.96},
     )
```

### Comparing `mteb-1.4.1/mteb/tasks/Clustering/de/TenKGnadClusteringS2S.py` & `mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackWebmastersRetrieval.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks.AbsTaskClustering import AbsTaskClustering
+from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class TenKGnadClusteringS2S(AbsTaskClustering):
+class CQADupstackWebmastersRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="TenKGnadClusteringS2S",
-        description="Clustering of news article titles. Clustering of 10 splits on the news article category.",
-        reference="https://tblock.github.io/10kGNAD/",
-        hf_hub_name="slvnwhrl/tenkgnad-clustering-s2s",
-        type="Clustering",
-        category="s2s",
+        name="CQADupstackWebmastersRetrieval",
+        description="CQADupStack: A Benchmark Data Set for Community Question-Answering Research",
+        reference="http://nlp.cis.unimelb.edu.au/resources/cqadupstack/",
+        dataset={
+            "path": "mteb/cqadupstack-webmasters",
+            "revision": "160c094312a0e1facb97e55eeddb698c0abe3571",
+        },
+        type="Retrieval",
+        category="s2p",
         eval_splits=["test"],
-        eval_langs=["de"],
-        main_score="v_measure",
-        revision="6cddbe003f12b9b140aec477b583ac4191f01786",
+        eval_langs=["en"],
+        main_score="ndcg_at_10",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples={"test": 45914},
-        avg_character_length={"test": 50.96},
+        n_samples=None,
+        avg_character_length=None,
     )
```

### Comparing `mteb-1.4.1/mteb/tasks/Clustering/en/ArxivClusteringP2P.py` & `mteb-1.5.0/mteb/tasks/Clustering/en/RedditClusteringP2P.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskClustering import AbsTaskClustering
 
 
-class ArxivClusteringP2P(AbsTaskClustering):
+class RedditClusteringP2P(AbsTaskClustering):
     metadata = TaskMetadata(
-        name="ArxivClusteringP2P",
-        description="Clustering of titles+abstract from arxiv. Clustering of 30 sets, either on the main or secondary category",
-        reference="https://www.kaggle.com/Cornell-University/arxiv",
-        hf_hub_name="mteb/arxiv-clustering-p2p",
+        name="RedditClusteringP2P",
+        description="Clustering of title+posts from reddit. Clustering of 10 sets of 50k paragraphs and 40 sets of 10k paragraphs.",
+        reference="https://arxiv.org/abs/2104.07081",
+        dataset={
+            "path": "mteb/reddit-clustering-p2p",
+            "revision": "385e3cb46b4cfa89021f56c4380204149d0efe33",
+        },
         type="Clustering",
         category="p2p",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="v_measure",
-        revision="a122ad7f3f0291bf49cc6f4d32aa80929df69d5d",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples={"test": 732723},
-        avg_character_length={"test": 1009.98},
+        n_samples={"test": 459399},
+        avg_character_length={"test": 727.7},
     )
```

### Comparing `mteb-1.4.1/mteb/tasks/Clustering/en/ArxivClusteringS2S.py` & `mteb-1.5.0/mteb/tasks/Clustering/en/ArxivClusteringP2P.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskClustering import AbsTaskClustering
 
 
-class ArxivClusteringS2S(AbsTaskClustering):
+class ArxivClusteringP2P(AbsTaskClustering):
     metadata = TaskMetadata(
-        name="ArxivClusteringS2S",
-        description="Clustering of titles from arxiv. Clustering of 30 sets, either on the main or secondary category",
+        name="ArxivClusteringP2P",
+        description="Clustering of titles+abstract from arxiv. Clustering of 30 sets, either on the main or secondary category",
         reference="https://www.kaggle.com/Cornell-University/arxiv",
-        hf_hub_name="mteb/arxiv-clustering-s2s",
+        dataset={
+            "path": "mteb/arxiv-clustering-p2p",
+            "revision": "a122ad7f3f0291bf49cc6f4d32aa80929df69d5d",
+        },
         type="Clustering",
-        category="s2s",
+        category="p2p",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="v_measure",
-        revision="f910caf1a6075f7329cdf8c1a6135696f37dbd53",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
         n_samples={"test": 732723},
-        avg_character_length={"test": 74},
+        avg_character_length={"test": 1009.98},
     )
```

### Comparing `mteb-1.4.1/mteb/tasks/Clustering/en/BigPatentClustering.py` & `mteb-1.5.0/mteb/tasks/Clustering/en/BigPatentClustering.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 
 class BigPatentClustering(AbsTaskClustering):
     metadata = TaskMetadata(
         name="BigPatentClustering",
         description="Clustering of documents from the Big Patent dataset. Test set only includes documents"
         "belonging to a single category, with a total of 9 categories.",
         reference="https://www.kaggle.com/datasets/big_patent",
-        hf_hub_name="jinaai/big-patent-clustering",
+        dataset={
+            "path": "jinaai/big-patent-clustering",
+            "revision": "62d5330920bca426ce9d3c76ea914f15fc83e891",
+        },
         type="Clustering",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="v_measure",
-        revision="62d5330920bca426ce9d3c76ea914f15fc83e891",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Clustering/en/BiorxivClusteringP2P.py` & `mteb-1.5.0/mteb/tasks/Clustering/en/BiorxivClusteringP2P.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 
 
 class BiorxivClusteringP2P(AbsTaskClustering):
     metadata = TaskMetadata(
         name="BiorxivClusteringP2P",
         description="Clustering of titles+abstract from biorxiv. Clustering of 10 sets, based on the main category.",
         reference="https://api.biorxiv.org/",
-        hf_hub_name="mteb/biorxiv-clustering-p2p",
+        dataset={
+            "path": "mteb/biorxiv-clustering-p2p",
+            "revision": "65b79d1d13f80053f67aca9498d9402c2d9f1f40",
+        },
         type="Clustering",
         category="p2p",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="v_measure",
-        revision="65b79d1d13f80053f67aca9498d9402c2d9f1f40",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Clustering/en/BiorxivClusteringS2S.py` & `mteb-1.5.0/mteb/tasks/Clustering/en/BiorxivClusteringS2S.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 
 
 class BiorxivClusteringS2S(AbsTaskClustering):
     metadata = TaskMetadata(
         name="BiorxivClusteringS2S",
         description="Clustering of titles from biorxiv. Clustering of 10 sets, based on the main category.",
         reference="https://api.biorxiv.org/",
-        hf_hub_name="mteb/biorxiv-clustering-s2s",
+        dataset={
+            "path": "mteb/biorxiv-clustering-s2s",
+            "revision": "258694dd0231531bc1fd9de6ceb52a0853c6d908",
+        },
         type="Clustering",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="v_measure",
-        revision="258694dd0231531bc1fd9de6ceb52a0853c6d908",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Clustering/en/MedrxivClusteringP2P.py` & `mteb-1.5.0/mteb/tasks/Clustering/de/BlurbsClusteringP2P.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from __future__ import annotations
 
+from mteb.abstasks.AbsTaskClustering import AbsTaskClustering
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks.AbsTaskClustering import AbsTaskClustering
 
-
-class MedrxivClusteringP2P(AbsTaskClustering):
+class BlurbsClusteringP2P(AbsTaskClustering):
     metadata = TaskMetadata(
-        name="MedrxivClusteringP2P",
-        description="Clustering of titles+abstract from medrxiv. Clustering of 10 sets, based on the main category.",
-        reference="https://api.medrxiv.org/",
-        hf_hub_name="mteb/medrxiv-clustering-p2p",
+        name="BlurbsClusteringP2P",
+        description="Clustering of book titles+blurbs. Clustering of 28 sets, either on the main or secondary genre.",
+        reference="https://www.inf.uni-hamburg.de/en/inst/ab/lt/resources/data/germeval-2019-hmc.html",
+        dataset={
+            "path": "slvnwhrl/blurbs-clustering-p2p",
+            "revision": "a2dd5b02a77de3466a3eaa98ae586b5610314496",
+        },
         type="Clustering",
         category="p2p",
         eval_splits=["test"],
-        eval_langs=["en"],
+        eval_langs=["de"],
         main_score="v_measure",
-        revision="e7a26af6f3ae46b30dde8737f02c07b1505bcc73",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples={"test": 375000},
-        avg_character_length={"test": 1981.2},
+        n_samples={"test": 174637},
+        avg_character_length={"test": 664.09},
     )
```

### Comparing `mteb-1.4.1/mteb/tasks/Clustering/en/MedrxivClusteringS2S.py` & `mteb-1.5.0/mteb/tasks/Clustering/en/MedrxivClusteringS2S.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 
 
 class MedrxivClusteringS2S(AbsTaskClustering):
     metadata = TaskMetadata(
         name="MedrxivClusteringS2S",
         description="Clustering of titles from medrxiv. Clustering of 10 sets, based on the main category.",
         reference="https://api.medrxiv.org/",
-        hf_hub_name="mteb/medrxiv-clustering-s2s",
+        dataset={
+            "path": "mteb/medrxiv-clustering-s2s",
+            "revision": "35191c8c0dca72d8ff3efcd72aa802307d469663",
+        },
         type="Clustering",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="v_measure",
-        revision="35191c8c0dca72d8ff3efcd72aa802307d469663",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Clustering/en/RedditClustering.py` & `mteb-1.5.0/mteb/tasks/Clustering/en/RedditClustering.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 
 
 class RedditClustering(AbsTaskClustering):
     metadata = TaskMetadata(
         name="RedditClustering",
         description="Clustering of titles from 199 subreddits. Clustering of 25 sets, each with 10-50 classes, and each class with 100 - 1000 sentences.",
         reference="https://arxiv.org/abs/2104.07081",
-        hf_hub_name="mteb/reddit-clustering",
+        dataset={
+            "path": "mteb/reddit-clustering",
+            "revision": "24640382cdbf8abc73003fb0fa6d111a705499eb",
+        },
         type="Clustering",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="v_measure",
-        revision="24640382cdbf8abc73003fb0fa6d111a705499eb",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Clustering/en/RedditClusteringP2P.py` & `mteb-1.5.0/mteb/tasks/Clustering/en/StackExchangeClusteringP2P.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskClustering import AbsTaskClustering
 
 
-class RedditClusteringP2P(AbsTaskClustering):
+class StackExchangeClusteringP2P(AbsTaskClustering):
     metadata = TaskMetadata(
-        name="RedditClusteringP2P",
-        description="Clustering of title+posts from reddit. Clustering of 10 sets of 50k paragraphs and 40 sets of 10k paragraphs.",
+        name="StackExchangeClusteringP2P",
+        description="Clustering of title+body from stackexchange. Clustering of 5 sets of 10k paragraphs and 5 sets of 5k paragraphs.",
         reference="https://arxiv.org/abs/2104.07081",
-        hf_hub_name="mteb/reddit-clustering-p2p",
+        dataset={
+            "path": "mteb/stackexchange-clustering-p2p",
+            "revision": "815ca46b2622cec33ccafc3735d572c266efdb44",
+        },
         type="Clustering",
         category="p2p",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="v_measure",
-        revision="385e3cb46b4cfa89021f56c4380204149d0efe33",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples={"test": 459399},
-        avg_character_length={"test": 727.7},
+        n_samples={"test": 75000},
+        avg_character_length={"test": 1090.7},
     )
```

### Comparing `mteb-1.4.1/mteb/tasks/Clustering/en/StackExchangeClustering.py` & `mteb-1.5.0/mteb/tasks/Clustering/en/StackExchangeClustering.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 
 
 class StackExchangeClustering(AbsTaskClustering):
     metadata = TaskMetadata(
         name="StackExchangeClustering",
         description="Clustering of titles from 121 stackexchanges. Clustering of 25 sets, each with 10-50 classes, and each class with 100 - 1000 sentences.",
         reference="https://arxiv.org/abs/2104.07081",
-        hf_hub_name="mteb/stackexchange-clustering",
+        dataset={
+            "path": "mteb/stackexchange-clustering",
+            "revision": "6cbc1f7b2bc0622f2e39d2c77fa502909748c259",
+        },
         type="Clustering",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="v_measure",
-        revision="6cbc1f7b2bc0622f2e39d2c77fa502909748c259",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Clustering/en/StackExchangeClusteringP2P.py` & `mteb-1.5.0/mteb/tasks/Clustering/en/TwentyNewsgroupsClustering.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskClustering import AbsTaskClustering
 
 
-class StackExchangeClusteringP2P(AbsTaskClustering):
+class TwentyNewsgroupsClustering(AbsTaskClustering):
     metadata = TaskMetadata(
-        name="StackExchangeClusteringP2P",
-        description="Clustering of title+body from stackexchange. Clustering of 5 sets of 10k paragraphs and 5 sets of 5k paragraphs.",
-        reference="https://arxiv.org/abs/2104.07081",
-        hf_hub_name="mteb/stackexchange-clustering-p2p",
+        name="TwentyNewsgroupsClustering",
+        description="Clustering of the 20 Newsgroups dataset (subject only).",
+        reference="https://scikit-learn.org/0.19/datasets/twenty_newsgroups.html",
+        dataset={
+            "path": "mteb/twentynewsgroups-clustering",
+            "revision": "6125ec4e24fa026cec8a478383ee943acfbd5449",
+        },
         type="Clustering",
-        category="p2p",
+        category="s2s",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="v_measure",
-        revision="815ca46b2622cec33ccafc3735d572c266efdb44",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples={"test": 75000},
-        avg_character_length={"test": 1090.7},
+        n_samples={"test": 59545},
+        avg_character_length={"test": 32.0},
     )
```

### Comparing `mteb-1.4.1/mteb/tasks/Clustering/en/TwentyNewsgroupsClustering.py` & `mteb-1.5.0/mteb/tasks/Clustering/en/ArxivClusteringS2S.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskClustering import AbsTaskClustering
 
 
-class TwentyNewsgroupsClustering(AbsTaskClustering):
+class ArxivClusteringS2S(AbsTaskClustering):
     metadata = TaskMetadata(
-        name="TwentyNewsgroupsClustering",
-        description="Clustering of the 20 Newsgroups dataset (subject only).",
-        reference="https://scikit-learn.org/0.19/datasets/twenty_newsgroups.html",
-        hf_hub_name="mteb/twentynewsgroups-clustering",
+        name="ArxivClusteringS2S",
+        description="Clustering of titles from arxiv. Clustering of 30 sets, either on the main or secondary category",
+        reference="https://www.kaggle.com/Cornell-University/arxiv",
+        dataset={
+            "path": "mteb/arxiv-clustering-s2s",
+            "revision": "f910caf1a6075f7329cdf8c1a6135696f37dbd53",
+        },
         type="Clustering",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="v_measure",
-        revision="6125ec4e24fa026cec8a478383ee943acfbd5449",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples={"test": 59545},
-        avg_character_length={"test": 32.0},
+        n_samples={"test": 732723},
+        avg_character_length={"test": 74},
     )
```

### Comparing `mteb-1.4.1/mteb/tasks/Clustering/en/WikiCitiesClustering.py` & `mteb-1.5.0/mteb/tasks/Clustering/en/WikiCitiesClustering.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 
 
 class WikiCitiesClustering(AbsTaskClustering):
     metadata = TaskMetadata(
         name="WikiCitiesClustering",
         description="Clustering of Wikipedia articles of cities by country from https://huggingface.co/datasets/wikipedia. Test set includes 126 countries, and a total of 3531 cities.",
         reference="https://huggingface.co/datasets/wikipedia",
-        hf_hub_name="jinaai/cities_wiki_clustering",
+        dataset={
+            "path": "jinaai/cities_wiki_clustering",
+            "revision": "ddc9ee9242fa65332597f70e967ecc38b9d734fa",
+        },
         type="Clustering",
         category="p2p",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="v_measure",
-        revision="ddc9ee9242fa65332597f70e967ecc38b9d734fa",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Clustering/es/FloresClusteringS2S.py` & `mteb-1.5.0/mteb/tasks/Clustering/es/FloresClusteringS2S.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 
 
 class FloresClusteringS2S(AbsTaskClustering):
     metadata = TaskMetadata(
         name="FloresClusteringS2S",
         description="Clustering of sentences from various web articles, 32 topics in total.",
         reference="https://huggingface.co/datasets/facebook/flores",
-        hf_hub_name="mteb/flores",
+        dataset={
+            "path": "mteb/flores",
+            "revision": "480b580487f53a46f881354a8348335d4edbb2de",
+        },
         type="Clustering",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["es"],
         main_score="v_measure",
-        revision="480b580487f53a46f881354a8348335d4edbb2de",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Clustering/es/SpanishNewsClusteringP2P.py` & `mteb-1.5.0/mteb/tasks/Clustering/es/SpanishNewsClusteringP2P.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 
 
 class SpanishNewsClusteringP2P(AbsTaskClustering):
     metadata = TaskMetadata(
         name="SpanishNewsClusteringP2P",
         description="Clustering of news articles, 7 topics in total.",
         reference="https://www.kaggle.com/datasets/kevinmorgado/spanish-news-classification",
-        hf_hub_name="mteb/spanish_news_clustering",
+        dataset={
+            "path": "mteb/spanish_news_clustering",
+            "revision": "b5edc3d3d7c12c7b9f883e9da50f6732f3624142",
+        },
         type="Clustering",
         category="p2p",
         eval_splits=["test"],
         eval_langs=["es"],
         main_score="v_measure",
-        revision="b5edc3d3d7c12c7b9f883e9da50f6732f3624142",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Clustering/fr/AlloProfClusteringP2P.py` & `mteb-1.5.0/mteb/tasks/Clustering/fr/AlloProfClusteringP2P.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,50 +9,38 @@
 
 
 class AlloProfClusteringP2P(AbsTaskClustering):
     metadata = TaskMetadata(
         name="AlloProfClusteringP2P",
         description="Clustering of document titles and descriptions from Allo Prof dataset. Clustering of 10 sets on the document topic.",
         reference="https://huggingface.co/datasets/lyon-nlp/alloprof",
-        hf_hub_name="mteb/alloprof",
+        dataset={
+            "path": "mteb/alloprof",
+            "revision": "392ba3f5bcc8c51f578786c1fc3dae648662cb9b",
+            "name": "documents",
+        },
         type="Clustering",
         category="p2p",
         eval_splits=["test"],
         eval_langs=["fr"],
         main_score="v_measure",
-        revision="392ba3f5bcc8c51f578786c1fc3dae648662cb9b",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
-    def load_data(self, **kwargs):
-        """
-        Load dataset from HuggingFace hub and convert it to the standard format.
-        """
-        if self.data_loaded:
-            return
-
-        self.dataset = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            "documents",
-            revision=self.metadata_dict.get("revision", None),
-        )
-        self.dataset_transform()
-        self.data_loaded = True
-
     def create_description(self, example):
         example["text"] = example["title"] + " " + example["text"]
         return example
 
     def dataset_transform(self):
         """
         Convert to standard format
```

### Comparing `mteb-1.4.1/mteb/tasks/Clustering/fr/AlloProfClusteringS2S.py` & `mteb-1.5.0/mteb/tasks/Clustering/fr/HALClusteringS2S.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,61 +4,47 @@
 import numpy as np
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskClustering import AbsTaskClustering
 
 
-class AlloProfClusteringS2S(AbsTaskClustering):
+class HALClusteringS2S(AbsTaskClustering):
     metadata = TaskMetadata(
-        name="AlloProfClusteringS2S",
-        description="Clustering of document titles from Allo Prof dataset. Clustering of 10 sets on the document topic.",
-        reference="https://huggingface.co/datasets/lyon-nlp/alloprof",
-        hf_hub_name="mteb/alloprof",
+        name="HALClusteringS2S",
+        description="Clustering of titles from HAL (https://huggingface.co/datasets/lyon-nlp/clustering-hal-s2s)",
+        reference="https://huggingface.co/datasets/lyon-nlp/clustering-hal-s2s",
+        dataset={
+            "path": "mteb/hal",
+            "revision": "e06ebbbb123f8144bef1a5d18796f3dec9ae2915",
+        },
         type="Clustering",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["fr"],
         main_score="v_measure",
-        revision="392ba3f5bcc8c51f578786c1fc3dae648662cb9b",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
-    def load_data(self, **kwargs):
-        """
-        Load dataset from HuggingFace hub and convert it to the standard format.
-        """
-        if self.data_loaded:
-            return
-        self.dataset = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            "documents",
-            revision=self.metadata_dict.get("revision", None),
-        )
-        self.dataset_transform()
-        self.data_loaded = True
-
     def dataset_transform(self):
         """
         Convert to standard format
         """
-        self.dataset = self.dataset.remove_columns("uuid")
-        self.dataset = self.dataset.remove_columns("text")
-        titles = self.dataset["documents"]["title"]
-        topics = self.dataset["documents"]["topic"]
+        self.dataset = self.dataset.remove_columns("hal_id")
+        titles = self.dataset["test"]["title"]
+        domains = self.dataset["test"]["domain"]
         new_format = {
             "sentences": [split.tolist() for split in np.array_split(titles, 10)],
-            "labels": [split.tolist() for split in np.array_split(topics, 10)],
+            "labels": [split.tolist() for split in np.array_split(domains, 10)],
         }
         self.dataset["test"] = datasets.Dataset.from_dict(new_format)
-        self.dataset.pop("documents")
```

### Comparing `mteb-1.4.1/mteb/tasks/Clustering/fr/HALClusteringS2S.py` & `mteb-1.5.0/mteb/tasks/Clustering/fr/MLSUMClusteringP2P.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,59 +4,56 @@
 import numpy as np
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskClustering import AbsTaskClustering
 
 
-class HALClusteringS2S(AbsTaskClustering):
+class MLSUMClusteringP2P(AbsTaskClustering):
     metadata = TaskMetadata(
-        name="HALClusteringS2S",
-        description="Clustering of titles from HAL (https://huggingface.co/datasets/lyon-nlp/clustering-hal-s2s)",
-        reference="https://huggingface.co/datasets/lyon-nlp/clustering-hal-s2s",
-        hf_hub_name="mteb/hal",
+        name="MLSUMClusteringP2P",
+        description="Clustering of newspaper article contents and titles from MLSUM dataset. Clustering of 10 sets on the newpaper article topics.",
+        reference="https://huggingface.co/datasets/mlsum",
+        dataset={
+            "path": "mteb/mlsum",
+            "revision": "b5d54f8f3b61ae17845046286940f03c6bc79bc7",
+            "name": "fr",
+            "split": "test",
+        },
         type="Clustering",
-        category="s2s",
+        category="p2p",
         eval_splits=["test"],
         eval_langs=["fr"],
         main_score="v_measure",
-        revision="e06ebbbb123f8144bef1a5d18796f3dec9ae2915",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
-    def load_data(self, **kwargs):
-        """
-        Load dataset from HuggingFace hub and convert it to the standard format.
-        """
-        if self.data_loaded:
-            return
-
-        self.dataset = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            revision=self.metadata_dict.get("revision", None),
-        )
-        self.dataset_transform()
-        self.data_loaded = True
+    def create_description(self, example):
+        example["text"] = example["title"] + " " + example["text"]
+        return example
 
     def dataset_transform(self):
         """
         Convert to standard format
         """
-        self.dataset = self.dataset.remove_columns("hal_id")
-        titles = self.dataset["test"]["title"]
-        domains = self.dataset["test"]["domain"]
+        self.dataset = self.dataset.map(self.create_description)
+        self.dataset = self.dataset.remove_columns(["summary", "url", "date", "title"])
+        texts = self.dataset["text"]
+        topics = self.dataset["topic"]
         new_format = {
-            "sentences": [split.tolist() for split in np.array_split(titles, 10)],
-            "labels": [split.tolist() for split in np.array_split(domains, 10)],
+            "sentences": [split.tolist() for split in np.array_split(texts, 10)],
+            "labels": [split.tolist() for split in np.array_split(topics, 10)],
+        }
+        self.dataset = {
+            self.metadata_dict["eval_splits"][0]: datasets.Dataset.from_dict(new_format)
         }
-        self.dataset["test"] = datasets.Dataset.from_dict(new_format)
```

### Comparing `mteb-1.4.1/mteb/tasks/Clustering/fr/MLSUMClusteringP2P.py` & `mteb-1.5.0/mteb/tasks/Clustering/fr/MLSUMClusteringS2S.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,67 +4,53 @@
 import numpy as np
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskClustering import AbsTaskClustering
 
 
-class MLSUMClusteringP2P(AbsTaskClustering):
+class MLSUMClusteringS2S(AbsTaskClustering):
     metadata = TaskMetadata(
-        name="MLSUMClusteringP2P",
+        name="MLSUMClusteringS2S",
         description="Clustering of newspaper article contents and titles from MLSUM dataset. Clustering of 10 sets on the newpaper article topics.",
         reference="https://huggingface.co/datasets/mlsum",
-        hf_hub_name="mteb/mlsum",
+        dataset={
+            "path": "mteb/mlsum",
+            "revision": "b5d54f8f3b61ae17845046286940f03c6bc79bc7",
+            "name": "fr",
+            "split": "test",
+        },
         type="Clustering",
-        category="p2p",
+        category="s2s",
         eval_splits=["test"],
         eval_langs=["fr"],
         main_score="v_measure",
-        revision="b5d54f8f3b61ae17845046286940f03c6bc79bc7",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
-    def load_data(self, **kwargs):
-        """
-        Load dataset from HuggingFace hub and convert it to the standard format.
-        """
-        if self.data_loaded:
-            return
-        self.dataset = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            "fr",
-            split=self.metadata_dict["eval_splits"][0],
-            revision=self.metadata_dict.get("revision", None),
-        )
-        self.dataset_transform()
-        self.data_loaded = True
-
-    def create_description(self, example):
-        example["text"] = example["title"] + " " + example["text"]
-        return example
-
     def dataset_transform(self):
         """
         Convert to standard format
         """
-        self.dataset = self.dataset.map(self.create_description)
-        self.dataset = self.dataset.remove_columns(["summary", "url", "date", "title"])
-        texts = self.dataset["text"]
-        topics = self.dataset["topic"]
+        self.dataset = self.dataset.remove_columns(["summary", "text", "url", "date"])
         new_format = {
-            "sentences": [split.tolist() for split in np.array_split(texts, 10)],
-            "labels": [split.tolist() for split in np.array_split(topics, 10)],
+            "sentences": [
+                split.tolist() for split in np.array_split(self.dataset["title"], 10)
+            ],
+            "labels": [
+                split.tolist() for split in np.array_split(self.dataset["topic"], 10)
+            ],
         }
         self.dataset = {
             self.metadata_dict["eval_splits"][0]: datasets.Dataset.from_dict(new_format)
         }
```

### Comparing `mteb-1.4.1/mteb/tasks/Clustering/fr/MLSUMClusteringS2S.py` & `mteb-1.5.0/mteb/tasks/PairClassification/multilingual/PawsX.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 from __future__ import annotations
 
 import datasets
-import numpy as np
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks.AbsTaskClustering import AbsTaskClustering
+from ....abstasks import MultilingualTask
+from ....abstasks.AbsTaskPairClassification import AbsTaskPairClassification
 
 
-class MLSUMClusteringS2S(AbsTaskClustering):
+class PawsX(MultilingualTask, AbsTaskPairClassification):
     metadata = TaskMetadata(
-        name="MLSUMClusteringS2S",
-        description="Clustering of newspaper article contents and titles from MLSUM dataset. Clustering of 10 sets on the newpaper article topics.",
-        reference="https://huggingface.co/datasets/mlsum",
-        hf_hub_name="mteb/mlsum",
-        type="Clustering",
+        name="PawsX",
+        dataset={
+            "path": "paws-x",
+            "revision": "8a04d940a42cd40658986fdd8e3da561533a3646",
+        },
+        description="",
+        reference="https://arxiv.org/abs/1908.11828",
         category="s2s",
-        eval_splits=["test"],
-        eval_langs=["fr"],
-        main_score="v_measure",
-        revision="b5d54f8f3b61ae17845046286940f03c6bc79bc7",
+        type="PairClassification",
+        eval_splits=["test.full", "validation.full"],
+        eval_langs=["de", "en", "es", "fr", "ja", "ko", "zh"],
+        main_score="ap",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -31,37 +33,37 @@
         text_creation=None,
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
     def load_data(self, **kwargs):
-        """
-        Load dataset from HuggingFace hub and convert it to the standard format.
-        """
         if self.data_loaded:
             return
-        self.dataset = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            "fr",
-            split=self.metadata_dict["eval_splits"][0],
-            revision=self.metadata_dict.get("revision", None),
-        )
-        self.dataset_transform()
-        self.data_loaded = True
 
-    def dataset_transform(self):
-        """
-        Convert to standard format
-        """
-        self.dataset = self.dataset.remove_columns(["summary", "text", "url", "date"])
-        new_format = {
-            "sentences": [
-                split.tolist() for split in np.array_split(self.dataset["title"], 10)
-            ],
-            "labels": [
-                split.tolist() for split in np.array_split(self.dataset["topic"], 10)
-            ],
-        }
-        self.dataset = {
-            self.metadata_dict["eval_splits"][0]: datasets.Dataset.from_dict(new_format)
-        }
+        self.dataset = dict()
+        for lang in self.langs:
+            hf_dataset = datasets.load_dataset(
+                name=lang,
+                **self.metadata_dict["dataset"],
+            )
+
+            sent1 = []
+            sent2 = []
+            labels = []
+
+            for line in hf_dataset["test"]:
+                sent1.append(line["sentence1"])
+                sent2.append(line["sentence2"])
+                labels.append(line["label"])
+
+            self.dataset[lang] = {
+                "test": [
+                    {
+                        "sent1": sent1,
+                        "sent2": sent2,
+                        "labels": labels,
+                    }
+                ]
+            }
+
+        self.data_loaded = True
```

### Comparing `mteb-1.4.1/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py` & `mteb-1.5.0/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,21 +28,23 @@
 
 
 class MasakhaNEWSClusteringP2P(AbsTaskClustering, MultilingualTask):
     metadata = TaskMetadata(
         name="MasakhaNEWSClusteringP2P",
         description="Clustering of news article headlines and texts from MasakhaNEWS dataset. Clustering of 10 sets on the news article label.",
         reference="https://huggingface.co/datasets/masakhane/masakhanews",
-        hf_hub_name="mteb/masakhanews",
+        dataset={
+            "path": "mteb/masakhanews",
+            "revision": "8ccc72e69e65f40c70e117d8b3c08306bb788b60",
+        },
         type="Clustering",
         category="p2p",
         eval_splits=["test"],
         eval_langs=_LANGUAGES,
         main_score="v_measure",
-        revision="8ccc72e69e65f40c70e117d8b3c08306bb788b60",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -58,17 +60,16 @@
         Load dataset from HuggingFace hub and convert it to the standard format.
         """
         if self.data_loaded:
             return
         self.dataset = {}
         for lang in self.langs:
             self.dataset[lang] = datasets.load_dataset(
-                self.metadata_dict["hf_hub_name"],
-                lang,
-                revision=self.metadata_dict.get("revision", None),
+                name=lang,
+                **self.metadata_dict["dataset"],
             )
             self.dataset_transform(lang)
         self.data_loaded = True
 
     def dataset_transform(self, lang):
         """
         Convert to standard format
```

### Comparing `mteb-1.4.1/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py` & `mteb-1.5.0/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,25 +26,27 @@
     "yor",
 ]
 
 
 class MasakhaNEWSClusteringS2S(AbsTaskClustering, MultilingualTask):
     metadata = TaskMetadata(
         name="MasakhaNEWSClusteringS2S",
-        hf_hub_name="masakhane/masakhanews",
+        dataset={
+            "path": "masakhane/masakhanews",
+            "revision": "8ccc72e69e65f40c70e117d8b3c08306bb788b60",
+        },
         description=(
             "Clustering of news article headlines from MasakhaNEWS dataset. Clustering of 10 sets on the news article label."
         ),
         reference="https://huggingface.co/datasets/masakhane/masakhanews",
         type="Clustering",
         category="s2s",
         eval_splits=["test"],
         eval_langs=_LANGUAGES,
         main_score="v_measure",
-        revision="8ccc72e69e65f40c70e117d8b3c08306bb788b60",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -60,17 +62,16 @@
         Load dataset from HuggingFace hub and convert it to the standard format.
         """
         if self.data_loaded:
             return
         self.dataset = {}
         for lang in self.langs:
             self.dataset[lang] = datasets.load_dataset(
-                self.metadata_dict["hf_hub_name"],
-                lang,
-                revision=self.metadata_dict.get("revision", None),
+                name=lang,
+                **self.metadata_dict["dataset"],
             )
             self.dataset_transform(lang)
         self.data_loaded = True
 
     def dataset_transform(self, lang):
         """
         Convert to standard format
```

### Comparing `mteb-1.4.1/mteb/tasks/Clustering/nb/snl_clustering.py` & `mteb-1.5.0/mteb/tasks/Clustering/nb/vg_clustering.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,98 +16,89 @@
     if n < 1:
         raise ValueError("n must be at least one")
     it = iter(iterable)
     while batch := tuple(islice(it, n)):
         yield batch
 
 
-class SNLClustering(AbsTaskClustering):
+class VGClustering(AbsTaskClustering):
     metadata = TaskMetadata(
-        name="SNLClustering",
-        hf_hub_name="navjordj/SNL_summarization",
-        description="Webscrabed articles from the Norwegian lexicon 'Det Store Norske Leksikon'. Uses articles categories as clusters.",
-        reference="https://huggingface.co/datasets/navjordj/SNL_summarization",
+        name="VGClustering",
+        dataset={
+            "path": "navjordj/VG_summarization",
+            "revision": "d4c5a8ba10ae71224752c727094ac4c46947fa29",
+        },
+        description="Articles and their classes (e.g. sports) from VG news articles extracted from Norsk Aviskorpus.",
+        reference="https://huggingface.co/datasets/navjordj/VG_summarization",
         type="Clustering",
         category="p2p",
         eval_splits=["test"],
         eval_langs=["nb"],
         main_score="v_measure",
-        revision="3d3d27aa7af8941408cefc3991ada5d12a4273d1",
         date=("2020-01-01", "2024-12-31"),  # best guess
         form=["written"],
-        domains=["Encyclopaedic", "Non-fiction"],
+        domains=["News", "Non-fiction"],
         license=None,
-        socioeconomic_status="high",
+        socioeconomic_status="mixed",
         annotations_creators="derived",
         dialect=[],
         task_subtypes=["Thematic clustering"],
         text_creation="found",
         bibtex_citation="""@mastersthesis{navjord2023beyond,
-  title={Beyond extractive: advancing abstractive automatic text summarization in Norwegian with transformers},
-  author={Navjord, J{\o}rgen Johnsen and Korsvik, Jon-Mikkel Ryen},
-  year={2023},
-  school={Norwegian University of Life Sciences, {\AA}s}
+    title={Beyond extractive: advancing abstractive automatic text summarization in Norwegian with transformers},
+    author={Navjord, J{\o}rgen Johnsen and Korsvik, Jon-Mikkel Ryen},
+    year={2023},
+    school={Norwegian University of Life Sciences, {\AA}s}
 }""",
         n_samples={"test": 2048},
-        avg_character_length={"test": 1101.30},
+        avg_character_length={"test": 1009.65},
     )
 
-    def load_data(self, **kwargs: dict):  # noqa: ARG002
-        """
-        Load dataset from HuggingFace hub
-        """
-        if self.data_loaded:
-            return
-
-        self.dataset: datasets.DatasetDict = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            revision=self.metadata_dict.get("revision"),
-        )  # type: ignore
-
-        self.dataset_transform()
-        self.data_loaded = True
-
     def dataset_transform(self):
         splits = self.metadata_dict["eval_splits"]
 
         documents: list = []
         labels: list = []
-        label_col = "category"
+        label_col = "classes"
 
         ds = {}
         for split in splits:
             ds_split = self.dataset[split]
 
             _label = self.normalize_labels(ds_split[label_col])
+            documents.extend(ds_split["title"])
+            labels.extend(_label)
+
             documents.extend(ds_split["ingress"])
             labels.extend(_label)
 
             documents.extend(ds_split["article"])
             labels.extend(_label)
 
             assert len(documents) == len(labels)
 
-            rng = random.Random(42)  # local only seed
+            rng = random.Random(1111)  # local only seed
+            # resampling changes scores from 12.68, 11.30, 12.65 (sample model)
             pairs = list(zip(documents, labels))
             rng.shuffle(pairs)
             documents, labels = [list(collection) for collection in zip(*pairs)]
 
             # reduce size of dataset to not have too large datasets in the clustering task
             documents_batched = list(batched(documents, 512))[:4]
             labels_batched = list(batched(labels, 512))[:4]
+            # See:
+            # https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/pull/96
+            # for a discussion on sizes
 
             ds[split] = datasets.Dataset.from_dict(
                 {
                     "sentences": documents_batched,
                     "labels": labels_batched,
                 }
             )
 
         self.dataset = datasets.DatasetDict(ds)
 
     @staticmethod
     def normalize_labels(labels: list[str]) -> list[str]:
-        # example label:
-        # Store norske leksikon,Kunst og estetikk,Musikk,Klassisk musikk,Internasjonale dirigenter
-        # When using 2 levels there is 17 unique labels
-        # When using 3 levels there is 121 unique labels
-        return [",".join(tuple(label.split(",")[:3])) for label in labels]
+        # Agreed on and debated in: https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/issues/83
+        return [label.split(",")[0] for label in labels]
```

### Comparing `mteb-1.4.1/mteb/tasks/Clustering/nb/vg_clustering.py` & `mteb-1.5.0/mteb/tasks/Clustering/nb/snl_clustering.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,102 +16,85 @@
     if n < 1:
         raise ValueError("n must be at least one")
     it = iter(iterable)
     while batch := tuple(islice(it, n)):
         yield batch
 
 
-class VGClustering(AbsTaskClustering):
+class SNLClustering(AbsTaskClustering):
     metadata = TaskMetadata(
-        name="VGClustering",
-        hf_hub_name="navjordj/VG_summarization",
-        description="Articles and their classes (e.g. sports) from VG news articles extracted from Norsk Aviskorpus.",
-        reference="https://huggingface.co/datasets/navjordj/VG_summarization",
+        name="SNLClustering",
+        dataset={
+            "path": "navjordj/SNL_summarization",
+            "revision": "3d3d27aa7af8941408cefc3991ada5d12a4273d1",
+        },
+        description="Webscrabed articles from the Norwegian lexicon 'Det Store Norske Leksikon'. Uses articles categories as clusters.",
+        reference="https://huggingface.co/datasets/navjordj/SNL_summarization",
         type="Clustering",
         category="p2p",
         eval_splits=["test"],
         eval_langs=["nb"],
         main_score="v_measure",
-        revision="d4c5a8ba10ae71224752c727094ac4c46947fa29",
         date=("2020-01-01", "2024-12-31"),  # best guess
         form=["written"],
-        domains=["News", "Non-fiction"],
+        domains=["Encyclopaedic", "Non-fiction"],
         license=None,
-        socioeconomic_status="mixed",
+        socioeconomic_status="high",
         annotations_creators="derived",
         dialect=[],
         task_subtypes=["Thematic clustering"],
         text_creation="found",
         bibtex_citation="""@mastersthesis{navjord2023beyond,
-    title={Beyond extractive: advancing abstractive automatic text summarization in Norwegian with transformers},
-    author={Navjord, J{\o}rgen Johnsen and Korsvik, Jon-Mikkel Ryen},
-    year={2023},
-    school={Norwegian University of Life Sciences, {\AA}s}
+  title={Beyond extractive: advancing abstractive automatic text summarization in Norwegian with transformers},
+  author={Navjord, J{\o}rgen Johnsen and Korsvik, Jon-Mikkel Ryen},
+  year={2023},
+  school={Norwegian University of Life Sciences, {\AA}s}
 }""",
         n_samples={"test": 2048},
-        avg_character_length={"test": 1009.65},
+        avg_character_length={"test": 1101.30},
     )
 
-    def load_data(self, **kwargs: dict):  # noqa: ARG002
-        """
-        Load dataset from HuggingFace hub
-        """
-        if self.data_loaded:
-            return
-
-        self.dataset: datasets.DatasetDict = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            revision=self.metadata_dict.get("revision"),
-        )  # type: ignore
-
-        self.dataset_transform()
-        self.data_loaded = True
-
     def dataset_transform(self):
         splits = self.metadata_dict["eval_splits"]
 
         documents: list = []
         labels: list = []
-        label_col = "classes"
+        label_col = "category"
 
         ds = {}
         for split in splits:
             ds_split = self.dataset[split]
 
             _label = self.normalize_labels(ds_split[label_col])
-            documents.extend(ds_split["title"])
-            labels.extend(_label)
-
             documents.extend(ds_split["ingress"])
             labels.extend(_label)
 
             documents.extend(ds_split["article"])
             labels.extend(_label)
 
             assert len(documents) == len(labels)
 
-            rng = random.Random(1111)  # local only seed
-            # resampling changes scores from 12.68, 11.30, 12.65 (sample model)
+            rng = random.Random(42)  # local only seed
             pairs = list(zip(documents, labels))
             rng.shuffle(pairs)
             documents, labels = [list(collection) for collection in zip(*pairs)]
 
             # reduce size of dataset to not have too large datasets in the clustering task
             documents_batched = list(batched(documents, 512))[:4]
             labels_batched = list(batched(labels, 512))[:4]
-            # See:
-            # https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/pull/96
-            # for a discussion on sizes
 
             ds[split] = datasets.Dataset.from_dict(
                 {
                     "sentences": documents_batched,
                     "labels": labels_batched,
                 }
             )
 
         self.dataset = datasets.DatasetDict(ds)
 
     @staticmethod
     def normalize_labels(labels: list[str]) -> list[str]:
-        # Agreed on and debated in: https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/issues/83
-        return [label.split(",")[0] for label in labels]
+        # example label:
+        # Store norske leksikon,Kunst og estetikk,Musikk,Klassisk musikk,Internasjonale dirigenter
+        # When using 2 levels there is 17 unique labels
+        # When using 3 levels there is 121 unique labels
+        return [",".join(tuple(label.split(",")[:3])) for label in labels]
```

### Comparing `mteb-1.4.1/mteb/tasks/Clustering/pl/PolishClustering.py` & `mteb-1.5.0/mteb/tasks/Clustering/pl/PolishClustering.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 
 class EightTagsClustering(AbsTaskClustering):
     metadata = TaskMetadata(
         name="EightTagsClustering",
         description="Clustering of headlines from social media posts in Polish belonging to 8 categories: film, history, "
         "food, medicine, motorization, work, sport and technology.",
         reference="https://aclanthology.org/2020.lrec-1.207.pdf",
-        hf_hub_name="mteb/polish-clustering",
+        dataset={
+            "path": "mteb/polish-clustering",
+            "revision": "e7a26af6f3ae46b30dde8737f02c07b1505bcc73",
+        },
         type="Clustering",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["pl"],
         main_score="v_measure",
-        revision="e7a26af6f3ae46b30dde8737f02c07b1505bcc73",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Clustering/sv/swedn_clustering.py` & `mteb-1.5.0/mteb/tasks/Clustering/sv/swedn_clustering.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,23 +20,26 @@
     while batch := tuple(islice(it, n)):
         yield batch
 
 
 class SwednClustering(AbsTaskClustering):
     metadata = TaskMetadata(
         name="SwednClustering",
-        hf_hub_name="sbx/superlim-2",
+        dataset={
+            "path": "sbx/superlim-2",
+            "revision": "ef1661775d746e0844b299164773db733bdc0bf6",
+            "name": "swedn",
+        },
         description="The SWE-DN corpus is based on 1,963,576 news articles from the Swedish newspaper Dagens Nyheter (DN) during the years 2000--2020. The articles are filtered to resemble the CNN/DailyMail dataset both regarding textual structure. This dataset uses the category labels as clusters.",
         reference="https://spraakbanken.gu.se/en/resources/swedn",
         type="Clustering",
         category="p2p",
         eval_splits=["all"],
         eval_langs=["sv"],
         main_score="v_measure",
-        revision="ef1661775d746e0844b299164773db733bdc0bf6",
         date=("2000-01-01", "2020-12-31"),  # best guess
         form=["written"],
         domains=["News", "Non-fiction"],
         license=None,
         socioeconomic_status="mixed",
         annotations_creators="derived",
         dialect=[],
@@ -48,30 +51,14 @@
   booktitle={Proceedings of CLARIN Annual Conference},
   year={2021}
 }""",
         n_samples={"all": 2048},
         avg_character_length={"all": 1619.71},
     )
 
-    def load_data(self, **kwargs: dict):  # noqa: ARG002
-        """
-        Load dataset from HuggingFace hub
-        """
-        if self.data_loaded:
-            return
-
-        self.dataset: datasets.DatasetDict = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            "swedn",  # chose the relevant subset
-            revision=self.metadata_dict.get("revision"),
-        )  # type: ignore
-
-        self.dataset_transform()
-        self.data_loaded = True
-
     def dataset_transform(self):
         """
         The article_category clusters differ between the splits (with the test set only having 1 cluster). Therefore we combine it all into one
         cluster.
         """
         splits = ["train", "validation"]
         # performance of sample models with test set: 8.74, 2.43 -removing test-> 11.26, 4.27
```

### Comparing `mteb-1.4.1/mteb/tasks/Clustering/zh/CMTEBClustering.py` & `mteb-1.5.0/mteb/tasks/Clustering/zh/CMTEBClustering.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 
 
 class CLSClusteringS2S(AbsTaskClustering):
     metadata = TaskMetadata(
         name="CLSClusteringS2S",
         description="Clustering of titles from CLS dataset. Clustering of 13 sets on the main category.",
         reference="https://arxiv.org/abs/2209.05034",
-        hf_hub_name="mteb/cls",
+        dataset={
+            "path": "mteb/cls",
+            "revision": "e458b3f5414b62b7f9f83499ac1f5497ae2e869f",
+        },
         type="Clustering",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["zh"],
         main_score="v_measure",
-        revision="e458b3f5414b62b7f9f83499ac1f5497ae2e869f",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -33,21 +35,23 @@
 
 
 class CLSClusteringP2P(AbsTaskClustering):
     metadata = TaskMetadata(
         name="CLSClusteringP2P",
         description="Clustering of titles + abstract from CLS dataset. Clustering of 13 sets on the main category.",
         reference="https://arxiv.org/abs/2209.05034",
-        hf_hub_name="mteb/cls",
+        dataset={
+            "path": "mteb/cls",
+            "revision": "4b6227591c6c1a73bc76b1055f3b7f3588e72476",
+        },
         type="Clustering",
         category="p2p",
         eval_splits=["test"],
         eval_langs=["zh"],
         main_score="v_measure",
-        revision="4b6227591c6c1a73bc76b1055f3b7f3588e72476",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -58,23 +62,25 @@
         avg_character_length=None,
     )
 
 
 class ThuNewsClusteringS2S(AbsTaskClustering):
     metadata = TaskMetadata(
         name="ThuNewsClusteringS2S",
-        hf_hub_name="C-MTEB/ThuNewsClusteringS2S",
+        dataset={
+            "path": "C-MTEB/ThuNewsClusteringS2S",
+            "revision": "8a8b2caeda43f39e13c4bc5bea0f8a667896e10d",
+        },
         description="Clustering of titles from the THUCNews dataset",
         reference="http://thuctc.thunlp.org/",
         type="Clustering",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["zh"],
         main_score="v_measure",
-        revision="8a8b2caeda43f39e13c4bc5bea0f8a667896e10d",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -85,23 +91,25 @@
         avg_character_length=None,
     )
 
 
 class ThuNewsClusteringP2P(AbsTaskClustering):
     metadata = TaskMetadata(
         name="ThuNewsClusteringP2P",
-        hf_hub_name="C-MTEB/ThuNewsClusteringP2P",
+        dataset={
+            "path": "C-MTEB/ThuNewsClusteringP2P",
+            "revision": "5798586b105c0434e4f0fe5e767abe619442cf93",
+        },
         description="Clustering of titles + abstracts from the THUCNews dataset",
         reference="http://thuctc.thunlp.org/",
         type="Clustering",
         category="p2p",
         eval_splits=["test"],
         eval_langs=["zh"],
         main_score="v_measure",
-        revision="5798586b105c0434e4f0fe5e767abe619442cf93",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/PairClassification/en/SprintDuplicateQuestionsPC.py` & `mteb-1.5.0/mteb/tasks/PairClassification/en/SprintDuplicateQuestionsPC.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 
 
 class SprintDuplicateQuestionsPC(AbsTaskPairClassification):
     metadata = TaskMetadata(
         name="SprintDuplicateQuestions",
         description="Duplicate questions from the Sprint community.",
         reference="https://www.aclweb.org/anthology/D18-1131/",
-        hf_hub_name="mteb/sprintduplicatequestions-pairclassification",
+        dataset={
+            "path": "mteb/sprintduplicatequestions-pairclassification",
+            "revision": "d66bd1f72af766a5cc4b0ca5e00c162f89e8cc46",
+        },
         type="PairClassification",
         category="s2s",
         eval_splits=["validation", "test"],
         eval_langs=["en"],
         main_score="ap",
-        revision="d66bd1f72af766a5cc4b0ca5e00c162f89e8cc46",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/PairClassification/en/TwitterSemEval2015PC.py` & `mteb-1.5.0/mteb/tasks/PairClassification/en/TwitterSemEval2015PC.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 
 from ....abstasks.AbsTaskPairClassification import AbsTaskPairClassification
 
 
 class TwitterSemEval2015PC(AbsTaskPairClassification):
     metadata = TaskMetadata(
         name="TwitterSemEval2015",
-        hf_hub_name="mteb/twittersemeval2015-pairclassification",
+        dataset={
+            "path": "mteb/twittersemeval2015-pairclassification",
+            "revision": "70970daeab8776df92f5ea462b6173c0b46fd2d1",
+        },
         description="Paraphrase-Pairs of Tweets from the SemEval 2015 workshop.",
         reference="https://alt.qcri.org/semeval2015/task1/",
         category="s2s",
         type="PairClassification",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="ap",
-        revision="70970daeab8776df92f5ea462b6173c0b46fd2d1",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/PairClassification/en/TwitterURLCorpusPC.py` & `mteb-1.5.0/mteb/tasks/Reranking/fr/AlloprofReranking.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks.AbsTaskPairClassification import AbsTaskPairClassification
+from ....abstasks.AbsTaskReranking import AbsTaskReranking
 
 
-class TwitterURLCorpusPC(AbsTaskPairClassification):
+class AlloprofReranking(AbsTaskReranking):
     metadata = TaskMetadata(
-        name="TwitterURLCorpus",
-        hf_hub_name="mteb/twitterurlcorpus-pairclassification",
-        description="Paraphrase-Pairs of Tweets.",
-        reference="https://languagenet.github.io/",
+        name="AlloprofReranking",
+        description="This dataset was provided by AlloProf, an organisation in Quebec, Canada offering resources and a help forum curated by a large number of teachers to students on all subjects taught from in primary and secondary school",
+        reference="https://huggingface.co/datasets/antoinelb7/alloprof",
+        dataset={
+            "path": "mteb/alloprof-reranking",
+            "revision": "666fdacebe0291776e86f29345663dfaf80a0db9",
+        },
+        type="Reranking",
         category="s2s",
-        type="PairClassification",
         eval_splits=["test"],
-        eval_langs=["en"],
-        main_score="ap",
-        revision="8b6510b0b1fa4e4c4f879467980e9be563ec1cdf",
+        eval_langs=["fr"],
+        main_score="map",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples={"test": 51534},
-        avg_character_length={"test": 79.5},
+        n_samples=None,
+        avg_character_length=None,
     )
```

### Comparing `mteb-1.4.1/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py` & `mteb-1.5.0/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,23 +8,25 @@
 
 _LANGUAGES = ["de", "en", "fi", "fr", "ru", "sv"]
 
 
 class OpusparcusPC(AbsTaskPairClassification, MultilingualTask):
     metadata = TaskMetadata(
         name="OpusparcusPC",
-        hf_hub_name="GEM/opusparcus",
+        dataset={
+            "path": "GEM/opusparcus",
+            "revision": "9e9b1f8ef51616073f47f306f7f47dd91663f86a",
+        },
         description="Opusparcus is a paraphrase corpus for six European language: German, English, Finnish, French, Russian, and Swedish. The paraphrases consist of subtitles from movies and TV shows.",
         reference="https://gem-benchmark.com/data_cards/opusparcus",
         category="s2s",
         type="PairClassification",
         eval_splits=["test.full", "validation.full"],
         eval_langs=_LANGUAGES,
         main_score="ap",
-        revision="9e9b1f8ef51616073f47f306f7f47dd91663f86a",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -40,18 +42,17 @@
         Load dataset from HuggingFace hub
         """
         if self.data_loaded:
             return
         self.dataset = {}
         for lang in self.langs:
             self.dataset[lang] = datasets.load_dataset(
-                self.metadata_dict["hf_hub_name"],
                 lang=lang,
                 quality=100,
-                revision=self.metadata_dict.get("revision", None),
+                **self.metadata_dict["dataset"],
             )
             self.dataset_transform(lang)
         self.data_loaded = True
 
     def dataset_transform(self, lang):
         for split in self.dataset[lang]:
             # Renaming features
```

### Comparing `mteb-1.4.1/mteb/tasks/PairClassification/multilingual/PawsX.py` & `mteb-1.5.0/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2S.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from __future__ import annotations
 
 import datasets
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks import MultilingualTask
-from ....abstasks.AbsTaskPairClassification import AbsTaskPairClassification
+from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class PawsX(MultilingualTask, AbsTaskPairClassification):
+class SpanishPassageRetrievalS2S(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="PawsX",
-        hf_hub_name="paws-x",
-        description="",
-        reference="https://arxiv.org/abs/1908.11828",
+        name="SpanishPassageRetrievalS2S",
+        description="Test collection for passage retrieval from health-related Web resources in Spanish.",
+        reference="https://mklab.iti.gr/results/spanish-passage-retrieval-dataset/",
+        dataset={
+            "path": "jinaai/spanish_passage_retrieval",
+            "revision": "9cddf2ce5209ade52c2115ccfa00eb22c6d3a837",
+        },
+        type="Retrieval",
         category="s2s",
-        type="PairClassification",
-        eval_splits=["test.full", "validation.full"],
-        eval_langs=["de", "en", "es", "fr", "ja", "ko", "zh"],
-        main_score="ap",
-        revision="8a04d940a42cd40658986fdd8e3da561533a3646",
+        eval_splits=["test"],
+        eval_langs=["es"],
+        main_score="ndcg_at_10",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -34,35 +35,35 @@
         avg_character_length=None,
     )
 
     def load_data(self, **kwargs):
         if self.data_loaded:
             return
 
-        self.dataset = dict()
-        for lang in self.langs:
-            hf_dataset = datasets.load_dataset(
-                self.metadata_dict["hf_hub_name"],
-                lang,
-                revision=self.metadata_dict.get("revision", None),
-            )
-
-            sent1 = []
-            sent2 = []
-            labels = []
-
-            for line in hf_dataset["test"]:
-                sent1.append(line["sentence1"])
-                sent2.append(line["sentence2"])
-                labels.append(line["label"])
-
-            self.dataset[lang] = {
-                "test": [
-                    {
-                        "sent1": sent1,
-                        "sent2": sent2,
-                        "labels": labels,
-                    }
-                ]
+        query_rows = datasets.load_dataset(
+            name="queries",
+            split="test",
+            trust_remote_code=True,
+            **self.metadata_dict["dataset"],
+        )
+        corpus_rows = datasets.load_dataset(
+            name="corpus.sentences",
+            split="test",
+            trust_remote_code=True,
+            **self.metadata_dict["dataset"],
+        )
+        qrels_rows = datasets.load_dataset(
+            name="qrels.s2s",
+            split="test",
+            trust_remote_code=True,
+            **self.metadata_dict["dataset"],
+        )
+
+        self.queries = {"test": {row["_id"]: row["text"] for row in query_rows}}
+        self.corpus = {"test": {row["_id"]: row for row in corpus_rows}}
+        self.relevant_docs = {
+            "test": {
+                row["_id"]: {v: 1 for v in row["text"].split(" ")} for row in qrels_rows
             }
+        }
 
         self.data_loaded = True
```

### Comparing `mteb-1.4.1/mteb/tasks/PairClassification/pl/PolishPC.py` & `mteb-1.5.0/mteb/tasks/PairClassification/pl/PolishPC.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 
 from ....abstasks.AbsTaskPairClassification import AbsTaskPairClassification
 
 
 class SickePLPC(AbsTaskPairClassification):
     metadata = TaskMetadata(
         name="SICK-E-PL",
-        hf_hub_name="PL-MTEB/sicke-pl-pairclassification",
+        dataset={
+            "path": "PL-MTEB/sicke-pl-pairclassification",
+            "revision": "5c59e41555244b7e45c9a6be2d720ab4bafae558",
+        },
         description="Polish version of SICK dataset for textual entailment.",
         reference="https://aclanthology.org/2020.lrec-1.207",
         category="s2s",
         type="PairClassification",
         eval_splits=["test"],
         eval_langs=["pl"],
         main_score="ap",
-        revision="5c59e41555244b7e45c9a6be2d720ab4bafae558",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -31,23 +33,25 @@
         avg_character_length=None,
     )
 
 
 class PpcPC(AbsTaskPairClassification):
     metadata = TaskMetadata(
         name="PpcPC",
-        hf_hub_name="PL-MTEB/ppc-pairclassification",
+        dataset={
+            "path": "PL-MTEB/ppc-pairclassification",
+            "revision": "1.0",
+        },
         description="Polish Paraphrase Corpus",
         reference="https://arxiv.org/pdf/2207.12759.pdf",
         category="s2s",
         type="PairClassification",
         eval_splits=["test"],
         eval_langs=["pl"],
         main_score="ap",
-        revision="1.0",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -58,23 +62,25 @@
         avg_character_length=None,
     )
 
 
 class CdscePC(AbsTaskPairClassification):
     metadata = TaskMetadata(
         name="CDSC-E",
-        hf_hub_name="PL-MTEB/cdsce-pairclassification",
+        dataset={
+            "path": "PL-MTEB/cdsce-pairclassification",
+            "revision": "1.0",
+        },
         description="Compositional Distributional Semantics Corpus for textual entailment.",
         reference="https://aclanthology.org/P17-1073.pdf",
         category="s2s",
         type="PairClassification",
         eval_splits=["test"],
         eval_langs=["pl"],
         main_score="ap",
-        revision="1.0",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -85,23 +91,25 @@
         avg_character_length=None,
     )
 
 
 class PscPC(AbsTaskPairClassification):
     metadata = TaskMetadata(
         name="PSC",
-        hf_hub_name="PL-MTEB/psc-pairclassification",
+        dataset={
+            "path": "PL-MTEB/psc-pairclassification",
+            "revision": "1.0",
+        },
         description="Polish Summaries Corpus",
         reference="http://www.lrec-conf.org/proceedings/lrec2014/pdf/1211_Paper.pdf",
         category="s2s",
         type="PairClassification",
         eval_splits=["test"],
         eval_langs=["pl"],
         main_score="ap",
-        revision="1.0",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/PairClassification/zh/CMTEBPairClassification.py` & `mteb-1.5.0/mteb/tasks/Retrieval/pl/ArguAnaPLRetrieval.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,52 +1,28 @@
 from __future__ import annotations
 
-from mteb.abstasks.AbsTaskPairClassification import AbsTaskPairClassification
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-
-class Ocnli(AbsTaskPairClassification):
-    metadata = TaskMetadata(
-        name="Ocnli",
-        description="Original Chinese Natural Language Inference dataset",
-        reference="https://arxiv.org/abs/2010.05444",
-        hf_hub_name="C-MTEB/OCNLI",
-        type="PairClassification",
-        category="s2s",
-        eval_splits=["validation", "test"],
-        eval_langs=["zh"],
-        main_score="accuracy",
-        revision="7bd1ee0ae3a820d8a4b6f8a624063f8504a3564d",
-        date=None,
-        form=None,
-        domains=None,
-        task_subtypes=None,
-        license=None,
-        socioeconomic_status=None,
-        annotations_creators=None,
-        dialect=None,
-        text_creation=None,
-        bibtex_citation=None,
-        n_samples=None,
-        avg_character_length=None,
-    )
+from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class Cmnli(AbsTaskPairClassification):
+class ArguAnaPL(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="Cmnli",
-        description="Chinese Multi-Genre NLI",
-        reference="https://huggingface.co/datasets/clue/viewer/cmnli",
-        hf_hub_name="C-MTEB/CMNLI",
-        type="PairClassification",
-        category="s2s",
-        eval_splits=["validation", "test"],
-        eval_langs=["zh"],
-        main_score="accuracy",
-        revision="41bc36f332156f7adc9e38f53777c959b2ae9766",
+        name="ArguAna-PL",
+        description="ArguAna-PL",
+        reference="https://huggingface.co/datasets/clarin-knext/arguana-pl",
+        dataset={
+            "path": "clarin-knext/arguana-pl",
+            "revision": "63fc86750af76253e8c760fc9e534bbf24d260a2",
+        },
+        type="Retrieval",
+        category="s2p",
+        eval_splits=["test"],
+        eval_langs=["pl"],
+        main_score="ndcg_at_10",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Reranking/en/AskUbuntuDupQuestions.py` & `mteb-1.5.0/mteb/tasks/Reranking/en/AskUbuntuDupQuestions.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 
 
 class AskUbuntuDupQuestions(AbsTaskReranking):
     metadata = TaskMetadata(
         name="AskUbuntuDupQuestions",
         description="AskUbuntu Question Dataset - Questions from AskUbuntu with manual annotations marking pairs of questions as similar or non-similar",
         reference="https://github.com/taolei87/askubuntu",
-        hf_hub_name="mteb/askubuntudupquestions-reranking",
+        dataset={
+            "path": "mteb/askubuntudupquestions-reranking",
+            "revision": "2000358ca161889fa9c082cb41daa8dcfb161a54",
+        },
         type="Reranking",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="map",
-        revision="2000358ca161889fa9c082cb41daa8dcfb161a54",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Reranking/en/MindSmallReranking.py` & `mteb-1.5.0/mteb/tasks/Reranking/en/MindSmallReranking.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 
 
 class MindSmallReranking(AbsTaskReranking):
     metadata = TaskMetadata(
         name="MindSmallReranking",
         description="Microsoft News Dataset: A Large-Scale English Dataset for News Recommendation Research",
         reference="https://msnews.github.io/assets/doc/ACL2020_MIND.pdf",
-        hf_hub_name="mteb/mind_small",
+        dataset={
+            "path": "mteb/mind_small",
+            "revision": "3bdac13927fdc888b903db93b2ffdbd90b295a69",
+        },
         type="Reranking",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="map",
-        revision="3bdac13927fdc888b903db93b2ffdbd90b295a69",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Reranking/en/SciDocsReranking.py` & `mteb-1.5.0/mteb/tasks/Reranking/en/SciDocsReranking.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 
 
 class SciDocsReranking(AbsTaskReranking):
     metadata = TaskMetadata(
         name="SciDocsRR",
         description="Ranking of related scientific papers based on their title.",
         reference="https://allenai.org/data/scidocs",
-        hf_hub_name="mteb/scidocs-reranking",
+        dataset={
+            "path": "mteb/scidocs-reranking",
+            "revision": "d3c5e1fc0b855ab6097bf1cda04dd73947d7caab",
+        },
         type="Reranking",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="map",
-        revision="d3c5e1fc0b855ab6097bf1cda04dd73947d7caab",
         date=None,
         form=["written"],
         domains=["Academic", "Non-fiction"],
         task_subtypes=["Scientific Reranking"],
         license="cc-by-4.0",
         socioeconomic_status="high",
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Reranking/en/StackOverflowDupQuestions.py` & `mteb-1.5.0/mteb/tasks/Reranking/en/StackOverflowDupQuestions.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 
 
 class StackOverflowDupQuestions(AbsTaskReranking):
     metadata = TaskMetadata(
         name="StackOverflowDupQuestions",
         description="Stack Overflow Duplicate Questions Task for questions with the tags Java, JavaScript and Python",
         reference="https://www.microsoft.com/en-us/research/uploads/prod/2019/03/nl4se18LinkSO.pdf",
-        hf_hub_name="mteb/stackoverflowdupquestions-reranking",
+        dataset={
+            "path": "mteb/stackoverflowdupquestions-reranking",
+            "revision": "e185fbe320c72810689fc5848eb6114e1ef5ec69",
+        },
         type="Reranking",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="map",
-        revision="e185fbe320c72810689fc5848eb6114e1ef5ec69",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Reranking/fr/AlloprofReranking.py` & `mteb-1.5.0/mteb/tasks/Reranking/multilingual/MIRACLReranking.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
+from ....abstasks import MultilingualTask
 from ....abstasks.AbsTaskReranking import AbsTaskReranking
 
 
-class AlloprofReranking(AbsTaskReranking):
+class MIRACLReranking(MultilingualTask, AbsTaskReranking):
     metadata = TaskMetadata(
-        name="AlloprofReranking",
-        description="This dataset was provided by AlloProf, an organisation in Quebec, Canada offering resources and a help forum curated by a large number of teachers to students on all subjects taught from in primary and secondary school",
-        reference="https://huggingface.co/datasets/antoinelb7/alloprof",
-        hf_hub_name="mteb/alloprof-reranking",
+        name="MIRACLReranking",
+        description="MIRACL (Multilingual Information Retrieval Across a Continuum of Languages) is a multilingual retrieval dataset that focuses on search across 18 different languages. This task focuses on the German and Spanish subset.",
+        reference="https://project-miracl.github.io/",
+        dataset={
+            "path": "jinaai/miracl",
+            "revision": "d28a029f35c4ff7f616df47b0edf54e6882395e6",
+        },
         type="Reranking",
         category="s2s",
         eval_splits=["test"],
-        eval_langs=["fr"],
+        eval_langs=["de", "es"],
         main_score="map",
-        revision="666fdacebe0291776e86f29345663dfaf80a0db9",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Reranking/fr/SyntecReranking.py` & `mteb-1.5.0/mteb/tasks/Reranking/fr/SyntecReranking.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 
 
 class SyntecReranking(AbsTaskReranking):
     metadata = TaskMetadata(
         name="SyntecReranking",
         description="This dataset has been built from the Syntec Collective bargaining agreement.",
         reference="https://huggingface.co/datasets/lyon-nlp/mteb-fr-reranking-syntec-s2p",
-        hf_hub_name="lyon-nlp/mteb-fr-reranking-syntec-s2p",
+        dataset={
+            "path": "lyon-nlp/mteb-fr-reranking-syntec-s2p",
+            "revision": "b205c5084a0934ce8af14338bf03feb19499c84d",
+        },
         type="Reranking",
         category="s2p",
         eval_splits=["test"],
         eval_langs=["fr"],
         main_score="map",
-        revision="b205c5084a0934ce8af14338bf03feb19499c84d",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Reranking/multilingual/MIRACLReranking.py` & `mteb-1.5.0/mteb/tasks/Retrieval/pl/TRECCOVIDPLRetrieval.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks import MultilingualTask
-from ....abstasks.AbsTaskReranking import AbsTaskReranking
+from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class MIRACLReranking(MultilingualTask, AbsTaskReranking):
+class TRECCOVIDPL(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="MIRACLReranking",
-        description="MIRACL (Multilingual Information Retrieval Across a Continuum of Languages) is a multilingual retrieval dataset that focuses on search across 18 different languages. This task focuses on the German and Spanish subset.",
-        reference="https://project-miracl.github.io/",
-        hf_hub_name="jinaai/miracl",
-        type="Reranking",
-        category="s2s",
+        name="TRECCOVID-PL",
+        description="TRECCOVID is an ad-hoc search challenge based on the COVID-19 dataset containing scientific articles related to the COVID-19 pandemic.",
+        reference="https://ir.nist.gov/covidSubmit/index.html",
+        dataset={
+            "path": "clarin-knext/trec-covid-pl",
+            "revision": "81bcb408f33366c2a20ac54adafad1ae7e877fdd",
+        },
+        type="Retrieval",
+        category="s2p",
         eval_splits=["test"],
-        eval_langs=["de", "es"],
-        main_score="map",
-        revision="d28a029f35c4ff7f616df47b0edf54e6882395e6",
+        eval_langs=["pl"],
+        main_score="ndcg_at_10",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Reranking/zh/CMTEBReranking.py` & `mteb-1.5.0/mteb/tasks/Reranking/zh/CMTEBReranking.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 
 
 class T2Reranking(AbsTaskReranking):
     metadata = TaskMetadata(
         name="T2Reranking",
         description="T2Ranking: A large-scale Chinese Benchmark for Passage Ranking",
         reference="https://arxiv.org/abs/2304.03679",
-        hf_hub_name="C-MTEB/T2Reranking",
+        dataset={
+            "path": "C-MTEB/T2Reranking",
+            "revision": "76631901a18387f85eaa53e5450019b87ad58ef9",
+        },
         type="Reranking",
         category="s2s",
         eval_splits=["dev"],
         eval_langs=["zh"],
         main_score="map",
-        revision="76631901a18387f85eaa53e5450019b87ad58ef9",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -32,21 +34,23 @@
 
 
 class MMarcoReranking(AbsTaskReranking):
     metadata = TaskMetadata(
         name="MMarcoReranking",
         description="mMARCO is a multilingual version of the MS MARCO passage ranking dataset",
         reference="https://github.com/unicamp-dl/mMARCO",
-        hf_hub_name="C-MTEB/Mmarco-reranking",
+        dataset={
+            "path": "C-MTEB/Mmarco-reranking",
+            "revision": "8e0c766dbe9e16e1d221116a3f36795fbade07f6",
+        },
         type="Reranking",
         category="s2s",
         eval_splits=["dev"],
         eval_langs=["zh"],
         main_score="map",
-        revision="8e0c766dbe9e16e1d221116a3f36795fbade07f6",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -59,21 +63,23 @@
 
 
 class CMedQAv1(AbsTaskReranking):
     metadata = TaskMetadata(
         name="CMedQAv1-reranking",
         description="Chinese community medical question answering",
         reference="https://github.com/zhangsheng93/cMedQA",
-        hf_hub_name="C-MTEB/CMedQAv1-reranking",
+        dataset={
+            "path": "C-MTEB/CMedQAv1-reranking",
+            "revision": "cd540c506dae1cf9e9a59c3e06f42030d54e7301",
+        },
         type="Reranking",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["zh"],
         main_score="map",
-        revision="cd540c506dae1cf9e9a59c3e06f42030d54e7301",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -86,21 +92,23 @@
 
 
 class CMedQAv2(AbsTaskReranking):
     metadata = TaskMetadata(
         name="CMedQAv2-reranking",
         description="Chinese community medical question answering",
         reference="https://github.com/zhangsheng93/cMedQA2",
-        hf_hub_name="C-MTEB/CMedQAv2-reranking",
+        dataset={
+            "path": "C-MTEB/CMedQAv2-reranking",
+            "revision": "23d186750531a14a0357ca22cd92d712fd512ea0",
+        },
         type="Reranking",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["zh"],
         main_score="map",
-        revision="23d186750531a14a0357ca22cd92d712fd512ea0",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/__init__.py` & `mteb-1.5.0/mteb/tasks/Retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/da/dan_fever.py` & `mteb-1.5.0/mteb/tasks/Retrieval/da/dan_fever.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import datasets
-
 from mteb.abstasks import AbsTaskRetrieval, TaskMetadata
 
 
 class DanFever(AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="DanFEVER",
-        hf_hub_name="strombergnlp/danfever",
+        dataset={
+            "path": "strombergnlp/danfever",
+            "revision": "5d01e3f6a661d48e127ab5d7e3aaa0dc8331438a",
+        },
         description="A Danish dataset intended for misinformation research. It follows the same format as the English FEVER dataset.",
         reference="https://aclanthology.org/2021.nodalida-main.47/",
         type="Retrieval",
         category="p2p",
         eval_splits=["train"],
         eval_langs=["da"],
         main_score="ndcg_at_10",
-        revision="5d01e3f6a661d48e127ab5d7e3aaa0dc8331438a",
         date=("2020-01-01", "2021-12-31"),  # best guess
         form=["spoken"],
         domains=["Encyclopaedic", "Non-fiction"],
         license="CC BY-SA 4.0",
         socioeconomic_status="mixed",
         annotations_creators="human-annotated",
         dialect=[],
@@ -41,29 +41,14 @@
 }
 """,
         n_samples={"train": 8897},
         avg_character_length={"train": 124.84},
         task_subtypes=["Claim verification"],
     )
 
-    def load_data(self, **kwargs: dict):  # noqa: ARG002
-        """
-        Load dataset from HuggingFace hub
-        """
-        if self.data_loaded:
-            return
-
-        self.dataset: datasets.DatasetDict = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            revision=self.metadata_dict.get("revision"),
-        )  # type: ignore
-
-        self.dataset_transform()
-        self.data_loaded = True
-
     def dataset_transform(self) -> None:
         """
         and transform to a retrieval datset, which have the following attributes
 
         self.corpus = Dict[doc_id, Dict[str, str]] #id => dict with document data like title and text
         self.queries = Dict[query_id, str] #id => query
         self.relevant_docs = Dict[query_id, Dict[[doc_id, score]]
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/da/t2nord_retrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/da/t2nord_retrieval.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,52 +2,39 @@
 
 from mteb.abstasks import AbsTaskRetrieval, TaskMetadata
 
 
 class TV2Nordretrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="TV2Nordretrieval",
-        hf_hub_name="alexandrainst/nordjylland-news-summarization",
+        dataset={
+            "path": "alexandrainst/nordjylland-news-summarization",
+            "revision": "80cdb115ec2ef46d4e926b252f2b59af62d6c070",
+        },
         description="News Article and corresponding summaries extracted from the Danish newspaper TV2 Nord.",
         reference="https://huggingface.co/datasets/alexandrainst/nordjylland-news-summarization",
         type="Retrieval",
         category="p2p",
         eval_splits=["test"],
         eval_langs=["da"],
         main_score="ndcg_at_10",
-        revision="80cdb115ec2ef46d4e926b252f2b59af62d6c070",
         date=("2020-01-01", "2024-12-31"),  # best guess
         form=["written"],
         domains=["News", "Non-fiction"],
         license="CC0",
         socioeconomic_status="high",
         annotations_creators="derived",
         dialect=[],
         text_creation="found",
         bibtex_citation=None,
         n_samples={"test": 4096},
         avg_character_length={"test": 784.11},
         task_subtypes=["Article retrieval"],
     )
 
-    def load_data(self, **kwargs: dict):  # noqa: ARG002
-        """
-        Load dataset from HuggingFace hub
-        """
-        if self.data_loaded:
-            return
-
-        self.dataset: datasets.DatasetDict = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            revision=self.metadata_dict.get("revision"),
-        )  # type: ignore
-
-        self.dataset_transform()
-        self.data_loaded = True
-
     def dataset_transform(self) -> None:
         """
         and transform to a retrieval datset, which have the following attributes
 
         self.corpus = Dict[doc_id, Dict[str, str]] #id => dict with document datas like title and text
         self.queries = Dict[query_id, str] #id => query
         self.relevant_docs = Dict[query_id, Dict[[doc_id, score]]
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/da/twitterhjerne.py` & `mteb-1.5.0/mteb/tasks/Retrieval/da/twitterhjerne.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 
 from mteb.abstasks import AbsTaskRetrieval, TaskMetadata
 
 
 class TwitterHjerneRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="TwitterHjerneRetrieval",
-        hf_hub_name="sorenmulli/da-hashtag-twitterhjerne",
+        dataset={
+            "path": "sorenmulli/da-hashtag-twitterhjerne",
+            "revision": "099ee143c7fdfa6bd7965be8c801cb161c313b29",
+        },
         description="Danish question asked on Twitter with the Hashtag #Twitterhjerne ('Twitter brain') and their corresponding answer.",
         reference="https://huggingface.co/datasets/sorenmulli/da-hashtag-twitterhjerne",
         type="Retrieval",
         category="p2p",
         eval_splits=["train"],
         eval_langs=["da"],
         main_score="ndcg_at_10",
-        revision="099ee143c7fdfa6bd7965be8c801cb161c313b29",
         date=("2006-01-01", "2024-12-31"),  # best guess
         form=["written"],
         domains=["Social"],
         license=None,
         socioeconomic_status="mixed",
         annotations_creators="derived",
         dialect=[],
@@ -31,29 +33,14 @@
 }
 """,
         n_samples={"train": 340},
         avg_character_length={"train": 138.23},
         task_subtypes=["Question answering"],
     )
 
-    def load_data(self, **kwargs: dict):  # noqa: ARG002
-        """
-        Load dataset from HuggingFace hub
-        """
-        if self.data_loaded:
-            return
-
-        self.dataset: datasets.DatasetDict = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            revision=self.metadata_dict.get("revision"),
-        )  # type: ignore
-
-        self.dataset_transform()
-        self.data_loaded = True
-
     def dataset_transform(self) -> None:
         """
         and transform to a retrieval datset, which have the following attributes
 
         self.corpus = Dict[doc_id, Dict[str, str]] #id => dict with document datas like title and text
         self.queries = Dict[query_id, str] #id => query
         self.relevant_docs = Dict[query_id, Dict[[doc_id, score]]
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/de/GerDaLIRRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/de/GerDaLIRRetrieval.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,21 +9,23 @@
 class GerDaLIR(AbsTaskRetrieval):
     _EVAL_SPLIT = "test"
 
     metadata = TaskMetadata(
         name="GerDaLIR",
         description="GerDaLIR is a legal information retrieval dataset created from the Open Legal Data platform.",
         reference="https://github.com/lavis-nlp/GerDaLIR",
-        hf_hub_name="jinaai/ger_da_lir",
+        dataset={
+            "path": "jinaai/ger_da_lir",
+            "revision": "0bb47f1d73827e96964edb84dfe552f62f4fd5eb",
+        },
         type="Retrieval",
         category="s2p",
         eval_splits=[_EVAL_SPLIT],
         eval_langs=["de"],
         main_score="ndcg_at_10",
-        revision="0bb47f1d73827e96964edb84dfe552f62f4fd5eb",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -35,30 +37,26 @@
     )
 
     def load_data(self, **kwargs):
         if self.data_loaded:
             return
 
         query_rows = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            "queries",
-            revision=self.metadata_dict.get("revision", None),
+            name="queries",
             split=self._EVAL_SPLIT,
         )
         corpus_rows = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            "corpus",
-            revision=self.metadata_dict.get("revision", None),
+            name="corpus",
             split=self._EVAL_SPLIT,
+            **self.metadata_dict["dataset"],
         )
         qrels_rows = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            "qrels",
-            revision=self.metadata_dict.get("revision", None),
+            name="qrels",
             split=self._EVAL_SPLIT,
+            **self.metadata_dict["dataset"],
         )
 
         self.queries = {
             self._EVAL_SPLIT: {row["_id"]: row["text"] for row in query_rows}
         }
         self.corpus = {self._EVAL_SPLIT: {row["_id"]: row for row in corpus_rows}}
         self.relevant_docs = {
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/de/GermanDPRRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/de/GermanDPRRetrieval.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,21 +11,23 @@
     _EVAL_SPLIT = "test"
     _LANGUAGE = "de"
 
     metadata = TaskMetadata(
         name="GermanDPR",
         description="GermanDPR is a German Question Answering dataset for open-domain QA. It associates questions with a textual context containing the answer",
         reference="https://www.deepset.ai/germanquad",
-        hf_hub_name="deepset/germanquad",
+        dataset={
+            "path": "deepset/germanquad",
+            "revision": "5129d02422a66be600ac89cd3e8531b4f97d347d",
+        },
         type="Retrieval",
         category="s2p",
         eval_splits=[_EVAL_SPLIT],
         eval_langs=[_LANGUAGE],
         main_score="ndcg_at_10",
-        revision="5129d02422a66be600ac89cd3e8531b4f97d347d",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -52,17 +54,16 @@
         return result
 
     def load_data(self, **kwargs):
         if self.data_loaded:
             return
 
         data = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            revision=self.metadata_dict.get("revision", None),
             split=self._EVAL_SPLIT,
+            **self.metadata_dict["dataset"],
         )
         corpus = dict()
         queries = dict()
         relevant_docs = dict()
         all_docs = dict()
         for i, row in enumerate(data):
             q_id = f"q_{i}"
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/de/GermanQuADRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/fr/AlloprofRetrieval.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,30 @@
 from __future__ import annotations
 
-from collections import defaultdict
-
-from datasets import DatasetDict, load_dataset
+import datasets
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-def load_retrieval_data(hf_hub_name, eval_splits):
-    eval_split = eval_splits[0]
-    corpus_dataset = load_dataset(hf_hub_name, "corpus")
-    queries_dataset = load_dataset(hf_hub_name, "queries")
-    qrels = load_dataset(hf_hub_name + "-qrels")[eval_split]
-
-    corpus = {e["_id"]: {"text": e["text"]} for e in corpus_dataset["corpus"]}
-    queries = {e["_id"]: e["text"] for e in queries_dataset["queries"]}
-    relevant_docs = defaultdict(dict)
-    for e in qrels:
-        relevant_docs[e["query-id"]][e["corpus-id"]] = e["score"]
-
-    corpus = DatasetDict({eval_split: corpus})
-    queries = DatasetDict({eval_split: queries})
-    relevant_docs = DatasetDict({eval_split: relevant_docs})
-    return corpus, queries, relevant_docs
-
-
-class GermanQuADRetrieval(AbsTaskRetrieval):
+class AlloprofRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="GermanQuAD-Retrieval",
-        description="Context Retrieval for German Question Answering",
-        reference="https://www.kaggle.com/datasets/GermanQuAD",
-        hf_hub_name="mteb/germanquad",
+        name="AlloprofRetrieval",
+        description="This dataset was provided by AlloProf, an organisation in Quebec, Canada offering resources and a help forum curated by a large number of teachers to students on all subjects taught from in primary and secondary school",
+        reference="https://huggingface.co/datasets/antoinelb7/alloprof",
+        dataset={
+            "path": "mteb/alloprof",
+            "revision": "392ba3f5bcc8c51f578786c1fc3dae648662cb9b",
+        },
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
-        eval_langs=["de"],
-        main_score="mrr_at_5",
-        revision="f5c87ae5a2e7a5106606314eef45255f03151bb3",
+        eval_langs=["fr"],
+        main_score="ndcg_at_10",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -52,12 +34,33 @@
         n_samples=None,
         avg_character_length=None,
     )
 
     def load_data(self, **kwargs):
         if self.data_loaded:
             return
-
-        self.corpus, self.queries, self.relevant_docs = load_retrieval_data(
-            self.metadata_dict["hf_hub_name"], self.metadata_dict["eval_splits"]
+        # fetch both subsets of the dataset
+        # BUGFIX: the revision is now used
+        corpus_raw = datasets.load_dataset(
+            name="documents",
+            **self.metadata_dict["dataset"],
+        )
+        queries_raw = datasets.load_dataset(
+            name="queries",
+            **self.metadata_dict["dataset"],
         )
+        eval_split = self.metadata_dict["eval_splits"][0]
+        self.queries = {
+            eval_split: {str(q["id"]): q["text"] for q in queries_raw[eval_split]}
+        }
+        self.corpus = {
+            eval_split: {
+                str(d["uuid"]): {"text": d["text"]} for d in corpus_raw["documents"]
+            }
+        }
+
+        self.relevant_docs = {eval_split: {}}
+        for q in queries_raw[eval_split]:
+            for r in q["relevant"]:
+                self.relevant_docs[eval_split][str(q["id"])] = {r: 1}
+
         self.data_loaded = True
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/en/ArguAnaRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/pl/NFCorpusPLRetrieval.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class ArguAna(AbsTaskRetrieval):
+class NFCorpusPL(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="ArguAna",
+        name="NFCorpus-PL",
         description="NFCorpus: A Full-Text Learning to Rank Dataset for Medical Information Retrieval",
-        reference="http://argumentation.bplaced.net/arguana/data",
-        hf_hub_name="mteb/arguana",
+        reference="https://www.cl.uni-heidelberg.de/statnlpgroup/nfcorpus/",
+        dataset={
+            "path": "clarin-knext/nfcorpus-pl",
+            "revision": "9a6f9567fda928260afed2de480d79c98bf0bec0",
+        },
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
-        eval_langs=["en"],
+        eval_langs=["pl"],
         main_score="ndcg_at_10",
-        revision="c22ab2a51041ffd869aaddef7af8d8215647e41a",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/en/CQADupstackAndroidRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackAndroidRetrieval.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 
 
 class CQADupstackAndroidRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="CQADupstackAndroidRetrieval",
         description="CQADupStack: A Benchmark Data Set for Community Question-Answering Research",
         reference="http://nlp.cis.unimelb.edu.au/resources/cqadupstack/",
-        hf_hub_name="mteb/cqadupstack-android",
+        dataset={
+            "path": "mteb/cqadupstack-android",
+            "revision": "f46a197baaae43b4f621051089b82a364682dfeb",
+        },
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="ndcg_at_10",
-        revision="f46a197baaae43b4f621051089b82a364682dfeb",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/en/CQADupstackEnglishRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackEnglishRetrieval.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 
 
 class CQADupstackEnglishRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="CQADupstackEnglishRetrieval",
         description="CQADupStack: A Benchmark Data Set for Community Question-Answering Research",
         reference="http://nlp.cis.unimelb.edu.au/resources/cqadupstack/",
-        hf_hub_name="mteb/cqadupstack-english",
+        dataset={
+            "path": "mteb/cqadupstack-english",
+            "revision": "ad9991cb51e31e31e430383c75ffb2885547b5f0",
+        },
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="ndcg_at_10",
-        revision="ad9991cb51e31e31e430383c75ffb2885547b5f0",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/en/CQADupstackGamingRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackGamingRetrieval.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 
 
 class CQADupstackGamingRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="CQADupstackGamingRetrieval",
         description="CQADupStack: A Benchmark Data Set for Community Question-Answering Research",
         reference="http://nlp.cis.unimelb.edu.au/resources/cqadupstack/",
-        hf_hub_name="mteb/cqadupstack-gaming",
+        dataset={
+            "path": "mteb/cqadupstack-gaming",
+            "revision": "4885aa143210c98657558c04aaf3dc47cfb54340",
+        },
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="ndcg_at_10",
-        revision="4885aa143210c98657558c04aaf3dc47cfb54340",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/en/CQADupstackGisRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackGisRetrieval.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 
 
 class CQADupstackGisRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="CQADupstackGisRetrieval",
         description="CQADupStack: A Benchmark Data Set for Community Question-Answering Research",
         reference="http://nlp.cis.unimelb.edu.au/resources/cqadupstack/",
-        hf_hub_name="mteb/cqadupstack-gis",
+        dataset={
+            "path": "mteb/cqadupstack-gis",
+            "revision": "5003b3064772da1887988e05400cf3806fe491f2",
+        },
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="ndcg_at_10",
-        revision="5003b3064772da1887988e05400cf3806fe491f2",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/en/CQADupstackMathematicaRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackMathematicaRetrieval.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 
 
 class CQADupstackMathematicaRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="CQADupstackMathematicaRetrieval",
         description="CQADupStack: A Benchmark Data Set for Community Question-Answering Research",
         reference="http://nlp.cis.unimelb.edu.au/resources/cqadupstack/",
-        hf_hub_name="mteb/cqadupstack-mathematica",
+        dataset={
+            "path": "mteb/cqadupstack-mathematica",
+            "revision": "90fceea13679c63fe563ded68f3b6f06e50061de",
+        },
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="ndcg_at_10",
-        revision="90fceea13679c63fe563ded68f3b6f06e50061de",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/en/CQADupstackPhysicsRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackPhysicsRetrieval.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 
 
 class CQADupstackPhysicsRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="CQADupstackPhysicsRetrieval",
         description="CQADupStack: A Benchmark Data Set for Community Question-Answering Research",
         reference="http://nlp.cis.unimelb.edu.au/resources/cqadupstack/",
-        hf_hub_name="mteb/cqadupstack-physics",
+        dataset={
+            "path": "mteb/cqadupstack-physics",
+            "revision": "79531abbd1fb92d06c6d6315a0cbbbf5bb247ea4",
+        },
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="ndcg_at_10",
-        revision="79531abbd1fb92d06c6d6315a0cbbbf5bb247ea4",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/en/CQADupstackProgrammersRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/en/MSMARCOv2Retrieval.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class CQADupstackProgrammersRetrieval(AbsTaskRetrieval):
+class MSMARCOv2(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="CQADupstackProgrammersRetrieval",
-        description="CQADupStack: A Benchmark Data Set for Community Question-Answering Research",
-        reference="http://nlp.cis.unimelb.edu.au/resources/cqadupstack/",
-        hf_hub_name="mteb/cqadupstack-programmers",
+        name="MSMARCOv2",
+        dataset={
+            "path": "mteb/msmarco-v2",
+            "revision": "b1663124850d305ab7c470bb0548acf8e2e7ea43",
+        },
+        description="MS MARCO is a collection of datasets focused on deep learning in search",
+        reference="https://microsoft.github.io/msmarco/TREC-Deep-Learning.html",
         type="Retrieval",
         category="s2p",
-        eval_splits=["test"],
+        eval_splits=["train", "dev", "dev2"],
         eval_langs=["en"],
         main_score="ndcg_at_10",
-        revision="6184bc1440d2dbc7612be22b50686b8826d22b32",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/en/CQADupstackStatsRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/pl/SCIDOCSPLRetrieval.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class CQADupstackStatsRetrieval(AbsTaskRetrieval):
+class SCIDOCSPL(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="CQADupstackStatsRetrieval",
-        description="CQADupStack: A Benchmark Data Set for Community Question-Answering Research",
-        reference="http://nlp.cis.unimelb.edu.au/resources/cqadupstack/",
-        hf_hub_name="mteb/cqadupstack-stats",
+        name="SCIDOCS-PL",
+        description="SciDocs, a new evaluation benchmark consisting of seven document-level tasks ranging from citation prediction, to document classification and recommendation.",
+        reference="https://allenai.org/data/scidocs",
+        dataset={
+            "path": "clarin-knext/scidocs-pl",
+            "revision": "45452b03f05560207ef19149545f168e596c9337",
+        },
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
-        eval_langs=["en"],
+        eval_langs=["pl"],
         main_score="ndcg_at_10",
-        revision="65ac3a16b8e91f9cee4c9828cc7c335575432a2a",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/en/CQADupstackTexRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackTexRetrieval.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 
 
 class CQADupstackTexRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="CQADupstackTexRetrieval",
         description="CQADupStack: A Benchmark Data Set for Community Question-Answering Research",
         reference="http://nlp.cis.unimelb.edu.au/resources/cqadupstack/",
-        hf_hub_name="mteb/cqadupstack-tex",
+        dataset={
+            "path": "mteb/cqadupstack-tex",
+            "revision": "6c6430d3a6d36f8d2a829195bc5dc94d7e063e53",
+        },
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="ndcg_at_10",
-        revision="6c6430d3a6d36f8d2a829195bc5dc94d7e063e53",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/en/CQADupstackUnixRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackUnixRetrieval.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 
 
 class CQADupstackUnixRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="CQADupstackUnixRetrieval",
         description="CQADupStack: A Benchmark Data Set for Community Question-Answering Research",
         reference="http://nlp.cis.unimelb.edu.au/resources/cqadupstack/",
-        hf_hub_name="mteb/cqadupstack-unix",
+        dataset={
+            "path": "mteb/cqadupstack-unix",
+            "revision": "6c6430d3a6d36f8d2a829195bc5dc94d7e063e53",
+        },
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="ndcg_at_10",
-        revision="6c6430d3a6d36f8d2a829195bc5dc94d7e063e53",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/en/CQADupstackWebmastersRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackWordpressRetrieval.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class CQADupstackWebmastersRetrieval(AbsTaskRetrieval):
+class CQADupstackWordpressRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="CQADupstackWebmastersRetrieval",
+        name="CQADupstackWordpressRetrieval",
+        dataset={
+            "path": "mteb/cqadupstack-wordpress",
+            "revision": "4ffe81d471b1924886b33c7567bfb200e9eec5c4",
+        },
         description="CQADupStack: A Benchmark Data Set for Community Question-Answering Research",
         reference="http://nlp.cis.unimelb.edu.au/resources/cqadupstack/",
-        hf_hub_name="mteb/cqadupstack-webmasters",
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="ndcg_at_10",
-        revision="160c094312a0e1facb97e55eeddb698c0abe3571",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/en/CQADupstackWordpressRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/pl/HotpotQAPLRetrieval.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class CQADupstackWordpressRetrieval(AbsTaskRetrieval):
+class HotpotQAPL(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="CQADupstackWordpressRetrieval",
-        hf_hub_name="mteb/cqadupstack-wordpress",
-        description="CQADupStack: A Benchmark Data Set for Community Question-Answering Research",
-        reference="http://nlp.cis.unimelb.edu.au/resources/cqadupstack/",
+        name="HotpotQA-PL",
+        description="HotpotQA is a question answering dataset featuring natural, multi-hop questions, with strong supervision for supporting facts to enable more explainable question answering systems.",
+        reference="https://hotpotqa.github.io/",
+        dataset={
+            "path": "clarin-knext/hotpotqa-pl",
+            "revision": "a0bd479ac97b4ccb5bd6ce320c415d0bb4beb907",
+        },
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
-        eval_langs=["en"],
+        eval_langs=["pl"],
         main_score="ndcg_at_10",
-        revision="4ffe81d471b1924886b33c7567bfb200e9eec5c4",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/en/ClimateFEVERRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/en/FEVERRetrieval.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class ClimateFEVER(AbsTaskRetrieval):
+class FEVER(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="ClimateFEVER",
-        description="CLIMATE-FEVER is a dataset adopting the FEVER methodology that consists of 1,535 real-world claims regarding climate-change. ",
-        reference="https://www.sustainablefinance.uzh.ch/en/research/climate-fever.html",
-        hf_hub_name="mteb/climate-fever",
+        name="FEVER",
+        dataset={
+            "path": "mteb/fever",
+            "revision": "bea83ef9e8fb933d90a2f1d5515737465d613e12",
+        },
+        description=(
+            "FEVER (Fact Extraction and VERification) consists of 185,445 claims generated by altering sentences"
+            " extracted from Wikipedia and subsequently verified without knowledge of the sentence they were"
+            " derived from."
+        ),
+        reference="https://fever.ai/",
         type="Retrieval",
         category="s2p",
-        eval_splits=["test"],
+        eval_splits=["train", "dev", "test"],
         eval_langs=["en"],
         main_score="ndcg_at_10",
-        revision="47f2ac6acb640fc46020b02a5b59fdda04d39380",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/en/DBPediaRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/pl/MSMARCOPLRetrieval.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class DBPedia(AbsTaskRetrieval):
+class MSMARCOPL(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="DBPedia",
-        description="DBpedia-Entity is a standard test collection for entity search over the DBpedia knowledge base",
-        reference="https://github.com/iai-group/DBpedia-Entity/",
-        hf_hub_name="mteb/dbpedia",
+        name="MSMARCO-PL",
+        description="MS MARCO is a collection of datasets focused on deep learning in search",
+        reference="https://microsoft.github.io/msmarco/",
+        dataset={
+            "path": "clarin-knext/msmarco-pl",
+            "revision": "8634c07806d5cce3a6138e260e59b81760a0a640",
+        },
         type="Retrieval",
         category="s2p",
-        eval_splits=["dev", "test"],
-        eval_langs=["en"],
+        eval_splits=["test"],
+        eval_langs=["pl"],
         main_score="ndcg_at_10",
-        revision="c0f706b76e590d620bd6618b3ca8efdd34e2d659",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/en/FEVERRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/en/TRECCOVIDRetrieval.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class FEVER(AbsTaskRetrieval):
+class TRECCOVID(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="FEVER",
-        hf_hub_name="mteb/fever",
-        description=(
-            "FEVER (Fact Extraction and VERification) consists of 185,445 claims generated by altering sentences"
-            " extracted from Wikipedia and subsequently verified without knowledge of the sentence they were"
-            " derived from."
-        ),
-        reference="https://fever.ai/",
+        name="TRECCOVID",
+        description="TRECCOVID is an ad-hoc search challenge based on the COVID-19 dataset containing scientific articles related to the COVID-19 pandemic.",
+        reference="https://ir.nist.gov/covidSubmit/index.html",
+        dataset={
+            "path": "mteb/trec-covid",
+            "revision": "1271c7809071a13532e05f25fb53511ffce77117",
+        },
         type="Retrieval",
         category="s2p",
-        eval_splits=["train", "dev", "test"],
+        eval_splits=["test"],
         eval_langs=["en"],
         main_score="ndcg_at_10",
-        revision="bea83ef9e8fb933d90a2f1d5515737465d613e12",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/en/FiQA2018Retrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/en/FiQA2018Retrieval.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 
 
 class FiQA2018(AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="FiQA2018",
         description="Financial Opinion Mining and Question Answering",
         reference="https://sites.google.com/view/fiqa/",
-        hf_hub_name="mteb/fiqa",
+        dataset={
+            "path": "mteb/fiqa",
+            "revision": "27a168819829fe9bcd655c2df245fb19452e8e06",
+        },
         type="Retrieval",
         category="s2p",
         eval_splits=["train", "dev", "test"],
         eval_langs=["en"],
         main_score="ndcg_at_10",
-        revision="27a168819829fe9bcd655c2df245fb19452e8e06",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/en/HagridRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/en/HagridRetrieval.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,27 +9,29 @@
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
 class HagridRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="HagridRetrieval",
-        hf_hub_name="miracl/hagrid",
+        dataset={
+            "path": "miracl/hagrid",
+            "revision": "b2a085913606be3c4f2f1a8bff1810e38bade8fa",
+        },
         reference="https://github.com/project-miracl/hagrid",
         description=(
             "HAGRID (Human-in-the-loop Attributable Generative Retrieval for Information-seeking Dataset)"
             "is a dataset for generative information-seeking scenarios. It consists of queries"
             "along with a set of manually labelled relevant passages"
         ),
         type="Retrieval",
         category="s2p",
         eval_splits=["dev"],
         eval_langs=["en"],
         main_score="ndcg_at_10",
-        revision="b2a085913606be3c4f2f1a8bff1810e38bade8fa",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -46,15 +48,15 @@
         """
         if self.data_loaded:
             return
 
         data = datasets.load_dataset(
             "miracl/hagrid",
             split=self.metadata.eval_splits[0],
-            revision=self.metadata_dict.get("revision", None),
+            revision=self.metadata_dict["dataset"].get("revision", None),
         )
         proc_data = self.preprocess_data(data)
 
         self.queries = {
             self.metadata.eval_splits[0]: {
                 d["query_id"]: d["query_text"] for d in proc_data
             }
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/en/HotpotQARetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/en/NFCorpusRetrieval.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class HotpotQA(AbsTaskRetrieval):
+class NFCorpus(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="HotpotQA",
-        hf_hub_name="mteb/hotpotqa",
-        description=(
-            "HotpotQA is a question answering dataset featuring natural, multi-hop questions, with strong"
-            " supervision for supporting facts to enable more explainable question answering systems."
-        ),
-        reference="https://hotpotqa.github.io/",
+        name="NFCorpus",
+        dataset={
+            "path": "mteb/nfcorpus",
+            "revision": "ec0fa4fe99da2ff19ca1214b7966684033a58814",
+        },
+        description="NFCorpus: A Full-Text Learning to Rank Dataset for Medical Information Retrieval",
+        reference="https://www.cl.uni-heidelberg.de/statnlpgroup/nfcorpus/",
         type="Retrieval",
         category="s2p",
-        eval_splits=["train", "dev", "test"],
+        eval_splits=["test"],
         eval_langs=["en"],
         main_score="ndcg_at_10",
-        revision="ab518f4d6fcca38d87c25209f94beba119d02014",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/en/MSMARCORetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/en/QuoraRetrieval.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class MSMARCO(AbsTaskRetrieval):
+class QuoraRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="MSMARCO",
-        hf_hub_name="mteb/msmarco",
-        description="MS MARCO is a collection of datasets focused on deep learning in search",
-        reference="https://microsoft.github.io/msmarco/",
+        name="QuoraRetrieval",
+        dataset={
+            "path": "mteb/quora",
+            "revision": "0be27e93455051e531182b85e85e425aba12e9d4",
+        },
+        description=(
+            "QuoraRetrieval is based on questions that are marked as duplicates on the Quora platform. Given a"
+            " question, find other (duplicate) questions."
+        ),
+        reference="https://quoradata.quora.com/First-Quora-Dataset-Release-Question-Pairs",
         type="Retrieval",
-        category="s2p",
-        eval_splits=["train", "dev", "test"],
+        category="s2s",
+        eval_splits=["dev", "test"],
         eval_langs=["en"],
         main_score="ndcg_at_10",
-        revision="c5a29a104738b98a9e76336939199e264163d4a0",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/en/MSMARCOv2Retrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/en/MSMARCORetrieval.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class MSMARCOv2(AbsTaskRetrieval):
+class MSMARCO(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="MSMARCOv2",
-        hf_hub_name="mteb/msmarco-v2",
+        name="MSMARCO",
+        dataset={
+            "path": "mteb/msmarco",
+            "revision": "c5a29a104738b98a9e76336939199e264163d4a0",
+        },
         description="MS MARCO is a collection of datasets focused on deep learning in search",
-        reference="https://microsoft.github.io/msmarco/TREC-Deep-Learning.html",
+        reference="https://microsoft.github.io/msmarco/",
         type="Retrieval",
         category="s2p",
-        eval_splits=["train", "dev", "dev2"],
+        eval_splits=["train", "dev", "test"],
         eval_langs=["en"],
         main_score="ndcg_at_10",
-        revision="b1663124850d305ab7c470bb0548acf8e2e7ea43",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/en/NFCorpusRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/en/SCIDOCSRetrieval.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class NFCorpus(AbsTaskRetrieval):
+class SCIDOCS(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="NFCorpus",
-        hf_hub_name="mteb/nfcorpus",
-        description="NFCorpus: A Full-Text Learning to Rank Dataset for Medical Information Retrieval",
-        reference="https://www.cl.uni-heidelberg.de/statnlpgroup/nfcorpus/",
+        name="SCIDOCS",
+        dataset={
+            "path": "mteb/scidocs",
+            "revision": "56a6d0140cf6356659e2a7c1413286a774468d44",
+        },
+        description=(
+            "SciDocs, a new evaluation benchmark consisting of seven document-level tasks ranging from citation"
+            " prediction, to document classification and recommendation."
+        ),
+        reference="https://allenai.org/data/scidocs",
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="ndcg_at_10",
-        revision="ec0fa4fe99da2ff19ca1214b7966684033a58814",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/en/NQRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/en/ArguAnaRetrieval.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class NQ(AbsTaskRetrieval):
+class ArguAna(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="NQ",
-        hf_hub_name="mteb/nq",
+        name="ArguAna",
         description="NFCorpus: A Full-Text Learning to Rank Dataset for Medical Information Retrieval",
-        reference="https://ai.google.com/research/NaturalQuestions/",
+        reference="http://argumentation.bplaced.net/arguana/data",
+        dataset={
+            "path": "mteb/arguana",
+            "revision": "c22ab2a51041ffd869aaddef7af8d8215647e41a",
+        },
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="ndcg_at_10",
-        revision="b774495ed302d8c44a3a7ea25c90dbce03968f31",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/en/NarrativeQARetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/en/NarrativeQARetrieval.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,26 +8,28 @@
 
 
 class NarrativeQARetrieval(AbsTaskRetrieval):
     _EVAL_SPLIT = "test"
 
     metadata = TaskMetadata(
         name="NarrativeQARetrieval",
-        hf_hub_name="narrativeqa",
+        dataset={
+            "path": "narrativeqa",
+            "revision": "2e643e7363944af1c33a652d1c87320d0871c4e4",
+        },
         reference="https://metatext.io/datasets/narrativeqa",
         description=(
             "NarrativeQA is a dataset for the task of question answering on long narratives. It consists of "
             "realistic QA instances collected from literature (fiction and non-fiction) and movie scripts. "
         ),
         type="Retrieval",
         category="s2p",
         eval_splits=[_EVAL_SPLIT],
         eval_langs=["en"],
         main_score="ndcg_at_10",
-        revision="2e643e7363944af1c33a652d1c87320d0871c4e4",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -39,15 +41,17 @@
     )
 
     def load_data(self, **kwargs):
         if self.data_loaded:
             return
 
         data = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"], split=self._EVAL_SPLIT
+            split=self._EVAL_SPLIT
+            # BUGFIX: the revision is now used
+            ** self.metadata_dict["dataset"],
         )
         self.queries = {
             self._EVAL_SPLIT: {
                 str(i): row["question"]["text"] for i, row in enumerate(data)
             }
         }
         self.corpus = {
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/en/QuoraRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/pl/QuoraPLRetrieval.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class QuoraRetrieval(AbsTaskRetrieval):
+class QuoraPLRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="QuoraRetrieval",
-        hf_hub_name="mteb/quora",
-        description=(
-            "QuoraRetrieval is based on questions that are marked as duplicates on the Quora platform. Given a"
-            " question, find other (duplicate) questions."
-        ),
+        name="Quora-PL",
+        description="QuoraRetrieval is based on questions that are marked as duplicates on the Quora platform. Given a question, find other (duplicate) questions.",
         reference="https://quoradata.quora.com/First-Quora-Dataset-Release-Question-Pairs",
+        dataset={
+            "path": "clarin-knext/quora-pl",
+            "revision": "0be27e93455051e531182b85e85e425aba12e9d4",
+        },
         type="Retrieval",
         category="s2s",
-        eval_splits=["dev", "test"],
-        eval_langs=["en"],
+        eval_splits=["validation", "test"],  # validation for new DataLoader
+        eval_langs=["pl"],
         main_score="ndcg_at_10",
-        revision="0be27e93455051e531182b85e85e425aba12e9d4",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/en/SCIDOCSRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/pl/SciFactPLRetrieval.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class SCIDOCS(AbsTaskRetrieval):
+class SciFactPL(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="SCIDOCS",
-        hf_hub_name="mteb/scidocs",
-        description=(
-            "SciDocs, a new evaluation benchmark consisting of seven document-level tasks ranging from citation"
-            " prediction, to document classification and recommendation."
-        ),
-        reference="https://allenai.org/data/scidocs",
+        name="SciFact-PL",
+        description="SciFact verifies scientific claims using evidence from the research literature containing scientific paper abstracts.",
+        reference="https://github.com/allenai/scifact",
+        dataset={
+            "path": "clarin-knext/scifact-pl",
+            "revision": "47932a35f045ef8ed01ba82bf9ff67f6e109207e",
+        },
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
-        eval_langs=["en"],
+        eval_langs=["pl"],
         main_score="ndcg_at_10",
-        revision="56a6d0140cf6356659e2a7c1413286a774468d44",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/en/SciFactRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/ko/KoMrtydi.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class SciFact(AbsTaskRetrieval):
+class KoMrtydi(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="SciFact",
-        hf_hub_name="mteb/scifact",
-        description="SciFact verifies scientific claims using evidence from the research literature containing scientific paper abstracts.",
-        reference="https://github.com/allenai/scifact",
+        name="Ko-mrtydi",
+        description="Ko-mrtydi",
+        reference=None,
+        dataset={
+            "path": "taeminlee/Ko-mrtydi",
+            "revision": "71a2e011a42823051a2b4eb303a3366bdbe048d3",
+        },
         type="Retrieval",
         category="s2p",
-        eval_splits=["train", "test"],
-        eval_langs=["en"],
+        eval_splits=["dev"],
+        eval_langs=["ko"],
         main_score="ndcg_at_10",
-        revision="0228b52cf27578f30900b9e5271d331663a030d7",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/en/TRECCOVIDRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/en/Touche2020Retrieval.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class TRECCOVID(AbsTaskRetrieval):
+class Touche2020(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="TRECCOVID",
-        description="TRECCOVID is an ad-hoc search challenge based on the COVID-19 dataset containing scientific articles related to the COVID-19 pandemic.",
-        reference="https://ir.nist.gov/covidSubmit/index.html",
-        hf_hub_name="mteb/trec-covid",
+        name="Touche2020",
+        description="Touché Task 1: Argument Retrieval for Controversial Questions",
+        reference="https://webis.de/events/touche-20/shared-task-1.html",
+        dataset={
+            "path": "mteb/touche2020",
+            "revision": "a34f9a33db75fa0cbb21bb5cfc3dae8dc8bec93f",
+        },
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="ndcg_at_10",
-        revision="1271c7809071a13532e05f25fb53511ffce77117",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/en/Touche2020Retrieval.py` & `mteb-1.5.0/mteb/tasks/STS/en/SickrSTS.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
+from ....abstasks.AbsTaskSTS import AbsTaskSTS
 
 
-class Touche2020(AbsTaskRetrieval):
+class SickrSTS(AbsTaskSTS):
     metadata = TaskMetadata(
-        name="Touche2020",
-        description="Touché Task 1: Argument Retrieval for Controversial Questions",
-        reference="https://webis.de/events/touche-20/shared-task-1.html",
-        hf_hub_name="mteb/touche2020",
-        type="Retrieval",
-        category="s2p",
+        name="SICK-R",
+        dataset={
+            "path": "MMathematica/sickr-sts",
+            "revision": "a6ea5a8cab320b040a23452cc28066d9beae2cee",
+        },
+        description="Semantic Textual Similarity SICK-R dataset as described here:",
+        reference="https://aclanthology.org/2020.lrec-1.207",
+        type="STS",
+        category="s2s",
         eval_splits=["test"],
         eval_langs=["en"],
-        main_score="ndcg_at_10",
-        revision="a34f9a33db75fa0cbb21bb5cfc3dae8dc8bec93f",
+        main_score="cosine_spearman",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
+
+    @property
+    def metadata_dict(self) -> dict[str, str]:
+        metadata_dict = super().metadata_dict
+        metadata_dict["min_score"] = 0
+        metadata_dict["max_score"] = 5
+        return metadata_dict
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2P.py` & `mteb-1.5.0/mteb/tasks/Retrieval/fr/BSARDRetrieval.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 import datasets
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class SpanishPassageRetrievalS2P(AbsTaskRetrieval):
+class BSARDRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="SpanishPassageRetrievalS2P",
-        description="Test collection for passage retrieval from health-related Web resources in Spanish.",
-        reference="https://mklab.iti.gr/results/spanish-passage-retrieval-dataset/",
-        hf_hub_name="jinaai/spanish_passage_retrieval",
+        name="BSARDRetrieval",
+        description="The Belgian Statutory Article Retrieval Dataset (BSARD) is a French native dataset for studying legal information retrieval. BSARD consists of more than 22,600 statutory articles from Belgian law and about 1,100 legal questions posed by Belgian citizens and labeled by experienced jurists with relevant articles from the corpus.",
+        reference="https://huggingface.co/datasets/maastrichtlawtech/bsard",
+        dataset={
+            "path": "mteb/bsard",
+            "revision": "5effa1b9b5fa3b0f9e12523e6e43e5f86a6e6d59",
+        },
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
-        eval_langs=["es"],
-        main_score="ndcg_at_10",
-        revision="9cddf2ce5209ade52c2115ccfa00eb22c6d3a837",
+        eval_langs=["fr"],
+        main_score="ndcg_at_100",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -32,36 +34,40 @@
         n_samples=None,
         avg_character_length=None,
     )
 
     def load_data(self, **kwargs):
         if self.data_loaded:
             return
-
-        query_rows = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            "queries",
-            split="test",
-            trust_remote_code=True,
-        )
-        corpus_rows = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            "corpus.documents",
-            split="test",
-            trust_remote_code=True,
+        # fetch both subsets of the dataset, only test split
+        corpus_raw = datasets.load_dataset(
+            name="corpus",
+            split="corpus",
+            **self.metadata_dict["dataset"],
         )
-        qrels_rows = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            "qrels.s2p",
-            split="test",
-            trust_remote_code=True,
+        queries_raw = datasets.load_dataset(
+            name="questions",
+            split=self.metadata.eval_splits[0],
+            **self.metadata_dict["dataset"],
         )
 
-        self.queries = {"test": {row["_id"]: row["text"] for row in query_rows}}
-        self.corpus = {"test": {row["_id"]: row for row in corpus_rows}}
-        self.relevant_docs = {
-            "test": {
-                row["_id"]: {v: 1 for v in row["text"].split(" ")} for row in qrels_rows
+        self.queries = {
+            self.metadata.eval_splits[0]: {
+                str(q["id"]): " ".join((q["question"] + q["extra_description"]))
+                for q in queries_raw
+            }
+        }
+
+        self.corpus = {
+            self.metadata.eval_splits[0]: {
+                str(d["id"]): {"text": d["article"]} for d in corpus_raw
             }
         }
 
+        self.relevant_docs = {self.metadata.eval_splits[0]: {}}
+        for q in queries_raw:
+            for doc_id in q["article_ids"]:
+                self.relevant_docs[self.metadata.eval_splits[0]][str(q["id"])] = {
+                    str(doc_id): 1
+                }
+
         self.data_loaded = True
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2S.py` & `mteb-1.5.0/mteb/tasks/STS/pl/PolishSTS.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,67 +1,76 @@
 from __future__ import annotations
 
-import datasets
-
+from mteb.abstasks.AbsTaskSTS import AbsTaskSTS
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
+
+class SickrPLSTS(AbsTaskSTS):
+    metadata = TaskMetadata(
+        name="SICK-R-PL",
+        dataset={
+            "path": "PL-MTEB/sickr-pl-sts",
+            "revision": "a6ea5a8cab320b040a23452cc28066d9beae2cee",
+        },
+        description="Polish version of SICK dataset for textual relatedness.",
+        reference="https://aclanthology.org/2020.lrec-1.207",
+        type="STS",
+        category="s2s",
+        eval_splits=["test"],
+        eval_langs=["pl"],
+        main_score="cosine_spearman",
+        date=None,
+        form=None,
+        domains=None,
+        task_subtypes=None,
+        license=None,
+        socioeconomic_status=None,
+        annotations_creators=None,
+        dialect=None,
+        text_creation=None,
+        bibtex_citation=None,
+        n_samples={"test": 9812},
+        avg_character_length={"test": 42.8},
+    )
+
+    @property
+    def metadata_dict(self) -> dict[str, str]:
+        metadata_dict = super().metadata_dict
+        metadata_dict["min_score"] = 1
+        metadata_dict["max_score"] = 5
+        return metadata_dict
 
 
-class SpanishPassageRetrievalS2S(AbsTaskRetrieval):
+class CdscrSTS(AbsTaskSTS):
     metadata = TaskMetadata(
-        name="SpanishPassageRetrievalS2S",
-        description="Test collection for passage retrieval from health-related Web resources in Spanish.",
-        reference="https://mklab.iti.gr/results/spanish-passage-retrieval-dataset/",
-        hf_hub_name="jinaai/spanish_passage_retrieval",
-        type="Retrieval",
+        name="CDSC-R",
+        dataset={
+            "path": "PL-MTEB/cdscr-sts",
+            "revision": "1de08520a7b361e92ffa2a2201ebd41942c54675",
+        },
+        description="Compositional Distributional Semantics Corpus for textual relatedness.",
+        reference="https://aclanthology.org/P17-1073.pdf",
+        type="STS",
         category="s2s",
         eval_splits=["test"],
-        eval_langs=["es"],
-        main_score="ndcg_at_10",
-        revision="9cddf2ce5209ade52c2115ccfa00eb22c6d3a837",
+        eval_langs=["pl"],
+        main_score="cosine_spearman",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
-    def load_data(self, **kwargs):
-        if self.data_loaded:
-            return
-
-        query_rows = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            "queries",
-            split="test",
-            trust_remote_code=True,
-        )
-        corpus_rows = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            "corpus.sentences",
-            split="test",
-            trust_remote_code=True,
-        )
-        qrels_rows = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            "qrels.s2s",
-            split="test",
-            trust_remote_code=True,
-        )
-
-        self.queries = {"test": {row["_id"]: row["text"] for row in query_rows}}
-        self.corpus = {"test": {row["_id"]: row for row in corpus_rows}}
-        self.relevant_docs = {
-            "test": {
-                row["_id"]: {v: 1 for v in row["text"].split(" ")} for row in qrels_rows
-            }
-        }
-
-        self.data_loaded = True
+    @property
+    def metadata_dict(self) -> dict[str, str]:
+        metadata_dict = super().metadata_dict
+        metadata_dict["min_score"] = 1
+        metadata_dict["max_score"] = 5
+        return metadata_dict
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/fr/AlloprofRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/fr/SyntecRetrieval.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,26 +3,30 @@
 import datasets
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class AlloprofRetrieval(AbsTaskRetrieval):
+class SyntecRetrieval(AbsTaskRetrieval):
+    _EVAL_SPLITS = ["test"]
+
     metadata = TaskMetadata(
-        name="AlloprofRetrieval",
-        description="This dataset was provided by AlloProf, an organisation in Quebec, Canada offering resources and a help forum curated by a large number of teachers to students on all subjects taught from in primary and secondary school",
-        reference="https://huggingface.co/datasets/antoinelb7/alloprof",
-        hf_hub_name="mteb/alloprof",
+        name="SyntecRetrieval",
+        description="This dataset has been built from the Syntec Collective bargaining agreement.",
+        reference="https://huggingface.co/datasets/lyon-nlp/mteb-fr-retrieval-syntec-s2p",
+        dataset={
+            "path": "lyon-nlp/mteb-fr-retrieval-syntec-s2p",
+            "revision": "b205c5084a0934ce8af14338bf03feb19499c84d",
+        },
         type="Retrieval",
         category="s2p",
-        eval_splits=["test"],
+        eval_splits=_EVAL_SPLITS,
         eval_langs=["fr"],
-        main_score="ndcg_at_10",
-        revision="392ba3f5bcc8c51f578786c1fc3dae648662cb9b",
+        main_score="map",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -33,29 +37,37 @@
         avg_character_length=None,
     )
 
     def load_data(self, **kwargs):
         if self.data_loaded:
             return
         # fetch both subsets of the dataset
+        # BUGFIX: the revision is now used
         corpus_raw = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"], "documents"
+            name="documents",
+            **self.metadata_dict["dataset"],
         )
         queries_raw = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"], "queries"
+            name="queries",
+            **self.metadata_dict["dataset"],
         )
-        eval_split = self.metadata_dict["eval_splits"][0]
+
         self.queries = {
-            eval_split: {str(q["id"]): q["text"] for q in queries_raw[eval_split]}
+            self._EVAL_SPLITS[0]: {
+                str(i): q["Question"] for i, q in enumerate(queries_raw["queries"])
+            }
         }
+
+        corpus_raw = corpus_raw["documents"]
+        corpus_raw = corpus_raw.rename_column("content", "text")
         self.corpus = {
-            eval_split: {
-                str(d["uuid"]): {"text": d["text"]} for d in corpus_raw["documents"]
-            }
+            self._EVAL_SPLITS[0]: {str(row["id"]): row for row in corpus_raw}
         }
 
-        self.relevant_docs = {eval_split: {}}
-        for q in queries_raw[eval_split]:
-            for r in q["relevant"]:
-                self.relevant_docs[eval_split][str(q["id"])] = {r: 1}
+        self.relevant_docs = {
+            self._EVAL_SPLITS[0]: {
+                str(i): {str(q["Article"]): 1}
+                for i, q in enumerate(queries_raw["queries"])
+            }
+        }
 
         self.data_loaded = True
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/fr/SyntecRetrieval.py` & `mteb-1.5.0/mteb/tasks/STS/es/STSES.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,68 +1,52 @@
 from __future__ import annotations
 
-import datasets
+from datasets import load_dataset
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
+from ....abstasks.AbsTaskSTS import AbsTaskSTS
 
+_EVAL_SPLIT = "test"
 
-class SyntecRetrieval(AbsTaskRetrieval):
-    _EVAL_SPLITS = ["test"]
 
+class STSES(AbsTaskSTS):
     metadata = TaskMetadata(
-        name="SyntecRetrieval",
-        description="This dataset has been built from the Syntec Collective bargaining agreement.",
-        reference="https://huggingface.co/datasets/lyon-nlp/mteb-fr-retrieval-syntec-s2p",
-        hf_hub_name="lyon-nlp/mteb-fr-retrieval-syntec-s2p",
-        type="Retrieval",
-        category="s2p",
-        eval_splits=_EVAL_SPLITS,
-        eval_langs=["fr"],
-        main_score="map",
-        revision="b205c5084a0934ce8af14338bf03feb19499c84d",
+        name="STSES",
+        dataset={
+            "path": "PlanTL-GOB-ES/sts-es",
+            "revision": "0912bb6c9393c76d62a7c5ee81c4c817ff47c9f4",
+            "trust_remote_code": True
+        },
+        description="Spanish test sets from SemEval-2014 (Agirre et al., 2014) and SemEval-2015 (Agirre et al., 2015)",
+        reference="https://huggingface.co/datasets/PlanTL-GOB-ES/sts-es",
+        type="STS",
+        category="s2s",
+        eval_splits=[_EVAL_SPLIT],
+        eval_langs=["es"],
+        main_score="cosine_spearman",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
-    def load_data(self, **kwargs):
-        if self.data_loaded:
-            return
-        # fetch both subsets of the dataset
-        corpus_raw = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"], "documents"
-        )
-        queries_raw = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"], "queries"
-        )
-
-        self.queries = {
-            self._EVAL_SPLITS[0]: {
-                str(i): q["Question"] for i, q in enumerate(queries_raw["queries"])
-            }
-        }
-
-        corpus_raw = corpus_raw["documents"]
-        corpus_raw = corpus_raw.rename_column("content", "text")
-        self.corpus = {
-            self._EVAL_SPLITS[0]: {str(row["id"]): row for row in corpus_raw}
-        }
-
-        self.relevant_docs = {
-            self._EVAL_SPLITS[0]: {
-                str(i): {str(q["Article"]): 1}
-                for i, q in enumerate(queries_raw["queries"])
-            }
-        }
+    @property
+    def metadata_dict(self) -> dict[str, str]:
+        metadata_dict = super().metadata_dict
+        metadata_dict["min_score"] = 0
+        metadata_dict["max_score"] = 5
+        return metadata_dict
+
+    def dataset_transform(self):
+        data = self.dataset[_EVAL_SPLIT]
+        data = data.add_column("score", [d["label"] for d in data])
+        self.dataset = {_EVAL_SPLIT: data}
 
-        self.data_loaded = True
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/ko/KoMiracl.py` & `mteb-1.5.0/mteb/tasks/Retrieval/ko/KoMiracl.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 
 
 class KoMiracl(AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="Ko-miracl",
         description="Ko-miracl",
         reference=None,
-        hf_hub_name="taeminlee/Ko-miracl",
+        dataset={
+            "path": "taeminlee/Ko-miracl",
+            "revision": "5c7690518e481375551916f24241048cf7b017d0",
+        },
         type="Retrieval",
         category="s2p",
         eval_splits=["dev"],
         eval_langs=["ko"],
         main_score="ndcg_at_10",
-        revision="5c7690518e481375551916f24241048cf7b017d0",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/ko/KoMrtydi.py` & `mteb-1.5.0/mteb/tasks/Retrieval/pl/DBPediaPLRetrieval.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class KoMrtydi(AbsTaskRetrieval):
+class DBPediaPL(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="Ko-mrtydi",
-        description="Ko-mrtydi",
-        reference=None,
-        hf_hub_name="taeminlee/Ko-mrtydi",
+        name="DBPedia-PL",
+        description="DBpedia-Entity is a standard test collection for entity search over the DBpedia knowledge base",
+        reference="https://github.com/iai-group/DBpedia-Entity/",
+        dataset={
+            "path": "clarin-knext/dbpedia-pl",
+            "revision": "76afe41d9af165cc40999fcaa92312b8b012064a",
+        },
         type="Retrieval",
         category="s2p",
-        eval_splits=["dev"],
-        eval_langs=["ko"],
+        eval_splits=["test"],
+        eval_langs=["pl"],
         main_score="ndcg_at_10",
-        revision="71a2e011a42823051a2b4eb303a3366bdbe048d3",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/ko/KoStrategyQA.py` & `mteb-1.5.0/mteb/tasks/Retrieval/en/DBPediaRetrieval.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class KoStrategyQA(AbsTaskRetrieval):
+class DBPedia(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="Ko-StrategyQA",
-        description="Ko-StrategyQA",
-        reference=None,
-        hf_hub_name="taeminlee/Ko-StrategyQA",
+        name="DBPedia",
+        description="DBpedia-Entity is a standard test collection for entity search over the DBpedia knowledge base",
+        reference="https://github.com/iai-group/DBpedia-Entity/",
+        dataset={
+            "path": "mteb/dbpedia",
+            "revision": "c0f706b76e590d620bd6618b3ca8efdd34e2d659",
+        },
         type="Retrieval",
         category="s2p",
-        eval_splits=["dev"],
-        eval_langs=["ko"],
+        eval_splits=["dev", "test"],
+        eval_langs=["en"],
         main_score="ndcg_at_10",
-        revision="d243889a3eb6654029dbd7e7f9319ae31d58f97c",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py`

 * *Files 10% similar despite different names*

```diff
@@ -60,21 +60,23 @@
 
 
 class MIRACLRetrieval(MultilingualTask, AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="MIRACLRetrieval",
         description="MIRACLRetrieval",
         reference=None,
-        hf_hub_name="jinaai/miracl",
+        dataset={
+            "path": "jinaai/miracl",
+            "revision": "d28a029f35c4ff7f616df47b0edf54e6882395e6",
+        },
         type="Retrieval",
         category="s2p",
         eval_splits=[_EVAL_SPLIT],
         eval_langs=_LANGS,
         main_score="ndcg_at_10",
-        revision="d28a029f35c4ff7f616df47b0edf54e6882395e6",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -86,15 +88,15 @@
     )
 
     def load_data(self, **kwargs):
         if self.data_loaded:
             return
 
         self.corpus, self.queries, self.relevant_docs = _load_miracl_data(
-            path=self.metadata_dict["hf_hub_name"],
+            path=self.metadata_dict["dataset"]["path"],
             langs=self.langs,
             split=self.metadata_dict["eval_splits"][0],
             cache_dir=kwargs.get("cache_dir", None),
-            revision=self.metadata_dict["revision"],
+            revision=self.metadata_dict["dataset"]["revision"],
         )
 
         self.data_loaded = True
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,21 +50,23 @@
 
 
 class MintakaRetrieval(MultilingualTask, AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="MintakaRetrieval",
         description="MintakaRetrieval",
         reference=None,
-        hf_hub_name="jinaai/mintakaqa",
+        dataset={
+            "path": "jinaai/mintakaqa",
+            "revision": "efa78cc2f74bbcd21eff2261f9e13aebe40b814e",
+        },
         type="Retrieval",
         category="s2p",
         eval_splits=[_EVAL_SPLIT],
         eval_langs=_LANGS,
         main_score="ndcg_at_10",
-        revision="efa78cc2f74bbcd21eff2261f9e13aebe40b814e",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -76,15 +78,15 @@
     )
 
     def load_data(self, **kwargs):
         if self.data_loaded:
             return
 
         self.corpus, self.queries, self.relevant_docs = _load_mintaka_data(
-            path=self.metadata_dict["hf_hub_name"],
+            path=self.metadata_dict["dataset"]["path"],
             langs=self.metadata.eval_langs,
             split=self.metadata_dict["eval_splits"][0],
             cache_dir=kwargs.get("cache_dir", None),
-            revision=self.metadata_dict["revision"],
+            revision=self.metadata_dict["dataset"]["revision"],
         )
 
         self.data_loaded = True
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,22 +20,28 @@
     "pt",
     "ru",
     "th",
     "zh",
 ]
 
 
-def load_mldr_data(path: str, langs: list, eval_splits: list, cache_dir: str = None):
+def load_mldr_data(
+    path: str,
+    langs: list,
+    eval_splits: list,
+    cache_dir: str = None,
+    revision: str = None,
+):
     corpus = {lang: {split: None for split in eval_splits} for lang in langs}
     queries = {lang: {split: None for split in eval_splits} for lang in langs}
     relevant_docs = {lang: {split: None for split in eval_splits} for lang in langs}
 
     for lang in langs:
         lang_corpus = datasets.load_dataset(
-            path, f"corpus-{lang}", cache_dir=cache_dir
+            path, f"corpus-{lang}", cache_dir=cache_dir, revision=revision
         )["corpus"]
         lang_corpus = {e["docid"]: {"text": e["text"]} for e in lang_corpus}
         lang_data = datasets.load_dataset(path, lang, cache_dir=cache_dir)
         for split in eval_splits:
             corpus[lang][split] = lang_corpus
             queries[lang][split] = {e["query_id"]: e["query"] for e in lang_data[split]}
             relevant_docs[lang][split] = {
@@ -50,32 +56,34 @@
 
 
 class MultiLongDocRetrieval(MultilingualTask, AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="MultiLongDocRetrieval",
         description="MultiLongDocRetrieval",
         reference="https://arxiv.org/abs/2402.03216",
-        hf_hub_name="Shitao/MLDR",
+        dataset={
+            "path": "Shitao/MLDR",
+            "revision": "d79af07e969a6678fcbbe819956840425816468f",
+        },
         type="Retrieval",
         category="s2p",
         eval_splits=["dev", "test"],
         eval_langs=_LANGUAGES,
         main_score="ndcg_at_10",
-        revision="d79af07e969a6678fcbbe819956840425816468f",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation="""@misc{bge-m3,
-      title={BGE M3-Embedding: Multi-Lingual, Multi-Functionality, Multi-Granularity Text Embeddings Through Self-Knowledge Distillation}, 
+      title={BGE M3-Embedding: Multi-Lingual, Multi-Functionality, Multi-Granularity Text Embeddings Through Self-Knowledge Distillation},
       author={Jianlv Chen and Shitao Xiao and Peitian Zhang and Kun Luo and Defu Lian and Zheng Liu},
       year={2024},
       eprint={2402.03216},
       archivePrefix={arXiv},
       primaryClass={cs.CL}
 }
 """,
@@ -84,13 +92,14 @@
     )
 
     def load_data(self, **kwargs):
         if self.data_loaded:
             return
 
         self.corpus, self.queries, self.relevant_docs = load_mldr_data(
-            path=self.metadata_dict["hf_hub_name"],
+            path=self.metadata_dict["dataset"]["path"],
             langs=self.metadata.eval_langs,
             eval_splits=self.metadata_dict["eval_splits"],
             cache_dir=kwargs.get("cache_dir", None),
+            revision=self.metadata_dict["dataset"]["revision"],
         )
         self.data_loaded = True
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,21 +57,23 @@
 
 
 class XMarket(MultilingualTask, AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="XMarket",
         description="XMarket",
         reference=None,
-        hf_hub_name="jinaai/xmarket_ml",
+        dataset={
+            "path": "jinaai/xmarket_ml",
+            "revision": "dfe57acff5b62c23732a7b7d3e3fb84ff501708b",
+        },
         type="Retrieval",
         category="s2p",
         eval_splits=[_EVAL_SPLIT],
         eval_langs=_EVAL_LANGS,
         main_score="ndcg_at_10",
-        revision="dfe57acff5b62c23732a7b7d3e3fb84ff501708b",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -83,15 +85,15 @@
     )
 
     def load_data(self, **kwargs):
         if self.data_loaded:
             return
 
         self.corpus, self.queries, self.relevant_docs = _load_xmarket_data(
-            path=self.metadata_dict["hf_hub_name"],
+            path=self.metadata_dict["dataset"]["path"],
             langs=self.metadata.eval_langs,
             split=self.metadata_dict["eval_splits"][0],
             cache_dir=kwargs.get("cache_dir", None),
-            revision=self.metadata_dict["revision"],
+            revision=self.metadata_dict["dataset"]["revision"],
         )
 
         self.data_loaded = True
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,21 +50,23 @@
 
 
 class XPQARetrieval(MultilingualTask, AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="XPQARetrieval",
         description="XPQARetrieval",
         reference="https://arxiv.org/abs/2305.09249",
-        hf_hub_name="jinaai/xpqa",
+        dataset={
+            "path": "jinaai/xpqa",
+            "revision": "c99d599f0a6ab9b85b065da6f9d94f9cf731679f",
+        },
         type="Retrieval",
         category="s2p",
         eval_splits=[_EVAL_SPLIT],
         eval_langs=_LANGS,
         main_score="ndcg_at_10",
-        revision="c99d599f0a6ab9b85b065da6f9d94f9cf731679f",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -76,15 +78,15 @@
     )
 
     def load_data(self, **kwargs):
         if self.data_loaded:
             return
 
         self.corpus, self.queries, self.relevant_docs = _load_xpqa_data(
-            path=self.metadata_dict["hf_hub_name"],
+            path=self.metadata_dict["dataset"]["path"],
             langs=self.langs,
             split=self.metadata_dict["eval_splits"][0],
             cache_dir=kwargs.get("cache_dir", None),
-            revision=self.metadata_dict["revision"],
+            revision=self.metadata_dict["dataset"]["revision"],
         )
 
         self.data_loaded = True
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/nb/norquad.py` & `mteb-1.5.0/mteb/tasks/Retrieval/nb/norquad.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 
 from mteb.abstasks import AbsTaskRetrieval, TaskMetadata
 
 
 class NorQuadRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="NorQuadRetrieval",
-        hf_hub_name="ScandEval/norquad-mini",
+        dataset={
+            "path": "ScandEval/norquad-mini",
+            "revision": "a47881440ce4b18ef61a99be66dc4badbf5aac6e",
+        },
         description="Human-created question for Norwegian wikipedia passages.",
         reference="https://aclanthology.org/2023.nodalida-1.17/",
         type="Retrieval",
         category="p2p",
         eval_splits=["test"],
         eval_langs=["nb"],
         main_score="ndcg_at_10",
-        revision="a47881440ce4b18ef61a99be66dc4badbf5aac6e",
         date=("2022-01-01", "2023-12-31"),
         form=["written"],
         task_subtypes=["Question answering"],
         domains=["Encyclopaedic", "Non-fiction"],
         license="CC-BY-SA-4.0",
         socioeconomic_status="high",
         annotations_creators="derived",
@@ -42,29 +44,14 @@
     pages = "159--168",
     abstract = "In this paper we present NorQuAD: the first Norwegian question answering dataset for machine reading comprehension. The dataset consists of 4,752 manually created question-answer pairs. We here detail the data collection procedure and present statistics of the dataset. We also benchmark several multilingual and Norwegian monolingual language models on the dataset and compare them against human performance. The dataset will be made freely available.",
 }""",
         n_samples={"test": 2602},
         avg_character_length={"test": 502.19},
     )
 
-    def load_data(self, **kwargs: dict):  # noqa: ARG002
-        """
-        Load dataset from HuggingFace hub
-        """
-        if self.data_loaded:
-            return
-
-        self.dataset: datasets.DatasetDict = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            revision=self.metadata_dict.get("revision"),
-        )  # type: ignore
-
-        self.dataset_transform()
-        self.data_loaded = True
-
     def dataset_transform(self) -> None:
         """
         and transform to a retrieval datset, which have the following attributes
 
         self.corpus = Dict[doc_id, Dict[str, str]] #id => dict with document datas like title and text
         self.queries = Dict[query_id, str] #id => query
         self.relevant_docs = Dict[query_id, Dict[[doc_id, score]]
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/nb/snl_retrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/nb/snl_retrieval.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 
 from mteb.abstasks import AbsTaskRetrieval, TaskMetadata
 
 
 class SNLRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="SNLRetrieval",
-        hf_hub_name="navjordj/SNL_summarization",
+        dataset={
+            "path": "navjordj/SNL_summarization",
+            "revision": "3d3d27aa7af8941408cefc3991ada5d12a4273d1",
+        },
         description="Webscrabed articles and ingresses from the Norwegian lexicon 'Det Store Norske Leksikon'.",
         reference="https://huggingface.co/datasets/navjordj/SNL_summarization",
         type="Retrieval",
         category="p2p",
         eval_splits=["test"],
         eval_langs=["nb"],
         main_score="ndcg_at_10",
-        revision="3d3d27aa7af8941408cefc3991ada5d12a4273d1",
         date=("2020-01-01", "2024-12-31"),  # best guess
         form=["written"],
         domains=["Encyclopaedic", "Non-fiction"],
         license=None,
         socioeconomic_status="high",
         annotations_creators="derived",
         dialect=[],
@@ -30,29 +32,14 @@
     school={Norwegian University of Life Sciences, {\AA}s}
 }""",
         n_samples={"test": 2048},
         avg_character_length={"test": 1101.30},
         task_subtypes=["Article retrieval"],
     )
 
-    def load_data(self, **kwargs: dict):  # noqa: ARG002
-        """
-        Load dataset from HuggingFace hub
-        """
-        if self.data_loaded:
-            return
-
-        self.dataset: datasets.DatasetDict = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            revision=self.metadata_dict.get("revision"),
-        )  # type: ignore
-
-        self.dataset_transform()
-        self.data_loaded = True
-
     def dataset_transform(self) -> None:
         """
         and transform to a retrieval datset, which have the following attributes
 
         self.corpus = Dict[doc_id, Dict[str, str]] #id => dict with document datas like title and text
         self.queries = Dict[query_id, str] #id => query
         self.relevant_docs = Dict[query_id, Dict[[doc_id, score]]
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/pl/ArguAnaPLRetrieval.py` & `mteb-1.5.0/mteb/tasks/Clustering/de/BlurbsClusteringS2S.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
+from ....abstasks.AbsTaskClustering import AbsTaskClustering
 
 
-class ArguAnaPL(AbsTaskRetrieval):
+class BlurbsClusteringS2S(AbsTaskClustering):
     metadata = TaskMetadata(
-        name="ArguAna-PL",
-        description="ArguAna-PL",
-        reference="https://huggingface.co/datasets/clarin-knext/arguana-pl",
-        hf_hub_name="clarin-knext/arguana-pl",
-        type="Retrieval",
-        category="s2p",
+        name="BlurbsClusteringS2S",
+        description="Clustering of book titles. Clustering of 28 sets, either on the main or secondary genre.",
+        reference="https://www.inf.uni-hamburg.de/en/inst/ab/lt/resources/data/germeval-2019-hmc.html",
+        dataset={
+            "path": "slvnwhrl/blurbs-clustering-s2s",
+            "revision": "5bfd9ee0ae3d2ef0d9a0e0bd0c3b2d0",
+        },
+        type="Clustering",
+        category="s2s",
         eval_splits=["test"],
-        eval_langs=["pl"],
-        main_score="ndcg_at_10",
-        revision="63fc86750af76253e8c760fc9e534bbf24d260a2",
+        eval_langs=["de"],
+        main_score="v_measure",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples=None,
-        avg_character_length=None,
+        n_samples={"test": 174637},
+        avg_character_length={"test": 23.02},
     )
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/pl/DBPediaPLRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackStatsRetrieval.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class DBPediaPL(AbsTaskRetrieval):
+class CQADupstackStatsRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="DBPedia-PL",
-        description="DBpedia-Entity is a standard test collection for entity search over the DBpedia knowledge base",
-        reference="https://github.com/iai-group/DBpedia-Entity/",
-        hf_hub_name="clarin-knext/dbpedia-pl",
+        name="CQADupstackStatsRetrieval",
+        description="CQADupStack: A Benchmark Data Set for Community Question-Answering Research",
+        reference="http://nlp.cis.unimelb.edu.au/resources/cqadupstack/",
+        dataset={
+            "path": "mteb/cqadupstack-stats",
+            "revision": "65ac3a16b8e91f9cee4c9828cc7c335575432a2a",
+        },
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
-        eval_langs=["pl"],
+        eval_langs=["en"],
         main_score="ndcg_at_10",
-        revision="76afe41d9af165cc40999fcaa92312b8b012064a",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/pl/FiQAPLRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/pl/FiQAPLRetrieval.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 
 
 class FiQAPLRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="FiQA-PL",
         description="Financial Opinion Mining and Question Answering",
         reference="https://sites.google.com/view/fiqa/",
-        hf_hub_name="clarin-knext/fiqa-pl",
+        dataset={
+            "path": "clarin-knext/fiqa-pl",
+            "revision": "2e535829717f8bf9dc829b7f911cc5bbd4e6608e",
+        },
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
         eval_langs=["pl"],
         main_score="ndcg_at_10",
-        revision="2e535829717f8bf9dc829b7f911cc5bbd4e6608e",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/pl/HotpotQAPLRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/en/NQRetrieval.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class HotpotQAPL(AbsTaskRetrieval):
+class NQ(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="HotpotQA-PL",
-        description="HotpotQA is a question answering dataset featuring natural, multi-hop questions, with strong supervision for supporting facts to enable more explainable question answering systems.",
-        reference="https://hotpotqa.github.io/",
-        hf_hub_name="clarin-knext/hotpotqa-pl",
+        name="NQ",
+        dataset={
+            "path": "mteb/nq",
+            "revision": "b774495ed302d8c44a3a7ea25c90dbce03968f31",
+        },
+        description="NFCorpus: A Full-Text Learning to Rank Dataset for Medical Information Retrieval",
+        reference="https://ai.google.com/research/NaturalQuestions/",
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
-        eval_langs=["pl"],
+        eval_langs=["en"],
         main_score="ndcg_at_10",
-        revision="a0bd479ac97b4ccb5bd6ce320c415d0bb4beb907",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/pl/MSMARCOPLRetrieval.py` & `mteb-1.5.0/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,45 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
+from ....abstasks import AbsTaskClassification, MultilingualTask
 
+_LANGUAGES = ["en", "de", "en-ext", "ja"]
 
-class MSMARCOPL(AbsTaskRetrieval):
+
+class AmazonCounterfactualClassification(MultilingualTask, AbsTaskClassification):
     metadata = TaskMetadata(
-        name="MSMARCO-PL",
-        description="MS MARCO is a collection of datasets focused on deep learning in search",
-        reference="https://microsoft.github.io/msmarco/",
-        hf_hub_name="clarin-knext/msmarco-pl",
-        type="Retrieval",
-        category="s2p",
-        eval_splits=["test"],
-        eval_langs=["pl"],
-        main_score="ndcg_at_10",
-        revision="8634c07806d5cce3a6138e260e59b81760a0a640",
+        name="AmazonCounterfactualClassification",
+        dataset={
+            "path": "mteb/amazon_counterfactual",
+            "revision": "e8379541af4e31359cca9fbcf4b00f2671dba205",
+        },
+        description=(
+            "A collection of Amazon customer reviews annotated for counterfactual detection pair classification."
+        ),
+        reference="https://arxiv.org/abs/2104.06893",
+        category="s2s",
+        type="Classification",
+        eval_splits=["validation", "test"],
+        eval_langs=_LANGUAGES,
+        main_score="accuracy",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples=None,
-        avg_character_length=None,
+        n_samples={"validation": 335, "test": 670},
+        avg_character_length={"validation": 109.2, "test": 106.1},
     )
+
+    @property
+    def metadata_dict(self) -> dict[str, str]:
+        metadata_dict = super().metadata_dict
+        metadata_dict["n_experiments"] = 10
+        metadata_dict["samples_per_label"] = 32
+        return metadata_dict
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/pl/NFCorpusPLRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/ko/KoStrategyQA.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class NFCorpusPL(AbsTaskRetrieval):
+class KoStrategyQA(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="NFCorpus-PL",
-        description="NFCorpus: A Full-Text Learning to Rank Dataset for Medical Information Retrieval",
-        reference="https://www.cl.uni-heidelberg.de/statnlpgroup/nfcorpus/",
-        hf_hub_name="clarin-knext/nfcorpus-pl",
+        name="Ko-StrategyQA",
+        description="Ko-StrategyQA",
+        reference=None,
+        dataset={
+            "path": "taeminlee/Ko-StrategyQA",
+            "revision": "d243889a3eb6654029dbd7e7f9319ae31d58f97c",
+        },
         type="Retrieval",
         category="s2p",
-        eval_splits=["test"],
-        eval_langs=["pl"],
+        eval_splits=["dev"],
+        eval_langs=["ko"],
         main_score="ndcg_at_10",
-        revision="9a6f9567fda928260afed2de480d79c98bf0bec0",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/pl/NQPLRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/en/CQADupstackProgrammersRetrieval.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class NQPL(AbsTaskRetrieval):
+class CQADupstackProgrammersRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="NQ-PL",
-        description="Natural Questions: A Benchmark for Question Answering Research",
-        reference="https://ai.google.com/research/NaturalQuestions/",
-        hf_hub_name="clarin-knext/nq-pl",
+        name="CQADupstackProgrammersRetrieval",
+        description="CQADupStack: A Benchmark Data Set for Community Question-Answering Research",
+        reference="http://nlp.cis.unimelb.edu.au/resources/cqadupstack/",
+        dataset={
+            "path": "mteb/cqadupstack-programmers",
+            "revision": "6184bc1440d2dbc7612be22b50686b8826d22b32",
+        },
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
-        eval_langs=["pl"],
+        eval_langs=["en"],
         main_score="ndcg_at_10",
-        revision="f171245712cf85dd4700b06bef18001578d0ca8d",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/pl/QuoraPLRetrieval.py` & `mteb-1.5.0/mteb/tasks/PairClassification/zh/CMTEBPairClassification.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,56 @@
 from __future__ import annotations
 
+from mteb.abstasks.AbsTaskPairClassification import AbsTaskPairClassification
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
+
+class Ocnli(AbsTaskPairClassification):
+    metadata = TaskMetadata(
+        name="Ocnli",
+        description="Original Chinese Natural Language Inference dataset",
+        reference="https://arxiv.org/abs/2010.05444",
+        dataset={
+            "path": "C-MTEB/OCNLI",
+            "revision": "7bd1ee0ae3a820d8a4b6f8a624063f8504a3564d",
+        },
+        type="PairClassification",
+        category="s2s",
+        eval_splits=["validation", "test"],
+        eval_langs=["zh"],
+        main_score="accuracy",
+        date=None,
+        form=None,
+        domains=None,
+        task_subtypes=None,
+        license=None,
+        socioeconomic_status=None,
+        annotations_creators=None,
+        dialect=None,
+        text_creation=None,
+        bibtex_citation=None,
+        n_samples=None,
+        avg_character_length=None,
+    )
 
 
-class QuoraPLRetrieval(AbsTaskRetrieval):
+class Cmnli(AbsTaskPairClassification):
     metadata = TaskMetadata(
-        name="Quora-PL",
-        description="QuoraRetrieval is based on questions that are marked as duplicates on the Quora platform. Given a question, find other (duplicate) questions.",
-        reference="https://quoradata.quora.com/First-Quora-Dataset-Release-Question-Pairs",
-        hf_hub_name="clarin-knext/quora-pl",
-        type="Retrieval",
+        name="Cmnli",
+        description="Chinese Multi-Genre NLI",
+        reference="https://huggingface.co/datasets/clue/viewer/cmnli",
+        dataset={
+            "path": "C-MTEB/CMNLI",
+            "revision": "41bc36f332156f7adc9e38f53777c959b2ae9766",
+        },
+        type="PairClassification",
         category="s2s",
-        eval_splits=["validation", "test"],  # validation for new DataLoader
-        eval_langs=["pl"],
-        main_score="ndcg_at_10",
-        revision="0be27e93455051e531182b85e85e425aba12e9d4",
+        eval_splits=["validation", "test"],
+        eval_langs=["zh"],
+        main_score="accuracy",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/pl/SCIDOCSPLRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/en/SciFactRetrieval.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class SCIDOCSPL(AbsTaskRetrieval):
+class SciFact(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="SCIDOCS-PL",
-        description="SciDocs, a new evaluation benchmark consisting of seven document-level tasks ranging from citation prediction, to document classification and recommendation.",
-        reference="https://allenai.org/data/scidocs",
-        hf_hub_name="clarin-knext/scidocs-pl",
+        name="SciFact",
+        dataset={
+            "path": "mteb/scifact",
+            "revision": "0228b52cf27578f30900b9e5271d331663a030d7",
+        },
+        description="SciFact verifies scientific claims using evidence from the research literature containing scientific paper abstracts.",
+        reference="https://github.com/allenai/scifact",
         type="Retrieval",
         category="s2p",
-        eval_splits=["test"],
-        eval_langs=["pl"],
+        eval_splits=["train", "test"],
+        eval_langs=["en"],
         main_score="ndcg_at_10",
-        revision="45452b03f05560207ef19149545f168e596c9337",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/pl/SciFactPLRetrieval.py` & `mteb-1.5.0/mteb/tasks/STS/en/STS16STS.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
+from ....abstasks.AbsTaskSTS import AbsTaskSTS
 
 
-class SciFactPL(AbsTaskRetrieval):
+class STS16STS(AbsTaskSTS):
     metadata = TaskMetadata(
-        name="SciFact-PL",
-        description="SciFact verifies scientific claims using evidence from the research literature containing scientific paper abstracts.",
-        reference="https://github.com/allenai/scifact",
-        hf_hub_name="clarin-knext/scifact-pl",
-        type="Retrieval",
-        category="s2p",
+        name="STS16",
+        dataset={
+            "path": "mteb/sts16-sts",
+            "revision": "4d8694f8f0e0100860b497b999b3dbed754a0513",
+        },
+        description="SemEval STS 2016 dataset",
+        reference="https://www.aclweb.org/anthology/S16-1001",
+        type="STS",
+        category="s2s",
         eval_splits=["test"],
-        eval_langs=["pl"],
-        main_score="ndcg_at_10",
-        revision="47932a35f045ef8ed01ba82bf9ff67f6e109207e",
+        eval_langs=["en"],
+        main_score="cosine_spearman",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
+
+    @property
+    def metadata_dict(self) -> dict[str, str]:
+        metadata_dict = super().metadata_dict
+        metadata_dict["min_score"] = 0
+        metadata_dict["max_score"] = 5
+        return metadata_dict
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/sv/swedn_retrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/sv/swedn_retrieval.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,23 +2,26 @@
 
 from mteb.abstasks import AbsTaskRetrieval, TaskMetadata
 
 
 class SwednRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="SwednRetrieval",
-        hf_hub_name="sbx/superlim-2",
+        dataset={
+            "path": "sbx/superlim-2",
+            "revision": "ef1661775d746e0844b299164773db733bdc0bf6",
+            "name": "swedn",
+        },
         description="The SWE-DN corpus is based on 1,963,576 news articles from the Swedish newspaper Dagens Nyheter (DN) during the years 2000--2020. The articles are filtered to resemble the CNN/DailyMail dataset both regarding textual structure",
         reference="https://spraakbanken.gu.se/en/resources/swedn",
         type="Retrieval",
         category="p2p",
         eval_splits=["test"],
         eval_langs=["sv"],
         main_score="ndcg_at_10",
-        revision="ef1661775d746e0844b299164773db733bdc0bf6",
         date=("2000-01-01", "2020-12-31"),
         form=["written"],
         domains=["News", "Non-fiction"],
         license="CC BY-SA 4.0",
         socioeconomic_status="mixed",
         annotations_creators="derived",
         dialect=[],
@@ -30,30 +33,14 @@
     booktitle={Proceedings of CLARIN Annual Conference},
     year={2021}
 }""",
         n_samples={"test": 2048},
         avg_character_length={"test": 1946.35},
     )
 
-    def load_data(self, **kwargs: dict):  # noqa: ARG002
-        """
-        Load dataset from HuggingFace hub
-        """
-        if self.data_loaded:
-            return
-
-        self.dataset: datasets.DatasetDict = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            "swedn",  # chose the relevant subset
-            revision=self.metadata_dict.get("revision"),
-        )  # type: ignore
-
-        self.dataset_transform()
-        self.data_loaded = True
-
     def dataset_transform(self) -> None:
         """
         and transform to a retrieval datset, which have the following attributes
 
         self.corpus = Dict[doc_id, Dict[str, str]] #id => dict with document datas like title and text
         self.queries = Dict[query_id, str] #id => query
         self.relevant_docs = Dict[query_id, Dict[[doc_id, score]]
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/sv/swefaq_retrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/sv/swefaq_retrieval.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,53 +2,40 @@
 
 from mteb.abstasks import AbsTaskRetrieval, TaskMetadata
 
 
 class SweFaqRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="SweFaqRetrieval",
-        hf_hub_name="AI-Sweden/SuperLim",
+        dataset={
+            "path": "AI-Sweden/SuperLim",
+            "revision": "7ebf0b4caa7b2ae39698a889de782c09e6f5ee56",
+            "name": "swefaq",
+        },
         description="A Swedish QA dataset derived from FAQ",
         reference="https://spraakbanken.gu.se/en/resources/superlim",
         type="Retrieval",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["sv"],
         main_score="ndcg_at_10",
-        revision="7ebf0b4caa7b2ae39698a889de782c09e6f5ee56",
         date=("2000-01-01", "2024-12-31"),  # best guess
         form=["written"],
         task_subtypes=["Question answering"],
         domains=["Government", "Non-fiction"],
         license="CC-BY-SA-4.0",
         socioeconomic_status="mixed",
         annotations_creators="derived",
         dialect=[],
         text_creation="found",
         bibtex_citation=None,
         n_samples={"test": 1024},
         avg_character_length={"test": 195.44},
     )
 
-    def load_data(self, **kwargs: dict):  # noqa: ARG002
-        """
-        Load dataset from HuggingFace hub
-        """
-        if self.data_loaded:
-            return
-
-        self.dataset: datasets.DatasetDict = datasets.load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            "swefaq",  # chose the relevant subset
-            revision=self.metadata_dict.get("revision"),
-        )  # type: ignore
-
-        self.dataset_transform()
-        self.data_loaded = True
-
     def dataset_transform(self) -> None:
         """
         and transform to a retrieval datset, which have the following attributes
 
         self.corpus = Dict[doc_id, Dict[str, str]] #id => dict with document datas like title and text
         self.queries = Dict[query_id, str] #id => query
         self.relevant_docs = Dict[query_id, Dict[[doc_id, score]]
```

### Comparing `mteb-1.4.1/mteb/tasks/Retrieval/zh/CMTEBRetrieval.py` & `mteb-1.5.0/mteb/tasks/Retrieval/zh/CMTEBRetrieval.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 from datasets import DatasetDict, load_dataset
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-def load_retrieval_data(hf_hub_name, eval_splits):
+def load_retrieval_data(dataset_path, revision, eval_splits):
     eval_split = eval_splits[0]
-    dataset = load_dataset(hf_hub_name)
-    qrels = load_dataset(hf_hub_name + "-qrels")[eval_split]
+    dataset = load_dataset(dataset_path, revision=revision)
+    qrels = load_dataset(dataset_path + "-qrels", revision=revision)[eval_split]
 
     corpus = {e["id"]: {"text": e["text"]} for e in dataset["corpus"]}
     queries = {e["id"]: e["text"] for e in dataset["queries"]}
     relevant_docs = defaultdict(dict)
     for e in qrels:
         relevant_docs[e["qid"]][e["pid"]] = e["score"]
 
@@ -27,21 +27,23 @@
 
 
 class T2Retrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="T2Retrieval",
         description="T2Ranking: A large-scale Chinese Benchmark for Passage Ranking",
         reference="https://arxiv.org/abs/2304.03679",
-        hf_hub_name="C-MTEB/T2Retrieval",
+        dataset={
+            "path": "C-MTEB/T2Retrieval",
+            "revision": "8731a845f1bf500a4f111cf1070785c793d10e64",
+        },
         type="Retrieval",
         category="s2p",
         eval_splits=["dev"],
         eval_langs=["zh"],
         main_score="ndcg_at_10",
-        revision="8731a845f1bf500a4f111cf1070785c793d10e64",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -53,31 +55,35 @@
     )
 
     def load_data(self, **kwargs):
         if self.data_loaded:
             return
 
         self.corpus, self.queries, self.relevant_docs = load_retrieval_data(
-            self.metadata_dict["hf_hub_name"], self.metadata_dict["eval_splits"]
+            self.metadata_dict["dataset"]["path"],
+            self.metadata_dict["dataset"]["revision"],
+            self.metadata_dict["eval_splits"],
         )
         self.data_loaded = True
 
 
 class MMarcoRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="MMarcoRetrieval",
         description="MMarcoRetrieval",
         reference="https://arxiv.org/abs/2309.07597",
-        hf_hub_name="C-MTEB/MMarcoRetrieval",
+        dataset={
+            "path": "C-MTEB/MMarcoRetrieval",
+            "revision": "539bbde593d947e2a124ba72651aafc09eb33fc2",
+        },
         type="Retrieval",
         category="s2p",
         eval_splits=["dev"],
         eval_langs=["zh"],
         main_score="ndcg_at_10",
-        revision="539bbde593d947e2a124ba72651aafc09eb33fc2",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -89,31 +95,35 @@
     )
 
     def load_data(self, **kwargs):
         if self.data_loaded:
             return
 
         self.corpus, self.queries, self.relevant_docs = load_retrieval_data(
-            self.metadata_dict["hf_hub_name"], self.metadata_dict["eval_splits"]
+            self.metadata_dict["dataset"]["path"],
+            self.metadata_dict["dataset"]["revision"],
+            self.metadata_dict["eval_splits"],
         )
         self.data_loaded = True
 
 
 class DuRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="DuRetrieval",
         description="A Large-scale Chinese Benchmark for Passage Retrieval from Web Search Engine",
         reference="https://aclanthology.org/2022.emnlp-main.357.pdf",
-        hf_hub_name="C-MTEB/DuRetrieval",
+        dataset={
+            "path": "C-MTEB/DuRetrieval",
+            "revision": "a1a333e290fe30b10f3f56498e3a0d911a693ced",
+        },
         type="Retrieval",
         category="s2p",
         eval_splits=["dev"],
         eval_langs=["zh"],
         main_score="ndcg_at_10",
-        revision="a1a333e290fe30b10f3f56498e3a0d911a693ced",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -125,31 +135,35 @@
     )
 
     def load_data(self, **kwargs):
         if self.data_loaded:
             return
 
         self.corpus, self.queries, self.relevant_docs = load_retrieval_data(
-            self.metadata_dict["hf_hub_name"], self.metadata_dict["eval_splits"]
+            self.metadata_dict["dataset"]["path"],
+            self.metadata_dict["dataset"]["revision"],
+            self.metadata_dict["eval_splits"],
         )
         self.data_loaded = True
 
 
 class CovidRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="CovidRetrieval",
         description="COVID-19 news articles",
         reference="https://arxiv.org/abs/2203.03367",
-        hf_hub_name="C-MTEB/CovidRetrieval",
+        dataset={
+            "path": "C-MTEB/CovidRetrieval",
+            "revision": "687de13dc7294d6fd9be10c6945f9e8fec8166b9",
+        },
         type="Retrieval",
         category="s2p",
         eval_splits=["test"],
         eval_langs=["zh"],
         main_score="ndcg_at_10",
-        revision="687de13dc7294d6fd9be10c6945f9e8fec8166b9",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -161,31 +175,35 @@
     )
 
     def load_data(self, **kwargs):
         if self.data_loaded:
             return
 
         self.corpus, self.queries, self.relevant_docs = load_retrieval_data(
-            self.metadata_dict["hf_hub_name"], self.metadata_dict["eval_splits"]
+            self.metadata_dict["dataset"]["path"],
+            self.metadata_dict["dataset"]["revision"],
+            self.metadata_dict["eval_splits"],
         )
         self.data_loaded = True
 
 
 class CmedqaRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="CmedqaRetrieval",
         description="Online medical consultation text",
         reference="https://aclanthology.org/2022.emnlp-main.357.pdf",
-        hf_hub_name="C-MTEB/CmedqaRetrieval",
+        dataset={
+            "path": "C-MTEB/CmedqaRetrieval",
+            "revision": "cd540c506dae1cf9e9a59c3e06f42030d54e7301",
+        },
         type="Retrieval",
         category="s2p",
         eval_splits=["dev"],
         eval_langs=["zh"],
         main_score="ndcg_at_10",
-        revision="cd540c506dae1cf9e9a59c3e06f42030d54e7301",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -197,31 +215,35 @@
     )
 
     def load_data(self, **kwargs):
         if self.data_loaded:
             return
 
         self.corpus, self.queries, self.relevant_docs = load_retrieval_data(
-            self.metadata_dict["hf_hub_name"], self.metadata_dict["eval_splits"]
+            self.metadata_dict["dataset"]["path"],
+            self.metadata_dict["dataset"]["revision"],
+            self.metadata_dict["eval_splits"],
         )
         self.data_loaded = True
 
 
 class EcomRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="EcomRetrieval",
         description="EcomRetrieval",
         reference="https://arxiv.org/abs/2203.03367",
-        hf_hub_name="C-MTEB/EcomRetrieval",
+        dataset={
+            "path": "C-MTEB/EcomRetrieval",
+            "revision": "687de13dc7294d6fd9be10c6945f9e8fec8166b9",
+        },
         type="Retrieval",
         category="s2p",
         eval_splits=["dev"],
         eval_langs=["zh"],
         main_score="ndcg_at_10",
-        revision="687de13dc7294d6fd9be10c6945f9e8fec8166b9",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -233,31 +255,35 @@
     )
 
     def load_data(self, **kwargs):
         if self.data_loaded:
             return
 
         self.corpus, self.queries, self.relevant_docs = load_retrieval_data(
-            self.metadata_dict["hf_hub_name"], self.metadata_dict["eval_splits"]
+            self.metadata_dict["dataset"]["path"],
+            self.metadata_dict["dataset"]["revision"],
+            self.metadata_dict["eval_splits"],
         )
         self.data_loaded = True
 
 
 class MedicalRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="MedicalRetrieval",
         description="MedicalRetrieval",
         reference="https://arxiv.org/abs/2203.03367",
-        hf_hub_name="C-MTEB/MedicalRetrieval",
+        dataset={
+            "path": "C-MTEB/MedicalRetrieval",
+            "revision": "2039188fb5800a9803ba5048df7b76e6fb151fc6",
+        },
         type="Retrieval",
         category="s2p",
         eval_splits=["dev"],
         eval_langs=["zh"],
         main_score="ndcg_at_10",
-        revision="2039188fb5800a9803ba5048df7b76e6fb151fc6",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -269,31 +295,35 @@
     )
 
     def load_data(self, **kwargs):
         if self.data_loaded:
             return
 
         self.corpus, self.queries, self.relevant_docs = load_retrieval_data(
-            self.metadata_dict["hf_hub_name"], self.metadata_dict["eval_splits"]
+            self.metadata_dict["dataset"]["path"],
+            self.metadata_dict["dataset"]["revision"],
+            self.metadata_dict["eval_splits"],
         )
         self.data_loaded = True
 
 
 class VideoRetrieval(AbsTaskRetrieval):
     metadata = TaskMetadata(
         name="VideoRetrieval",
         description="VideoRetrieval",
         reference="https://arxiv.org/abs/2203.03367",
-        hf_hub_name="C-MTEB/VideoRetrieval",
+        dataset={
+            "path": "C-MTEB/VideoRetrieval",
+            "revision": "58c2597a5943a2ba48f4668c3b90d796283c5639",
+        },
         type="Retrieval",
         category="s2p",
         eval_splits=["dev"],
         eval_langs=["zh"],
         main_score="ndcg_at_10",
-        revision="58c2597a5943a2ba48f4668c3b90d796283c5639",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -305,10 +335,12 @@
     )
 
     def load_data(self, **kwargs):
         if self.data_loaded:
             return
 
         self.corpus, self.queries, self.relevant_docs = load_retrieval_data(
-            self.metadata_dict["hf_hub_name"], self.metadata_dict["eval_splits"]
+            self.metadata_dict["dataset"]["path"],
+            self.metadata_dict["dataset"]["revision"],
+            self.metadata_dict["eval_splits"],
         )
         self.data_loaded = True
```

### Comparing `mteb-1.4.1/mteb/tasks/STS/__init__.py` & `mteb-1.5.0/mteb/tasks/STS/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/mteb/tasks/STS/de/GermanSTSBenchmarkSTS.py` & `mteb-1.5.0/mteb/tasks/STS/en/STS15STS.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskSTS import AbsTaskSTS
 
 
-class GermanSTSBenchmarkSTS(AbsTaskSTS):
+class STS15STS(AbsTaskSTS):
     metadata = TaskMetadata(
-        name="GermanSTSBenchmark",
-        hf_hub_name="jinaai/german-STSbenchmark",
-        description="Semantic Textual Similarity Benchmark (STSbenchmark) dataset translated into German. "
-        "Translations were originally done by T-Systems on site services GmbH.",
-        reference="https://github.com/t-systems-on-site-services-gmbh/german-STSbenchmark",
+        name="STS15",
+        dataset={
+            "path": "mteb/sts15-sts",
+            "revision": "ae752c7c21bf194d8b67fd573edf7ae58183cbe3",
+        },
+        description="SemEval STS 2015 dataset",
+        reference="https://www.aclweb.org/anthology/S15-2010",
         type="STS",
         category="s2s",
-        eval_splits=["validation", "test"],
-        eval_langs=["de"],
+        eval_splits=["test"],
+        eval_langs=["en"],
         main_score="cosine_spearman",
-        revision="e36907544d44c3a247898ed81540310442329e20",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -30,11 +31,11 @@
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
+        metadata_dict = super().metadata_dict
         metadata_dict["min_score"] = 0
         metadata_dict["max_score"] = 5
         return metadata_dict
```

### Comparing `mteb-1.4.1/mteb/tasks/STS/en/BiossesSTS.py` & `mteb-1.5.0/mteb/tasks/STS/en/BiossesSTS.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 
 from ....abstasks.AbsTaskSTS import AbsTaskSTS
 
 
 class BiossesSTS(AbsTaskSTS):
     metadata = TaskMetadata(
         name="BIOSSES",
-        hf_hub_name="mteb/biosses-sts",
+        dataset={
+            "path": "mteb/biosses-sts",
+            "revision": "d3fb88f8f02e40887cd149695127462bbcf29b4a",
+        },
         description="Biomedical Semantic Similarity Estimation.",
         reference="https://tabilab.cmpe.boun.edu.tr/BIOSSES/DataSet.html",
         type="STS",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="cosine_spearman",
-        revision="d3fb88f8f02e40887cd149695127462bbcf29b4a",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -29,11 +31,11 @@
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
+        metadata_dict = super().metadata_dict
         metadata_dict["min_score"] = 0
         metadata_dict["max_score"] = 5
         return metadata_dict
```

### Comparing `mteb-1.4.1/mteb/tasks/STS/en/STS12STS.py` & `mteb-1.5.0/mteb/tasks/STS/en/STS14STS.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskSTS import AbsTaskSTS
 
 
-class STS12STS(AbsTaskSTS):
+class STS14STS(AbsTaskSTS):
     metadata = TaskMetadata(
-        name="STS12",
-        hf_hub_name="mteb/sts12-sts",
-        description="SemEval STS 2012 dataset.",
-        reference="https://www.aclweb.org/anthology/S12-1051.pdf",
+        name="STS14",
+        dataset={
+            "path": "mteb/sts14-sts",
+            "revision": "6031580fec1f6af667f0bd2da0a551cf4f0b2375",
+        },
+        description="SemEval STS 2014 dataset. Currently only the English dataset",
+        reference="https://www.aclweb.org/anthology/S14-1002",
         type="STS",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="cosine_spearman",
-        revision="a0d554a64d88156834ff5ae9920b964011b16384",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -29,11 +31,11 @@
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
+        metadata_dict = super().metadata_dict
         metadata_dict["min_score"] = 0
         metadata_dict["max_score"] = 5
         return metadata_dict
```

### Comparing `mteb-1.4.1/mteb/tasks/STS/en/STS13STS.py` & `mteb-1.5.0/mteb/tasks/STS/en/STS13STS.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 
 from ....abstasks.AbsTaskSTS import AbsTaskSTS
 
 
 class STS13STS(AbsTaskSTS):
     metadata = TaskMetadata(
         name="STS13",
-        hf_hub_name="mteb/sts13-sts",
+        dataset={
+            "path": "mteb/sts13-sts",
+            "revision": "7e90230a92c190f1bf69ae9002b8cea547a64cca",
+        },
         description="SemEval STS 2013 dataset.",
         reference="https://www.aclweb.org/anthology/S13-1004/",
         type="STS",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="cosine_spearman",
-        revision="7e90230a92c190f1bf69ae9002b8cea547a64cca",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -29,11 +31,11 @@
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
+        metadata_dict = super().metadata_dict
         metadata_dict["min_score"] = 0
         metadata_dict["max_score"] = 5
         return metadata_dict
```

### Comparing `mteb-1.4.1/mteb/tasks/STS/en/STS14STS.py` & `mteb-1.5.0/mteb/tasks/STS/en/STS12STS.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskSTS import AbsTaskSTS
 
 
-class STS14STS(AbsTaskSTS):
+class STS12STS(AbsTaskSTS):
     metadata = TaskMetadata(
-        name="STS14",
-        hf_hub_name="mteb/sts14-sts",
-        description="SemEval STS 2014 dataset. Currently only the English dataset",
-        reference="https://www.aclweb.org/anthology/S14-1002",
+        name="STS12",
+        dataset={
+            "path": "mteb/sts12-sts",
+            "revision": "a0d554a64d88156834ff5ae9920b964011b16384",
+        },
+        description="SemEval STS 2012 dataset.",
+        reference="https://www.aclweb.org/anthology/S12-1051.pdf",
         type="STS",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="cosine_spearman",
-        revision="6031580fec1f6af667f0bd2da0a551cf4f0b2375",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -29,11 +31,11 @@
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
+        metadata_dict = super().metadata_dict
         metadata_dict["min_score"] = 0
         metadata_dict["max_score"] = 5
         return metadata_dict
```

### Comparing `mteb-1.4.1/mteb/tasks/STS/en/STS15STS.py` & `mteb-1.5.0/mteb/tasks/STS/en/STSBenchmarkSTS.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
 from ....abstasks.AbsTaskSTS import AbsTaskSTS
 
 
-class STS15STS(AbsTaskSTS):
+class STSBenchmarkSTS(AbsTaskSTS):
     metadata = TaskMetadata(
-        name="STS15",
-        hf_hub_name="mteb/sts15-sts",
-        description="SemEval STS 2015 dataset",
-        reference="https://www.aclweb.org/anthology/S15-2010",
+        name="STSBenchmark",
+        dataset={
+            "path": "mteb/stsbenchmark-sts",
+            "revision": "b0fddb56ed78048fa8b90373c8a3cfc37b684831",
+        },
+        description="Semantic Textual Similarity Benchmark (STSbenchmark) dataset.",
+        reference="https://github.com/PhilipMay/stsb-multi-mt/",
         type="STS",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["en"],
         main_score="cosine_spearman",
-        revision="ae752c7c21bf194d8b67fd573edf7ae58183cbe3",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -29,11 +31,11 @@
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
+        metadata_dict = super().metadata_dict
         metadata_dict["min_score"] = 0
         metadata_dict["max_score"] = 5
         return metadata_dict
```

### Comparing `mteb-1.4.1/mteb/tasks/STS/en/STS16STS.py` & `mteb-1.5.0/mteb/tasks/Summarization/fr/SummEvalFrSummarization.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 from __future__ import annotations
 
+from mteb.abstasks import AbsTaskSummarization
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks.AbsTaskSTS import AbsTaskSTS
 
-
-class STS16STS(AbsTaskSTS):
+class SummEvalFrSummarization(AbsTaskSummarization):
     metadata = TaskMetadata(
-        name="STS16",
-        hf_hub_name="mteb/sts16-sts",
-        description="SemEval STS 2016 dataset",
-        reference="https://www.aclweb.org/anthology/S16-1001",
-        type="STS",
-        category="s2s",
+        name="SummEvalFr",
+        description="News Article Summary Semantic Similarity Estimation translated from english to french with DeepL.",
+        reference="https://github.com/Yale-LILY/SummEval",
+        dataset={
+            "path": "lyon-nlp/summeval",
+            "revision": "b385812de6a9577b6f4d0f88c6a6e35395a94054",
+        },
+        type="Summarization",
+        category="p2p",
         eval_splits=["test"],
-        eval_langs=["en"],
+        eval_langs=["fr"],
         main_score="cosine_spearman",
-        revision="4d8694f8f0e0100860b497b999b3dbed754a0513",
         date=None,
-        form=None,
+        form=["written"],
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
-        text_creation=None,
+        text_creation="machine-translated",
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
+        metadata_dict = super().metadata_dict
         metadata_dict["min_score"] = 0
         metadata_dict["max_score"] = 5
+
         return metadata_dict
```

### Comparing `mteb-1.4.1/mteb/tasks/STS/en/STSBenchmarkSTS.py` & `mteb-1.5.0/mteb/tasks/Classification/en/ImdbClassification.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,34 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks.AbsTaskSTS import AbsTaskSTS
+from ....abstasks import AbsTaskClassification
 
 
-class STSBenchmarkSTS(AbsTaskSTS):
+class ImdbClassification(AbsTaskClassification):
     metadata = TaskMetadata(
-        name="STSBenchmark",
-        hf_hub_name="mteb/stsbenchmark-sts",
-        description="Semantic Textual Similarity Benchmark (STSbenchmark) dataset.",
-        reference="https://github.com/PhilipMay/stsb-multi-mt/",
-        type="STS",
-        category="s2s",
+        name="ImdbClassification",
+        description="Large Movie Review Dataset",
+        dataset={
+            "path": "mteb/imdb",
+            "revision": "3d86128a09e091d6018b6d26cad27f2739fc2db7",
+        },
+        reference="http://www.aclweb.org/anthology/P11-1015",
+        type="Classification",
+        category="p2p",
         eval_splits=["test"],
         eval_langs=["en"],
-        main_score="cosine_spearman",
-        revision="b0fddb56ed78048fa8b90373c8a3cfc37b684831",
+        main_score="accuracy",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples=None,
-        avg_character_length=None,
+        n_samples={"test": 25000},
+        avg_character_length={"test": 1293.8},
     )
-
-    @property
-    def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
-        metadata_dict["min_score"] = 0
-        metadata_dict["max_score"] = 5
-        return metadata_dict
```

### Comparing `mteb-1.4.1/mteb/tasks/STS/en/SickrSTS.py` & `mteb-1.5.0/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 from __future__ import annotations
 
+from mteb.abstasks import AbsTaskBitextMining
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks.AbsTaskSTS import AbsTaskSTS
 
-
-class SickrSTS(AbsTaskSTS):
+class NorwegianCourtsBitextMining(AbsTaskBitextMining):
     metadata = TaskMetadata(
-        name="SICK-R",
-        hf_hub_name="MMathematica/sickr-sts",
-        description="Semantic Textual Similarity SICK-R dataset as described here:",
-        reference="https://aclanthology.org/2020.lrec-1.207",
-        type="STS",
+        name="NorwegianCourtsBitextMining",
+        dataset={
+            "path": "kardosdrur/norwegian-courts",
+            "revision": "d79af07e969a6678fcbbe819956840425816468f",
+        },
+        description="Nynorsk and Bokmål parallel corpus from Norwegian courts. Norwegian courts have two standardised written languages. Bokmål is a variant closer to Danish, while Nynorsk was created to resemble regional dialects of Norwegian.",
+        reference="https://opus.nlpl.eu/index.php",
+        type="BitextMining",
         category="s2s",
         eval_splits=["test"],
-        eval_langs=["en"],
-        main_score="cosine_spearman",
-        revision="a6ea5a8cab320b040a23452cc28066d9beae2cee",
+        eval_langs=["nb", "nn"],
+        main_score="f1",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples=None,
-        avg_character_length=None,
+        n_samples={"test": 2050},
+        avg_character_length={"test": 1884.0},
     )
 
-    @property
-    def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
-        metadata_dict["min_score"] = 0
-        metadata_dict["max_score"] = 5
-        return metadata_dict
+    def dataset_transform(self):
+        # Convert to standard format
+        self.dataset = self.dataset.rename_column("nb", "sentence1")
+        self.dataset = self.dataset.rename_column("nn", "sentence2")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mteb-1.4.1/mteb/tasks/STS/es/STSES.py` & `mteb-1.5.0/mteb/tasks/Summarization/en/SummEvalSummarization.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,58 +1,41 @@
 from __future__ import annotations
 
-from datasets import load_dataset
-
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks.AbsTaskSTS import AbsTaskSTS
-
-_EVAL_SPLIT = "test"
+from ....abstasks import AbsTaskSummarization
 
 
-class STSES(AbsTaskSTS):
+class SummEvalSummarization(AbsTaskSummarization):
     metadata = TaskMetadata(
-        name="STSES",
-        hf_hub_name="PlanTL-GOB-ES/sts-es",
-        description="Spanish test sets from SemEval-2014 (Agirre et al., 2014) and SemEval-2015 (Agirre et al., 2015)",
-        reference="https://huggingface.co/datasets/PlanTL-GOB-ES/sts-es",
-        type="STS",
-        category="s2s",
-        eval_splits=[_EVAL_SPLIT],
-        eval_langs=["es"],
+        name="SummEval",
+        description="News Article Summary Semantic Similarity Estimation.",
+        reference="https://tabilab.cmpe.boun.edu.tr/BIOSSES/DataSet.html",
+        dataset={
+            "path": "mteb/summeval",
+            "revision": "cda12ad7615edc362dbf25a00fdd61d3b1eaf93c",
+        },
+        type="Summarization",
+        category="p2p",
+        eval_splits=["test"],
+        eval_langs=["en"],
         main_score="cosine_spearman",
-        revision="0912bb6c9393c76d62a7c5ee81c4c817ff47c9f4",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples=None,
-        avg_character_length=None,
+        n_samples={"test": 2800},
+        avg_character_length={"test": 359.8},
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
+        metadata_dict = super().metadata_dict
         metadata_dict["min_score"] = 0
         metadata_dict["max_score"] = 5
-
-        return dict(self.metadata)
-
-    def load_data(self, **kwargs):
-        if self.data_loaded:
-            return
-
-        data = load_dataset(
-            self.metadata_dict["hf_hub_name"],
-            trust_remote_code=True,
-            revision=self.metadata_dict.get("revision", None),
-        )[_EVAL_SPLIT]
-        data = data.add_column("score", [d["label"] for d in data])
-        self.dataset = {_EVAL_SPLIT: data}
-
-        self.data_loaded = True
+        return metadata_dict
```

### Comparing `mteb-1.4.1/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py` & `mteb-1.5.0/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,23 +18,25 @@
     "nl-en",
 ]
 
 
 class STS17Crosslingual(AbsTaskSTS, CrosslingualTask):
     metadata = TaskMetadata(
         name="STS17",
-        hf_hub_name="mteb/sts17-crosslingual-sts",
+        dataset={
+            "path": "mteb/sts17-crosslingual-sts",
+            "revision": "af5e6fb845001ecf41f4c1e033ce921939a2a68d",
+        },
         description="STS 2017 dataset",
         reference="http://alt.qcri.org/semeval2016/task1/",
         type="STS",
         category="s2s",
         eval_splits=["test"],
         eval_langs=_LANGUAGES,
         main_score="cosine_spearman",
-        revision="af5e6fb845001ecf41f4c1e033ce921939a2a68d",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -43,11 +45,11 @@
         bibtex_citation=None,
         n_samples={"test": 500},
         avg_character_length={"test": 43.3},
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
+        metadata_dict = super().metadata_dict
         metadata_dict["min_score"] = 0
         metadata_dict["max_score"] = 5
         return metadata_dict
```

### Comparing `mteb-1.4.1/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py` & `mteb-1.5.0/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,23 +25,25 @@
     "fr-pl",
 ]
 
 
 class STS22CrosslingualSTS(AbsTaskSTS, CrosslingualTask):
     metadata = TaskMetadata(
         name="STS22",
-        hf_hub_name="mteb/sts22-crosslingual-sts",
+        dataset={
+            "path": "mteb/sts22-crosslingual-sts",
+            "revision": "eea2b4fe26a775864c896887d910b76a8098ad3f",
+        },
         description="SemEval 2022 Task 8: Multilingual News Article Similarity",
         reference="https://competitions.codalab.org/competitions/33835",
         type="STS",
         category="p2p",
         eval_splits=["test"],
         eval_langs=_LANGUAGES,
         main_score="cosine_spearman",
-        revision="eea2b4fe26a775864c896887d910b76a8098ad3f",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -50,11 +52,11 @@
         bibtex_citation=None,
         n_samples={"test": 8060},
         avg_character_length={"train": 1992.8},
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
+        metadata_dict = super().metadata_dict
         metadata_dict["min_score"] = 1
         metadata_dict["max_score"] = 4
         return metadata_dict
```

### Comparing `mteb-1.4.1/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py` & `mteb-1.5.0/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,26 +9,28 @@
 _LANGUAGES = ["en", "de", "es", "fr", "it", "nl", "pl", "pt", "ru", "zh"]
 _SPLITS = ["dev", "test"]
 
 
 class STSBenchmarkMultilingualSTS(AbsTaskSTS, MultilingualTask):
     metadata = TaskMetadata(
         name="STSBenchmarkMultilingualSTS",
-        hf_hub_name="stsb_multi_mt",
+        dataset={
+            "path": "stsb_multi_mt",
+            "revision": "93d57ef91790589e3ce9c365164337a8a78b7632",
+        },
         description=(
             "Semantic Textual Similarity Benchmark (STSbenchmark) dataset,"
             "but translated using DeepL API."
         ),
         reference="https://github.com/PhilipMay/stsb-multi-mt/",
         type="STS",
         category="s2s",
         eval_splits=_SPLITS,
         eval_langs=_LANGUAGES,
         main_score="cosine_spearman",
-        revision="93d57ef91790589e3ce9c365164337a8a78b7632",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -37,15 +39,15 @@
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
+        metadata_dict = super().metadata_dict
         metadata_dict["min_score"] = 0
         metadata_dict["max_score"] = 5
         return metadata_dict
 
     def load_data(self, **kwargs):
         if self.data_loaded:
             return
@@ -62,18 +64,17 @@
                 datasets.DatasetDict: the dataset of the specified language
             """
             subset = datasets.DatasetDict(
                 **dict(
                     zip(
                         _SPLITS,
                         datasets.load_dataset(
-                            self.metadata_dict["hf_hub_name"],
-                            lang,
+                            name=lang,
                             split=_SPLITS,
-                            revision=self.metadata_dict.get("revision", None),
+                            **self.metadata_dict["dataset"],
                         ),
                     )
                 )
             )
             return subset.rename_column("similarity_score", "score")
 
         self.dataset = datasets.DatasetDict(
```

### Comparing `mteb-1.4.1/mteb/tasks/STS/zh/CMTEBSTS.py` & `mteb-1.5.0/mteb/tasks/STS/zh/CMTEBSTS.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 
 from ....abstasks.AbsTaskSTS import AbsTaskSTS
 
 
 class ATEC(AbsTaskSTS):
     metadata = TaskMetadata(
         name="ATEC",
-        hf_hub_name="C-MTEB/ATEC",
+        dataset={
+            "path": "C-MTEB/ATEC",
+            "revision": "0f319b1142f2ae3f7dc7be10c3c7f3598ec6c602",
+        },
         description="A Chinese dataset for textual relatedness",
         reference="https://aclanthology.org/2021.emnlp-main.357",
         type="STS",
         category="s2s",
         eval_splits=["validation", "test"],
         eval_langs=["zh"],
         main_score="cosine_spearman",
-        revision="0f319b1142f2ae3f7dc7be10c3c7f3598ec6c602",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -29,32 +31,34 @@
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
+        metadata_dict = super().metadata_dict
         metadata_dict["min_score"] = 0
         metadata_dict["max_score"] = 1
         return metadata_dict
 
 
 class BQ(AbsTaskSTS):
     metadata = TaskMetadata(
         name="BQ",
-        hf_hub_name="C-MTEB/BQ",
+        dataset={
+            "path": "C-MTEB/BQ",
+            "revision": "e3dda5e115e487b39ec7e618c0c6a29137052a55",
+        },
         description="A Chinese dataset for textual relatedness",
         reference="https://aclanthology.org/2021.emnlp-main.357",
         type="STS",
         category="s2s",
         eval_splits=["validation", "test"],
         eval_langs=["zh"],
         main_score="cosine_spearman",
-        revision="e3dda5e115e487b39ec7e618c0c6a29137052a55",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -63,32 +67,34 @@
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
+        metadata_dict = super().metadata_dict
         metadata_dict["min_score"] = 0
         metadata_dict["max_score"] = 1
         return metadata_dict
 
 
 class LCQMC(AbsTaskSTS):
     metadata = TaskMetadata(
         name="LCQMC",
-        hf_hub_name="C-MTEB/LCQMC",
+        dataset={
+            "path": "C-MTEB/LCQMC",
+            "revision": "17f9b096f80380fce5ed12a9be8be7784b337daf",
+        },
         description="A Chinese dataset for textual relatedness",
         reference="https://aclanthology.org/2021.emnlp-main.357",
         type="STS",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["zh"],
         main_score="cosine_spearman",
-        revision="17f9b096f80380fce5ed12a9be8be7784b337daf",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -97,32 +103,34 @@
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
+        metadata_dict = super().metadata_dict
         metadata_dict["min_score"] = 0
         metadata_dict["max_score"] = 1
         return metadata_dict
 
 
 class PAWSX(AbsTaskSTS):
     metadata = TaskMetadata(
         name="PAWSX",
-        hf_hub_name="C-MTEB/PAWSX",
+        dataset={
+            "path": "C-MTEB/PAWSX",
+            "revision": "9c6a90e430ac22b5779fb019a23e820b11a8b5e1",
+        },
         description="A Chinese dataset for textual relatedness",
         reference="https://aclanthology.org/2021.emnlp-main.357",
         type="STS",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["zh"],
         main_score="cosine_spearman",
-        revision="9c6a90e430ac22b5779fb019a23e820b11a8b5e1",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -131,32 +139,34 @@
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
+        metadata_dict = super().metadata_dict
         metadata_dict["min_score"] = 0
         metadata_dict["max_score"] = 1
         return metadata_dict
 
 
 class STSB(AbsTaskSTS):
     metadata = TaskMetadata(
         name="STSB",
-        hf_hub_name="C-MTEB/STSB",
+        dataset={
+            "path": "C-MTEB/STSB",
+            "revision": "0cde68302b3541bb8b3c340dc0644b0b745b3dc0",
+        },
         description="A Chinese dataset for textual relatedness",
         reference="https://aclanthology.org/2021.emnlp-main.357",
         type="STS",
         category="s2s",
         eval_splits=["validation", "test"],
         eval_langs=["zh"],
         main_score="cosine_spearman",
-        revision="0cde68302b3541bb8b3c340dc0644b0b745b3dc0",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -165,32 +175,34 @@
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
+        metadata_dict = super().metadata_dict
         metadata_dict["min_score"] = 0
         metadata_dict["max_score"] = 5
         return metadata_dict
 
 
 class AFQMC(AbsTaskSTS):
     metadata = TaskMetadata(
         name="AFQMC",
-        hf_hub_name="C-MTEB/AFQMC",
+        dataset={
+            "path": "C-MTEB/AFQMC",
+            "revision": "b44c3b011063adb25877c13823db83bb193913c4",
+        },
         description="A Chinese dataset for textual relatedness",
         reference="https://aclanthology.org/2021.emnlp-main.357",
         type="STS",
         category="s2s",
         eval_splits=["validation", "test"],
         eval_langs=["zh"],
         main_score="cosine_spearman",
-        revision="b44c3b011063adb25877c13823db83bb193913c4",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
@@ -199,32 +211,34 @@
         bibtex_citation=None,
         n_samples=None,
         avg_character_length=None,
     )
 
     @property
     def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
+        metadata_dict = super().metadata_dict
         metadata_dict["min_score"] = 0
         metadata_dict["max_score"] = 1
         return metadata_dict
 
 
 class QBQTC(AbsTaskSTS):
     metadata = TaskMetadata(
         name="QBQTC",
-        hf_hub_name="C-MTEB/QBQTC",
+        dataset={
+            "path": "C-MTEB/QBQTC",
+            "revision": "790b0510dc52b1553e8c49f3d2afb48c0e5c48b7",
+        },
         description="",
         reference="https://github.com/CLUEbenchmark/QBQTC/tree/main/dataset",
         type="STS",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["zh"],
         main_score="cosine_spearman",
-        revision="790b0510dc52b1553e8c49f3d2afb48c0e5c48b7",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
```

### Comparing `mteb-1.4.1/mteb/tasks/Summarization/en/SummEvalSummarization.py` & `mteb-1.5.0/mteb/tasks/Retrieval/en/HotpotQARetrieval.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 from __future__ import annotations
 
 from mteb.abstasks.TaskMetadata import TaskMetadata
 
-from ....abstasks import AbsTaskSummarization
+from ....abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 
-class SummEvalSummarization(AbsTaskSummarization):
+class HotpotQA(AbsTaskRetrieval):
     metadata = TaskMetadata(
-        name="SummEval",
-        description="News Article Summary Semantic Similarity Estimation.",
-        reference="https://tabilab.cmpe.boun.edu.tr/BIOSSES/DataSet.html",
-        hf_hub_name="mteb/summeval",
-        type="Summarization",
-        category="p2p",
-        eval_splits=["test"],
+        name="HotpotQA",
+        dataset={
+            "path": "mteb/hotpotqa",
+            "revision": "ab518f4d6fcca38d87c25209f94beba119d02014",
+        },
+        description=(
+            "HotpotQA is a question answering dataset featuring natural, multi-hop questions, with strong"
+            " supervision for supporting facts to enable more explainable question answering systems."
+        ),
+        reference="https://hotpotqa.github.io/",
+        type="Retrieval",
+        category="s2p",
+        eval_splits=["train", "dev", "test"],
         eval_langs=["en"],
-        main_score="cosine_spearman",
-        revision="cda12ad7615edc362dbf25a00fdd61d3b1eaf93c",
+        main_score="ndcg_at_10",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
         socioeconomic_status=None,
         annotations_creators=None,
         dialect=None,
         text_creation=None,
         bibtex_citation=None,
-        n_samples={"test": 2800},
-        avg_character_length={"test": 359.8},
+        n_samples=None,
+        avg_character_length=None,
     )
-
-    @property
-    def metadata_dict(self) -> dict[str, str]:
-        metadata_dict = dict(self.metadata)
-        metadata_dict["min_score"] = 0
-        metadata_dict["max_score"] = 5
-        return metadata_dict
```

### Comparing `mteb-1.4.1/mteb.egg-info/PKG-INFO` & `mteb-1.5.0/mteb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mteb
-Version: 1.4.1
+Version: 1.5.0
 Summary: Massive Text Embedding Benchmark
 Author-email: MTEB Contributors <niklas@huggingface.co>, nouamane@huggingface.co, info@nils-reimers.de
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `mteb-1.4.1/mteb.egg-info/SOURCES.txt` & `mteb-1.5.0/mteb.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -281,8 +281,9 @@
 scripts/data/sts22-crosslingual-sts/create_data.py
 scripts/data/summeval_fr/create_data.py
 scripts/data/toxic_conversations_50k/create_data.py
 tests/test_ClusteringEvaluator.py
 tests/test_PairClassificationEvaluator.py
 tests/test_RerankingEvaluator.py
 tests/test_RetrievalEvaluator.py
+tests/test_TaskMetadata.py
 tests/test_all_abstasks.py
```

### Comparing `mteb-1.4.1/pyproject.toml` & `mteb-1.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mteb"
-version = "1.4.1"
+version = "1.5.0"
 description = "Massive Text Embedding Benchmark"
 readme = "README.md"
 authors = [
     { name = "MTEB Contributors", email = "niklas@huggingface.co" },
     { email = "nouamane@huggingface.co" },
     { email = "info@nils-reimers.de" },
 ]
```

### Comparing `mteb-1.4.1/scripts/data/amazon_polarity/create_data.py` & `mteb-1.5.0/scripts/data/amazon_polarity/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/scripts/data/amazon_reviews_multi/create_data.py` & `mteb-1.5.0/scripts/data/amazon_reviews_multi/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/scripts/data/arxiv/script_clustering.py` & `mteb-1.5.0/scripts/data/arxiv/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/scripts/data/arxiv/script_raw.py` & `mteb-1.5.0/scripts/data/arxiv/script_raw.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/scripts/data/biorxiv/script_clustering.py` & `mteb-1.5.0/scripts/data/biorxiv/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/scripts/data/biorxiv/script_raw.py` & `mteb-1.5.0/scripts/data/biorxiv/script_raw.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/scripts/data/bucc/create_data.py` & `mteb-1.5.0/scripts/data/bucc/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/scripts/data/create_task_table.py` & `mteb-1.5.0/scripts/data/create_task_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,16 +134,16 @@
         avg_lens["test"],
     )
 
 
 # Select all tasks
 for task in MTEB().tasks:
     print("Task: ", task)
-    if "hf_hub_name" in task.metadata_dict:
-        hub_name = hub_url = task.metadata_dict.get("hf_hub_name")
+    if "dataset" in task.metadata_dict:
+        hub_name = hub_url = task.metadata_dict["dataset"]["path"]
         ds_stats = get_ds_stats(hub_name.split("/")[-1])
     elif "beir_name" in task.metadata_dict:
         hub_name = hub_url = "BeIR/" + task.metadata_dict.get("beir_name")
         ds_stats = get_ds_stats_beir("/".join(hub_name.split("/")[1:]))
         if "cqadupstack" in hub_name:
             hub_url = "BeIR/cqadupstack-qrels"
     TABLE_STRING += "\n" + ONE_LINE.format(
```

### Comparing `mteb-1.4.1/scripts/data/germanquad/process_data.py` & `mteb-1.5.0/scripts/data/germanquad/process_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/scripts/data/hal/create_data.py` & `mteb-1.5.0/scripts/data/hal/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/scripts/data/imdb/create_data.py` & `mteb-1.5.0/scripts/data/imdb/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/scripts/data/medrxiv/script_clustering.py` & `mteb-1.5.0/scripts/data/medrxiv/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/scripts/data/medrxiv/script_raw.py` & `mteb-1.5.0/scripts/data/medrxiv/script_raw.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/scripts/data/mind/prepare_data.py` & `mteb-1.5.0/scripts/data/mind/prepare_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/scripts/data/redditp2p/script_clustering.py` & `mteb-1.5.0/scripts/data/redditp2p/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/scripts/data/stackexchangep2p/script_clustering.py` & `mteb-1.5.0/scripts/data/stackexchangep2p/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/scripts/data/sts22-crosslingual-sts/create_data.py` & `mteb-1.5.0/scripts/data/sts22-crosslingual-sts/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/scripts/data/summeval_fr/create_data.py` & `mteb-1.5.0/scripts/data/summeval_fr/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/scripts/data/toxic_conversations_50k/create_data.py` & `mteb-1.5.0/scripts/data/toxic_conversations_50k/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/scripts/merge_cqadupstack.py` & `mteb-1.5.0/scripts/merge_cqadupstack.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/scripts/mteb_meta.py` & `mteb-1.5.0/scripts/mteb_meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,19 @@
             tasks=[
                 ds_name.replace("CQADupstackRetrieval", "CQADupstackAndroidRetrieval")
             ]
         )
         .tasks[0]
         .metadata_dict
     )
-    hf_hub_name = mteb_desc.get("hf_hub_name", mteb_desc.get("beir_name"))
+    hf_hub_name = (
+        mteb_desc["dataset"]["path"]
+        if "dataset" in mteb_desc
+        else mteb_desc.get("beir_name")
+    )
     if "beir_name" in mteb_desc:
         logger.warning(
             "`beir_name` is deprecated and will be removed in the future. New result files contain `hf_hub_name` instead."
         )
     if ds_name == "CQADupstackRetrieval" in ds_name:
         hf_hub_name = "mteb/cqadupstack"
     mteb_type = mteb_desc["type"]
```

### Comparing `mteb-1.4.1/scripts/run_mteb_chinese.py` & `mteb-1.5.0/scripts/run_mteb_chinese.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/scripts/run_mteb_english.py` & `mteb-1.5.0/scripts/run_mteb_english.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/scripts/run_mteb_french.py` & `mteb-1.5.0/scripts/run_mteb_french.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/scripts/run_mteb_german.py` & `mteb-1.5.0/scripts/run_mteb_german.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/scripts/run_mteb_korean.py` & `mteb-1.5.0/scripts/run_mteb_korean.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/scripts/run_mteb_polish.py` & `mteb-1.5.0/scripts/run_mteb_polish.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/tests/test_ClusteringEvaluator.py` & `mteb-1.5.0/tests/test_ClusteringEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/tests/test_PairClassificationEvaluator.py` & `mteb-1.5.0/tests/test_PairClassificationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/tests/test_RerankingEvaluator.py` & `mteb-1.5.0/tests/test_RerankingEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/tests/test_RetrievalEvaluator.py` & `mteb-1.5.0/tests/test_RetrievalEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.4.1/tests/test_all_abstasks.py` & `mteb-1.5.0/tests/test_all_abstasks.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,17 +5,32 @@
 
 import pytest
 from sentence_transformers import SentenceTransformer
 
 from mteb import MTEB
 from mteb.abstasks import AbsTask
 from mteb.tasks.BitextMining.da.BornholmskBitextMining import BornholmBitextMining
+from unittest.mock import patch, Mock
+from mteb.abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 
 logging.basicConfig(level=logging.INFO)
 
+@pytest.mark.parametrize("task", MTEB().tasks_cls)
+@patch("datasets.load_dataset")
+def test_load_data(mock_load_dataset: Mock, task: AbsTask):
+    # TODO: We skip because this load_data is completely different.
+    if isinstance(task, AbsTaskRetrieval):
+        pytest.skip()
+    with patch.object(task, "dataset_transform") as mock_dataset_transform:
+        task.load_data()
+        mock_load_dataset.assert_called()
+
+        # They don't yet but should they so they can be expanded more easily?
+        if not task.is_crosslingual and not task.is_multilingual:
+            mock_dataset_transform.assert_called_once()
 
 def test_two_mteb_tasks():
     """
     Test that two tasks can be fetched and run
     """
     model = SentenceTransformer("average_word_embeddings_komninos")
     eval = MTEB(
```

